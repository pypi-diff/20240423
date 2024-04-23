# Comparing `tmp/openscap-report-0.2.7.tar.gz` & `tmp/openscap_report-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openscap-report-0.2.7.tar", last modified: Fri Jan 26 15:05:42 2024, max compression
+gzip compressed data, was "openscap_report-0.2.9.tar", last modified: Tue Apr 23 13:04:55 2024, max compression
```

## Comparing `openscap-report-0.2.7.tar` & `openscap_report-0.2.9.tar`

### file list

```diff
@@ -1,250 +1,253 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.577112 openscap-report-0.2.7/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-01-26 15:05:32.000000 openscap-report-0.2.7/.eslintignore
--rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-01-26 15:05:32.000000 openscap-report-0.2.7/.eslintrc.yml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-01-26 15:05:32.000000 openscap-report-0.2.7/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    20901 2024-01-26 15:05:32.000000 openscap-report-0.2.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)    26955 2024-01-26 15:05:32.000000 openscap-report-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-01-26 15:05:32.000000 openscap-report-0.2.7/LICENSE.spdx
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-01-26 15:05:32.000000 openscap-report-0.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-26 15:05:42.577112 openscap-report-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-01-26 15:05:32.000000 openscap-report-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.449112 openscap-report-0.2.7/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/README
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.441112 openscap-report-0.2.7/docs/exts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.449112 openscap-report-0.2.7/docs/exts/sphinxarg/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/exts/sphinxarg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21796 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/exts/sphinxarg/ext.py
--rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/exts/sphinxarg/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/exts/sphinxarg/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.449112 openscap-report-0.2.7/docs/manual/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.465112 openscap-report-0.2.7/docs/manual/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    46854 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/about_profile.png
--rw-r--r--   0 runner    (1001) docker     (127)    44006 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/compliance_and_scoring.png
--rw-r--r--   0 runner    (1001) docker     (127)   114896 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/cpe_aplicability_language.png
--rw-r--r--   0 runner    (1001) docker     (127)    79764 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/evaluation_characteristics.png
--rw-r--r--   0 runner    (1001) docker     (127)  8589473 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/example_report.html
--rw-r--r--   0 runner    (1001) docker     (127)  1072728 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/oval.gif
--rw-r--r--   0 runner    (1001) docker     (127)    41993 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/remediation.png
--rw-r--r--   0 runner    (1001) docker     (127)   168763 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/rule_detail.png
--rw-r--r--   0 runner    (1001) docker     (127)    50802 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/assets/rule_overview_section.png
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/report.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/test-suite.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/manual/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.465112 openscap-report-0.2.7/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/openscap_report.report_generators.rst
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/openscap_report.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.data_structures.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.parsers.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.rst
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/oscap-report.1.rst
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-26 15:05:32.000000 openscap-report-0.2.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.465112 openscap-report-0.2.7/openscap_report/
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/debug_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.469112 openscap-report-0.2.7/openscap_report/report_generators/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.469112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.469112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
--rw-r--r--   0 runner    (1001) docker     (127)   102224 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    79100 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.473112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/pficon/
--rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
--rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
--rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/base_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/cpe_graph.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.473112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/css/
--rw-r--r--   0 runner    (1001) docker     (127)  1413415 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/css/patternfly.css
--rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/css/style.css
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/evaluation_characteristics.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.473112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/debug_script.js
--rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/interactive_script.js
--rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.473112 openscap-report-0.2.7/openscap_report/report_generators/html_templates/macros/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/macros/list_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/oval_definition_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/oval_graph.html
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/profile_info.html
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/remedations.html
--rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/rule_detail.html
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/rule_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/rules_overview.html
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/score_bar.html
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/search_input.html
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/summary_banner.html
--rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/html_templates/template_report.html
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/old_style_html.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/report_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.477112 openscap-report-0.2.7/openscap_report/report_generators/xsl/
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-branding.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-references.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    55343 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.477112 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/
--rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
--rw-r--r--   0 runner    (1001) docker     (127)    88498 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    97163 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
--rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
--rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
--rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources-build.sh
--rw-r--r--   0 runner    (1001) docker     (127)   223540 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources.xsl
--rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-share.xsl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.481112 openscap-report-0.2.7/openscap_report/scap_results_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.485112 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/cpe_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/json_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_node.py
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_variable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/profile_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/reference.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/remediation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/result_of_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1864 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/rule.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/warning.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.485112 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/group_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/known_references.py
--rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_endpoint_information_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_object_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6587 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_state_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_variable_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/profile_info_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/remediation_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/report_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8613 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/scan_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/scap_results_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    45405 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    22573 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    72864 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    29292 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/catalog.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xlink.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xml.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (127)    13927 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.445112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.489112 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
--rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
--rw-r--r--   0 runner    (1001) docker     (127)   230463 2024-01-26 15:05:32.000000 openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.573112 openscap-report-0.2.7/openscap_report.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10808 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-26 15:05:42.000000 openscap-report-0.2.7/openscap_report.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 15:05:32.000000 openscap-report-0.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-26 15:05:42.577112 openscap-report-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-01-26 15:05:32.000000 openscap-report-0.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.493112 openscap-report-0.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/integration.fmf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.493112 openscap-report-0.2.7/tests/integration_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/integration_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/integration_tests/test_basic_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/integration_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/integration_tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/json_schema_of_report.json
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/smoke.fmf
--rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-01-26 15:05:32.000000 openscap-report-0.2.7/tests/smoke.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.573112 openscap-report-0.2.7/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127) 12129838 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf-container.xml
--rw-r--r--   0 runner    (1001) docker     (127) 23777754 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf-dangling-reference-to.xml
--rw-r--r--   0 runner    (1001) docker     (127) 19008654 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf-report.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20294 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (127)    48058 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_cpe_check_os_platform.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (127)    18595 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (127)    36477 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (127)    21028 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/arf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/empty.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/empty.xml
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/plant_catalog.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.573112 openscap-report-0.2.7/tests/test_data/remediations_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
--rw-r--r--   0 runner    (1001) docker     (127)  7631650 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf-report.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf-with-removed-info.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf_multi_check.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf_no_system_data.xml
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf_rule_and_cpe_check.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf_simple_rule_fail.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_data/xccdf_simple_rule_pass.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:42.573112 openscap-report-0.2.7/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_cpe_al_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_data_structure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_debug_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_full_text_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_json_transitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_oval_result_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_oval_tree_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)    15973 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_scap_result_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tests/unit_tests/test_shared_static_methods_of_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-01-26 15:05:33.000000 openscap-report-0.2.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.478152 openscap_report-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 13:04:50.000000 openscap_report-0.2.9/.eslintignore
+-rw-r--r--   0 runner    (1001) docker     (127)     5739 2024-04-23 13:04:50.000000 openscap_report-0.2.9/.eslintrc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 13:04:50.000000 openscap_report-0.2.9/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    20901 2024-04-23 13:04:50.000000 openscap_report-0.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)    26955 2024-04-23 13:04:50.000000 openscap_report-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-23 13:04:50.000000 openscap_report-0.2.9/LICENSE.spdx
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-23 13:04:50.000000 openscap_report-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 13:04:55.478152 openscap_report-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-04-23 13:04:50.000000 openscap_report-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.350152 openscap_report-0.2.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/README
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/docs/exts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.350152 openscap_report-0.2.9/docs/exts/sphinxarg/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/exts/sphinxarg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21796 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/exts/sphinxarg/ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10306 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/exts/sphinxarg/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6922 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/exts/sphinxarg/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.354152 openscap_report-0.2.9/docs/manual/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.366152 openscap_report-0.2.9/docs/manual/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    46854 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/about_profile.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44006 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/compliance_and_scoring.png
+-rw-r--r--   0 runner    (1001) docker     (127)   114896 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/cpe_aplicability_language.png
+-rw-r--r--   0 runner    (1001) docker     (127)    79764 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/evaluation_characteristics.png
+-rw-r--r--   0 runner    (1001) docker     (127)  8589473 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/example_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)  1072728 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/oval.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    41993 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/remediation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   168763 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/rule_detail.png
+-rw-r--r--   0 runner    (1001) docker     (127)    50802 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/assets/rule_overview_section.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/report.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/test-suite.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/manual/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.366152 openscap_report-0.2.9/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/openscap_report.report_generators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/openscap_report.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6073 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.data_structures.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.parsers.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/oscap-report.1.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-23 13:04:50.000000 openscap_report-0.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.366152 openscap_report-0.2.9/openscap_report/
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7102 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.370152 openscap_report-0.2.9/openscap_report/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45855 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/dataclasses/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/debug_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.370152 openscap_report-0.2.9/openscap_report/report_generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/webfonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   102224 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    79100 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/pficon/
+-rw-r--r--   0 runner    (1001) docker     (127)    20416 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    17172 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     6507 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/base_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/cpe_graph.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/css/
+-rw-r--r--   0 runner    (1001) docker     (127)  1413415 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/css/patternfly.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/evaluation_characteristics.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/debug_script.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7122 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/interactive_script.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35120 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.374152 openscap_report-0.2.9/openscap_report/report_generators/html_templates/macros/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/macros/list_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/oval_definition_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/oval_graph.html
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/profile_info.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/remedations.html
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/rule_detail.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/rule_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/rules_overview.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/score_bar.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/search_input.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/severity_of_failed_rules.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/summary_banner.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/html_templates/template_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/old_style_html.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/report_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.378152 openscap_report-0.2.9/openscap_report/report_generators/xsl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-branding.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-references.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    55343 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report-impl.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    13750 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.378152 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/
+-rw-r--r--   0 runner    (1001) docker     (127)    17087 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    88498 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14148 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    97163 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16611 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8157 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/openscap.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/openscap.js
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1691 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources-build.sh
+-rw-r--r--   0 runner    (1001) docker     (127)   223540 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources.xsl
+-rw-r--r--   0 runner    (1001) docker     (127)    21382 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-share.xsl
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.378152 openscap_report-0.2.9/openscap_report/scap_results_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.382152 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/cpe_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/json_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_variable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/profile_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/remediation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5245 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/result_of_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/warning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.386152 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/group_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/known_references.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_definition_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_endpoint_information_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_object_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6604 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_state_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_variable_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/profile_info_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/remediation_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/report_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8630 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/scan_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/scap_results_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.386152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    45405 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    22573 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    72864 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    29292 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.386152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/catalog.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     8029 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xlink.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xml.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.386152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7927 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.386152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.390152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    13644 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.390152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    13324 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)    13927 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.346152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.390152 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    16018 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)    14174 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd
+-rw-r--r--   0 runner    (1001) docker     (127)   230463 2024-04-23 13:04:50.000000 openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.478152 openscap_report-0.2.9/openscap_report.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10891 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 13:04:55.000000 openscap_report-0.2.9/openscap_report.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:04:50.000000 openscap_report-0.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:04:55.478152 openscap_report-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-23 13:04:50.000000 openscap_report-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.390152 openscap_report-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/integration.fmf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.390152 openscap_report-0.2.9/tests/integration_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/integration_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2036 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/integration_tests/test_basic_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/integration_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/integration_tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11203 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/json_schema_of_report.json
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/smoke.fmf
+-rwxr-xr-x   0 runner    (1001) docker     (127)      517 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/smoke.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.474152 openscap_report-0.2.9/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127) 12129838 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf-container.xml
+-rw-r--r--   0 runner    (1001) docker     (127) 23777754 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf-dangling-reference-to.xml
+-rw-r--r--   0 runner    (1001) docker     (127) 19008654 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20294 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    48058 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_cpe_check_os_platform.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    18595 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    36477 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    21028 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (127)    20987 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/arf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/empty.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/empty.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/plant_catalog.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.474152 openscap_report-0.2.9/tests/test_data/remediations_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  7631650 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf-report.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf-with-removed-info.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf_multi_check.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf_no_system_data.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf_rule_and_cpe_check.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5209 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf_simple_rule_fail.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_data/xccdf_simple_rule_pass.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:55.478152 openscap_report-0.2.9/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4364 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_cpe_al_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_debug_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3310 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_full_text_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_json_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7291 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_oval_result_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_oval_tree_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_scap_result_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tests/unit_tests/test_shared_static_methods_of_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2024-04-23 13:04:50.000000 openscap_report-0.2.9/tox.ini
```

### Comparing `openscap-report-0.2.7/.eslintrc.yml` & `openscap_report-0.2.9/.eslintrc.yml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/.pylintrc` & `openscap_report-0.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/LICENSE` & `openscap_report-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/PKG-INFO` & `openscap_report-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.7
+Version: 0.2.9
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.spdx
 Requires-Dist: lxml
 Requires-Dist: jinja2
 
 # OpenSCAP Report Generator
```

### Comparing `openscap-report-0.2.7/README.md` & `openscap_report-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/conf.py` & `openscap_report-0.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/exts/sphinxarg/ext.py` & `openscap_report-0.2.9/docs/exts/sphinxarg/ext.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/exts/sphinxarg/markdown.py` & `openscap_report-0.2.9/docs/exts/sphinxarg/markdown.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/exts/sphinxarg/parser.py` & `openscap_report-0.2.9/docs/exts/sphinxarg/parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/about_profile.png` & `openscap_report-0.2.9/docs/manual/assets/about_profile.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/compliance_and_scoring.png` & `openscap_report-0.2.9/docs/manual/assets/compliance_and_scoring.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/cpe_aplicability_language.png` & `openscap_report-0.2.9/docs/manual/assets/cpe_aplicability_language.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/evaluation_characteristics.png` & `openscap_report-0.2.9/docs/manual/assets/evaluation_characteristics.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/example_report.html` & `openscap_report-0.2.9/docs/manual/assets/example_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/oval.gif` & `openscap_report-0.2.9/docs/manual/assets/oval.gif`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/remediation.png` & `openscap_report-0.2.9/docs/manual/assets/remediation.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/rule_detail.png` & `openscap_report-0.2.9/docs/manual/assets/rule_detail.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/assets/rule_overview_section.png` & `openscap_report-0.2.9/docs/manual/assets/rule_overview_section.png`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/installation.rst` & `openscap_report-0.2.9/docs/manual/installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     sudo pip3 install openscap-report
 
 Installation from source
 ------------------------
 
 Requirements:
 
-* Python 3.8+
+* Python 3.6+
 * `lxml`_
 * `jinja2`_
 
 .. code-block:: console
 
     # Get repository with code
     git clone https://github.com/OpenSCAP/openscap-report.git
```

### Comparing `openscap-report-0.2.7/docs/manual/report.rst` & `openscap_report-0.2.9/docs/manual/report.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/test-suite.rst` & `openscap_report-0.2.9/docs/manual/test-suite.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/manual/usage.rst` & `openscap_report-0.2.9/docs/manual/usage.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/modules/openscap_report.report_generators.rst` & `openscap_report-0.2.9/docs/modules/openscap_report.report_generators.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/modules/openscap_report.rst` & `openscap_report-0.2.9/docs/modules/openscap_report.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.data_structures.rst` & `openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.data_structures.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.parsers.rst` & `openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.parsers.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/docs/modules/openscap_report.scap_results_parser.rst` & `openscap_report-0.2.9/docs/modules/openscap_report.scap_results_parser.rst`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/cli.py` & `openscap_report-0.2.9/openscap_report/cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/debug_settings.py` & `openscap_report-0.2.9/openscap_report/debug_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import dataclass
+from openscap_report.dataclasses import dataclass
 
 
 @dataclass
 class DebugSetting():
     no_minify: bool = False
     options_require_debug_script: tuple = (
         "BUTTON-SHOW-ALL-RULES",
```

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html.py` & `openscap_report-0.2.9/openscap_report/report_generators/html.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/fonts/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/assets/pficon/pficon.woff2`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/base_report.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/base_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/cpe_graph.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/cpe_graph.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/css/patternfly.css` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/css/patternfly.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/css/style.css` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/css/style.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/evaluation_characteristics.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/evaluation_characteristics.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/debug_script.js` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/debug_script.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/interactive_script.js` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/interactive_script.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/js/oval_graph_generation_script.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/oval_definition_detail.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/oval_definition_detail.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/oval_graph.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/oval_graph.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/remedations.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/remedations.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/rule_detail.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/rule_detail.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/rule_results.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/rule_results.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/rules_overview.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/rules_overview.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/score_bar.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/score_bar.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/search_input.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/search_input.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/severity_of_failed_rules.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/severity_of_failed_rules.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/summary_banner.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/summary_banner.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/html_templates/template_report.html` & `openscap_report-0.2.9/openscap_report/report_generators/html_templates/template_report.html`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/json.py` & `openscap_report-0.2.9/openscap_report/report_generators/json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/old_style_html.py` & `openscap_report-0.2.9/openscap_report/report_generators/old_style_html.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-branding.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-branding.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-references.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-references.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report-impl.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report-impl.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report-oval-details.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-report.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-report.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap-config.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.min.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/jquery.treetable.theme.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/openscap.css` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/openscap.css`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources/openscap.js` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources/openscap.js`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources-build.sh` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources-build.sh`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-resources.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-resources.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/report_generators/xsl/xccdf-share.xsl` & `openscap_report-0.2.9/openscap_report/report_generators/xsl/xccdf-share.xsl`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/__init__.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/cpe_logical_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 from collections import Counter
-from dataclasses import asdict, dataclass, field
 from typing import List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from .cpe_result_eval import EMPTY_RESULT, OVAL_RESULT_TO_CPE_RESULT, CpeResult
 from .oval_node import OvalNode
 
 NEGATE_VALUE = {
     "true": "false",
     "false": "true",
     "error": "error",
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/cpe_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/group.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/group.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 GROUP_JSON_KEYS = [
     "group_id",
     "title",
     "description",
     "platforms",
     "rules_ids",
     "sub_groups",
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/json_transformation.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/json_transformation.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_definition.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from .oval_node import OvalNode
 from .oval_reference import OvalReference
 
 OVAL_DEFINITION_JSON_KEYS = [
     "definition_id",
     "title",
     "description",
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_node.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import json
 import logging
 from collections import Counter
-from dataclasses import asdict, dataclass, field
 from typing import List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from .oval_result_eval import (EMPTY_RESULT, FULL_RESULT_TO_SHORT_RESULT,
                                SHORT_RESULT_TO_FULL_RESULT, OvalResult)
 from .oval_test import OvalTest
 
 
 @dataclass
 class OvalNode:  # pylint: disable=R0902
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_result_eval.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/oval_test.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/oval_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import Dict, List, Union
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from .oval_object import OvalObject
 from .oval_state import OvalState
 from .oval_variable import OvalVariable
 
 
 @dataclass
 class OvalTest:  # pylint: disable=R0902
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/profile_info.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/profile_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import Dict, List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 PROFILE_JSON_KEYS = [
     "profile_id",
     "description",
     "title",
     "extends",
 ]
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/remediation.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/remediation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass
+from openscap_report.dataclasses import asdict, dataclass
 
 REMEDIATION_JSON_KEYS = [
     "remediation_id",
     "system",
     "complexity",
     "disruption",
     "strategy",
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/report.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import logging
-from dataclasses import asdict, dataclass, field
 from typing import Dict
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from ..exceptions import MissingProcessableRules
 from .group import GROUP_JSON_KEYS, Group
 from .identifier import IDENTIFIER_JSON_KEYS
 from .json_transformation import (rearrange_identifiers, rearrange_references,
                                   remove_empty_values,
                                   remove_not_selected_rules)
 from .oval_definition import OVAL_DEFINITION_JSON_KEYS
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/result_of_scan.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/result_of_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import Dict, List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 SCAN_JSON_KEYS = [
     "title",
     "identity",
     "profile_id",
     "target",
     "cpe_platforms",
     "scanner",
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/data_structures/rule.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/data_structures/rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
-from dataclasses import asdict, dataclass, field
 from typing import Dict, List
 
+from openscap_report.dataclasses import asdict, dataclass, field
+
 from .cpe_platform import Platform
 from .identifier import Identifier
 from .oval_definition import OvalDefinition
 from .oval_node import OvalNode
 from .reference import Reference
 from .remediation import Remediation
 from .warning import RuleWarning
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/exceptions.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/namespaces.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/namespaces.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/oval_and_cpe_tree_builder.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/__init__.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/cpe_al_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/cpe_al_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/full_text_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/group_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/group_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/known_references.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/known_references.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_definition_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_definition_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_endpoint_information_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_endpoint_information_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_object_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_object_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_result_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_result_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import logging
 import uuid
-from dataclasses import dataclass
 
 from lxml.etree import Element
 
+from openscap_report.dataclasses import dataclass
+
 from ..data_structures import OvalNode
 from ..exceptions import MissingOVALResult
 from ..namespaces import NAMESPACES
 from .oval_test_parser import OVALTestParser
 
 STR_TO_BOOL = {'true': True, 'false': False}
 STR_NEGATION_BOOL = {'true': 'false', 'false': 'true'}
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_state_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_state_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_test_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_test_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/oval_variable_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/oval_variable_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/profile_info_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/profile_info_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/remediation_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/remediation_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/report_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/report_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/rule_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/rule_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import collections
-from dataclasses import replace
+
+from openscap_report.dataclasses import replace
 
 from ..data_structures import Identifier, Reference, Rule, RuleWarning
 from ..namespaces import NAMESPACES
 from .full_text_parser import FullTextParser
 from .known_references import KNOWN_REFERENCES, update_references
 from .remediation_parser import RemediationParser
```

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/scan_result_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/scan_result_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/parsers/shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/scap_results_parser.py` & `openscap_report-0.2.9/openscap_report/scap_results_parser/scap_results_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/asset-identification_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/asset-reporting-format_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/reporting-core_1.1.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/xAL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/arf/1.1/xNL.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/catalog.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/catalog.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xlink.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xlink.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xml.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xml.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/common/xmldsig-core-schema.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.0/cpe-dictionary_2.0.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.1/cpe-dictionary_2.1.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.2/cpe-dictionary_2.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-dictionary_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/cpe/2.3/cpe-naming_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/XMLSchema.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/cpe-language_2.3.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/datatypes.dtd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd` & `openscap_report-0.2.9/openscap_report/scap_results_parser/schemas/xccdf/1.2/xccdf_1.2.xsd`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/openscap_report.egg-info/PKG-INFO` & `openscap_report-0.2.9/openscap_report.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: openscap-report
-Version: 0.2.7
+Version: 0.2.9
 Summary: Tool for generating report from results of oscap scan.
 Home-page: https://github.com/OpenSCAP/oscap-report
 Author: Jan Rodak
 Author-email: jrodak@redhat.com
 License: LGPL-2.1 License
-Requires-Python: >=3.8
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.spdx
 Requires-Dist: lxml
 Requires-Dist: jinja2
 
 # OpenSCAP Report Generator
```

### Comparing `openscap-report-0.2.7/openscap_report.egg-info/SOURCES.txt` & `openscap_report-0.2.9/openscap_report.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 openscap_report.egg-info/PKG-INFO
 openscap_report.egg-info/SOURCES.txt
 openscap_report.egg-info/dependency_links.txt
 openscap_report.egg-info/entry_points.txt
 openscap_report.egg-info/not-zip-safe
 openscap_report.egg-info/requires.txt
 openscap_report.egg-info/top_level.txt
+openscap_report/dataclasses/__init__.py
+openscap_report/dataclasses/dataclasses.py
 openscap_report/report_generators/__init__.py
 openscap_report/report_generators/exceptions.py
 openscap_report/report_generators/html.py
 openscap_report/report_generators/json.py
 openscap_report/report_generators/old_style_html.py
 openscap_report/report_generators/report_generator.py
 openscap_report/report_generators/html_templates/base_report.html
```

### Comparing `openscap-report-0.2.7/setup.py` & `openscap_report-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
+# pylint: disable=import-error
 from setuptools import find_packages, setup
 
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as readme_file:
         return readme_file.read()
 
 
 setup(name='openscap-report',
-      version='0.2.7',
+      version='0.2.9',
       description='Tool for generating report from results of oscap scan.',
       long_description=get_long_description(),
       long_description_content_type="text/markdown",
       url='https://github.com/OpenSCAP/oscap-report',
       author='Jan Rodak',
       author_email='jrodak@redhat.com',
       license='LGPL-2.1 License',
@@ -26,9 +27,9 @@
       include_package_data=True,
       zip_safe=False,
       entry_points={
           'console_scripts': [
               'oscap-report=openscap_report.cli:main',
           ],
       },
-      python_requires='>=3.8',
+      python_requires='>=3.6',
       )
```

### Comparing `openscap-report-0.2.7/tests/constants.py` & `openscap_report-0.2.9/tests/constants.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/integration.fmf` & `openscap_report-0.2.9/tests/integration.fmf`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/integration_tests/test_basic_usage.py` & `openscap_report-0.2.9/tests/integration_tests/test_basic_usage.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/integration_tests/test_cli.py` & `openscap_report-0.2.9/tests/integration_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/integration_tests/test_json.py` & `openscap_report-0.2.9/tests/integration_tests/test_json.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/json_schema_of_report.json` & `openscap_report-0.2.9/tests/json_schema_of_report.json`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/smoke.sh` & `openscap_report-0.2.9/tests/smoke.sh`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf-container.xml` & `openscap_report-0.2.9/tests/test_data/arf-container.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf-dangling-reference-to.xml` & `openscap_report-0.2.9/tests/test_data/arf-dangling-reference-to.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf-report.xml` & `openscap_report-0.2.9/tests/test_data/arf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf-with-removed-info.xml` & `openscap_report-0.2.9/tests/test_data/arf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_cpe_check_os_platform.xml` & `openscap_report-0.2.9/tests/test_data/arf_cpe_check_os_platform.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_multi_check.xml` & `openscap_report-0.2.9/tests/test_data/arf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_no_system_data.xml` & `openscap_report-0.2.9/tests/test_data/arf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_rule_and_cpe_check.xml` & `openscap_report-0.2.9/tests/test_data/arf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_simple_rule_fail.xml` & `openscap_report-0.2.9/tests/test_data/arf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/arf_simple_rule_pass.xml` & `openscap_report-0.2.9/tests/test_data/arf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/plant_catalog.xml` & `openscap_report-0.2.9/tests/test_data/plant_catalog.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt` & `openscap_report-0.2.9/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt` & `openscap_report-0.2.9/tests/test_data/remediations_scripts/auditd_data_retention_action_mail_acct_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt` & `openscap_report-0.2.9/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_ansible.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt` & `openscap_report-0.2.9/tests/test_data/remediations_scripts/dconf_gnome_screensaver_lock_enabled_sh.txt`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf-report.xml` & `openscap_report-0.2.9/tests/test_data/xccdf-report.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf-with-removed-info.xml` & `openscap_report-0.2.9/tests/test_data/xccdf-with-removed-info.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf_multi_check.xml` & `openscap_report-0.2.9/tests/test_data/xccdf_multi_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf_no_system_data.xml` & `openscap_report-0.2.9/tests/test_data/xccdf_no_system_data.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf_rule_and_cpe_check.xml` & `openscap_report-0.2.9/tests/test_data/xccdf_rule_and_cpe_check.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf_simple_rule_fail.xml` & `openscap_report-0.2.9/tests/test_data/xccdf_simple_rule_fail.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_data/xccdf_simple_rule_pass.xml` & `openscap_report-0.2.9/tests/test_data/xccdf_simple_rule_pass.xml`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/test_utils.py` & `openscap_report-0.2.9/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import argparse
 import tempfile
-from dataclasses import replace
 from pathlib import Path
 
 try:
     from functools import cache
 except ImportError:
     from functools import lru_cache
 
     cache = lru_cache(maxsize=None)
 
 from lxml import etree
 
+from openscap_report.dataclasses import replace
 from openscap_report.scap_results_parser import SCAPResultsParser
 from openscap_report.scap_results_parser.data_structures import OvalDefinition
 from openscap_report.scap_results_parser.namespaces import NAMESPACES
 from openscap_report.scap_results_parser.parsers import (
     CPEApplicabilityLanguageParser, RuleParser)
 
 from .constants import (PATH_TO_ARF,
```

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_cli.py` & `openscap_report-0.2.9/tests/unit_tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_cpe_al_parser.py` & `openscap_report-0.2.9/tests/unit_tests/test_cpe_al_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_data_structure.py` & `openscap_report-0.2.9/tests/unit_tests/test_data_structure.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_debug_settings.py` & `openscap_report-0.2.9/tests/unit_tests/test_debug_settings.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_full_text_parser.py` & `openscap_report-0.2.9/tests/unit_tests/test_full_text_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_json_transitions.py` & `openscap_report-0.2.9/tests/unit_tests/test_json_transitions.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_oval_result_eval.py` & `openscap_report-0.2.9/tests/unit_tests/test_oval_result_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_oval_tree_eval.py` & `openscap_report-0.2.9/tests/unit_tests/test_oval_tree_eval.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_scap_result_parser.py` & `openscap_report-0.2.9/tests/unit_tests/test_scap_result_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright 2022, Red Hat, Inc.
 # SPDX-License-Identifier: LGPL-2.1-or-later
 
 import logging
-from contextlib import nullcontext as does_not_raise
 
 import pytest
 from lxml.etree import XMLSyntaxError
 
 from openscap_report.scap_results_parser import ARF_SCHEMAS_PATH
 from openscap_report.scap_results_parser.data_structures import (Report, Rule,
                                                                  RuleWarning)
@@ -52,18 +51,29 @@
     (PATH_TO_XCCDF_WITHOUT_SYSTEM_DATA, False),
 ])
 def test_validation(file_path, result):
     parser = get_parser(file_path)
     assert parser.validate(ARF_SCHEMAS_PATH) == result
 
 
+class DoesNotRaise:
+    def __init__(self, enter_result=None):
+        self.enter_result = enter_result
+
+    def __enter__(self):
+        return self.enter_result
+
+    def __exit__(self, *excinfo):
+        pass
+
+
 @pytest.mark.unit_test
 @pytest.mark.parametrize("file_path, expectation, e_msg", [
-    (PATH_TO_ARF, does_not_raise(), ""),
-    (PATH_TO_XCCDF, does_not_raise(), "input is the XCCDF"),
+    (PATH_TO_ARF, DoesNotRaise(), ""),
+    (PATH_TO_XCCDF, DoesNotRaise(), "input is the XCCDF"),
     (PATH_TO_EMPTY_XML_FILE, pytest.raises(NotSupportedReportingFormat), "isn't a valid"),
     (PATH_TO_EMPTY_FILE, pytest.raises(XMLSyntaxError), "empty"),
     (PATH_TO_XML_FILE, pytest.raises(NotSupportedReportingFormat), "isn't a valid"),
 ])
 def test_parsers_init(file_path, expectation, e_msg, caplog):
     caplog.set_level(logging.WARNING)
     with expectation as excinfo:
```

### Comparing `openscap-report-0.2.7/tests/unit_tests/test_shared_static_methods_of_parser.py` & `openscap_report-0.2.9/tests/unit_tests/test_shared_static_methods_of_parser.py`

 * *Files identical despite different names*

### Comparing `openscap-report-0.2.7/tox.ini` & `openscap_report-0.2.9/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 # tox (https://tox.readthedocs.io/) is a tool for running tests
 # in multiple virtualenvs. This configuration file will run the
 # test suite on all supported python versions. To use it, "pip install tox"
 # and then run "tox" from this directory.
 
 [tox]
-envlist = clean, py3, py38, report, code_style
+envlist = clean, py3, py36, py38, report, code_style
 
 [pytest]
 markers =
     integration_test: marks tests as integration tests (deselect with '-m "not integration_test"')
     unit_test: marks tests as unit tests (deselect with '-m "not unit_test"')
     serial
 
 [testenv]
 commands =
         py.test --cov=openscap_report --cov-append --cov-report=term-missing -m "not integration_test"
         py.test --cov-report=term-missing -m "not unit_test"
 deps =
-    pytest
     pytest-cov
     jsonschema
     -rrequirements.txt
 
 [testenv:report]
 deps = coverage
 skip_install = true
@@ -45,11 +44,11 @@
     jsonschema
     pylint
     isort
     flake8
 skip_install = true
 allowlist_externals = eslint
 commands =
-        -isort --check-only --diff ./openscap_report ./tests setup.py
-        -flake8 ./openscap_report ./tests setup.py
-        -pylint --rcfile=.pylintrc ./openscap_report ./tests setup.py
+        isort --check-only --diff ./openscap_report ./tests setup.py
+        flake8 ./openscap_report ./tests setup.py
+        pylint --rcfile=.pylintrc ./openscap_report ./tests setup.py
         -eslint ./openscap_report/**
```

