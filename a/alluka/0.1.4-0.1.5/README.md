# Comparing `tmp/alluka-0.1.4.tar.gz` & `tmp/alluka-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alluka-0.1.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "alluka-0.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `alluka-0.1.4.tar` & `alluka-0.1.5.tar`

### file list

```diff
@@ -1,131 +1,133 @@
--rw-r--r--   0        0        0      320 2023-12-27 22:16:34.445702 alluka-0.1.4/.codeclimate.yml
--rw-r--r--   0        0        0       14 2023-12-27 22:16:34.445702 alluka-0.1.4/.gitattributes
--rw-r--r--   0        0        0       26 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      459 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/dependabot.yml
--rw-r--r--   0        0        0      524 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/pull_request_template.md
--rw-r--r--   0        0        0     1144 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0     1034 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1516 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/pr-docs.yml
--rw-r--r--   0        0        0      872 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2343 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/py-test.yml
--rw-r--r--   0        0        0      980 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1263 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/release-docs.yml
--rw-r--r--   0        0        0     1039 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      836 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1186 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1221 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1060 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0      854 2023-12-27 22:16:34.445702 alluka-0.1.4/.github/workflows/verify-types.yml
--rw-r--r--   0        0        0     1748 2023-12-27 22:16:34.445702 alluka-0.1.4/.gitignore
--rw-r--r--   0        0        0       85 2023-12-27 22:16:34.445702 alluka-0.1.4/.gitmodules
--rw-r--r--   0        0        0     3233 2023-12-27 22:16:34.445702 alluka-0.1.4/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2023-12-27 22:16:34.445702 alluka-0.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     6399 2023-12-27 22:16:34.445702 alluka-0.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0     1520 2023-12-27 22:16:34.449702 alluka-0.1.4/LICENSE
--rw-r--r--   0        0        0      607 2023-12-27 22:16:34.449702 alluka-0.1.4/README.md
--rw-r--r--   0        0        0     2376 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/__init__.py
--rw-r--r--   0        0        0    14935 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_client.py
--rw-r--r--   0        0        0     2531 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_errors.py
--rw-r--r--   0        0        0     6275 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_self_injecting.py
--rw-r--r--   0        0        0     9396 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_types.py
--rw-r--r--   0        0        0      167 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_vendor/__init__.py
--rw-r--r--   0        0        0   123930 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_vendor/inspect.py
--rw-r--r--   0        0        0    13931 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_vendor/inspect.py.LICENSE
--rw-r--r--   0        0        0    12305 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_vendor/inspect.pyi
--rw-r--r--   0        0        0    12657 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_vendor/inspect.pyi.LICENSE
--rw-r--r--   0        0        0     9344 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/_visitor.py
--rw-r--r--   0        0        0    21073 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/abc.py
--rw-r--r--   0        0        0        0 2023-12-27 22:16:34.449702 alluka-0.1.4/alluka/py.typed
--rw-r--r--   0        0        0       56 2023-12-27 22:16:34.449702 alluka-0.1.4/dev-requirements/flake8.txt
--rw-r--r--   0        0        0      251 2023-12-27 22:16:34.449702 alluka-0.1.4/dev-requirements/tests.in
--rw-r--r--   0        0        0    15058 2023-12-27 22:16:34.449702 alluka-0.1.4/dev-requirements/tests.txt
--rw-r--r--   0        0        0      112 2023-12-27 22:16:34.449702 alluka-0.1.4/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    35102 2023-12-27 22:16:34.449702 alluka-0.1.4/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0       17 2023-12-27 22:16:34.449702 alluka-0.1.4/docs/changelog.md
--rw-r--r--   0        0        0       14 2023-12-27 22:16:34.449702 alluka-0.1.4/docs/index.md
--rw-r--r--   0        0        0       29 2023-12-27 22:16:34.449702 alluka-0.1.4/docs/reference/abc.md
--rw-r--r--   0        0        0       21 2023-12-27 22:16:34.449702 alluka-0.1.4/docs/reference/index.md
--rw-r--r--   0        0        0     5220 2023-12-27 22:16:34.449702 alluka-0.1.4/docs/usage.md
--rw-r--r--   0        0        0     1593 2023-12-27 22:16:34.449702 alluka-0.1.4/mkdocs.yml
--rw-r--r--   0        0        0     1714 2023-12-27 22:16:34.449702 alluka-0.1.4/noxfile.py
--rw-r--r--   0        0        0       14 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.gitattributes
--rw-r--r--   0        0        0      458 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/dependabot.yml
--rw-r--r--   0        0        0     1240 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/freeze-for-pr.yml
--rw-r--r--   0        0        0      959 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/lint.yml
--rw-r--r--   0        0        0      976 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/reformat.yml
--rw-r--r--   0        0        0     1032 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/resync-piped.yml
--rw-r--r--   0        0        0      832 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/type-check.yml
--rw-r--r--   0        0        0     1182 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/update-licence.yml
--rw-r--r--   0        0        0     1217 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/upgrade-locks.yml
--rw-r--r--   0        0        0     1114 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.github/workflows/verify-locks.yml
--rw-r--r--   0        0        0     1751 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/.gitignore
--rw-r--r--   0        0        0     1520 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/LICENSE
--rw-r--r--   0        0        0      138 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/README.md
--rw-r--r--   0        0        0       50 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/.env.example
--rw-r--r--   0        0        0      612 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/Dockerfile
--rw-r--r--   0        0        0    30882 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/main.py
--rw-r--r--   0        0        0       10 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/requirements-extra.txt
--rw-r--r--   0        0        0      196 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/requirements.in
--rw-r--r--   0        0        0    24624 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/bot/requirements.txt
--rw-r--r--   0        0        0      933 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/dev-requirements/flake8.in
--rw-r--r--   0        0        0    21215 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/dev-requirements/flake8.txt
--rw-r--r--   0        0        0       10 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/dev-requirements/type-checking-extra.txt
--rw-r--r--   0        0        0      112 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/dev-requirements/type-checking.in
--rw-r--r--   0        0        0    35337 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/dev-requirements/type-checking.txt
--rw-r--r--   0        0        0      250 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/docker-compose.yml
--rw-r--r--   0        0        0       26 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/CODEOWNERS
--rw-r--r--   0        0        0       45 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/FUNDING.yml
--rw-r--r--   0        0        0      764 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/clippy.yml
--rw-r--r--   0        0        0     1133 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/freeze-for-pr.yml
--rw-r--r--   0        0        0     1271 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/lint.yml
--rw-r--r--   0        0        0     1577 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/pr-docs.yml
--rw-r--r--   0        0        0      964 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/publish.yml
--rw-r--r--   0        0        0     2399 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/py-test.yml
--rw-r--r--   0        0        0     1013 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/reformat.yml
--rw-r--r--   0        0        0     1373 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/release-docs.yml
--rw-r--r--   0        0        0     1075 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/resync-piped.yml
--rw-r--r--   0        0        0     1223 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/rustfmt.yml
--rw-r--r--   0        0        0      869 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/type-check.yml
--rw-r--r--   0        0        0     1191 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/update-licence.yml
--rw-r--r--   0        0        0     1226 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/upgrade-locks.yml
--rw-r--r--   0        0        0     1130 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/verify-locks.yml
--rw-r--r--   0        0        0      887 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/actions/verify-types.yml
--rw-r--r--   0        0        0      550 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/dependabot.yml
--rw-r--r--   0        0        0      524 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/github/pull_request_template.md
--rw-r--r--   0        0        0     1713 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/noxfile.py
--rw-r--r--   0        0        0     4853 2023-12-27 22:16:34.785700 alluka-0.1.4/piped/pyproject.toml
--rw-r--r--   0        0        0      115 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/docs.in
--rw-r--r--   0        0        0    36158 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/docs.txt
--rw-r--r--   0        0        0       90 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/flake8.in
--rw-r--r--   0        0        0     1665 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/flake8.txt
--rw-r--r--   0        0        0      223 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/freeze-locks.in
--rw-r--r--   0        0        0    52149 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/freeze-locks.txt
--rw-r--r--   0        0        0     1068 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/library-flake8.in
--rw-r--r--   0        0        0    32045 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/library-flake8.txt
--rw-r--r--   0        0        0       58 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/lint.in
--rw-r--r--   0        0        0     6308 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/lint.txt
--rw-r--r--   0        0        0       60 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/nox.in
--rw-r--r--   0        0        0    17785 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/nox.txt
--rw-r--r--   0        0        0       12 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/publish.in
--rw-r--r--   0        0        0     9863 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/publish.txt
--rw-r--r--   0        0        0       78 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/reformat.in
--rw-r--r--   0        0        0    17673 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/reformat.txt
--rw-r--r--   0        0        0       64 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/tests.in
--rw-r--r--   0        0        0     7400 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/tests.txt
--rw-r--r--   0        0        0       29 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/type-checking.in
--rw-r--r--   0        0        0     4050 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/base-requirements/type-checking.txt
--rw-r--r--   0        0        0    24224 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/noxfile.py
--rw-r--r--   0        0        0     1714 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/noxfile.template.py
--rw-r--r--   0        0        0     4527 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/piped_shared/__init__.py
--rw-r--r--   0        0        0        0 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/piped_shared/py.typed
--rw-r--r--   0        0        0      334 2023-12-27 22:16:34.789700 alluka-0.1.4/piped/python/pyproject.toml
--rw-r--r--   0        0        0     6716 2023-12-27 22:16:34.449702 alluka-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1596 2023-12-27 22:16:34.449702 alluka-0.1.4/tests/__init__.py
--rw-r--r--   0        0        0    13533 2023-12-27 22:16:34.449702 alluka-0.1.4/tests/test__client.py
--rw-r--r--   0        0        0     2883 2023-12-27 22:16:34.449702 alluka-0.1.4/tests/test__self_injecting.py
--rw-r--r--   0        0        0    50885 2023-12-27 22:16:34.449702 alluka-0.1.4/tests/test_async_callback_di.py
--rw-r--r--   0        0        0    52170 2023-12-27 22:16:34.453702 alluka-0.1.4/tests/test_async_callback_di_future_annotations.py
--rw-r--r--   0        0        0    45842 2023-12-27 22:16:34.453702 alluka-0.1.4/tests/test_callback_di.py
--rw-r--r--   0        0        0    46226 2023-12-27 22:16:34.453702 alluka-0.1.4/tests/test_callback_di_future_annotations.py
--rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 alluka-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      320 2024-04-22 22:53:50.525395 alluka-0.1.5/.codeclimate.yml
+-rw-r--r--   0        0        0       14 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitattributes
+-rw-r--r--   0        0        0       26 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      459 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/dependabot.yml
+-rw-r--r--   0        0        0      524 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1144 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1034 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1516 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/pr-docs.yml
+-rw-r--r--   0        0        0     1002 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     2343 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/py-test.yml
+-rw-r--r--   0        0        0      980 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1263 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/release-docs.yml
+-rw-r--r--   0        0        0     1039 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      836 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1186 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1221 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1060 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0      854 2024-04-22 22:53:50.525395 alluka-0.1.5/.github/workflows/verify-types.yml
+-rw-r--r--   0        0        0     1748 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitignore
+-rw-r--r--   0        0        0       85 2024-04-22 22:53:50.525395 alluka-0.1.5/.gitmodules
+-rw-r--r--   0        0        0     3409 2024-04-22 22:53:50.525395 alluka-0.1.5/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2024-04-22 22:53:50.525395 alluka-0.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     6399 2024-04-22 22:53:50.525395 alluka-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1520 2024-04-22 22:53:50.525395 alluka-0.1.5/LICENSE
+-rw-r--r--   0        0        0      607 2024-04-22 22:53:50.525395 alluka-0.1.5/README.md
+-rw-r--r--   0        0        0     2376 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/__init__.py
+-rw-r--r--   0        0        0    14896 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_client.py
+-rw-r--r--   0        0        0     2531 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_errors.py
+-rw-r--r--   0        0        0     6261 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_self_injecting.py
+-rw-r--r--   0        0        0     9605 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_types.py
+-rw-r--r--   0        0        0      167 2024-04-22 22:53:50.525395 alluka-0.1.5/alluka/_vendor/__init__.py
+-rw-r--r--   0        0        0   123930 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.py
+-rw-r--r--   0        0        0    13931 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.py.LICENSE
+-rw-r--r--   0        0        0    12305 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.pyi
+-rw-r--r--   0        0        0    12657 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_vendor/inspect.pyi.LICENSE
+-rw-r--r--   0        0        0     9336 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/_visitor.py
+-rw-r--r--   0        0        0    20961 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/abc.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:53:50.529395 alluka-0.1.5/alluka/py.typed
+-rw-r--r--   0        0        0       56 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0      251 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/tests.in
+-rw-r--r--   0        0        0    15059 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/tests.txt
+-rw-r--r--   0        0        0      112 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    32893 2024-04-22 22:53:50.529395 alluka-0.1.5/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0       17 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/changelog.md
+-rw-r--r--   0        0        0       14 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/index.md
+-rw-r--r--   0        0        0       29 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/reference/abc.md
+-rw-r--r--   0        0        0       21 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/reference/index.md
+-rw-r--r--   0        0        0     5220 2024-04-22 22:53:50.529395 alluka-0.1.5/docs/usage.md
+-rw-r--r--   0        0        0     1593 2024-04-22 22:53:50.529395 alluka-0.1.5/mkdocs.yml
+-rw-r--r--   0        0        0     1714 2024-04-22 22:53:50.529395 alluka-0.1.5/noxfile.py
+-rw-r--r--   0        0        0       50 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.env.example
+-rw-r--r--   0        0        0       14 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.gitattributes
+-rw-r--r--   0        0        0      454 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/dependabot.yml
+-rw-r--r--   0        0        0     3675 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/docker-publish.yml
+-rw-r--r--   0        0        0     1240 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/freeze-for-pr.yml
+-rw-r--r--   0        0        0      959 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      976 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/reformat.yml
+-rw-r--r--   0        0        0     1032 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/resync-piped.yml
+-rw-r--r--   0        0        0      832 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/type-check.yml
+-rw-r--r--   0        0        0     1182 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/update-licence.yml
+-rw-r--r--   0        0        0     1217 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/upgrade-locks.yml
+-rw-r--r--   0        0        0     1114 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.github/workflows/verify-locks.yml
+-rw-r--r--   0        0        0     1751 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/.gitignore
+-rw-r--r--   0        0        0      404 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/Dockerfile
+-rw-r--r--   0        0        0     1520 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/LICENSE
+-rw-r--r--   0        0        0      138 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/README.md
+-rw-r--r--   0        0        0    31151 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/main.py
+-rw-r--r--   0        0        0       10 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements-extra.txt
+-rw-r--r--   0        0        0      123 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements.in
+-rw-r--r--   0        0        0    23268 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/bot/requirements.txt
+-rw-r--r--   0        0        0      933 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/flake8.in
+-rw-r--r--   0        0        0    20501 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/flake8.txt
+-rw-r--r--   0        0        0       10 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking-extra.txt
+-rw-r--r--   0        0        0      112 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking.in
+-rw-r--r--   0        0        0    33981 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/dev-requirements/type-checking.txt
+-rw-r--r--   0        0        0      240 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/docker-compose.yml
+-rw-r--r--   0        0        0       26 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/CODEOWNERS
+-rw-r--r--   0        0        0       45 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/FUNDING.yml
+-rw-r--r--   0        0        0      764 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/clippy.yml
+-rw-r--r--   0        0        0     3953 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/docker-publish.yml
+-rw-r--r--   0        0        0     1133 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/freeze-for-pr.yml
+-rw-r--r--   0        0        0     1271 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/lint.yml
+-rw-r--r--   0        0        0     1577 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/pr-docs.yml
+-rw-r--r--   0        0        0     1073 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/publish.yml
+-rw-r--r--   0        0        0     2399 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/py-test.yml
+-rw-r--r--   0        0        0     1013 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/reformat.yml
+-rw-r--r--   0        0        0     1373 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/release-docs.yml
+-rw-r--r--   0        0        0     1075 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/resync-piped.yml
+-rw-r--r--   0        0        0     1223 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/rustfmt.yml
+-rw-r--r--   0        0        0      869 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/type-check.yml
+-rw-r--r--   0        0        0     1191 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/update-licence.yml
+-rw-r--r--   0        0        0     1226 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/upgrade-locks.yml
+-rw-r--r--   0        0        0     1130 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/verify-locks.yml
+-rw-r--r--   0        0        0      887 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/actions/verify-types.yml
+-rw-r--r--   0        0        0      550 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/dependabot.yml
+-rw-r--r--   0        0        0      524 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/github/pull_request_template.md
+-rw-r--r--   0        0        0     1713 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/noxfile.py
+-rw-r--r--   0        0        0     4896 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/pyproject.toml
+-rw-r--r--   0        0        0      115 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/docs.in
+-rw-r--r--   0        0        0    36417 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/docs.txt
+-rw-r--r--   0        0        0       31 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/flake8.in
+-rw-r--r--   0        0        0     1580 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/flake8.txt
+-rw-r--r--   0        0        0       32 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/freeze-locks.in
+-rw-r--r--   0        0        0    48844 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/freeze-locks.txt
+-rw-r--r--   0        0        0     1068 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/library-flake8.in
+-rw-r--r--   0        0        0    33521 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/library-flake8.txt
+-rw-r--r--   0        0        0       58 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/lint.in
+-rw-r--r--   0        0        0     6314 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/lint.txt
+-rw-r--r--   0        0        0       60 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/nox.in
+-rw-r--r--   0        0        0    15576 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/nox.txt
+-rw-r--r--   0        0        0       12 2024-04-22 22:53:51.201402 alluka-0.1.5/piped/python/base-requirements/publish.in
+-rw-r--r--   0        0        0     9861 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/publish.txt
+-rw-r--r--   0        0        0       78 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/reformat.in
+-rw-r--r--   0        0        0    18195 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/reformat.txt
+-rw-r--r--   0        0        0       64 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/tests.in
+-rw-r--r--   0        0        0     7400 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/tests.txt
+-rw-r--r--   0        0        0       29 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/type-checking.in
+-rw-r--r--   0        0        0     4051 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/base-requirements/type-checking.txt
+-rw-r--r--   0        0        0    24295 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/noxfile.py
+-rw-r--r--   0        0        0     1714 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/noxfile.template.py
+-rw-r--r--   0        0        0     4527 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/piped_shared/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/piped_shared/py.typed
+-rw-r--r--   0        0        0      334 2024-04-22 22:53:51.205402 alluka-0.1.5/piped/python/pyproject.toml
+-rw-r--r--   0        0        0     6898 2024-04-22 22:53:50.529395 alluka-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1596 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/__init__.py
+-rw-r--r--   0        0        0    13421 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test__client.py
+-rw-r--r--   0        0        0     2881 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test__self_injecting.py
+-rw-r--r--   0        0        0    50719 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_async_callback_di.py
+-rw-r--r--   0        0        0    52004 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_async_callback_di_future_annotations.py
+-rw-r--r--   0        0        0    45828 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_callback_di.py
+-rw-r--r--   0        0        0    46212 2024-04-22 22:53:50.529395 alluka-0.1.5/tests/test_callback_di_future_annotations.py
+-rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 alluka-0.1.5/PKG-INFO
```

### Comparing `alluka-0.1.4/.github/pull_request_template.md` & `alluka-0.1.5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/.github/workflows/freeze-for-pr.yml` & `alluka-0.1.5/.github/workflows/freeze-for-pr.yml`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     paths: ["piped", "pyproject.toml", "requirements.in", "dev-requirements/*.in", "!dev-requirements/constraints.in"]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/.github/workflows/lint.yml` & `alluka-0.1.5/.github/workflows/lint.yml`

 * *Files 20% similar despite different names*

```diff
@@ -16,20 +16,20 @@
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
```

### Comparing `alluka-0.1.4/.github/workflows/pr-docs.yml` & `alluka-0.1.5/.github/workflows/pr-docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
 jobs:
   deploy-docs-preview:
     runs-on: ubuntu-latest
 
     steps:
       - name: Fetch merge branch
-        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           ref: ${{ github.event.pull_request.head.sha }}
           repository: ${{ github.event.pull_request.head.repo.full_name }}
           submodules: "true"
 
       - name: Set up Python 3.9
         if: github.event.action != 'closed'
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         if: github.event.action != 'closed'
         run: |
           python -m pip install --upgrade pip wheel
```

### Comparing `alluka-0.1.4/.github/workflows/publish.yml` & `alluka-0.1.5/.github/workflows/type-check.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,34 +1,38 @@
-name: Publish a new release
+name: Type check
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 on:
-  release:
-    # Only use the types keyword to narrow down the activity types that will trigger your workflow.
-    types:
-      - published
+  push:
+    branches:
+      - master
+  pull_request:
+    branches:
+      - master
+  schedule:
+    - cron: "0 12 * * 6"
+  workflow_dispatch:
 
 jobs:
-  publish-docs:
-    uses: ./.github/workflows/release-docs.yml
-
-  publish:
+  type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
-      - name: Install prerequisites
+      - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
-      - name: publish
-        run: python -m nox -s publish
-        env:
-          PUBLISH_TOKEN: ${{ secrets.PUBLISH_TOKEN }}
+      - name: Run type checker
+        run: python -m nox -s type-check
```

### Comparing `alluka-0.1.4/.github/workflows/py-test.yml` & `alluka-0.1.5/.github/workflows/py-test.yml`

 * *Files 12% similar despite different names*

```diff
@@ -22,20 +22,20 @@
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
         python-version: ["3.9", "3.10", "3.11", "3.12"]
 
     runs-on: ${{ matrix.os }}
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
@@ -47,20 +47,20 @@
   # TODO: Could we switch over to gather coverage from the normal test runs and combining
   # the result once https://github.com/nedbat/coveragepy/issues/1002 is fixed?
   upload-coverage:
     # needs: [test]
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
@@ -73,12 +73,12 @@
         uses: paambaati/codeclimate-action@a1831d7162ea1fbc612ffe5fb3b90278b7999d59
         env:
           CC_TEST_REPORTER_ID: a965935acdc9066802d7201945219784c0f24d22e8a2dff0e6529207726bc8af
         with:
           coverageLocations: .coverage.xml:coverage.py
 
       - name: Archive coverage
-        uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: coverage
           path: ./coverage_html
           if-no-files-found: error
```

### Comparing `alluka-0.1.4/.github/workflows/reformat.yml` & `alluka-0.1.5/piped/.github/workflows/resync-piped.yml`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,41 @@
-name: Reformat PR code
+name: Resync piped
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
+    paths: ["github/actions/*", "pyproject.toml"]
 
 jobs:
-  reformat:
+  resync-piped:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python 3.11
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
-      - name: Reformat
-        run: python -m nox -s reformat bot-package-diff
+      - name: Resync Piped
+        run: python -m nox -s copy-piped bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/.github/workflows/release-docs.yml` & `alluka-0.1.5/.github/workflows/release-docs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,20 @@
   workflow_dispatch:
 
 jobs:
   publish-docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: Install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
@@ -27,15 +27,15 @@
         id: doc_info
         run: |
           mkdir site
           python -m nox -s generate-docs -- -o ./site -j
           echo "GIT_HASH=$(git rev-parse HEAD)" >> $GITHUB_STATE
 
       - name: Push
-        uses: JamesIves/github-pages-deploy-action@65b5dfd4f5bcd3a7403bbc2959c144256167464e
+        uses: JamesIves/github-pages-deploy-action@ec9c88baef04b842ca6f0a132fd61c762aa6c1b0
         with:
           branch: docs
           commit-message: "${{ steps.doc_info.outputs.GIT_HASH }} docs (${{ github.event.release.tag_name || github.event.ref }})"
           clean-exclude: pr-preview
           folder: ./site
           git-config-email: "120557446+always-on-duty[bot]@users.noreply.github.com"
           git-config-name: "always-on-duty[bot]"
```

### Comparing `alluka-0.1.4/.github/workflows/resync-piped.yml` & `alluka-0.1.5/.github/workflows/resync-piped.yml`

 * *Files 17% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     paths: ["piped", "piped.toml", "pyproject.toml"]
 
 jobs:
   resync-piped:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Resync Piped
         run: python -m nox -s copy-piped bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/.github/workflows/type-check.yml` & `alluka-0.1.5/.github/workflows/verify-types.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Type check
+name: Verify type-completeness
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   push:
@@ -12,27 +12,27 @@
     branches:
       - master
   schedule:
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
-  type-check:
+  verify-types:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
-      - name: Run type checker
-        run: python -m nox -s type-check
+      - name: Run verify types
+        run: python -m nox -s verify-types
```

### Comparing `alluka-0.1.4/.github/workflows/update-licence.yml` & `alluka-0.1.5/.github/workflows/update-licence.yml`

 * *Files 14% similar despite different names*

```diff
@@ -6,33 +6,33 @@
   workflow_dispatch:
 
 jobs:
   update-licence:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Update licence
         run: python -m nox -s update-licence
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@153407881ec5c347639a548ade7d8ad1d6740e38
+        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/update-licence
           commit-message: Update licence
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Update licence
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.4/.github/workflows/upgrade-locks.yml` & `alluka-0.1.5/.github/workflows/upgrade-locks.yml`

 * *Files 18% similar despite different names*

```diff
@@ -6,33 +6,33 @@
   workflow_dispatch:
 
 jobs:
   upgrade-deps:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@153407881ec5c347639a548ade7d8ad1d6740e38
+        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
         with:
           author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           branch: task/upgrade-deps
           commit-message: Upgrade dependency locks
           committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
           title: Upgrade dependency locks
           token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
```

### Comparing `alluka-0.1.4/.github/workflows/verify-locks.yml` & `alluka-0.1.5/.github/workflows/verify-locks.yml`

 * *Files 7% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     paths: ["dev-requirements/*.txt"]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./piped/python/base-requirements/nox.txt
```

### Comparing `alluka-0.1.4/.github/workflows/verify-types.yml` & `alluka-0.1.5/piped/.github/workflows/lint.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Verify type-completeness
+name: Lint
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   push:
@@ -12,27 +12,33 @@
     branches:
       - master
   schedule:
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
-  verify-types:
+  lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.9
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python 3.11
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.9"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./piped/python/base-requirements/nox.txt
+          python -m pip install -r ./python/base-requirements/nox.txt
 
-      - name: Run verify types
-        run: python -m nox -s verify-types
+      - name: Lint markup
+        run: python -m nox -s verify-markup
+
+      - name: Check spelling
+        run: python -m nox -s spell-check
+
+      - name: Lint with flake8
+        run: python -m nox -s flake8
```

### Comparing `alluka-0.1.4/.gitignore` & `alluka-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/CHANGELOG.md` & `alluka-0.1.5/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.1.5] - 2024-04-22
+- Improve error message when attempting to use [alluka.inject][] without DI.
+
 ## [0.1.4] - 2023-12-27
 ### Added
 - Python 3.12 support.
 
 ## [0.1.3] - 2022-11-12
 ### Added
 - `alluka.abc.Client` is now set as a type dependency by default.
@@ -66,13 +69,14 @@
 ### Changed
 - Passed keyword arguments are now prioritised over dependency injection.
 
 ### Removed
 - The public `CallackDescriptor` and `TypeDescriptor` classes as callbacks
   are now processed within the client and any necessary caching is kept internal.
 
-[Unreleased]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.4...HEAD
+[Unreleased]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.5...HEAD
+[0.1.5]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.4...v0.1.5
 [0.1.4]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.3...v0.1.4
 [0.1.3]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.2...v0.1.3
 [0.1.2]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.1...v0.1.2
 [0.1.1]: https://github.com/FasterSpeeding/Alluka/compare/v0.1.0...v0.1.1
 [0.1.0]: https://github.com/FasterSpeeding/Alluka/compare/ed0567142b8e11f98408735495dbc4f771dc8643...v0.1.0
```

### Comparing `alluka-0.1.4/CODE_OF_CONDUCT.md` & `alluka-0.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/CONTRIBUTING.md` & `alluka-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/LICENSE` & `alluka-0.1.5/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020-2023, Faster Speeding
+Copyright (c) 2020-2024, Faster Speeding
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/README.md` & `alluka-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/alluka/__init__.py` & `alluka-0.1.5/alluka/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/alluka/_client.py` & `alluka-0.1.5/alluka/_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -58,16 +58,15 @@
 _SyncCallbackSigT = typing.TypeVar("_SyncCallbackSigT", bound=collections.Callable[..., typing.Any])
 
 _TypeT = type[_T]
 _UndefinedOr = typing.Union[alluka.Undefined, _T]
 
 
 @typing.overload
-def inject(*, callback: alluka.CallbackSig[_T]) -> _T:
-    ...
+def inject(*, callback: alluka.CallbackSig[_T]) -> _T: ...
 
 
 @typing.overload
 def inject(*, type: _TypeT[_T]) -> _T:  # noqa: A002
     ...
 
 
@@ -172,40 +171,36 @@
     def as_self_injecting(self, callback: _SyncCallbackSigT, /) -> alluka.SelfInjecting[_SyncCallbackSigT]:
         # <<inherited docstring from alluka.abc.Client>>.
         return _self_injecting.SelfInjecting(self, callback)
 
     @typing.overload
     def call_with_di(
         self, callback: collections.Callable[..., _AnyCoro], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        ...
+    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         # <<inherited docstring from alluka.abc.Client>>.
         return BasicContext(self).call_with_di(callback, *args, **kwargs)
 
     @typing.overload
     def call_with_ctx(
         self,
         ctx: alluka.Context,
         callback: collections.Callable[..., _AnyCoro],
         *args: typing.Any,
         **kwargs: typing.Any,
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
     def call_with_ctx(
         self, ctx: alluka.Context, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     def call_with_ctx(
         self, ctx: alluka.Context, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any
     ) -> _T:
         # <<inherited docstring from alluka.abc.Client>>.
         descriptors = self._build_descriptors(callback)
         if descriptors:
@@ -234,28 +229,26 @@
                 for n, v in descriptors.items()
             } | kwargs
 
         result = callback(*args, **kwargs)
         if asyncio.iscoroutine(result):
             return typing.cast("_T", await result)
 
-        return typing.cast("_T", result)
+        return typing.cast("_T", result)  # noqa: ASYNC910  # This is ignored for performance's sake.
 
     def set_type_dependency(self, type_: type[_T], value: _T, /) -> Self:
         # <<inherited docstring from alluka.abc.Client>>.
         self._type_dependencies[type_] = value
         return self
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     def get_type_dependency(
         self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
     ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
         # <<inherited docstring from alluka.abc.Client>>.
         return self._type_dependencies.get(type_, default)
 
@@ -307,52 +300,46 @@
             self._result_cache = {}
 
         self._result_cache[callback] = value
 
     @typing.overload
     def call_with_di(
         self, callback: collections.Callable[..., _AnyCoro], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        ...
+    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         # <<inherited docstring from alluka.abc.Context>>.
         return self._injection_client.call_with_ctx(self, callback, *args, **kwargs)
 
     async def call_with_async_di(self, callback: alluka.CallbackSig[_T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         # <<inherited docstring from alluka.abc.Context>>.
         return await self._injection_client.call_with_ctx_async(self, callback, *args, **kwargs)
 
     @typing.overload
-    def get_cached_result(self, callback: alluka.CallbackSig[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_cached_result(self, callback: alluka.CallbackSig[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
     def get_cached_result(
         self, callback: alluka.CallbackSig[_T], /, *, default: _DefaultT
-    ) -> typing.Union[_T, _DefaultT]:
-        ...
+    ) -> typing.Union[_T, _DefaultT]: ...
 
     def get_cached_result(
         self, callback: alluka.CallbackSig[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
     ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
         # <<inherited docstring from alluka.abc.Context>>.
         return self._result_cache.get(callback, default) if self._result_cache else default
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
-    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     def get_type_dependency(
         self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = alluka.UNDEFINED
     ) -> typing.Union[_T, _DefaultT, alluka.Undefined]:
         # <<inherited docstring from alluka.abc.Context>>.
         if self._special_case_types and (value := self._special_case_types.get(type_, default)) is not default:
             return typing.cast("_T", value)
```

### Comparing `alluka-0.1.4/alluka/_errors.py` & `alluka-0.1.5/alluka/_errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/alluka/_self_injecting.py` & `alluka-0.1.5/alluka/_self_injecting.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -40,15 +40,15 @@
 _CallbackSigT = typing.TypeVar("_CallbackSigT", bound=alluka.CallbackSig[typing.Any])
 _SyncCallbackT = typing.TypeVar("_SyncCallbackT", bound=collections.Callable[..., typing.Any])
 _T = typing.TypeVar("_T")
 _CoroT = collections.Coroutine[typing.Any, typing.Any, _T]
 
 
 class AsyncSelfInjecting(alluka.AsyncSelfInjecting[_CallbackSigT]):
-    """Class used to link a sync function to a client to make it self-injecting.
+    """Class used to link an async function to a client to make it self-injecting.
 
     Examples
     --------
     ```py
     async def callback(database: Database = alluka.inject(type=Database)) -> None:
         await database.do_something()
     ...
@@ -91,22 +91,20 @@
         """
         self._callback = callback
         self._client = client
 
     @typing.overload
     async def __call__(
         self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     @typing.overload
     async def __call__(
         self: AsyncSelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     async def __call__(  # pyright: ignore[reportIncompatibleMethodOverride]
         self: typing.Union[
             AsyncSelfInjecting[collections.Callable[..., _T]], AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]]
         ],
         *args: typing.Any,
         **kwargs: typing.Any,
```

### Comparing `alluka-0.1.4/alluka/_types.py` & `alluka-0.1.5/alluka/_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -25,14 +25,15 @@
 # FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """Internal types used by Alluka."""
+
 from __future__ import annotations
 
 __all__: list[str] = ["Injected", "InjectedDescriptor"]
 
 import enum
 import typing
 
@@ -252,14 +253,19 @@
         """
         if callback is not None and type is not None:
             raise ValueError("Only one of `callback` or `type` can be specified")
 
         self.callback = callback
         self.type = type
 
+    def __getattr__(self, __name: str) -> typing.NoReturn:
+        raise AttributeError(
+            "Tried accessing a parameter that was not injected yet. Did you forget to inject dependencies?"
+        )
+
 
 Injected = typing.Annotated[_T, InjectedTypes.TYPE]
 """Type alias used to declare a keyword argument as requiring an injected type.
 
 If a union (e.g. `typing.Union[A, B]`, `A | B`, `typing.Optional[A]`)
 is passed then each type in the union will be tried separately rather than
 the literal type, allowing for resolving `A | B` to the value set by
```

### Comparing `alluka-0.1.4/alluka/_vendor/inspect.py` & `alluka-0.1.5/alluka/_vendor/inspect.py`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/alluka/_vendor/inspect.py.LICENSE` & `alluka-0.1.5/alluka/_vendor/inspect.py.LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/alluka/_vendor/inspect.pyi` & `alluka-0.1.5/alluka/_vendor/inspect.pyi`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/alluka/_vendor/inspect.pyi.LICENSE` & `alluka-0.1.5/alluka/_vendor/inspect.pyi.LICENSE`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/alluka/_visitor.py` & `alluka-0.1.5/alluka/_visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -56,16 +56,15 @@
 
 class Node(abc.ABC):
     """Represents a node which may hold parameter injection information."""
 
     __slots__ = ()
 
     @abc.abstractmethod
-    def accept(self, visitor: ParameterVisitor, /) -> typing.Optional[_types.InjectedTuple]:
-        ...
+    def accept(self, visitor: ParameterVisitor, /) -> typing.Optional[_types.InjectedTuple]: ...
 
 
 class Annotation(Node):
     """Node which represent's a parameter's type-hint."""
 
     __slots__ = ("_callback", "_name", "_raw_annotation")
```

### Comparing `alluka-0.1.4/alluka/abc.py` & `alluka-0.1.5/alluka/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -149,21 +149,19 @@
             The self-injecting callback.
         """
 
     @typing.overload
     @abc.abstractmethod
     def call_with_di(
         self, callback: collections.Callable[..., _CoroT[typing.Any]], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
     @abc.abstractmethod
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        ...
+    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
     @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Call a function with sync dependency injection.
 
         Parameters
         ----------
@@ -194,23 +192,21 @@
     @abc.abstractmethod
     def call_with_ctx(
         self,
         ctx: Context,
         callback: collections.Callable[..., _CoroT[typing.Any]],
         *args: typing.Any,
         **kwargs: typing.Any,
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
     @abc.abstractmethod
     def call_with_ctx(
         self, ctx: Context, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     @abc.abstractmethod
     def call_with_ctx(
         self, ctx: Context, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any
     ) -> _T:
         """Call a function with an existing DI context.
 
@@ -320,21 +316,19 @@
         -------
         Self
             The client instance to allow chaining.
         """
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
     def get_type_dependency(
         self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
     ) -> typing.Union[_T, _DefaultT, Undefined]:
         """Get the implementation for an injected type.
 
@@ -453,21 +447,19 @@
             The value to cache.
         """
 
     @typing.overload
     @abc.abstractmethod
     def call_with_di(
         self, callback: collections.Callable[..., _CoroT[typing.Any]], *args: typing.Any, **kwargs: typing.Any
-    ) -> typing.NoReturn:
-        ...
+    ) -> typing.NoReturn: ...
 
     @typing.overload
     @abc.abstractmethod
-    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
-        ...
+    def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T: ...
 
     @abc.abstractmethod
     def call_with_di(self, callback: collections.Callable[..., _T], *args: typing.Any, **kwargs: typing.Any) -> _T:
         """Call a function with the current DI context.
 
         Parameters
         ----------
@@ -519,21 +511,19 @@
         alluka.MissingDependencyError
             If any of the callback's required type dependencies aren't implemented
             by the client.
         """
 
     @typing.overload
     @abc.abstractmethod
-    def get_cached_result(self, callback: CallbackSig[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_cached_result(self, callback: CallbackSig[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
     @abc.abstractmethod
-    def get_cached_result(self, callback: CallbackSig[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]:
-        ...
+    def get_cached_result(self, callback: CallbackSig[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
     def get_cached_result(
         self, callback: CallbackSig[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
     ) -> typing.Union[_T, _DefaultT, Undefined]:
         """Get the cached result of a callback.
 
@@ -556,21 +546,19 @@
             If the callback's result hasn't been cached or caching isn't
             implementing then this will return the value of `default` if it
             is provided, else [alluka.abc.UNDEFINED][].
         """
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /) -> _UndefinedOr[_T]: ...
 
     @typing.overload
     @abc.abstractmethod
-    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]:
-        ...
+    def get_type_dependency(self, type_: type[_T], /, *, default: _DefaultT) -> typing.Union[_T, _DefaultT]: ...
 
     @abc.abstractmethod
     def get_type_dependency(
         self, type_: type[_T], /, *, default: _UndefinedOr[_DefaultT] = UNDEFINED
     ) -> typing.Union[_T, _DefaultT, Undefined]:
         """Get the implementation for an injected type.
 
@@ -619,23 +607,21 @@
     def callback(self) -> _CallbackT:
         """The callback this wraps."""
 
     @typing.overload
     @abc.abstractmethod
     async def __call__(
         self: AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     @typing.overload
     @abc.abstractmethod
     async def __call__(
         self: AsyncSelfInjecting[collections.Callable[..., _T]], *args: typing.Any, **kwargs: typing.Any
-    ) -> _T:
-        ...
+    ) -> _T: ...
 
     @abc.abstractmethod
     async def __call__(
         self: typing.Union[
             AsyncSelfInjecting[collections.Callable[..., _T]], AsyncSelfInjecting[collections.Callable[..., _CoroT[_T]]]
         ],
         *args: typing.Any,
```

### Comparing `alluka-0.1.4/dev-requirements/tests.txt` & `alluka-0.1.5/dev-requirements/tests.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform dev-requirements/tests.in --output-file dev-requirements/tests.txt --min-python-version 3.9.0,<3.13
 #
-anyio==4.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:745843b39e829e108e518c489b31dc757de7d2131d53fac32bd8df268227bfee \
-    --hash=sha256:e1875bb4b4e2de1669f4bc7869b6d3f54231cdced71605e6e64c9be77e3be50f
-attrs==23.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
+anyio==4.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8 \
+    --hash=sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6
+attrs==23.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
 cffi==1.16.0 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
@@ -62,120 +62,120 @@
     --hash=sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4 \
     --hash=sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627 \
     --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.13" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-coverage[toml]==7.3.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:020d56d2da5bc22a0e00a5b0d54597ee91ad72446fa4cf1b97c35022f6b6dbf0 \
-    --hash=sha256:11ab62d0ce5d9324915726f611f511a761efcca970bd49d876cf831b4de65be5 \
-    --hash=sha256:183c16173a70caf92e2dfcfe7c7a576de6fa9edc4119b8e13f91db7ca33a7923 \
-    --hash=sha256:27ee94f088397d1feea3cb524e4313ff0410ead7d968029ecc4bc5a7e1d34fbf \
-    --hash=sha256:3024ec1b3a221bd10b5d87337d0373c2bcaf7afd86d42081afe39b3e1820323b \
-    --hash=sha256:309ed6a559bc942b7cc721f2976326efbfe81fc2b8f601c722bff927328507dc \
-    --hash=sha256:33e63c578f4acce1b6cd292a66bc30164495010f1091d4b7529d014845cd9bee \
-    --hash=sha256:36797b3625d1da885b369bdaaa3b0d9fb8865caed3c2b8230afaa6005434aa2f \
-    --hash=sha256:36d75ef2acab74dc948d0b537ef021306796da551e8ac8b467810911000af66a \
-    --hash=sha256:38d0b307c4d99a7aca4e00cad4311b7c51b7ac38fb7dea2abe0d182dd4008e05 \
-    --hash=sha256:3d892a19ae24b9801771a5a989fb3e850bd1ad2e2b6e83e949c65e8f37bc67a1 \
-    --hash=sha256:3f477fb8a56e0c603587b8278d9dbd32e54bcc2922d62405f65574bd76eba78a \
-    --hash=sha256:47ee56c2cd445ea35a8cc3ad5c8134cb9bece3a5cb50bb8265514208d0a65928 \
-    --hash=sha256:4a4184dcbe4f98d86470273e758f1d24191ca095412e4335ff27b417291f5964 \
-    --hash=sha256:5214362abf26e254d749fc0c18af4c57b532a4bfde1a057565616dd3b8d7cc94 \
-    --hash=sha256:607b6c6b35aa49defaebf4526729bd5238bc36fe3ef1a417d9839e1d96ee1e4c \
-    --hash=sha256:610afaf929dc0e09a5eef6981edb6a57a46b7eceff151947b836d869d6d567c1 \
-    --hash=sha256:6879fe41c60080aa4bb59703a526c54e0412b77e649a0d06a61782ecf0853ee1 \
-    --hash=sha256:74397a1263275bea9d736572d4cf338efaade2de9ff759f9c26bcdceb383bb49 \
-    --hash=sha256:758ebaf74578b73f727acc4e8ab4b16ab6f22a5ffd7dd254e5946aba42a4ce76 \
-    --hash=sha256:782693b817218169bfeb9b9ba7f4a9f242764e180ac9589b45112571f32a0ba6 \
-    --hash=sha256:7c4277ddaad9293454da19121c59f2d850f16bcb27f71f89a5c4836906eb35ef \
-    --hash=sha256:85072e99474d894e5df582faec04abe137b28972d5e466999bc64fc37f564a03 \
-    --hash=sha256:8a9c5bc5db3eb4cd55ecb8397d8e9b70247904f8eca718cc53c12dcc98e59fc8 \
-    --hash=sha256:8ce03e25e18dd9bf44723e83bc202114817f3367789052dc9e5b5c79f40cf59d \
-    --hash=sha256:93698ac0995516ccdca55342599a1463ed2e2d8942316da31686d4d614597ef9 \
-    --hash=sha256:997aa14b3e014339d8101b9886063c5d06238848905d9ad6c6eabe533440a9a7 \
-    --hash=sha256:9ac17b94ab4ca66cf803f2b22d47e392f0977f9da838bf71d1f0db6c32893cb9 \
-    --hash=sha256:a02ac7c51819702b384fea5ee033a7c202f732a2a2f1fe6c41e3d4019828c8d3 \
-    --hash=sha256:a1c3e9d2bbd6f3f79cfecd6f20854f4dc0c6e0ec317df2b265266d0dc06535f1 \
-    --hash=sha256:a877810ef918d0d345b783fc569608804f3ed2507bf32f14f652e4eaf5d8f8d0 \
-    --hash=sha256:a8e258dcc335055ab59fe79f1dec217d9fb0cdace103d6b5c6df6b75915e7959 \
-    --hash=sha256:aefbb29dc56317a4fcb2f3857d5bce9b881038ed7e5aa5d3bcab25bd23f57328 \
-    --hash=sha256:aff2bd3d585969cc4486bfc69655e862028b689404563e6b549e6a8244f226df \
-    --hash=sha256:b1e0f25ae99cf247abfb3f0fac7ae25739e4cd96bf1afa3537827c576b4847e5 \
-    --hash=sha256:b710869a15b8caf02e31d16487a931dbe78335462a122c8603bb9bd401ff6fb2 \
-    --hash=sha256:bfed0ec4b419fbc807dec417c401499ea869436910e1ca524cfb4f81cf3f60e7 \
-    --hash=sha256:c15fdfb141fcf6a900e68bfa35689e1256a670db32b96e7a931cab4a0e1600e5 \
-    --hash=sha256:c6a23ae9348a7a92e7f750f9b7e828448e428e99c24616dec93a0720342f241d \
-    --hash=sha256:c75738ce13d257efbb6633a049fb2ed8e87e2e6c2e906c52d1093a4d08d67c6b \
-    --hash=sha256:d1d0ce6c6947a3a4aa5479bebceff2c807b9f3b529b637e2b33dea4468d75fc7 \
-    --hash=sha256:d5b14abde6f8d969e6b9dd8c7a013d9a2b52af1235fe7bebef25ad5c8f47fa18 \
-    --hash=sha256:d6ed790728fb71e6b8247bd28e77e99d0c276dff952389b5388169b8ca7b1c28 \
-    --hash=sha256:e0d84099ea7cba9ff467f9c6f747e3fc3906e2aadac1ce7b41add72e8d0a3712 \
-    --hash=sha256:e4353923f38d752ecfbd3f1f20bf7a3546993ae5ecd7c07fd2f25d40b4e54571 \
-    --hash=sha256:e91029d7f151d8bf5ab7d8bfe2c3dbefd239759d642b211a677bc0709c9fdb96 \
-    --hash=sha256:ea473c37872f0159294f7073f3fa72f68b03a129799f3533b2bb44d5e9fa4f82 \
-    --hash=sha256:f154bd866318185ef5865ace5be3ac047b6d1cc0aeecf53bf83fe846f4384d5d \
-    --hash=sha256:f97ff5a9fc2ca47f3383482858dd2cb8ddbf7514427eecf5aa5f7992d0571429 \
-    --hash=sha256:f99b7d3f7a7adfa3d11e3a48d1a91bb65739555dd6a0d3fa68aa5852d962e5b1 \
-    --hash=sha256:fb220b3596358a86361139edce40d97da7458412d412e1e10c8e1970ee8c09ab \
-    --hash=sha256:fd2f8a641f8f193968afdc8fd1697e602e199931012b574194052d132a79be13
-exceptiongroup==1.2.0 ; python_full_version >= "3.9.0" and python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
-execnet==2.0.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:88256416ae766bc9e8895c76a87928c0012183da3cc4fc18016e6f050e025f41 \
-    --hash=sha256:cc59bc4423742fd71ad227122eb0dd44db51efb3dc4095b45ac9a08c770096af
-idna==3.6 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+coverage[toml]==7.4.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
+    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
+    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
+    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
+    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
+    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
+    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
+    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
+    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
+    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
+    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
+    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
+    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
+    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
+    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
+    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
+    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
+    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
+    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
+    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
+    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
+    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
+    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
+    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
+    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
+    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
+    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
+    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
+    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
+    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
+    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
+    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
+    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
+    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
+    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
+    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
+    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
+    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
+    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
+    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
+    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
+    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
+    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
+    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
+    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
+    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
+    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
+    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
+    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
+    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
+    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
+    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
+exceptiongroup==1.2.1 ; python_full_version >= "3.9.0" and python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
+execnet==2.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:26dee51f1b80cebd6d0ca8e74dd8745419761d3bef34163928cbebbdc4749fdc \
+    --hash=sha256:5189b52c6121c24feae288166ab41b32549c7e2348652736540b9e6e7d4e72e3
+idna==3.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
 iniconfig==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
 mock==5.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:18c694e5ae8a208cdb3d2c20a993ca1a7b0efa258c247a1e565150f477f83744 \
     --hash=sha256:5e96aad5ccda4718e0a229ed94b2024df75cc2d55575ba5762d31f5767b8767d
 outcome==1.3.0.post0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:9dcf02e65f2971b80047b377468e72a268e15c0af3cf1238e6ff14f7f91143b8 \
     --hash=sha256:e771c5ce06d1415e356078d3bdd68523f284b4ce5419828922b6871e65eda82b
-packaging==23.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-pluggy==1.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12 \
-    --hash=sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7
-pycparser==2.21 ; python_full_version >= "3.9.0" and os_name == "nt" and implementation_name != "pypy" and python_version < "3.13" \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
-pytest-cov==4.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
-pytest-sugar==0.9.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:8cb5a4e5f8bbcd834622b0235db9e50432f4cbd71fef55b467fe44e43701e062 \
-    --hash=sha256:f1e74c1abfa55f7241cf7088032b6e378566f16b938f3f08905e2cf4494edd46
-pytest-timeout==2.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:3b0b95dabf3cb50bac9ef5ca912fa0cfc286526af17afc806824df20c2f72c90 \
-    --hash=sha256:bde531e096466f49398a59f2dde76fa78429a09a12411466f88a07213e220de2
+packaging==24.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+pluggy==1.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
+pycparser==2.22 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pytest-cov==5.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
+pytest-sugar==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a \
+    --hash=sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd
+pytest-timeout==2.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:12397729125c6ecbdaca01035b9e5239d4db97352320af155b3f5de1ba5165d9 \
+    --hash=sha256:68188cb703edfc6a18fad98dc25a3c61e9f24d644b0b70f33af545219fc7813e
 pytest-xdist==3.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:cbb36f3d67e0c478baa57fa4edc8843887e0f6cfc42d677530a36d7472b32d8a \
     --hash=sha256:d075629c7e00b611df89f490a5063944bee7a4362a5ff11c7cc7824a03dfce24
-pytest==7.4.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0d009c083ea859a71b76adf7c1d502e4bc170b80a8ef002da5806527b9591fac \
-    --hash=sha256:d989d136982de4e3b29dabcc838ad581c64e8ed52c11fbe86ddebd9da0818cd5
-sniffio==1.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
-    --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
+pytest==8.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
+    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
+sniffio==1.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
+    --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
 sortedcontainers==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
 termcolor==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63 \
     --hash=sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a
 tomli==2.0.1 ; python_full_version >= "3.9.0" and python_full_version <= "3.11.0a6" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-trio==0.23.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:5a0b566fa5d50cf231cfd6b08f3b03aa4179ff004b8f3144059587039e2b26d3 \
-    --hash=sha256:da1d35b9a2b17eb32cae2e763b16551f9aa6703634735024e32f325c9285069e
-typing-extensions==4.9.0 ; python_full_version >= "3.9.0" and python_version < "3.11" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+trio==0.25.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:9b41f5993ad2c0e5f62d0acca320ec657fdb6b2a2c22b8c7aed6caf154475c4e \
+    --hash=sha256:e6458efe29cc543e557a91e614e2b51710eba2961669329ce9c862d50c6e8e81
+typing-extensions==4.11.0 ; python_full_version >= "3.9.0" and python_version < "3.11" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
```

### Comparing `alluka-0.1.4/dev-requirements/type-checking.txt` & `alluka-0.1.5/dev-requirements/type-checking.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # To update, run:
 #
 #    pip-compile-cross-platform dev-requirements/type-checking.in --output-file dev-requirements/type-checking.txt --min-python-version 3.9.0,<3.13
 #
 annotated-types==0.6.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
     --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-anyio==4.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:745843b39e829e108e518c489b31dc757de7d2131d53fac32bd8df268227bfee \
-    --hash=sha256:e1875bb4b4e2de1669f4bc7869b6d3f54231cdced71605e6e64c9be77e3be50f
-argcomplete==3.2.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:30891d87f3c1abe091f2142613c9d33cac84a5e15404489f033b20399b691fec \
-    --hash=sha256:437f67fb9b058da5a090df505ef9be0297c4883993f3f56cb186ff087778cfb4
-attrs==23.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
+anyio==4.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8 \
+    --hash=sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6
+argcomplete==3.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
+    --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
+attrs==23.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
 cffi==1.16.0 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
@@ -68,351 +68,325 @@
     --hash=sha256:ed86a35631f7bfbb28e108dd96773b9d5a6ce4811cf6ea468bb6a359b256b1e4 \
     --hash=sha256:ee07e47c12890ef248766a6e55bd38ebfb2bb8edd4142d56db91b21ea68b7627 \
     --hash=sha256:fa3a0128b152627161ce47201262d3140edb5a5c3da88d73a1b790a959126956 \
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 colorama==0.4.6 ; python_full_version >= "3.9.0" and python_version < "3.13" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-colorlog==6.8.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:4ed23b05a1154294ac99f511fabe8c1d6d4364ec1f7fc989c7fb515ccc29d375 \
-    --hash=sha256:fbb6fdf9d5685f2517f388fb29bb27d54e8654dd31f58bc2a3b217e967a95ca6
-coverage[toml]==7.3.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:020d56d2da5bc22a0e00a5b0d54597ee91ad72446fa4cf1b97c35022f6b6dbf0 \
-    --hash=sha256:11ab62d0ce5d9324915726f611f511a761efcca970bd49d876cf831b4de65be5 \
-    --hash=sha256:183c16173a70caf92e2dfcfe7c7a576de6fa9edc4119b8e13f91db7ca33a7923 \
-    --hash=sha256:27ee94f088397d1feea3cb524e4313ff0410ead7d968029ecc4bc5a7e1d34fbf \
-    --hash=sha256:3024ec1b3a221bd10b5d87337d0373c2bcaf7afd86d42081afe39b3e1820323b \
-    --hash=sha256:309ed6a559bc942b7cc721f2976326efbfe81fc2b8f601c722bff927328507dc \
-    --hash=sha256:33e63c578f4acce1b6cd292a66bc30164495010f1091d4b7529d014845cd9bee \
-    --hash=sha256:36797b3625d1da885b369bdaaa3b0d9fb8865caed3c2b8230afaa6005434aa2f \
-    --hash=sha256:36d75ef2acab74dc948d0b537ef021306796da551e8ac8b467810911000af66a \
-    --hash=sha256:38d0b307c4d99a7aca4e00cad4311b7c51b7ac38fb7dea2abe0d182dd4008e05 \
-    --hash=sha256:3d892a19ae24b9801771a5a989fb3e850bd1ad2e2b6e83e949c65e8f37bc67a1 \
-    --hash=sha256:3f477fb8a56e0c603587b8278d9dbd32e54bcc2922d62405f65574bd76eba78a \
-    --hash=sha256:47ee56c2cd445ea35a8cc3ad5c8134cb9bece3a5cb50bb8265514208d0a65928 \
-    --hash=sha256:4a4184dcbe4f98d86470273e758f1d24191ca095412e4335ff27b417291f5964 \
-    --hash=sha256:5214362abf26e254d749fc0c18af4c57b532a4bfde1a057565616dd3b8d7cc94 \
-    --hash=sha256:607b6c6b35aa49defaebf4526729bd5238bc36fe3ef1a417d9839e1d96ee1e4c \
-    --hash=sha256:610afaf929dc0e09a5eef6981edb6a57a46b7eceff151947b836d869d6d567c1 \
-    --hash=sha256:6879fe41c60080aa4bb59703a526c54e0412b77e649a0d06a61782ecf0853ee1 \
-    --hash=sha256:74397a1263275bea9d736572d4cf338efaade2de9ff759f9c26bcdceb383bb49 \
-    --hash=sha256:758ebaf74578b73f727acc4e8ab4b16ab6f22a5ffd7dd254e5946aba42a4ce76 \
-    --hash=sha256:782693b817218169bfeb9b9ba7f4a9f242764e180ac9589b45112571f32a0ba6 \
-    --hash=sha256:7c4277ddaad9293454da19121c59f2d850f16bcb27f71f89a5c4836906eb35ef \
-    --hash=sha256:85072e99474d894e5df582faec04abe137b28972d5e466999bc64fc37f564a03 \
-    --hash=sha256:8a9c5bc5db3eb4cd55ecb8397d8e9b70247904f8eca718cc53c12dcc98e59fc8 \
-    --hash=sha256:8ce03e25e18dd9bf44723e83bc202114817f3367789052dc9e5b5c79f40cf59d \
-    --hash=sha256:93698ac0995516ccdca55342599a1463ed2e2d8942316da31686d4d614597ef9 \
-    --hash=sha256:997aa14b3e014339d8101b9886063c5d06238848905d9ad6c6eabe533440a9a7 \
-    --hash=sha256:9ac17b94ab4ca66cf803f2b22d47e392f0977f9da838bf71d1f0db6c32893cb9 \
-    --hash=sha256:a02ac7c51819702b384fea5ee033a7c202f732a2a2f1fe6c41e3d4019828c8d3 \
-    --hash=sha256:a1c3e9d2bbd6f3f79cfecd6f20854f4dc0c6e0ec317df2b265266d0dc06535f1 \
-    --hash=sha256:a877810ef918d0d345b783fc569608804f3ed2507bf32f14f652e4eaf5d8f8d0 \
-    --hash=sha256:a8e258dcc335055ab59fe79f1dec217d9fb0cdace103d6b5c6df6b75915e7959 \
-    --hash=sha256:aefbb29dc56317a4fcb2f3857d5bce9b881038ed7e5aa5d3bcab25bd23f57328 \
-    --hash=sha256:aff2bd3d585969cc4486bfc69655e862028b689404563e6b549e6a8244f226df \
-    --hash=sha256:b1e0f25ae99cf247abfb3f0fac7ae25739e4cd96bf1afa3537827c576b4847e5 \
-    --hash=sha256:b710869a15b8caf02e31d16487a931dbe78335462a122c8603bb9bd401ff6fb2 \
-    --hash=sha256:bfed0ec4b419fbc807dec417c401499ea869436910e1ca524cfb4f81cf3f60e7 \
-    --hash=sha256:c15fdfb141fcf6a900e68bfa35689e1256a670db32b96e7a931cab4a0e1600e5 \
-    --hash=sha256:c6a23ae9348a7a92e7f750f9b7e828448e428e99c24616dec93a0720342f241d \
-    --hash=sha256:c75738ce13d257efbb6633a049fb2ed8e87e2e6c2e906c52d1093a4d08d67c6b \
-    --hash=sha256:d1d0ce6c6947a3a4aa5479bebceff2c807b9f3b529b637e2b33dea4468d75fc7 \
-    --hash=sha256:d5b14abde6f8d969e6b9dd8c7a013d9a2b52af1235fe7bebef25ad5c8f47fa18 \
-    --hash=sha256:d6ed790728fb71e6b8247bd28e77e99d0c276dff952389b5388169b8ca7b1c28 \
-    --hash=sha256:e0d84099ea7cba9ff467f9c6f747e3fc3906e2aadac1ce7b41add72e8d0a3712 \
-    --hash=sha256:e4353923f38d752ecfbd3f1f20bf7a3546993ae5ecd7c07fd2f25d40b4e54571 \
-    --hash=sha256:e91029d7f151d8bf5ab7d8bfe2c3dbefd239759d642b211a677bc0709c9fdb96 \
-    --hash=sha256:ea473c37872f0159294f7073f3fa72f68b03a129799f3533b2bb44d5e9fa4f82 \
-    --hash=sha256:f154bd866318185ef5865ace5be3ac047b6d1cc0aeecf53bf83fe846f4384d5d \
-    --hash=sha256:f97ff5a9fc2ca47f3383482858dd2cb8ddbf7514427eecf5aa5f7992d0571429 \
-    --hash=sha256:f99b7d3f7a7adfa3d11e3a48d1a91bb65739555dd6a0d3fa68aa5852d962e5b1 \
-    --hash=sha256:fb220b3596358a86361139edce40d97da7458412d412e1e10c8e1970ee8c09ab \
-    --hash=sha256:fd2f8a641f8f193968afdc8fd1697e602e199931012b574194052d132a79be13
+colorlog==6.8.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:3e3e079a41feb5a1b64f978b5ea4f46040a94f11f0e8bbb8261e3dbbeca64d44 \
+    --hash=sha256:4dcbb62368e2800cb3c5abd348da7e53f6c362dda502ec27c560b2e58a66bd33
+coverage[toml]==7.4.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
+    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
+    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
+    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
+    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
+    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
+    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
+    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
+    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
+    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
+    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
+    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
+    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
+    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
+    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
+    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
+    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
+    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
+    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
+    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
+    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
+    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
+    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
+    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
+    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
+    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
+    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
+    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
+    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
+    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
+    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
+    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
+    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
+    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
+    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
+    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
+    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
+    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
+    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
+    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
+    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
+    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
+    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
+    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
+    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
+    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
+    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
+    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
+    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
+    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
+    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
+    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
 distlib==0.3.8 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
-exceptiongroup==1.2.0 ; python_full_version >= "3.9.0" and python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
-execnet==2.0.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:88256416ae766bc9e8895c76a87928c0012183da3cc4fc18016e6f050e025f41 \
-    --hash=sha256:cc59bc4423742fd71ad227122eb0dd44db51efb3dc4095b45ac9a08c770096af
-filelock==3.13.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
-idna==3.6 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+exceptiongroup==1.2.1 ; python_full_version >= "3.9.0" and python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
+execnet==2.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:26dee51f1b80cebd6d0ca8e74dd8745419761d3bef34163928cbebbdc4749fdc \
+    --hash=sha256:5189b52c6121c24feae288166ab41b32549c7e2348652736540b9e6e7d4e72e3
+filelock==3.13.4 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
+idna==3.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
 iniconfig==2.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-jinja2==3.1.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-markupsafe==2.1.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+jinja2==3.1.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+markupsafe==2.1.5 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
 mock==5.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:18c694e5ae8a208cdb3d2c20a993ca1a7b0efa258c247a1e565150f477f83744 \
     --hash=sha256:5e96aad5ccda4718e0a229ed94b2024df75cc2d55575ba5762d31f5767b8767d
 mypy-extensions==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-mypy==1.8.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02 \
-    --hash=sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66 \
-    --hash=sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8 \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6 \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a \
-    --hash=sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592 \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+mypy==1.9.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
 nodeenv==1.8.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
-nox==2023.4.22 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891 \
-    --hash=sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f
+nox==2024.4.15 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:6492236efa15a460ecb98e7b67562a28b70da006ab0be164e8821177577c0565 \
+    --hash=sha256:ecf6700199cdfa9e5ea0a41ff5e6ef4641d09508eda6edb89d9987864115817f
 outcome==1.3.0.post0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:9dcf02e65f2971b80047b377468e72a268e15c0af3cf1238e6ff14f7f91143b8 \
     --hash=sha256:e771c5ce06d1415e356078d3bdd68523f284b4ce5419828922b6871e65eda82b
-packaging==23.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-platformdirs==4.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
-pluggy==1.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12 \
-    --hash=sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7
-pycparser==2.21 ; python_full_version >= "3.9.0" and os_name == "nt" and implementation_name != "pypy" and python_version < "3.13" \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
-pydantic-core==2.14.6 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:00646784f6cd993b1e1c0e7b0fdcbccc375d539db95555477771c27555e3c556 \
-    --hash=sha256:00b1087dabcee0b0ffd104f9f53d7d3eaddfaa314cdd6726143af6bc713aa27e \
-    --hash=sha256:0348b1dc6b76041516e8a854ff95b21c55f5a411c3297d2ca52f5528e49d8411 \
-    --hash=sha256:036137b5ad0cb0004c75b579445a1efccd072387a36c7f217bb8efd1afbe5245 \
-    --hash=sha256:095b707bb287bfd534044166ab767bec70a9bba3175dcdc3371782175c14e43c \
-    --hash=sha256:0c08de15d50fa190d577e8591f0329a643eeaed696d7771760295998aca6bc66 \
-    --hash=sha256:1302a54f87b5cd8528e4d6d1bf2133b6aa7c6122ff8e9dc5220fbc1e07bffebd \
-    --hash=sha256:172de779e2a153d36ee690dbc49c6db568d7b33b18dc56b69a7514aecbcf380d \
-    --hash=sha256:1b027c86c66b8627eb90e57aee1f526df77dc6d8b354ec498be9a757d513b92b \
-    --hash=sha256:1ce830e480f6774608dedfd4a90c42aac4a7af0a711f1b52f807130c2e434c06 \
-    --hash=sha256:1fd0c1d395372843fba13a51c28e3bb9d59bd7aebfeb17358ffaaa1e4dbbe948 \
-    --hash=sha256:23598acb8ccaa3d1d875ef3b35cb6376535095e9405d91a3d57a8c7db5d29341 \
-    --hash=sha256:24368e31be2c88bd69340fbfe741b405302993242ccb476c5c3ff48aeee1afe0 \
-    --hash=sha256:26a92ae76f75d1915806b77cf459811e772d8f71fd1e4339c99750f0e7f6324f \
-    --hash=sha256:27e524624eace5c59af499cd97dc18bb201dc6a7a2da24bfc66ef151c69a5f2a \
-    --hash=sha256:2b8719037e570639e6b665a4050add43134d80b687288ba3ade18b22bbb29dd2 \
-    --hash=sha256:2c5bcf3414367e29f83fd66f7de64509a8fd2368b1edf4351e862910727d3e51 \
-    --hash=sha256:2dbe357bc4ddda078f79d2a36fc1dd0494a7f2fad83a0a684465b6f24b46fe80 \
-    --hash=sha256:2f5fa187bde8524b1e37ba894db13aadd64faa884657473b03a019f625cee9a8 \
-    --hash=sha256:2f6ffc6701a0eb28648c845f4945a194dc7ab3c651f535b81793251e1185ac3d \
-    --hash=sha256:314ccc4264ce7d854941231cf71b592e30d8d368a71e50197c905874feacc8a8 \
-    --hash=sha256:36026d8f99c58d7044413e1b819a67ca0e0b8ebe0f25e775e6c3d1fabb3c38fb \
-    --hash=sha256:36099c69f6b14fc2c49d7996cbf4f87ec4f0e66d1c74aa05228583225a07b590 \
-    --hash=sha256:36fa402dcdc8ea7f1b0ddcf0df4254cc6b2e08f8cd80e7010d4c4ae6e86b2a87 \
-    --hash=sha256:370ffecb5316ed23b667d99ce4debe53ea664b99cc37bfa2af47bc769056d534 \
-    --hash=sha256:3860c62057acd95cc84044e758e47b18dcd8871a328ebc8ccdefd18b0d26a21b \
-    --hash=sha256:399ac0891c284fa8eb998bcfa323f2234858f5d2efca3950ae58c8f88830f145 \
-    --hash=sha256:3a0b5db001b98e1c649dd55afa928e75aa4087e587b9524a4992316fa23c9fba \
-    --hash=sha256:3dcf1978be02153c6a31692d4fbcc2a3f1db9da36039ead23173bc256ee3b91b \
-    --hash=sha256:4241204e4b36ab5ae466ecec5c4c16527a054c69f99bba20f6f75232a6a534e2 \
-    --hash=sha256:438027a975cc213a47c5d70672e0d29776082155cfae540c4e225716586be75e \
-    --hash=sha256:43e166ad47ba900f2542a80d83f9fc65fe99eb63ceec4debec160ae729824052 \
-    --hash=sha256:478e9e7b360dfec451daafe286998d4a1eeaecf6d69c427b834ae771cad4b622 \
-    --hash=sha256:4ce8299b481bcb68e5c82002b96e411796b844d72b3e92a3fbedfe8e19813eab \
-    --hash=sha256:4f86f1f318e56f5cbb282fe61eb84767aee743ebe32c7c0834690ebea50c0a6b \
-    --hash=sha256:55a23dcd98c858c0db44fc5c04fc7ed81c4b4d33c653a7c45ddaebf6563a2f66 \
-    --hash=sha256:599c87d79cab2a6a2a9df4aefe0455e61e7d2aeede2f8577c1b7c0aec643ee8e \
-    --hash=sha256:5aa90562bc079c6c290f0512b21768967f9968e4cfea84ea4ff5af5d917016e4 \
-    --hash=sha256:64634ccf9d671c6be242a664a33c4acf12882670b09b3f163cd00a24cffbd74e \
-    --hash=sha256:667aa2eac9cd0700af1ddb38b7b1ef246d8cf94c85637cbb03d7757ca4c3fdec \
-    --hash=sha256:6a31d98c0d69776c2576dda4b77b8e0c69ad08e8b539c25c7d0ca0dc19a50d6c \
-    --hash=sha256:6af4b3f52cc65f8a0bc8b1cd9676f8c21ef3e9132f21fed250f6958bd7223bed \
-    --hash=sha256:6c8edaea3089bf908dd27da8f5d9e395c5b4dc092dbcce9b65e7156099b4b937 \
-    --hash=sha256:71d72ca5eaaa8d38c8df16b7deb1a2da4f650c41b58bb142f3fb75d5ad4a611f \
-    --hash=sha256:72f9a942d739f09cd42fffe5dc759928217649f070056f03c70df14f5770acf9 \
-    --hash=sha256:747265448cb57a9f37572a488a57d873fd96bf51e5bb7edb52cfb37124516da4 \
-    --hash=sha256:75ec284328b60a4e91010c1acade0c30584f28a1f345bc8f72fe8b9e46ec6a96 \
-    --hash=sha256:78d0768ee59baa3de0f4adac9e3748b4b1fffc52143caebddfd5ea2961595277 \
-    --hash=sha256:78ee52ecc088c61cce32b2d30a826f929e1708f7b9247dc3b921aec367dc1b23 \
-    --hash=sha256:7be719e4d2ae6c314f72844ba9d69e38dff342bc360379f7c8537c48e23034b7 \
-    --hash=sha256:7e1f4744eea1501404b20b0ac059ff7e3f96a97d3e3f48ce27a139e053bb370b \
-    --hash=sha256:7e90d6cc4aad2cc1f5e16ed56e46cebf4877c62403a311af20459c15da76fd91 \
-    --hash=sha256:7ebe3416785f65c28f4f9441e916bfc8a54179c8dea73c23023f7086fa601c5d \
-    --hash=sha256:7f41533d7e3cf9520065f610b41ac1c76bc2161415955fbcead4981b22c7611e \
-    --hash=sha256:7f5025db12fc6de7bc1104d826d5aee1d172f9ba6ca936bf6474c2148ac336c1 \
-    --hash=sha256:86c963186ca5e50d5c8287b1d1c9d3f8f024cbe343d048c5bd282aec2d8641f2 \
-    --hash=sha256:86ce5fcfc3accf3a07a729779d0b86c5d0309a4764c897d86c11089be61da160 \
-    --hash=sha256:8a14c192c1d724c3acbfb3f10a958c55a2638391319ce8078cb36c02283959b9 \
-    --hash=sha256:8b93785eadaef932e4fe9c6e12ba67beb1b3f1e5495631419c784ab87e975670 \
-    --hash=sha256:8ed1af8692bd8d2a29d702f1a2e6065416d76897d726e45a1775b1444f5928a7 \
-    --hash=sha256:92879bce89f91f4b2416eba4429c7b5ca22c45ef4a499c39f0c5c69257522c7c \
-    --hash=sha256:94fc0e6621e07d1e91c44e016cc0b189b48db053061cc22d6298a611de8071bb \
-    --hash=sha256:982487f8931067a32e72d40ab6b47b1628a9c5d344be7f1a4e668fb462d2da42 \
-    --hash=sha256:9862bf828112e19685b76ca499b379338fd4c5c269d897e218b2ae8fcb80139d \
-    --hash=sha256:99b14dbea2fdb563d8b5a57c9badfcd72083f6006caf8e126b491519c7d64ca8 \
-    --hash=sha256:9c6a5c79b28003543db3ba67d1df336f253a87d3112dac3a51b94f7d48e4c0e1 \
-    --hash=sha256:a19b794f8fe6569472ff77602437ec4430f9b2b9ec7a1105cfd2232f9ba355e6 \
-    --hash=sha256:a306cdd2ad3a7d795d8e617a58c3a2ed0f76c8496fb7621b6cd514eb1532cae8 \
-    --hash=sha256:a3dde6cac75e0b0902778978d3b1646ca9f438654395a362cb21d9ad34b24acf \
-    --hash=sha256:a874f21f87c485310944b2b2734cd6d318765bcbb7515eead33af9641816506e \
-    --hash=sha256:a983cca5ed1dd9a35e9e42ebf9f278d344603bfcb174ff99a5815f953925140a \
-    --hash=sha256:aca48506a9c20f68ee61c87f2008f81f8ee99f8d7f0104bff3c47e2d148f89d9 \
-    --hash=sha256:b2602177668f89b38b9f84b7b3435d0a72511ddef45dc14446811759b82235a1 \
-    --hash=sha256:b3e5fe4538001bb82e2295b8d2a39356a84694c97cb73a566dc36328b9f83b40 \
-    --hash=sha256:b6ca36c12a5120bad343eef193cc0122928c5c7466121da7c20f41160ba00ba2 \
-    --hash=sha256:b89f4477d915ea43b4ceea6756f63f0288941b6443a2b28c69004fe07fde0d0d \
-    --hash=sha256:b9a9d92f10772d2a181b5ca339dee066ab7d1c9a34ae2421b2a52556e719756f \
-    --hash=sha256:c99462ffc538717b3e60151dfaf91125f637e801f5ab008f81c402f1dff0cd0f \
-    --hash=sha256:cb92f9061657287eded380d7dc455bbf115430b3aa4741bdc662d02977e7d0af \
-    --hash=sha256:cdee837710ef6b56ebd20245b83799fce40b265b3b406e51e8ccc5b85b9099b7 \
-    --hash=sha256:cf10b7d58ae4a1f07fccbf4a0a956d705356fea05fb4c70608bb6fa81d103cda \
-    --hash=sha256:d15687d7d7f40333bd8266f3814c591c2e2cd263fa2116e314f60d82086e353a \
-    --hash=sha256:d5c28525c19f5bb1e09511669bb57353d22b94cf8b65f3a8d141c389a55dec95 \
-    --hash=sha256:d5f916acf8afbcab6bacbb376ba7dc61f845367901ecd5e328fc4d4aef2fcab0 \
-    --hash=sha256:dab03ed811ed1c71d700ed08bde8431cf429bbe59e423394f0f4055f1ca0ea60 \
-    --hash=sha256:db453f2da3f59a348f514cfbfeb042393b68720787bbef2b4c6068ea362c8149 \
-    --hash=sha256:de2a0645a923ba57c5527497daf8ec5df69c6eadf869e9cd46e86349146e5975 \
-    --hash=sha256:dea7fcd62915fb150cdc373212141a30037e11b761fbced340e9db3379b892d4 \
-    --hash=sha256:dfcbebdb3c4b6f739a91769aea5ed615023f3c88cb70df812849aef634c25fbe \
-    --hash=sha256:dfcebb950aa7e667ec226a442722134539e77c575f6cfaa423f24371bb8d2e94 \
-    --hash=sha256:e0641b506486f0b4cd1500a2a65740243e8670a2549bb02bc4556a83af84ae03 \
-    --hash=sha256:e33b0834f1cf779aa839975f9d8755a7c2420510c0fa1e9fa0497de77cd35d2c \
-    --hash=sha256:e4ace1e220b078c8e48e82c081e35002038657e4b37d403ce940fa679e57113b \
-    --hash=sha256:e4cf2d5829f6963a5483ec01578ee76d329eb5caf330ecd05b3edd697e7d768a \
-    --hash=sha256:e574de99d735b3fc8364cba9912c2bec2da78775eba95cbb225ef7dda6acea24 \
-    --hash=sha256:e646c0e282e960345314f42f2cea5e0b5f56938c093541ea6dbf11aec2862391 \
-    --hash=sha256:e8a5ac97ea521d7bde7621d86c30e86b798cdecd985723c4ed737a2aa9e77d0c \
-    --hash=sha256:eedf97be7bc3dbc8addcef4142f4b4164066df0c6f36397ae4aaed3eb187d8ab \
-    --hash=sha256:ef633add81832f4b56d3b4c9408b43d530dfca29e68fb1b797dcb861a2c734cd \
-    --hash=sha256:f27207e8ca3e5e021e2402ba942e5b4c629718e665c81b8b306f3c8b1ddbb786 \
-    --hash=sha256:f85f3843bdb1fe80e8c206fe6eed7a1caeae897e496542cee499c374a85c6e08 \
-    --hash=sha256:f8e81e4b55930e5ffab4a68db1af431629cf2e4066dbdbfef65348b8ab804ea8 \
-    --hash=sha256:f96ae96a060a8072ceff4cfde89d261837b4294a4f28b84a28765470d502ccc6 \
-    --hash=sha256:fd9e98b408384989ea4ab60206b8e100d8687da18b5c813c11e92fd8212a98e0 \
-    --hash=sha256:ffff855100bc066ff2cd3aa4a60bc9534661816b110f0243e59503ec2df38421
-pydantic==2.5.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:b3ef57c62535b0941697cce638c08900d87fcb67e29cfa99e8a68f747f393f7a \
-    --hash=sha256:d0caf5954bee831b6bfe7e338c32b9e30c85dfe080c843680783ac2b631673b4
-pyright==1.1.343 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:75a0d24e8227328198bdfa1f4904ce66b78c2bacf49c269d9e6e3b174b026225 \
-    --hash=sha256:871e122d74003e8e5fddb17867220b06ee892de61fa967ca7ca031acdc176738
-pytest-cov==4.1.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
-pytest-sugar==0.9.7 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:8cb5a4e5f8bbcd834622b0235db9e50432f4cbd71fef55b467fe44e43701e062 \
-    --hash=sha256:f1e74c1abfa55f7241cf7088032b6e378566f16b938f3f08905e2cf4494edd46
-pytest-timeout==2.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:3b0b95dabf3cb50bac9ef5ca912fa0cfc286526af17afc806824df20c2f72c90 \
-    --hash=sha256:bde531e096466f49398a59f2dde76fa78429a09a12411466f88a07213e220de2
+packaging==24.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+platformdirs==4.2.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+pluggy==1.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
+pycparser==2.22 ; os_name == "nt" and implementation_name != "pypy" and python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pydantic-core==2.18.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+pydantic==2.7.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
+pyright==1.1.359 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
+    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
+pytest-cov==5.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
+pytest-sugar==1.0.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a \
+    --hash=sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd
+pytest-timeout==2.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:12397729125c6ecbdaca01035b9e5239d4db97352320af155b3f5de1ba5165d9 \
+    --hash=sha256:68188cb703edfc6a18fad98dc25a3c61e9f24d644b0b70f33af545219fc7813e
 pytest-xdist==3.5.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:cbb36f3d67e0c478baa57fa4edc8843887e0f6cfc42d677530a36d7472b32d8a \
     --hash=sha256:d075629c7e00b611df89f490a5063944bee7a4362a5ff11c7cc7824a03dfce24
-pytest==7.4.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:0d009c083ea859a71b76adf7c1d502e4bc170b80a8ef002da5806527b9591fac \
-    --hash=sha256:d989d136982de4e3b29dabcc838ad581c64e8ed52c11fbe86ddebd9da0818cd5
-setuptools==69.0.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
-sniffio==1.3.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
-    --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
+pytest==8.1.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
+    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
+setuptools==69.5.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
+sniffio==1.3.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
+    --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
 sortedcontainers==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:25caa5a06cc30b6b83d11423433f65d1f9d76c4c6a0c90e3379eaa43b9bfdb88 \
     --hash=sha256:a163dcaede0f1c021485e957a39245190e74249897e2ae4b2aa38595db237ee0
 termcolor==2.4.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63 \
     --hash=sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a
 tomli==2.0.1 ; python_full_version >= "3.9.0" and python_version < "3.13" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-trio==0.23.2 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:5a0b566fa5d50cf231cfd6b08f3b03aa4179ff004b8f3144059587039e2b26d3 \
-    --hash=sha256:da1d35b9a2b17eb32cae2e763b16551f9aa6703634735024e32f325c9285069e
-typing-extensions==4.9.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-virtualenv==20.25.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
-    --hash=sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3 \
-    --hash=sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b
+trio==0.25.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:9b41f5993ad2c0e5f62d0acca320ec657fdb6b2a2c22b8c7aed6caf154475c4e \
+    --hash=sha256:e6458efe29cc543e557a91e614e2b51710eba2961669329ce9c862d50c6e8e81
+typing-extensions==4.11.0 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+virtualenv==20.25.3 ; python_full_version >= "3.9.0" and python_version < "3.13" \
+    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
+    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
```

### Comparing `alluka-0.1.4/docs/usage.md` & `alluka-0.1.5/docs/usage.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/mkdocs.yml` & `alluka-0.1.5/mkdocs.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,21 +16,21 @@
       danger: octicons/zap-16
       bug: octicons/bug-16
       example: octicons/beaker-16
       quote: octicons/quote-16
   palette:
     - media: "(prefers-color-scheme: light)"
       scheme: default
-      primary: cyan
+      primary: pink
       toggle:
         icon: material/lightbulb
         name: Switch to dark mode
     - media: "(prefers-color-scheme: dark)"
       scheme: slate
-      primary: cyan
+      primary: pink
       toggle:
         icon: material/lightbulb
         name: Switch to light mode
 
 markdown_extensions:
   - admonition
   - pymdownx.details
```

### Comparing `alluka-0.1.4/noxfile.py` & `alluka-0.1.5/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/piped/.github/workflows/freeze-for-pr.yml` & `alluka-0.1.5/piped/.github/workflows/freeze-for-pr.yml`

 * *Files 16% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     paths: ["piped", "pyproject.toml", "requirements.in", "bot/requirements.in", "dev-requirements/*.in", "!dev-requirements/constraints.in", "python/base-requirements/*.in", "!python/base-requirements/constraints.in"]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/.github/workflows/lint.yml` & `alluka-0.1.5/piped/github/actions/type-check.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-name: Lint
+name: Type check
 
 concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
+  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 on:
   push:
     branches:
       - master
   pull_request:
     branches:
       - master
   schedule:
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
-  lint:
+  type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python {{ DEFAULT_PY_VER }}
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
-      - name: Lint markup
-        run: python -m nox -s verify-markup
-
-      - name: Check spelling
-        run: python -m nox -s spell-check
-
-      - name: Lint with flake8
-        run: python -m nox -s flake8
+      - name: Run type checker
+        run: python -m nox -s type-check
```

### Comparing `alluka-0.1.4/piped/.github/workflows/reformat.yml` & `alluka-0.1.5/piped/github/actions/reformat.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 name: Reformat PR code
 
 concurrency:
-  group: ${{ github.workflow }}-${{ github.ref }}
+  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
 
 jobs:
   reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python {{ DEFAULT_PY_VER }}
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Reformat
         run: python -m nox -s reformat bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/.github/workflows/resync-piped.yml` & `alluka-0.1.5/.github/workflows/reformat.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,40 @@
-name: Resync piped
+name: Reformat PR code
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
-    paths: ["github/actions/*", "pyproject.toml"]
 
 jobs:
-  resync-piped:
+  reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python 3.9
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "3.9"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
 
-      - name: Resync Piped
-        run: python -m nox -s copy-piped bot-package-diff
+      - name: Reformat
+        run: python -m nox -s reformat bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/.github/workflows/type-check.yml` & `alluka-0.1.5/piped/.github/workflows/type-check.yml`

 * *Files 27% similar despite different names*

```diff
@@ -16,20 +16,20 @@
   workflow_dispatch:
 
 jobs:
   type-check:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./python/base-requirements/nox.txt
```

### Comparing `alluka-0.1.4/piped/.github/workflows/update-licence.yml` & `alluka-0.1.5/piped/github/actions/resync-piped.yml`

 * *Files 23% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-name: Update licence
+name: Resync piped
+
+concurrency:
+  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
+  cancel-in-progress: true
 
 on:
-  schedule:
-    - cron: "0 7 1 1 *"
-  workflow_dispatch:
+  pull_request:
+    branches:
+      - master
+    paths: [{{ FILTERS | map("quoted") | join(", ") }}]
 
 jobs:
-  update-licence:
+  resync-piped:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python {{ DEFAULT_PY_VER }}
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
-      - name: Update licence
-        run: python -m nox -s update-licence
+      - name: Resync Piped
+        run: python -m nox -s copy-piped bot-package-diff
 
-      - name: Create Pull Request
-        uses: peter-evans/create-pull-request@153407881ec5c347639a548ade7d8ad1d6740e38
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
-          author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
-          branch: task/update-licence
-          commit-message: Update licence
-          committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
-          title: Update licence
-          token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
+          name: gogo.patch
+          path: gogo.patch
+
+      - name: Check diff file
+        run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/.github/workflows/upgrade-locks.yml` & `alluka-0.1.5/piped/github/actions/upgrade-locks.yml`

 * *Files 20% similar despite different names*

```diff
@@ -6,33 +6,33 @@
   workflow_dispatch:
 
 jobs:
   upgrade-deps:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python {{ DEFAULT_PY_VER }}
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "3.11"
+          python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r ./python/base-requirements/nox.txt
+          python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks
 
       - name: Create Pull Request
-        uses: peter-evans/create-pull-request@153407881ec5c347639a548ade7d8ad1d6740e38
+        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
         with:
-          author: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
+          author: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           branch: task/upgrade-deps
           commit-message: Upgrade dependency locks
-          committer: "always-on-duty[bot] <120557446+always-on-duty[bot]@users.noreply.github.com>"
+          committer: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
           title: Upgrade dependency locks
-          token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}
+          {% raw %}token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}{% endraw %}
```

### Comparing `alluka-0.1.4/piped/.github/workflows/verify-locks.yml` & `alluka-0.1.5/piped/.github/workflows/verify-locks.yml`

 * *Files 12% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     paths: ["bot/requirements.txt", "dev-requirements/*.txt", "python/base-requirements/*.txt"]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python 3.11
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r ./python/base-requirements/nox.txt
```

### Comparing `alluka-0.1.4/piped/.gitignore` & `alluka-0.1.5/piped/.gitignore`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/piped/LICENSE` & `alluka-0.1.5/piped/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2020-2023, Faster Speeding
+Copyright (c) 2020-2024, Faster Speeding
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/piped/bot/main.py` & `alluka-0.1.5/piped/bot/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -182,16 +182,23 @@
 
 class _Tokens:
     """Index of the Github API tokens this application has authorised."""
 
     __slots__ = ("_installation_tokens", "_private_key")
 
     def __init__(self) -> None:
+        private_key = os.environ["PRIVATE_KEY"].strip()
+        if private_key.startswith("-"):
+            private_key = private_key.encode()
+
+        else:
+            private_key = pathlib.Path(private_key).read_bytes()
+
         self._installation_tokens: dict[int, tuple[datetime.datetime, str]] = {}
-        self._private_key = jwt.jwk_from_pem(os.environ["PRIVATE_KEY"].encode())
+        self._private_key = jwt.jwk_from_pem(private_key)
 
     def app_token(self, *, on_gen: collections.Callable[[str], None] | None = None) -> str:
         """Generate an application app token.
 
         !!! warning
             This cannot does not provide authorization for repos or
             organisations the application is authorised in.
@@ -563,15 +570,16 @@
 async def _on_shutdown():
     assert isinstance(app.state.index, _ProcessingIndex)
     assert isinstance(app.state.http, httpx.AsyncClient)
     await app.state.index.close()
     await app.state.http.aclose()
 
 
-app = fastapi.FastAPI(middleware=[starlette.middleware.Middleware(AuthMiddleware)])
+auth = starlette.middleware.Middleware(AuthMiddleware)  # pyright: ignore[reportCallIssue, reportArgumentType]
+app = fastapi.FastAPI(middleware=[auth])
 app.router.on_startup.append(_on_startup)
 app.router.on_shutdown.append(_on_shutdown)
 
 
 @app.post("/webhook")
 async def post_webhook(
     body: dict[str, typing.Any],
```

### Comparing `alluka-0.1.4/piped/bot/requirements.txt` & `alluka-0.1.5/piped/bot/requirements.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # To update, run:
 #
 #    pip-compile-cross-platform bot/requirements.in --output-file bot/requirements.txt --min-python-version 3.9
 #
 annotated-types==0.6.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
     --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-anyio==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:745843b39e829e108e518c489b31dc757de7d2131d53fac32bd8df268227bfee \
-    --hash=sha256:e1875bb4b4e2de1669f4bc7869b6d3f54231cdced71605e6e64c9be77e3be50f
-asgiref==3.7.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
-certifi==2023.11.17 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
-cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
+anyio==4.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8 \
+    --hash=sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6
+asgiref==3.8.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" and platform_python_implementation != "PyPy" \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
     --hash=sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743 \
@@ -71,203 +71,186 @@
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-cryptography==41.0.7 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:079b85658ea2f59c4f43b70f8119a52414cdb7be34da5d019a77bf96d473b960 \
-    --hash=sha256:09616eeaef406f99046553b8a40fbf8b1e70795a91885ba4c96a70793de5504a \
-    --hash=sha256:13f93ce9bea8016c253b34afc6bd6a75993e5c40672ed5405a9c832f0d4a00bc \
-    --hash=sha256:37a138589b12069efb424220bf78eac59ca68b95696fc622b6ccc1c0a197204a \
-    --hash=sha256:3c78451b78313fa81607fa1b3f1ae0a5ddd8014c38a02d9db0616133987b9cdf \
-    --hash=sha256:43f2552a2378b44869fe8827aa19e69512e3245a219104438692385b0ee119d1 \
-    --hash=sha256:48a0476626da912a44cc078f9893f292f0b3e4c739caf289268168d8f4702a39 \
-    --hash=sha256:49f0805fc0b2ac8d4882dd52f4a3b935b210935d500b6b805f321addc8177406 \
-    --hash=sha256:5429ec739a29df2e29e15d082f1d9ad683701f0ec7709ca479b3ff2708dae65a \
-    --hash=sha256:5a1b41bc97f1ad230a41657d9155113c7521953869ae57ac39ac7f1bb471469a \
-    --hash=sha256:68a2dec79deebc5d26d617bfdf6e8aab065a4f34934b22d3b5010df3ba36612c \
-    --hash=sha256:7a698cb1dac82c35fcf8fe3417a3aaba97de16a01ac914b89a0889d364d2f6be \
-    --hash=sha256:841df4caa01008bad253bce2a6f7b47f86dc9f08df4b433c404def869f590a15 \
-    --hash=sha256:90452ba79b8788fa380dfb587cca692976ef4e757b194b093d845e8d99f612f2 \
-    --hash=sha256:928258ba5d6f8ae644e764d0f996d61a8777559f72dfeb2eea7e2fe0ad6e782d \
-    --hash=sha256:af03b32695b24d85a75d40e1ba39ffe7db7ffcb099fe507b39fd41a565f1b157 \
-    --hash=sha256:b640981bf64a3e978a56167594a0e97db71c89a479da8e175d8bb5be5178c003 \
-    --hash=sha256:c5ca78485a255e03c32b513f8c2bc39fedb7f5c5f8535545bdc223a03b24f248 \
-    --hash=sha256:c7f3201ec47d5207841402594f1d7950879ef890c0c495052fa62f58283fde1a \
-    --hash=sha256:d5ec85080cce7b0513cfd233914eb8b7bbd0633f1d1703aa28d1dd5a72f678ec \
-    --hash=sha256:d6c391c021ab1f7a82da5d8d0b3cee2f4b2c455ec86c8aebbc84837a631ff309 \
-    --hash=sha256:e3114da6d7f95d2dee7d3f4eec16dacff819740bbab931aff8648cb13c5ff5e7 \
-    --hash=sha256:f983596065a18a2183e7f79ab3fd4c475205b839e02cbc0efbbf9666c4b3083d
-exceptiongroup==1.2.0 ; python_version >= "3.9" and python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
-fastapi==0.108.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5056e504ac6395bf68493d71fcfc5352fdbd5fda6f88c21f6420d80d81163296 \
-    --hash=sha256:8c7bc6d315da963ee4cdb605557827071a9a7f95aeb8fcdd3bde48cdc8764dd7
+cryptography==42.0.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
+exceptiongroup==1.2.1 ; python_version >= "3.9" and python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
+fastapi==0.110.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:239403f2c0a3dda07a9420f95157a7f014ddb2b770acdbc984f9bdf3ead7afdb \
+    --hash=sha256:b53d673652da3b65e8cd787ad214ec0fe303cad00d2b529b86ce7db13f17518d
 h11==0.14.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d \
     --hash=sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761
 h2==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03a46bcf682256c95b5fd9e9a99c1323584c3eec6440d379b9903d709476bc6d \
     --hash=sha256:a83aca08fbe7aacb79fec788c9c0bac936343560ed9ec18b82a13a12c28d2abb
 hpack==4.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c \
     --hash=sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095
-httpcore==1.0.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:096cc05bca73b8e459a1fc3dcf585148f63e534eae4339559c9b8a8d6399acc7 \
-    --hash=sha256:9fc092e4799b26174648e54b74ed5f683132a464e95643b226e00c2ed2fa6535
-httpx[http2]==0.26.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:451b55c30d5185ea6b23c2c793abf9bb237d2a7dfb901ced6ff69ad37ec1dfaf \
-    --hash=sha256:8915f5a3627c4d47b73e8202457cb28f1266982d1159bd5779d86a80c0eab1cd
+httpcore==1.0.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:34a38e2f9291467ee3b44e89dd52615370e152954ba21721378a87b2960f7a61 \
+    --hash=sha256:421f18bac248b25d310f3cacd198d55b8e6125c107797b609ff9b7a6ba7991b5
+httpx[http2]==0.27.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:71d5465162c13681bff01ad59b2cc68dd838ea1f10e51574bac27103f00c91a5 \
+    --hash=sha256:a0cb88a46f32dc874e04ee956e4c2764aba2aa228f650b06788ba6bda2962ab5
 hyperframe==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0ec6bafd80d8ad2195c4f03aacba3a8265e57bc4cff261e802bf39970ed02a15 \
     --hash=sha256:ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914
-idna==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
 jwt==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:61c9170f92e736b530655e75374681d4fcca9cfa8763ab42be57353b2b203494
-pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
-pydantic-core==2.14.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:00646784f6cd993b1e1c0e7b0fdcbccc375d539db95555477771c27555e3c556 \
-    --hash=sha256:00b1087dabcee0b0ffd104f9f53d7d3eaddfaa314cdd6726143af6bc713aa27e \
-    --hash=sha256:0348b1dc6b76041516e8a854ff95b21c55f5a411c3297d2ca52f5528e49d8411 \
-    --hash=sha256:036137b5ad0cb0004c75b579445a1efccd072387a36c7f217bb8efd1afbe5245 \
-    --hash=sha256:095b707bb287bfd534044166ab767bec70a9bba3175dcdc3371782175c14e43c \
-    --hash=sha256:0c08de15d50fa190d577e8591f0329a643eeaed696d7771760295998aca6bc66 \
-    --hash=sha256:1302a54f87b5cd8528e4d6d1bf2133b6aa7c6122ff8e9dc5220fbc1e07bffebd \
-    --hash=sha256:172de779e2a153d36ee690dbc49c6db568d7b33b18dc56b69a7514aecbcf380d \
-    --hash=sha256:1b027c86c66b8627eb90e57aee1f526df77dc6d8b354ec498be9a757d513b92b \
-    --hash=sha256:1ce830e480f6774608dedfd4a90c42aac4a7af0a711f1b52f807130c2e434c06 \
-    --hash=sha256:1fd0c1d395372843fba13a51c28e3bb9d59bd7aebfeb17358ffaaa1e4dbbe948 \
-    --hash=sha256:23598acb8ccaa3d1d875ef3b35cb6376535095e9405d91a3d57a8c7db5d29341 \
-    --hash=sha256:24368e31be2c88bd69340fbfe741b405302993242ccb476c5c3ff48aeee1afe0 \
-    --hash=sha256:26a92ae76f75d1915806b77cf459811e772d8f71fd1e4339c99750f0e7f6324f \
-    --hash=sha256:27e524624eace5c59af499cd97dc18bb201dc6a7a2da24bfc66ef151c69a5f2a \
-    --hash=sha256:2b8719037e570639e6b665a4050add43134d80b687288ba3ade18b22bbb29dd2 \
-    --hash=sha256:2c5bcf3414367e29f83fd66f7de64509a8fd2368b1edf4351e862910727d3e51 \
-    --hash=sha256:2dbe357bc4ddda078f79d2a36fc1dd0494a7f2fad83a0a684465b6f24b46fe80 \
-    --hash=sha256:2f5fa187bde8524b1e37ba894db13aadd64faa884657473b03a019f625cee9a8 \
-    --hash=sha256:2f6ffc6701a0eb28648c845f4945a194dc7ab3c651f535b81793251e1185ac3d \
-    --hash=sha256:314ccc4264ce7d854941231cf71b592e30d8d368a71e50197c905874feacc8a8 \
-    --hash=sha256:36026d8f99c58d7044413e1b819a67ca0e0b8ebe0f25e775e6c3d1fabb3c38fb \
-    --hash=sha256:36099c69f6b14fc2c49d7996cbf4f87ec4f0e66d1c74aa05228583225a07b590 \
-    --hash=sha256:36fa402dcdc8ea7f1b0ddcf0df4254cc6b2e08f8cd80e7010d4c4ae6e86b2a87 \
-    --hash=sha256:370ffecb5316ed23b667d99ce4debe53ea664b99cc37bfa2af47bc769056d534 \
-    --hash=sha256:3860c62057acd95cc84044e758e47b18dcd8871a328ebc8ccdefd18b0d26a21b \
-    --hash=sha256:399ac0891c284fa8eb998bcfa323f2234858f5d2efca3950ae58c8f88830f145 \
-    --hash=sha256:3a0b5db001b98e1c649dd55afa928e75aa4087e587b9524a4992316fa23c9fba \
-    --hash=sha256:3dcf1978be02153c6a31692d4fbcc2a3f1db9da36039ead23173bc256ee3b91b \
-    --hash=sha256:4241204e4b36ab5ae466ecec5c4c16527a054c69f99bba20f6f75232a6a534e2 \
-    --hash=sha256:438027a975cc213a47c5d70672e0d29776082155cfae540c4e225716586be75e \
-    --hash=sha256:43e166ad47ba900f2542a80d83f9fc65fe99eb63ceec4debec160ae729824052 \
-    --hash=sha256:478e9e7b360dfec451daafe286998d4a1eeaecf6d69c427b834ae771cad4b622 \
-    --hash=sha256:4ce8299b481bcb68e5c82002b96e411796b844d72b3e92a3fbedfe8e19813eab \
-    --hash=sha256:4f86f1f318e56f5cbb282fe61eb84767aee743ebe32c7c0834690ebea50c0a6b \
-    --hash=sha256:55a23dcd98c858c0db44fc5c04fc7ed81c4b4d33c653a7c45ddaebf6563a2f66 \
-    --hash=sha256:599c87d79cab2a6a2a9df4aefe0455e61e7d2aeede2f8577c1b7c0aec643ee8e \
-    --hash=sha256:5aa90562bc079c6c290f0512b21768967f9968e4cfea84ea4ff5af5d917016e4 \
-    --hash=sha256:64634ccf9d671c6be242a664a33c4acf12882670b09b3f163cd00a24cffbd74e \
-    --hash=sha256:667aa2eac9cd0700af1ddb38b7b1ef246d8cf94c85637cbb03d7757ca4c3fdec \
-    --hash=sha256:6a31d98c0d69776c2576dda4b77b8e0c69ad08e8b539c25c7d0ca0dc19a50d6c \
-    --hash=sha256:6af4b3f52cc65f8a0bc8b1cd9676f8c21ef3e9132f21fed250f6958bd7223bed \
-    --hash=sha256:6c8edaea3089bf908dd27da8f5d9e395c5b4dc092dbcce9b65e7156099b4b937 \
-    --hash=sha256:71d72ca5eaaa8d38c8df16b7deb1a2da4f650c41b58bb142f3fb75d5ad4a611f \
-    --hash=sha256:72f9a942d739f09cd42fffe5dc759928217649f070056f03c70df14f5770acf9 \
-    --hash=sha256:747265448cb57a9f37572a488a57d873fd96bf51e5bb7edb52cfb37124516da4 \
-    --hash=sha256:75ec284328b60a4e91010c1acade0c30584f28a1f345bc8f72fe8b9e46ec6a96 \
-    --hash=sha256:78d0768ee59baa3de0f4adac9e3748b4b1fffc52143caebddfd5ea2961595277 \
-    --hash=sha256:78ee52ecc088c61cce32b2d30a826f929e1708f7b9247dc3b921aec367dc1b23 \
-    --hash=sha256:7be719e4d2ae6c314f72844ba9d69e38dff342bc360379f7c8537c48e23034b7 \
-    --hash=sha256:7e1f4744eea1501404b20b0ac059ff7e3f96a97d3e3f48ce27a139e053bb370b \
-    --hash=sha256:7e90d6cc4aad2cc1f5e16ed56e46cebf4877c62403a311af20459c15da76fd91 \
-    --hash=sha256:7ebe3416785f65c28f4f9441e916bfc8a54179c8dea73c23023f7086fa601c5d \
-    --hash=sha256:7f41533d7e3cf9520065f610b41ac1c76bc2161415955fbcead4981b22c7611e \
-    --hash=sha256:7f5025db12fc6de7bc1104d826d5aee1d172f9ba6ca936bf6474c2148ac336c1 \
-    --hash=sha256:86c963186ca5e50d5c8287b1d1c9d3f8f024cbe343d048c5bd282aec2d8641f2 \
-    --hash=sha256:86ce5fcfc3accf3a07a729779d0b86c5d0309a4764c897d86c11089be61da160 \
-    --hash=sha256:8a14c192c1d724c3acbfb3f10a958c55a2638391319ce8078cb36c02283959b9 \
-    --hash=sha256:8b93785eadaef932e4fe9c6e12ba67beb1b3f1e5495631419c784ab87e975670 \
-    --hash=sha256:8ed1af8692bd8d2a29d702f1a2e6065416d76897d726e45a1775b1444f5928a7 \
-    --hash=sha256:92879bce89f91f4b2416eba4429c7b5ca22c45ef4a499c39f0c5c69257522c7c \
-    --hash=sha256:94fc0e6621e07d1e91c44e016cc0b189b48db053061cc22d6298a611de8071bb \
-    --hash=sha256:982487f8931067a32e72d40ab6b47b1628a9c5d344be7f1a4e668fb462d2da42 \
-    --hash=sha256:9862bf828112e19685b76ca499b379338fd4c5c269d897e218b2ae8fcb80139d \
-    --hash=sha256:99b14dbea2fdb563d8b5a57c9badfcd72083f6006caf8e126b491519c7d64ca8 \
-    --hash=sha256:9c6a5c79b28003543db3ba67d1df336f253a87d3112dac3a51b94f7d48e4c0e1 \
-    --hash=sha256:a19b794f8fe6569472ff77602437ec4430f9b2b9ec7a1105cfd2232f9ba355e6 \
-    --hash=sha256:a306cdd2ad3a7d795d8e617a58c3a2ed0f76c8496fb7621b6cd514eb1532cae8 \
-    --hash=sha256:a3dde6cac75e0b0902778978d3b1646ca9f438654395a362cb21d9ad34b24acf \
-    --hash=sha256:a874f21f87c485310944b2b2734cd6d318765bcbb7515eead33af9641816506e \
-    --hash=sha256:a983cca5ed1dd9a35e9e42ebf9f278d344603bfcb174ff99a5815f953925140a \
-    --hash=sha256:aca48506a9c20f68ee61c87f2008f81f8ee99f8d7f0104bff3c47e2d148f89d9 \
-    --hash=sha256:b2602177668f89b38b9f84b7b3435d0a72511ddef45dc14446811759b82235a1 \
-    --hash=sha256:b3e5fe4538001bb82e2295b8d2a39356a84694c97cb73a566dc36328b9f83b40 \
-    --hash=sha256:b6ca36c12a5120bad343eef193cc0122928c5c7466121da7c20f41160ba00ba2 \
-    --hash=sha256:b89f4477d915ea43b4ceea6756f63f0288941b6443a2b28c69004fe07fde0d0d \
-    --hash=sha256:b9a9d92f10772d2a181b5ca339dee066ab7d1c9a34ae2421b2a52556e719756f \
-    --hash=sha256:c99462ffc538717b3e60151dfaf91125f637e801f5ab008f81c402f1dff0cd0f \
-    --hash=sha256:cb92f9061657287eded380d7dc455bbf115430b3aa4741bdc662d02977e7d0af \
-    --hash=sha256:cdee837710ef6b56ebd20245b83799fce40b265b3b406e51e8ccc5b85b9099b7 \
-    --hash=sha256:cf10b7d58ae4a1f07fccbf4a0a956d705356fea05fb4c70608bb6fa81d103cda \
-    --hash=sha256:d15687d7d7f40333bd8266f3814c591c2e2cd263fa2116e314f60d82086e353a \
-    --hash=sha256:d5c28525c19f5bb1e09511669bb57353d22b94cf8b65f3a8d141c389a55dec95 \
-    --hash=sha256:d5f916acf8afbcab6bacbb376ba7dc61f845367901ecd5e328fc4d4aef2fcab0 \
-    --hash=sha256:dab03ed811ed1c71d700ed08bde8431cf429bbe59e423394f0f4055f1ca0ea60 \
-    --hash=sha256:db453f2da3f59a348f514cfbfeb042393b68720787bbef2b4c6068ea362c8149 \
-    --hash=sha256:de2a0645a923ba57c5527497daf8ec5df69c6eadf869e9cd46e86349146e5975 \
-    --hash=sha256:dea7fcd62915fb150cdc373212141a30037e11b761fbced340e9db3379b892d4 \
-    --hash=sha256:dfcbebdb3c4b6f739a91769aea5ed615023f3c88cb70df812849aef634c25fbe \
-    --hash=sha256:dfcebb950aa7e667ec226a442722134539e77c575f6cfaa423f24371bb8d2e94 \
-    --hash=sha256:e0641b506486f0b4cd1500a2a65740243e8670a2549bb02bc4556a83af84ae03 \
-    --hash=sha256:e33b0834f1cf779aa839975f9d8755a7c2420510c0fa1e9fa0497de77cd35d2c \
-    --hash=sha256:e4ace1e220b078c8e48e82c081e35002038657e4b37d403ce940fa679e57113b \
-    --hash=sha256:e4cf2d5829f6963a5483ec01578ee76d329eb5caf330ecd05b3edd697e7d768a \
-    --hash=sha256:e574de99d735b3fc8364cba9912c2bec2da78775eba95cbb225ef7dda6acea24 \
-    --hash=sha256:e646c0e282e960345314f42f2cea5e0b5f56938c093541ea6dbf11aec2862391 \
-    --hash=sha256:e8a5ac97ea521d7bde7621d86c30e86b798cdecd985723c4ed737a2aa9e77d0c \
-    --hash=sha256:eedf97be7bc3dbc8addcef4142f4b4164066df0c6f36397ae4aaed3eb187d8ab \
-    --hash=sha256:ef633add81832f4b56d3b4c9408b43d530dfca29e68fb1b797dcb861a2c734cd \
-    --hash=sha256:f27207e8ca3e5e021e2402ba942e5b4c629718e665c81b8b306f3c8b1ddbb786 \
-    --hash=sha256:f85f3843bdb1fe80e8c206fe6eed7a1caeae897e496542cee499c374a85c6e08 \
-    --hash=sha256:f8e81e4b55930e5ffab4a68db1af431629cf2e4066dbdbfef65348b8ab804ea8 \
-    --hash=sha256:f96ae96a060a8072ceff4cfde89d261837b4294a4f28b84a28765470d502ccc6 \
-    --hash=sha256:fd9e98b408384989ea4ab60206b8e100d8687da18b5c813c11e92fd8212a98e0 \
-    --hash=sha256:ffff855100bc066ff2cd3aa4a60bc9534661816b110f0243e59503ec2df38421
-pydantic==2.5.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b3ef57c62535b0941697cce638c08900d87fcb67e29cfa99e8a68f747f393f7a \
-    --hash=sha256:d0caf5954bee831b6bfe7e338c32b9e30c85dfe080c843680783ac2b631673b4
-python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:a8df96034aae6d2d50a4ebe8216326c61c3eb64836776504fcca410e5937a3ba \
-    --hash=sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a
+pycparser==2.22 ; python_version >= "3.9" and python_version < "4.0" and platform_python_implementation != "PyPy" \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pydantic-core==2.18.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+pydantic==2.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
+python-dateutil==2.9.0.post0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
+python-dotenv==1.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
+    --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
-    --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
-starlette==0.32.0.post1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cd0cb10ddb49313f609cedfac62c8c12e56c7314b66d89bb077ba228bada1b09 \
-    --hash=sha256:e54e2b7e2fb06dff9eac40133583f10dfa05913f5a85bf26f427c7a40a9a3d02
+sniffio==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
+    --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
+starlette==0.37.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6fe59f29268538e5d0d182f2791a479a0c64638e6935d1c6989e63fb2699c6ee \
+    --hash=sha256:9af890290133b79fc3db55474ade20f6220a364a0402e0b556e7cd5e1e093823
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-uvicorn==0.25.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6dddbad1d7ee0f5140aba5ec138ddc9612c5109399903828b4874c9937f009c2 \
-    --hash=sha256:ce107f5d9bd02b4636001a77a4e74aab5e1e2b146868ebbad565237145af444c
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+uvicorn==0.29.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2c2aac7ff4f4365c206fd773a39bf4ebd1047c238f8b8268ad996829323473de \
+    --hash=sha256:6a69214c0b6a087462412670b3ef21224fa48cae0e452b5883e8e8bdfdd11dd0
 uvloop==0.19.0 ; python_version >= "3.9" and python_version < "4.0" and platform_system != "Windows" \
     --hash=sha256:0246f4fd1bf2bf702e06b0d45ee91677ee5c31242f39aab4ea6fe0c51aedd0fd \
     --hash=sha256:02506dc23a5d90e04d4f65c7791e65cf44bd91b37f24cfc3ef6cf2aff05dc7ec \
     --hash=sha256:13dfdf492af0aa0a0edf66807d2b465607d11c4fa48f4a1fd41cbea5b18e8e8b \
     --hash=sha256:2693049be9d36fef81741fddb3f441673ba12a34a704e7b4361efb75cf30befc \
     --hash=sha256:271718e26b3e17906b28b67314c45d19106112067205119dddbd834c2b7ce797 \
     --hash=sha256:2df95fca285a9f5bfe730e51945ffe2fa71ccbfdde3b0da5772b4ee4f2e770d5 \
```

### Comparing `alluka-0.1.4/piped/dev-requirements/flake8.in` & `alluka-0.1.5/piped/dev-requirements/flake8.in`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/piped/dev-requirements/flake8.txt` & `alluka-0.1.5/piped/dev-requirements/flake8.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,43 +3,43 @@
 # To update, run:
 #
 #    pip-compile-cross-platform dev-requirements/flake8.in --output-file dev-requirements/flake8.txt --min-python-version 3.9
 #
 astor==0.8.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
-attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
-bandit==1.7.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:36da17c67fc87579a5d20c323c8d0b1643a890a2b93f00b3d1229966624694ff \
-    --hash=sha256:72ce7bc9741374d96fb2f1c9a8960829885f1243ffde743de70a19cee353e8f3
-black==23.12.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0808494f2b2df923ffc5723ed3c7b096bd76341f6213989759287611e9837d50 \
-    --hash=sha256:1fa88a0f74e50e4487477bc0bb900c6781dbddfdfa32691e780bf854c3b4a47f \
-    --hash=sha256:25e57fd232a6d6ff3f4478a6fd0580838e47c93c83eaf1ccc92d4faf27112c4e \
-    --hash=sha256:2d9e13db441c509a3763a7a3d9a49ccc1b4e974a47be4e08ade2a228876500ec \
-    --hash=sha256:3e1b38b3135fd4c025c28c55ddfc236b05af657828a8a6abe5deec419a0b7055 \
-    --hash=sha256:3fa4be75ef2a6b96ea8d92b1587dd8cb3a35c7e3d51f0738ced0781c3aa3a5a3 \
-    --hash=sha256:4ce3ef14ebe8d9509188014d96af1c456a910d5b5cbf434a09fef7e024b3d0d5 \
-    --hash=sha256:4f0031eaa7b921db76decd73636ef3a12c942ed367d8c3841a0739412b260a54 \
-    --hash=sha256:602cfb1196dc692424c70b6507593a2b29aac0547c1be9a1d1365f0d964c353b \
-    --hash=sha256:6d1bd9c210f8b109b1762ec9fd36592fdd528485aadb3f5849b2740ef17e674e \
-    --hash=sha256:78baad24af0f033958cad29731e27363183e140962595def56423e626f4bee3e \
-    --hash=sha256:8d4df77958a622f9b5a4c96edb4b8c0034f8434032ab11077ec6c56ae9f384ba \
-    --hash=sha256:97e56155c6b737854e60a9ab1c598ff2533d57e7506d97af5481141671abf3ea \
-    --hash=sha256:9c4352800f14be5b4864016882cdba10755bd50805c95f728011bcb47a4afd59 \
-    --hash=sha256:a4d6a9668e45ad99d2f8ec70d5c8c04ef4f32f648ef39048d010b0689832ec6d \
-    --hash=sha256:a920b569dc6b3472513ba6ddea21f440d4b4c699494d2e972a1753cdc25df7b0 \
-    --hash=sha256:ae76c22bde5cbb6bfd211ec343ded2163bba7883c7bc77f6b756a1049436fbb9 \
-    --hash=sha256:b18fb2ae6c4bb63eebe5be6bd869ba2f14fd0259bda7d18a46b764d8fb86298a \
-    --hash=sha256:c04b6d9d20e9c13f43eee8ea87d44156b8505ca8a3c878773f68b4e4812a421e \
-    --hash=sha256:c88b3711d12905b74206227109272673edce0cb29f27e1385f33b0163c414bba \
-    --hash=sha256:dd15245c8b68fe2b6bd0f32c1556509d11bb33aec9b5d0866dd8e2ed3dba09c2 \
-    --hash=sha256:e0aaf6041986767a5e0ce663c7a2f0e9eaf21e6ff87a5f95cbf3675bfd4c41d2
+attrs==23.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
+bandit==1.7.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:36de50f720856ab24a24dbaa5fee2c66050ed97c1477e0a1159deab1775eab6b \
+    --hash=sha256:509f7af645bc0cd8fd4587abc1a038fc795636671ee8204d502b933aee44f381
+black==24.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d \
+    --hash=sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd \
+    --hash=sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33 \
+    --hash=sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965 \
+    --hash=sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070 \
+    --hash=sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397 \
+    --hash=sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745 \
+    --hash=sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1 \
+    --hash=sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665 \
+    --hash=sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436 \
+    --hash=sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb \
+    --hash=sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e \
+    --hash=sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6 \
+    --hash=sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702 \
+    --hash=sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8 \
+    --hash=sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8 \
+    --hash=sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3 \
+    --hash=sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad \
+    --hash=sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf \
+    --hash=sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e \
+    --hash=sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641 \
+    --hash=sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2
 click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 eradicate==2.3.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -50,17 +50,17 @@
     --hash=sha256:4c8a53eb48f23d4ef1e59293657181a3c989d0077c9952717e98a0eace43e06d
 flake8-black==0.3.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0dfbca3274777792a5bcb2af887a4cad72c72d0e86c94e08e3a3de151bb41c34 \
     --hash=sha256:fe8ea2eca98d8a504f22040d9117347f6b367458366952862ac3586e7d4eeaca
 flake8-broken-line==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:96c964336024a5030dc536a9f6fb02aa679e2d2a6b35b80a558b5136c35832a9 \
     --hash=sha256:e2c6a17f8d9a129e99c1320fce89b33843e2963871025c4c2bb7b8b8d8732a85
-flake8-builtins==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:392d5af3a0720c5a863aa93dc47f48c879081345a143fe9f20d995fe9ff5686a \
-    --hash=sha256:7ee5766d9c60e5d579dfda84e65c6d0e6c26005f6f59cb9bf722462d7987a807
+flake8-builtins==2.5.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:8cac7c52c6f0708c0902b46b385bc7e368a9068965083796f1431c0d2e6550cf \
+    --hash=sha256:bdaa3dd823e4f5308c5e712d19fa5f69daa52781ea874f5ea9c3637bcf56faa6
 flake8-coding==1.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:79704112c44d09d4ab6c8965e76a20c3f7073d52146db60303bce777d9612260 \
     --hash=sha256:b8f4d5157a8f74670e6cfea732c3d9f4291a4e994c8701d2c55f787c6e6cb741
 flake8-comments==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:42250cb4a51dc59e6db25f1291cfb16b78ea233f72dac32a5bc7b09c691235ea \
     --hash=sha256:780b4fc2820ed4ff8a0a98f3fc993f776ede1aecbe0c6cec64d93814b21c9234
 flake8-comprehensions==3.14.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -107,85 +107,78 @@
     --hash=sha256:e4848c57d9d50f19100c2d75fa794b72df068666a9041b4b0409be923356a3ed
 flake8-print==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:76915a2a389cc1c0879636c219eb909c38501d3a43cc8dae542081c9ba48bdf9 \
     --hash=sha256:84a1a6ea10d7056b804221ac5e62b1cee1aefc897ce16f2e5c42d3046068f5d8
 flake8-printf-formatting==1.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0f9e1308ac290356e4b271d4f26adfc3f9165680a7b6c221503b0f3e155a2784 \
     --hash=sha256:d908ffabdf08581043a50572744fd60563d82386630b0335445894120089d2df
+flake8-pyproject==1.2.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6249fe53545205af5e76837644dc80b4c10037e73a0e5db87ff562d75fb5bd4a
 flake8-raise==0.0.5 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0a9890e16b851402d9b0d4fafe6c34890eab73835a2c2079c3850a25be575623 \
     --hash=sha256:df26e5c542a58c8f8786d978e18ad7e54126a0ef5c6241c35dafaca7e2bbb808
 flake8-simplify==0.21.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:439391e762a9370b371208add0b5c5c40c3d25a98e1f5421d263215d08194183 \
     --hash=sha256:c95ff1dcc1de5949af47e0087cbf1164445881131b15bcd7a71252670f492f4d
 flake8-use-fstring==1.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6550bf722585eb97dffa8343b0f1c372101f5c4ab5b07ebf0edd1c79880cdd39
 flake8-use-pathlib==0.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0ef19f255a51601bcf04ff54f25ef8a466dff68210cd95b4f1db36a78ace5223 \
     --hash=sha256:c7b6d71575b575f7d70ebf3f1d7f2dd6685e401d3280208f1db9dbb6bfa32608
 flake8-variables-names==0.0.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:292c50e4813d632aa3adcd02c185e7bb583f5fc8ebe02e70f13c958bfe46ad91 \
     --hash=sha256:4aff935d54b3f7afcd026b4dae55029877bd05a7c507b294b45bc7bf577d7b47
-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
-    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
-gitdb==4.0.11 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:81a3407ddd2ee8df444cbacea00e2d038e40150acfa3001696fe0dcf1d3adfa4 \
-    --hash=sha256:bf5421126136d6d0af55bc1e7c1af1c397a34f5b7bd79e776cd3e89785c2b04b
-gitpython==3.1.40 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:22b126e9ffb671fdd0c129796343a02bf67bf2994b35449ffc9321aa755e18a4 \
-    --hash=sha256:cf14627d5a8049ffbf49915732e5eddbe8134c3bdb9d476e6182b676fc573f8a
+flake8==7.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
+    --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
 isort==5.13.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
     --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
 markdown-it-py==3.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
-more-itertools==10.1.0 ; python_version == "3.9" \
-    --hash=sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a \
-    --hash=sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6
+more-itertools==10.2.0 ; python_version == "3.9" \
+    --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
+    --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
 mr-proper==0.0.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03b517b19e617537f711ce418b125e5f2efd82ec881539cdee83195c78c14a02 \
     --hash=sha256:74a1b60240c46f10ba518707ef72811a01e5c270da0a78b5dd2dd923d99fdb14
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
 pbr==6.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda \
     --hash=sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9
 pep8-naming==0.13.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1705f046dfcd851378aac3be1cd1551c7c1e5ff363bacad707d43007877fa971 \
     --hash=sha256:1a86b8c71a03337c97181917e2b472f0f5e4ccb06844a0d6f0a33522549e7a80
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
 pycodestyle==2.11.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
-pyflakes==3.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
-    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
+pyflakes==3.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
+    --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
 pygments==2.17.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-pyproject-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6da8e5a264395e0148bc11844c6fb50546f1fac83ac9210f7328664135f9e70f \
-    --hash=sha256:86ea5559263c098e1aa4f866776aa2cf45362fd91a576b9fd8fbbbb55db12c4e
 pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
     --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
     --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
     --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
@@ -208,14 +201,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -229,34 +223,31 @@
     --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
-rich==13.7.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa \
-    --hash=sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235
-setuptools==69.0.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
-smmap==5.0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62 \
-    --hash=sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da
+rich==13.7.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
+setuptools==69.5.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
 stdlib-list==0.10.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6519c50d645513ed287657bfe856d527f277331540691ddeaf77b25459964a14 \
     --hash=sha256:b3a911bc441d03e0332dd1a9e7d0870ba3bb0a542a74d7524f54fb431256e214
-stevedore==5.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d \
-    --hash=sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c
+stevedore==5.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1c15d95766ca0569cad14cb6272d4d31dae66b011a929d7c18219c176ea1b5c9 \
+    --hash=sha256:46b93ca40e1114cea93d738a6c1e365396981bb6bb78c27045b7587c9473544d
 toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:032fa3cf3659c9865a07b59057edf9efe9e38631e6b977fdae04064888cb62ba \
     --hash=sha256:e9d77811d8f7d886c4ceaeadccd2675c6f2d794344775463faf1cb969e49d865
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "3.11" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "3.11" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
```

### Comparing `alluka-0.1.4/piped/dev-requirements/type-checking.txt` & `alluka-0.1.5/piped/dev-requirements/type-checking.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 # To update, run:
 #
 #    pip-compile-cross-platform dev-requirements/type-checking.in --output-file dev-requirements/type-checking.txt --min-python-version 3.9
 #
 annotated-types==0.6.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
     --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-anyio==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:745843b39e829e108e518c489b31dc757de7d2131d53fac32bd8df268227bfee \
-    --hash=sha256:e1875bb4b4e2de1669f4bc7869b6d3f54231cdced71605e6e64c9be77e3be50f
-argcomplete==3.2.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:30891d87f3c1abe091f2142613c9d33cac84a5e15404489f033b20399b691fec \
-    --hash=sha256:437f67fb9b058da5a090df505ef9be0297c4883993f3f56cb186ff087778cfb4
-asgiref==3.7.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:89b2ef2247e3b562a16eef663bc0e2e703ec6468e2fa8a5cd61cd449786d4f6e \
-    --hash=sha256:9e0ce3aa93a819ba5b45120216b23878cf6e8525eb3848653452b4192b92afed
-certifi==2023.11.17 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
-cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
+anyio==4.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:048e05d0f6caeed70d731f3db756d35dcc1f35747c8c403364a8332c630441b8 \
+    --hash=sha256:f75253795a87df48568485fd18cdd2a3fa5c4f7c5be8e5e36637733fce06fed6
+argcomplete==3.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
+    --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
+asgiref==3.8.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3e1e3ecc849832fe52ccf2cb6686b7a55f82bb1d6aee72a58826471390335e47 \
+    --hash=sha256:c343bd80a0bec947a9860adb4c432ffa7db769836c64238fc34bdc3fec84d590
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" and platform_python_implementation != "PyPy" \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
     --hash=sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743 \
@@ -74,325 +74,308 @@
     --hash=sha256:fcc8eb6d5902bb1cf6dc4f187ee3ea80a1eba0a89aba40a5cb20a5087d961357
 click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "win32" or platform_system == "Windows") \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-colorlog==6.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4ed23b05a1154294ac99f511fabe8c1d6d4364ec1f7fc989c7fb515ccc29d375 \
-    --hash=sha256:fbb6fdf9d5685f2517f388fb29bb27d54e8654dd31f58bc2a3b217e967a95ca6
-cryptography==41.0.7 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:079b85658ea2f59c4f43b70f8119a52414cdb7be34da5d019a77bf96d473b960 \
-    --hash=sha256:09616eeaef406f99046553b8a40fbf8b1e70795a91885ba4c96a70793de5504a \
-    --hash=sha256:13f93ce9bea8016c253b34afc6bd6a75993e5c40672ed5405a9c832f0d4a00bc \
-    --hash=sha256:37a138589b12069efb424220bf78eac59ca68b95696fc622b6ccc1c0a197204a \
-    --hash=sha256:3c78451b78313fa81607fa1b3f1ae0a5ddd8014c38a02d9db0616133987b9cdf \
-    --hash=sha256:43f2552a2378b44869fe8827aa19e69512e3245a219104438692385b0ee119d1 \
-    --hash=sha256:48a0476626da912a44cc078f9893f292f0b3e4c739caf289268168d8f4702a39 \
-    --hash=sha256:49f0805fc0b2ac8d4882dd52f4a3b935b210935d500b6b805f321addc8177406 \
-    --hash=sha256:5429ec739a29df2e29e15d082f1d9ad683701f0ec7709ca479b3ff2708dae65a \
-    --hash=sha256:5a1b41bc97f1ad230a41657d9155113c7521953869ae57ac39ac7f1bb471469a \
-    --hash=sha256:68a2dec79deebc5d26d617bfdf6e8aab065a4f34934b22d3b5010df3ba36612c \
-    --hash=sha256:7a698cb1dac82c35fcf8fe3417a3aaba97de16a01ac914b89a0889d364d2f6be \
-    --hash=sha256:841df4caa01008bad253bce2a6f7b47f86dc9f08df4b433c404def869f590a15 \
-    --hash=sha256:90452ba79b8788fa380dfb587cca692976ef4e757b194b093d845e8d99f612f2 \
-    --hash=sha256:928258ba5d6f8ae644e764d0f996d61a8777559f72dfeb2eea7e2fe0ad6e782d \
-    --hash=sha256:af03b32695b24d85a75d40e1ba39ffe7db7ffcb099fe507b39fd41a565f1b157 \
-    --hash=sha256:b640981bf64a3e978a56167594a0e97db71c89a479da8e175d8bb5be5178c003 \
-    --hash=sha256:c5ca78485a255e03c32b513f8c2bc39fedb7f5c5f8535545bdc223a03b24f248 \
-    --hash=sha256:c7f3201ec47d5207841402594f1d7950879ef890c0c495052fa62f58283fde1a \
-    --hash=sha256:d5ec85080cce7b0513cfd233914eb8b7bbd0633f1d1703aa28d1dd5a72f678ec \
-    --hash=sha256:d6c391c021ab1f7a82da5d8d0b3cee2f4b2c455ec86c8aebbc84837a631ff309 \
-    --hash=sha256:e3114da6d7f95d2dee7d3f4eec16dacff819740bbab931aff8648cb13c5ff5e7 \
-    --hash=sha256:f983596065a18a2183e7f79ab3fd4c475205b839e02cbc0efbbf9666c4b3083d
+colorlog==6.8.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3e3e079a41feb5a1b64f978b5ea4f46040a94f11f0e8bbb8261e3dbbeca64d44 \
+    --hash=sha256:4dcbb62368e2800cb3c5abd348da7e53f6c362dda502ec27c560b2e58a66bd33
+cryptography==42.0.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
 distlib==0.3.8 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
-exceptiongroup==1.2.0 ; python_version >= "3.9" and python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
-fastapi==0.108.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5056e504ac6395bf68493d71fcfc5352fdbd5fda6f88c21f6420d80d81163296 \
-    --hash=sha256:8c7bc6d315da963ee4cdb605557827071a9a7f95aeb8fcdd3bde48cdc8764dd7
-filelock==3.13.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
+exceptiongroup==1.2.1 ; python_version >= "3.9" and python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
+fastapi==0.110.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:239403f2c0a3dda07a9420f95157a7f014ddb2b770acdbc984f9bdf3ead7afdb \
+    --hash=sha256:b53d673652da3b65e8cd787ad214ec0fe303cad00d2b529b86ce7db13f17518d
+filelock==3.13.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
 h11==0.14.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8f19fbbe99e72420ff35c00b27a34cb9937e902a8b810e2c88300c6f0a3b699d \
     --hash=sha256:e3fe4ac4b851c468cc8363d500db52c2ead036020723024a109d37346efaa761
 h2==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03a46bcf682256c95b5fd9e9a99c1323584c3eec6440d379b9903d709476bc6d \
     --hash=sha256:a83aca08fbe7aacb79fec788c9c0bac936343560ed9ec18b82a13a12c28d2abb
 hpack==4.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84a076fad3dc9a9f8063ccb8041ef100867b1878b25ef0ee63847a5d53818a6c \
     --hash=sha256:fc41de0c63e687ebffde81187a948221294896f6bdc0ae2312708df339430095
-httpcore==1.0.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:096cc05bca73b8e459a1fc3dcf585148f63e534eae4339559c9b8a8d6399acc7 \
-    --hash=sha256:9fc092e4799b26174648e54b74ed5f683132a464e95643b226e00c2ed2fa6535
-httpx[http2]==0.26.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:451b55c30d5185ea6b23c2c793abf9bb237d2a7dfb901ced6ff69ad37ec1dfaf \
-    --hash=sha256:8915f5a3627c4d47b73e8202457cb28f1266982d1159bd5779d86a80c0eab1cd
+httpcore==1.0.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:34a38e2f9291467ee3b44e89dd52615370e152954ba21721378a87b2960f7a61 \
+    --hash=sha256:421f18bac248b25d310f3cacd198d55b8e6125c107797b609ff9b7a6ba7991b5
+httpx[http2]==0.27.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:71d5465162c13681bff01ad59b2cc68dd838ea1f10e51574bac27103f00c91a5 \
+    --hash=sha256:a0cb88a46f32dc874e04ee956e4c2764aba2aa228f650b06788ba6bda2962ab5
 hyperframe==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0ec6bafd80d8ad2195c4f03aacba3a8265e57bc4cff261e802bf39970ed02a15 \
     --hash=sha256:ae510046231dc8e9ecb1a6586f63d2347bf4c8905914aa84ba585ae85f28a914
-idna==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
-jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
+jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
 jwt==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:61c9170f92e736b530655e75374681d4fcca9cfa8763ab42be57353b2b203494
-markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-mypy==1.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02 \
-    --hash=sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66 \
-    --hash=sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8 \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6 \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a \
-    --hash=sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592 \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+mypy==1.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
 nodeenv==1.8.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
-nox==2023.4.22 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891 \
-    --hash=sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
-pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
-pydantic-core==2.14.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:00646784f6cd993b1e1c0e7b0fdcbccc375d539db95555477771c27555e3c556 \
-    --hash=sha256:00b1087dabcee0b0ffd104f9f53d7d3eaddfaa314cdd6726143af6bc713aa27e \
-    --hash=sha256:0348b1dc6b76041516e8a854ff95b21c55f5a411c3297d2ca52f5528e49d8411 \
-    --hash=sha256:036137b5ad0cb0004c75b579445a1efccd072387a36c7f217bb8efd1afbe5245 \
-    --hash=sha256:095b707bb287bfd534044166ab767bec70a9bba3175dcdc3371782175c14e43c \
-    --hash=sha256:0c08de15d50fa190d577e8591f0329a643eeaed696d7771760295998aca6bc66 \
-    --hash=sha256:1302a54f87b5cd8528e4d6d1bf2133b6aa7c6122ff8e9dc5220fbc1e07bffebd \
-    --hash=sha256:172de779e2a153d36ee690dbc49c6db568d7b33b18dc56b69a7514aecbcf380d \
-    --hash=sha256:1b027c86c66b8627eb90e57aee1f526df77dc6d8b354ec498be9a757d513b92b \
-    --hash=sha256:1ce830e480f6774608dedfd4a90c42aac4a7af0a711f1b52f807130c2e434c06 \
-    --hash=sha256:1fd0c1d395372843fba13a51c28e3bb9d59bd7aebfeb17358ffaaa1e4dbbe948 \
-    --hash=sha256:23598acb8ccaa3d1d875ef3b35cb6376535095e9405d91a3d57a8c7db5d29341 \
-    --hash=sha256:24368e31be2c88bd69340fbfe741b405302993242ccb476c5c3ff48aeee1afe0 \
-    --hash=sha256:26a92ae76f75d1915806b77cf459811e772d8f71fd1e4339c99750f0e7f6324f \
-    --hash=sha256:27e524624eace5c59af499cd97dc18bb201dc6a7a2da24bfc66ef151c69a5f2a \
-    --hash=sha256:2b8719037e570639e6b665a4050add43134d80b687288ba3ade18b22bbb29dd2 \
-    --hash=sha256:2c5bcf3414367e29f83fd66f7de64509a8fd2368b1edf4351e862910727d3e51 \
-    --hash=sha256:2dbe357bc4ddda078f79d2a36fc1dd0494a7f2fad83a0a684465b6f24b46fe80 \
-    --hash=sha256:2f5fa187bde8524b1e37ba894db13aadd64faa884657473b03a019f625cee9a8 \
-    --hash=sha256:2f6ffc6701a0eb28648c845f4945a194dc7ab3c651f535b81793251e1185ac3d \
-    --hash=sha256:314ccc4264ce7d854941231cf71b592e30d8d368a71e50197c905874feacc8a8 \
-    --hash=sha256:36026d8f99c58d7044413e1b819a67ca0e0b8ebe0f25e775e6c3d1fabb3c38fb \
-    --hash=sha256:36099c69f6b14fc2c49d7996cbf4f87ec4f0e66d1c74aa05228583225a07b590 \
-    --hash=sha256:36fa402dcdc8ea7f1b0ddcf0df4254cc6b2e08f8cd80e7010d4c4ae6e86b2a87 \
-    --hash=sha256:370ffecb5316ed23b667d99ce4debe53ea664b99cc37bfa2af47bc769056d534 \
-    --hash=sha256:3860c62057acd95cc84044e758e47b18dcd8871a328ebc8ccdefd18b0d26a21b \
-    --hash=sha256:399ac0891c284fa8eb998bcfa323f2234858f5d2efca3950ae58c8f88830f145 \
-    --hash=sha256:3a0b5db001b98e1c649dd55afa928e75aa4087e587b9524a4992316fa23c9fba \
-    --hash=sha256:3dcf1978be02153c6a31692d4fbcc2a3f1db9da36039ead23173bc256ee3b91b \
-    --hash=sha256:4241204e4b36ab5ae466ecec5c4c16527a054c69f99bba20f6f75232a6a534e2 \
-    --hash=sha256:438027a975cc213a47c5d70672e0d29776082155cfae540c4e225716586be75e \
-    --hash=sha256:43e166ad47ba900f2542a80d83f9fc65fe99eb63ceec4debec160ae729824052 \
-    --hash=sha256:478e9e7b360dfec451daafe286998d4a1eeaecf6d69c427b834ae771cad4b622 \
-    --hash=sha256:4ce8299b481bcb68e5c82002b96e411796b844d72b3e92a3fbedfe8e19813eab \
-    --hash=sha256:4f86f1f318e56f5cbb282fe61eb84767aee743ebe32c7c0834690ebea50c0a6b \
-    --hash=sha256:55a23dcd98c858c0db44fc5c04fc7ed81c4b4d33c653a7c45ddaebf6563a2f66 \
-    --hash=sha256:599c87d79cab2a6a2a9df4aefe0455e61e7d2aeede2f8577c1b7c0aec643ee8e \
-    --hash=sha256:5aa90562bc079c6c290f0512b21768967f9968e4cfea84ea4ff5af5d917016e4 \
-    --hash=sha256:64634ccf9d671c6be242a664a33c4acf12882670b09b3f163cd00a24cffbd74e \
-    --hash=sha256:667aa2eac9cd0700af1ddb38b7b1ef246d8cf94c85637cbb03d7757ca4c3fdec \
-    --hash=sha256:6a31d98c0d69776c2576dda4b77b8e0c69ad08e8b539c25c7d0ca0dc19a50d6c \
-    --hash=sha256:6af4b3f52cc65f8a0bc8b1cd9676f8c21ef3e9132f21fed250f6958bd7223bed \
-    --hash=sha256:6c8edaea3089bf908dd27da8f5d9e395c5b4dc092dbcce9b65e7156099b4b937 \
-    --hash=sha256:71d72ca5eaaa8d38c8df16b7deb1a2da4f650c41b58bb142f3fb75d5ad4a611f \
-    --hash=sha256:72f9a942d739f09cd42fffe5dc759928217649f070056f03c70df14f5770acf9 \
-    --hash=sha256:747265448cb57a9f37572a488a57d873fd96bf51e5bb7edb52cfb37124516da4 \
-    --hash=sha256:75ec284328b60a4e91010c1acade0c30584f28a1f345bc8f72fe8b9e46ec6a96 \
-    --hash=sha256:78d0768ee59baa3de0f4adac9e3748b4b1fffc52143caebddfd5ea2961595277 \
-    --hash=sha256:78ee52ecc088c61cce32b2d30a826f929e1708f7b9247dc3b921aec367dc1b23 \
-    --hash=sha256:7be719e4d2ae6c314f72844ba9d69e38dff342bc360379f7c8537c48e23034b7 \
-    --hash=sha256:7e1f4744eea1501404b20b0ac059ff7e3f96a97d3e3f48ce27a139e053bb370b \
-    --hash=sha256:7e90d6cc4aad2cc1f5e16ed56e46cebf4877c62403a311af20459c15da76fd91 \
-    --hash=sha256:7ebe3416785f65c28f4f9441e916bfc8a54179c8dea73c23023f7086fa601c5d \
-    --hash=sha256:7f41533d7e3cf9520065f610b41ac1c76bc2161415955fbcead4981b22c7611e \
-    --hash=sha256:7f5025db12fc6de7bc1104d826d5aee1d172f9ba6ca936bf6474c2148ac336c1 \
-    --hash=sha256:86c963186ca5e50d5c8287b1d1c9d3f8f024cbe343d048c5bd282aec2d8641f2 \
-    --hash=sha256:86ce5fcfc3accf3a07a729779d0b86c5d0309a4764c897d86c11089be61da160 \
-    --hash=sha256:8a14c192c1d724c3acbfb3f10a958c55a2638391319ce8078cb36c02283959b9 \
-    --hash=sha256:8b93785eadaef932e4fe9c6e12ba67beb1b3f1e5495631419c784ab87e975670 \
-    --hash=sha256:8ed1af8692bd8d2a29d702f1a2e6065416d76897d726e45a1775b1444f5928a7 \
-    --hash=sha256:92879bce89f91f4b2416eba4429c7b5ca22c45ef4a499c39f0c5c69257522c7c \
-    --hash=sha256:94fc0e6621e07d1e91c44e016cc0b189b48db053061cc22d6298a611de8071bb \
-    --hash=sha256:982487f8931067a32e72d40ab6b47b1628a9c5d344be7f1a4e668fb462d2da42 \
-    --hash=sha256:9862bf828112e19685b76ca499b379338fd4c5c269d897e218b2ae8fcb80139d \
-    --hash=sha256:99b14dbea2fdb563d8b5a57c9badfcd72083f6006caf8e126b491519c7d64ca8 \
-    --hash=sha256:9c6a5c79b28003543db3ba67d1df336f253a87d3112dac3a51b94f7d48e4c0e1 \
-    --hash=sha256:a19b794f8fe6569472ff77602437ec4430f9b2b9ec7a1105cfd2232f9ba355e6 \
-    --hash=sha256:a306cdd2ad3a7d795d8e617a58c3a2ed0f76c8496fb7621b6cd514eb1532cae8 \
-    --hash=sha256:a3dde6cac75e0b0902778978d3b1646ca9f438654395a362cb21d9ad34b24acf \
-    --hash=sha256:a874f21f87c485310944b2b2734cd6d318765bcbb7515eead33af9641816506e \
-    --hash=sha256:a983cca5ed1dd9a35e9e42ebf9f278d344603bfcb174ff99a5815f953925140a \
-    --hash=sha256:aca48506a9c20f68ee61c87f2008f81f8ee99f8d7f0104bff3c47e2d148f89d9 \
-    --hash=sha256:b2602177668f89b38b9f84b7b3435d0a72511ddef45dc14446811759b82235a1 \
-    --hash=sha256:b3e5fe4538001bb82e2295b8d2a39356a84694c97cb73a566dc36328b9f83b40 \
-    --hash=sha256:b6ca36c12a5120bad343eef193cc0122928c5c7466121da7c20f41160ba00ba2 \
-    --hash=sha256:b89f4477d915ea43b4ceea6756f63f0288941b6443a2b28c69004fe07fde0d0d \
-    --hash=sha256:b9a9d92f10772d2a181b5ca339dee066ab7d1c9a34ae2421b2a52556e719756f \
-    --hash=sha256:c99462ffc538717b3e60151dfaf91125f637e801f5ab008f81c402f1dff0cd0f \
-    --hash=sha256:cb92f9061657287eded380d7dc455bbf115430b3aa4741bdc662d02977e7d0af \
-    --hash=sha256:cdee837710ef6b56ebd20245b83799fce40b265b3b406e51e8ccc5b85b9099b7 \
-    --hash=sha256:cf10b7d58ae4a1f07fccbf4a0a956d705356fea05fb4c70608bb6fa81d103cda \
-    --hash=sha256:d15687d7d7f40333bd8266f3814c591c2e2cd263fa2116e314f60d82086e353a \
-    --hash=sha256:d5c28525c19f5bb1e09511669bb57353d22b94cf8b65f3a8d141c389a55dec95 \
-    --hash=sha256:d5f916acf8afbcab6bacbb376ba7dc61f845367901ecd5e328fc4d4aef2fcab0 \
-    --hash=sha256:dab03ed811ed1c71d700ed08bde8431cf429bbe59e423394f0f4055f1ca0ea60 \
-    --hash=sha256:db453f2da3f59a348f514cfbfeb042393b68720787bbef2b4c6068ea362c8149 \
-    --hash=sha256:de2a0645a923ba57c5527497daf8ec5df69c6eadf869e9cd46e86349146e5975 \
-    --hash=sha256:dea7fcd62915fb150cdc373212141a30037e11b761fbced340e9db3379b892d4 \
-    --hash=sha256:dfcbebdb3c4b6f739a91769aea5ed615023f3c88cb70df812849aef634c25fbe \
-    --hash=sha256:dfcebb950aa7e667ec226a442722134539e77c575f6cfaa423f24371bb8d2e94 \
-    --hash=sha256:e0641b506486f0b4cd1500a2a65740243e8670a2549bb02bc4556a83af84ae03 \
-    --hash=sha256:e33b0834f1cf779aa839975f9d8755a7c2420510c0fa1e9fa0497de77cd35d2c \
-    --hash=sha256:e4ace1e220b078c8e48e82c081e35002038657e4b37d403ce940fa679e57113b \
-    --hash=sha256:e4cf2d5829f6963a5483ec01578ee76d329eb5caf330ecd05b3edd697e7d768a \
-    --hash=sha256:e574de99d735b3fc8364cba9912c2bec2da78775eba95cbb225ef7dda6acea24 \
-    --hash=sha256:e646c0e282e960345314f42f2cea5e0b5f56938c093541ea6dbf11aec2862391 \
-    --hash=sha256:e8a5ac97ea521d7bde7621d86c30e86b798cdecd985723c4ed737a2aa9e77d0c \
-    --hash=sha256:eedf97be7bc3dbc8addcef4142f4b4164066df0c6f36397ae4aaed3eb187d8ab \
-    --hash=sha256:ef633add81832f4b56d3b4c9408b43d530dfca29e68fb1b797dcb861a2c734cd \
-    --hash=sha256:f27207e8ca3e5e021e2402ba942e5b4c629718e665c81b8b306f3c8b1ddbb786 \
-    --hash=sha256:f85f3843bdb1fe80e8c206fe6eed7a1caeae897e496542cee499c374a85c6e08 \
-    --hash=sha256:f8e81e4b55930e5ffab4a68db1af431629cf2e4066dbdbfef65348b8ab804ea8 \
-    --hash=sha256:f96ae96a060a8072ceff4cfde89d261837b4294a4f28b84a28765470d502ccc6 \
-    --hash=sha256:fd9e98b408384989ea4ab60206b8e100d8687da18b5c813c11e92fd8212a98e0 \
-    --hash=sha256:ffff855100bc066ff2cd3aa4a60bc9534661816b110f0243e59503ec2df38421
-pydantic==2.5.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b3ef57c62535b0941697cce638c08900d87fcb67e29cfa99e8a68f747f393f7a \
-    --hash=sha256:d0caf5954bee831b6bfe7e338c32b9e30c85dfe080c843680783ac2b631673b4
-pyright==1.1.343 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:75a0d24e8227328198bdfa1f4904ce66b78c2bacf49c269d9e6e3b174b026225 \
-    --hash=sha256:871e122d74003e8e5fddb17867220b06ee892de61fa967ca7ca031acdc176738
-python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
-python-dotenv==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:a8df96034aae6d2d50a4ebe8216326c61c3eb64836776504fcca410e5937a3ba \
-    --hash=sha256:f5971a9226b701070a4bf2c38c89e5a3f0d64de8debda981d1db98583009122a
-setuptools==69.0.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
+nox==2024.4.15 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6492236efa15a460ecb98e7b67562a28b70da006ab0be164e8821177577c0565 \
+    --hash=sha256:ecf6700199cdfa9e5ea0a41ff5e6ef4641d09508eda6edb89d9987864115817f
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+pycparser==2.22 ; python_version >= "3.9" and python_version < "4.0" and platform_python_implementation != "PyPy" \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pydantic-core==2.18.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+pydantic==2.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
+pyright==1.1.359 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
+    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
+python-dateutil==2.9.0.post0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
+python-dotenv==1.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:e324ee90a023d808f1959c46bcbc04446a10ced277783dc6ee09987c37ec10ca \
+    --hash=sha256:f7b63ef50f1b690dddf550d03497b66d609393b40b564ed0d674909a68ebf16a
+setuptools==69.5.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-sniffio==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:e60305c5e5d314f5389259b7f22aaa33d8f7dee49763119234af3755c55b9101 \
-    --hash=sha256:eecefdce1e5bbfb7ad2eeaabf7c1eeb404d7757c379bd1f7e5cce9d8bf425384
-starlette==0.32.0.post1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cd0cb10ddb49313f609cedfac62c8c12e56c7314b66d89bb077ba228bada1b09 \
-    --hash=sha256:e54e2b7e2fb06dff9eac40133583f10dfa05913f5a85bf26f427c7a40a9a3d02
+sniffio==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2f6da418d1f1e0fddd844478f41680e794e6051915791a034ff65e5f100525a2 \
+    --hash=sha256:f4324edc670a0f49750a81b895f35c3adb843cca46f0530f79fc1babb23789dc
+starlette==0.37.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6fe59f29268538e5d0d182f2791a479a0c64638e6935d1c6989e63fb2699c6ee \
+    --hash=sha256:9af890290133b79fc3db55474ade20f6220a364a0402e0b556e7cd5e1e093823
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-uvicorn==0.25.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6dddbad1d7ee0f5140aba5ec138ddc9612c5109399903828b4874c9937f009c2 \
-    --hash=sha256:ce107f5d9bd02b4636001a77a4e74aab5e1e2b146868ebbad565237145af444c
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+uvicorn==0.29.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2c2aac7ff4f4365c206fd773a39bf4ebd1047c238f8b8268ad996829323473de \
+    --hash=sha256:6a69214c0b6a087462412670b3ef21224fa48cae0e452b5883e8e8bdfdd11dd0
 uvloop==0.19.0 ; python_version >= "3.9" and python_version < "4.0" and platform_system != "Windows" \
     --hash=sha256:0246f4fd1bf2bf702e06b0d45ee91677ee5c31242f39aab4ea6fe0c51aedd0fd \
     --hash=sha256:02506dc23a5d90e04d4f65c7791e65cf44bd91b37f24cfc3ef6cf2aff05dc7ec \
     --hash=sha256:13dfdf492af0aa0a0edf66807d2b465607d11c4fa48f4a1fd41cbea5b18e8e8b \
     --hash=sha256:2693049be9d36fef81741fddb3f441673ba12a34a704e7b4361efb75cf30befc \
     --hash=sha256:271718e26b3e17906b28b67314c45d19106112067205119dddbd834c2b7ce797 \
     --hash=sha256:2df95fca285a9f5bfe730e51945ffe2fa71ccbfdde3b0da5772b4ee4f2e770d5 \
@@ -417,10 +400,10 @@
     --hash=sha256:8ca4956c9ab567d87d59d49fa3704cf29e37109ad348f2d5223c9bf761a332e7 \
     --hash=sha256:91ab01c6cd00e39cde50173ba4ec68a1e578fee9279ba64f5221810a9e786533 \
     --hash=sha256:cd81bdc2b8219cb4b2556eea39d2e36bfa375a2dd021404f90a62e44efaaf957 \
     --hash=sha256:da8435a3bd498419ee8c13c34b89b5005130a476bda1d6ca8cfdde3de35cd650 \
     --hash=sha256:de4313d7f575474c8f5a12e163f6d89c0a878bc49219641d49e6f1444369a90e \
     --hash=sha256:e27f100e1ff17f6feeb1f33968bc185bf8ce41ca557deee9d9bbbffeb72030b7 \
     --hash=sha256:f467a5fd23b4fc43ed86342641f3936a68ded707f4627622fa3f82a120e18256
-virtualenv==20.25.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3 \
-    --hash=sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b
+virtualenv==20.25.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
+    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
```

### Comparing `alluka-0.1.4/piped/github/actions/clippy.yml` & `alluka-0.1.5/piped/github/actions/clippy.yml`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     - cron: "0 12 * * 6"
   workflow_dispatch:
 
 jobs:
   clippy:
     runs-on: ubuntu-latest
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
 
       - uses: actions-rs/toolchain@16499b5e05bf2e26879000db0c1d13f7e13fa3af
         with:
             toolchain: nightly
             components: clippy
             override: true
```

### Comparing `alluka-0.1.4/piped/github/actions/freeze-for-pr.yml` & `alluka-0.1.5/piped/github/actions/freeze-for-pr.yml`

 * *Files 23% similar despite different names*

```diff
@@ -11,31 +11,31 @@
     paths: [{{ (FILTERS + EXTEND_FILTERS) | map("quoted") | join(", ") }}]
 
 jobs:
   freeze-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
 
       - name: Upgrade dependency locks
         run: python -m nox -s freeze-locks bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/github/actions/lint.yml` & `alluka-0.1.5/piped/github/actions/lint.yml`

 * *Files 24% similar despite different names*

```diff
@@ -16,20 +16,20 @@
   workflow_dispatch:
 
 jobs:
   lint:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}{% if "verify-markup" not in config.hide %}
```

### Comparing `alluka-0.1.4/piped/github/actions/pr-docs.yml` & `alluka-0.1.5/piped/github/actions/pr-docs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,23 +18,23 @@
 
 jobs:
   deploy-docs-preview:
     runs-on: ubuntu-latest
 
     steps:
       - name: Fetch merge branch
-        uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+        uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           {% raw %}ref: ${{ github.event.pull_request.head.sha }}{% endraw %}
           {% raw %}repository: ${{ github.event.pull_request.head.repo.full_name }}{% endraw %}
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
         if: github.event.action != 'closed'
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         if: github.event.action != 'closed'
         run: |
           python -m pip install --upgrade pip wheel
```

### Comparing `alluka-0.1.4/piped/github/actions/publish.yml` & `alluka-0.1.5/piped/github/actions/publish.yml`

 * *Files 16% similar despite different names*

```diff
@@ -7,28 +7,31 @@
       - published
 
 jobs:{% if "release_docs" in config.github_actions %}
   publish-docs:
     uses: ./.github/workflows/release-docs.yml
 {% endif %}
   publish:
+    name: upload release to PyPI
     runs-on: ubuntu-latest
+    environment: release
+    permissions:
+      id-token: write
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
-      - name: Install prerequisites
+      - name: Build project
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
+          python -m nox -s build
 
-      - name: publish
-        run: python -m nox -s publish
-        env:
-          {% raw %}PUBLISH_TOKEN: ${{ secrets.PUBLISH_TOKEN }}{% endraw %}
+      - name: Publish package distributions to PyPI
+        uses: pypa/gh-action-pypi-publish@81e9d935c883d0b210363ab89cf05f3894778450
```

### Comparing `alluka-0.1.4/piped/github/actions/py-test.yml` & `alluka-0.1.5/piped/github/actions/py-test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -22,20 +22,20 @@
       matrix:
         os: {{ OSES }}
         python-version: [{{ PYTHON_VERSIONS | map("quoted") | join(", ") }}]
 
     {% raw %}runs-on: ${{ matrix.os }}{% endraw %}
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       {% raw %}- name: Set up Python ${{ matrix.python-version }}{% endraw %}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           {% raw %}python-version: ${{ matrix.python-version }}{% endraw %}
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
@@ -47,20 +47,20 @@
   # TODO: Could we switch over to gather coverage from the normal test runs and combining
   # the result once https://github.com/nedbat/coveragepy/issues/1002 is fixed?
   upload-coverage:
     # needs: [test]
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
@@ -73,12 +73,12 @@
         uses: paambaati/codeclimate-action@a1831d7162ea1fbc612ffe5fb3b90278b7999d59
         env:
           CC_TEST_REPORTER_ID: {{ CODECLIMATE_TOKEN }}
         with:
           coverageLocations: .coverage.xml:coverage.py
 
       - name: Archive coverage
-        uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+        uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: coverage
           path: ./coverage_html
           if-no-files-found: error{% endif %}
```

### Comparing `alluka-0.1.4/piped/github/actions/reformat.yml` & `alluka-0.1.5/piped/.github/workflows/reformat.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 name: Reformat PR code
 
 concurrency:
-  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
+  group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 on:
   pull_request:
     branches:
       - master
 
 jobs:
   reformat:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
-      - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+      - name: Set up Python 3.11
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
-          python-version: "{{ DEFAULT_PY_VER }}"
+          python-version: "3.11"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r {{ NOX_DEP_PATH }}
+          python -m pip install -r ./python/base-requirements/nox.txt
 
       - name: Reformat
         run: python -m nox -s reformat bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/github/actions/release-docs.yml` & `alluka-0.1.5/piped/github/actions/release-docs.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,20 +7,20 @@
     branches: [{{ BRANCH_PUSHES | join(", ") }}]{% endif %}
 
 jobs:
   publish-docs:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: Install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
@@ -29,15 +29,15 @@
         id: doc_info
         run: |
           mkdir site
           python -m nox -s generate-docs -- -o ./site -j
           echo "GIT_HASH=$(git rev-parse HEAD)" >> $GITHUB_STATE
 
       - name: Push
-        uses: JamesIves/github-pages-deploy-action@65b5dfd4f5bcd3a7403bbc2959c144256167464e
+        uses: JamesIves/github-pages-deploy-action@ec9c88baef04b842ca6f0a132fd61c762aa6c1b0
         with:
           branch: docs
           {% raw %}commit-message: "${{ steps.doc_info.outputs.GIT_HASH }} docs (${{ github.event.release.tag_name || github.event.ref }})"{% endraw %}
           clean-exclude: pr-preview
           folder: ./site
           git-config-email: "{{ ACTION_COMMITTER_EMAIL }}"
           git-config-name: "{{ ACTION_COMMITTER_USERNAME }}"
```

### Comparing `alluka-0.1.4/piped/github/actions/resync-piped.yml` & `alluka-0.1.5/piped/github/actions/rustfmt.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,45 @@
-name: Resync piped
+name: Run Rustfmt
 
 concurrency:
   {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
   cancel-in-progress: true
 
-on:
-  pull_request:
-    branches:
-      - master
-    paths: [{{ FILTERS | map("quoted") | join(", ") }}]
+on: pull_request
 
 jobs:
-  resync-piped:
+  rustfmt:
     runs-on: ubuntu-latest
-
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
-          python -m pip install -r {{ NOX_DEP_PATH }}
+          python -m pip install -r ./piped/python/base-requirements/nox.txt
+
+      - uses: actions-rs/toolchain@16499b5e05bf2e26879000db0c1d13f7e13fa3af
+        with:
+            toolchain: nightly
+            components: rustfmt
+            override: true
+
+      - name: Reformat
+        run: cargo +nightly fmt
 
-      - name: Resync Piped
-        run: python -m nox -s copy-piped bot-package-diff
+      - name: Package
+        run: python -m nox -s bot-package-diff
 
-      - uses: actions/upload-artifact@c7d193f32edcb7bfad88892161225aeda64e9392
+      - uses: actions/upload-artifact@65462800fd760344b1a7b4382951275a0abb4808
         with:
           name: gogo.patch
           path: gogo.patch
 
       - name: Check diff file
         run: python -m nox -s is-diff-file-empty
```

### Comparing `alluka-0.1.4/piped/github/actions/type-check.yml` & `alluka-0.1.5/piped/github/actions/update-licence.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-name: Type check
-
-concurrency:
-  {% raw %}group: ${{ github.workflow }}-${{ github.ref }}{% endraw %}
-  cancel-in-progress: true
+name: Update licence
 
 on:
-  push:
-    branches:
-      - master
-  pull_request:
-    branches:
-      - master
   schedule:
-    - cron: "0 12 * * 6"
+    - cron: "0 7 1 1 *"
   workflow_dispatch:
 
 jobs:
-  type-check:
+  update-licence:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
 
-      - name: Run type checker
-        run: python -m nox -s type-check
+      - name: Update licence
+        run: python -m nox -s update-licence
+
+      - name: Create Pull Request
+        uses: peter-evans/create-pull-request@9153d834b60caba6d51c9b9510b087acf9f33f83
+        with:
+          author: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
+          branch: task/update-licence
+          commit-message: Update licence
+          committer: "{{ ACTION_COMMITTER_USERNAME }} <{{ ACTION_COMMITTER_EMAIL }}>"
+          title: Update licence
+          {% raw %}token: ${{ secrets.ACTIONS_TOKEN || secrets.GITHUB_TOKEN }}{% endraw %}
```

### Comparing `alluka-0.1.4/piped/github/actions/verify-locks.yml` & `alluka-0.1.5/piped/github/actions/verify-locks.yml`

 * *Files 8% similar despite different names*

```diff
@@ -14,20 +14,20 @@
     paths: [{{ (FILTERS + EXTEND_FILTERS) | map("quoted") | join(", ") }}]
 
 jobs:
   verify-pr-dep-changes:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
```

### Comparing `alluka-0.1.4/piped/github/actions/verify-types.yml` & `alluka-0.1.5/piped/github/actions/verify-types.yml`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,20 @@
   workflow_dispatch:
 
 jobs:
   verify-types:
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@b4ffde65f46336ab88eb53be808477a3936bae11
+      - uses: actions/checkout@1d96c772d19495a3b5c517cd2bc0cb401ea0529f
         with:
           submodules: "true"
 
       - name: Set up Python {{ DEFAULT_PY_VER }}
-        uses: actions/setup-python@0a5c61591373683505ea898e09a3ea4f39ef2b9c
+        uses: actions/setup-python@82c7e631bb3cdc910f68e0081d67478d79c6982d
         with:
           python-version: "{{ DEFAULT_PY_VER }}"
 
       - name: install prerequisites
         run: |
           python -m pip install --upgrade pip wheel
           python -m pip install -r {{ NOX_DEP_PATH }}
```

### Comparing `alluka-0.1.4/piped/github/dependabot.yml` & `alluka-0.1.5/piped/github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/piped/github/pull_request_template.md` & `alluka-0.1.5/piped/github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/piped/noxfile.py` & `alluka-0.1.5/piped/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/piped/pyproject.toml` & `alluka-0.1.5/piped/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 top_level_targets = ["./bot", "./noxfile.py", "./python"]
 version_constraint = "3.9"
 
 [tool.piped.github_actions."*"]
 default_py_ver = "3.11"
 nox_dep_path = "./python/base-requirements/nox.txt"
 
+[tool.piped.github_actions.docker_publish]
 [tool.piped.github_actions.freeze_for_pr]
 [tool.piped.github_actions.lint]
 [tool.piped.github_actions.reformat]
 [tool.piped.github_actions.resync_piped]
 FILTERS = ["github/actions/*", "pyproject.toml"]
 
 [tool.piped.github_actions.type_check]
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/docs.txt` & `alluka-0.1.5/piped/python/base-requirements/docs.txt`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/docs.in --output-file python/base-requirements/docs.txt --min-python-version 3.9
 #
 babel==2.14.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6919867db036398ba21eb5c7a0f6b28ab8cbc3ae7a73a44ebe34ae74a4e7d363 \
     --hash=sha256:efb1a25b7118e67ce3a259bed20545c29cb68be8ad2c784c83689981b7a57287
-certifi==2023.11.17 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
 charset-normalizer==3.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
     --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
     --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
     --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
     --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
     --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
@@ -108,144 +108,144 @@
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 csscompressor==0.9.5 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:afa22badbcf3120a4f392e4d22f9fff485c044a1feda4a950ecc5eba9dd31a05
 ghp-import==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:8337dd7b50877f163d4c0289bc1f1c7f127550241988d568c1db512c4324a619 \
     --hash=sha256:9c535c4c61193c2df8871222567d7fd7e5014d835f97dc7b7439069e2413d343
-griffe==0.38.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:334c79d3b5964ade65c05dfcaf53518c576dedd387aaba5c9fd71212f34f1483 \
-    --hash=sha256:bd68d7da7f3d87bc57eb9962b250db123efd9bbcc06c11c1a91b6e583b2a9361
+griffe==0.44.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:34aee1571042f9bf00529bc715de4516fb6f482b164e90d030300601009e0223 \
+    --hash=sha256:8a4471c469ba980b87c843f1168850ce39d0c1d0c7be140dca2480f76c8e5446
 htmlmin2==0.1.13 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:75609f2a42e64f7ce57dbff28a39890363bde9e7e5885db633317efbdf8c79a2
-idna==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
-importlib-metadata==7.0.1 ; python_version >= "3.9" and python_version < "3.10" \
-    --hash=sha256:4805911c3a4ec7c3966410053e9ec6a1fecd629117df5adee56dfc9432a1081e \
-    --hash=sha256:f238736bb06590ae52ac1fab06a3a9ef1d8dce2b7a35b5ab329371d6c8f5d2cc
-jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
+importlib-metadata==7.1.0 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
+    --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
+jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
 jsmin==3.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:c0959a121ef94542e807a674142606f7e90214a2b3d1eb17300244bbb5cc2bfc
 markdown-include==0.8.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1d0623e0fc2757c38d35df53752768356162284259d259c486b4ab6285cdbbe3 \
     --hash=sha256:32f0635b9cfef46997b307e2430022852529f7a5b87c0075c504283e7cc7db53
-markdown==3.5.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5874b47d4ee3f0b14d764324d2c94c03ea66bee56f2d929da9f2508d65e722dc \
-    --hash=sha256:b65d7beb248dc22f2e8a31fb706d93798093c308dc1aba295aedeb9d41a813bd
-markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+markdown==3.6 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:48f276f4d8cfb8ce6527c8f79e2ee29708508bf4d40aa410fbc3b4ee832c850f \
+    --hash=sha256:ed4f41f6daecbeeb96e576ce414c41d2d876daa9a16cb35fa8ed8c2ddfad0224
+markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
 mergedeep==1.3.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0096d52e9dad9939c3d975a774666af186eda617e6ca84df4c94dec30004f2a8 \
     --hash=sha256:70775750742b25c0d8f36c55aed03d24c3384d17c951b3175d898bd778ef0307
-mkdocs-autorefs==0.5.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:7930fcb8ac1249f10e683967aeaddc0af49d90702af111a5e390e8b20b3d97ff \
-    --hash=sha256:9a5054a94c08d28855cfab967ada10ed5be76e2bfad642302a610b252c3274c0
+mkdocs-autorefs==1.0.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:aacdfae1ab197780fb7a2dac92ad8a3d8f7ca8049a9cbe56a4218cd52e8da570 \
+    --hash=sha256:f684edf847eced40b570b57846b15f0bf57fb93ac2c510450775dcf16accb971
 mkdocs-material-extensions==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:10c9511cea88f568257f960358a467d12b970e1f7b2c0e5fb2bb48cab1928443 \
     --hash=sha256:adff8b62700b25cb77b53358dad940f3ef973dd6db797907c49e3c2ef3ab4e31
-mkdocs-material==9.5.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5899219f422f0a6de784232d9d40374416302ffae3c160cacc72969fcc1ee372 \
-    --hash=sha256:76c93a8525cceb0b395b9cedab3428bf518cf6439adef2b940f1c1574b775d89
-mkdocs-minify-plugin==0.7.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6a551e22d6517eaef9e1890afd60021dc1dcd1255de02d266f588d1ace040713 \
-    --hash=sha256:ae8bfc4a68806883e990ea025938b3f989da7b9fa08ea8390dba47adf25e0c5b
+mkdocs-material==9.5.18 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1e0e27fc9fe239f9064318acf548771a4629d5fd5dfd45444fd80a953fe21eb4 \
+    --hash=sha256:a43f470947053fa2405c33995f282d24992c752a50114f23f30da9d8d0c57e62
+mkdocs-minify-plugin==0.8.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5fba1a3f7bd9a2142c9954a6559a57e946587b21f133165ece30ea145c66aee6 \
+    --hash=sha256:bc11b78b8120d79e817308e2b11539d790d21445eb63df831e393f76e52e753d
 mkdocs==1.5.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:3b3a78e736b31158d64dbb2f8ba29bd46a379d0c6e324c2246c3bc3d2189cfc1 \
     --hash=sha256:eb7c99214dcb945313ba30426c2451b735992c73c2e10838f76d09e39ff4d0e2
-mkdocstrings-python==1.7.5 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5f6246026353f0c0785135db70c3fe9a5d9318990fc7ceb11d62097b8ffdd704 \
-    --hash=sha256:c7d143728257dbf1aa550446555a554b760dcd40a763f077189d298502b800be
-mkdocstrings==0.24.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:222b1165be41257b494a9d29b14135d2b7ca43f38161d5b10caae03b87bd4f7e \
-    --hash=sha256:f4908560c10f587326d8f5165d1908817b2e280bbf707607f601c996366a2264
-mkdocstrings[python]==0.24.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:222b1165be41257b494a9d29b14135d2b7ca43f38161d5b10caae03b87bd4f7e \
-    --hash=sha256:f4908560c10f587326d8f5165d1908817b2e280bbf707607f601c996366a2264
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+mkdocstrings-python==1.10.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:71678fac657d4d2bb301eed4e4d2d91499c095fd1f8a90fa76422a87a5693828 \
+    --hash=sha256:ba833fbd9d178a4b9d5cb2553a4df06e51dc1f51e41559a4d2398c16a6f69ecc
+mkdocstrings==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
+    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
+mkdocstrings[python]==0.24.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5c9cf2a32958cd161d5428699b79c8b0988856b0d4a8c5baf8395fc1bf4087c3 \
+    --hash=sha256:f327b234eb8d2551a306735436e157d0a22d45f79963c60a8b585d5f7a94c1d2
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 paginate==0.5.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:5e6007b6a9398177a7e1648d04fdd9f8c9766a1a945bceac82f1929e8c78af2d
 pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
 pygments==2.17.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-pymdown-extensions==10.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:561eb3a5f3c3c2512952a4d6f5b311aa124b7147bd54a3ea0f36ce030c7e3dd9 \
-    --hash=sha256:e4531379e0d74b329ff264217ef5b8b1a37bed3afe36f98001b74ecff52215c0
-python-dateutil==2.8.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
-    --hash=sha256:961d03dc3453ebbc59dbdea9e4e11c5651520a876d0f4db161e8674aae935da9
+pymdown-extensions==10.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3539003ff0d5e219ba979d2dc961d18fcad5ac259e66c764482e8347b4c0503c \
+    --hash=sha256:91ca336caf414e1e5e0626feca86e145de9f85a3921a7bcbd32890b51738c428
+python-dateutil==2.9.0.post0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:37dd54208da7e1cd875388217d5e00ebd4179249f90fb72437e91a35459a0ad3 \
+    --hash=sha256:a8b2bc7bffae282281c8140a97d3aa9c14da0b136dfe83f850eea9a5f7470427
 pyyaml-env-tag==0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:70092675bda14fdec33b31ba77e7543de9ddc88f2e5b99160396572d11525bdb \
     --hash=sha256:af31106dec8a4d68c60207c1886031cbf839b68aa7abccdb19868200532c2069
 pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
@@ -271,14 +271,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -292,144 +293,146 @@
     --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
-regex==2023.12.25 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0694219a1d54336fd0445ea382d49d36882415c0134ee1e8332afd1529f0baa5 \
-    --hash=sha256:086dd15e9435b393ae06f96ab69ab2d333f5d65cbe65ca5a3ef0ec9564dfe770 \
-    --hash=sha256:094ba386bb5c01e54e14434d4caabf6583334090865b23ef58e0424a6286d3dc \
-    --hash=sha256:09da66917262d9481c719599116c7dc0c321ffcec4b1f510c4f8a066f8768105 \
-    --hash=sha256:0ecf44ddf9171cd7566ef1768047f6e66975788258b1c6c6ca78098b95cf9a3d \
-    --hash=sha256:0fda75704357805eb953a3ee15a2b240694a9a514548cd49b3c5124b4e2ad01b \
-    --hash=sha256:11a963f8e25ab5c61348d090bf1b07f1953929c13bd2309a0662e9ff680763c9 \
-    --hash=sha256:150c39f5b964e4d7dba46a7962a088fbc91f06e606f023ce57bb347a3b2d4630 \
-    --hash=sha256:1b9d811f72210fa9306aeb88385b8f8bcef0dfbf3873410413c00aa94c56c2b6 \
-    --hash=sha256:1e0eabac536b4cc7f57a5f3d095bfa557860ab912f25965e08fe1545e2ed8b4c \
-    --hash=sha256:22a86d9fff2009302c440b9d799ef2fe322416d2d58fc124b926aa89365ec482 \
-    --hash=sha256:22f3470f7524b6da61e2020672df2f3063676aff444db1daa283c2ea4ed259d6 \
-    --hash=sha256:263ef5cc10979837f243950637fffb06e8daed7f1ac1e39d5910fd29929e489a \
-    --hash=sha256:283fc8eed679758de38fe493b7d7d84a198b558942b03f017b1f94dda8efae80 \
-    --hash=sha256:29171aa128da69afdf4bde412d5bedc335f2ca8fcfe4489038577d05f16181e5 \
-    --hash=sha256:298dc6354d414bc921581be85695d18912bea163a8b23cac9a2562bbcd5088b1 \
-    --hash=sha256:2aae8101919e8aa05ecfe6322b278f41ce2994c4a430303c4cd163fef746e04f \
-    --hash=sha256:2f4e475a80ecbd15896a976aa0b386c5525d0ed34d5c600b6d3ebac0a67c7ddf \
-    --hash=sha256:34e4af5b27232f68042aa40a91c3b9bb4da0eeb31b7632e0091afc4310afe6cb \
-    --hash=sha256:37f8e93a81fc5e5bd8db7e10e62dc64261bcd88f8d7e6640aaebe9bc180d9ce2 \
-    --hash=sha256:3a17d3ede18f9cedcbe23d2daa8a2cd6f59fe2bf082c567e43083bba3fb00347 \
-    --hash=sha256:3b1de218d5375cd6ac4b5493e0b9f3df2be331e86520f23382f216c137913d20 \
-    --hash=sha256:43f7cd5754d02a56ae4ebb91b33461dc67be8e3e0153f593c509e21d219c5060 \
-    --hash=sha256:4558410b7a5607a645e9804a3e9dd509af12fb72b9825b13791a37cd417d73a5 \
-    --hash=sha256:4719bb05094d7d8563a450cf8738d2e1061420f79cfcc1fa7f0a44744c4d8f73 \
-    --hash=sha256:4bfc2b16e3ba8850e0e262467275dd4d62f0d045e0e9eda2bc65078c0110a11f \
-    --hash=sha256:518440c991f514331f4850a63560321f833979d145d7d81186dbe2f19e27ae3d \
-    --hash=sha256:51f4b32f793812714fd5307222a7f77e739b9bc566dc94a18126aba3b92b98a3 \
-    --hash=sha256:531ac6cf22b53e0696f8e1d56ce2396311254eb806111ddd3922c9d937151dae \
-    --hash=sha256:5cd05d0f57846d8ba4b71d9c00f6f37d6b97d5e5ef8b3c3840426a475c8f70f4 \
-    --hash=sha256:5dd58946bce44b53b06d94aa95560d0b243eb2fe64227cba50017a8d8b3cd3e2 \
-    --hash=sha256:60080bb3d8617d96f0fb7e19796384cc2467447ef1c491694850ebd3670bc457 \
-    --hash=sha256:636ba0a77de609d6510235b7f0e77ec494d2657108f777e8765efc060094c98c \
-    --hash=sha256:67d3ccfc590e5e7197750fcb3a2915b416a53e2de847a728cfa60141054123d4 \
-    --hash=sha256:68191f80a9bad283432385961d9efe09d783bcd36ed35a60fb1ff3f1ec2efe87 \
-    --hash=sha256:7502534e55c7c36c0978c91ba6f61703faf7ce733715ca48f499d3dbbd7657e0 \
-    --hash=sha256:7aa47c2e9ea33a4a2a05f40fcd3ea36d73853a2aae7b4feab6fc85f8bf2c9704 \
-    --hash=sha256:7d2af3f6b8419661a0c421584cfe8aaec1c0e435ce7e47ee2a97e344b98f794f \
-    --hash=sha256:7e316026cc1095f2a3e8cc012822c99f413b702eaa2ca5408a513609488cb62f \
-    --hash=sha256:88ad44e220e22b63b0f8f81f007e8abbb92874d8ced66f32571ef8beb0643b2b \
-    --hash=sha256:88d1f7bef20c721359d8675f7d9f8e414ec5003d8f642fdfd8087777ff7f94b5 \
-    --hash=sha256:89723d2112697feaa320c9d351e5f5e7b841e83f8b143dba8e2d2b5f04e10923 \
-    --hash=sha256:8a0ccf52bb37d1a700375a6b395bff5dd15c50acb745f7db30415bae3c2b0715 \
-    --hash=sha256:8c2c19dae8a3eb0ea45a8448356ed561be843b13cbc34b840922ddf565498c1c \
-    --hash=sha256:905466ad1702ed4acfd67a902af50b8db1feeb9781436372261808df7a2a7bca \
-    --hash=sha256:9852b76ab558e45b20bf1893b59af64a28bd3820b0c2efc80e0a70a4a3ea51c1 \
-    --hash=sha256:98a2636994f943b871786c9e82bfe7883ecdaba2ef5df54e1450fa9869d1f756 \
-    --hash=sha256:9aa1a67bbf0f957bbe096375887b2505f5d8ae16bf04488e8b0f334c36e31360 \
-    --hash=sha256:9eda5f7a50141291beda3edd00abc2d4a5b16c29c92daf8d5bd76934150f3edc \
-    --hash=sha256:a6d1047952c0b8104a1d371f88f4ab62e6275567d4458c1e26e9627ad489b445 \
-    --hash=sha256:a9b6d73353f777630626f403b0652055ebfe8ff142a44ec2cf18ae470395766e \
-    --hash=sha256:a9cc99d6946d750eb75827cb53c4371b8b0fe89c733a94b1573c9dd16ea6c9e4 \
-    --hash=sha256:ad83e7545b4ab69216cef4cc47e344d19622e28aabec61574b20257c65466d6a \
-    --hash=sha256:b014333bd0217ad3d54c143de9d4b9a3ca1c5a29a6d0d554952ea071cff0f1f8 \
-    --hash=sha256:b43523d7bc2abd757119dbfb38af91b5735eea45537ec6ec3a5ec3f9562a1c53 \
-    --hash=sha256:b521dcecebc5b978b447f0f69b5b7f3840eac454862270406a39837ffae4e697 \
-    --hash=sha256:b77e27b79448e34c2c51c09836033056a0547aa360c45eeeb67803da7b0eedaf \
-    --hash=sha256:b7a635871143661feccce3979e1727c4e094f2bdfd3ec4b90dfd4f16f571a87a \
-    --hash=sha256:b7fca9205b59c1a3d5031f7e64ed627a1074730a51c2a80e97653e3e9fa0d415 \
-    --hash=sha256:ba1b30765a55acf15dce3f364e4928b80858fa8f979ad41f862358939bdd1f2f \
-    --hash=sha256:ba99d8077424501b9616b43a2d208095746fb1284fc5ba490139651f971d39d9 \
-    --hash=sha256:c25a8ad70e716f96e13a637802813f65d8a6760ef48672aa3502f4c24ea8b400 \
-    --hash=sha256:c3c4a78615b7762740531c27cf46e2f388d8d727d0c0c739e72048beb26c8a9d \
-    --hash=sha256:c40281f7d70baf6e0db0c2f7472b31609f5bc2748fe7275ea65a0b4601d9b392 \
-    --hash=sha256:c7ad32824b7f02bb3c9f80306d405a1d9b7bb89362d68b3c5a9be53836caebdb \
-    --hash=sha256:cb3fe77aec8f1995611f966d0c656fdce398317f850d0e6e7aebdfe61f40e1cd \
-    --hash=sha256:cc038b2d8b1470364b1888a98fd22d616fba2b6309c5b5f181ad4483e0017861 \
-    --hash=sha256:cc37b9aeebab425f11f27e5e9e6cf580be7206c6582a64467a14dda211abc232 \
-    --hash=sha256:cc6bb9aa69aacf0f6032c307da718f61a40cf970849e471254e0e91c56ffca95 \
-    --hash=sha256:d126361607b33c4eb7b36debc173bf25d7805847346dd4d99b5499e1fef52bc7 \
-    --hash=sha256:d15b274f9e15b1a0b7a45d2ac86d1f634d983ca40d6b886721626c47a400bf39 \
-    --hash=sha256:d166eafc19f4718df38887b2bbe1467a4f74a9830e8605089ea7a30dd4da8887 \
-    --hash=sha256:d498eea3f581fbe1b34b59c697512a8baef88212f92e4c7830fcc1499f5b45a5 \
-    --hash=sha256:d6f7e255e5fa94642a0724e35406e6cb7001c09d476ab5fce002f652b36d0c39 \
-    --hash=sha256:d78bd484930c1da2b9679290a41cdb25cc127d783768a0369d6b449e72f88beb \
-    --hash=sha256:d865984b3f71f6d0af64d0d88f5733521698f6c16f445bb09ce746c92c97c586 \
-    --hash=sha256:d902a43085a308cef32c0d3aea962524b725403fd9373dea18110904003bac97 \
-    --hash=sha256:d94a1db462d5690ebf6ae86d11c5e420042b9898af5dcf278bd97d6bda065423 \
-    --hash=sha256:da695d75ac97cb1cd725adac136d25ca687da4536154cdc2815f576e4da11c69 \
-    --hash=sha256:db2a0b1857f18b11e3b0e54ddfefc96af46b0896fb678c85f63fb8c37518b3e7 \
-    --hash=sha256:df26481f0c7a3f8739fecb3e81bc9da3fcfae34d6c094563b9d4670b047312e1 \
-    --hash=sha256:e14b73607d6231f3cc4622809c196b540a6a44e903bcfad940779c80dffa7be7 \
-    --hash=sha256:e2610e9406d3b0073636a3a2e80db05a02f0c3169b5632022b4e81c0364bcda5 \
-    --hash=sha256:e692296c4cc2873967771345a876bcfc1c547e8dd695c6b89342488b0ea55cd8 \
-    --hash=sha256:e693e233ac92ba83a87024e1d32b5f9ab15ca55ddd916d878146f4e3406b5c91 \
-    --hash=sha256:e81469f7d01efed9b53740aedd26085f20d49da65f9c1f41e822a33992cb1590 \
-    --hash=sha256:e8c7e08bb566de4faaf11984af13f6bcf6a08f327b13631d41d62592681d24fe \
-    --hash=sha256:ed19b3a05ae0c97dd8f75a5d8f21f7723a8c33bbc555da6bbe1f96c470139d3c \
-    --hash=sha256:efb2d82f33b2212898f1659fb1c2e9ac30493ac41e4d53123da374c3b5541e64 \
-    --hash=sha256:f44dd4d68697559d007462b0a3a1d9acd61d97072b71f6d1968daef26bc744bd \
-    --hash=sha256:f72cbae7f6b01591f90814250e636065850c5926751af02bb48da94dfced7baa \
-    --hash=sha256:f7bc09bc9c29ebead055bcba136a67378f03d66bf359e87d0f7c759d6d4ffa31 \
-    --hash=sha256:ff100b203092af77d1a5a7abe085b3506b7eaaf9abf65b73b7d6905b6cb76988
+regex==2024.4.16 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00169caa125f35d1bca6045d65a662af0202704489fada95346cfa092ec23f39 \
+    --hash=sha256:03576e3a423d19dda13e55598f0fd507b5d660d42c51b02df4e0d97824fdcae3 \
+    --hash=sha256:03e68f44340528111067cecf12721c3df4811c67268b897fbe695c95f860ac42 \
+    --hash=sha256:0534b034fba6101611968fae8e856c1698da97ce2efb5c2b895fc8b9e23a5834 \
+    --hash=sha256:08dea89f859c3df48a440dbdcd7b7155bc675f2fa2ec8c521d02dc69e877db70 \
+    --hash=sha256:0a38d151e2cdd66d16dab550c22f9521ba79761423b87c01dae0a6e9add79c0d \
+    --hash=sha256:0c8290b44d8b0af4e77048646c10c6e3aa583c1ca67f3b5ffb6e06cf0c6f0f89 \
+    --hash=sha256:10188fe732dec829c7acca7422cdd1bf57d853c7199d5a9e96bb4d40db239c73 \
+    --hash=sha256:1210365faba7c2150451eb78ec5687871c796b0f1fa701bfd2a4a25420482d26 \
+    --hash=sha256:12f6a3f2f58bb7344751919a1876ee1b976fe08b9ffccb4bbea66f26af6017b9 \
+    --hash=sha256:159dc4e59a159cb8e4e8f8961eb1fa5d58f93cb1acd1701d8aff38d45e1a84a6 \
+    --hash=sha256:20b7a68444f536365af42a75ccecb7ab41a896a04acf58432db9e206f4e525d6 \
+    --hash=sha256:23cff1b267038501b179ccbbd74a821ac4a7192a1852d1d558e562b507d46013 \
+    --hash=sha256:2c72608e70f053643437bd2be0608f7f1c46d4022e4104d76826f0839199347a \
+    --hash=sha256:3399dd8a7495bbb2bacd59b84840eef9057826c664472e86c91d675d007137f5 \
+    --hash=sha256:34422d5a69a60b7e9a07a690094e824b66f5ddc662a5fc600d65b7c174a05f04 \
+    --hash=sha256:370c68dc5570b394cbaadff50e64d705f64debed30573e5c313c360689b6aadc \
+    --hash=sha256:3a1018e97aeb24e4f939afcd88211ace472ba566efc5bdf53fd8fd7f41fa7170 \
+    --hash=sha256:3d5ac5234fb5053850d79dd8eb1015cb0d7d9ed951fa37aa9e6249a19aa4f336 \
+    --hash=sha256:4313ab9bf6a81206c8ac28fdfcddc0435299dc88cad12cc6305fd0e78b81f9e4 \
+    --hash=sha256:445ca8d3c5a01309633a0c9db57150312a181146315693273e35d936472df912 \
+    --hash=sha256:479595a4fbe9ed8f8f72c59717e8cf222da2e4c07b6ae5b65411e6302af9708e \
+    --hash=sha256:4918fd5f8b43aa7ec031e0fef1ee02deb80b6afd49c85f0790be1dc4ce34cb50 \
+    --hash=sha256:4aba818dcc7263852aabb172ec27b71d2abca02a593b95fa79351b2774eb1d2b \
+    --hash=sha256:4e819a806420bc010489f4e741b3036071aba209f2e0989d4750b08b12a9343f \
+    --hash=sha256:4facc913e10bdba42ec0aee76d029aedda628161a7ce4116b16680a0413f658a \
+    --hash=sha256:549c3584993772e25f02d0656ac48abdda73169fe347263948cf2b1cead622f3 \
+    --hash=sha256:5c02fcd2bf45162280613d2e4a1ca3ac558ff921ae4e308ecb307650d3a6ee51 \
+    --hash=sha256:5f580c651a72b75c39e311343fe6875d6f58cf51c471a97f15a938d9fe4e0d37 \
+    --hash=sha256:62120ed0de69b3649cc68e2965376048793f466c5a6c4370fb27c16c1beac22d \
+    --hash=sha256:6295004b2dd37b0835ea5c14a33e00e8cfa3c4add4d587b77287825f3418d310 \
+    --hash=sha256:65436dce9fdc0aeeb0a0effe0839cb3d6a05f45aa45a4d9f9c60989beca78b9c \
+    --hash=sha256:684008ec44ad275832a5a152f6e764bbe1914bea10968017b6feaecdad5736e0 \
+    --hash=sha256:684e52023aec43bdf0250e843e1fdd6febbe831bd9d52da72333fa201aaa2335 \
+    --hash=sha256:6cc38067209354e16c5609b66285af17a2863a47585bcf75285cab33d4c3b8df \
+    --hash=sha256:6f2f017c5be19984fbbf55f8af6caba25e62c71293213f044da3ada7091a4455 \
+    --hash=sha256:743deffdf3b3481da32e8a96887e2aa945ec6685af1cfe2bcc292638c9ba2f48 \
+    --hash=sha256:7571f19f4a3fd00af9341c7801d1ad1967fc9c3f5e62402683047e7166b9f2b4 \
+    --hash=sha256:7731728b6568fc286d86745f27f07266de49603a6fdc4d19c87e8c247be452af \
+    --hash=sha256:785c071c982dce54d44ea0b79cd6dfafddeccdd98cfa5f7b86ef69b381b457d9 \
+    --hash=sha256:78fddb22b9ef810b63ef341c9fcf6455232d97cfe03938cbc29e2672c436670e \
+    --hash=sha256:7bb966fdd9217e53abf824f437a5a2d643a38d4fd5fd0ca711b9da683d452969 \
+    --hash=sha256:7cbc5d9e8a1781e7be17da67b92580d6ce4dcef5819c1b1b89f49d9678cc278c \
+    --hash=sha256:803b8905b52de78b173d3c1e83df0efb929621e7b7c5766c0843704d5332682f \
+    --hash=sha256:80b696e8972b81edf0af2a259e1b2a4a661f818fae22e5fa4fa1a995fb4a40fd \
+    --hash=sha256:81500ed5af2090b4a9157a59dbc89873a25c33db1bb9a8cf123837dcc9765047 \
+    --hash=sha256:89ec7f2c08937421bbbb8b48c54096fa4f88347946d4747021ad85f1b3021b3c \
+    --hash=sha256:8ba6745440b9a27336443b0c285d705ce73adb9ec90e2f2004c64d95ab5a7598 \
+    --hash=sha256:8c91e1763696c0eb66340c4df98623c2d4e77d0746b8f8f2bee2c6883fd1fe18 \
+    --hash=sha256:8d015604ee6204e76569d2f44e5a210728fa917115bef0d102f4107e622b08d5 \
+    --hash=sha256:8d1f86f3f4e2388aa3310b50694ac44daefbd1681def26b4519bd050a398dc5a \
+    --hash=sha256:8f83b6fd3dc3ba94d2b22717f9c8b8512354fd95221ac661784df2769ea9bba9 \
+    --hash=sha256:8fc6976a3395fe4d1fbeb984adaa8ec652a1e12f36b56ec8c236e5117b585427 \
+    --hash=sha256:904c883cf10a975b02ab3478bce652f0f5346a2c28d0a8521d97bb23c323cc8b \
+    --hash=sha256:911742856ce98d879acbea33fcc03c1d8dc1106234c5e7d068932c945db209c0 \
+    --hash=sha256:91797b98f5e34b6a49f54be33f72e2fb658018ae532be2f79f7c63b4ae225145 \
+    --hash=sha256:95399831a206211d6bc40224af1c635cb8790ddd5c7493e0bd03b85711076a53 \
+    --hash=sha256:956b58d692f235cfbf5b4f3abd6d99bf102f161ccfe20d2fd0904f51c72c4c66 \
+    --hash=sha256:98c1165f3809ce7774f05cb74e5408cd3aa93ee8573ae959a97a53db3ca3180d \
+    --hash=sha256:9ab40412f8cd6f615bfedea40c8bf0407d41bf83b96f6fc9ff34976d6b7037fd \
+    --hash=sha256:9df1bfef97db938469ef0a7354b2d591a2d438bc497b2c489471bec0e6baf7c4 \
+    --hash=sha256:a01fe2305e6232ef3e8f40bfc0f0f3a04def9aab514910fa4203bafbc0bb4682 \
+    --hash=sha256:a70b51f55fd954d1f194271695821dd62054d949efd6368d8be64edd37f55c86 \
+    --hash=sha256:a7ccdd1c4a3472a7533b0a7aa9ee34c9a2bef859ba86deec07aff2ad7e0c3b94 \
+    --hash=sha256:b340cccad138ecb363324aa26893963dcabb02bb25e440ebdf42e30963f1a4e0 \
+    --hash=sha256:b74586dd0b039c62416034f811d7ee62810174bb70dffcca6439f5236249eb09 \
+    --hash=sha256:b9d320b3bf82a39f248769fc7f188e00f93526cc0fe739cfa197868633d44701 \
+    --hash=sha256:ba2336d6548dee3117520545cfe44dc28a250aa091f8281d28804aa8d707d93d \
+    --hash=sha256:ba8122e3bb94ecda29a8de4cf889f600171424ea586847aa92c334772d200331 \
+    --hash=sha256:bd727ad276bb91928879f3aa6396c9a1d34e5e180dce40578421a691eeb77f47 \
+    --hash=sha256:c21fc21a4c7480479d12fd8e679b699f744f76bb05f53a1d14182b31f55aac76 \
+    --hash=sha256:c2d0e7cbb6341e830adcbfa2479fdeebbfbb328f11edd6b5675674e7a1e37730 \
+    --hash=sha256:c2ef6f7990b6e8758fe48ad08f7e2f66c8f11dc66e24093304b87cae9037bb4a \
+    --hash=sha256:c4ed75ea6892a56896d78f11006161eea52c45a14994794bcfa1654430984b22 \
+    --hash=sha256:cccc79a9be9b64c881f18305a7c715ba199e471a3973faeb7ba84172abb3f317 \
+    --hash=sha256:d0800631e565c47520aaa04ae38b96abc5196fe8b4aa9bd864445bd2b5848a7a \
+    --hash=sha256:d2da13568eff02b30fd54fccd1e042a70fe920d816616fda4bf54ec705668d81 \
+    --hash=sha256:d61ae114d2a2311f61d90c2ef1358518e8f05eafda76eaf9c772a077e0b465ec \
+    --hash=sha256:d83c2bc678453646f1a18f8db1e927a2d3f4935031b9ad8a76e56760461105dd \
+    --hash=sha256:dd5acc0a7d38fdc7a3a6fd3ad14c880819008ecb3379626e56b163165162cc46 \
+    --hash=sha256:df79012ebf6f4efb8d307b1328226aef24ca446b3ff8d0e30202d7ebcb977a8c \
+    --hash=sha256:e0a2df336d1135a0b3a67f3bbf78a75f69562c1199ed9935372b82215cddd6e2 \
+    --hash=sha256:e2f142b45c6fed48166faeb4303b4b58c9fcd827da63f4cf0a123c3480ae11fb \
+    --hash=sha256:e697e1c0238133589e00c244a8b676bc2cfc3ab4961318d902040d099fec7483 \
+    --hash=sha256:e757d475953269fbf4b441207bb7dbdd1c43180711b6208e129b637792ac0b93 \
+    --hash=sha256:e87ab229332ceb127a165612d839ab87795972102cb9830e5f12b8c9a5c1b508 \
+    --hash=sha256:ea355eb43b11764cf799dda62c658c4d2fdb16af41f59bb1ccfec517b60bcb07 \
+    --hash=sha256:ec7e0043b91115f427998febaa2beb82c82df708168b35ece3accb610b91fac1 \
+    --hash=sha256:eeaa0b5328b785abc344acc6241cffde50dc394a0644a968add75fcefe15b9d4 \
+    --hash=sha256:f2d80a6749724b37853ece57988b39c4e79d2b5fe2869a86e8aeae3bbeef9eb0 \
+    --hash=sha256:fa454d26f2e87ad661c4f0c5a5fe4cf6aab1e307d1b94f16ffdfcb089ba685c0 \
+    --hash=sha256:fb83cc090eac63c006871fd24db5e30a1f282faa46328572661c0a24a2323a08 \
+    --hash=sha256:fd80d1280d473500d8086d104962a82d77bfbf2b118053824b7be28cd5a79ea5
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "3.10" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-urllib3==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
-    --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
-watchdog==3.0.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0e06ab8858a76e1219e68c7573dfeba9dd1c0219476c5a44d5333b01d7e1743a \
-    --hash=sha256:13bbbb462ee42ec3c5723e1205be8ced776f05b100e4737518c67c8325cf6100 \
-    --hash=sha256:233b5817932685d39a7896b1090353fc8efc1ef99c9c054e46c8002561252fb8 \
-    --hash=sha256:25f70b4aa53bd743729c7475d7ec41093a580528b100e9a8c5b5efe8899592fc \
-    --hash=sha256:2b57a1e730af3156d13b7fdddfc23dea6487fceca29fc75c5a868beed29177ae \
-    --hash=sha256:336adfc6f5cc4e037d52db31194f7581ff744b67382eb6021c868322e32eef41 \
-    --hash=sha256:3aa7f6a12e831ddfe78cdd4f8996af9cf334fd6346531b16cec61c3b3c0d8da0 \
-    --hash=sha256:3ed7c71a9dccfe838c2f0b6314ed0d9b22e77d268c67e015450a29036a81f60f \
-    --hash=sha256:4c9956d27be0bb08fc5f30d9d0179a855436e655f046d288e2bcc11adfae893c \
-    --hash=sha256:4d98a320595da7a7c5a18fc48cb633c2e73cda78f93cac2ef42d42bf609a33f9 \
-    --hash=sha256:4f94069eb16657d2c6faada4624c39464f65c05606af50bb7902e036e3219be3 \
-    --hash=sha256:5113334cf8cf0ac8cd45e1f8309a603291b614191c9add34d33075727a967709 \
-    --hash=sha256:51f90f73b4697bac9c9a78394c3acbbd331ccd3655c11be1a15ae6fe289a8c83 \
-    --hash=sha256:5d9f3a10e02d7371cd929b5d8f11e87d4bad890212ed3901f9b4d68767bee759 \
-    --hash=sha256:7ade88d0d778b1b222adebcc0927428f883db07017618a5e684fd03b83342bd9 \
-    --hash=sha256:7c5f84b5194c24dd573fa6472685b2a27cc5a17fe5f7b6fd40345378ca6812e3 \
-    --hash=sha256:7e447d172af52ad204d19982739aa2346245cc5ba6f579d16dac4bfec226d2e7 \
-    --hash=sha256:8ae9cda41fa114e28faf86cb137d751a17ffd0316d1c34ccf2235e8a84365c7f \
-    --hash=sha256:8f3ceecd20d71067c7fd4c9e832d4e22584318983cabc013dbf3f70ea95de346 \
-    --hash=sha256:9fac43a7466eb73e64a9940ac9ed6369baa39b3bf221ae23493a9ec4d0022674 \
-    --hash=sha256:a70a8dcde91be523c35b2bf96196edc5730edb347e374c7de7cd20c43ed95397 \
-    --hash=sha256:adfdeab2da79ea2f76f87eb42a3ab1966a5313e5a69a0213a3cc06ef692b0e96 \
-    --hash=sha256:ba07e92756c97e3aca0912b5cbc4e5ad802f4557212788e72a72a47ff376950d \
-    --hash=sha256:c07253088265c363d1ddf4b3cdb808d59a0468ecd017770ed716991620b8f77a \
-    --hash=sha256:c9d8c8ec7efb887333cf71e328e39cffbf771d8f8f95d308ea4125bf5f90ba64 \
-    --hash=sha256:d00e6be486affb5781468457b21a6cbe848c33ef43f9ea4a73b4882e5f188a44 \
-    --hash=sha256:d429c2430c93b7903914e4db9a966c7f2b068dd2ebdd2fa9b9ce094c7d459f33
-zipp==3.17.0 ; python_version >= "3.9" and python_version < "3.10" \
-    --hash=sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31 \
-    --hash=sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+urllib3==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
+watchdog==4.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:11e12fafb13372e18ca1bbf12d50f593e7280646687463dd47730fd4f4d5d257 \
+    --hash=sha256:2895bf0518361a9728773083908801a376743bcc37dfa252b801af8fd281b1ca \
+    --hash=sha256:39cb34b1f1afbf23e9562501673e7146777efe95da24fab5707b88f7fb11649b \
+    --hash=sha256:45cc09cc4c3b43fb10b59ef4d07318d9a3ecdbff03abd2e36e77b6dd9f9a5c85 \
+    --hash=sha256:4986db5e8880b0e6b7cd52ba36255d4793bf5cdc95bd6264806c233173b1ec0b \
+    --hash=sha256:5369136a6474678e02426bd984466343924d1df8e2fd94a9b443cb7e3aa20d19 \
+    --hash=sha256:557ba04c816d23ce98a06e70af6abaa0485f6d94994ec78a42b05d1c03dcbd50 \
+    --hash=sha256:6a4db54edea37d1058b08947c789a2354ee02972ed5d1e0dca9b0b820f4c7f92 \
+    --hash=sha256:6a80d5cae8c265842c7419c560b9961561556c4361b297b4c431903f8c33b269 \
+    --hash=sha256:6a9c71a0b02985b4b0b6d14b875a6c86ddea2fdbebd0c9a720a806a8bbffc69f \
+    --hash=sha256:6c47bdd680009b11c9ac382163e05ca43baf4127954c5f6d0250e7d772d2b80c \
+    --hash=sha256:6e949a8a94186bced05b6508faa61b7adacc911115664ccb1923b9ad1f1ccf7b \
+    --hash=sha256:73c7a935e62033bd5e8f0da33a4dcb763da2361921a69a5a95aaf6c93aa03a87 \
+    --hash=sha256:76ad8484379695f3fe46228962017a7e1337e9acadafed67eb20aabb175df98b \
+    --hash=sha256:8350d4055505412a426b6ad8c521bc7d367d1637a762c70fdd93a3a0d595990b \
+    --hash=sha256:87e9df830022488e235dd601478c15ad73a0389628588ba0b028cb74eb72fed8 \
+    --hash=sha256:8f9a542c979df62098ae9c58b19e03ad3df1c9d8c6895d96c0d51da17b243b1c \
+    --hash=sha256:8fec441f5adcf81dd240a5fe78e3d83767999771630b5ddfc5867827a34fa3d3 \
+    --hash=sha256:9a03e16e55465177d416699331b0f3564138f1807ecc5f2de9d55d8f188d08c7 \
+    --hash=sha256:ba30a896166f0fee83183cec913298151b73164160d965af2e93a20bbd2ab605 \
+    --hash=sha256:c17d98799f32e3f55f181f19dd2021d762eb38fdd381b4a748b9f5a36738e935 \
+    --hash=sha256:c522392acc5e962bcac3b22b9592493ffd06d1fc5d755954e6be9f4990de932b \
+    --hash=sha256:d0f9bd1fd919134d459d8abf954f63886745f4660ef66480b9d753a7c9d40927 \
+    --hash=sha256:d18d7f18a47de6863cd480734613502904611730f8def45fc52a5d97503e5101 \
+    --hash=sha256:d31481ccf4694a8416b681544c23bd271f5a123162ab603c7d7d2dd7dd901a07 \
+    --hash=sha256:e3e7065cbdabe6183ab82199d7a4f6b3ba0a438c5a512a68559846ccb76a78ec \
+    --hash=sha256:eed82cdf79cd7f0232e2fdc1ad05b06a5e102a43e331f7d041e5f0e0a34a51c4 \
+    --hash=sha256:f970663fa4f7e80401a7b0cbeec00fa801bf0287d93d48368fc3e6fa32716245 \
+    --hash=sha256:f9b2fdca47dc855516b2d66eef3c39f2672cbf7e7a42e7e67ad2cbfcd6ba107d
+zipp==3.18.1 ; python_version >= "3.9" and python_version < "3.10" \
+    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
+    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/flake8.txt` & `alluka-0.1.5/piped/python/base-requirements/flake8.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/flake8.in --output-file python/base-requirements/flake8.txt --min-python-version 3.9
 #
-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
-    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
+flake8-pyproject==1.2.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6249fe53545205af5e76837644dc80b4c10037e73a0e5db87ff562d75fb5bd4a
+flake8==7.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
+    --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 pycodestyle==2.11.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
-pyflakes==3.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
-    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
-pyproject-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6da8e5a264395e0148bc11844c6fb50546f1fac83ac9210f7328664135f9e70f \
-    --hash=sha256:86ea5559263c098e1aa4f866776aa2cf45362fd91a576b9fd8fbbbb55db12c4e
+pyflakes==3.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
+    --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/freeze-locks.txt` & `alluka-0.1.5/piped/python/base-requirements/freeze-locks.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/freeze-locks.in --output-file python/base-requirements/freeze-locks.txt --min-python-version 3.9
 #
-attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
-build==0.10.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:af266720050a66c893a6096a2f410989eeac74ff9a68ba194b3f6473e8e26171 \
-    --hash=sha256:d5b71264afdb5951d6704482aac78de887c80691c52b88a9ad195983ca2c9269
-cachecontrol[filecache]==0.13.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:95dedbec849f46dda3137866dc28b9d133fc9af55f5b805ab1291833e4457aa4 \
-    --hash=sha256:f012366b79d2243a6118309ce73151bf52a38d4a5dac8ea57f09bd29087e506b
-certifi==2023.11.17 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
-cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") \
+build==1.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:526263f4870c26f26c433545579475377b2b7588b6f1eac76a001e873ae3e19d \
+    --hash=sha256:75e10f767a433d9a86e50d83f418e83efc18ede923ee5ff7df93b6cb0306c5d4
+cachecontrol[filecache]==0.14.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7db1195b41c81f8274a7bbd97c956f44e8348265a1bc7641c37dfebc39f0c938 \
+    --hash=sha256:f5bf3f0620c38db2e5122c0726bdebb0d16869de966ea6a2befe92470b740ea0
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
+cffi==1.16.0 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") and (sys_platform == "darwin" or platform_python_implementation != "PyPy") \
     --hash=sha256:0c9ef6ff37e974b73c25eecc13952c55bceed9112be2d9d938ded8e856138bcc \
     --hash=sha256:131fd094d1065b19540c3d72594260f118b231090295d8c34e19a7bbcf2e860a \
     --hash=sha256:1b8ebc27c014c59692bb2664c7d13ce7a6e9a629be20e54e7271fa696ff2b417 \
     --hash=sha256:2c56b361916f390cd758a57f2e16233eb4f64bcbeee88a4881ea90fca14dc6ab \
     --hash=sha256:2d92b25dbf6cae33f65005baf472d2c245c050b1ce709cc4588cdcdd5495b520 \
     --hash=sha256:31d13b0f99e0836b7ff893d37af07366ebc90b678b6664c955b54561fc36ef36 \
     --hash=sha256:32c68ef735dbe5857c810328cb2481e24722a59a2003018885514d4c09af9743 \
@@ -165,38 +162,47 @@
     --hash=sha256:4a31bd4dd45695a64ee3c4758f583f134267c2bc518d8ae9a29cf237d009b07e
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and os_name == "nt" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 crashtest==0.4.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:80d7b1f316ebfbd429f648076d6275c877ba30ba48979de4191714a75266f0ce \
     --hash=sha256:8d23eac5fa660409f57472e3851dab7ac18aba459a8d19cbbba86d3d5aecd2a5
-cryptography==41.0.7 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
-    --hash=sha256:079b85658ea2f59c4f43b70f8119a52414cdb7be34da5d019a77bf96d473b960 \
-    --hash=sha256:09616eeaef406f99046553b8a40fbf8b1e70795a91885ba4c96a70793de5504a \
-    --hash=sha256:13f93ce9bea8016c253b34afc6bd6a75993e5c40672ed5405a9c832f0d4a00bc \
-    --hash=sha256:37a138589b12069efb424220bf78eac59ca68b95696fc622b6ccc1c0a197204a \
-    --hash=sha256:3c78451b78313fa81607fa1b3f1ae0a5ddd8014c38a02d9db0616133987b9cdf \
-    --hash=sha256:43f2552a2378b44869fe8827aa19e69512e3245a219104438692385b0ee119d1 \
-    --hash=sha256:48a0476626da912a44cc078f9893f292f0b3e4c739caf289268168d8f4702a39 \
-    --hash=sha256:49f0805fc0b2ac8d4882dd52f4a3b935b210935d500b6b805f321addc8177406 \
-    --hash=sha256:5429ec739a29df2e29e15d082f1d9ad683701f0ec7709ca479b3ff2708dae65a \
-    --hash=sha256:5a1b41bc97f1ad230a41657d9155113c7521953869ae57ac39ac7f1bb471469a \
-    --hash=sha256:68a2dec79deebc5d26d617bfdf6e8aab065a4f34934b22d3b5010df3ba36612c \
-    --hash=sha256:7a698cb1dac82c35fcf8fe3417a3aaba97de16a01ac914b89a0889d364d2f6be \
-    --hash=sha256:841df4caa01008bad253bce2a6f7b47f86dc9f08df4b433c404def869f590a15 \
-    --hash=sha256:90452ba79b8788fa380dfb587cca692976ef4e757b194b093d845e8d99f612f2 \
-    --hash=sha256:928258ba5d6f8ae644e764d0f996d61a8777559f72dfeb2eea7e2fe0ad6e782d \
-    --hash=sha256:af03b32695b24d85a75d40e1ba39ffe7db7ffcb099fe507b39fd41a565f1b157 \
-    --hash=sha256:b640981bf64a3e978a56167594a0e97db71c89a479da8e175d8bb5be5178c003 \
-    --hash=sha256:c5ca78485a255e03c32b513f8c2bc39fedb7f5c5f8535545bdc223a03b24f248 \
-    --hash=sha256:c7f3201ec47d5207841402594f1d7950879ef890c0c495052fa62f58283fde1a \
-    --hash=sha256:d5ec85080cce7b0513cfd233914eb8b7bbd0633f1d1703aa28d1dd5a72f678ec \
-    --hash=sha256:d6c391c021ab1f7a82da5d8d0b3cee2f4b2c455ec86c8aebbc84837a631ff309 \
-    --hash=sha256:e3114da6d7f95d2dee7d3f4eec16dacff819740bbab931aff8648cb13c5ff5e7 \
-    --hash=sha256:f983596065a18a2183e7f79ab3fd4c475205b839e02cbc0efbbf9666c4b3083d
+cryptography==42.0.5 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
+    --hash=sha256:0270572b8bd2c833c3981724b8ee9747b3ec96f699a9665470018594301439ee \
+    --hash=sha256:111a0d8553afcf8eb02a4fea6ca4f59d48ddb34497aa8706a6cf536f1a5ec576 \
+    --hash=sha256:16a48c23a62a2f4a285699dba2e4ff2d1cff3115b9df052cdd976a18856d8e3d \
+    --hash=sha256:1b95b98b0d2af784078fa69f637135e3c317091b615cd0905f8b8a087e86fa30 \
+    --hash=sha256:1f71c10d1e88467126f0efd484bd44bca5e14c664ec2ede64c32f20875c0d413 \
+    --hash=sha256:2424ff4c4ac7f6b8177b53c17ed5d8fa74ae5955656867f5a8affaca36a27abb \
+    --hash=sha256:2bce03af1ce5a5567ab89bd90d11e7bbdff56b8af3acbbec1faded8f44cb06da \
+    --hash=sha256:329906dcc7b20ff3cad13c069a78124ed8247adcac44b10bea1130e36caae0b4 \
+    --hash=sha256:37dd623507659e08be98eec89323469e8c7b4c1407c85112634ae3dbdb926fdd \
+    --hash=sha256:3eaafe47ec0d0ffcc9349e1708be2aaea4c6dd4978d76bf6eb0cb2c13636c6fc \
+    --hash=sha256:5e6275c09d2badf57aea3afa80d975444f4be8d3bc58f7f80d2a484c6f9485c8 \
+    --hash=sha256:6fe07eec95dfd477eb9530aef5bead34fec819b3aaf6c5bd6d20565da607bfe1 \
+    --hash=sha256:7367d7b2eca6513681127ebad53b2582911d1736dc2ffc19f2c3ae49997496bc \
+    --hash=sha256:7cde5f38e614f55e28d831754e8a3bacf9ace5d1566235e39d91b35502d6936e \
+    --hash=sha256:9481ffe3cf013b71b2428b905c4f7a9a4f76ec03065b05ff499bb5682a8d9ad8 \
+    --hash=sha256:98d8dc6d012b82287f2c3d26ce1d2dd130ec200c8679b6213b3c73c08b2b7940 \
+    --hash=sha256:a011a644f6d7d03736214d38832e030d8268bcff4a41f728e6030325fea3e400 \
+    --hash=sha256:a2913c5375154b6ef2e91c10b5720ea6e21007412f6437504ffea2109b5a33d7 \
+    --hash=sha256:a30596bae9403a342c978fb47d9b0ee277699fa53bbafad14706af51fe543d16 \
+    --hash=sha256:b03c2ae5d2f0fc05f9a2c0c997e1bc18c8229f392234e8a0194f202169ccd278 \
+    --hash=sha256:b6cd2203306b63e41acdf39aa93b86fb566049aeb6dc489b70e34bcd07adca74 \
+    --hash=sha256:b7ffe927ee6531c78f81aa17e684e2ff617daeba7f189f911065b2ea2d526dec \
+    --hash=sha256:b8cac287fafc4ad485b8a9b67d0ee80c66bf3574f655d3b97ef2e1082360faf1 \
+    --hash=sha256:ba334e6e4b1d92442b75ddacc615c5476d4ad55cc29b15d590cc6b86efa487e2 \
+    --hash=sha256:ba3e4a42397c25b7ff88cdec6e2a16c2be18720f317506ee25210f6d31925f9c \
+    --hash=sha256:c41fb5e6a5fe9ebcd58ca3abfeb51dffb5d83d6775405305bfa8715b76521922 \
+    --hash=sha256:cd2030f6650c089aeb304cf093f3244d34745ce0cfcc39f20c6fbfe030102e2a \
+    --hash=sha256:cd65d75953847815962c84a4654a84850b2bb4aed3f26fadcc1c13892e1e29f6 \
+    --hash=sha256:e4985a790f921508f36f81831817cbc03b102d643b5fcb81cd33df3fa291a1a1 \
+    --hash=sha256:e807b3188f9eb0eaa7bbb579b462c5ace579f1cedb28107ce8b48a9f7ad3679e \
+    --hash=sha256:f12764b8fffc7a123f641d7d049d382b73f96a34117e0b637b80643169cec8ac \
+    --hash=sha256:f8837fe1d6ac4a8052a9a8ddab256bc006242696f03368a4009be7ee3075cdb7
 distlib==0.3.8 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
 dulwich==0.21.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0fc3078a1ba04c588fabb0969d3530efd5cd1ce2cf248eefb6baf7cbc15fc285 \
     --hash=sha256:10893105c6566fc95bc2a67b61df7cc1e8f9126d02a1df6a8b2b82eb59db8ab9 \
     --hash=sha256:12d61334a575474e707614f2e93d6ed4cdae9eb47214f9277076d9e5615171d3 \
@@ -262,264 +268,231 @@
     --hash=sha256:e84cc606b1f581733df4350ca4070e6a8b30be3662bbb81a590b177d0c996c91 \
     --hash=sha256:ecd315847dea406a4decfa39d388a2521e4e31acde3bd9c2609c989e817c6d62 \
     --hash=sha256:ed60d1f610ef6437586f7768254c2a93820ccbd4cfdac7d182cf2d6e615969bb \
     --hash=sha256:f34bf9b9fa9308376263fd9ac43143c7c09da9bc75037bb75c6c2423a151b92c \
     --hash=sha256:f6c88acb60a1f4d31bd6d13bfba465853b3df940ee4a0f2a3d6c7a0778c705b7 \
     --hash=sha256:fa4d14767cf7a49c9231c2e52cb2a3e90d0c83f843eb6a2ca2b5d81d254cf6b9 \
     --hash=sha256:ffc27fb063f740712e02b4d2f826aee8bbed737ed799962fef625e2ce56e2d29
-filelock==3.13.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
-idna==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
-importlib-metadata==7.0.1 ; python_version >= "3.9" and python_version < "3.12" \
-    --hash=sha256:4805911c3a4ec7c3966410053e9ec6a1fecd629117df5adee56dfc9432a1081e \
-    --hash=sha256:f238736bb06590ae52ac1fab06a3a9ef1d8dce2b7a35b5ab329371d6c8f5d2cc
+fastjsonschema==2.19.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3672b47bc94178c9f23dbb654bf47440155d4db9df5f7bc47643315f9c405cd0 \
+    --hash=sha256:e3126a94bdc4623d3de4485f8d468a12f02a67921315ddc87836d6e456dc789d
+filelock==3.13.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
+importlib-metadata==7.1.0 ; python_version >= "3.9" and python_version < "3.12" \
+    --hash=sha256:30962b96c0c223483ed6cc7280e7f0199feb01a0e40cfae4d4450fc6fab1f570 \
+    --hash=sha256:b78938b926ee8d5f020fc4772d487045805a55ddbad2ecf21c6d60938dc7fcd2
 installer==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:05d1933f0a5ba7d8d6296bb6d5018e7c94fa473ceb10cf198a92ccea19c27b53 \
     --hash=sha256:a26d3e3116289bb08216e0d0f7d925fcef0b0194eedfa0c944bcaaa106c4b631
-jaraco-classes==3.3.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:10afa92b6743f25c0cf5f37c6bb6e18e2c5bb84a16527ccfc0040ea377e7aaeb \
-    --hash=sha256:c063dd08e89217cee02c8d5e5ec560f2c8ce6cdc2fcdc2e68f7b2e5547ed3621
+jaraco-classes==3.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:47a024b51d0239c0dd8c8540c6c7f484be3b8fcf0b2d85c13825780d3b3f3acd \
+    --hash=sha256:f662826b6bed8cace05e7ff873ce0f9283b5c924470fe664fff1c2f00f581790
 jeepney==0.8.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
     --hash=sha256:5efe48d255973902f6badc3ce55e2aa6c5c3b3bc642059ef3a91247bcfcc5806 \
     --hash=sha256:c0a454ad016ca575060802ee4d590dd912e35c122fa04e70306de3d076cce755
-jsonschema==4.17.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0f864437ab8b6076ba6707453ef8f98a6a0d512a80e93f8abdb676f737ecb60d \
-    --hash=sha256:a870ad254da1a8ca84b6a2905cac29d265f805acc57af304784962a2aa6508f6
-keyring==24.3.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4446d35d636e6a10b8bce7caa66913dd9eca5fd222ca03a3d42c38608ac30836 \
-    --hash=sha256:e730ecffd309658a08ee82535a3b5ec4b4c8669a9be11efb66249d8e0aeb9a25
-more-itertools==10.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a \
-    --hash=sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6
-msgpack==1.0.7 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:04ad6069c86e531682f9e1e71b71c1c3937d6014a7c3e9edd2aa81ad58842862 \
-    --hash=sha256:0bfdd914e55e0d2c9e1526de210f6fe8ffe9705f2b1dfcc4aecc92a4cb4b533d \
-    --hash=sha256:1dc93e8e4653bdb5910aed79f11e165c85732067614f180f70534f056da97db3 \
-    --hash=sha256:1e2d69948e4132813b8d1131f29f9101bc2c915f26089a6d632001a5c1349672 \
-    --hash=sha256:235a31ec7db685f5c82233bddf9858748b89b8119bf4538d514536c485c15fe0 \
-    --hash=sha256:27dcd6f46a21c18fa5e5deed92a43d4554e3df8d8ca5a47bf0615d6a5f39dbc9 \
-    --hash=sha256:28efb066cde83c479dfe5a48141a53bc7e5f13f785b92ddde336c716663039ee \
-    --hash=sha256:3476fae43db72bd11f29a5147ae2f3cb22e2f1a91d575ef130d2bf49afd21c46 \
-    --hash=sha256:36e17c4592231a7dbd2ed09027823ab295d2791b3b1efb2aee874b10548b7524 \
-    --hash=sha256:384d779f0d6f1b110eae74cb0659d9aa6ff35aaf547b3955abf2ab4c901c4819 \
-    --hash=sha256:38949d30b11ae5f95c3c91917ee7a6b239f5ec276f271f28638dec9156f82cfc \
-    --hash=sha256:3967e4ad1aa9da62fd53e346ed17d7b2e922cba5ab93bdd46febcac39be636fc \
-    --hash=sha256:3e7bf4442b310ff154b7bb9d81eb2c016b7d597e364f97d72b1acc3817a0fdc1 \
-    --hash=sha256:3f0c8c6dfa6605ab8ff0611995ee30d4f9fcff89966cf562733b4008a3d60d82 \
-    --hash=sha256:484ae3240666ad34cfa31eea7b8c6cd2f1fdaae21d73ce2974211df099a95d81 \
-    --hash=sha256:4a7b4f35de6a304b5533c238bee86b670b75b03d31b7797929caa7a624b5dda6 \
-    --hash=sha256:4cb14ce54d9b857be9591ac364cb08dc2d6a5c4318c1182cb1d02274029d590d \
-    --hash=sha256:4e71bc4416de195d6e9b4ee93ad3f2f6b2ce11d042b4d7a7ee00bbe0358bd0c2 \
-    --hash=sha256:52700dc63a4676669b341ba33520f4d6e43d3ca58d422e22ba66d1736b0a6e4c \
-    --hash=sha256:572efc93db7a4d27e404501975ca6d2d9775705c2d922390d878fcf768d92c87 \
-    --hash=sha256:576eb384292b139821c41995523654ad82d1916da6a60cff129c715a6223ea84 \
-    --hash=sha256:5b0bf0effb196ed76b7ad883848143427a73c355ae8e569fa538365064188b8e \
-    --hash=sha256:5b6ccc0c85916998d788b295765ea0e9cb9aac7e4a8ed71d12e7d8ac31c23c95 \
-    --hash=sha256:5ed82f5a7af3697b1c4786053736f24a0efd0a1b8a130d4c7bfee4b9ded0f08f \
-    --hash=sha256:6d4c80667de2e36970ebf74f42d1088cc9ee7ef5f4e8c35eee1b40eafd33ca5b \
-    --hash=sha256:730076207cb816138cf1af7f7237b208340a2c5e749707457d70705715c93b93 \
-    --hash=sha256:7687e22a31e976a0e7fc99c2f4d11ca45eff652a81eb8c8085e9609298916dcf \
-    --hash=sha256:822ea70dc4018c7e6223f13affd1c5c30c0f5c12ac1f96cd8e9949acddb48a61 \
-    --hash=sha256:84b0daf226913133f899ea9b30618722d45feffa67e4fe867b0b5ae83a34060c \
-    --hash=sha256:85765fdf4b27eb5086f05ac0491090fc76f4f2b28e09d9350c31aac25a5aaff8 \
-    --hash=sha256:8dd178c4c80706546702c59529ffc005681bd6dc2ea234c450661b205445a34d \
-    --hash=sha256:8f5b234f567cf76ee489502ceb7165c2a5cecec081db2b37e35332b537f8157c \
-    --hash=sha256:98bbd754a422a0b123c66a4c341de0474cad4a5c10c164ceed6ea090f3563db4 \
-    --hash=sha256:993584fc821c58d5993521bfdcd31a4adf025c7d745bbd4d12ccfecf695af5ba \
-    --hash=sha256:a40821a89dc373d6427e2b44b572efc36a2778d3f543299e2f24eb1a5de65415 \
-    --hash=sha256:b291f0ee7961a597cbbcc77709374087fa2a9afe7bdb6a40dbbd9b127e79afee \
-    --hash=sha256:b573a43ef7c368ba4ea06050a957c2a7550f729c31f11dd616d2ac4aba99888d \
-    --hash=sha256:b610ff0f24e9f11c9ae653c67ff8cc03c075131401b3e5ef4b82570d1728f8a9 \
-    --hash=sha256:bdf38ba2d393c7911ae989c3bbba510ebbcdf4ecbdbfec36272abe350c454075 \
-    --hash=sha256:bfef2bb6ef068827bbd021017a107194956918ab43ce4d6dc945ffa13efbc25f \
-    --hash=sha256:cab3db8bab4b7e635c1c97270d7a4b2a90c070b33cbc00c99ef3f9be03d3e1f7 \
-    --hash=sha256:cb70766519500281815dfd7a87d3a178acf7ce95390544b8c90587d76b227681 \
-    --hash=sha256:cca1b62fe70d761a282496b96a5e51c44c213e410a964bdffe0928e611368329 \
-    --hash=sha256:ccf9a39706b604d884d2cb1e27fe973bc55f2890c52f38df742bc1d79ab9f5e1 \
-    --hash=sha256:dc43f1ec66eb8440567186ae2f8c447d91e0372d793dfe8c222aec857b81a8cf \
-    --hash=sha256:dd632777ff3beaaf629f1ab4396caf7ba0bdd075d948a69460d13d44357aca4c \
-    --hash=sha256:e45ae4927759289c30ccba8d9fdce62bb414977ba158286b5ddaf8df2cddb5c5 \
-    --hash=sha256:e50ebce52f41370707f1e21a59514e3375e3edd6e1832f5e5235237db933c98b \
-    --hash=sha256:ebbbba226f0a108a7366bf4b59bf0f30a12fd5e75100c630267d94d7f0ad20e5 \
-    --hash=sha256:ec79ff6159dffcc30853b2ad612ed572af86c92b5168aa3fc01a67b0fa40665e \
-    --hash=sha256:f0936e08e0003f66bfd97e74ee530427707297b0d0361247e9b4f59ab78ddc8b \
-    --hash=sha256:f26a07a6e877c76a88e3cecac8531908d980d3d5067ff69213653649ec0f60ad \
-    --hash=sha256:f64e376cd20d3f030190e8c32e1c64582eba56ac6dc7d5b0b49a9d44021b52fd \
-    --hash=sha256:f6ffbc252eb0d229aeb2f9ad051200668fc3a9aaa8994e49f0cb2ffe2b7867e7 \
-    --hash=sha256:f9a7c509542db4eceed3dcf21ee5267ab565a83555c9b88a8109dcecc4709002 \
-    --hash=sha256:ff1d0899f104f3921d94579a5638847f783c9b04f2d5f229392ca77fba5b82fc
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+keyring==24.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:c3327b6ffafc0e8befbdb597cacdb4928ffe5c1212f7645f186e6d9957a898db \
+    --hash=sha256:df38a4d7419a6a60fea5cef1e45a948a3e8430dd12ad88b0f423c5c143906218
+more-itertools==10.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
+    --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
+msgpack==1.0.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e073efcba9ea99db5acef3959efa45b52bc67b61b00823d2a1a6944bf45982 \
+    --hash=sha256:0726c282d188e204281ebd8de31724b7d749adebc086873a59efb8cf7ae27df3 \
+    --hash=sha256:0ceea77719d45c839fd73abcb190b8390412a890df2f83fb8cf49b2a4b5c2f40 \
+    --hash=sha256:114be227f5213ef8b215c22dde19532f5da9652e56e8ce969bf0a26d7c419fee \
+    --hash=sha256:13577ec9e247f8741c84d06b9ece5f654920d8365a4b636ce0e44f15e07ec693 \
+    --hash=sha256:1876b0b653a808fcd50123b953af170c535027bf1d053b59790eebb0aeb38950 \
+    --hash=sha256:1ab0bbcd4d1f7b6991ee7c753655b481c50084294218de69365f8f1970d4c151 \
+    --hash=sha256:1cce488457370ffd1f953846f82323cb6b2ad2190987cd4d70b2713e17268d24 \
+    --hash=sha256:26ee97a8261e6e35885c2ecd2fd4a6d38252246f94a2aec23665a4e66d066305 \
+    --hash=sha256:3528807cbbb7f315bb81959d5961855e7ba52aa60a3097151cb21956fbc7502b \
+    --hash=sha256:374a8e88ddab84b9ada695d255679fb99c53513c0a51778796fcf0944d6c789c \
+    --hash=sha256:376081f471a2ef24828b83a641a02c575d6103a3ad7fd7dade5486cad10ea659 \
+    --hash=sha256:3923a1778f7e5ef31865893fdca12a8d7dc03a44b33e2a5f3295416314c09f5d \
+    --hash=sha256:4916727e31c28be8beaf11cf117d6f6f188dcc36daae4e851fee88646f5b6b18 \
+    --hash=sha256:493c5c5e44b06d6c9268ce21b302c9ca055c1fd3484c25ba41d34476c76ee746 \
+    --hash=sha256:505fe3d03856ac7d215dbe005414bc28505d26f0c128906037e66d98c4e95868 \
+    --hash=sha256:5845fdf5e5d5b78a49b826fcdc0eb2e2aa7191980e3d2cfd2a30303a74f212e2 \
+    --hash=sha256:5c330eace3dd100bdb54b5653b966de7f51c26ec4a7d4e87132d9b4f738220ba \
+    --hash=sha256:5dbf059fb4b7c240c873c1245ee112505be27497e90f7c6591261c7d3c3a8228 \
+    --hash=sha256:5e390971d082dba073c05dbd56322427d3280b7cc8b53484c9377adfbae67dc2 \
+    --hash=sha256:5fbb160554e319f7b22ecf530a80a3ff496d38e8e07ae763b9e82fadfe96f273 \
+    --hash=sha256:64d0fcd436c5683fdd7c907eeae5e2cbb5eb872fafbc03a43609d7941840995c \
+    --hash=sha256:69284049d07fce531c17404fcba2bb1df472bc2dcdac642ae71a2d079d950653 \
+    --hash=sha256:6a0e76621f6e1f908ae52860bdcb58e1ca85231a9b0545e64509c931dd34275a \
+    --hash=sha256:73ee792784d48aa338bba28063e19a27e8d989344f34aad14ea6e1b9bd83f596 \
+    --hash=sha256:74398a4cf19de42e1498368c36eed45d9528f5fd0155241e82c4082b7e16cffd \
+    --hash=sha256:7938111ed1358f536daf311be244f34df7bf3cdedb3ed883787aca97778b28d8 \
+    --hash=sha256:82d92c773fbc6942a7a8b520d22c11cfc8fd83bba86116bfcf962c2f5c2ecdaa \
+    --hash=sha256:83b5c044f3eff2a6534768ccfd50425939e7a8b5cf9a7261c385de1e20dcfc85 \
+    --hash=sha256:8db8e423192303ed77cff4dce3a4b88dbfaf43979d280181558af5e2c3c71afc \
+    --hash=sha256:9517004e21664f2b5a5fd6333b0731b9cf0817403a941b393d89a2f1dc2bd836 \
+    --hash=sha256:95c02b0e27e706e48d0e5426d1710ca78e0f0628d6e89d5b5a5b91a5f12274f3 \
+    --hash=sha256:99881222f4a8c2f641f25703963a5cefb076adffd959e0558dc9f803a52d6a58 \
+    --hash=sha256:9ee32dcb8e531adae1f1ca568822e9b3a738369b3b686d1477cbc643c4a9c128 \
+    --hash=sha256:a22e47578b30a3e199ab067a4d43d790249b3c0587d9a771921f86250c8435db \
+    --hash=sha256:b5505774ea2a73a86ea176e8a9a4a7c8bf5d521050f0f6f8426afe798689243f \
+    --hash=sha256:bd739c9251d01e0279ce729e37b39d49a08c0420d3fee7f2a4968c0576678f77 \
+    --hash=sha256:d16a786905034e7e34098634b184a7d81f91d4c3d246edc6bd7aefb2fd8ea6ad \
+    --hash=sha256:d3420522057ebab1728b21ad473aa950026d07cb09da41103f8e597dfbfaeb13 \
+    --hash=sha256:d56fd9f1f1cdc8227d7b7918f55091349741904d9520c65f0139a9755952c9e8 \
+    --hash=sha256:d661dc4785affa9d0edfdd1e59ec056a58b3dbb9f196fa43587f3ddac654ac7b \
+    --hash=sha256:dfe1f0f0ed5785c187144c46a292b8c34c1295c01da12e10ccddfc16def4448a \
+    --hash=sha256:e1dd7839443592d00e96db831eddb4111a2a81a46b028f0facd60a09ebbdd543 \
+    --hash=sha256:e2872993e209f7ed04d963e4b4fbae72d034844ec66bc4ca403329db2074377b \
+    --hash=sha256:e2f879ab92ce502a1e65fce390eab619774dda6a6ff719718069ac94084098ce \
+    --hash=sha256:e3aa7e51d738e0ec0afbed661261513b38b3014754c9459508399baf14ae0c9d \
+    --hash=sha256:e532dbd6ddfe13946de050d7474e3f5fb6ec774fbb1a188aaf469b08cf04189a \
+    --hash=sha256:e6b7842518a63a9f17107eb176320960ec095a8ee3b4420b5f688e24bf50c53c \
+    --hash=sha256:e75753aeda0ddc4c28dce4c32ba2f6ec30b1b02f6c0b14e547841ba5b24f753f \
+    --hash=sha256:eadb9f826c138e6cf3c49d6f8de88225a3c0ab181a9b4ba792e006e5292d150e \
+    --hash=sha256:ed59dd52075f8fc91da6053b12e8c89e37aa043f8986efd89e61fae69dc1b011 \
+    --hash=sha256:ef254a06bcea461e65ff0373d8a0dd1ed3aa004af48839f002a0c994a6f72d04 \
+    --hash=sha256:f3709997b228685fe53e8c433e2df9f0cdb5f4542bd5114ed17ac3c0129b0480 \
+    --hash=sha256:f51bab98d52739c50c56658cc303f190785f9a2cd97b823357e7aeae54c8f68a \
+    --hash=sha256:f9904e24646570539a8950400602d66d2b2c492b9010ea7e965025cb71d0c86d \
+    --hash=sha256:f9af38a89b6a5c04b7d18c492c8ccf2aee7048aff1ce8437c4683bb5a1df893d
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pexpect==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7236d1e080e4936be2dc3e326cec0af72acf9212a7e1d060210e70a47e253523 \
     --hash=sha256:ee7d41123f3c9911050ea2c2dac107568dc43b2d3b0c7557a33212c398ead30f
-pip-compile-cross-platform==1.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6737478e4fe959a220165ea83b89dc07244e8c18a8f6b5c91f4a496ce25a681d \
-    --hash=sha256:a6d50dcab8d375889302bebeef22da83a439d2a0da327cb65e1ff60c1197d1d7
+pip-compile-cross-platform==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:06910a8cd91bf184f93687373ce1ce099b5b35cafe3c1717dae783f78a9d2760 \
+    --hash=sha256:a0382d46c55cadf5f9fcaa63a0f80c16ce01c68f7859619f47b9fcf5d2c34c90
 pip-requirements-parser==32.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4659bc2a667783e7a15d190f6fccf8b2486685b6dba4c19c3876314769c57526 \
     --hash=sha256:b4fa3a7a0be38243123cf9d1f3518da10c51bdb165a2b2985566247f9155a7d3
-pkginfo==1.9.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4b7a555a6d5a22169fcc9cf7bfd78d296b0361adad412a346c1226849af5e546 \
-    --hash=sha256:8fd5896e8718a4372f0ea9cc9d96f6417c9b986e23a4d116dda26b62cc29d046
-platformdirs==3.11.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cf8ee52a3afdb965072dcc652433e0c7e3e40cf5ea1477cd4b3b1d2eb75495b3 \
-    --hash=sha256:e9d171d00af68be50e9202731309c4e658fd8bc76f55c11c7dd760d023bda68e
-poetry-core==1.7.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:38e174cdb00a84ee4a1cab66a378b435747f72414f5573bc18cfc3850a94df38 \
-    --hash=sha256:8f679b83bd9c820082637beca1204124d5d2a786e4818da47ec8acefd0353b74
-poetry-plugin-export==1.5.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cd8267597970375ca29868daec5e7718bad500c7584663af3eeb0ed16f24e2bd \
-    --hash=sha256:ecc8738da0c81c3758e36b4e72e04ae59648a547492af2ffe6245af3594bb00f
-poetry==1.6.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0ab9b1a592731cc8b252b8d6aaeea19c72cc0a109d7468b829ad57e6c48039d2 \
-    --hash=sha256:9b4cb6079c08cc0d91e8cba18a6bd4d4f7d7830263a7fb18ecb3faa77937c988
+pkginfo==1.10.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5df73835398d10db79f8eecd5cd86b1f6d29317589ea70796994d49399af6297 \
+    --hash=sha256:889a6da2ed7ffc58ab5b900d888ddce90bce912f2d2de1dc1c26f4cb9fe65097
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+poetry-core==1.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4e0c9c6ad8cf89956f03b308736d84ea6ddb44089d16f2adc94050108ec1f5a1 \
+    --hash=sha256:fa7a4001eae8aa572ee84f35feb510b321bd652e5cf9293249d62853e1f935a2
+poetry-plugin-export==1.7.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:b2258e53ae0d369a73806f957ed0e726eb95c571a0ce8b1f273da686528cc1da \
+    --hash=sha256:cf62cfb6218a904290ba6db3bc1a24aa076d10f81c48c6e48b2ded430131e22e
+poetry==1.8.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:49cceb3838104647c3e1021f3a4f13c6053704cc18d33f849a90fe687a29cb73 \
+    --hash=sha256:b42b400d9a803af6e788a30a6f3e9998020b77860e28df20647eb10b6f414910
 ptyprocess==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4b41f3967fce3af57cc7e94b888626c18bf37a083e3651ca8feeb66d492fef35 \
     --hash=sha256:5c5d0a3b48ceee0b48485e0c26037c0acd7d29765ca3fbb5cb3831d347423220
-pycparser==2.21 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") \
-    --hash=sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9 \
-    --hash=sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206
-pyparsing==3.1.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:32c7c0b711493c72ff18a981d24f28aaf9c1fb7ed5e9667c9e84e3db623bdbfb \
-    --hash=sha256:ede28a1a32462f5a9705e07aea48001a08f7cf81a021585011deba701581a0db
+pycparser==2.22 ; python_version >= "3.9" and python_version < "4.0" and (sys_platform == "darwin" or sys_platform == "linux") and (sys_platform == "darwin" or platform_python_implementation != "PyPy") \
+    --hash=sha256:491c8be9c040f5390f5bf44a5b07752bd07f56edf992381b05c701439eec10f6 \
+    --hash=sha256:c3702b6d3dd8c7abc1afa565d7e63d53a1d0bd86cdc24edd75470f4de499cfcc
+pyparsing==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a1bac0ce561155ecc3ed78ca94d3c9378656ad4c94c1270de543f621420f94ad \
+    --hash=sha256:f9db75911801ed778fe61bb643079ff86601aca99fcae6345aa67292038fb742
 pyproject-hooks==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:283c11acd6b928d2f6a7c73fa0d01cb2bdc5f07c57a2eeb6e83d5e56b97976f8 \
     --hash=sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5
-pyrsistent==0.20.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0724c506cd8b63c69c7f883cc233aac948c1ea946ea95996ad8b1380c25e1d3f \
-    --hash=sha256:09848306523a3aba463c4b49493a760e7a6ca52e4826aa100ee99d8d39b7ad1e \
-    --hash=sha256:0f3b1bcaa1f0629c978b355a7c37acd58907390149b7311b5db1b37648eb6958 \
-    --hash=sha256:21cc459636983764e692b9eba7144cdd54fdec23ccdb1e8ba392a63666c60c34 \
-    --hash=sha256:2e14c95c16211d166f59c6611533d0dacce2e25de0f76e4c140fde250997b3ca \
-    --hash=sha256:2e2c116cc804d9b09ce9814d17df5edf1df0c624aba3b43bc1ad90411487036d \
-    --hash=sha256:4021a7f963d88ccd15b523787d18ed5e5269ce57aa4037146a2377ff607ae87d \
-    --hash=sha256:4c48f78f62ab596c679086084d0dd13254ae4f3d6c72a83ffdf5ebdef8f265a4 \
-    --hash=sha256:4f5c2d012671b7391803263419e31b5c7c21e7c95c8760d7fc35602353dee714 \
-    --hash=sha256:58b8f6366e152092194ae68fefe18b9f0b4f89227dfd86a07770c3d86097aebf \
-    --hash=sha256:59a89bccd615551391f3237e00006a26bcf98a4d18623a19909a2c48b8e986ee \
-    --hash=sha256:5cdd7ef1ea7a491ae70d826b6cc64868de09a1d5ff9ef8d574250d0940e275b8 \
-    --hash=sha256:6288b3fa6622ad8a91e6eb759cfc48ff3089e7c17fb1d4c59a919769314af224 \
-    --hash=sha256:6d270ec9dd33cdb13f4d62c95c1a5a50e6b7cdd86302b494217137f760495b9d \
-    --hash=sha256:79ed12ba79935adaac1664fd7e0e585a22caa539dfc9b7c7c6d5ebf91fb89054 \
-    --hash=sha256:7d29c23bdf6e5438c755b941cef867ec2a4a172ceb9f50553b6ed70d50dfd656 \
-    --hash=sha256:8441cf9616d642c475684d6cf2520dd24812e996ba9af15e606df5f6fd9d04a7 \
-    --hash=sha256:881bbea27bbd32d37eb24dd320a5e745a2a5b092a17f6debc1349252fac85423 \
-    --hash=sha256:8c3aba3e01235221e5b229a6c05f585f344734bd1ad42a8ac51493d74722bbce \
-    --hash=sha256:a14798c3005ec892bbada26485c2eea3b54109cb2533713e355c806891f63c5e \
-    --hash=sha256:b14decb628fac50db5e02ee5a35a9c0772d20277824cfe845c8a8b717c15daa3 \
-    --hash=sha256:b318ca24db0f0518630e8b6f3831e9cba78f099ed5c1d65ffe3e023003043ba0 \
-    --hash=sha256:c1beb78af5423b879edaf23c5591ff292cf7c33979734c99aa66d5914ead880f \
-    --hash=sha256:c55acc4733aad6560a7f5f818466631f07efc001fd023f34a6c203f8b6df0f0b \
-    --hash=sha256:ca52d1ceae015859d16aded12584c59eb3825f7b50c6cfd621d4231a6cc624ce \
-    --hash=sha256:cae40a9e3ce178415040a0383f00e8d68b569e97f31928a3a8ad37e3fde6df6a \
-    --hash=sha256:e78d0c7c1e99a4a45c99143900ea0546025e41bb59ebc10182e947cf1ece9174 \
-    --hash=sha256:ef3992833fbd686ee783590639f4b8343a57f1f75de8633749d984dc0eb16c86 \
-    --hash=sha256:f058a615031eea4ef94ead6456f5ec2026c19fb5bd6bfe86e9665c4158cf802f \
-    --hash=sha256:f5ac696f02b3fc01a710427585c855f65cd9c640e14f52abe52020722bb4906b \
-    --hash=sha256:f920385a11207dc372a028b3f1e1038bb244b3ec38d448e6d8e43c6b3ba20e98 \
-    --hash=sha256:fed2c3216a605dc9a6ea50c7e84c82906e3684c4e80d2908208f662a6cbf9022
 pywin32-ctypes==0.2.2 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" \
     --hash=sha256:3426e063bdd5fd4df74a14fa3cf80a0b42845a87e1d1e81f6549f9daec593a60 \
     --hash=sha256:bf490a1a709baf35d688fe0ecf980ed4de11d2b3e37b51e5442587a75d9957e7
-rapidfuzz==3.6.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:029ae17bbe55671884702adc16225ca25ca447f86c1dba95b564fcd51eb82d44 \
-    --hash=sha256:0c8d8e72030c7ad2b486a6cdcb0af7b51c0041db1e9e0e6c41fa3e3d244df284 \
-    --hash=sha256:12eaf1aed5b0ded8c4b638a892b4fda53bf6f9f2d8597d8507ba6d697a34170a \
-    --hash=sha256:17b23ef8fae6aa08fe0a02b9e171ef6443ad876bebfdab8d491e07942e36bca6 \
-    --hash=sha256:187751b2b5c4e5b53ea4c30bcbdf6f545dbd985808c0750f990152e95357638f \
-    --hash=sha256:19159a69f9d1132cffeb5fcea344f09ec02212654b92a913c9d3deaf3d387f46 \
-    --hash=sha256:195cc2a216223ff6118a1eb6cddb077cd264bc828ba7064ebb6e3bc61dd9d864 \
-    --hash=sha256:1ed25d6d7b184725bd26ecfe64dfe6a17d261705435e7c38415499b1316120a9 \
-    --hash=sha256:1f2ecf1e23ee64a7cdce01be1350b977169ac866d27f7301a3add21993163b68 \
-    --hash=sha256:23b278a7d8f2cdc1a54cf9b72a48f76dc9f1b68373f2a3299f8b6cc5e796c160 \
-    --hash=sha256:25d98d242e7626c577ab702902040afb87e257ee93c9575884f82e6e7b4aaec0 \
-    --hash=sha256:26c671bd3f2954df7e3d9635d5870177ba7d7433ec610bc3d4ba75648d89b9e9 \
-    --hash=sha256:2a317f1a7c318957bd5ca54bf8258263936320c49857fac69c5ed0b10c81ef0d \
-    --hash=sha256:2a31a6f6442219bb494a4d5293abb106f95adfdbad3fef597377f7344883afa9 \
-    --hash=sha256:2a3c44bafd6d919ccf3f36d454c3e70cafc4c1aa8557970befbb9ae4930e32d7 \
-    --hash=sha256:2dfba991ea3e9963a1d24946f7932893384a64369bf3c28c6d07eb8ee4c4fc86 \
-    --hash=sha256:2e96db4dfd4bf853898438dbf821c5017229aa8064b4b9a12a4bc7ff3112aa1e \
-    --hash=sha256:306ca0358fc7d2e4660de3fce782bfea9c6bf443d60f9134ea8d4b8e8f1869e3 \
-    --hash=sha256:346422d616bdc9d90c2d800f963cde370c4bdc3b99ea1d9bd7b16d43f88d4313 \
-    --hash=sha256:392effa32f235b2b30c9f00ece8002e21255fbbffa0ce0d4a1cbcbb88e02d019 \
-    --hash=sha256:3bf1f610954ec936d87d58eb0247af61e35c41a92c30f3cfe0478baf764558bf \
-    --hash=sha256:3fce2489072ae2362abeabdc7745a5b9eb0ff4291c7a69be2318025e1184f016 \
-    --hash=sha256:40e381099e36df52e073abe18aa24e9ace17b7800c2b38d7818b9c77ba22a622 \
-    --hash=sha256:454ecaf9bd547b8a7ff8f461f5b25bd60ec15800ff2fab562e663732f53f0829 \
-    --hash=sha256:48314743e61394e6418cec38a5389dd3ad6c1b33fc15d525898a303450f958e7 \
-    --hash=sha256:4c1de6260975d5589374abca04a76c3e968907ccdc6daf5f9dd2b4cca1a7a64d \
-    --hash=sha256:4c9c495ebe81a2996cb737060181703822215360abdd60a619839397667f8e4e \
-    --hash=sha256:4cdf564c3eeb2d95148bd7199e7869fa927f47cc3aea42f299aa836cfb2b6cfd \
-    --hash=sha256:4d58f3fd98495d3597137056eb88372ac9360b74a46ab298115230f259e1efa2 \
-    --hash=sha256:4d67f9f180faf341bc04be4f633707b773844a9c07f21dd2eabc27ea54591c8e \
-    --hash=sha256:4ea93d044eaf0d0204a088dbaab18ce2cda1bb0738062c8d2834a8b3832f496c \
-    --hash=sha256:514b15338b7f59b80bbe014d1ffc0093d17abf96f82eb20d8bb573ce24d84a12 \
-    --hash=sha256:52ecaa0619248cc0faa098cc8fa96a65296a9b734f2e8cd509a2cf1358041ae5 \
-    --hash=sha256:5475ea451df17a802c3f78c58f63701c2e99762ce71b9953c2a8da574f450807 \
-    --hash=sha256:583f9cca4e53b5ff93f86a9cf5ca15a6fed3094a2b49acaa3851b4eb00ea04f9 \
-    --hash=sha256:5d7e82a29af3c8052f78c9b2d98a0586ebd6bf41f27298b92b80293c6506e1d7 \
-    --hash=sha256:606eb61b04f1f023048dae46e9a002354bde304a192d3b7f6fcc6e75d3910879 \
-    --hash=sha256:62be08cdd370cc491b594b80493850cf83aafec938b3ca2c98fc4d45667baac8 \
-    --hash=sha256:67a97425abac462e0cb6be02a9adf581577d72e18aa922ef121400e203273657 \
-    --hash=sha256:68dd5912a1b0cc145a674aa45513d595fd6691b263f860d00ac71388ebde09bc \
-    --hash=sha256:6be8fd7b7a39cb2655a0d216da8fc424bc334cfe43f1dcf00fbc3e0426252a35 \
-    --hash=sha256:708457ab87c6eb2aec6f278697b03e088744623c63f450bae2571ce8f29e37d2 \
-    --hash=sha256:76e3d6507ce10696765709093cdedfc814e64960535dcd4f684564c02b6e6d07 \
-    --hash=sha256:7927fff9dd2a34522704c665f9846e0f13e1824f014af8f14294858921bed731 \
-    --hash=sha256:7c1eccce1125676537322d7bc14ecb917b6464700ea222703e131ccb9d165658 \
-    --hash=sha256:82db5d39f9d87b639a23d700200fea379916114d5352e9574d1a11f82b9d8bca \
-    --hash=sha256:834d9bd0fca92fb5cd92a7027df5d0492c3d3c2111f365dc8168f5a2f2582a36 \
-    --hash=sha256:863c6ee97d156026bc1685fb7878c440833c221e935474e5b0ffb255b0888356 \
-    --hash=sha256:88813871a373dc600a8ac831b6900ff57c9ed72e61128e065190e30c502b2e7a \
-    --hash=sha256:8a5087f5c0b4e8584cd6044c279b4a6df15420a0074bf914e50bdebc9ac4db77 \
-    --hash=sha256:8b6205e8d730e0ad3e0472b4fde8f93c740c2165a198ab0ad457e35371b28e08 \
-    --hash=sha256:8ee4151e1ca81cdc8247847d8e041f2ed9e087d550bc21088506b1599c4c842a \
-    --hash=sha256:90fb0e1f931031a0fa967d77d8be21220d5b8e626546d3e774dc28c5a0aea10d \
-    --hash=sha256:9557792003addc7e141e63fd60edc8d77bbd983c212f0f1683bf542cb0d396d9 \
-    --hash=sha256:96d46e9664c53b07f446ceb0f09973a46766e0fd4a26904e75f067ed78f07db2 \
-    --hash=sha256:9a09731ed953126ac3f89f5a8d4998f93eca8a81e41e57b173edc3e44f0afd20 \
-    --hash=sha256:9a743db763cba0aad39e8c8c6a6d1210247cb468f514891632211adad3935a29 \
-    --hash=sha256:a0271e194a5c811db02c7350a119cabde6757587312c70247f6e50984ce36144 \
-    --hash=sha256:a0938400bb41f738809aae6cd9b4d9985ec2c8cfb34c4931c5a16dba76edf58c \
-    --hash=sha256:a09cdfd9c1a11a91e207df138aa2e20a9267cf5f7cde6e9a53a4551454b06333 \
-    --hash=sha256:a14ebea5e14b3b8c91c02be8adf9397247397f1f2be7e9cb6962ded9cc4d2cba \
-    --hash=sha256:a1d8640e1cad1757378a810c363695822462f331c40b23f30c1bbbc477d77c68 \
-    --hash=sha256:a3aec96905badee77915f6cd791019aa06376b252ca4da3676339c4f8dd64e8f \
-    --hash=sha256:a40e52fcd1b61421de465113624bc802546b106fa02aa28b001b0db493651fd1 \
-    --hash=sha256:a5801f45fb585c21b6dbe08658a0d38e08ddca7b1ffb3825f39a59bb78998529 \
-    --hash=sha256:a5a76e488060fde32bfd2dc789821da95ca172a718752d0e65a2b168c7742612 \
-    --hash=sha256:a6ae64784f0e8a7f989e0d24a401fce68fbe37b9e0d61c24ec983828b1dee768 \
-    --hash=sha256:a829e8486988889d6a316f528d92364a88c11a10fb53a8b981ae9cd52ab5846b \
-    --hash=sha256:a99dc8dc8c2d6da1f5b15c9364bcad262f23da098e7bbd54056bee087423d74d \
-    --hash=sha256:ac328c83d49811b36e2699d5132193c5a82139e1a3d0b340babc1bce7428754e \
-    --hash=sha256:ac480cdef530a5a9c8e560e5f77783f3dccd65373e0a09dabe32446e212ea3c4 \
-    --hash=sha256:adbc4686e7252b97ef344fb9fb05080c8524ac2e77a20e835d166b8330024ac3 \
-    --hash=sha256:b21e65818a7e4846bacfa1bd77bc337b02107cc88a7b262dbaeb7944e0c8958d \
-    --hash=sha256:b54cd11ee89b606252c90c5eb711eb6735e2b63305cc8c2e70479166017733a3 \
-    --hash=sha256:b89591f5eb1c3a7509a5294bfd65b3eaca7ee7e0583bdd84122e2fc2e37e6973 \
-    --hash=sha256:b9b7baab3245df24447c5dbd6d6ca4ce400e3bb088ffe6c994407c16852157b6 \
-    --hash=sha256:bc6604d6f1be13d9fb6b01442805ae2ec3bcccc54247ecabba8d3712aff9685a \
-    --hash=sha256:be2e2b96ea1fcefe0a2ed2560fd33a510dc8afe8e93062e111b40d1cb0e34b6a \
-    --hash=sha256:c715df0f21116e830c666d35ea413d528501c50079079ecaa5904ec244661992 \
-    --hash=sha256:cb2ddc1afe32fc8d70dc37d825a04ab1df98a91f40ad6b17d976c5b6fbd99130 \
-    --hash=sha256:d7a4b458096be3b39bf5778e26ac96ac10399b8e4fd40a03fd55a155c093acf5 \
-    --hash=sha256:d920bead489ff2f02893261dd180f2c24afa4f0d00ec24b6b31311966e02f66f \
-    --hash=sha256:da1f2cff6f0128f1ff7c2745051a87f3cd8946036d4036a9dc464868ad5d3a53 \
-    --hash=sha256:db23d692ba27f58e5b97c724005e6a478168cb41af5d793bbc5478cb52842306 \
-    --hash=sha256:e4ba08ba184e530a770b0fc8897f4ce77ae0863039e139ef3180502b37586fec \
-    --hash=sha256:f4378ad75d176c067dc9f79898a8b767305cfac97712f769859b118164852893 \
-    --hash=sha256:f70743f5626743dfab402697953ce0e9458d52000a2d5f52ae0e110facfd62bd \
-    --hash=sha256:f916630b388d465ab54bb205398abbb38b3f8eeed8f224accee534271ca52fba \
-    --hash=sha256:fad2c70768f83a1f202c191f0e4a3ef3d376659728a4602b22dc62bd7f118973 \
-    --hash=sha256:fcf2ab337b7d331c6cbe7a5296b9f703666e7c1b00771a1dbac6e2d62e46b9a4
+rapidfuzz==3.8.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00b5ee47b387fa3805f4038362a085ec58149135dc5bc640ca315a9893a16f9e \
+    --hash=sha256:0798e32304b8009d215026bf7e1c448f1831da0a03987b7de30059a41bee92f3 \
+    --hash=sha256:07d7d4a3c49a15146d65f06e44d7545628ca0437c929684e32ef122852f44d95 \
+    --hash=sha256:14791324f0c753f5a0918df1249b91515f5ddc16281fbaa5ec48bff8fa659229 \
+    --hash=sha256:16153a97efacadbd693ccc612a3285df2f072fd07c121f30c2c135a709537075 \
+    --hash=sha256:17d79398849c1244f646425cf31d856eab9ebd67b7d6571273e53df724ca817e \
+    --hash=sha256:1905d9319a97bed29f21584ca641190dbc9218a556202b77876f1e37618d2e03 \
+    --hash=sha256:1b176f01490b48337183da5b4223005bc0c2354a4faee5118917d2fba0bedc1c \
+    --hash=sha256:1c0264d03dcee1bb975975b77c2fe041820fb4d4a25a99e3cb74ddd083d671ca \
+    --hash=sha256:1d5592b08e3cadc9e06ef3af6a9d66b6ef1bf871ed5acd7f9b1e162d78806a65 \
+    --hash=sha256:1edafc0a2737df277d3ddf401f3a73f76e246b7502762c94a3916453ae67e9b1 \
+    --hash=sha256:1ef119fc127c982053fb9ec638dcc3277f83b034b5972eb05941984b9ec4a290 \
+    --hash=sha256:2084193fd8fd346db496a2220363437eb9370a06d1d5a7a9dba00a64390c6a28 \
+    --hash=sha256:209bb712c448cdec4def6260b9f059bd4681ec61a01568f5e70e37bfe9efe830 \
+    --hash=sha256:231dc1cb63b1c8dd78c0597aa3ad3749a86a2b7e76af295dd81609522699a558 \
+    --hash=sha256:25498650e30122f4a5ad6b27c7614b4af8628c1d32b19d406410d33f77a86c80 \
+    --hash=sha256:267ff42370e031195e3020fff075420c136b69dc918ecb5542ec75c1e36af81f \
+    --hash=sha256:2a8a007fdc5cf646e48e361a39eabe725b93af7673c5ab90294e551cae72ff58 \
+    --hash=sha256:2ba0e43e9a94d256a704a674c7010e6f8ef9225edf7287cf3e7f66c9894b06cd \
+    --hash=sha256:2c6a43446f0cd8ff347b1fbb918dc0d657bebf484ddfa960ee069e422a477428 \
+    --hash=sha256:30c282612b7ebf2d7646ebebfd98dd308c582246a94d576734e4b0162f57baf4 \
+    --hash=sha256:313bdcd16e9cd5e5568b4a31d18a631f0b04cc10a3fd916e4ef75b713e6f177e \
+    --hash=sha256:392582aa784737d95255ca122ebe7dca3c774da900d100c07b53d32cd221a60e \
+    --hash=sha256:3aff3b829b0b04bdf78bd780ec9faf5f26eac3591df98c35a0ae216c925ae436 \
+    --hash=sha256:3fee62ae76e3b8b9fff8aa2ca4061575ee358927ffbdb2919a8c84a98da59f78 \
+    --hash=sha256:41219536634bd6f85419f38450ef080cfb519638125d805cf8626443e677dc61 \
+    --hash=sha256:48b6e5a337a814aec7c6dda5d6460f947c9330860615301f35b519e16dde3c77 \
+    --hash=sha256:4969fe0eb179aedacee53ca8f8f1be3c655964a6d62db30f247fee444b9c52b4 \
+    --hash=sha256:4d5cd86aca3f12e73bfc70015db7e8fc44122da03aa3761138b95112e83f66e4 \
+    --hash=sha256:50db3867864422bf6a6435ea65b9ac9de71ef52ed1e05d62f498cd430189eece \
+    --hash=sha256:58999b21d01dd353f49511a61937eac20c7a5b22eab87612063947081855d85f \
+    --hash=sha256:5f4174079dfe8ed1f13ece9bde7660f19f98ab17e0c0d002d90cc845c3a7e238 \
+    --hash=sha256:63044a7b6791a2e945dce9d812a6886e93159deb0464984eb403617ded257f08 \
+    --hash=sha256:63db612bb6da1bb9f6aa7412739f0e714b1910ec07bc675943044fe683ef192c \
+    --hash=sha256:68b185a0397aebe78bcc5d0e1efd96509d4e2f3c4a05996e5c843732f547e9ef \
+    --hash=sha256:6d4f1956fe1fc618e34ac79a6ed84fff5a6f23e41a8a476dd3e8570f0b12f02b \
+    --hash=sha256:6f34a541895627c2bc9ef7757f16f02428a08d960d33208adfb96b33338d0945 \
+    --hash=sha256:6f7641992de44ec2ca54102422be44a8e3fb75b9690ccd74fff72b9ac7fc00ee \
+    --hash=sha256:6f8b62fdccc429e6643cefffd5df9c7bca65588d06e8925b78014ad9ad983bf5 \
+    --hash=sha256:718ea99f84b16c4bdbf6a93e53552cdccefa18e12ff9a02c5041e621460e2e61 \
+    --hash=sha256:747265f39978bbaad356f5c6b6c808f0e8f5e8994875af0119b82b4700c55387 \
+    --hash=sha256:77ea62879932b32aba77ab23a9296390a67d024bf2f048dee99143be80a4ce26 \
+    --hash=sha256:78a0d2a11bb3936463609777c6d6d4984a27ebb2360b58339c699899d85db036 \
+    --hash=sha256:799f5f221d639d1c2ed8a2348d1edf5e22aa489b58b2cc99f5bf0c1917e2d0f2 \
+    --hash=sha256:81fd28389bedab28251f0535b3c034b0e63a618efc3ff1d338c81a3da723adb3 \
+    --hash=sha256:827ddf2d5d157ac3d1001b52e84c9e20366237a742946599ffc435af7fdd26d0 \
+    --hash=sha256:8b76abfec195bf1ee6f9ec56c33ba5e9615ff2d0a9530a54001ed87e5a6ced3b \
+    --hash=sha256:8c40da44ca20235cda05751d6e828b6b348e7a7c5de2922fa0f9c63f564fd675 \
+    --hash=sha256:8e02425bfc7ebed617323a674974b70eaecd8f07b64a7d16e0bf3e766b93e3c9 \
+    --hash=sha256:8e08b01dc9369941a24d7e512b0d81bf514e7d6add1b93d8aeec3c8fa08a824e \
+    --hash=sha256:90167a48de3ed7f062058826608a80242b8561d0fb0cce2c610d741624811a61 \
+    --hash=sha256:9441aca94b21f7349cdb231cd0ce9ca251b2355836e8a02bf6ccbea5b442d7a9 \
+    --hash=sha256:97c13f156f14f10667e1cfc4257069b775440ce005e896c09ce3aff21c9ae665 \
+    --hash=sha256:987cd277d27d14301019fdf61c17524f6127f5d364be5482228726049d8e0d10 \
+    --hash=sha256:9a16ef3702cecf16056c5fd66398b7ea8622ff4e3afeb00a8db3e74427e850af \
+    --hash=sha256:9ea3d2e41d8fac71cb63ee72f75bee0ed1e9c50709d4c58587f15437761c1858 \
+    --hash=sha256:a02def2eb526cc934d2125533cf2f15aa71c72ed4397afca38427ab047901e88 \
+    --hash=sha256:a0643a25937fafe8d117f2907606e9940cd1cc905c66f16ece9ab93128299994 \
+    --hash=sha256:a2ee3909f611cc5860cc8d9f92d039fd84241ce7360b49ea88e657181d2b45f6 \
+    --hash=sha256:a357aae6791118011ad3ab4f2a4aa7bd7a487e5f9981b390e9f3c2c5137ecadf \
+    --hash=sha256:aa223c73c59cc45c12eaa9c439318084003beced0447ff92b578a890288e19eb \
+    --hash=sha256:ad4dbd06c1f579eb043b2dcfc635bc6c9fb858240a70f0abd3bed84d8ac79994 \
+    --hash=sha256:b0ba20be465566264fa5580d874ccf5eabba6975dba45857e2c76e2df3359c6d \
+    --hash=sha256:b27cea618601ca5032ea98ee116ca6e0fe67be7b286bcb0b9f956d64db697472 \
+    --hash=sha256:b7b9cbc60e3eb08da6d18636c62c6eb6206cd9d0c7ad73996f7a1df3fc415b27 \
+    --hash=sha256:bb571dbd4cc93342be0ba632f0b8d7de4cbd9d959d76371d33716d2216090d41 \
+    --hash=sha256:bbc15985c5658691f637a6b97651771147744edfad2a4be56b8a06755e3932fa \
+    --hash=sha256:bc5a1ec3bd05b55d3070d557c0cdd4412272d51b4966c79aa3e9da207bd33d65 \
+    --hash=sha256:bca5acf77508d1822023a85118c2dd8d3c16abdd56d2762359a46deb14daa5e0 \
+    --hash=sha256:c04ef83c9ca3162d200df36e933b3ea0327a2626cee2e01bbe55acbc004ce261 \
+    --hash=sha256:c21d5c7cfa6078c79897e5e482a7e84ff927143d2f3fb020dd6edd27f5469574 \
+    --hash=sha256:c22b32a57ab47afb207e8fe4bd7bb58c90f9291a63723cafd4e704742166e368 \
+    --hash=sha256:c458085e067c766112f089f78ce39eab2b69ba027d7bbb11d067a0b085774367 \
+    --hash=sha256:c4dbb1ebc9a811f38da33f32ed2bb5f58b149289b89eb11e384519e9ba7ca881 \
+    --hash=sha256:c754ce1fab41b731259f100d5d46529a38aa2c9b683c92aeb7e96ef5b2898cd8 \
+    --hash=sha256:c763d99cf087e7b2c5be0cf34ae9a0e1b031f5057d2341a0a0ed782458645b7e \
+    --hash=sha256:c9597a05d08e8103ad59ebdf29e3fbffb0d0dbf3b641f102cfbeadc3a77bde51 \
+    --hash=sha256:cc4af7090a626c902c48db9b5d786c1faa0d8e141571e8a63a5350419ea575bd \
+    --hash=sha256:ceb10039e7346927cec47eaa490b34abb602b537e738ee9914bb41b8de029fbc \
+    --hash=sha256:d1a15fef1938b43468002f2d81012dbc9e7b50eb8533af202b0559c2dc7865d9 \
+    --hash=sha256:d4276c7ee061db0bac54846933b40339f60085523675f917f37de24a4b3ce0ee \
+    --hash=sha256:d48657a404fab82b2754faa813a10c5ad6aa594cb1829dca168a49438b61b4ec \
+    --hash=sha256:e3f882110f2f4894942e314451773c47e8b1b4920b5ea2b6dd2e2d4079dd3135 \
+    --hash=sha256:e4c647795c5b901091a68e210c76b769af70a33a8624ac496ac3e34d33366c0d \
+    --hash=sha256:e62bde7d5df3312acc528786ee801c472cae5078b1f1e42761c853ba7fe1072a \
+    --hash=sha256:e6ec696a268e8d730b42711537e500f7397afc06125c0e8fa9c8211386d315a5 \
+    --hash=sha256:f176867f438ff2a43e6a837930153ca78fddb3ca94e378603a1e7b860d7869bf \
+    --hash=sha256:f8af980695b866255447703bf634551e67e1a4e1c2d2d26501858d9233d886d7 \
+    --hash=sha256:f8e57f9c2367706a320b78e91f8bf9a3b03bf9069464eb7b54455fa340d03e4c \
+    --hash=sha256:f9d5d924970b07128c61c08eebee718686f4bd9838ef712a50468169520c953f
 requests-toolbelt==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7681a0a3d047012b5bdc0ee37d7f8f07ebe76ab08caeccfc3921ce23c88d5bc6 \
     --hash=sha256:cccfdd665f0a24fcf4726e690f65639d272bb0637b9b92dfd91a5568ccf6bd06
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
 secretstorage==3.3.3 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "linux" \
@@ -527,95 +500,81 @@
     --hash=sha256:f356e6628222568e3af06f2eba8df495efa13b3b63081dafd4f7d9a7b7bc9f99
 shellingham==1.5.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
     --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-tomlkit==0.12.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:75baf5012d06501f07bee5bf8e801b9f343e7aac5a92581f20f80ce632e6b5a4 \
-    --hash=sha256:b0a645a9156dc7cb5d3a1f0d4bab66db287fcb8e0430bdd4664a095ea16414ba
-trove-classifiers==2023.11.29 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:02307750cbbac2b3d13078662f8a5bf077732bf506e9c33c97204b7f68f3699e \
-    --hash=sha256:ff8f7fd82c7932113b46e7ef6742c70091cc63640c8c65db00d91f2e940b9514
-urllib3==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
-    --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
-virtualenv==20.25.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3 \
-    --hash=sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b
-xattr==0.10.1 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" \
-    --hash=sha256:042ad818cda6013162c0bfd3816f6b74b7700e73c908cde6768da824686885f8 \
-    --hash=sha256:0aedf55b116beb6427e6f7958ccd80a8cbc80e82f87a4cd975ccb61a8d27b2ee \
-    --hash=sha256:0e14bd5965d3db173d6983abdc1241c22219385c22df8b0eb8f1846c15ce1fee \
-    --hash=sha256:13279fe8f7982e3cdb0e088d5cb340ce9cbe5ef92504b1fd80a0d3591d662f68 \
-    --hash=sha256:148466e5bb168aba98f80850cf976e931469a3c6eb11e9880d9f6f8b1e66bd06 \
-    --hash=sha256:16a660a883e703b311d1bbbcafc74fa877585ec081cd96e8dd9302c028408ab1 \
-    --hash=sha256:183ad611a2d70b5a3f5f7aadef0fcef604ea33dcf508228765fd4ddac2c7321d \
-    --hash=sha256:199b20301b6acc9022661412346714ce764d322068ef387c4de38062474db76c \
-    --hash=sha256:1dc9b9f580ef4b8ac5e2c04c16b4d5086a611889ac14ecb2e7e87170623a0b75 \
-    --hash=sha256:1e2973e72faa87ca29d61c23b58c3c89fe102d1b68e091848b0e21a104123503 \
-    --hash=sha256:1f0563196ee54756fe2047627d316977dc77d11acd7a07970336e1a711e934db \
-    --hash=sha256:209fb84c09b41c2e4cf16dd2f481bb4a6e2e81f659a47a60091b9bcb2e388840 \
-    --hash=sha256:2677d40b95636f3482bdaf64ed9138fb4d8376fb7933f434614744780e46e42d \
-    --hash=sha256:295b3ab335fcd06ca0a9114439b34120968732e3f5e9d16f456d5ec4fa47a0a2 \
-    --hash=sha256:3725746a6502f40f72ef27e0c7bfc31052a239503ff3eefa807d6b02a249be22 \
-    --hash=sha256:3e5825b5fc99ecdd493b0cc09ec35391e7a451394fdf623a88b24726011c950d \
-    --hash=sha256:3e739d624491267ec5bb740f4eada93491de429d38d2fcdfb97b25efe1288eca \
-    --hash=sha256:3ff0dbe4a6ce2ce065c6de08f415bcb270ecfd7bf1655a633ddeac695ce8b250 \
-    --hash=sha256:40039f1532c4456fd0f4c54e9d4e01eb8201248c321c6c6856262d87e9a99593 \
-    --hash=sha256:436e1aaf23c07e15bed63115f1712d2097e207214fc6bcde147c1efede37e2c5 \
-    --hash=sha256:46c32cd605673606b9388a313b0050ee7877a0640d7561eea243ace4fa2cc5a6 \
-    --hash=sha256:475c38da0d3614cc5564467c4efece1e38bd0705a4dbecf8deeb0564a86fb010 \
-    --hash=sha256:485539262c2b1f5acd6b6ea56e0da2bc281a51f74335c351ea609c23d82c9a79 \
-    --hash=sha256:49626096ddd72dcc1654aadd84b103577d8424f26524a48d199847b5d55612d0 \
-    --hash=sha256:4abef557028c551d59cf2fb3bf63f2a0c89f00d77e54c1c15282ecdd56943496 \
-    --hash=sha256:5267e5f9435c840d2674194150b511bef929fa7d3bc942a4a75b9eddef18d8d8 \
-    --hash=sha256:5b49d591cf34cda2079fd7a5cb2a7a1519f54dc2e62abe3e0720036f6ed41a85 \
-    --hash=sha256:5bc40570155beb85e963ae45300a530223d9822edfdf09991b880e69625ba38a \
-    --hash=sha256:5dc6099e76e33fa3082a905fe59df766b196534c705cf7a2e3ad9bed2b8a180e \
-    --hash=sha256:636ebdde0277bce4d12d2ef2550885804834418fee0eb456b69be928e604ecc4 \
-    --hash=sha256:6b8705ac6791426559c1a5c2b88bb2f0e83dc5616a09b4500899bfff6a929302 \
-    --hash=sha256:6b905e808df61b677eb972f915f8a751960284358b520d0601c8cbc476ba2df6 \
-    --hash=sha256:7298455ccf3a922d403339781b10299b858bb5ec76435445f2da46fb768e31a5 \
-    --hash=sha256:772b22c4ff791fe5816a7c2a1c9fcba83f9ab9bea138eb44d4d70f34676232b4 \
-    --hash=sha256:7880c8a54c18bc091a4ce0adc5c6d81da1c748aec2fe7ac586d204d6ec7eca5b \
-    --hash=sha256:789bd406d1aad6735e97b20c6d6a1701e1c0661136be9be862e6a04564da771f \
-    --hash=sha256:7f9be588a4b6043b03777d50654c6079af3da60cc37527dbb80d36ec98842b1e \
-    --hash=sha256:80638d1ce7189dc52f26c234cee3522f060fadab6a8bc3562fe0ddcbe11ba5a4 \
-    --hash=sha256:8068df3ebdfa9411e58d5ae4a05d807ec5994645bb01af66ec9f6da718b65c5b \
-    --hash=sha256:827b5a97673b9997067fde383a7f7dc67342403093b94ea3c24ae0f4f1fec649 \
-    --hash=sha256:89c93b42c3ba8aedbc29da759f152731196c2492a2154371c0aae3ef8ba8301b \
-    --hash=sha256:8faaacf311e2b5cc67c030c999167a78a9906073e6abf08eaa8cf05b0416515c \
-    --hash=sha256:925284a4a28e369459b2b7481ea22840eed3e0573a4a4c06b6b0614ecd27d0a7 \
-    --hash=sha256:986c2305c6c1a08f78611eb38ef9f1f47682774ce954efb5a4f3715e8da00d5f \
-    --hash=sha256:9d4c306828a45b41b76ca17adc26ac3dc00a80e01a5ba85d71df2a3e948828f2 \
-    --hash=sha256:a126eb38e14a2f273d584a692fe36cff760395bf7fc061ef059224efdb4eb62c \
-    --hash=sha256:a3878e1aff8eca64badad8f6d896cb98c52984b1e9cd9668a3ab70294d1ef92d \
-    --hash=sha256:a5ea974930e876bc5c146f54ac0f85bb39b7b5de2b6fc63f90364712ae368ebe \
-    --hash=sha256:a606280b0c9071ef52572434ecd3648407b20df3d27af02c6592e84486b05894 \
-    --hash=sha256:a9a7a807ab538210ff8532220d8fc5e2d51c212681f63dbd4e7ede32543b070f \
-    --hash=sha256:aa32f1b45fed9122bed911de0fcc654da349e1f04fa4a9c8ef9b53e1cc98b91e \
-    --hash=sha256:b0e919c24f5b74428afa91507b15e7d2ef63aba98e704ad13d33bed1288dca81 \
-    --hash=sha256:b27dfc13b193cb290d5d9e62f806bb9a99b00cd73bb6370d556116ad7bb5dc12 \
-    --hash=sha256:b34df5aad035d0343bd740a95ca30db99b776e2630dca9cc1ba8e682c9cc25ea \
-    --hash=sha256:b7bc4ae264aa679aacf964abf3ea88e147eb4a22aea6af8c6d03ebdebd64cfd6 \
-    --hash=sha256:c0cd2d02ef2fb45ecf2b0da066a58472d54682c6d4f0452dfe7ae2f3a76a42ea \
-    --hash=sha256:c12e7d81ffaa0605b3ac8c22c2994a8e18a9cf1c59287a1b7722a2289c952ec5 \
-    --hash=sha256:c3024a9ff157247c8190dd0eb54db4a64277f21361b2f756319d9d3cf20e475f \
-    --hash=sha256:c4120090dac33eddffc27e487f9c8f16b29ff3f3f8bcb2251b2c6c3f974ca1e1 \
-    --hash=sha256:c5d3d0e728bace64b74c475eb4da6148cd172b2d23021a1dcd055d92f17619ac \
-    --hash=sha256:cc6b8d5ca452674e1a96e246a3d2db5f477aecbc7c945c73f890f56323e75203 \
-    --hash=sha256:ceaa26bef8fcb17eb59d92a7481c2d15d20211e217772fb43c08c859b01afc6a \
-    --hash=sha256:d1ef954d0655f93a34d07d0cc7e02765ec779ff0b59dc898ee08c6326ad614d5 \
-    --hash=sha256:d60c27922ec80310b45574351f71e0dd3a139c5295e8f8b19d19c0010196544f \
-    --hash=sha256:e31d062cfe1aaeab6ba3db6bd255f012d105271018e647645941d6609376af18 \
-    --hash=sha256:e8c014c371391f28f8cd27d73ea59f42b30772cd640b5a2538ad4f440fd9190b \
-    --hash=sha256:ec0956a8ab0f0d3f9011ba480f1e1271b703d11542375ef73eb8695a6bd4b78b \
-    --hash=sha256:f1be6e733e9698f645dbb98565bb8df9b75e80e15a21eb52787d7d96800e823b \
-    --hash=sha256:f24a7c04ff666d0fe905dfee0a84bc899d624aeb6dccd1ea86b5c347f15c20c1 \
-    --hash=sha256:f55a2dd73a12a1ae5113c5d9cd4b4ab6bf7950f4d76d0a1a0c0c4264d50da61d \
-    --hash=sha256:fc354f086f926a1c7f04886f97880fed1a26d20e3bc338d0d965fd161dbdb8ab \
-    --hash=sha256:ffcb57ca1be338d69edad93cf59aac7c6bb4dbb92fd7bf8d456c69ea42f7e6d2
-zipp==3.17.0 ; python_version >= "3.9" and python_version < "3.12" \
-    --hash=sha256:0e923e726174922dce09c53c59ad483ff7bbb8e572e00c7f7c46b88556409f31 \
-    --hash=sha256:84e64a1c28cf7e91ed2078bb8cc8c259cb19b76942096c8d7b84947690cabaf0
+tomlkit==0.12.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+trove-classifiers==2024.4.10 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:49f40bb6a746b72a1cba4f8d55ee8252169cda0f70802e3fd24f04b7fb25a492 \
+    --hash=sha256:678bd6fcc5218d72e3304e27a608acc9b91e17bd00c3f3d8c968497c843ad98b
+urllib3==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
+virtualenv==20.25.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
+    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
+xattr==1.1.0 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "darwin" \
+    --hash=sha256:00d2b415cf9d6a24112d019e721aa2a85652f7bbc9f3b9574b2d1cd8668eb491 \
+    --hash=sha256:0683dae7609f7280b0c89774d00b5957e6ffcb181c6019c46632b389706b77e6 \
+    --hash=sha256:08f61cbed52dc6f7c181455826a9ff1e375ad86f67dd9d5eb7663574abb32451 \
+    --hash=sha256:0a9c431b0e66516a078125e9a273251d4b8e5ba84fe644b619f2725050d688a0 \
+    --hash=sha256:0f06e0c1e4d06b4e0e49aaa1184b6f0e81c3758c2e8365597918054890763b53 \
+    --hash=sha256:1a5921ea3313cc1c57f2f53b63ea8ca9a91e48f4cc7ebec057d2447ec82c7efe \
+    --hash=sha256:23705c7079b05761ff2fa778ad17396e7599c8759401abc05b312dfb3bc99f69 \
+    --hash=sha256:24d97f0d28f63695e3344ffdabca9fcc30c33e5c8ccc198c7524361a98d526f2 \
+    --hash=sha256:27272afeba8422f2a9d27e1080a9a7b807394e88cce73db9ed8d2dde3afcfb87 \
+    --hash=sha256:46a641ac038a9f53d2f696716147ca4dbd6a01998dc9cd4bc628801bc0df7f4d \
+    --hash=sha256:47a3bdfe034b4fdb70e5941d97037405e3904accc28e10dbef6d1c9061fb6fd7 \
+    --hash=sha256:4cb70c16e7c3ae6ba0ab6c6835c8448c61d8caf43ea63b813af1f4dbe83dd156 \
+    --hash=sha256:54cb15cd94e5ef8a0ef02309f1bf973ba0e13c11e87686e983f371948cfee6af \
+    --hash=sha256:6461a43b585e5f2e049b39bcbfcb6391bfef3c5118231f1b15d10bdb89ef17fe \
+    --hash=sha256:6480589c1dac7785d1f851347a32c4a97305937bf7b488b857fe8b28a25de9e9 \
+    --hash=sha256:687e7d18611ef8d84a6ecd8f4d1ab6757500c1302f4c2046ce0aa3585e13da3f \
+    --hash=sha256:6881b120f9a4b36ccd8a28d933bc0f6e1de67218b6ce6e66874e0280fc006844 \
+    --hash=sha256:6ad47d89968c9097900607457a0c89160b4771601d813e769f68263755516065 \
+    --hash=sha256:78b377832dd0ee408f9f121a354082c6346960f7b6b1480483ed0618b1912120 \
+    --hash=sha256:793c01deaadac50926c0e1481702133260c7cb5e62116762f6fe1543d07b826f \
+    --hash=sha256:7a92aff66c43fa3e44cbeab7cbeee66266c91178a0f595e044bf3ce51485743b \
+    --hash=sha256:7e4ca0956fd11679bb2e0c0d6b9cdc0f25470cc00d8da173bb7656cc9a9cf104 \
+    --hash=sha256:83652910ef6a368b77b00825ad67815e5c92bfab551a848ca66e9981d14a7519 \
+    --hash=sha256:9013f290387f1ac90bccbb1926555ca9aef75651271098d99217284d9e010f7c \
+    --hash=sha256:918e1f83f2e8a072da2671eac710871ee5af337e9bf8554b5ce7f20cdb113186 \
+    --hash=sha256:96ca300c0acca4f0cddd2332bb860ef58e1465d376364f0e72a1823fdd58e90d \
+    --hash=sha256:9b1664edf003153ac8d1911e83a0fc60db1b1b374ee8ac943f215f93754a1102 \
+    --hash=sha256:9c5a78c7558989492c4cb7242e490ffb03482437bf782967dfff114e44242343 \
+    --hash=sha256:9d4f71b673339aeaae1f6ea9ef8ea6c9643c8cd0df5003b9a0eaa75403e2e06c \
+    --hash=sha256:9dcd5dfbcee73c7be057676ecb900cabb46c691aff4397bf48c579ffb30bb963 \
+    --hash=sha256:a20de1c47b5cd7b47da61799a3b34e11e5815d716299351f82a88627a43f9a96 \
+    --hash=sha256:afacebbc1fa519f41728f8746a92da891c7755e6745164bd0d5739face318e86 \
+    --hash=sha256:b0d73150f2f9655b4da01c2369eb33a294b7f9d56eccb089819eafdbeb99f896 \
+    --hash=sha256:b489b7916f239100956ea0b39c504f3c3a00258ba65677e4c8ba1bd0b5513446 \
+    --hash=sha256:b6ceb9efe0657a982ccb8b8a2efe96b690891779584c901d2f920784e5d20ae3 \
+    --hash=sha256:b735ac2625a4fc2c9343b19f806793db6494336338537d2911c8ee4c390dda46 \
+    --hash=sha256:caab2c2986c30f92301f12e9c50415d324412e8e6a739a52a603c3e6a54b3610 \
+    --hash=sha256:ccab735d0632fe71f7d72e72adf886f45c18b7787430467ce0070207882cfe25 \
+    --hash=sha256:cd11e917f5b89f2a0ad639d9875943806c6c9309a3dd02da5a3e8ef92db7bed9 \
+    --hash=sha256:cebcf8a303a44fbc439b68321408af7267507c0d8643229dbb107f6c132d389c \
+    --hash=sha256:d1059b2f726e2702c8bbf9bbf369acfc042202a4cc576c2dec6791234ad5e948 \
+    --hash=sha256:d1418705f253b6b6a7224b69773842cac83fcbcd12870354b6e11dd1cd54630f \
+    --hash=sha256:d44e8f955218638c9ab222eed21e9bd9ab430d296caf2176fb37abe69a714e5c \
+    --hash=sha256:d6eb7d5f281014cd44e2d847a9107491af1bf3087f5afeded75ed3e37ec87239 \
+    --hash=sha256:dab29d9288aa28e68a6f355ddfc3f0a7342b40c9012798829f3e7bd765e85c2c \
+    --hash=sha256:dba4f80b9855cc98513ddf22b7ad8551bc448c70d3147799ea4f6c0b758fb466 \
+    --hash=sha256:dc53cab265f6e8449bd683d5ee3bc5a191e6dd940736f3de1a188e6da66b0653 \
+    --hash=sha256:dd43978966de3baf4aea367c99ffa102b289d6c2ea5f3d9ce34a203dc2f2ab73 \
+    --hash=sha256:dda2684228798e937a7c29b0e1c7ef3d70e2b85390a69b42a1c61b2039ba81de \
+    --hash=sha256:ded771eaf27bb4eb3c64c0d09866460ee8801d81dc21097269cf495b3cac8657 \
+    --hash=sha256:e0c80bbf55339c93770fc294b4b6586b5bf8e85ec00a4c2d585c33dbd84b5006 \
+    --hash=sha256:e189e440bcd04ccaad0474720abee6ee64890823ec0db361fb0a4fb5e843a1bf \
+    --hash=sha256:e2255f36ebf2cb2dbf772a7437ad870836b7396e60517211834cf66ce678b595 \
+    --hash=sha256:ef2fa0f85458736178fd3dcfeb09c3cf423f0843313e25391db2cfd1acec8888 \
+    --hash=sha256:f6ad2a7bd5e6cf71d4a862413234a067cf158ca0ae94a40d4b87b98b62808498 \
+    --hash=sha256:fa6a7af7a4ada43f15ccc58b6f9adcdbff4c36ba040013d2681e589e07ae280a \
+    --hash=sha256:fecbf3b05043ed3487a28190dec3e4c4d879b2fcec0e30bafd8ec5d4b6043630 \
+    --hash=sha256:ff6223a854229055e803c2ad0c0ea9a6da50c6be30d92c198cf5f9f28819a921
+zipp==3.18.1 ; python_version >= "3.9" and python_version < "3.12" \
+    --hash=sha256:206f5a15f2af3dbaee80769fb7dc6f249695e940acca08dfb2a4769fe61e538b \
+    --hash=sha256:2884ed22e7d8961de1c9a05142eb69a247f120291bc0206a00a7642f09b5b715
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/library-flake8.in` & `alluka-0.1.5/piped/python/base-requirements/library-flake8.in`

 * *Files identical despite different names*

### Comparing `alluka-0.1.4/piped/python/base-requirements/library-flake8.txt` & `alluka-0.1.5/piped/python/base-requirements/library-flake8.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,82 +9,82 @@
     --hash=sha256:6d8c914f01fbea252cb8f31563f2e766a9ab03c02b9bcc37d18f7d9138828401
 astor==0.8.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:070a54e890cefb5b3739d19f30f5a5ec840ffc9c50ffa7d23cc9fc1a38ebbfc5 \
     --hash=sha256:6a6effda93f4e1ce9f618779b2dd1d9d84f1e32812c23a29b3fff6fd7f63fa5e
 asttokens==2.4.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:051ed49c3dcae8913ea7cd08e46a606dba30b79993209636c4875bc1d637bc24 \
     --hash=sha256:b03869718ba9a6eb027e134bfdf69f38a236d681c83c160d510768af11254ba0
-attrs==23.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
-bandit==1.7.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:36da17c67fc87579a5d20c323c8d0b1643a890a2b93f00b3d1229966624694ff \
-    --hash=sha256:72ce7bc9741374d96fb2f1c9a8960829885f1243ffde743de70a19cee353e8f3
-black==23.12.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0808494f2b2df923ffc5723ed3c7b096bd76341f6213989759287611e9837d50 \
-    --hash=sha256:1fa88a0f74e50e4487477bc0bb900c6781dbddfdfa32691e780bf854c3b4a47f \
-    --hash=sha256:25e57fd232a6d6ff3f4478a6fd0580838e47c93c83eaf1ccc92d4faf27112c4e \
-    --hash=sha256:2d9e13db441c509a3763a7a3d9a49ccc1b4e974a47be4e08ade2a228876500ec \
-    --hash=sha256:3e1b38b3135fd4c025c28c55ddfc236b05af657828a8a6abe5deec419a0b7055 \
-    --hash=sha256:3fa4be75ef2a6b96ea8d92b1587dd8cb3a35c7e3d51f0738ced0781c3aa3a5a3 \
-    --hash=sha256:4ce3ef14ebe8d9509188014d96af1c456a910d5b5cbf434a09fef7e024b3d0d5 \
-    --hash=sha256:4f0031eaa7b921db76decd73636ef3a12c942ed367d8c3841a0739412b260a54 \
-    --hash=sha256:602cfb1196dc692424c70b6507593a2b29aac0547c1be9a1d1365f0d964c353b \
-    --hash=sha256:6d1bd9c210f8b109b1762ec9fd36592fdd528485aadb3f5849b2740ef17e674e \
-    --hash=sha256:78baad24af0f033958cad29731e27363183e140962595def56423e626f4bee3e \
-    --hash=sha256:8d4df77958a622f9b5a4c96edb4b8c0034f8434032ab11077ec6c56ae9f384ba \
-    --hash=sha256:97e56155c6b737854e60a9ab1c598ff2533d57e7506d97af5481141671abf3ea \
-    --hash=sha256:9c4352800f14be5b4864016882cdba10755bd50805c95f728011bcb47a4afd59 \
-    --hash=sha256:a4d6a9668e45ad99d2f8ec70d5c8c04ef4f32f648ef39048d010b0689832ec6d \
-    --hash=sha256:a920b569dc6b3472513ba6ddea21f440d4b4c699494d2e972a1753cdc25df7b0 \
-    --hash=sha256:ae76c22bde5cbb6bfd211ec343ded2163bba7883c7bc77f6b756a1049436fbb9 \
-    --hash=sha256:b18fb2ae6c4bb63eebe5be6bd869ba2f14fd0259bda7d18a46b764d8fb86298a \
-    --hash=sha256:c04b6d9d20e9c13f43eee8ea87d44156b8505ca8a3c878773f68b4e4812a421e \
-    --hash=sha256:c88b3711d12905b74206227109272673edce0cb29f27e1385f33b0163c414bba \
-    --hash=sha256:dd15245c8b68fe2b6bd0f32c1556509d11bb33aec9b5d0866dd8e2ed3dba09c2 \
-    --hash=sha256:e0aaf6041986767a5e0ce663c7a2f0e9eaf21e6ff87a5f95cbf3675bfd4c41d2
+attrs==23.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:935dc3b529c262f6cf76e50877d35a4bd3c1de194fd41f47a2b7ae8f19971f30 \
+    --hash=sha256:99b87a485a5820b23b879f04c2305b44b951b502fd64be915879d77a7e8fc6f1
+bandit==1.7.8 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:36de50f720856ab24a24dbaa5fee2c66050ed97c1477e0a1159deab1775eab6b \
+    --hash=sha256:509f7af645bc0cd8fd4587abc1a038fc795636671ee8204d502b933aee44f381
+black==24.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d \
+    --hash=sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd \
+    --hash=sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33 \
+    --hash=sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965 \
+    --hash=sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070 \
+    --hash=sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397 \
+    --hash=sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745 \
+    --hash=sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1 \
+    --hash=sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665 \
+    --hash=sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436 \
+    --hash=sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb \
+    --hash=sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e \
+    --hash=sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6 \
+    --hash=sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702 \
+    --hash=sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8 \
+    --hash=sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8 \
+    --hash=sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3 \
+    --hash=sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad \
+    --hash=sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf \
+    --hash=sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e \
+    --hash=sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641 \
+    --hash=sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2
 classify-imports==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:7abfb7ea92149b29d046bd34573d247ba6e68cc28100c801eba4af17964fc40e \
     --hash=sha256:dbbc264b70a470ed8c6c95976a11dfb8b7f63df44ed1af87328bbed2663f5161
 click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-consolekit==1.6.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:1e7ece22b2fe4ae296d70e8be46ed37aa77950dfff2840e8b4792e45f0f96dd9 \
-    --hash=sha256:53d05dba2a38c28532f2b193a4e7b68054821e201d39d7ca818753d4add603c1
+consolekit==1.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:064e32c520d63443ac47da7b2d4010c5646c1c78c9b1649adb9dd5d27116cb05 \
+    --hash=sha256:0ea8bce2a7941a2af0e33d5acb76eeacb78711278d2b60c33ed3e7a49cc3fd0c
 deprecation-alias==0.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1c9e1a5ddd0a276a1a18e7a4f9d56b53232217491c4549eaa45e51753013ce76 \
     --hash=sha256:ed2e9dde582530e2a364cae4fa26077fda4adc9b28a44ce94a8ef0ee9271e312
 deprecation==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:72b3bde64e5d778694b0cf68178aed03d15e15477116add3fb773e581f9518ff \
     --hash=sha256:a10811591210e1fb0e768a8c25517cabeabcba6f0bf96564f8ff45189f90b14a
 domdf-python-tools==3.8.0.post2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a1fd255ea29f767b08de462d2da39d360262304389227d980bc307ee8aa3366a \
     --hash=sha256:ad2c763c8d00850a7fa92ad95e9891a1918281ea25322c4dbb1734fd32f905dd
 eradicate==2.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:06df115be3b87d0fc1c483db22a2ebb12bcf40585722810d809cc770f5031c37 \
     --hash=sha256:2b29b3dd27171f209e4ddd8204b70c02f0682ae95eecb353f10e8d72b149c63e
-flake8-async==22.11.14 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:317cf0f882a2f4a09c2250c451acff8358d7faec8a0aa54521b6e69336fe9d0b \
-    --hash=sha256:b4db2d55883653b47d4bfd946fdf506e8958bb4ca35974790b8c3e620fc1abff
+flake8-async==24.4.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:44ab537cda26b9e5898b9afd64836dc8356701aa558ddfe2a84e3e41de99c3dd \
+    --hash=sha256:9e44b22c48a5d43450fe46f84bf355fad5018a0d46c78cb0a6b7487cc384b75e
 flake8-bandit==4.1.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:068e09287189cbfd7f986e92605adea2067630b75380c6b5733dab7d87f9a84e \
     --hash=sha256:4c8a53eb48f23d4ef1e59293657181a3c989d0077c9952717e98a0eace43e06d
 flake8-black==0.3.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0dfbca3274777792a5bcb2af887a4cad72c72d0e86c94e08e3a3de151bb41c34 \
     --hash=sha256:fe8ea2eca98d8a504f22040d9117347f6b367458366952862ac3586e7d4eeaca
 flake8-broken-line==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:96c964336024a5030dc536a9f6fb02aa679e2d2a6b35b80a558b5136c35832a9 \
     --hash=sha256:e2c6a17f8d9a129e99c1320fce89b33843e2963871025c4c2bb7b8b8d8732a85
-flake8-builtins==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:392d5af3a0720c5a863aa93dc47f48c879081345a143fe9f20d995fe9ff5686a \
-    --hash=sha256:7ee5766d9c60e5d579dfda84e65c6d0e6c26005f6f59cb9bf722462d7987a807
+flake8-builtins==2.5.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:8cac7c52c6f0708c0902b46b385bc7e368a9068965083796f1431c0d2e6550cf \
+    --hash=sha256:bdaa3dd823e4f5308c5e712d19fa5f69daa52781ea874f5ea9c3637bcf56faa6
 flake8-coding==1.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:79704112c44d09d4ab6c8965e76a20c3f7073d52146db60303bce777d9612260 \
     --hash=sha256:b8f4d5157a8f74670e6cfea732c3d9f4291a4e994c8701d2c55f787c6e6cb741
 flake8-comments==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:42250cb4a51dc59e6db25f1291cfb16b78ea233f72dac32a5bc7b09c691235ea \
     --hash=sha256:780b4fc2820ed4ff8a0a98f3fc993f776ede1aecbe0c6cec64d93814b21c9234
 flake8-comprehensions==3.14.0 ; python_version >= "3.9" and python_version < "4.0" \
@@ -92,17 +92,17 @@
     --hash=sha256:81768c61bfc064e1a06222df08a2580d97de10cb388694becaf987c331c6c0cf
 flake8-deprecated==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:3819ed2badb68631593312edb9c4881d974b995d96a4427566ddb1593a4c8fea \
     --hash=sha256:ee96ca001d1ca0561fa8e46f23e2d2460b18a86696373cab644e102ae0ff2aa2
 flake8-docstrings==1.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4c8cc748dc16e6869728699e5d0d685da9a10b0ea718e090b1ba088e67a941af \
     --hash=sha256:51f2344026da083fc084166a9353f5082b01f72901df422f74b4d953ae88ac75
-flake8-dunder-all==0.3.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cf3c39198e6846e666ffd2afe97b94babbb2e2d44f3dcba131fa340c63d67280 \
-    --hash=sha256:e852845a12a9b2cb0757f9a744c9552ec74e6d5b09ee157b663614cc5ed43a68
+flake8-dunder-all==0.4.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:566b57946cea29419cc8fe30538f0a797aee830f651bc4fa22d6c61e3477a5ca \
+    --hash=sha256:bfea5ad2587cbd45f6ada8bbc67495d339f13a899bb27279aac35448324db19b
 flake8-eradicate==1.5.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:18acc922ad7de623f5247c7d5595da068525ec5437dd53b22ec2259b96ce9d22 \
     --hash=sha256:aee636cb9ecb5594a7cd92d67ad73eb69909e5cc7bd81710cf9d00970f3983a6
 flake8-executable==2.1.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:619fe023e00c3d8e5113521d7200e1ebb04587c12d157f9a2fb167feb8cae66b \
     --hash=sha256:f0a66c97c3b99ce63bc1f01ce602d6bd048e4fc5dc0d7a13be2bfa3deb023a34
 flake8-fixme==1.1.1 ; python_version >= "3.9" and python_version < "4.0" \
@@ -146,170 +146,189 @@
     --hash=sha256:e4848c57d9d50f19100c2d75fa794b72df068666a9041b4b0409be923356a3ed
 flake8-print==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:76915a2a389cc1c0879636c219eb909c38501d3a43cc8dae542081c9ba48bdf9 \
     --hash=sha256:84a1a6ea10d7056b804221ac5e62b1cee1aefc897ce16f2e5c42d3046068f5d8
 flake8-printf-formatting==1.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0f9e1308ac290356e4b271d4f26adfc3f9165680a7b6c221503b0f3e155a2784 \
     --hash=sha256:d908ffabdf08581043a50572744fd60563d82386630b0335445894120089d2df
-flake8-pytest-style==1.7.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b924197c99b951315949920b0e5547f34900b1844348432e67a44ab191582109 \
-    --hash=sha256:f5d2aa3219163a052dd92226589d45fab8ea027a3269922f0c4029f548ea5cd1
+flake8-pyproject==1.2.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6249fe53545205af5e76837644dc80b4c10037e73a0e5db87ff562d75fb5bd4a
+flake8-pytest-style==2.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:919c328cacd4bc4f873ea61ab4db0d8f2c32e0db09a3c73ab46b1de497556464 \
+    --hash=sha256:abcb9f56f277954014b749e5a0937fae215be01a21852e9d05e7600c3de6aae5
 flake8-pytest==1.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:19f543b2d1cc89d61b76f19d0a9e58e9a110a035175f701b3425c363a7732c56 \
     --hash=sha256:97328f258ffad9fe18babb3b0714a16b121505ad3ac87d4e33020874555d0784
 flake8-raise==0.0.5 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0a9890e16b851402d9b0d4fafe6c34890eab73835a2c2079c3850a25be575623 \
     --hash=sha256:df26e5c542a58c8f8786d978e18ad7e54126a0ef5c6241c35dafaca7e2bbb808
 flake8-simplify==0.21.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:439391e762a9370b371208add0b5c5c40c3d25a98e1f5421d263215d08194183 \
     --hash=sha256:c95ff1dcc1de5949af47e0087cbf1164445881131b15bcd7a71252670f492f4d
-flake8-type-checking==2.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:07d949b686f39eb0cb828a394aa29d48bd1ca0df92d552d9794d17b22c309cd7 \
-    --hash=sha256:a6f9ded325f0c9845f073609c557bf481882adc4d18571a39b137ef2d284dc85
+flake8-type-checking==2.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6fcc0e8a63f6a87b5b26b776388c21907e66c4efbd15dcc1bcbd96fe884da93d \
+    --hash=sha256:b63e1745f6e7deee1403d7e0150a5bca378315e9fe4d4cdaa7b71338034dbcc3
 flake8-typing-imports==1.15.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4594830f9ecfbe9c75f73de32db3db45d427e837df42bfc478bee6584a2400ec \
     --hash=sha256:6c04b1e9986874d81399f115f5ec683325675268e9b4924e8464f8b1b6b211d1
 flake8-use-fstring==1.4 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6550bf722585eb97dffa8343b0f1c372101f5c4ab5b07ebf0edd1c79880cdd39
 flake8-use-pathlib==0.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0ef19f255a51601bcf04ff54f25ef8a466dff68210cd95b4f1db36a78ace5223 \
     --hash=sha256:c7b6d71575b575f7d70ebf3f1d7f2dd6685e401d3280208f1db9dbb6bfa32608
 flake8-variables-names==0.0.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:292c50e4813d632aa3adcd02c185e7bb583f5fc8ebe02e70f13c958bfe46ad91 \
     --hash=sha256:4aff935d54b3f7afcd026b4dae55029877bd05a7c507b294b45bc7bf577d7b47
-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:d5b3857f07c030bdb5bf41c7f53799571d75c4491748a3adcd47de929e34cd23 \
-    --hash=sha256:ffdfce58ea94c6580c77888a86506937f9a1a227dfcd15f245d694ae20a6b6e5
-gitdb==4.0.11 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:81a3407ddd2ee8df444cbacea00e2d038e40150acfa3001696fe0dcf1d3adfa4 \
-    --hash=sha256:bf5421126136d6d0af55bc1e7c1af1c397a34f5b7bd79e776cd3e89785c2b04b
-gitpython==3.1.40 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:22b126e9ffb671fdd0c129796343a02bf67bf2994b35449ffc9321aa755e18a4 \
-    --hash=sha256:cf14627d5a8049ffbf49915732e5eddbe8134c3bdb9d476e6182b676fc573f8a
+flake8==7.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:33f96621059e65eec474169085dc92bf26e7b2d47366b70be2f67ab80dc25132 \
+    --hash=sha256:a6dfbb75e03252917f2473ea9653f7cd799c3064e54d4c8140044c5c065f53c3
 isort==5.13.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
     --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
-jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
+jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+libcst==1.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:03b1df1ae02456f1d465fcd5ead1d0d454bb483caefd8c8e6bde515ffdb53d1b \
+    --hash=sha256:0a0d250fb6a2c1d158f30d25ba5e33e3ed3672d2700d480dd47beffd1431a008 \
+    --hash=sha256:16880711be03a1f5da7028fe791ba5b482a50d830225a70272dc332dfd927652 \
+    --hash=sha256:181372386c986e3de07d7a93f269214cd825adc714f1f9da8252b44f05e181c4 \
+    --hash=sha256:189bb28c19c5dd3c64583f969b72f7732dbdb1dee9eca3acc85099e4cef9148b \
+    --hash=sha256:2dbac1ac0a9d59ea7bbc3f87cdcca5bfe98835e31c668e95cb6f3d907ffc53fc \
+    --hash=sha256:4186076ce12141609ce950d61867b2a73ea199a7a9870dbafa76ad600e075b3c \
+    --hash=sha256:431badf0e544b79c0ac9682dbd291ff63ddbc3c3aca0d13d3cc7a10c3a9db8a2 \
+    --hash=sha256:4ad5741b251d901f3da1819ac539192230cc6f8f81aaf04eb4ec0009c1c97285 \
+    --hash=sha256:4ed52a1a2fe4d8603de51649db5e438317b8116ebb9fc09ec68703535fe6c1c8 \
+    --hash=sha256:701f5335e4fd566871497b9af1e871c98e1ef10c30b3b244f39343d709213401 \
+    --hash=sha256:7c6e709623b68ca9148e8ecbdc145f7b83befb26032e4bf6a8122500ba558b17 \
+    --hash=sha256:7cdb7e8a118b60e064a02f6cbfa4d328212a3a115d125244495190f405709d5f \
+    --hash=sha256:8c2020f7449270e3ff0bdc481ae244d812f2d9a8b7dbff0ea66b830f4b350f54 \
+    --hash=sha256:904c4cc5c801a5747e64b43e0accc87c67a4c804842d977ee215872c4cf8cf88 \
+    --hash=sha256:9e6bc95fa7dde79cde63a34a0412cd4a3d9fcc27be781a590f8c45c840c83658 \
+    --hash=sha256:a2d64d86dcd6c80a5dac2e243c5ed7a7a193242209ac33bad4b0639b24f6d131 \
+    --hash=sha256:b740dc0c3d1adbd91442fb878343d5a11e23a0e3ac5484be301fd8d148bcb085 \
+    --hash=sha256:be3bf9aaafebda6a21e241e819f0ab67e186e898c3562704e41241cf8738353a \
+    --hash=sha256:c0886a9963597367b227345f19b24931b3ed6a4703fff237760745f90f0e6a20 \
+    --hash=sha256:c12b7b01d8745f82dd86a82acd2a9f8e8e7d6c94ddcfda996896e83d1a8d5c42 \
+    --hash=sha256:db084f7bbf825c7bd5ed256290066d0336df6a7dc3a029c9870a64cd2298b87f \
+    --hash=sha256:de93193cba6d54f2a4419e94ba2de642b111f52e4fa01bb6e2c655914585f65b \
+    --hash=sha256:ede0f026a82b03b33a559ec566860085ece2e76d8f9bc21cb053eedf9cde8c79 \
+    --hash=sha256:f2995ca687118a9d3d41876f7270bc29305a2d402f4b8c81a3cff0aeee6d4c81
 markdown-it-py==3.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
     --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
-markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
+markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
 mccabe==0.7.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:348e0240c33b60bbdf4e523192ef919f28cb2c3d7d5c7794f74009290f236325 \
     --hash=sha256:6c2d30ab6be0e4a46919781807b4f0d834ebdd6c6e3dca0bda5a15f863427b6e
 mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
     --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
-mistletoe==1.2.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:620563ac06380ce0629b4a2afa2f2ab797ffac3efdcccaf2362a7266600e6dcc \
-    --hash=sha256:7d0c1ab3747047d169f9fc4b925d1cba3f5c13eaf0b90c365b72e47e59d00a02
-more-itertools==10.1.0 ; python_version == "3.9" \
-    --hash=sha256:626c369fa0eb37bac0291bce8259b332fd59ac792fa5497b59837309cd5b114a \
-    --hash=sha256:64e0735fcfdc6f3464ea133afe8ea4483b1c5fe3a3d69852e6503b43a0b222e6
+mistletoe==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a0710d0cdb7d2458cef91cf6b9b897db442927f8778dae890cbbfb1853a51700 \
+    --hash=sha256:bd0e788add9b4478d19ec792f6d5fb908a20e70abfe61193f29178c55d3adbe9
+more-itertools==10.2.0 ; python_version == "3.9" \
+    --hash=sha256:686b06abe565edfab151cb8fd385a05651e1fdf8f0a14191e4439283421f8684 \
+    --hash=sha256:8fccb480c43d3e99a00087634c06dd02b0d50fbf088b380de5a41a015ec239e1
 mr-proper==0.0.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:03b517b19e617537f711ce418b125e5f2efd82ec881539cdee83195c78c14a02 \
     --hash=sha256:74a1b60240c46f10ba518707ef72811a01e5c270da0a78b5dd2dd923d99fdb14
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
 natsort==8.4.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:45312c4a0e5507593da193dedd04abb1469253b601ecaf63445ad80f0a1ea581 \
     --hash=sha256:4732914fb471f56b5cce04d7bae6f164a592c7712e1c85f9ef585e197299521c
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
 pbr==6.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4a7317d5e3b17a3dccb6a8cfe67dab65b20551404c52c8ed41279fa4f0cb4cda \
     --hash=sha256:d1377122a5a00e2f940ee482999518efe16d745d423a670c27773dfbc3c9a7d9
 pep8-naming==0.13.3 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1705f046dfcd851378aac3be1cd1551c7c1e5ff363bacad707d43007877fa971 \
     --hash=sha256:1a86b8c71a03337c97181917e2b472f0f5e4ccb06844a0d6f0a33522549e7a80
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
 pycodestyle==2.11.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:41ba0e7afc9752dfb53ced5489e89f8186be00e599e712660695b7a75ff2663f \
     --hash=sha256:44fe31000b2d866f2e41841b18528a505fbd7fef9017b04eff4e2648a0fadc67
 pydocstyle==6.3.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:118762d452a49d6b05e194ef344a55822987a462831ade91ec5c06fd2169d019 \
     --hash=sha256:7ce43f0c0ac87b07494eb9c0b462c0b73e6ff276807f204d6b53edc72b7e44e1
-pyflakes==3.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4132f6d49cb4dae6819e5379898f2b8cce3c5f23994194c24b77d5da2e36f774 \
-    --hash=sha256:a0aae034c444db0071aa077972ba4768d40c830d9539fd45bf4cd3f8f6992efc
+pyflakes==3.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1c61603ff154621fb2a9172037d84dca3500def8c8b630657d1701f026f8af3f \
+    --hash=sha256:84b5be138a2dfbb40689ca07e2152deb896a65c3a3e24c251c5c62489568074a
 pygments==2.17.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
     --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
-pyproject-flake8==6.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:6da8e5a264395e0148bc11844c6fb50546f1fac83ac9210f7328664135f9e70f \
-    --hash=sha256:86ea5559263c098e1aa4f866776aa2cf45362fd91a576b9fd8fbbbb55db12c4e
 pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
     --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
     --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
     --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
@@ -332,14 +351,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -353,40 +373,37 @@
     --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
-rich==13.7.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:5cb5123b5cf9ee70584244246816e9114227e0b98ad9176eede6ad54bf5403fa \
-    --hash=sha256:6da14c108c4866ee9520bbffa71f6fe3962e193b7da68720583850cd4548e235
-setuptools==69.0.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
+rich==13.7.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
+setuptools==69.5.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
 six==1.16.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926 \
     --hash=sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254
-smmap==5.0.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:dceeb6c0028fdb6734471eb07c0cd2aae706ccaecab45965ee83f11c8d3b1f62 \
-    --hash=sha256:e6d8668fa5f93e706934a62d7b4db19c8d9eb8cf2adbb75ef1b675aa332b69da
 snowballstemmer==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1 \
     --hash=sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a
 stdlib-list==0.10.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:6519c50d645513ed287657bfe856d527f277331540691ddeaf77b25459964a14 \
     --hash=sha256:b3a911bc441d03e0332dd1a9e7d0870ba3bb0a542a74d7524f54fb431256e214
-stevedore==5.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8cc040628f3cea5d7128f2e76cf486b2251a4e543c7b938f58d9a377f6694a2d \
-    --hash=sha256:a54534acf9b89bc7ed264807013b505bf07f74dbe4bcfa37d32bd063870b087c
+stevedore==5.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1c15d95766ca0569cad14cb6272d4d31dae66b011a929d7c18219c176ea1b5c9 \
+    --hash=sha256:46b93ca40e1114cea93d738a6c1e365396981bb6bb78c27045b7587c9473544d
 toml==0.10.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:806143ae5bfb6a3c6e736a764057db0e6a0e05e338b5630894a5f779cabb4f9b \
     --hash=sha256:b3bda1d108d5dd99f4a20d24d9c348e91c4db7ab1b749200bded2f839ccbe68f
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
 tryceratops==2.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:032fa3cf3659c9865a07b59057edf9efe9e38631e6b977fdae04064888cb62ba \
     --hash=sha256:e9d77811d8f7d886c4ceaeadccd2675c6f2d794344775463faf1cb969e49d865
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/lint.txt` & `alluka-0.1.5/piped/python/base-requirements/lint.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/lint.in --output-file python/base-requirements/lint.txt --min-python-version 3.9
 #
-click==8.1.7 ; python_version >= "3.9" and python_version < "4" \
+click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 codespell==2.2.6 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:9ee9a3e5df0990604013ac2a9f22fa8e57669c827124a2e961fe8a1da4cacc07 \
     --hash=sha256:a8c65d8eb3faa03deabab6b3bbe798bea72e1799c7e9e955d57eca4096abcff9
-colorama==0.4.6 ; python_version >= "3.9" and python_version < "4" and platform_system == "Windows" \
+colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-pre-commit-hooks==4.5.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b779d5c44ede9b1fda48e2d96b08e9aa5b1d2fdb8903ca09f0dbaca22d529edb \
-    --hash=sha256:ffbe2af1c85ac9a7695866955680b4dee98822638b748a6f3debefad79748c8a
+pre-commit-hooks==4.6.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a69199e6a2d45ec59c1020a81ca1549abddc2afb798276d9a0d951752d6abbfe \
+    --hash=sha256:eb1f43ee67869cd41b4c59017fad4a0f9d4d61201d163f2135535aaf65035a2b
 ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.13" and python_version >= "3.9" \
     --hash=sha256:024cfe1fc7c7f4e1aff4a81e718109e13409767e4f871443cbff3dba3578203d \
     --hash=sha256:03d1162b6d1df1caa3a4bd27aa51ce17c9afc2046c31b0ad60a0a96ec22f8001 \
     --hash=sha256:07238db9cbdf8fc1e9de2489a4f68474e70dffcb32232db7c08fa61ca0c7c462 \
     --hash=sha256:09b055c05697b38ecacb7ac50bdab2240bfca1a0c4872b0fd309bb07dc9aa3a9 \
     --hash=sha256:1707814f0d9791df063f8c19bb51b0d1278b8e9a2353abbb676c2f685dee6afe \
     --hash=sha256:1758ce7d8e1a29d23de54a16ae867abd370f01b5a69e1a3ba75223eaa3ca1a1b \
@@ -63,16 +63,16 @@
     --hash=sha256:da09ad1c359a728e112d60116f626cc9f29730ff3e0e7db72b9a2dbc2e4beed5 \
     --hash=sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28 \
     --hash=sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d \
     --hash=sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1 \
     --hash=sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2 \
     --hash=sha256:f481f16baec5290e45aebdc2a5168ebc6d35189ae6fea7a58787613a25f6e875 \
     --hash=sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412
-ruamel-yaml==0.18.5 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:61917e3a35a569c1133a8f772e1226961bf5a1198bea7e23f06a0841dea1ab0e \
-    --hash=sha256:a013ac02f99a69cdd6277d9664689eb1acba07069f912823177c5eced21a6ada
-slotscheck==0.17.1 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:214f822016dcc7d3f3b254d5f9b8c731eabdc0e8dd29d0253618f65eb6deade2 \
-    --hash=sha256:fdef47766530df994cf99dda484a15f212eaf6f2e2402026c39348f3f0e62827
+ruamel-yaml==0.18.6 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636 \
+    --hash=sha256:8b27e6a217e786c6fbe5634d8f3f11bc63e0f80f6a5890f28863d9c45aac311b
+slotscheck==0.19.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:53fbc9befacb331a2ab25b385004d99ea72b5cee4f3deb6da676c8f08d0fcdd9 \
+    --hash=sha256:707b4339d280664139ffd2c78fef99b3028e215f13cc77244147dd6126fe2e0d
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/nox.txt` & `alluka-0.1.5/piped/python/base-requirements/nox.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,213 +3,187 @@
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/nox.in --output-file python/base-requirements/nox.txt --min-python-version 3.9
 #
 annotated-types==0.6.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:0641064de18ba7a25dee8f96403ebc39113d0cb953a01429249d5c7564666a43 \
     --hash=sha256:563339e807e53ffd9c267e99fc6d9ea23eb8443c08f112651963e24e22f84a5d
-argcomplete==3.2.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:30891d87f3c1abe091f2142613c9d33cac84a5e15404489f033b20399b691fec \
-    --hash=sha256:437f67fb9b058da5a090df505ef9be0297c4883993f3f56cb186ff087778cfb4
+argcomplete==3.3.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:c168c3723482c031df3c207d4ba8fa702717ccb9fc0bfe4117166c1f537b4a54 \
+    --hash=sha256:fd03ff4a5b9e6580569d34b273f741e85cd9e072f3feeeee3eba4891c70eda62
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-colorlog==6.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4ed23b05a1154294ac99f511fabe8c1d6d4364ec1f7fc989c7fb515ccc29d375 \
-    --hash=sha256:fbb6fdf9d5685f2517f388fb29bb27d54e8654dd31f58bc2a3b217e967a95ca6
+colorlog==6.8.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:3e3e079a41feb5a1b64f978b5ea4f46040a94f11f0e8bbb8261e3dbbeca64d44 \
+    --hash=sha256:4dcbb62368e2800cb3c5abd348da7e53f6c362dda502ec27c560b2e58a66bd33
 distlib==0.3.8 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:034db59a0b96f8ca18035f36290806a9a6e6bd9d1ff91e45a7f172eb17e51784 \
     --hash=sha256:1530ea13e350031b6312d8580ddb6b27a104275a31106523b8f123787f494f64
-filelock==3.13.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:521f5f56c50f8426f5e03ad3b281b490a87ef15bc6c526f168290f0c7148d44e \
-    --hash=sha256:57dbda9b35157b05fb3e58ee91448612eb674172fab98ee235ccb0b5bee19a1c
-jinja2==3.1.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:31351a702a408a9e7595a8fc6150fc3f43bb6bf7e319770cbc0db9df9437e852 \
-    --hash=sha256:6088930bfe239f0e6710546ab9c19c9ef35e29792895fed6e6e31a023a182a61
-markupsafe==2.1.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
-    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
-    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
-    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
-    --hash=sha256:14ff806850827afd6b07a5f32bd917fb7f45b046ba40c57abdb636674a8b559c \
-    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
-    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
-    --hash=sha256:1b8dd8c3fd14349433c79fa8abeb573a55fc0fdd769133baac1f5e07abf54aeb \
-    --hash=sha256:1f67c7038d560d92149c060157d623c542173016c4babc0c1913cca0564b9939 \
-    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
-    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
-    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
-    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
-    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
-    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
-    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
-    --hash=sha256:47d4f1c5f80fc62fdd7777d0d40a2e9dda0a05883ab11374334f6c4de38adffd \
-    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
-    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
-    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
-    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
-    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
-    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
-    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
-    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
-    --hash=sha256:715d3562f79d540f251b99ebd6d8baa547118974341db04f5ad06d5ea3eb8007 \
-    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
-    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
-    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
-    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
-    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
-    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
-    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
-    --hash=sha256:8f9293864fe09b8149f0cc42ce56e3f0e54de883a9de90cd427f191c346eb2e1 \
-    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
-    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
-    --hash=sha256:9aad3c1755095ce347e26488214ef77e0485a3c34a50c5a5e2471dff60b9dd9c \
-    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
-    --hash=sha256:aa57bd9cf8ae831a362185ee444e15a93ecb2e344c8e52e4d721ea3ab6ef1823 \
-    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
-    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
-    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
-    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
-    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
-    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
-    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
-    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
-    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
-    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
-    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
-    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
-    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
-    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
-    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
-    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
-    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
-    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
-    --hash=sha256:f698de3fd0c4e6972b92290a45bd9b1536bffe8c6759c62471efaa8acb4c37bc \
-    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2 \
-    --hash=sha256:ffcc3f7c66b5f5b7931a5aa68fc9cecc51e685ef90282f4a82f0f5e9b704ad11
-nox==2023.4.22 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0b1adc619c58ab4fa57d6ab2e7823fe47a32e70202f287d78474adcc7bda1891 \
-    --hash=sha256:46c0560b0dc609d7d967dc99e22cb463d3c4caf54a5fda735d6c11b5177e3a9f
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
-pydantic-core==2.14.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:00646784f6cd993b1e1c0e7b0fdcbccc375d539db95555477771c27555e3c556 \
-    --hash=sha256:00b1087dabcee0b0ffd104f9f53d7d3eaddfaa314cdd6726143af6bc713aa27e \
-    --hash=sha256:0348b1dc6b76041516e8a854ff95b21c55f5a411c3297d2ca52f5528e49d8411 \
-    --hash=sha256:036137b5ad0cb0004c75b579445a1efccd072387a36c7f217bb8efd1afbe5245 \
-    --hash=sha256:095b707bb287bfd534044166ab767bec70a9bba3175dcdc3371782175c14e43c \
-    --hash=sha256:0c08de15d50fa190d577e8591f0329a643eeaed696d7771760295998aca6bc66 \
-    --hash=sha256:1302a54f87b5cd8528e4d6d1bf2133b6aa7c6122ff8e9dc5220fbc1e07bffebd \
-    --hash=sha256:172de779e2a153d36ee690dbc49c6db568d7b33b18dc56b69a7514aecbcf380d \
-    --hash=sha256:1b027c86c66b8627eb90e57aee1f526df77dc6d8b354ec498be9a757d513b92b \
-    --hash=sha256:1ce830e480f6774608dedfd4a90c42aac4a7af0a711f1b52f807130c2e434c06 \
-    --hash=sha256:1fd0c1d395372843fba13a51c28e3bb9d59bd7aebfeb17358ffaaa1e4dbbe948 \
-    --hash=sha256:23598acb8ccaa3d1d875ef3b35cb6376535095e9405d91a3d57a8c7db5d29341 \
-    --hash=sha256:24368e31be2c88bd69340fbfe741b405302993242ccb476c5c3ff48aeee1afe0 \
-    --hash=sha256:26a92ae76f75d1915806b77cf459811e772d8f71fd1e4339c99750f0e7f6324f \
-    --hash=sha256:27e524624eace5c59af499cd97dc18bb201dc6a7a2da24bfc66ef151c69a5f2a \
-    --hash=sha256:2b8719037e570639e6b665a4050add43134d80b687288ba3ade18b22bbb29dd2 \
-    --hash=sha256:2c5bcf3414367e29f83fd66f7de64509a8fd2368b1edf4351e862910727d3e51 \
-    --hash=sha256:2dbe357bc4ddda078f79d2a36fc1dd0494a7f2fad83a0a684465b6f24b46fe80 \
-    --hash=sha256:2f5fa187bde8524b1e37ba894db13aadd64faa884657473b03a019f625cee9a8 \
-    --hash=sha256:2f6ffc6701a0eb28648c845f4945a194dc7ab3c651f535b81793251e1185ac3d \
-    --hash=sha256:314ccc4264ce7d854941231cf71b592e30d8d368a71e50197c905874feacc8a8 \
-    --hash=sha256:36026d8f99c58d7044413e1b819a67ca0e0b8ebe0f25e775e6c3d1fabb3c38fb \
-    --hash=sha256:36099c69f6b14fc2c49d7996cbf4f87ec4f0e66d1c74aa05228583225a07b590 \
-    --hash=sha256:36fa402dcdc8ea7f1b0ddcf0df4254cc6b2e08f8cd80e7010d4c4ae6e86b2a87 \
-    --hash=sha256:370ffecb5316ed23b667d99ce4debe53ea664b99cc37bfa2af47bc769056d534 \
-    --hash=sha256:3860c62057acd95cc84044e758e47b18dcd8871a328ebc8ccdefd18b0d26a21b \
-    --hash=sha256:399ac0891c284fa8eb998bcfa323f2234858f5d2efca3950ae58c8f88830f145 \
-    --hash=sha256:3a0b5db001b98e1c649dd55afa928e75aa4087e587b9524a4992316fa23c9fba \
-    --hash=sha256:3dcf1978be02153c6a31692d4fbcc2a3f1db9da36039ead23173bc256ee3b91b \
-    --hash=sha256:4241204e4b36ab5ae466ecec5c4c16527a054c69f99bba20f6f75232a6a534e2 \
-    --hash=sha256:438027a975cc213a47c5d70672e0d29776082155cfae540c4e225716586be75e \
-    --hash=sha256:43e166ad47ba900f2542a80d83f9fc65fe99eb63ceec4debec160ae729824052 \
-    --hash=sha256:478e9e7b360dfec451daafe286998d4a1eeaecf6d69c427b834ae771cad4b622 \
-    --hash=sha256:4ce8299b481bcb68e5c82002b96e411796b844d72b3e92a3fbedfe8e19813eab \
-    --hash=sha256:4f86f1f318e56f5cbb282fe61eb84767aee743ebe32c7c0834690ebea50c0a6b \
-    --hash=sha256:55a23dcd98c858c0db44fc5c04fc7ed81c4b4d33c653a7c45ddaebf6563a2f66 \
-    --hash=sha256:599c87d79cab2a6a2a9df4aefe0455e61e7d2aeede2f8577c1b7c0aec643ee8e \
-    --hash=sha256:5aa90562bc079c6c290f0512b21768967f9968e4cfea84ea4ff5af5d917016e4 \
-    --hash=sha256:64634ccf9d671c6be242a664a33c4acf12882670b09b3f163cd00a24cffbd74e \
-    --hash=sha256:667aa2eac9cd0700af1ddb38b7b1ef246d8cf94c85637cbb03d7757ca4c3fdec \
-    --hash=sha256:6a31d98c0d69776c2576dda4b77b8e0c69ad08e8b539c25c7d0ca0dc19a50d6c \
-    --hash=sha256:6af4b3f52cc65f8a0bc8b1cd9676f8c21ef3e9132f21fed250f6958bd7223bed \
-    --hash=sha256:6c8edaea3089bf908dd27da8f5d9e395c5b4dc092dbcce9b65e7156099b4b937 \
-    --hash=sha256:71d72ca5eaaa8d38c8df16b7deb1a2da4f650c41b58bb142f3fb75d5ad4a611f \
-    --hash=sha256:72f9a942d739f09cd42fffe5dc759928217649f070056f03c70df14f5770acf9 \
-    --hash=sha256:747265448cb57a9f37572a488a57d873fd96bf51e5bb7edb52cfb37124516da4 \
-    --hash=sha256:75ec284328b60a4e91010c1acade0c30584f28a1f345bc8f72fe8b9e46ec6a96 \
-    --hash=sha256:78d0768ee59baa3de0f4adac9e3748b4b1fffc52143caebddfd5ea2961595277 \
-    --hash=sha256:78ee52ecc088c61cce32b2d30a826f929e1708f7b9247dc3b921aec367dc1b23 \
-    --hash=sha256:7be719e4d2ae6c314f72844ba9d69e38dff342bc360379f7c8537c48e23034b7 \
-    --hash=sha256:7e1f4744eea1501404b20b0ac059ff7e3f96a97d3e3f48ce27a139e053bb370b \
-    --hash=sha256:7e90d6cc4aad2cc1f5e16ed56e46cebf4877c62403a311af20459c15da76fd91 \
-    --hash=sha256:7ebe3416785f65c28f4f9441e916bfc8a54179c8dea73c23023f7086fa601c5d \
-    --hash=sha256:7f41533d7e3cf9520065f610b41ac1c76bc2161415955fbcead4981b22c7611e \
-    --hash=sha256:7f5025db12fc6de7bc1104d826d5aee1d172f9ba6ca936bf6474c2148ac336c1 \
-    --hash=sha256:86c963186ca5e50d5c8287b1d1c9d3f8f024cbe343d048c5bd282aec2d8641f2 \
-    --hash=sha256:86ce5fcfc3accf3a07a729779d0b86c5d0309a4764c897d86c11089be61da160 \
-    --hash=sha256:8a14c192c1d724c3acbfb3f10a958c55a2638391319ce8078cb36c02283959b9 \
-    --hash=sha256:8b93785eadaef932e4fe9c6e12ba67beb1b3f1e5495631419c784ab87e975670 \
-    --hash=sha256:8ed1af8692bd8d2a29d702f1a2e6065416d76897d726e45a1775b1444f5928a7 \
-    --hash=sha256:92879bce89f91f4b2416eba4429c7b5ca22c45ef4a499c39f0c5c69257522c7c \
-    --hash=sha256:94fc0e6621e07d1e91c44e016cc0b189b48db053061cc22d6298a611de8071bb \
-    --hash=sha256:982487f8931067a32e72d40ab6b47b1628a9c5d344be7f1a4e668fb462d2da42 \
-    --hash=sha256:9862bf828112e19685b76ca499b379338fd4c5c269d897e218b2ae8fcb80139d \
-    --hash=sha256:99b14dbea2fdb563d8b5a57c9badfcd72083f6006caf8e126b491519c7d64ca8 \
-    --hash=sha256:9c6a5c79b28003543db3ba67d1df336f253a87d3112dac3a51b94f7d48e4c0e1 \
-    --hash=sha256:a19b794f8fe6569472ff77602437ec4430f9b2b9ec7a1105cfd2232f9ba355e6 \
-    --hash=sha256:a306cdd2ad3a7d795d8e617a58c3a2ed0f76c8496fb7621b6cd514eb1532cae8 \
-    --hash=sha256:a3dde6cac75e0b0902778978d3b1646ca9f438654395a362cb21d9ad34b24acf \
-    --hash=sha256:a874f21f87c485310944b2b2734cd6d318765bcbb7515eead33af9641816506e \
-    --hash=sha256:a983cca5ed1dd9a35e9e42ebf9f278d344603bfcb174ff99a5815f953925140a \
-    --hash=sha256:aca48506a9c20f68ee61c87f2008f81f8ee99f8d7f0104bff3c47e2d148f89d9 \
-    --hash=sha256:b2602177668f89b38b9f84b7b3435d0a72511ddef45dc14446811759b82235a1 \
-    --hash=sha256:b3e5fe4538001bb82e2295b8d2a39356a84694c97cb73a566dc36328b9f83b40 \
-    --hash=sha256:b6ca36c12a5120bad343eef193cc0122928c5c7466121da7c20f41160ba00ba2 \
-    --hash=sha256:b89f4477d915ea43b4ceea6756f63f0288941b6443a2b28c69004fe07fde0d0d \
-    --hash=sha256:b9a9d92f10772d2a181b5ca339dee066ab7d1c9a34ae2421b2a52556e719756f \
-    --hash=sha256:c99462ffc538717b3e60151dfaf91125f637e801f5ab008f81c402f1dff0cd0f \
-    --hash=sha256:cb92f9061657287eded380d7dc455bbf115430b3aa4741bdc662d02977e7d0af \
-    --hash=sha256:cdee837710ef6b56ebd20245b83799fce40b265b3b406e51e8ccc5b85b9099b7 \
-    --hash=sha256:cf10b7d58ae4a1f07fccbf4a0a956d705356fea05fb4c70608bb6fa81d103cda \
-    --hash=sha256:d15687d7d7f40333bd8266f3814c591c2e2cd263fa2116e314f60d82086e353a \
-    --hash=sha256:d5c28525c19f5bb1e09511669bb57353d22b94cf8b65f3a8d141c389a55dec95 \
-    --hash=sha256:d5f916acf8afbcab6bacbb376ba7dc61f845367901ecd5e328fc4d4aef2fcab0 \
-    --hash=sha256:dab03ed811ed1c71d700ed08bde8431cf429bbe59e423394f0f4055f1ca0ea60 \
-    --hash=sha256:db453f2da3f59a348f514cfbfeb042393b68720787bbef2b4c6068ea362c8149 \
-    --hash=sha256:de2a0645a923ba57c5527497daf8ec5df69c6eadf869e9cd46e86349146e5975 \
-    --hash=sha256:dea7fcd62915fb150cdc373212141a30037e11b761fbced340e9db3379b892d4 \
-    --hash=sha256:dfcbebdb3c4b6f739a91769aea5ed615023f3c88cb70df812849aef634c25fbe \
-    --hash=sha256:dfcebb950aa7e667ec226a442722134539e77c575f6cfaa423f24371bb8d2e94 \
-    --hash=sha256:e0641b506486f0b4cd1500a2a65740243e8670a2549bb02bc4556a83af84ae03 \
-    --hash=sha256:e33b0834f1cf779aa839975f9d8755a7c2420510c0fa1e9fa0497de77cd35d2c \
-    --hash=sha256:e4ace1e220b078c8e48e82c081e35002038657e4b37d403ce940fa679e57113b \
-    --hash=sha256:e4cf2d5829f6963a5483ec01578ee76d329eb5caf330ecd05b3edd697e7d768a \
-    --hash=sha256:e574de99d735b3fc8364cba9912c2bec2da78775eba95cbb225ef7dda6acea24 \
-    --hash=sha256:e646c0e282e960345314f42f2cea5e0b5f56938c093541ea6dbf11aec2862391 \
-    --hash=sha256:e8a5ac97ea521d7bde7621d86c30e86b798cdecd985723c4ed737a2aa9e77d0c \
-    --hash=sha256:eedf97be7bc3dbc8addcef4142f4b4164066df0c6f36397ae4aaed3eb187d8ab \
-    --hash=sha256:ef633add81832f4b56d3b4c9408b43d530dfca29e68fb1b797dcb861a2c734cd \
-    --hash=sha256:f27207e8ca3e5e021e2402ba942e5b4c629718e665c81b8b306f3c8b1ddbb786 \
-    --hash=sha256:f85f3843bdb1fe80e8c206fe6eed7a1caeae897e496542cee499c374a85c6e08 \
-    --hash=sha256:f8e81e4b55930e5ffab4a68db1af431629cf2e4066dbdbfef65348b8ab804ea8 \
-    --hash=sha256:f96ae96a060a8072ceff4cfde89d261837b4294a4f28b84a28765470d502ccc6 \
-    --hash=sha256:fd9e98b408384989ea4ab60206b8e100d8687da18b5c813c11e92fd8212a98e0 \
-    --hash=sha256:ffff855100bc066ff2cd3aa4a60bc9534661816b110f0243e59503ec2df38421
-pydantic==2.5.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b3ef57c62535b0941697cce638c08900d87fcb67e29cfa99e8a68f747f393f7a \
-    --hash=sha256:d0caf5954bee831b6bfe7e338c32b9e30c85dfe080c843680783ac2b631673b4
+filelock==3.13.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:404e5e9253aa60ad457cae1be07c0f0ca90a63931200a47d9b6a6af84fd7b45f \
+    --hash=sha256:d13f466618bfde72bd2c18255e269f72542c6e70e7bac83a0232d6b1cc5c8cf4
+jinja2==3.1.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7d6d50dd97d52cbc355597bd845fabfbac3f551e1f99619e39a35ce8c370b5fa \
+    --hash=sha256:ac8bd6544d4bb2c9792bf3a159e80bba8fda7f07e81bc3aed565432d5925ba90
+markupsafe==2.1.5 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00e046b6dd71aa03a41079792f8473dc494d564611a8f89bbbd7cb93295ebdcf \
+    --hash=sha256:075202fa5b72c86ad32dc7d0b56024ebdbcf2048c0ba09f1cde31bfdd57bcfff \
+    --hash=sha256:0e397ac966fdf721b2c528cf028494e86172b4feba51d65f81ffd65c63798f3f \
+    --hash=sha256:17b950fccb810b3293638215058e432159d2b71005c74371d784862b7e4683f3 \
+    --hash=sha256:1f3fbcb7ef1f16e48246f704ab79d79da8a46891e2da03f8783a5b6fa41a9532 \
+    --hash=sha256:2174c595a0d73a3080ca3257b40096db99799265e1c27cc5a610743acd86d62f \
+    --hash=sha256:2b7c57a4dfc4f16f7142221afe5ba4e093e09e728ca65c51f5620c9aaeb9a617 \
+    --hash=sha256:2d2d793e36e230fd32babe143b04cec8a8b3eb8a3122d2aceb4a371e6b09b8df \
+    --hash=sha256:30b600cf0a7ac9234b2638fbc0fb6158ba5bdcdf46aeb631ead21248b9affbc4 \
+    --hash=sha256:397081c1a0bfb5124355710fe79478cdbeb39626492b15d399526ae53422b906 \
+    --hash=sha256:3a57fdd7ce31c7ff06cdfbf31dafa96cc533c21e443d57f5b1ecc6cdc668ec7f \
+    --hash=sha256:3c6b973f22eb18a789b1460b4b91bf04ae3f0c4234a0a6aa6b0a92f6f7b951d4 \
+    --hash=sha256:3e53af139f8579a6d5f7b76549125f0d94d7e630761a2111bc431fd820e163b8 \
+    --hash=sha256:4096e9de5c6fdf43fb4f04c26fb114f61ef0bf2e5604b6ee3019d51b69e8c371 \
+    --hash=sha256:4275d846e41ecefa46e2015117a9f491e57a71ddd59bbead77e904dc02b1bed2 \
+    --hash=sha256:4c31f53cdae6ecfa91a77820e8b151dba54ab528ba65dfd235c80b086d68a465 \
+    --hash=sha256:4f11aa001c540f62c6166c7726f71f7573b52c68c31f014c25cc7901deea0b52 \
+    --hash=sha256:5049256f536511ee3f7e1b3f87d1d1209d327e818e6ae1365e8653d7e3abb6a6 \
+    --hash=sha256:58c98fee265677f63a4385256a6d7683ab1832f3ddd1e66fe948d5880c21a169 \
+    --hash=sha256:598e3276b64aff0e7b3451b72e94fa3c238d452e7ddcd893c3ab324717456bad \
+    --hash=sha256:5b7b716f97b52c5a14bffdf688f971b2d5ef4029127f1ad7a513973cfd818df2 \
+    --hash=sha256:5dedb4db619ba5a2787a94d877bc8ffc0566f92a01c0ef214865e54ecc9ee5e0 \
+    --hash=sha256:619bc166c4f2de5caa5a633b8b7326fbe98e0ccbfacabd87268a2b15ff73a029 \
+    --hash=sha256:629ddd2ca402ae6dbedfceeba9c46d5f7b2a61d9749597d4307f943ef198fc1f \
+    --hash=sha256:656f7526c69fac7f600bd1f400991cc282b417d17539a1b228617081106feb4a \
+    --hash=sha256:6ec585f69cec0aa07d945b20805be741395e28ac1627333b1c5b0105962ffced \
+    --hash=sha256:72b6be590cc35924b02c78ef34b467da4ba07e4e0f0454a2c5907f473fc50ce5 \
+    --hash=sha256:7502934a33b54030eaf1194c21c692a534196063db72176b0c4028e140f8f32c \
+    --hash=sha256:7a68b554d356a91cce1236aa7682dc01df0edba8d043fd1ce607c49dd3c1edcf \
+    --hash=sha256:7b2e5a267c855eea6b4283940daa6e88a285f5f2a67f2220203786dfa59b37e9 \
+    --hash=sha256:823b65d8706e32ad2df51ed89496147a42a2a6e01c13cfb6ffb8b1e92bc910bb \
+    --hash=sha256:8590b4ae07a35970728874632fed7bd57b26b0102df2d2b233b6d9d82f6c62ad \
+    --hash=sha256:8dd717634f5a044f860435c1d8c16a270ddf0ef8588d4887037c5028b859b0c3 \
+    --hash=sha256:8dec4936e9c3100156f8a2dc89c4b88d5c435175ff03413b443469c7c8c5f4d1 \
+    --hash=sha256:97cafb1f3cbcd3fd2b6fbfb99ae11cdb14deea0736fc2b0952ee177f2b813a46 \
+    --hash=sha256:a17a92de5231666cfbe003f0e4b9b3a7ae3afb1ec2845aadc2bacc93ff85febc \
+    --hash=sha256:a549b9c31bec33820e885335b451286e2969a2d9e24879f83fe904a5ce59d70a \
+    --hash=sha256:ac07bad82163452a6884fe8fa0963fb98c2346ba78d779ec06bd7a6262132aee \
+    --hash=sha256:ae2ad8ae6ebee9d2d94b17fb62763125f3f374c25618198f40cbb8b525411900 \
+    --hash=sha256:b91c037585eba9095565a3556f611e3cbfaa42ca1e865f7b8015fe5c7336d5a5 \
+    --hash=sha256:bc1667f8b83f48511b94671e0e441401371dfd0f0a795c7daa4a3cd1dde55bea \
+    --hash=sha256:bec0a414d016ac1a18862a519e54b2fd0fc8bbfd6890376898a6c0891dd82e9f \
+    --hash=sha256:bf50cd79a75d181c9181df03572cdce0fbb75cc353bc350712073108cba98de5 \
+    --hash=sha256:bff1b4290a66b490a2f4719358c0cdcd9bafb6b8f061e45c7a2460866bf50c2e \
+    --hash=sha256:c061bb86a71b42465156a3ee7bd58c8c2ceacdbeb95d05a99893e08b8467359a \
+    --hash=sha256:c8b29db45f8fe46ad280a7294f5c3ec36dbac9491f2d1c17345be8e69cc5928f \
+    --hash=sha256:ce409136744f6521e39fd8e2a24c53fa18ad67aa5bc7c2cf83645cce5b5c4e50 \
+    --hash=sha256:d050b3361367a06d752db6ead6e7edeb0009be66bc3bae0ee9d97fb326badc2a \
+    --hash=sha256:d283d37a890ba4c1ae73ffadf8046435c76e7bc2247bbb63c00bd1a709c6544b \
+    --hash=sha256:d9fad5155d72433c921b782e58892377c44bd6252b5af2f67f16b194987338a4 \
+    --hash=sha256:daa4ee5a243f0f20d528d939d06670a298dd39b1ad5f8a72a4275124a7819eff \
+    --hash=sha256:db0b55e0f3cc0be60c1f19efdde9a637c32740486004f20d1cff53c3c0ece4d2 \
+    --hash=sha256:e61659ba32cf2cf1481e575d0462554625196a1f2fc06a1c777d3f48e8865d46 \
+    --hash=sha256:ea3d8a3d18833cf4304cd2fc9cbb1efe188ca9b5efef2bdac7adc20594a0e46b \
+    --hash=sha256:ec6a563cff360b50eed26f13adc43e61bc0c04d94b8be985e6fb24b81f6dcfdf \
+    --hash=sha256:f5dfb42c4604dddc8e4305050aa6deb084540643ed5804d7455b5df8fe16f5e5 \
+    --hash=sha256:fa173ec60341d6bb97a89f5ea19c85c5643c1e7dedebc22f5181eb73573142c5 \
+    --hash=sha256:fa9db3f79de01457b03d4f01b34cf91bc0048eb2c3846ff26f66687c2f6d16ab \
+    --hash=sha256:fce659a462a1be54d2ffcacea5e3ba2d74daa74f30f5f143fe0c58636e355fdd \
+    --hash=sha256:ffee1f21e5ef0d712f9033568f8344d5da8cc2869dbd08d87c84656e6a2d2f68
+nox==2024.4.15 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6492236efa15a460ecb98e7b67562a28b70da006ab0be164e8821177577c0565 \
+    --hash=sha256:ecf6700199cdfa9e5ea0a41ff5e6ef4641d09508eda6edb89d9987864115817f
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+pydantic-core==2.18.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:030e4f9516f9947f38179249778709a460a3adb516bf39b5eb9066fcfe43d0e6 \
+    --hash=sha256:09f03dfc0ef8c22622eaa8608caa4a1e189cfb83ce847045eca34f690895eccb \
+    --hash=sha256:12a05db5013ec0ca4a32cc6433f53faa2a014ec364031408540ba858c2172bb0 \
+    --hash=sha256:14fe73881cf8e4cbdaded8ca0aa671635b597e42447fec7060d0868b52d074e6 \
+    --hash=sha256:1a0c3e718f4e064efde68092d9d974e39572c14e56726ecfaeebbe6544521f47 \
+    --hash=sha256:1be91ad664fc9245404a789d60cba1e91c26b1454ba136d2a1bf0c2ac0c0505a \
+    --hash=sha256:201713f2f462e5c015b343e86e68bd8a530a4f76609b33d8f0ec65d2b921712a \
+    --hash=sha256:2027493cc44c23b598cfaf200936110433d9caa84e2c6cf487a83999638a96ac \
+    --hash=sha256:250ae39445cb5475e483a36b1061af1bc233de3e9ad0f4f76a71b66231b07f88 \
+    --hash=sha256:2533ad2883f001efa72f3d0e733fb846710c3af6dcdd544fe5bf14fa5fe2d7db \
+    --hash=sha256:25595ac311f20e5324d1941909b0d12933f1fd2171075fcff763e90f43e92a0d \
+    --hash=sha256:2684a94fdfd1b146ff10689c6e4e815f6a01141781c493b97342cdc5b06f4d5d \
+    --hash=sha256:27f1009dc292f3b7ca77feb3571c537276b9aad5dd4efb471ac88a8bd09024e9 \
+    --hash=sha256:2adaeea59849ec0939af5c5d476935f2bab4b7f0335b0110f0f069a41024278e \
+    --hash=sha256:2ae80f72bb7a3e397ab37b53a2b49c62cc5496412e71bc4f1277620a7ce3f52b \
+    --hash=sha256:2d5728e93d28a3c63ee513d9ffbac9c5989de8c76e049dbcb5bfe4b923a9739d \
+    --hash=sha256:2e91711e36e229978d92642bfc3546333a9127ecebb3f2761372e096395fc649 \
+    --hash=sha256:2fe0c1ce5b129455e43f941f7a46f61f3d3861e571f2905d55cdbb8b5c6f5e2c \
+    --hash=sha256:38a5024de321d672a132b1834a66eeb7931959c59964b777e8f32dbe9523f6b1 \
+    --hash=sha256:3e352f0191d99fe617371096845070dee295444979efb8f27ad941227de6ad09 \
+    --hash=sha256:48dd883db92e92519201f2b01cafa881e5f7125666141a49ffba8b9facc072b0 \
+    --hash=sha256:54764c083bbe0264f0f746cefcded6cb08fbbaaf1ad1d78fb8a4c30cff999a90 \
+    --hash=sha256:54c7375c62190a7845091f521add19b0f026bcf6ae674bdb89f296972272e86d \
+    --hash=sha256:561cf62c8a3498406495cfc49eee086ed2bb186d08bcc65812b75fda42c38294 \
+    --hash=sha256:56823a92075780582d1ffd4489a2e61d56fd3ebb4b40b713d63f96dd92d28144 \
+    --hash=sha256:582cf2cead97c9e382a7f4d3b744cf0ef1a6e815e44d3aa81af3ad98762f5a9b \
+    --hash=sha256:58aca931bef83217fca7a390e0486ae327c4af9c3e941adb75f8772f8eeb03a1 \
+    --hash=sha256:5f7973c381283783cd1043a8c8f61ea5ce7a3a58b0369f0ee0ee975eaf2f2a1b \
+    --hash=sha256:6395a4435fa26519fd96fdccb77e9d00ddae9dd6c742309bd0b5610609ad7fb2 \
+    --hash=sha256:63d7523cd95d2fde0d28dc42968ac731b5bb1e516cc56b93a50ab293f4daeaad \
+    --hash=sha256:641a018af4fe48be57a2b3d7a1f0f5dbca07c1d00951d3d7463f0ac9dac66622 \
+    --hash=sha256:667880321e916a8920ef49f5d50e7983792cf59f3b6079f3c9dac2b88a311d17 \
+    --hash=sha256:684d840d2c9ec5de9cb397fcb3f36d5ebb6fa0d94734f9886032dd796c1ead06 \
+    --hash=sha256:68717c38a68e37af87c4da20e08f3e27d7e4212e99e96c3d875fbf3f4812abfc \
+    --hash=sha256:6b7bbb97d82659ac8b37450c60ff2e9f97e4eb0f8a8a3645a5568b9334b08b50 \
+    --hash=sha256:72722ce529a76a4637a60be18bd789d8fb871e84472490ed7ddff62d5fed620d \
+    --hash=sha256:73c1bc8a86a5c9e8721a088df234265317692d0b5cd9e86e975ce3bc3db62a59 \
+    --hash=sha256:76909849d1a6bffa5a07742294f3fa1d357dc917cb1fe7b470afbc3a7579d539 \
+    --hash=sha256:76b86e24039c35280ceee6dce7e62945eb93a5175d43689ba98360ab31eebc4a \
+    --hash=sha256:7a5d83efc109ceddb99abd2c1316298ced2adb4570410defe766851a804fcd5b \
+    --hash=sha256:80e0e57cc704a52fb1b48f16d5b2c8818da087dbee6f98d9bf19546930dc64b5 \
+    --hash=sha256:85233abb44bc18d16e72dc05bf13848a36f363f83757541f1a97db2f8d58cfd9 \
+    --hash=sha256:907a4d7720abfcb1c81619863efd47c8a85d26a257a2dbebdb87c3b847df0278 \
+    --hash=sha256:9376d83d686ec62e8b19c0ac3bf8d28d8a5981d0df290196fb6ef24d8a26f0d6 \
+    --hash=sha256:94b9769ba435b598b547c762184bcfc4783d0d4c7771b04a3b45775c3589ca44 \
+    --hash=sha256:9a29726f91c6cb390b3c2338f0df5cd3e216ad7a938762d11c994bb37552edb0 \
+    --hash=sha256:9b6431559676a1079eac0f52d6d0721fb8e3c5ba43c37bc537c8c83724031feb \
+    --hash=sha256:9ece8a49696669d483d206b4474c367852c44815fca23ac4e48b72b339807f80 \
+    --hash=sha256:a139fe9f298dc097349fb4f28c8b81cc7a202dbfba66af0e14be5cfca4ef7ce5 \
+    --hash=sha256:a32204489259786a923e02990249c65b0f17235073149d0033efcebe80095570 \
+    --hash=sha256:a3982b0a32d0a88b3907e4b0dc36809fda477f0757c59a505d4e9b455f384b8b \
+    --hash=sha256:aad17e462f42ddbef5984d70c40bfc4146c322a2da79715932cd8976317054de \
+    --hash=sha256:b560b72ed4816aee52783c66854d96157fd8175631f01ef58e894cc57c84f0f6 \
+    --hash=sha256:b6b0e4912030c6f28bcb72b9ebe4989d6dc2eebcd2a9cdc35fefc38052dd4fe8 \
+    --hash=sha256:baf1c7b78cddb5af00971ad5294a4583188bda1495b13760d9f03c9483bb6203 \
+    --hash=sha256:c0295d52b012cbe0d3059b1dba99159c3be55e632aae1999ab74ae2bd86a33d7 \
+    --hash=sha256:c562b49c96906b4029b5685075fe1ebd3b5cc2601dfa0b9e16c2c09d6cbce048 \
+    --hash=sha256:c69567ddbac186e8c0aadc1f324a60a564cfe25e43ef2ce81bcc4b8c3abffbae \
+    --hash=sha256:ca71d501629d1fa50ea7fa3b08ba884fe10cefc559f5c6c8dfe9036c16e8ae89 \
+    --hash=sha256:ca976884ce34070799e4dfc6fbd68cb1d181db1eefe4a3a94798ddfb34b8867f \
+    --hash=sha256:d0491006a6ad20507aec2be72e7831a42efc93193d2402018007ff827dc62926 \
+    --hash=sha256:d074b07a10c391fc5bbdcb37b2f16f20fcd9e51e10d01652ab298c0d07908ee2 \
+    --hash=sha256:d2ce426ee691319d4767748c8e0895cfc56593d725594e415f274059bcf3cb76 \
+    --hash=sha256:d4284c621f06a72ce2cb55f74ea3150113d926a6eb78ab38340c08f770eb9b4d \
+    --hash=sha256:d5e6b7155b8197b329dc787356cfd2684c9d6a6b1a197f6bbf45f5555a98d411 \
+    --hash=sha256:d816f44a51ba5175394bc6c7879ca0bd2be560b2c9e9f3411ef3a4cbe644c2e9 \
+    --hash=sha256:dd3f79e17b56741b5177bcc36307750d50ea0698df6aa82f69c7db32d968c1c2 \
+    --hash=sha256:dd63cec4e26e790b70544ae5cc48d11b515b09e05fdd5eff12e3195f54b8a586 \
+    --hash=sha256:de9d3e8717560eb05e28739d1b35e4eac2e458553a52a301e51352a7ffc86a35 \
+    --hash=sha256:df4249b579e75094f7e9bb4bd28231acf55e308bf686b952f43100a5a0be394c \
+    --hash=sha256:e178e5b66a06ec5bf51668ec0d4ac8cfb2bdcb553b2c207d58148340efd00143 \
+    --hash=sha256:e60defc3c15defb70bb38dd605ff7e0fae5f6c9c7cbfe0ad7868582cb7e844a6 \
+    --hash=sha256:ee2794111c188548a4547eccc73a6a8527fe2af6cf25e1a4ebda2fd01cdd2e60 \
+    --hash=sha256:ee7ccc7fb7e921d767f853b47814c3048c7de536663e82fbc37f5eb0d532224b \
+    --hash=sha256:ee9cf33e7fe14243f5ca6977658eb7d1042caaa66847daacbd2117adb258b226 \
+    --hash=sha256:f0f17814c505f07806e22b28856c59ac80cee7dd0fbb152aed273e116378f519 \
+    --hash=sha256:f3202a429fe825b699c57892d4371c74cc3456d8d71b7f35d6028c96dfecad31 \
+    --hash=sha256:f7054fdc556f5421f01e39cbb767d5ec5c1139ea98c3e5b350e02e62201740c7 \
+    --hash=sha256:fd1a9edb9dd9d79fbeac1ea1f9a8dd527a6113b18d2e9bcc0d541d308dae639b
+pydantic==2.7.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:9dee74a271705f14f9a1567671d144a851c675b072736f0a7b2608fd9e495352 \
+    --hash=sha256:b5ecdd42262ca2462e2624793551e80911a1e989f462910bb81aef974b4bb383
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-virtualenv==20.25.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:4238949c5ffe6876362d9c0180fc6c3a824a7b12b80604eeb8085f2ed7460de3 \
-    --hash=sha256:bf51c0d9c7dd63ea8e44086fa1e4fb1093a31e963b86959257378aef020e1f1b
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
+virtualenv==20.25.3 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:7bb554bbdfeaacc3349fa614ea5bff6ac300fc7c335e9facf3a3bcfc703f45be \
+    --hash=sha256:8aac4332f2ea6ef519c648d0bc48a5b1d324994753519919bddbb1aff25a104e
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/publish.txt` & `alluka-0.1.5/piped/python/base-requirements/publish.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/publish.in --output-file python/base-requirements/publish.txt --min-python-version 3.9
 #
-certifi==2023.11.17 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9b469f3a900bf28dc19b8cfbf8019bf47f7fdd1a65a1d4ffb98fc14166beb4d1 \
-    --hash=sha256:e036ab49d5b79556f99cfc2d9320b34cfbe5be05c5871b51de9329f0603b0474
+certifi==2024.2.2 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0569859f95fc761b18b45ef421b1290a0f65f147e92a1e5eb3e635f9a5e4e66f \
+    --hash=sha256:dc383c07b76109f368f6106eee2b593b04a011ea4d55f652c6ca24a754d1cdd1
 charset-normalizer==3.3.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:06435b539f889b1f6f4ac1758871aae42dc3a8c0e24ac9e60c2384973ad73027 \
     --hash=sha256:06a81e93cd441c56a9b65d8e1d043daeb97a3d0856d177d5c90ba85acb3db087 \
     --hash=sha256:0a55554a2fa0d408816b3b5cedf0045f4b8e1a6065aec45849de2d6f3f8e9786 \
     --hash=sha256:0b2b64d2bb6d3fb9112bafa732def486049e63de9618b5843bcdd081d8144cd8 \
     --hash=sha256:10955842570876604d404661fbccbc9c7e684caf432c09c715ec38fbae45ae09 \
     --hash=sha256:122c7fa62b130ed55f8f285bfd56d5f4b4a5b503609d181f9ad85e55c89f4185 \
@@ -94,28 +94,28 @@
     --hash=sha256:eb8821e09e916165e160797a6c17edda0679379a4be5c716c260e836e122f54b \
     --hash=sha256:efcb3f6676480691518c177e3b465bcddf57cea040302f9f4e6e191af91174d4 \
     --hash=sha256:f27273b60488abe721a075bcca6d7f3964f9f6f067c8c4c605743023d7d3944f \
     --hash=sha256:f30c3cb33b24454a82faecaf01b19c18562b1e89558fb6c56de4d9118a032fd5 \
     --hash=sha256:fb69256e180cb6c8a894fee62b3afebae785babc1ee98b81cdf68bbca1987f33 \
     --hash=sha256:fd1abc0d89e30cc4e02e4064dc67fcc51bd941eb395c502aac3ec19fab46b519 \
     --hash=sha256:ff8fa367d09b717b2a17a052544193ad76cd49979c805768879cb63d9ca50561
-docutils==0.20.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:96f387a2c5562db4476f09f13bbab2192e764cac08ebbf3a34a95d9b1e4a59d6 \
-    --hash=sha256:f08a4e276c3a1583a86dce3e34aba3fe04d02bba2dd51ed16106244e8a923e3b
+docutils==0.21.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:14c8d34a55b46c88f9f714adb29cefbdd69fb82f3fef825e59c5faab935390d8 \
+    --hash=sha256:65249d8a5345bc95e0f40f280ba63c98eb24de35c6c8f5b662e3e8948adea83f
 flit-core==3.9.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:72ad266176c4a3fcfab5f2930d76896059851240570ce9a98733b658cb786eba \
     --hash=sha256:7aada352fb0c7f5538c4fafeddf314d3a6a92ee8e2b1de70482329e42de70301
 flit==3.9.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:076c3aaba5ac24cf0ad3251f910900d95a08218e6bcb26f21fef1036cc4679ca \
     --hash=sha256:d75edf5eb324da20d53570a6a6f87f51e606eee8384925cd66a90611140844c7
-idna==3.6 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:9ecdbbd083b06798ae1e86adcbfe8ab1479cf864e4ee30fe4e46a003d12491ca \
-    --hash=sha256:c05567e9c24a6b9faaa835c4821bad0590fbb9d5779e7caa6e1cc4978e7eb24f
+idna==3.7 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:028ff3aadf0609c1fd278d8ea3089299412a7a8b9bd005dd08b9f8285bcb5cfc \
+    --hash=sha256:82fee1fc78add43492d3a1898bfa6d8a904cc97d8427f683ed8e798d07761aa0
 requests==2.31.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:58cd2187c01e70e6e26505bca751777aa9f2ee0b7f4300988b709f44e013003f \
     --hash=sha256:942c5a758f98d790eaed1a29cb6eefc7ffb0d1cf7af05c3d2791656dbd6ad1e1
 tomli-w==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:9f2a07e8be30a0729e533ec968016807069991ae2fd921a78d42f429ae5f4463 \
     --hash=sha256:f463434305e0336248cac9c2dc8076b707d8a12d019dd349f5c1e382dd1ae1b9
-urllib3==2.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:55901e917a5896a349ff771be919f8bd99aff50b79fe58fec595eb37bbc56bb3 \
-    --hash=sha256:df7aa8afb0148fa78488e7899b2c59b5f4ffcfa82e6c54ccb9dd37c1d7b52d54
+urllib3==2.2.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:450b20ec296a467077128bff42b73080516e71b56ff59a60a02bef2232c4fa9d \
+    --hash=sha256:d0570876c61ab9e520d776c38acbbb5b05a776d3f9ff98a5c8fd5162a444cf19
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/reformat.txt` & `alluka-0.1.5/piped/python/base-requirements/reformat.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,95 +1,98 @@
 #
 # This file is autogenerated by pip-compile-cross-platform
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/reformat.in --output-file python/base-requirements/reformat.txt --min-python-version 3.9
 #
-black==23.12.1 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0808494f2b2df923ffc5723ed3c7b096bd76341f6213989759287611e9837d50 \
-    --hash=sha256:1fa88a0f74e50e4487477bc0bb900c6781dbddfdfa32691e780bf854c3b4a47f \
-    --hash=sha256:25e57fd232a6d6ff3f4478a6fd0580838e47c93c83eaf1ccc92d4faf27112c4e \
-    --hash=sha256:2d9e13db441c509a3763a7a3d9a49ccc1b4e974a47be4e08ade2a228876500ec \
-    --hash=sha256:3e1b38b3135fd4c025c28c55ddfc236b05af657828a8a6abe5deec419a0b7055 \
-    --hash=sha256:3fa4be75ef2a6b96ea8d92b1587dd8cb3a35c7e3d51f0738ced0781c3aa3a5a3 \
-    --hash=sha256:4ce3ef14ebe8d9509188014d96af1c456a910d5b5cbf434a09fef7e024b3d0d5 \
-    --hash=sha256:4f0031eaa7b921db76decd73636ef3a12c942ed367d8c3841a0739412b260a54 \
-    --hash=sha256:602cfb1196dc692424c70b6507593a2b29aac0547c1be9a1d1365f0d964c353b \
-    --hash=sha256:6d1bd9c210f8b109b1762ec9fd36592fdd528485aadb3f5849b2740ef17e674e \
-    --hash=sha256:78baad24af0f033958cad29731e27363183e140962595def56423e626f4bee3e \
-    --hash=sha256:8d4df77958a622f9b5a4c96edb4b8c0034f8434032ab11077ec6c56ae9f384ba \
-    --hash=sha256:97e56155c6b737854e60a9ab1c598ff2533d57e7506d97af5481141671abf3ea \
-    --hash=sha256:9c4352800f14be5b4864016882cdba10755bd50805c95f728011bcb47a4afd59 \
-    --hash=sha256:a4d6a9668e45ad99d2f8ec70d5c8c04ef4f32f648ef39048d010b0689832ec6d \
-    --hash=sha256:a920b569dc6b3472513ba6ddea21f440d4b4c699494d2e972a1753cdc25df7b0 \
-    --hash=sha256:ae76c22bde5cbb6bfd211ec343ded2163bba7883c7bc77f6b756a1049436fbb9 \
-    --hash=sha256:b18fb2ae6c4bb63eebe5be6bd869ba2f14fd0259bda7d18a46b764d8fb86298a \
-    --hash=sha256:c04b6d9d20e9c13f43eee8ea87d44156b8505ca8a3c878773f68b4e4812a421e \
-    --hash=sha256:c88b3711d12905b74206227109272673edce0cb29f27e1385f33b0163c414bba \
-    --hash=sha256:dd15245c8b68fe2b6bd0f32c1556509d11bb33aec9b5d0866dd8e2ed3dba09c2 \
-    --hash=sha256:e0aaf6041986767a5e0ce663c7a2f0e9eaf21e6ff87a5f95cbf3675bfd4c41d2
+black==24.4.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:1bb9ca06e556a09f7f7177bc7cb604e5ed2d2df1e9119e4f7d2f1f7071c32e5d \
+    --hash=sha256:21f9407063ec71c5580b8ad975653c66508d6a9f57bd008bb8691d273705adcd \
+    --hash=sha256:4396ca365a4310beef84d446ca5016f671b10f07abdba3e4e4304218d2c71d33 \
+    --hash=sha256:44d99dfdf37a2a00a6f7a8dcbd19edf361d056ee51093b2445de7ca09adac965 \
+    --hash=sha256:5cd5b4f76056cecce3e69b0d4c228326d2595f506797f40b9233424e2524c070 \
+    --hash=sha256:64578cf99b6b46a6301bc28bdb89f9d6f9b592b1c5837818a177c98525dbe397 \
+    --hash=sha256:64e60a7edd71fd542a10a9643bf369bfd2644de95ec71e86790b063aa02ff745 \
+    --hash=sha256:652e55bb722ca026299eb74e53880ee2315b181dfdd44dca98e43448620ddec1 \
+    --hash=sha256:6644f97a7ef6f401a150cca551a1ff97e03c25d8519ee0bbc9b0058772882665 \
+    --hash=sha256:6ad001a9ddd9b8dfd1b434d566be39b1cd502802c8d38bbb1ba612afda2ef436 \
+    --hash=sha256:71d998b73c957444fb7c52096c3843875f4b6b47a54972598741fe9a7f737fcb \
+    --hash=sha256:74eb9b5420e26b42c00a3ff470dc0cd144b80a766128b1771d07643165e08d0e \
+    --hash=sha256:75a2d0b4f5eb81f7eebc31f788f9830a6ce10a68c91fbe0fade34fff7a2836e6 \
+    --hash=sha256:7852b05d02b5b9a8c893ab95863ef8986e4dda29af80bbbda94d7aee1abf8702 \
+    --hash=sha256:7f2966b9b2b3b7104fca9d75b2ee856fe3fdd7ed9e47c753a4bb1a675f2caab8 \
+    --hash=sha256:8e5537f456a22cf5cfcb2707803431d2feeb82ab3748ade280d6ccd0b40ed2e8 \
+    --hash=sha256:d4e71cdebdc8efeb6deaf5f2deb28325f8614d48426bed118ecc2dcaefb9ebf3 \
+    --hash=sha256:dae79397f367ac8d7adb6c779813328f6d690943f64b32983e896bcccd18cbad \
+    --hash=sha256:e3a3a092b8b756c643fe45f4624dbd5a389f770a4ac294cf4d0fce6af86addaf \
+    --hash=sha256:eb949f56a63c5e134dfdca12091e98ffb5fd446293ebae123d10fc1abad00b9e \
+    --hash=sha256:f07b69fda20578367eaebbd670ff8fc653ab181e1ff95d84497f9fa20e7d0641 \
+    --hash=sha256:f95cece33329dc4aa3b0e1a771c41075812e46cf3d6e3f1dfe3d91ff09826ed2
 click==8.1.7 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:ae74fb96c20a0277a1d615f1e4d73c8414f5a98db8b799a7931d1582f3390c28 \
     --hash=sha256:ca9853ad459e787e2192211578cc907e7594e294c7ccc834310722b41b9ca6de
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and platform_system == "Windows" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
 isort==5.13.2 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:48fdfcb9face5d58a4f6dde2e72a1fb8dcaf8ab26f95ab49fab84c2ddefb0109 \
     --hash=sha256:8ca5e72a8d85860d5a3fa69b8745237f2939afe12dbf656afbcb47fe72d947a6
-libcst==1.1.0 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:003e5e83a12eed23542c4ea20fdc8de830887cc03662432bb36f84f8c4841b81 \
-    --hash=sha256:0acbacb9a170455701845b7e940e2d7b9519db35a86768d86330a0b0deae1086 \
-    --hash=sha256:0bf69cbbab5016d938aac4d3ae70ba9ccb3f90363c588b3b97be434e6ba95403 \
-    --hash=sha256:2d37326bd6f379c64190a28947a586b949de3a76be00176b0732c8ee87d67ebe \
-    --hash=sha256:3a07ecfabbbb8b93209f952a365549e65e658831e9231649f4f4e4263cad24b1 \
-    --hash=sha256:3ebbb9732ae3cc4ae7a0e97890bed0a57c11d6df28790c2b9c869f7da653c7c7 \
-    --hash=sha256:4bc745d0c06420fe2644c28d6ddccea9474fb68a2135904043676deb4fa1e6bc \
-    --hash=sha256:5297a16e575be8173185e936b7765c89a3ca69d4ae217a4af161814a0f9745a7 \
-    --hash=sha256:5f1cd308a4c2f71d5e4eec6ee693819933a03b78edb2e4cc5e3ad1afd5fb3f07 \
-    --hash=sha256:63f75656fd733dc20354c46253fde3cf155613e37643c3eaf6f8818e95b7a3d1 \
-    --hash=sha256:73c086705ed34dbad16c62c9adca4249a556c1b022993d511da70ea85feaf669 \
-    --hash=sha256:75816647736f7e09c6120bdbf408456f99b248d6272277eed9a58cf50fb8bc7d \
-    --hash=sha256:78b7a38ec4c1c009ac39027d51558b52851fb9234669ba5ba62283185963a31c \
-    --hash=sha256:7ccaf53925f81118aeaadb068a911fac8abaff608817d7343da280616a5ca9c1 \
-    --hash=sha256:82d1271403509b0a4ee6ff7917c2d33b5a015f44d1e208abb1da06ba93b2a378 \
-    --hash=sha256:8ae11eb1ea55a16dc0cdc61b41b29ac347da70fec14cc4381248e141ee2fbe6c \
-    --hash=sha256:8afb6101b8b3c86c5f9cec6b90ab4da16c3c236fe7396f88e8b93542bb341f7c \
-    --hash=sha256:8c1f2da45f1c45634090fd8672c15e0159fdc46853336686959b2d093b6e10fa \
-    --hash=sha256:97fbc73c87e9040e148881041fd5ffa2a6ebf11f64b4ccb5b52e574b95df1a15 \
-    --hash=sha256:99fdc1929703fd9e7408aed2e03f58701c5280b05c8911753a8d8619f7dfdda5 \
-    --hash=sha256:9dffa1795c2804d183efb01c0f1efd20a7831db6a21a0311edf90b4100d67436 \
-    --hash=sha256:bca1841693941fdd18371824bb19a9702d5784cd347cb8231317dbdc7062c5bc \
-    --hash=sha256:c653d9121d6572d8b7f8abf20f88b0a41aab77ff5a6a36e5a0ec0f19af0072e8 \
-    --hash=sha256:c8f26250f87ca849a7303ed7a4fd6b2c7ac4dec16b7d7e68ca6a476d7c9bfcdb \
-    --hash=sha256:cc9b6ac36d7ec9db2f053014ea488086ca2ed9c322be104fbe2c71ca759da4bb \
-    --hash=sha256:d22d1abfe49aa60fc61fa867e10875a9b3024ba5a801112f4d7ba42d8d53242e \
-    --hash=sha256:d68c34e3038d3d1d6324eb47744cbf13f2c65e1214cf49db6ff2a6603c1cd838 \
-    --hash=sha256:e3d8cf974cfa2487b28f23f56c4bff90d550ef16505e58b0dca0493d5293784b \
-    --hash=sha256:f36f592e035ef84f312a12b75989dde6a5f6767fe99146cdae6a9ee9aff40dd0 \
-    --hash=sha256:f561c9a84eca18be92f4ad90aa9bd873111efbea995449301719a1a7805dbc5c \
-    --hash=sha256:fe41b33aa73635b1651f64633f429f7aa21f86d2db5748659a99d9b7b1ed2a90
+libcst==1.3.1 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:03b1df1ae02456f1d465fcd5ead1d0d454bb483caefd8c8e6bde515ffdb53d1b \
+    --hash=sha256:0a0d250fb6a2c1d158f30d25ba5e33e3ed3672d2700d480dd47beffd1431a008 \
+    --hash=sha256:16880711be03a1f5da7028fe791ba5b482a50d830225a70272dc332dfd927652 \
+    --hash=sha256:181372386c986e3de07d7a93f269214cd825adc714f1f9da8252b44f05e181c4 \
+    --hash=sha256:189bb28c19c5dd3c64583f969b72f7732dbdb1dee9eca3acc85099e4cef9148b \
+    --hash=sha256:2dbac1ac0a9d59ea7bbc3f87cdcca5bfe98835e31c668e95cb6f3d907ffc53fc \
+    --hash=sha256:4186076ce12141609ce950d61867b2a73ea199a7a9870dbafa76ad600e075b3c \
+    --hash=sha256:431badf0e544b79c0ac9682dbd291ff63ddbc3c3aca0d13d3cc7a10c3a9db8a2 \
+    --hash=sha256:4ad5741b251d901f3da1819ac539192230cc6f8f81aaf04eb4ec0009c1c97285 \
+    --hash=sha256:4ed52a1a2fe4d8603de51649db5e438317b8116ebb9fc09ec68703535fe6c1c8 \
+    --hash=sha256:701f5335e4fd566871497b9af1e871c98e1ef10c30b3b244f39343d709213401 \
+    --hash=sha256:7c6e709623b68ca9148e8ecbdc145f7b83befb26032e4bf6a8122500ba558b17 \
+    --hash=sha256:7cdb7e8a118b60e064a02f6cbfa4d328212a3a115d125244495190f405709d5f \
+    --hash=sha256:8c2020f7449270e3ff0bdc481ae244d812f2d9a8b7dbff0ea66b830f4b350f54 \
+    --hash=sha256:904c4cc5c801a5747e64b43e0accc87c67a4c804842d977ee215872c4cf8cf88 \
+    --hash=sha256:9e6bc95fa7dde79cde63a34a0412cd4a3d9fcc27be781a590f8c45c840c83658 \
+    --hash=sha256:a2d64d86dcd6c80a5dac2e243c5ed7a7a193242209ac33bad4b0639b24f6d131 \
+    --hash=sha256:b740dc0c3d1adbd91442fb878343d5a11e23a0e3ac5484be301fd8d148bcb085 \
+    --hash=sha256:be3bf9aaafebda6a21e241e819f0ab67e186e898c3562704e41241cf8738353a \
+    --hash=sha256:c0886a9963597367b227345f19b24931b3ed6a4703fff237760745f90f0e6a20 \
+    --hash=sha256:c12b7b01d8745f82dd86a82acd2a9f8e8e7d6c94ddcfda996896e83d1a8d5c42 \
+    --hash=sha256:db084f7bbf825c7bd5ed256290066d0336df6a7dc3a029c9870a64cd2298b87f \
+    --hash=sha256:de93193cba6d54f2a4419e94ba2de642b111f52e4fa01bb6e2c655914585f65b \
+    --hash=sha256:ede0f026a82b03b33a559ec566860085ece2e76d8f9bc21cb053eedf9cde8c79 \
+    --hash=sha256:f2995ca687118a9d3d41876f7270bc29305a2d402f4b8c81a3cff0aeee6d4c81
+markdown-it-py==3.0.0 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:355216845c60bd96232cd8d8c40e8f9765cc86f46880e43a8fd22dc1a1a8cab1 \
+    --hash=sha256:e3f60a94fa066dc52ec76661e37c851cb232d92f9886b15cb560aaada2df8feb
+mdurl==0.1.2 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:84008a41e51615a49fc9966191ff91509e3c40b939176e643fd50a5c2196b8f8 \
+    --hash=sha256:bb413d29f5eea38f31dd4754dd7377d4465116fb207585f97bf925588687c1ba
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
 pathspec==0.12.1 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:a0d503e138a4c123b27490a4f7beda6a01c6f288df0e4a8b79c7eb0dc7b4cc08 \
     --hash=sha256:a482d51503a1ab33b1c67a6c3813a26953dbdc71c31dacaef9a838c4e29f5712
-platformdirs==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:11c8f37bcca40db96d8144522d925583bdb7a31f7b0e37e3ed4318400a8e2380 \
-    --hash=sha256:906d548203468492d432bcb294d4bc2fff751bf84971fbb2c10918cc206ee420
-pre-commit-hooks==4.5.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:b779d5c44ede9b1fda48e2d96b08e9aa5b1d2fdb8903ca09f0dbaca22d529edb \
-    --hash=sha256:ffbe2af1c85ac9a7695866955680b4dee98822638b748a6f3debefad79748c8a
+platformdirs==4.2.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0614df2a2f37e1a662acbd8e2b25b92ccf8632929bc6d43467e17fe89c75e068 \
+    --hash=sha256:ef0cc731df711022c174543cb70a9b5bd22e5a9337c8624ef2c2ceb8ddad8768
+pre-commit-hooks==4.6.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:a69199e6a2d45ec59c1020a81ca1549abddc2afb798276d9a0d951752d6abbfe \
+    --hash=sha256:eb1f43ee67869cd41b4c59017fad4a0f9d4d61201d163f2135535aaf65035a2b
 pycln==2.4.0 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:1f3eefb7be18a9ee06c3bdd0ba2e91218cd39317e20130325f107e96eb84b9f6 \
     --hash=sha256:d1bf648df17077306100815d255d45430035b36f66bac635df04a323c61ba126
+pygments==2.17.2 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:b27c2826c47d0f3219f29554824c30c5e8945175d888647acd804ddd04af846c \
+    --hash=sha256:da46cec9fd2de5be3a8a784f434e4c4ab670b4ff54d605c4c2717e9d49c4c367
 pyyaml==6.0.1 ; python_version >= "3.9" and python_version < "4" \
     --hash=sha256:04ac92ad1925b2cff1db0cfebffb6ffc43457495c9b3c39d3fcae417d7125dc5 \
     --hash=sha256:062582fca9fabdd2c8b54a3ef1c978d786e0f6b3a1510e0ac93ef59e0ddae2bc \
     --hash=sha256:0d3304d8c0adc42be59c5f8a4d9e3d7379e6955ad754aa9d6ab7a398b59dd1df \
     --hash=sha256:1635fd110e8d85d55237ab316b5b011de701ea0f29d07611174a1b42f1444741 \
     --hash=sha256:184c5108a2aca3c5b3d3bf9395d50893a7ab82a38004c8f61c258d4428e80206 \
     --hash=sha256:18aeb1bf9a78867dc38b259769503436b7c72f7a1f1f4c93ff9a17de54319b27 \
@@ -112,14 +115,15 @@
     --hash=sha256:704219a11b772aea0d8ecd7058d0082713c3562b4e271b849ad7dc4a5c90c13c \
     --hash=sha256:7e07cbde391ba96ab58e532ff4803f79c4129397514e1413a7dc761ccd755735 \
     --hash=sha256:81e0b275a9ecc9c0c0c07b4b90ba548307583c125f54d5b6946cfee6360c733d \
     --hash=sha256:855fb52b0dc35af121542a76b9a84f8d1cd886ea97c84703eaa6d88e37a2ad28 \
     --hash=sha256:8d4e9c88387b0f5c7d5f281e55304de64cf7f9c0021a3525bd3b1c542da3b0e4 \
     --hash=sha256:9046c58c4395dff28dd494285c82ba00b546adfc7ef001486fbf0324bc174fba \
     --hash=sha256:9eb6caa9a297fc2c2fb8862bc5370d0303ddba53ba97e71f08023b6cd73d16a8 \
+    --hash=sha256:a08c6f0fe150303c1c6b71ebcd7213c2858041a7e01975da3a99aed1e7a378ef \
     --hash=sha256:a0cd17c15d3bb3fa06978b4e8958dcdc6e0174ccea823003a106c7d4d7899ac5 \
     --hash=sha256:afd7e57eddb1a54f0f1a974bc4391af8bcce0b444685d936840f125cf046d5bd \
     --hash=sha256:b1275ad35a5d18c62a7220633c913e1b42d44b46ee12554e5fd39c70a243d6a3 \
     --hash=sha256:b786eecbdf8499b9ca1d697215862083bd6d2a99965554781d0d8d1ad31e13a0 \
     --hash=sha256:ba336e390cd8e4d1739f42dfe9bb83a3cc2e80f567d8805e11b46f4a943f5515 \
     --hash=sha256:baa90d3f661d43131ca170712d903e6295d1f7a0f595074f151c0aed377c9b9c \
     --hash=sha256:bc1bf2925a1ecd43da378f4db9e4f799775d6367bdb94671027b73b393a7c42c \
@@ -133,14 +137,17 @@
     --hash=sha256:e7d73685e87afe9f3b36c799222440d6cf362062f78be1013661b00c5c6f678b \
     --hash=sha256:f003ed9ad21d6a4713f0a9b5a7a0a79e08dd0f221aff4525a2be4c346ee60aab \
     --hash=sha256:f22ac1c3cac4dbc50079e965eba2c1058622631e526bd9afd45fedd49ba781fa \
     --hash=sha256:faca3bdcf85b2fc05d06ff3fbc1f83e1391b3e724afa3feba7d13eeab355484c \
     --hash=sha256:fca0e3a251908a499833aa292323f32437106001d436eca0e6e7833256674585 \
     --hash=sha256:fd1592b3fdf65fff2ad0004b5e363300ef59ced41c2e6b3a99d4089fa8c5435d \
     --hash=sha256:fd66fc5d0da6d9815ba2cebeb4205f95818ff4b79c3ebe268e75d961704af52f
+rich==13.7.1 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222 \
+    --hash=sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432
 ruamel-yaml-clib==0.2.8 ; platform_python_implementation == "CPython" and python_version < "3.13" and python_version >= "3.9" \
     --hash=sha256:024cfe1fc7c7f4e1aff4a81e718109e13409767e4f871443cbff3dba3578203d \
     --hash=sha256:03d1162b6d1df1caa3a4bd27aa51ce17c9afc2046c31b0ad60a0a96ec22f8001 \
     --hash=sha256:07238db9cbdf8fc1e9de2489a4f68474e70dffcb32232db7c08fa61ca0c7c462 \
     --hash=sha256:09b055c05697b38ecacb7ac50bdab2240bfca1a0c4872b0fd309bb07dc9aa3a9 \
     --hash=sha256:1707814f0d9791df063f8c19bb51b0d1278b8e9a2353abbb676c2f685dee6afe \
     --hash=sha256:1758ce7d8e1a29d23de54a16ae867abd370f01b5a69e1a3ba75223eaa3ca1a1b \
@@ -184,31 +191,31 @@
     --hash=sha256:da09ad1c359a728e112d60116f626cc9f29730ff3e0e7db72b9a2dbc2e4beed5 \
     --hash=sha256:e2b4c44b60eadec492926a7270abb100ef9f72798e18743939bdbf037aab8c28 \
     --hash=sha256:e79e5db08739731b0ce4850bed599235d601701d5694c36570a99a0c5ca41a9d \
     --hash=sha256:ebc06178e8821efc9692ea7544aa5644217358490145629914d8020042c24aa1 \
     --hash=sha256:edaef1c1200c4b4cb914583150dcaa3bc30e592e907c01117c08b13a07255ec2 \
     --hash=sha256:f481f16baec5290e45aebdc2a5168ebc6d35189ae6fea7a58787613a25f6e875 \
     --hash=sha256:fff3573c2db359f091e1589c3d7c5fc2f86f5bdb6f24252c2d8e539d4e45f412
-ruamel-yaml==0.18.5 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:61917e3a35a569c1133a8f772e1226961bf5a1198bea7e23f06a0841dea1ab0e \
-    --hash=sha256:a013ac02f99a69cdd6277d9664689eb1acba07069f912823177c5eced21a6ada
+ruamel-yaml==0.18.6 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:57b53ba33def16c4f3d807c0ccbc00f8a6081827e81ba2491691b76882d0c636 \
+    --hash=sha256:8b27e6a217e786c6fbe5634d8f3f11bc63e0f80f6a5890f28863d9c45aac311b
+shellingham==1.5.4 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:7ecfff8f2fd72616f7481040475a65b2bf8af90a56c89140852d1120324e8686 \
+    --hash=sha256:8dbca0739d487e5bd35ab3ca4b36e11c4078f3a234bfce294b0a0291363404de
 sort-all==1.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:1eb6a91cc61f36bd48d697f687377c6eb67b4ef98e2850fc65130502bae945d8 \
     --hash=sha256:ccc0fc7191a486ff826cb4d21c2b67d93f9d9cb5eb72e8d572d017d50d4eca88
 tokenize-rt==5.2.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:9fe80f8a5c1edad2d3ede0f37481cc0cc1538a2f442c9c2f9e4feacd2792d054 \
     --hash=sha256:b79d41a65cfec71285433511b50271b05da3584a1da144a0752e9c621a285289
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-tomlkit==0.12.3 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:75baf5012d06501f07bee5bf8e801b9f343e7aac5a92581f20f80ce632e6b5a4 \
-    --hash=sha256:b0a645a9156dc7cb5d3a1f0d4bab66db287fcb8e0430bdd4664a095ea16414ba
-typer==0.9.0 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:50922fd79aea2f4751a8e0408ff10d2662bd0c8bbfa84755a699f3bada2978b2 \
-    --hash=sha256:5d96d986a21493606a358cae4461bd8cdf83cbf33a5aa950ae629ca3b51467ee
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
-typing-inspect==0.9.0 ; python_version >= "3.9" and python_version < "4" \
-    --hash=sha256:9ee6fc59062311ef8547596ab6b955e1b8aa46242d854bfc78f4f6b0eff35f9f \
-    --hash=sha256:b23fc42ff6f6ef6954e4852c1fb512cdd18dbea03134f91f856a95ccc9461f78
+tomlkit==0.12.4 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:5cd82d48a3dd89dee1f9d64420aa20ae65cfbd00668d6f094d7578a78efbb77b \
+    --hash=sha256:7ca1cfc12232806517a8515047ba66a19369e71edf2439d0f5824f91032b6cc3
+typer==0.12.3 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:070d7ca53f785acbccba8e7d28b08dcd88f79f1fbda035ade0aecec71ca5c914 \
+    --hash=sha256:49e73131481d804288ef62598d97a1ceef3058905aa536a1134f90891ba35482
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/tests.txt` & `alluka-0.1.5/piped/python/base-requirements/tests.txt`

 * *Files 20% similar despite different names*

```diff
@@ -3,90 +3,90 @@
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/tests.in --output-file python/base-requirements/tests.txt --min-python-version 3.9
 #
 colorama==0.4.6 ; python_version >= "3.9" and python_version < "4.0" and sys_platform == "win32" \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
-coverage[toml]==7.3.4 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:020d56d2da5bc22a0e00a5b0d54597ee91ad72446fa4cf1b97c35022f6b6dbf0 \
-    --hash=sha256:11ab62d0ce5d9324915726f611f511a761efcca970bd49d876cf831b4de65be5 \
-    --hash=sha256:183c16173a70caf92e2dfcfe7c7a576de6fa9edc4119b8e13f91db7ca33a7923 \
-    --hash=sha256:27ee94f088397d1feea3cb524e4313ff0410ead7d968029ecc4bc5a7e1d34fbf \
-    --hash=sha256:3024ec1b3a221bd10b5d87337d0373c2bcaf7afd86d42081afe39b3e1820323b \
-    --hash=sha256:309ed6a559bc942b7cc721f2976326efbfe81fc2b8f601c722bff927328507dc \
-    --hash=sha256:33e63c578f4acce1b6cd292a66bc30164495010f1091d4b7529d014845cd9bee \
-    --hash=sha256:36797b3625d1da885b369bdaaa3b0d9fb8865caed3c2b8230afaa6005434aa2f \
-    --hash=sha256:36d75ef2acab74dc948d0b537ef021306796da551e8ac8b467810911000af66a \
-    --hash=sha256:38d0b307c4d99a7aca4e00cad4311b7c51b7ac38fb7dea2abe0d182dd4008e05 \
-    --hash=sha256:3d892a19ae24b9801771a5a989fb3e850bd1ad2e2b6e83e949c65e8f37bc67a1 \
-    --hash=sha256:3f477fb8a56e0c603587b8278d9dbd32e54bcc2922d62405f65574bd76eba78a \
-    --hash=sha256:47ee56c2cd445ea35a8cc3ad5c8134cb9bece3a5cb50bb8265514208d0a65928 \
-    --hash=sha256:4a4184dcbe4f98d86470273e758f1d24191ca095412e4335ff27b417291f5964 \
-    --hash=sha256:5214362abf26e254d749fc0c18af4c57b532a4bfde1a057565616dd3b8d7cc94 \
-    --hash=sha256:607b6c6b35aa49defaebf4526729bd5238bc36fe3ef1a417d9839e1d96ee1e4c \
-    --hash=sha256:610afaf929dc0e09a5eef6981edb6a57a46b7eceff151947b836d869d6d567c1 \
-    --hash=sha256:6879fe41c60080aa4bb59703a526c54e0412b77e649a0d06a61782ecf0853ee1 \
-    --hash=sha256:74397a1263275bea9d736572d4cf338efaade2de9ff759f9c26bcdceb383bb49 \
-    --hash=sha256:758ebaf74578b73f727acc4e8ab4b16ab6f22a5ffd7dd254e5946aba42a4ce76 \
-    --hash=sha256:782693b817218169bfeb9b9ba7f4a9f242764e180ac9589b45112571f32a0ba6 \
-    --hash=sha256:7c4277ddaad9293454da19121c59f2d850f16bcb27f71f89a5c4836906eb35ef \
-    --hash=sha256:85072e99474d894e5df582faec04abe137b28972d5e466999bc64fc37f564a03 \
-    --hash=sha256:8a9c5bc5db3eb4cd55ecb8397d8e9b70247904f8eca718cc53c12dcc98e59fc8 \
-    --hash=sha256:8ce03e25e18dd9bf44723e83bc202114817f3367789052dc9e5b5c79f40cf59d \
-    --hash=sha256:93698ac0995516ccdca55342599a1463ed2e2d8942316da31686d4d614597ef9 \
-    --hash=sha256:997aa14b3e014339d8101b9886063c5d06238848905d9ad6c6eabe533440a9a7 \
-    --hash=sha256:9ac17b94ab4ca66cf803f2b22d47e392f0977f9da838bf71d1f0db6c32893cb9 \
-    --hash=sha256:a02ac7c51819702b384fea5ee033a7c202f732a2a2f1fe6c41e3d4019828c8d3 \
-    --hash=sha256:a1c3e9d2bbd6f3f79cfecd6f20854f4dc0c6e0ec317df2b265266d0dc06535f1 \
-    --hash=sha256:a877810ef918d0d345b783fc569608804f3ed2507bf32f14f652e4eaf5d8f8d0 \
-    --hash=sha256:a8e258dcc335055ab59fe79f1dec217d9fb0cdace103d6b5c6df6b75915e7959 \
-    --hash=sha256:aefbb29dc56317a4fcb2f3857d5bce9b881038ed7e5aa5d3bcab25bd23f57328 \
-    --hash=sha256:aff2bd3d585969cc4486bfc69655e862028b689404563e6b549e6a8244f226df \
-    --hash=sha256:b1e0f25ae99cf247abfb3f0fac7ae25739e4cd96bf1afa3537827c576b4847e5 \
-    --hash=sha256:b710869a15b8caf02e31d16487a931dbe78335462a122c8603bb9bd401ff6fb2 \
-    --hash=sha256:bfed0ec4b419fbc807dec417c401499ea869436910e1ca524cfb4f81cf3f60e7 \
-    --hash=sha256:c15fdfb141fcf6a900e68bfa35689e1256a670db32b96e7a931cab4a0e1600e5 \
-    --hash=sha256:c6a23ae9348a7a92e7f750f9b7e828448e428e99c24616dec93a0720342f241d \
-    --hash=sha256:c75738ce13d257efbb6633a049fb2ed8e87e2e6c2e906c52d1093a4d08d67c6b \
-    --hash=sha256:d1d0ce6c6947a3a4aa5479bebceff2c807b9f3b529b637e2b33dea4468d75fc7 \
-    --hash=sha256:d5b14abde6f8d969e6b9dd8c7a013d9a2b52af1235fe7bebef25ad5c8f47fa18 \
-    --hash=sha256:d6ed790728fb71e6b8247bd28e77e99d0c276dff952389b5388169b8ca7b1c28 \
-    --hash=sha256:e0d84099ea7cba9ff467f9c6f747e3fc3906e2aadac1ce7b41add72e8d0a3712 \
-    --hash=sha256:e4353923f38d752ecfbd3f1f20bf7a3546993ae5ecd7c07fd2f25d40b4e54571 \
-    --hash=sha256:e91029d7f151d8bf5ab7d8bfe2c3dbefd239759d642b211a677bc0709c9fdb96 \
-    --hash=sha256:ea473c37872f0159294f7073f3fa72f68b03a129799f3533b2bb44d5e9fa4f82 \
-    --hash=sha256:f154bd866318185ef5865ace5be3ac047b6d1cc0aeecf53bf83fe846f4384d5d \
-    --hash=sha256:f97ff5a9fc2ca47f3383482858dd2cb8ddbf7514427eecf5aa5f7992d0571429 \
-    --hash=sha256:f99b7d3f7a7adfa3d11e3a48d1a91bb65739555dd6a0d3fa68aa5852d962e5b1 \
-    --hash=sha256:fb220b3596358a86361139edce40d97da7458412d412e1e10c8e1970ee8c09ab \
-    --hash=sha256:fd2f8a641f8f193968afdc8fd1697e602e199931012b574194052d132a79be13
-exceptiongroup==1.2.0 ; python_version >= "3.9" and python_version < "3.11" \
-    --hash=sha256:4bfd3996ac73b41e9b9628b04e079f193850720ea5945fc96a08633c66912f14 \
-    --hash=sha256:91f5c769735f051a4290d52edd0858999b57e5876e9f85937691bd4c9fa3ed68
+coverage[toml]==7.4.4 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:00838a35b882694afda09f85e469c96367daa3f3f2b097d846a7216993d37f4c \
+    --hash=sha256:0513b9508b93da4e1716744ef6ebc507aff016ba115ffe8ecff744d1322a7b63 \
+    --hash=sha256:09c3255458533cb76ef55da8cc49ffab9e33f083739c8bd4f58e79fecfe288f7 \
+    --hash=sha256:09ef9199ed6653989ebbcaacc9b62b514bb63ea2f90256e71fea3ed74bd8ff6f \
+    --hash=sha256:09fa497a8ab37784fbb20ab699c246053ac294d13fc7eb40ec007a5043ec91f8 \
+    --hash=sha256:0f9f50e7ef2a71e2fae92774c99170eb8304e3fdf9c8c3c7ae9bab3e7229c5cf \
+    --hash=sha256:137eb07173141545e07403cca94ab625cc1cc6bc4c1e97b6e3846270e7e1fea0 \
+    --hash=sha256:1f384c3cc76aeedce208643697fb3e8437604b512255de6d18dae3f27655a384 \
+    --hash=sha256:201bef2eea65e0e9c56343115ba3814e896afe6d36ffd37bab783261db430f76 \
+    --hash=sha256:38dd60d7bf242c4ed5b38e094baf6401faa114fc09e9e6632374388a404f98e7 \
+    --hash=sha256:3b799445b9f7ee8bf299cfaed6f5b226c0037b74886a4e11515e569b36fe310d \
+    --hash=sha256:3ea79bb50e805cd6ac058dfa3b5c8f6c040cb87fe83de10845857f5535d1db70 \
+    --hash=sha256:40209e141059b9370a2657c9b15607815359ab3ef9918f0196b6fccce8d3230f \
+    --hash=sha256:41c9c5f3de16b903b610d09650e5e27adbfa7f500302718c9ffd1c12cf9d6818 \
+    --hash=sha256:54eb8d1bf7cacfbf2a3186019bcf01d11c666bd495ed18717162f7eb1e9dd00b \
+    --hash=sha256:598825b51b81c808cb6f078dcb972f96af96b078faa47af7dfcdf282835baa8d \
+    --hash=sha256:5fc1de20b2d4a061b3df27ab9b7c7111e9a710f10dc2b84d33a4ab25065994ec \
+    --hash=sha256:623512f8ba53c422fcfb2ce68362c97945095b864cda94a92edbaf5994201083 \
+    --hash=sha256:690db6517f09336559dc0b5f55342df62370a48f5469fabf502db2c6d1cffcd2 \
+    --hash=sha256:69eb372f7e2ece89f14751fbcbe470295d73ed41ecd37ca36ed2eb47512a6ab9 \
+    --hash=sha256:73bfb9c09951125d06ee473bed216e2c3742f530fc5acc1383883125de76d9cd \
+    --hash=sha256:742a76a12aa45b44d236815d282b03cfb1de3b4323f3e4ec933acfae08e54ade \
+    --hash=sha256:7c95949560050d04d46b919301826525597f07b33beba6187d04fa64d47ac82e \
+    --hash=sha256:8130a2aa2acb8788e0b56938786c33c7c98562697bf9f4c7d6e8e5e3a0501e4a \
+    --hash=sha256:8a2b2b78c78293782fd3767d53e6474582f62443d0504b1554370bde86cc8227 \
+    --hash=sha256:8ce1415194b4a6bd0cdcc3a1dfbf58b63f910dcb7330fe15bdff542c56949f87 \
+    --hash=sha256:9ca28a302acb19b6af89e90f33ee3e1906961f94b54ea37de6737b7ca9d8827c \
+    --hash=sha256:a4cdc86d54b5da0df6d3d3a2f0b710949286094c3a6700c21e9015932b81447e \
+    --hash=sha256:aa5b1c1bfc28384f1f53b69a023d789f72b2e0ab1b3787aae16992a7ca21056c \
+    --hash=sha256:aadacf9a2f407a4688d700e4ebab33a7e2e408f2ca04dbf4aef17585389eff3e \
+    --hash=sha256:ae71e7ddb7a413dd60052e90528f2f65270aad4b509563af6d03d53e979feafd \
+    --hash=sha256:b14706df8b2de49869ae03a5ccbc211f4041750cd4a66f698df89d44f4bd30ec \
+    --hash=sha256:b1a93009cb80730c9bca5d6d4665494b725b6e8e157c1cb7f2db5b4b122ea562 \
+    --hash=sha256:b2991665420a803495e0b90a79233c1433d6ed77ef282e8e152a324bbbc5e0c8 \
+    --hash=sha256:b2c5edc4ac10a7ef6605a966c58929ec6c1bd0917fb8c15cb3363f65aa40e677 \
+    --hash=sha256:b4d33f418f46362995f1e9d4f3a35a1b6322cb959c31d88ae56b0298e1c22357 \
+    --hash=sha256:b91cbc4b195444e7e258ba27ac33769c41b94967919f10037e6355e998af255c \
+    --hash=sha256:c74880fc64d4958159fbd537a091d2a585448a8f8508bf248d72112723974cbd \
+    --hash=sha256:c901df83d097649e257e803be22592aedfd5182f07b3cc87d640bbb9afd50f49 \
+    --hash=sha256:cac99918c7bba15302a2d81f0312c08054a3359eaa1929c7e4b26ebe41e9b286 \
+    --hash=sha256:cc4f1358cb0c78edef3ed237ef2c86056206bb8d9140e73b6b89fbcfcbdd40e1 \
+    --hash=sha256:ccd341521be3d1b3daeb41960ae94a5e87abe2f46f17224ba5d6f2b8398016cf \
+    --hash=sha256:ce4b94265ca988c3f8e479e741693d143026632672e3ff924f25fab50518dd51 \
+    --hash=sha256:cf271892d13e43bc2b51e6908ec9a6a5094a4df1d8af0bfc360088ee6c684409 \
+    --hash=sha256:d5ae728ff3b5401cc320d792866987e7e7e880e6ebd24433b70a33b643bb0384 \
+    --hash=sha256:d71eec7d83298f1af3326ce0ff1d0ea83c7cb98f72b577097f9083b20bdaf05e \
+    --hash=sha256:d898fe162d26929b5960e4e138651f7427048e72c853607f2b200909794ed978 \
+    --hash=sha256:d89d7b2974cae412400e88f35d86af72208e1ede1a541954af5d944a8ba46c57 \
+    --hash=sha256:dfa8fe35a0bb90382837b238fff375de15f0dcdb9ae68ff85f7a63649c98527e \
+    --hash=sha256:e0be5efd5127542ef31f165de269f77560d6cdef525fffa446de6f7e9186cfb2 \
+    --hash=sha256:fdfafb32984684eb03c2d83e1e51f64f0906b11e64482df3c5db936ce3839d48 \
+    --hash=sha256:ff7687ca3d7028d8a5f0ebae95a6e4827c5616b31a4ee1192bdfde697db110d4
+exceptiongroup==1.2.1 ; python_version >= "3.9" and python_version < "3.11" \
+    --hash=sha256:5258b9ed329c5bbdd31a309f53cbfb0b155341807f6ff7606a1e801a891b29ad \
+    --hash=sha256:a4785e48b045528f5bfe627b6ad554ff32def154f42372786903b7abcfe1aa16
 iniconfig==2.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:2d91e135bf72d31a410b17c16da610a82cb55f6b0477d1a902134b24a455b8b3 \
     --hash=sha256:b6a85871a79d2e3b22d2d1b94ac2824226a63c6b741c88f7ae975f18b6778374
-packaging==23.2 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:048fb0e9405036518eaaf48a55953c750c11e1a1b68e0dd1a9d62ed0c092cfc5 \
-    --hash=sha256:8c491190033a9af7e1d931d0b5dacc2ef47509b34dd0de67ed209b5203fc88c7
-pluggy==1.3.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:cf61ae8f126ac6f7c451172cf30e3e43d3ca77615509771b3a984a0730651e12 \
-    --hash=sha256:d89c696a773f8bd377d18e5ecda92b7a3793cbe66c87060a6fb58c7b6e1061f7
-pytest-cov==4.1.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:3904b13dfbfec47f003b8e77fd5b589cd11904a21ddf1ab38a64f204d6a10ef6 \
-    --hash=sha256:6ba70b9e97e69fcc3fb45bfeab2d0a138fb65c4d0d6a41ef33983ad114be8c3a
-pytest-sugar==0.9.7 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:8cb5a4e5f8bbcd834622b0235db9e50432f4cbd71fef55b467fe44e43701e062 \
-    --hash=sha256:f1e74c1abfa55f7241cf7088032b6e378566f16b938f3f08905e2cf4494edd46
-pytest-timeout==2.2.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:3b0b95dabf3cb50bac9ef5ca912fa0cfc286526af17afc806824df20c2f72c90 \
-    --hash=sha256:bde531e096466f49398a59f2dde76fa78429a09a12411466f88a07213e220de2
-pytest==7.4.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:0d009c083ea859a71b76adf7c1d502e4bc170b80a8ef002da5806527b9591fac \
-    --hash=sha256:d989d136982de4e3b29dabcc838ad581c64e8ed52c11fbe86ddebd9da0818cd5
+packaging==24.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2ddfb553fdf02fb784c234c7ba6ccc288296ceabec964ad2eae3777778130bc5 \
+    --hash=sha256:eb82c5e3e56209074766e6885bb04b8c38a0c015d0a30036ebe7ece34c9989e9
+pluggy==1.5.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2cffa88e94fdc978c4c574f15f9e59b7f4201d439195c3715ca9e2486f1d0cf1 \
+    --hash=sha256:44e1ad92c8ca002de6377e165f3e0f1be63266ab4d554740532335b9d75ea669
+pytest-cov==5.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:4f0764a1219df53214206bf1feea4633c3b558a2925c8b59f144f682861ce652 \
+    --hash=sha256:5837b58e9f6ebd335b0f8060eecce69b662415b16dc503883a02f45dfeb14857
+pytest-sugar==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6422e83258f5b0c04ce7c632176c7732cab5fdb909cb39cca5c9139f81276c0a \
+    --hash=sha256:70ebcd8fc5795dc457ff8b69d266a4e2e8a74ae0c3edc749381c64b5246c8dfd
+pytest-timeout==2.3.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:12397729125c6ecbdaca01035b9e5239d4db97352320af155b3f5de1ba5165d9 \
+    --hash=sha256:68188cb703edfc6a18fad98dc25a3c61e9f24d644b0b70f33af545219fc7813e
+pytest==8.1.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:2a8386cfc11fa9d2c50ee7b2a57e7d898ef90470a7a34c4b949ff59662bb78b7 \
+    --hash=sha256:ac978141a75948948817d360297b7aae0fcb9d6ff6bc9ec6d514b85d5a65c044
 termcolor==2.4.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:9297c0df9c99445c2412e832e882a7884038a25617c60cea2ad69488d4040d63 \
     --hash=sha256:aab9e56047c8ac41ed798fa36d892a37aca6b3e9159f3e0c24bc64a9b3ac7b7a
 tomli==2.0.1 ; python_version >= "3.9" and python_full_version <= "3.11.0a6" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
```

### Comparing `alluka-0.1.4/piped/python/base-requirements/type-checking.txt` & `alluka-0.1.5/piped/python/base-requirements/type-checking.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,50 +3,50 @@
 # To update, run:
 #
 #    pip-compile-cross-platform python/base-requirements/type-checking.in --output-file python/base-requirements/type-checking.txt --min-python-version 3.9
 #
 mypy-extensions==1.0.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:4392f6c0eb8a5668a69e23d168ffa70f0be9ccfd32b5cc2d26a34ae5b844552d \
     --hash=sha256:75dbf8955dc00442a438fc4d0666508a9a97b6bd41aa2f0ffe9d2f2725af0782
-mypy==1.8.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:028cf9f2cae89e202d7b6593cd98db6759379f17a319b5faf4f9978d7084cdc6 \
-    --hash=sha256:2afecd6354bbfb6e0160f4e4ad9ba6e4e003b767dd80d85516e71f2e955ab50d \
-    --hash=sha256:2b5b6c721bd4aabaadead3a5e6fa85c11c6c795e0c81a7215776ef8afc66de02 \
-    --hash=sha256:42419861b43e6962a649068a61f4a4839205a3ef525b858377a960b9e2de6e0d \
-    --hash=sha256:42c6680d256ab35637ef88891c6bd02514ccb7e1122133ac96055ff458f93fc3 \
-    --hash=sha256:485a8942f671120f76afffff70f259e1cd0f0cfe08f81c05d8816d958d4577d3 \
-    --hash=sha256:4c886c6cce2d070bd7df4ec4a05a13ee20c0aa60cb587e8d1265b6c03cf91da3 \
-    --hash=sha256:4e6d97288757e1ddba10dd9549ac27982e3e74a49d8d0179fc14d4365c7add66 \
-    --hash=sha256:4ef4be7baf08a203170f29e89d79064463b7fc7a0908b9d0d5114e8009c3a259 \
-    --hash=sha256:51720c776d148bad2372ca21ca29256ed483aa9a4cdefefcef49006dff2a6835 \
-    --hash=sha256:52825b01f5c4c1c4eb0db253ec09c7aa17e1a7304d247c48b6f3599ef40db8bd \
-    --hash=sha256:538fd81bb5e430cc1381a443971c0475582ff9f434c16cd46d2c66763ce85d9d \
-    --hash=sha256:5c1538c38584029352878a0466f03a8ee7547d7bd9f641f57a0f3017a7c905b8 \
-    --hash=sha256:6ff8b244d7085a0b425b56d327b480c3b29cafbd2eff27316a004f9a7391ae07 \
-    --hash=sha256:7178def594014aa6c35a8ff411cf37d682f428b3b5617ca79029d8ae72f5402b \
-    --hash=sha256:720a5ca70e136b675af3af63db533c1c8c9181314d207568bbe79051f122669e \
-    --hash=sha256:7f1478736fcebb90f97e40aff11a5f253af890c845ee0c850fe80aa060a267c6 \
-    --hash=sha256:855fe27b80375e5c5878492f0729540db47b186509c98dae341254c8f45f42ae \
-    --hash=sha256:8963b83d53ee733a6e4196954502b33567ad07dfd74851f32be18eb932fb1cb9 \
-    --hash=sha256:9261ed810972061388918c83c3f5cd46079d875026ba97380f3e3978a72f503d \
-    --hash=sha256:99b00bc72855812a60d253420d8a2eae839b0afa4938f09f4d2aa9bb4654263a \
-    --hash=sha256:ab3c84fa13c04aeeeabb2a7f67a25ef5d77ac9d6486ff33ded762ef353aa5592 \
-    --hash=sha256:afe3fe972c645b4632c563d3f3eff1cdca2fa058f730df2b93a35e3b0c538218 \
-    --hash=sha256:d19c413b3c07cbecf1f991e2221746b0d2a9410b59cb3f4fb9557f0365a1a817 \
-    --hash=sha256:df9824ac11deaf007443e7ed2a4a26bebff98d2bc43c6da21b2b64185da011c4 \
-    --hash=sha256:e46f44b54ebddbeedbd3d5b289a893219065ef805d95094d16a0af6630f5d410 \
-    --hash=sha256:f5ac9a4eeb1ec0f1ccdc6f326bcdb464de5f80eb07fb38b5ddd7b0de6bc61e55
+mypy==1.9.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:0235391f1c6f6ce487b23b9dbd1327b4ec33bb93934aa986efe8a9563d9349e6 \
+    --hash=sha256:190da1ee69b427d7efa8aa0d5e5ccd67a4fb04038c380237a0d96829cb157913 \
+    --hash=sha256:2418488264eb41f69cc64a69a745fad4a8f86649af4b1041a4c64ee61fc61129 \
+    --hash=sha256:3a3c007ff3ee90f69cf0a15cbcdf0995749569b86b6d2f327af01fd1b8aee9dc \
+    --hash=sha256:3cc5da0127e6a478cddd906068496a97a7618a21ce9b54bde5bf7e539c7af974 \
+    --hash=sha256:48533cdd345c3c2e5ef48ba3b0d3880b257b423e7995dada04248725c6f77374 \
+    --hash=sha256:49c87c15aed320de9b438ae7b00c1ac91cd393c1b854c2ce538e2a72d55df150 \
+    --hash=sha256:4d3dbd346cfec7cb98e6cbb6e0f3c23618af826316188d587d1c1bc34f0ede03 \
+    --hash=sha256:571741dc4194b4f82d344b15e8837e8c5fcc462d66d076748142327626a1b6e9 \
+    --hash=sha256:587ce887f75dd9700252a3abbc9c97bbe165a4a630597845c61279cf32dfbf02 \
+    --hash=sha256:5d741d3fc7c4da608764073089e5f58ef6352bedc223ff58f2f038c2c4698a89 \
+    --hash=sha256:5e6061f44f2313b94f920e91b204ec600982961e07a17e0f6cd83371cb23f5c2 \
+    --hash=sha256:61758fabd58ce4b0720ae1e2fea5cfd4431591d6d590b197775329264f86311d \
+    --hash=sha256:653265f9a2784db65bfca694d1edd23093ce49740b2244cde583aeb134c008f3 \
+    --hash=sha256:68edad3dc7d70f2f17ae4c6c1b9471a56138ca22722487eebacfd1eb5321d612 \
+    --hash=sha256:81a10926e5473c5fc3da8abb04119a1f5811a236dc3a38d92015cb1e6ba4cb9e \
+    --hash=sha256:85ca5fcc24f0b4aeedc1d02f93707bccc04733f21d41c88334c5482219b1ccb3 \
+    --hash=sha256:a260627a570559181a9ea5de61ac6297aa5af202f06fd7ab093ce74e7181e43e \
+    --hash=sha256:aceb1db093b04db5cd390821464504111b8ec3e351eb85afd1433490163d60cd \
+    --hash=sha256:b685154e22e4e9199fc95f298661deea28aaede5ae16ccc8cbb1045e716b3e04 \
+    --hash=sha256:d357423fa57a489e8c47b7c85dfb96698caba13d66e086b412298a1a0ea3b0ed \
+    --hash=sha256:d4d5ddc13421ba3e2e082a6c2d74c2ddb3979c39b582dacd53dd5d9431237185 \
+    --hash=sha256:e49499be624dead83927e70c756970a0bc8240e9f769389cdf5714b0784ca6bf \
+    --hash=sha256:e54396d70be04b34f31d2edf3362c1edd023246c82f1730bbf8768c28db5361b \
+    --hash=sha256:f88566144752999351725ac623471661c9d1cd8caa0134ff98cceeea181789f4 \
+    --hash=sha256:f8a67616990062232ee4c3952f41c779afac41405806042a8126fe96e098419f \
+    --hash=sha256:fe28657de3bfec596bbeef01cb219833ad9d38dd5393fc649f4b366840baefe6
 nodeenv==1.8.0 ; python_version >= "3.9" and python_version < "4.0" \
     --hash=sha256:d51e0c37e64fbf47d017feac3145cdbb58836d7eee8c6f6d3b6880c5456227d2 \
     --hash=sha256:df865724bb3c3adc86b3876fa209771517b0cfe596beff01a92700e0e8be4cec
-pyright==1.1.343 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:75a0d24e8227328198bdfa1f4904ce66b78c2bacf49c269d9e6e3b174b026225 \
-    --hash=sha256:871e122d74003e8e5fddb17867220b06ee892de61fa967ca7ca031acdc176738
-setuptools==69.0.3 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:385eb4edd9c9d5c17540511303e39a147ce2fc04bc55289c322b9e5904fe2c05 \
-    --hash=sha256:be1af57fc409f93647f2e8e4573a142ed38724b8cdd389706a867bb4efcf1e78
+pyright==1.1.359 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:5582777be7eab73512277ac7da7b41e15bc0737f488629cb9babd96e0769be61 \
+    --hash=sha256:f0eab50f3dafce8a7302caeafd6a733f39901a2bf5170bb23d77fd607c8a8dbc
+setuptools==69.5.1 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:6c1fccdac05a97e598fb0ae3bbed5904ccb317337a51139dcd51453611bbb987 \
+    --hash=sha256:c636ac361bc47580504644275c9ad802c50415c7522212252c033bd15f301f32
 tomli==2.0.1 ; python_version >= "3.9" and python_version < "3.11" \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
-typing-extensions==4.9.0 ; python_version >= "3.9" and python_version < "4.0" \
-    --hash=sha256:23478f88c37f27d76ac8aee6c905017a143b0b1b886c3c9f66bc2fd94f9f5783 \
-    --hash=sha256:af72aea155e91adfc61c3ae9e0e342dbc0cba726d6cba4b6c72c1f34e47291cd
+typing-extensions==4.11.0 ; python_version >= "3.9" and python_version < "4.0" \
+    --hash=sha256:83f085bd5ca59c80295fc2a82ab5dac679cbe02b9f33f7d83af68e241bea51b0 \
+    --hash=sha256:c1f94d72897edaf4ce775bb7558d5b79d8126906a14ea5ed1635921406c0387a
```

### Comparing `alluka-0.1.4/piped/python/noxfile.py` & `alluka-0.1.5/piped/python/noxfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -266,14 +266,15 @@
         output: piped_shared.ConfigT = dict(self.defaults)
         output.update(**config)
         return output
 
 
 _ACTIONS: dict[str, _Action] = {
     "clippy": _Action(),
+    "docker-publish": _Action(defaults={"DOCKER_DEPLOY_CONTEXT": "."}),
     "freeze-for-pr": _Action(defaults={"EXTEND_FILTERS": [], "FILTERS": _resync_filter}),
     "lint": _Action(),
     "pr-docs": _Action(),
     "publish": _Action(),
     "py-test": _Action(
         required=["PYTHON_VERSIONS"],
         defaults={"CODECLIMATE_TOKEN": "", "OSES": "[ubuntu-latest, macos-latest, windows-latest]"},
@@ -428,15 +429,15 @@
 
 
 @_filtered_session(reuse_venv=True)
 def flake8(session: nox.Session) -> None:
     """Run this project's modules against the pre-defined flake8 linters."""
     _install_deps(session, names=["flake8"])
     session.log("Running flake8")
-    session.run("pflake8", *_config.top_level_targets, log=False)
+    session.run("flake8", *_config.top_level_targets, log=False)
 
 
 @_filtered_session(reuse_venv=True, name="slot-check")
 def slot_check(session: nox.Session) -> None:
     """Check this project's slotted classes for common mistakes."""
     # TODO: don't require installing .?
     # https://github.com/pypa/pip/issues/10362
```

### Comparing `alluka-0.1.4/piped/python/noxfile.template.py` & `alluka-0.1.5/piped/python/noxfile.template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/piped/python/piped_shared/__init__.py` & `alluka-0.1.5/piped/python/piped_shared/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/pyproject.toml` & `alluka-0.1.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.3,<4,!=3.7"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "alluka"
-version = "0.1.4"
+version = "0.1.5"
 readme = "README.md"
 requires-python = ">=3.9.0,<3.13"
 license = {file = "LICENSE"}
 authors = [ {name = "Faster Speeding", email="lucina@lmbyrne.dev"} ]
 keywords = ["DI", "injection"]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -96,20 +96,22 @@
     "TRY003",  # Avoid specifying long messages outside the exception class (this hits way too many std exceptions rn)
     "T101",    # TO-DO comment detection (T102 is FIX-ME and T103 is XXX).
     "W503",    # line break before binary operator.
     "W504",    # line break before binary operator (again, I guess).
     "S101",    # Use of assert detected. The enclosed code will be removed when compiling to optimised byte code.
     "E203",    # whitespace before ':'
     "E231",    # missing whitespace after ','
+    "E701",    # Incompatible with black: E701 multiple statements on one line (colon)
+    "E704",    # Incompatible with black: E704 multiple statements on one line (def)
 ]
 # Doc errors don't matter in the tests
 per-file-ignores = [
     "alluka/py.typed: D100",
     "noxfile.py: D100, FA101, F401, F403, INP001",
-    "tests/*.py: CCE002, DALL000, D100, D101, D103, D104, FA100, FA101, M511"
+    "tests/*.py: ASYNC910, CCE002, DALL000, D100, D101, D103, D104, FA100, FA101, M511"
 ]
 
 [tool.isort]
 profile = "black"
 force_single_line = true
 skip = ["alluka/_vendor"]
```

### Comparing `alluka-0.1.4/tests/__init__.py` & `alluka-0.1.5/tests/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
```

### Comparing `alluka-0.1.4/tests/test__client.py` & `alluka-0.1.5/tests/test__client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -90,22 +90,19 @@
         result = client.as_self_injecting(mock_callback)
 
         assert isinstance(result, alluka.SelfInjecting)
         assert result._callback is mock_callback
         assert result._client is client
 
     def test_call_with_di(self):
-        class MockType1:
-            ...
+        class MockType1: ...
 
-        class MockType2:
-            ...
+        class MockType2: ...
 
-        class MockType3:
-            ...
+        class MockType3: ...
 
         mock_value_1 = MockType1()
         mock_value_2 = MockType2()
         mock_value_3 = MockType3()
         mock_callback = mock.Mock()
         mock_override = mock.Mock()
 
@@ -142,16 +139,15 @@
         )
 
         result = client.call_with_di(callback, 43234, value_2="nyaa")
 
         assert result == "ok"
 
     def test_call_with_di_when_type_not_found(self):
-        class MockType:
-            ...
+        class MockType: ...
 
         def callback(value: alluka.Injected[MockType]) -> typing.NoReturn:
             raise NotImplementedError
 
         client = alluka.Client()
 
         with pytest.raises(alluka.MissingDependencyError):
@@ -166,40 +162,36 @@
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=RuntimeWarning)
 
             with pytest.raises(alluka.SyncOnlyError):
                 client.call_with_di(callback)
 
     def test_call_with_di_when_type_not_found_when_async_dependency(self):
-        class MockType:
-            ...
+        class MockType: ...
 
         def callback(
             value: alluka.Injected[MockType], dep: int = alluka.inject(callback=mock.AsyncMock())
         ) -> typing.NoReturn:
             raise NotImplementedError
 
         client = alluka.Client().set_type_dependency(MockType, MockType())
 
         with warnings.catch_warnings():
             warnings.filterwarnings("ignore", category=RuntimeWarning)
 
             with pytest.raises(alluka.SyncOnlyError):
                 client.call_with_di(callback)
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di(self):
-        class MockType1:
-            ...
+        class MockType1: ...
 
-        class MockType2:
-            ...
+        class MockType2: ...
 
-        class MockType3:
-            ...
+        class MockType3: ...
 
         mock_value_1 = MockType1()
         mock_value_2 = MockType2()
         mock_value_3 = MockType3()
         mock_callback = mock.Mock()
         mock_override = mock.AsyncMock()
         mock_other_callback = mock.AsyncMock()
@@ -240,18 +232,17 @@
             .set_callback_override(mock_other_callback, mock_other_override)
         )
 
         result = await client.call_with_async_di(callback, 43234, bar="nyaa")
 
         assert result == "ok"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_when_type_not_found(self):
-        class MockType:
-            ...
+        class MockType: ...
 
         def callback(value: alluka.Injected[MockType]) -> typing.NoReturn:
             raise NotImplementedError
 
         client = alluka.Client()
 
         with pytest.raises(alluka.MissingDependencyError):
```

### Comparing `alluka-0.1.4/tests/test__self_injecting.py` & `alluka-0.1.5/tests/test__self_injecting.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -31,15 +31,15 @@
 import mock
 import pytest
 
 import alluka
 
 
 class TestAsyncSelfInjecting:
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_dunder_method(self):
         mock_callback = mock.Mock()
         mock_client = mock.AsyncMock()
         self_injecting = alluka.AsyncSelfInjecting(mock_client, mock_callback)
 
         result = await self_injecting()
```

### Comparing `alluka-0.1.4/tests/test_async_callback_di.py` & `alluka-0.1.5/tests/test_async_callback_di.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -39,64 +39,62 @@
 from alluka._vendor import inspect
 
 # pyright: reportUnknownMemberType=none
 # pyright: reportPrivateUsage=none
 # pyright: reportIncompatibleMethodOverride=none
 
 
-class MockType(int):
-    ...
+class MockType(int): ...
 
 
-class MockOtherType(int):
-    ...
+class MockOtherType(int): ...
 
 
-@pytest.fixture()
+@pytest.fixture
 def client() -> alluka.Client:
     return alluka.Client()
 
 
-@pytest.fixture()
+@pytest.fixture
 def context(client: alluka.Client) -> alluka.BasicContext:
     return alluka.BasicContext(client)
 
 
 ##############################
 # Async dependency injection #
 ##############################
 
 
 # TODO: test cases for type scoped dependencies
 # TODO: test cases for cached callback results
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_when_no_di(context: alluka.BasicContext):
     async def callback(value_1: int, value_2: str) -> str:
         assert value_1 == 42
         assert value_2 == "ok"
         return "nyaa"
 
     result = await context.call_with_async_di(callback, 42, value_2="ok")
 
     assert result == "nyaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_missing_annotations(context: alluka.BasicContext):
     async def callback(value_1, value_2) -> str:  # type: ignore
         assert value_1 == 543123
         assert value_2 == "sdasd"
         return "meow"
 
     result = await context.call_with_async_di(callback, 543123, value_2="sdasd")  # type: ignore
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_prioritises_defaults_over_annotations(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
     mock_callback = mock.AsyncMock()
 
     async def dependency(
         result: typing.Annotated[float, alluka.inject(type=123)] = alluka.inject(callback=mock_callback)
@@ -122,15 +120,15 @@
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_and_callback(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
     mock_callback = mock.AsyncMock()
 
     async def callback(
         value_1: int,
@@ -150,15 +148,15 @@
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         value_1: int,
         value_2: str,
@@ -174,15 +172,15 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_type(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         nyaa: str, meow: int, value_1: MockType = alluka.inject(), value_2: MockOtherType = alluka.inject()
     ) -> str:
@@ -195,15 +193,15 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_annotated_type(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         nyaa: str,
         meow: int,
@@ -219,24 +217,24 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_missing_type(context: alluka.BasicContext):
     async def callback(nyaa: str, meow: int, _: MockType = alluka.inject(), value_1=alluka.inject()) -> str:  # type: ignore
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Could not resolve type for parameter 'value_1' with no annotation"):
         await context.call_with_async_di(callback, "5412", meow=34123)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_not_found(context: alluka.BasicContext):
     value = mock.Mock()
 
     async def callback(
         _: int, value: str, __: str = alluka.inject(type=MockType), ___: int = alluka.inject(type=MockOtherType)
     ) -> str:
         raise NotImplementedError
@@ -246,15 +244,15 @@
     with pytest.raises(alluka.MissingDependencyError) as exc:
         await context.call_with_async_di(callback, 69, value="rew")
 
     assert exc.value.message == f"Couldn't resolve injected type(s) {MockOtherType} to actual value"
     assert exc.value.dependency_type is MockOtherType
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_type_dependency(context: alluka.BasicContext):  # TODO: THIS
     value = mock.Mock()
 
     async def callback(
         value_1: int, value_2: str, value_3: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> str:
         assert value_1 == 69
@@ -265,15 +263,15 @@
     context.injection_client.set_type_dependency(MockType, value)
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         yeet: int, raw: str, value_1: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> str:
         assert yeet == 420
         assert raw == "uwu"
         assert value_1 is None
@@ -283,15 +281,15 @@
 
     assert result == "yeet"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency(context: alluka.BasicContext):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType)
@@ -301,26 +299,26 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_not_found(context: alluka.BasicContext):
         async def callback(_: int, __: str, cope: int = alluka.inject(type=MockOtherType | MockType)) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockOtherType | MockType} to actual value"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_defaulting(context: alluka.BasicContext):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType | None)
@@ -330,15 +328,15 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType | None)
         ) -> float:
             assert value_1 == 123
@@ -347,15 +345,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(
         value_1: int, value_2: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType])
     ) -> float:
@@ -365,29 +363,29 @@
         return 243.234
 
     result = await context.call_with_async_di(callback, 123, "ok")
 
     assert result == 243.234
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(_: int, __: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType])) -> float:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, 123, "ok")
 
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     assert exc_info.value.message == (
         f"Couldn't resolve injected type(s) {typing.Union[MockType, MockOtherType]} to actual value"
     )
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(
         value_1: int, value_2: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType, None])
     ) -> float:
@@ -397,30 +395,30 @@
         return 243.234
 
     result = await context.call_with_async_di(callback, 123, "ok")
 
     assert result == 243.234
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         value_1: float, value_2: int, cope: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> float:
         assert value_1 == 123.321
         assert value_2 == 543
         assert cope is None
         return 321.123
 
     result = await context.call_with_async_di(callback, 123.321, 543)
 
     assert result == 321.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         rawr: int,
         xd: float,
@@ -436,15 +434,15 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, rawr=69, xd="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency_inferred_from_type(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         meow: int,
         nyaa: float,
@@ -460,15 +458,15 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, meow=2222, nyaa="xxxxx")
 
     assert result == "wewewewew"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency_not_found(context: alluka.BasicContext):
     mock_other_value = mock.Mock()
 
     async def callback(
         meow: int,
         nyaa: float,
         meowmeow: typing.Annotated[int, alluka.inject(type=MockType)],
@@ -484,15 +482,15 @@
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockType} to actual value"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency(context: alluka.BasicContext):
         value = MockType()
 
         async def callback(
             yeee: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=MockType | MockOtherType)]
         ) -> str:
             assert yeee == "yeee"
@@ -502,28 +500,28 @@
 
         context.injection_client.set_type_dependency(MockOtherType, value)
 
         result = await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
         assert result == "hey"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_not_found(context: alluka.BasicContext):
         async def callback(
             _: int, __: str, cope: typing.Annotated[int, alluka.inject(type=MockOtherType | MockType)]
         ) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockOtherType | MockType} to actual value"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_defaulting(
         context: alluka.BasicContext,
     ):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
@@ -535,15 +533,15 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int, value_2: str, cope: typing.Annotated[int, alluka.inject(type=MockOtherType | MockType | None)]
         ) -> float:
             assert value_1 == 123
@@ -551,15 +549,15 @@
             assert cope is None
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_natural_defaulting(
         context: alluka.BasicContext,
     ):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
@@ -573,15 +571,15 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_natural_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int,
             value_2: str,
             cope: typing.Annotated[int, alluka.inject(type=MockOtherType | MockType)] = 43123,
@@ -592,15 +590,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
 
     async def callback(
         meow: int, meowmeow: typing.Annotated[typing.Union[MockType, MockOtherType], alluka.inject()]
     ) -> str:
         assert meow == 1233212
@@ -610,15 +608,15 @@
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     result = await context.call_with_async_di(callback, 1233212)
 
     assert result == "yay"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         yeee: str, nyaa: bool, yeet: typing.Annotated[int, alluka.inject(type=typing.Union[MockType, MockOtherType])]
     ) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
@@ -627,15 +625,15 @@
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     assert (
         exc_info.value.message
         == f"Couldn't resolve injected type(s) {typing.Union[MockType, MockOtherType]} to actual value"
     )
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]
     ) -> str:
@@ -645,30 +643,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]
     ) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet is None
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=MockType)] = "default"
     ) -> str:
@@ -678,30 +676,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(eaaaa: str, nyaa: bool, yeet: typing.Annotated[int, alluka.inject(type=MockType)] = 123) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet == 123
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(
         vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType])]
     ) -> str:
@@ -710,29 +708,29 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]) -> str:
         assert vvvvv == 123
         assert value is None
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(
         vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType])] = "default"
     ) -> str:
@@ -741,15 +739,15 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(
         vvvvv: int,
         value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType, None])] = "default 2",
     ) -> str:
@@ -758,15 +756,15 @@
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         rawr: int, xd: float, meowmeow: alluka.Injected[MockType], other: alluka.Injected[MockOtherType]
     ) -> str:
@@ -779,15 +777,15 @@
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     result = await context.call_with_async_di(callback, 1233212, xd="seee")
 
     assert result == "eeesss"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_type_dependency_not_found(context: alluka.BasicContext):
     mock_other_value = mock.Mock()
 
     async def callback(
         meow: int, nyaa: float, meowmeow: alluka.Injected[MockType], imacow: alluka.Injected[MockOtherType]
     ) -> str:
         raise NotImplementedError
@@ -800,15 +798,15 @@
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockType} to actual value"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency(context: alluka.BasicContext):
         value = MockType()
 
         async def callback(yeee: str, nyaa: bool, yeet: alluka.Injected[MockType | MockOtherType]) -> str:
             assert yeee == "yeee"
             assert nyaa is True
             assert yeet is value
@@ -816,29 +814,29 @@
 
         context.injection_client.set_type_dependency(MockOtherType, value)
 
         result = await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
         assert result == "hey"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(_: int, __: str, cope: alluka.Injected[MockOtherType | MockType]) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         # For whatever reason the order and format of the union in message's repr
         # isn't consistent here so it isn't tested.
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_defaulting(
         context: alluka.BasicContext,
     ):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
@@ -848,29 +846,29 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(value_1: int, value_2: str, cope: alluka.Injected[MockOtherType | MockType | None]) -> float:
             assert value_1 == 123
             assert value_2 == "ok"
             assert cope is None
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_natural_defaulting(
         context: alluka.BasicContext,
     ):
         value = MockType()
 
         context.injection_client.set_type_dependency(MockType, value)
 
@@ -882,15 +880,15 @@
             assert cope is value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_natural_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         mock_default = mock.Mock()
 
         async def callback(
             value_1: int, value_2: str, cope: alluka.Injected[MockOtherType | MockType] = mock_default
@@ -901,15 +899,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_union_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
 
     async def callback(meow: int, meowmeow: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
         assert meow == 1233212
         assert meowmeow is value
         return "yay"
@@ -917,30 +915,30 @@
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     result = await context.call_with_async_di(callback, 1233212)
 
     assert result == "yay"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(yeee: str, nyaa: bool, yeet: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     # For whatever reason the order and format of the union in message's repr
     # isn't consistent here so it isn't tested.
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
@@ -948,30 +946,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet is None
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_type_dependency(
     context: alluka.BasicContext,
 ):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[MockType] = MockType(43123123)) -> str:
@@ -981,30 +979,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[MockType] = MockType(123)) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet == 123
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_union_type_dependency(
     context: alluka.BasicContext,
 ):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(vvvvv: int, value: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
@@ -1013,29 +1011,29 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(vvvvv: int, value: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert vvvvv == 123
         assert value is None
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_union_type_dependency(
     context: alluka.BasicContext,
 ):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, value)
 
     async def callback(
@@ -1046,15 +1044,15 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(
         vvvvv: int, value: alluka.Injected[typing.Union[MockType, MockOtherType, None]] = MockType(54123123)
     ) -> str:
         assert vvvvv == 123
@@ -1062,30 +1060,30 @@
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.AsyncMock()
 
     async def callback(value_1: int, result: int = alluka.inject(callback=mock_callback)) -> int:
         assert value_1 == 123
         assert result is mock_callback.return_value
         return 43123
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == 43123
     mock_callback.assert_awaited_once()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.Mock()
 
     async def dependency(result: int = alluka.inject(callback=mock_callback)) -> int:
         assert result is mock_callback.return_value
         return 541232
 
@@ -1096,30 +1094,30 @@
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "43123"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.AsyncMock()
 
     async def callback(value_1: int, result: typing.Annotated[int, alluka.inject(callback=mock_callback)]) -> int:
         assert value_1 == 123
         assert result is mock_callback.return_value
         return 43123
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == 43123
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sub_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.AsyncMock()
 
     async def dependency(result: typing.Annotated[int, alluka.inject(callback=mock_callback)]) -> int:
         assert result is mock_callback.return_value
         return 541232
 
@@ -1130,15 +1128,15 @@
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "43123"
     mock_callback.assert_awaited_once()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_type_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def dependency(result: int = alluka.inject(type=MockType)) -> int:
         assert result is value
         return 123321
@@ -1149,30 +1147,30 @@
         return "asddsa"
 
     result = await context.call_with_async_di(callback, 54123)
 
     assert result == "asddsa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_type_dependency_not_found(context: alluka.BasicContext):
     async def dependency(result: int = alluka.inject(type=MockType)) -> int:
         raise NotImplementedError
 
     async def callback(_: int, result: int = alluka.inject(callback=dependency)) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, 54123)
 
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == (f"Couldn't resolve injected type(s) {MockType} to actual value")
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_when_sync_callback(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, value)
 
     async def dependency(value_1: int = alluka.inject(callback=mock_callback)) -> str:
         assert value_1 is mock_callback.return_value
@@ -1192,15 +1190,15 @@
 
     result = await context.call_with_async_di(callback, 1234321, value_2="meow meow")
 
     assert result == 123.321
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sync_dependency_callback(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     def dependency(value_1: alluka.Injected[MockOtherType]) -> str:
         assert value_1 is mock_other_value
@@ -1212,15 +1210,15 @@
         return "bye bye"
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_callback_override(mock_callback, mock_override)
 
     async def callback(value_1: alluka.Injected[MockType], value_2: str = alluka.inject(callback=mock_callback)) -> str:
@@ -1230,15 +1228,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, value)
 
     def dependency(result: str = alluka.inject(callback=mock_callback)) -> str:
         assert result is mock_callback.return_value
@@ -1251,15 +1249,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_sub_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_callback_override(mock_callback, mock_override)
 
     def dependency(result: typing.Annotated[str, alluka.inject(callback=mock_callback)]) -> str:
@@ -1273,15 +1271,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_other_value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_type_dependency(MockOtherType, mock_other_value)
 
     def dependency(value_1: alluka.Injected[MockOtherType]) -> str:
         assert value_1 is mock_other_value
@@ -1295,15 +1293,15 @@
         return "bye bye"
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_annotated_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_callback_override(mock_callback, mock_override)
 
     async def callback(
@@ -1315,15 +1313,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sub_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, value)
 
     def dependency(result: str = alluka.inject(callback=mock_callback)) -> str:
         assert result is mock_callback.return_value
@@ -1338,15 +1336,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_annotated_sub_sync_dependency(context: alluka.BasicContext):
     value = mock.Mock()
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, value).set_callback_override(mock_callback, mock_override)
 
     def dependency(result: typing.Annotated[str, alluka.inject(callback=mock_callback)]) -> str:
@@ -1367,37 +1365,37 @@
 
 
 ################################
 # Positional-only dependencies #
 ################################
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_positional_only_type_dependency(context: alluka.BasicContext):
     async def callback(_: int, __: str = alluka.inject(type=float), /, ___: float = alluka.inject(type=float)) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_positional_only_callback_dependency(context: alluka.BasicContext):
     mock_dependency = mock.Mock()
 
     async def callback(
         _: int, __: str = alluka.inject(callback=mock_dependency), /, ___: float = alluka.inject(type=float)
     ) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_positional_only_callback_dependency(context: alluka.BasicContext):
     sub_dependency = mock.Mock()
 
     async def dependency(_: str = alluka.inject(callback=sub_dependency), /) -> str:
         raise NotImplementedError
 
     async def callback(
@@ -1405,15 +1403,15 @@
     ) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_positional_only_type_dependency(context: alluka.BasicContext):
     async def dependency(_: str = alluka.inject(type=int), /) -> str:
         raise NotImplementedError
 
     async def callback(
         _: int, __: str = alluka.inject(callback=dependency), /, ___: float = alluka.inject(type=float)
     ) -> None:
@@ -1424,25 +1422,25 @@
 
 
 ############################
 # Signature-less callbacks #
 ############################
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_signature_less_callback(context: alluka.BasicContext):
     with pytest.raises(ValueError, match="no signature found for builtin type <class 'str'>"):
         inspect.signature(str)
 
     result = await context.call_with_async_di(str, b"ok")
 
     assert result == "b'ok'"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_signature_less_callback_dependency(context: alluka.BasicContext):
     with pytest.raises(ValueError, match="no signature found for builtin type <class 'int'>"):
         inspect.signature(int)
 
     def callback(value: int = alluka.inject(callback=int)) -> int:
         assert value == 0
         return 222
```

### Comparing `alluka-0.1.4/tests/test_async_callback_di_future_annotations.py` & `alluka-0.1.5/tests/test_async_callback_di_future_annotations.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -41,64 +41,62 @@
 from alluka._vendor import inspect
 
 # pyright: reportUnknownMemberType=none
 # pyright: reportPrivateUsage=none
 # pyright: reportIncompatibleMethodOverride=none
 
 
-class MockType(int):
-    ...
+class MockType(int): ...
 
 
-class MockOtherType(int):
-    ...
+class MockOtherType(int): ...
 
 
-@pytest.fixture()
+@pytest.fixture
 def client() -> alluka.Client:
     return alluka.Client()
 
 
-@pytest.fixture()
+@pytest.fixture
 def context(client: alluka.Client) -> alluka.BasicContext:
     return alluka.BasicContext(client)
 
 
 #################################################
 # Async dependency injection future annotations #
 #################################################
 
 
 # TODO: test cases for type scoped dependencies
 # TODO: test cases for cached callback results
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_when_no_di(context: alluka.BasicContext):
     async def callback(value_1: int, value_2: str) -> str:
         assert value_1 == 42
         assert value_2 == "ok"
         return "nyaa"
 
     result = await context.call_with_async_di(callback, 42, value_2="ok")
 
     assert result == "nyaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_missing_annotations(context: alluka.BasicContext):
     async def callback(value_1, value_2) -> str:  # type: ignore
         assert value_1 == 543123
         assert value_2 == "sdasd"
         return "meow"
 
     result = await context.call_with_async_di(callback, 543123, value_2="sdasd")  # type: ignore
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_prioritises_defaults_over_annotations(context: alluka.BasicContext):
     mock_value = mock.Mock()
     mock_other_value = mock.Mock()
     mock_callback = mock.AsyncMock()
 
     async def dependency(
         result: typing.Annotated[float, alluka.inject(type=123)] = alluka.inject(callback=mock_callback)
@@ -126,15 +124,15 @@
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_and_callback(context: alluka.BasicContext):
     mock_value = mock.Mock()
     mock_other_value = mock.Mock()
     mock_callback = mock.AsyncMock()
 
     async def callback(
         value_1: int,
@@ -156,15 +154,15 @@
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency(context: alluka.BasicContext):
     mock_value = mock.Mock()
     mock_other_value = mock.Mock()
 
     async def callback(
         value_1: int,
         value_2: str,
@@ -182,15 +180,15 @@
     )
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_type(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
 
     async def callback(
         nyaa: str, meow: int, value_1: MockType = alluka.inject(), value_2: MockOtherType = alluka.inject()
     ) -> str:
@@ -205,15 +203,15 @@
     )
 
     result = await context.call_with_async_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_annotated_type(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
 
     async def callback(
         nyaa: str,
         meow: int,
@@ -231,24 +229,24 @@
     )
 
     result = await context.call_with_async_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_inferred_from_missing_type(context: alluka.BasicContext):
     async def callback(nyaa: str, meow: int, _: MockType = alluka.inject(), value_1=alluka.inject()) -> str:  # type: ignore
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Could not resolve type for parameter 'value_1' with no annotation"):
         await context.call_with_async_di(callback, "5412", meow=34123)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_type_dependency_not_found(context: alluka.BasicContext):
     mock_value = mock.Mock()
 
     async def callback(
         _: int, value_1: str, __: str = alluka.inject(type=MockType), ___: int = alluka.inject(type=MockOtherType)
     ) -> str:
         raise NotImplementedError
@@ -258,15 +256,15 @@
     with pytest.raises(alluka.MissingDependencyError) as exc:
         await context.call_with_async_di(callback, 69, value_1="rew")
 
     assert exc.value.message == f"Couldn't resolve injected type(s) {MockOtherType} to actual value"
     assert exc.value.dependency_type is MockOtherType
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_type_dependency(context: alluka.BasicContext):  # TODO: THIS
     mock_value = mock.Mock()
 
     async def callback(
         value_1: int, value_2: str, value_3: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> str:
         assert value_1 == 69
@@ -277,15 +275,15 @@
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     result = await context.call_with_async_di(callback, 69, value_2="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         yeet: int, raw: str, value_1: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> str:
         assert yeet == 420
         assert raw == "uwu"
         assert value_1 is None
@@ -295,15 +293,15 @@
 
     assert result == "yeet"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency(context: alluka.BasicContext):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType)
@@ -313,27 +311,27 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_not_found(context: alluka.BasicContext):
         async def callback(_: int, __: str, cope: int = alluka.inject(type=MockOtherType | MockType)) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         # 3.10.1/2+ and 3.11 may re-order the | union types while resolving them from a string
         # future annotation so we can't reliably assert these.
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_defaulting(context: alluka.BasicContext):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType | None)
@@ -343,15 +341,15 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int, value_2: str, cope: int = alluka.inject(type=MockOtherType | MockType | None)
         ) -> float:
             assert value_1 == 123
@@ -360,15 +358,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_union_type_dependency(context: alluka.BasicContext):
     mock_value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(
         value_1: int, value_2: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType])
     ) -> float:
@@ -378,28 +376,28 @@
         return 243.234
 
     result = await context.call_with_async_di(callback, 123, "ok")
 
     assert result == 243.234
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(_: int, __: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType])) -> float:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, 123, "ok")
 
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     # On 3.10.1/2+ typing.Unions are converted to | while resolving future annotations so we can't consistently
     # assert the message.
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_union_type_dependency(context: alluka.BasicContext):
     mock_value = mock.Mock()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(
         value_1: int, value_2: str, cope: int = alluka.inject(type=typing.Union[MockType, MockOtherType, None])
     ) -> float:
@@ -409,30 +407,30 @@
         return 243.234
 
     result = await context.call_with_async_di(callback, 123, "ok")
 
     assert result == 243.234
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_defaulting_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         value_1: float, value_2: int, cope: typing.Optional[int] = alluka.inject(type=typing.Optional[MockType])
     ) -> float:
         assert value_1 == 123.321
         assert value_2 == 543
         assert cope is None
         return 321.123
 
     result = await context.call_with_async_di(callback, 123.321, 543)
 
     assert result == 321.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
 
     async def callback(
         rawr: int,
         xd: float,
@@ -450,15 +448,15 @@
     )
 
     result = await context.call_with_async_di(callback, rawr=69, xd="rew")
 
     assert result == "meow"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency_inferred_from_type(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
 
     async def callback(
         meow: int,
         nyaa: float,
@@ -476,15 +474,15 @@
     )
 
     result = await context.call_with_async_di(callback, meow=2222, nyaa="xxxxx")
 
     assert result == "wewewewew"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_type_dependency_not_found(context: alluka.BasicContext):
     mock_other_value = MockOtherType()
 
     async def callback(
         meow: int,
         nyaa: float,
         meowmeow: typing.Annotated[int, alluka.inject(type=MockType)],
@@ -500,15 +498,15 @@
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockType} to actual value"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency(context: alluka.BasicContext):
         mock_value = MockOtherType()
 
         async def callback(
             yeee: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=MockType | MockOtherType)]
         ) -> str:
             assert yeee == "yeee"
@@ -518,29 +516,29 @@
 
         context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
         result = await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
         assert result == "hey"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_not_found(context: alluka.BasicContext):
         async def callback(
             _: int, __: str, cope: typing.Annotated[int, alluka.inject(type=MockOtherType | MockType)]
         ) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         # 3.10.1/2+ and 3.11 may re-order the | union types while resolving them from a string
         # future annotation so we can't reliably assert these.
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_defaulting(
         context: alluka.BasicContext,
     ):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
@@ -552,15 +550,15 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int, value_2: str, cope: typing.Annotated[int, alluka.inject(type=MockOtherType | MockType | None)]
         ) -> float:
             assert value_1 == 123
@@ -568,15 +566,15 @@
             assert cope is None
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_natural_defaulting(
         context: alluka.BasicContext,
     ):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
@@ -590,15 +588,15 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_annotated_3_10_union_type_dependency_natural_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(
             value_1: int, value_2: str, cope: typing.Annotated[int, alluka.inject(type=MockType | MockType)] = 43123
         ) -> float:
             assert value_1 == 123
@@ -607,15 +605,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_union_type_dependency(context: alluka.BasicContext):
     mock_value = MockOtherType()
 
     async def callback(
         meow: int, meowmeow: typing.Annotated[typing.Union[MockType, MockOtherType], alluka.inject()]
     ) -> str:
         assert meow == 1233212
@@ -625,30 +623,30 @@
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     result = await context.call_with_async_di(callback, 1233212)
 
     assert result == "yay"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_union_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         yeee: str, nyaa: bool, yeet: typing.Annotated[int, alluka.inject(type=typing.Union[MockType, MockOtherType])]
     ) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     # On 3.10.1/2+ typing.Unions are converted to | while resolving future annotations so we can't consistently
     # assert the message.
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_type_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]
     ) -> str:
@@ -658,30 +656,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_type_dependency_not_found(context: alluka.BasicContext):
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]
     ) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet is None
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_type_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def callback(
         eaaaa: str, nyaa: bool, yeet: typing.Annotated[str, alluka.inject(type=MockType)] = "default"
     ) -> str:
@@ -691,30 +689,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(eaaaa: str, nyaa: bool, yeet: typing.Annotated[int, alluka.inject(type=MockType)] = 123) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet == 123
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_union_type_dependency(context: alluka.BasicContext):
     mock_value = MockOtherType()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(
         vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType])]
     ) -> str:
@@ -723,29 +721,29 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Optional[MockType])]) -> str:
         assert vvvvv == 123
         assert value is None
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_union_type_dependency(context: alluka.BasicContext):
     mock_value = MockOtherType()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(
         vvvvv: int, value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType])] = "default"
     ) -> str:
@@ -754,15 +752,15 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_natural_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(
         vvvvv: int,
         value: typing.Annotated[str, alluka.inject(type=typing.Union[MockType, MockOtherType, None])] = "default 2",
     ) -> str:
@@ -771,15 +769,15 @@
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_type_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
 
     async def callback(
         rawr: int, xd: float, meowmeow: alluka.Injected[MockType], other: alluka.Injected[MockOtherType]
     ) -> str:
@@ -794,15 +792,15 @@
     )
 
     result = await context.call_with_async_di(callback, 1233212, xd="seee")
 
     assert result == "eeesss"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_type_dependency_not_found(context: alluka.BasicContext):
     mock_other_value = MockOtherType()
 
     async def callback(
         meow: int, nyaa: float, meowmeow: alluka.Injected[MockType], imacow: alluka.Injected[MockOtherType]
     ) -> str:
         raise NotImplementedError
@@ -815,15 +813,15 @@
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == f"Couldn't resolve injected type(s) {MockType} to actual value"
 
 
 # These tests covers syntax which was introduced in 3.10
 if sys.version_info >= (3, 10):  # TODO: do we want to dupe other test cases for |?
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency(context: alluka.BasicContext):
         mock_value = MockOtherType()
 
         async def callback(yeee: str, nyaa: bool, yeet: alluka.Injected[MockType | MockOtherType]) -> str:
             assert yeee == "yeee"
             assert nyaa is True
             assert yeet is mock_value
@@ -831,29 +829,29 @@
 
         context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
         result = await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
         assert result == "hey"
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(_: int, __: str, cope: alluka.Injected[MockOtherType | MockType]) -> float:
             raise NotImplementedError
 
         with pytest.raises(alluka.MissingDependencyError) as exc_info:
             await context.call_with_async_di(callback, 123, "ok")
 
         assert exc_info.value.dependency_type == MockOtherType | MockType
         # 3.10.1/2+ and 3.11 may re-order the | union types while resolving them from a string
         # future annotation so we can't reliably assert these.
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_defaulting(
         context: alluka.BasicContext,
     ):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
@@ -863,29 +861,29 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         async def callback(value_1: int, value_2: str, cope: alluka.Injected[MockOtherType | MockType | None]) -> float:
             assert value_1 == 123
             assert value_2 == "ok"
             assert cope is None
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_natural_defaulting(
         context: alluka.BasicContext,
     ):
         mock_value = MockType()
 
         context.injection_client.set_type_dependency(MockType, mock_value)
 
@@ -897,15 +895,15 @@
             assert cope is mock_value
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
-    @pytest.mark.anyio()
+    @pytest.mark.anyio
     async def test_call_with_async_di_with_shorthand_annotated_3_10_union_type_dependency_natural_defaulting_not_found(
         context: alluka.BasicContext,
     ):
         mock_default = MockOtherType()
 
         async def callback(
             value_1: int, value_2: str, cope: alluka.Injected[MockOtherType | MockType] = mock_default
@@ -916,15 +914,15 @@
             return 451.123
 
         result = await context.call_with_async_di(callback, 123, "ok")
 
         assert result == 451.123
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_union_type_dependency(context: alluka.BasicContext):
     mock_value = MockOtherType()
 
     async def callback(meow: int, meowmeow: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
         assert meow == 1233212
         assert meowmeow is mock_value
         return "yay"
@@ -932,30 +930,30 @@
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     result = await context.call_with_async_di(callback, 1233212)
 
     assert result == "yay"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(yeee: str, nyaa: bool, yeet: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, yeee="yeee", nyaa=True)
 
     assert exc_info.value.dependency_type == typing.Union[MockType, MockOtherType]
     # On 3.10.1/2+ typing.Unions are converted to | while resolving future annotations so we can't consistently
     # assert the message.
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_type_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
@@ -963,30 +961,30 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert eaaaa == "easd"
         assert nyaa is False
         assert yeet is None
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_type_dependency(
     context: alluka.BasicContext,
 ):
     mock_value = MockType()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[MockType] = MockType()) -> str:
@@ -996,15 +994,15 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     mock_default = MockType()
 
     async def callback(eaaaa: str, nyaa: bool, yeet: alluka.Injected[MockType] = mock_default) -> str:
         assert eaaaa == "easd"
@@ -1013,15 +1011,15 @@
         return "aaaaa"
 
     result = await context.call_with_async_di(callback, "easd", nyaa=False)
 
     assert result == "aaaaa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_union_type_dependency(
     context: alluka.BasicContext,
 ):
     mock_value = MockOtherType()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(vvvvv: int, value: alluka.Injected[typing.Union[MockType, MockOtherType]]) -> str:
@@ -1030,29 +1028,29 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     async def callback(vvvvv: int, value: alluka.Injected[typing.Optional[MockType]]) -> str:
         assert vvvvv == 123
         assert value is None
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_union_type_dependency(
     context: alluka.BasicContext,
 ):
     mock_value = MockOtherType()
     context.injection_client.set_type_dependency(MockOtherType, mock_value)
 
     async def callback(
@@ -1063,15 +1061,15 @@
         return "ea sports"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "ea sports"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_shorthand_annotated_natural_defaulting_union_type_dependency_not_found(
     context: alluka.BasicContext,
 ):
     mock_default = MockOtherType()
 
     async def callback(
         vvvvv: int, value: alluka.Injected[typing.Union[MockType, MockOtherType, None]] = mock_default
@@ -1081,30 +1079,30 @@
         return "yeeee"
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "yeeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.AsyncMock()
 
     async def callback(value_1: int, result: int = alluka.inject(callback=mock_callback)) -> int:
         assert value_1 == 123
         assert result is mock_callback.return_value
         return 43123
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == 43123
     mock_callback.assert_awaited_once()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_callback_dependency(context: alluka.BasicContext):
     mock_callback = mock.Mock()
 
     async def dependency(result: int = alluka.inject(callback=mock_callback)) -> int:
         assert result is mock_callback.return_value
         return 541232
 
@@ -1115,15 +1113,15 @@
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "43123"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_callback_dependency(context: alluka.BasicContext):
     global mock_callback
     mock_callback = mock.AsyncMock()
 
     async def callback(value_1: int, result: typing.Annotated[int, alluka.inject(callback=mock_callback)]) -> int:
         assert value_1 == 123
         assert result is mock_callback.return_value
@@ -1131,15 +1129,15 @@
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == 43123
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sub_callback_dependency(context: alluka.BasicContext):
     global mock_callback
     mock_callback = mock.AsyncMock()
     global dependency_3
 
     async def dependency_3(result: typing.Annotated[int, alluka.inject(callback=mock_callback)]) -> int:
         assert result is mock_callback.return_value
@@ -1152,15 +1150,15 @@
 
     result = await context.call_with_async_di(callback, 123)
 
     assert result == "43123"
     mock_callback.assert_awaited_once()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_type_dependency(context: alluka.BasicContext):
     mock_value = mock.Mock()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def dependency(result: int = alluka.inject(type=MockType)) -> int:
         assert result is mock_value
         return 123321
@@ -1171,30 +1169,30 @@
         return "asddsa"
 
     result = await context.call_with_async_di(callback, 54123)
 
     assert result == "asddsa"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_type_dependency_not_found(context: alluka.BasicContext):
     async def dependency(result: int = alluka.inject(type=MockType)) -> int:
         raise NotImplementedError
 
     async def callback(_: int, result: int = alluka.inject(callback=dependency)) -> str:
         raise NotImplementedError
 
     with pytest.raises(alluka.MissingDependencyError) as exc_info:
         await context.call_with_async_di(callback, 54123)
 
     assert exc_info.value.dependency_type is MockType
     assert exc_info.value.message == (f"Couldn't resolve injected type(s) {MockType} to actual value")
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_when_sync_callback(context: alluka.BasicContext):
     mock_value = MockType()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     async def dependency(value_1: int = alluka.inject(callback=mock_callback)) -> str:
         assert value_1 is mock_callback.return_value
@@ -1214,15 +1212,15 @@
 
     result = await context.call_with_async_di(callback, 1234321, value_2="meow meow")
 
     assert result == 123.321
     mock_callback.assert_awaited_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sync_dependency_callback(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
     context.injection_client.set_type_dependency(MockType, mock_value).set_type_dependency(
         MockOtherType, mock_other_value
     )
 
@@ -1236,15 +1234,15 @@
         return "bye bye"
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, mock_value).set_callback_override(
         mock_callback, mock_override
     )
@@ -1256,15 +1254,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     def dependency(result: str = alluka.inject(callback=mock_callback)) -> str:
         assert result is mock_callback.return_value
@@ -1277,15 +1275,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_sub_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     global mock_callback
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, mock_value).set_callback_override(
         mock_callback, mock_override
@@ -1302,15 +1300,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_other_value = MockOtherType()
     context.injection_client.set_type_dependency(MockType, mock_value).set_type_dependency(
         MockOtherType, mock_other_value
     )
     global dependency_4
@@ -1327,15 +1325,15 @@
         return "bye bye"
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_annotated_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     global mock_callback
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     context.injection_client.set_type_dependency(MockType, mock_value).set_callback_override(
         mock_callback, mock_override
@@ -1350,15 +1348,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_override.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_annotated_sub_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     mock_callback = mock.AsyncMock()
     context.injection_client.set_type_dependency(MockType, mock_value)
 
     global dependency
 
@@ -1375,15 +1373,15 @@
 
     result = await context.call_with_async_di(callback)
 
     assert result == "bye bye"
     mock_callback.assert_called_once_with()
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_overridden_annotated_sub_sync_dependency(context: alluka.BasicContext):
     mock_value = MockType()
     global mock_callback
     mock_callback = mock.AsyncMock()
     mock_override = mock.Mock()
     global dependency_1
     context.injection_client.set_type_dependency(MockType, mock_value).set_callback_override(
@@ -1408,37 +1406,37 @@
 
 
 ################################
 # Positional-only dependencies #
 ################################
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_positional_only_type_dependency(context: alluka.BasicContext):
     async def callback(_: int, __: str = alluka.inject(type=float), /, ___: float = alluka.inject(type=float)) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_positional_only_callback_dependency(context: alluka.BasicContext):
     mock_dependency = mock.Mock()
 
     async def callback(
         _: int, __: str = alluka.inject(callback=mock_dependency), /, ___: float = alluka.inject(type=float)
     ) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_positional_only_callback_dependency(context: alluka.BasicContext):
     sub_dependency = mock.Mock()
 
     async def dependency(_: str = alluka.inject(callback=sub_dependency), /) -> str:
         raise NotImplementedError
 
     async def callback(
@@ -1446,15 +1444,15 @@
     ) -> None:
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Injected positional only arguments are not supported"):
         await context.call_with_async_di(callback)
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_sub_positional_only_type_dependency(context: alluka.BasicContext):
     async def dependency(_: str = alluka.inject(type=int), /) -> str:
         raise NotImplementedError
 
     async def callback(
         _: int, __: str = alluka.inject(callback=dependency), /, ___: float = alluka.inject(type=float)
     ) -> None:
@@ -1465,25 +1463,25 @@
 
 
 ############################
 # Signature-less callbacks #
 ############################
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_di_with_signature_less_callback(context: alluka.BasicContext):
     with pytest.raises(ValueError, match="no signature found for builtin type <class 'str'>"):
         inspect.signature(str)
 
     result = await context.call_with_async_di(str, b"ok")
 
     assert result == "b'ok'"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 async def test_call_with_async_dix_with_signature_less_callback_dependency(context: alluka.BasicContext):
     with pytest.raises(ValueError, match="no signature found for builtin type <class 'int'>"):
         inspect.signature(int)
 
     def callback(value: int = alluka.inject(callback=int)) -> int:
         assert value == 0
         return 222
```

### Comparing `alluka-0.1.4/tests/test_callback_di.py` & `alluka-0.1.5/tests/test_callback_di.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -40,28 +40,26 @@
 from alluka._vendor import inspect
 
 # pyright: reportUnknownMemberType=none
 # pyright: reportPrivateUsage=none
 # pyright: reportIncompatibleMethodOverride=none
 
 
-class MockType(int):
-    ...
+class MockType(int): ...
 
 
-class MockOtherType(int):
-    ...
+class MockOtherType(int): ...
 
 
-@pytest.fixture()
+@pytest.fixture
 def client() -> alluka.Client:
     return alluka.Client()
 
 
-@pytest.fixture()
+@pytest.fixture
 def context(client: alluka.Client) -> alluka.BasicContext:
     return alluka.BasicContext(client)
 
 
 #############################
 # Sync dependency injection #
 #############################
@@ -223,15 +221,15 @@
     )
 
     result = context.call_with_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 def test_call_with_di_with_type_dependency_inferred_from_missing_type(context: alluka.BasicContext):
     def callback(nyaa: str, meow: int, _: MockType = alluka.inject(), value_1=alluka.inject()) -> str:  # type: ignore
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Could not resolve type for parameter 'value_1' with no annotation"):
         context.call_with_di(callback, "5412", meow=34123)
```

### Comparing `alluka-0.1.4/tests/test_callback_di_future_annotations.py` & `alluka-0.1.5/tests/test_callback_di_future_annotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # BSD 3-Clause License
 #
-# Copyright (c) 2020-2023, Faster Speeding
+# Copyright (c) 2020-2024, Faster Speeding
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions are met:
 #
 # * Redistributions of source code must retain the above copyright notice, this
 #   list of conditions and the following disclaimer.
@@ -42,28 +42,26 @@
 from alluka._vendor import inspect
 
 # pyright: reportUnknownMemberType=none
 # pyright: reportPrivateUsage=none
 # pyright: reportIncompatibleMethodOverride=none
 
 
-class MockType(int):
-    ...
+class MockType(int): ...
 
 
-class MockOtherType(int):
-    ...
+class MockOtherType(int): ...
 
 
-@pytest.fixture()
+@pytest.fixture
 def client() -> alluka.Client:
     return alluka.Client()
 
 
-@pytest.fixture()
+@pytest.fixture
 def context(client: alluka.Client) -> alluka.BasicContext:
     return alluka.BasicContext(client)
 
 
 ################################################
 # Sync dependency injection future annotations #
 ################################################
@@ -225,15 +223,15 @@
     )
 
     result = context.call_with_di(callback, "5412", meow=34123)
 
     assert result == "heeee"
 
 
-@pytest.mark.anyio()
+@pytest.mark.anyio
 def test_call_with_di_with_type_dependency_inferred_from_missing_type(context: alluka.BasicContext):
     def callback(nyaa: str, meow: int, _: MockType = alluka.inject(), value_1=alluka.inject()) -> str:  # type: ignore
         raise NotImplementedError
 
     with pytest.raises(ValueError, match="Could not resolve type for parameter 'value_1' with no annotation"):
         context.call_with_di(callback, "5412", meow=34123)
```

### Comparing `alluka-0.1.4/PKG-INFO` & `alluka-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alluka
-Version: 0.1.4
+Version: 0.1.5
 Summary: A type based dependency injection framework for Python 3.9+.
 Keywords: DI,injection
 Author-email: Faster Speeding <lucina@lmbyrne.dev>
 Requires-Python: >=3.9.0,<3.13
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AnyIO
```

