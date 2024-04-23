# Comparing `tmp/cityseer-4.8.1.tar.gz` & `tmp/cityseer-4.9.0.tar.gz`

## Comparing `cityseer-4.8.1.tar` & `cityseer-4.9.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
--rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 cityseer-4.8.1/Cargo.toml
--rw-r--r--   0     1001      127       57 2023-12-31 13:35:17.000000 cityseer-4.8.1/.gitattributes
--rw-r--r--   0     1001      127      457 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0     1001      127      595 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0     1001      127      639 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/release-drafter.yml
--rw-r--r--   0     1001      127      919 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/workflows/firebase-hosting-merge.yml
--rw-r--r--   0     1001      127      896 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/workflows/firebase-hosting-pull-request.yml
--rw-r--r--   0     1001      127     2995 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/workflows/publish_package.yml
--rw-r--r--   0     1001      127     3068 2023-12-31 13:35:17.000000 cityseer-4.8.1/.github/workflows/publish_package_dev.yml
--rw-r--r--   0     1001      127     1303 2023-12-31 13:35:17.000000 cityseer-4.8.1/.gitignore
--rw-r--r--   0     1001      127      495 2023-12-31 13:35:17.000000 cityseer-4.8.1/.vscode/launch.json
--rw-r--r--   0     1001      127     1216 2023-12-31 13:35:17.000000 cityseer-4.8.1/.vscode/settings.json
--rw-r--r--   0     1001      127    34523 2023-12-31 13:35:17.000000 cityseer-4.8.1/LICENSE.txt
--rw-r--r--   0     1001      127     4908 2023-12-31 13:35:17.000000 cityseer-4.8.1/README.md
--rw-r--r--   0     1001      127    56462 2023-12-31 13:35:17.000000 cityseer-4.8.1/coverage.lcov
--rw-r--r--   0     1001      127     1086 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.eslintrc.cjs
--rw-r--r--   0     1001      127       59 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.firebaserc
--rw-r--r--   0     1001      127      136 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.gitignore
--rw-r--r--   0     1001      127       94 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.markdownlint.json
--rw-r--r--   0     1001      127      477 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.prettierrc.cjs
--rw-r--r--   0     1001      127      131 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/.stylelintrc.cjs
--rw-r--r--   0     1001      127     3935 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/astro.config.mjs
--rw-r--r--   0     1001      127      874 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/firebase.json
--rw-r--r--   0     1001      127     9453 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/generate_docs.py
--rw-r--r--   0     1001      127       98 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/jsconfig.json
--rw-r--r--   0     1001      127   680491 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/package-lock.json
--rw-r--r--   0     1001      127     2060 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/package.json
--rw-r--r--   0     1001      127       80 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/pdoc_templates/frame.html.jinja2
--rw-r--r--   0     1001      127     5034 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/pdoc_templates/module.html.jinja2
--rw-r--r--   0     1001      127    30749 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/plots/matplotlibrc
--rw-r--r--   0     1001      127     8426 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/plots/plots.py
--rw-r--r--   0     1001      127      225 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/postcss.config.cjs
--rw-r--r--   0     1001      127    20009 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/favicons/192.png
--rw-r--r--   0     1001      127    53920 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/favicons/512.png
--rw-r--r--   0     1001      127    18313 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/favicons/apple-touch-icon.png
--rw-r--r--   0     1001      127     3094 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/favicons/favicon.ico
--rw-r--r--   0     1001      127     4792 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/favicons/icon.svg
--rw-r--r--   0     1001      127   150208 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/assignment.png
--rw-r--r--   0     1001      127   156699 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/assignment_decomposed.png
--rw-r--r--   0     1001      127   161095 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/assignment_plot.png
--rw-r--r--   0     1001      127    96510 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/betas.png
--rw-r--r--   0     1001      127   158785 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph.png
--rw-r--r--   0     1001      127   814163 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_1.png
--rw-r--r--   0     1001      127   714248 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_1b.png
--rw-r--r--   0     1001      127   783296 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_2.png
--rw-r--r--   0     1001      127   711826 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_3.png
--rw-r--r--   0     1001      127   713875 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_4.png
--rw-r--r--   0     1001      127   704350 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_5.png
--rw-r--r--   0     1001      127   703032 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_cleaning_6.png
--rw-r--r--   0     1001      127   197015 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_colour.png
--rw-r--r--   0     1001      127   169923 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_decomposed.png
--rw-r--r--   0     1001      127   286652 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_dual.png
--rw-r--r--   0     1001      127   169332 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_example.png
--rw-r--r--   0     1001      127   140961 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/graph_simple.png
--rw-r--r--   0     1001      127   291560 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/intro_mixed_uses.png
--rw-r--r--   0     1001      127   387283 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/images/intro_segment_harmonic.png
--rw-r--r--   0     1001      127    35386 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/logos/cityseer_logo_light_red.png
--rw-r--r--   0     1001      127    31349 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/logos/cityseer_logo_white.png
--rw-r--r--   0     1001      127      174 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/manifest.webmanifest
--rw-r--r--   0     1001      127       22 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/public/robots.txt
--rw-r--r--   0     1001      127     1378 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/bib/mendeley.bib
--rw-r--r--   0     1001      127    35885 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_deep_blue.png
--rw-r--r--   0     1001      127    35841 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_deep_red.png
--rw-r--r--   0     1001      127    35913 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_light_blue.png
--rw-r--r--   0     1001      127    35386 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_light_red.png
--rw-r--r--   0     1001      127    31349 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_white.png
--rw-r--r--   0     1001      127    35386 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/logo.png
--rw-r--r--   0     1001      127    17306 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/assets/logos/round_logo.png
--rw-r--r--   0     1001      127      929 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/components/ArXivLink.vue
--rw-r--r--   0     1001      127      154 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/components/Footer.astro
--rw-r--r--   0     1001      127     4286 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/components/NavColumn.vue
--rw-r--r--   0     1001      127      394 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/components/RepoLink.astro
--rw-r--r--   0     1001      127      192 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/components/StripeTitle.astro
--rw-r--r--   0     1001      127       38 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/env.d.ts
--rw-r--r--   0     1001      127    17305 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/favicon.png
--rw-r--r--   0     1001      127     1897 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/layouts/CommonLayout.astro
--rw-r--r--   0     1001      127     1899 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/layouts/PageLayout.astro
--rw-r--r--   0     1001      127     1447 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/attribution.md
--rw-r--r--   0     1001      127     2530 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/examples.md
--rw-r--r--   0     1001      127    13667 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/guide.md
--rw-r--r--   0     1001      127     2997 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/index.astro
--rw-r--r--   0     1001      127    17162 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/intro.md
--rw-r--r--   0     1001      127    38733 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/metrics/layers.md
--rw-r--r--   0     1001      127    23894 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/metrics/networks.md
--rw-r--r--   0     1001      127     9296 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/metrics/observe.md
--rw-r--r--   0     1001      127    13330 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/metrics/visibility.md
--rw-r--r--   0     1001      127    66320 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/rustalgos/rustalgos.md
--rw-r--r--   0     1001      127    26530 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/tools/graphs.md
--rw-r--r--   0     1001      127    31933 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/tools/io.md
--rw-r--r--   0     1001      127    12403 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/tools/mock.md
--rw-r--r--   0     1001      127    32612 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/tools/plot.md
--rw-r--r--   0     1001      127    21336 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/pages/tools/util.md
--rw-r--r--   0     1001      127     2826 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/styles/tailwind.css
--rw-r--r--   0     1001      127     1718 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/src/styles/yapper.css
--rw-r--r--   0     1001      127     1225 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/tailwind.config.cjs
--rw-r--r--   0     1001      127      246 2023-12-31 13:35:17.000000 cityseer-4.8.1/docs/tsconfig.json
--rw-r--r--   0     1001      127   176582 2023-12-31 13:35:17.000000 cityseer-4.8.1/pdm.lock
--rw-r--r--   0     1001      127      187 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/__init__.py
--rw-r--r--   0     1001      127     2200 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/config.py
--rw-r--r--   0     1001      127       71 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/metrics/__init__.py
--rw-r--r--   0     1001      127    35286 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/metrics/layers.py
--rw-r--r--   0     1001      127    22688 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/metrics/networks.py
--rw-r--r--   0     1001      127    15944 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/metrics/observe.py
--rw-r--r--   0     1001      127    12277 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/metrics/visibility.py
--rw-r--r--   0     1001      127    24631 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/rustalgos.pyi
--rw-r--r--   0     1001      127       72 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/__init__.py
--rw-r--r--   0     1001      127    74215 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/graphs.py
--rw-r--r--   0     1001      127    47806 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/io.py
--rw-r--r--   0     1001      127    14930 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/mock.py
--rw-r--r--   0     1001      127    38188 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/plot.py
--rw-r--r--   0     1001      127    24219 2023-12-31 13:35:17.000000 cityseer-4.8.1/pysrc/cityseer/tools/util.py
--rw-r--r--   0     1001      127    43805 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/centrality.rs
--rw-r--r--   0     1001      127     8810 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/common.rs
--rw-r--r--   0     1001      127    37742 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/data.rs
--rw-r--r--   0     1001      127    18460 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/diversity.rs
--rw-r--r--   0     1001      127    25182 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/graph.rs
--rw-r--r--   0     1001      127     2213 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/lib.rs
--rw-r--r--   0     1001      127     7072 2023-12-31 13:35:17.000000 cityseer-4.8.1/src/viewshed.rs
--rw-r--r--   0     1001      127    32065 2023-12-31 13:35:17.000000 cityseer-4.8.1/test.prof
--rw-r--r--   0     1001      127        0 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/__init__.py
--rw-r--r--   0     1001      127     3365 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/conftest.py
--rw-r--r--   0     1001      127        0 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/metrics/__init__.py
--rw-r--r--   0     1001      127    12322 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/metrics/test_layers.py
--rw-r--r--   0     1001      127     7856 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/metrics/test_networks.py
--rw-r--r--   0     1001      127      684 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/metrics/test_visibility.py
--rw-r--r--   0     1001      127        0 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/rustalgos/__init__.py
--rw-r--r--   0     1001      127    37355 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/rustalgos/test_centrality.py
--rw-r--r--   0     1001      127     9660 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/rustalgos/test_common.py
--rw-r--r--   0     1001      127    22447 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/rustalgos/test_data.py
--rw-r--r--   0     1001      127     8200 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/rustalgos/test_diversity.py
--rw-r--r--   0     1001      127     4389 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/test_performance.py
--rw-r--r--   0     1001      127        0 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/tools/__init__.py
--rw-r--r--   0     1001      127    26130 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/tools/test_graphs.py
--rw-r--r--   0     1001      127    36154 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/tools/test_io.py
--rw-r--r--   0     1001      127     3594 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/tools/test_mock.py
--rw-r--r--   0     1001      127     6859 2023-12-31 13:35:17.000000 cityseer-4.8.1/tests/tools/test_util.py
--rw-r--r--   0     1001      127    14400 2023-12-31 13:35:17.000000 cityseer-4.8.1/Cargo.lock
--rw-r--r--   0     1001      127     5691 2023-12-31 13:35:17.000000 cityseer-4.8.1/pyproject.toml
--rw-r--r--   0        0        0     6250 1970-01-01 00:00:00.000000 cityseer-4.8.1/PKG-INFO
+-rw-r--r--   0        0        0      867 1970-01-01 00:00:00.000000 cityseer-4.9.0/Cargo.toml
+-rw-r--r--   0     1001      127       57 2023-12-31 13:53:03.000000 cityseer-4.9.0/.gitattributes
+-rw-r--r--   0     1001      127      457 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0     1001      127      595 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0     1001      127      639 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/release-drafter.yml
+-rw-r--r--   0     1001      127      919 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/workflows/firebase-hosting-merge.yml
+-rw-r--r--   0     1001      127      896 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/workflows/firebase-hosting-pull-request.yml
+-rw-r--r--   0     1001      127     2995 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/workflows/publish_package.yml
+-rw-r--r--   0     1001      127     3068 2023-12-31 13:53:03.000000 cityseer-4.9.0/.github/workflows/publish_package_dev.yml
+-rw-r--r--   0     1001      127     1303 2023-12-31 13:53:03.000000 cityseer-4.9.0/.gitignore
+-rw-r--r--   0     1001      127      495 2023-12-31 13:53:03.000000 cityseer-4.9.0/.vscode/launch.json
+-rw-r--r--   0     1001      127     1216 2023-12-31 13:53:03.000000 cityseer-4.9.0/.vscode/settings.json
+-rw-r--r--   0     1001      127    34523 2023-12-31 13:53:03.000000 cityseer-4.9.0/LICENSE.txt
+-rw-r--r--   0     1001      127     4908 2023-12-31 13:53:03.000000 cityseer-4.9.0/README.md
+-rw-r--r--   0     1001      127    56462 2023-12-31 13:53:03.000000 cityseer-4.9.0/coverage.lcov
+-rw-r--r--   0     1001      127     1086 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.eslintrc.cjs
+-rw-r--r--   0     1001      127       59 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.firebaserc
+-rw-r--r--   0     1001      127      136 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.gitignore
+-rw-r--r--   0     1001      127       94 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.markdownlint.json
+-rw-r--r--   0     1001      127      477 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.prettierrc.cjs
+-rw-r--r--   0     1001      127      131 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/.stylelintrc.cjs
+-rw-r--r--   0     1001      127     3935 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/astro.config.mjs
+-rw-r--r--   0     1001      127      874 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/firebase.json
+-rw-r--r--   0     1001      127     9453 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/generate_docs.py
+-rw-r--r--   0     1001      127       98 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/jsconfig.json
+-rw-r--r--   0     1001      127   680491 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/package-lock.json
+-rw-r--r--   0     1001      127     2060 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/package.json
+-rw-r--r--   0     1001      127       80 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/pdoc_templates/frame.html.jinja2
+-rw-r--r--   0     1001      127     5034 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/pdoc_templates/module.html.jinja2
+-rw-r--r--   0     1001      127    30749 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/plots/matplotlibrc
+-rw-r--r--   0     1001      127     8426 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/plots/plots.py
+-rw-r--r--   0     1001      127      225 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/postcss.config.cjs
+-rw-r--r--   0     1001      127    20009 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/favicons/192.png
+-rw-r--r--   0     1001      127    53920 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/favicons/512.png
+-rw-r--r--   0     1001      127    18313 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/favicons/apple-touch-icon.png
+-rw-r--r--   0     1001      127     3094 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/favicons/favicon.ico
+-rw-r--r--   0     1001      127     4792 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/favicons/icon.svg
+-rw-r--r--   0     1001      127   150208 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/assignment.png
+-rw-r--r--   0     1001      127   156699 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/assignment_decomposed.png
+-rw-r--r--   0     1001      127   161095 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/assignment_plot.png
+-rw-r--r--   0     1001      127    96510 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/betas.png
+-rw-r--r--   0     1001      127   158785 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph.png
+-rw-r--r--   0     1001      127   814163 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_1.png
+-rw-r--r--   0     1001      127   714248 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_1b.png
+-rw-r--r--   0     1001      127   783296 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_2.png
+-rw-r--r--   0     1001      127   711826 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_3.png
+-rw-r--r--   0     1001      127   713875 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_4.png
+-rw-r--r--   0     1001      127   704350 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_5.png
+-rw-r--r--   0     1001      127   703032 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_cleaning_6.png
+-rw-r--r--   0     1001      127   197015 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_colour.png
+-rw-r--r--   0     1001      127   169923 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_decomposed.png
+-rw-r--r--   0     1001      127   286652 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_dual.png
+-rw-r--r--   0     1001      127   169332 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_example.png
+-rw-r--r--   0     1001      127   140961 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/graph_simple.png
+-rw-r--r--   0     1001      127   291560 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/intro_mixed_uses.png
+-rw-r--r--   0     1001      127   387283 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/images/intro_segment_harmonic.png
+-rw-r--r--   0     1001      127    35386 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/logos/cityseer_logo_light_red.png
+-rw-r--r--   0     1001      127    31349 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/logos/cityseer_logo_white.png
+-rw-r--r--   0     1001      127      174 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/manifest.webmanifest
+-rw-r--r--   0     1001      127       22 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/public/robots.txt
+-rw-r--r--   0     1001      127     1378 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/bib/mendeley.bib
+-rw-r--r--   0     1001      127    35885 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_deep_blue.png
+-rw-r--r--   0     1001      127    35841 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_deep_red.png
+-rw-r--r--   0     1001      127    35913 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_light_blue.png
+-rw-r--r--   0     1001      127    35386 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_light_red.png
+-rw-r--r--   0     1001      127    31349 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_white.png
+-rw-r--r--   0     1001      127    35386 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/logo.png
+-rw-r--r--   0     1001      127    17306 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/assets/logos/round_logo.png
+-rw-r--r--   0     1001      127      929 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/components/ArXivLink.vue
+-rw-r--r--   0     1001      127      154 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/components/Footer.astro
+-rw-r--r--   0     1001      127     4286 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/components/NavColumn.vue
+-rw-r--r--   0     1001      127      394 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/components/RepoLink.astro
+-rw-r--r--   0     1001      127      192 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/components/StripeTitle.astro
+-rw-r--r--   0     1001      127       38 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/env.d.ts
+-rw-r--r--   0     1001      127    17305 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/favicon.png
+-rw-r--r--   0     1001      127     1897 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/layouts/CommonLayout.astro
+-rw-r--r--   0     1001      127     1899 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/layouts/PageLayout.astro
+-rw-r--r--   0     1001      127     1447 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/attribution.md
+-rw-r--r--   0     1001      127     2530 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/examples.md
+-rw-r--r--   0     1001      127    13667 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/guide.md
+-rw-r--r--   0     1001      127     2997 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/index.astro
+-rw-r--r--   0     1001      127    17162 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/intro.md
+-rw-r--r--   0     1001      127    38733 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/metrics/layers.md
+-rw-r--r--   0     1001      127    23894 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/metrics/networks.md
+-rw-r--r--   0     1001      127     9296 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/metrics/observe.md
+-rw-r--r--   0     1001      127    13330 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/metrics/visibility.md
+-rw-r--r--   0     1001      127    66320 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/rustalgos/rustalgos.md
+-rw-r--r--   0     1001      127    26530 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/tools/graphs.md
+-rw-r--r--   0     1001      127    31931 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/tools/io.md
+-rw-r--r--   0     1001      127    12403 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/tools/mock.md
+-rw-r--r--   0     1001      127    32612 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/tools/plot.md
+-rw-r--r--   0     1001      127    21336 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/pages/tools/util.md
+-rw-r--r--   0     1001      127     2826 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/styles/tailwind.css
+-rw-r--r--   0     1001      127     1718 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/src/styles/yapper.css
+-rw-r--r--   0     1001      127     1225 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/tailwind.config.cjs
+-rw-r--r--   0     1001      127      246 2023-12-31 13:53:03.000000 cityseer-4.9.0/docs/tsconfig.json
+-rw-r--r--   0     1001      127   176582 2023-12-31 13:53:03.000000 cityseer-4.9.0/pdm.lock
+-rw-r--r--   0     1001      127      187 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/__init__.py
+-rw-r--r--   0     1001      127     2200 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/config.py
+-rw-r--r--   0     1001      127       71 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/metrics/__init__.py
+-rw-r--r--   0     1001      127    35286 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/metrics/layers.py
+-rw-r--r--   0     1001      127    22688 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/metrics/networks.py
+-rw-r--r--   0     1001      127    15944 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/metrics/observe.py
+-rw-r--r--   0     1001      127    12277 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/metrics/visibility.py
+-rw-r--r--   0     1001      127    24631 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/rustalgos.pyi
+-rw-r--r--   0     1001      127       72 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/__init__.py
+-rw-r--r--   0     1001      127    74215 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/graphs.py
+-rw-r--r--   0     1001      127    47800 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/io.py
+-rw-r--r--   0     1001      127    14930 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/mock.py
+-rw-r--r--   0     1001      127    38188 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/plot.py
+-rw-r--r--   0     1001      127    24219 2023-12-31 13:53:03.000000 cityseer-4.9.0/pysrc/cityseer/tools/util.py
+-rw-r--r--   0     1001      127    43805 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/centrality.rs
+-rw-r--r--   0     1001      127     8810 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/common.rs
+-rw-r--r--   0     1001      127    37742 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/data.rs
+-rw-r--r--   0     1001      127    18460 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/diversity.rs
+-rw-r--r--   0     1001      127    25182 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/graph.rs
+-rw-r--r--   0     1001      127     2213 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/lib.rs
+-rw-r--r--   0     1001      127     7072 2023-12-31 13:53:03.000000 cityseer-4.9.0/src/viewshed.rs
+-rw-r--r--   0     1001      127    32065 2023-12-31 13:53:03.000000 cityseer-4.9.0/test.prof
+-rw-r--r--   0     1001      127        0 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/__init__.py
+-rw-r--r--   0     1001      127     3365 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/conftest.py
+-rw-r--r--   0     1001      127        0 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/metrics/__init__.py
+-rw-r--r--   0     1001      127    12322 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/metrics/test_layers.py
+-rw-r--r--   0     1001      127     7856 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/metrics/test_networks.py
+-rw-r--r--   0     1001      127      684 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/metrics/test_visibility.py
+-rw-r--r--   0     1001      127        0 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/rustalgos/__init__.py
+-rw-r--r--   0     1001      127    37355 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/rustalgos/test_centrality.py
+-rw-r--r--   0     1001      127     9660 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/rustalgos/test_common.py
+-rw-r--r--   0     1001      127    22447 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/rustalgos/test_data.py
+-rw-r--r--   0     1001      127     8200 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/rustalgos/test_diversity.py
+-rw-r--r--   0     1001      127     4389 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/test_performance.py
+-rw-r--r--   0     1001      127        0 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/tools/__init__.py
+-rw-r--r--   0     1001      127    26130 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/tools/test_graphs.py
+-rw-r--r--   0     1001      127    36153 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/tools/test_io.py
+-rw-r--r--   0     1001      127     3594 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/tools/test_mock.py
+-rw-r--r--   0     1001      127     6859 2023-12-31 13:53:03.000000 cityseer-4.9.0/tests/tools/test_util.py
+-rw-r--r--   0     1001      127    14400 2023-12-31 13:53:03.000000 cityseer-4.9.0/Cargo.lock
+-rw-r--r--   0     1001      127     5691 2023-12-31 13:53:03.000000 cityseer-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0     6250 1970-01-01 00:00:00.000000 cityseer-4.9.0/PKG-INFO
```

### Comparing `cityseer-4.8.1/Cargo.toml` & `cityseer-4.9.0/Cargo.toml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/ISSUE_TEMPLATE/feature_request.md` & `cityseer-4.9.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/release-drafter.yml` & `cityseer-4.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/workflows/firebase-hosting-merge.yml` & `cityseer-4.9.0/.github/workflows/firebase-hosting-merge.yml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/workflows/firebase-hosting-pull-request.yml` & `cityseer-4.9.0/.github/workflows/firebase-hosting-pull-request.yml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/workflows/publish_package.yml` & `cityseer-4.9.0/.github/workflows/publish_package.yml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.github/workflows/publish_package_dev.yml` & `cityseer-4.9.0/.github/workflows/publish_package_dev.yml`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.gitignore` & `cityseer-4.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/.vscode/settings.json` & `cityseer-4.9.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/LICENSE.txt` & `cityseer-4.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/README.md` & `cityseer-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/coverage.lcov` & `cityseer-4.9.0/coverage.lcov`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/.eslintrc.cjs` & `cityseer-4.9.0/docs/.eslintrc.cjs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/astro.config.mjs` & `cityseer-4.9.0/docs/astro.config.mjs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/firebase.json` & `cityseer-4.9.0/docs/firebase.json`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/generate_docs.py` & `cityseer-4.9.0/docs/generate_docs.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/package-lock.json` & `cityseer-4.9.0/docs/package-lock.json`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/package.json` & `cityseer-4.9.0/docs/package.json`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/pdoc_templates/module.html.jinja2` & `cityseer-4.9.0/docs/pdoc_templates/module.html.jinja2`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/plots/matplotlibrc` & `cityseer-4.9.0/docs/plots/matplotlibrc`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/plots/plots.py` & `cityseer-4.9.0/docs/plots/plots.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/favicons/192.png` & `cityseer-4.9.0/docs/public/favicons/192.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/favicons/512.png` & `cityseer-4.9.0/docs/public/favicons/512.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/favicons/apple-touch-icon.png` & `cityseer-4.9.0/docs/public/favicons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/favicons/favicon.ico` & `cityseer-4.9.0/docs/public/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/favicons/icon.svg` & `cityseer-4.9.0/docs/public/favicons/icon.svg`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/assignment.png` & `cityseer-4.9.0/docs/public/images/assignment.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/assignment_decomposed.png` & `cityseer-4.9.0/docs/public/images/assignment_decomposed.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/assignment_plot.png` & `cityseer-4.9.0/docs/public/images/assignment_plot.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/betas.png` & `cityseer-4.9.0/docs/public/images/betas.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph.png` & `cityseer-4.9.0/docs/public/images/graph.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_1.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_1.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_1b.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_1b.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_2.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_2.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_3.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_3.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_4.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_4.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_5.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_5.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_cleaning_6.png` & `cityseer-4.9.0/docs/public/images/graph_cleaning_6.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_colour.png` & `cityseer-4.9.0/docs/public/images/graph_colour.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_decomposed.png` & `cityseer-4.9.0/docs/public/images/graph_decomposed.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_dual.png` & `cityseer-4.9.0/docs/public/images/graph_dual.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_example.png` & `cityseer-4.9.0/docs/public/images/graph_example.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/graph_simple.png` & `cityseer-4.9.0/docs/public/images/graph_simple.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/intro_mixed_uses.png` & `cityseer-4.9.0/docs/public/images/intro_mixed_uses.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/images/intro_segment_harmonic.png` & `cityseer-4.9.0/docs/public/images/intro_segment_harmonic.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/logos/cityseer_logo_light_red.png` & `cityseer-4.9.0/docs/public/logos/cityseer_logo_light_red.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/public/logos/cityseer_logo_white.png` & `cityseer-4.9.0/docs/public/logos/cityseer_logo_white.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/bib/mendeley.bib` & `cityseer-4.9.0/docs/src/assets/bib/mendeley.bib`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_deep_blue.png` & `cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_deep_blue.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_deep_red.png` & `cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_deep_red.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_light_blue.png` & `cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_light_blue.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_light_red.png` & `cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_light_red.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/cityseer_logo_white.png` & `cityseer-4.9.0/docs/src/assets/logos/cityseer_logo_white.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/logo.png` & `cityseer-4.9.0/docs/src/assets/logos/logo.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/assets/logos/round_logo.png` & `cityseer-4.9.0/docs/src/assets/logos/round_logo.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/components/ArXivLink.vue` & `cityseer-4.9.0/docs/src/components/ArXivLink.vue`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/components/NavColumn.vue` & `cityseer-4.9.0/docs/src/components/NavColumn.vue`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/favicon.png` & `cityseer-4.9.0/docs/src/favicon.png`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/layouts/CommonLayout.astro` & `cityseer-4.9.0/docs/src/layouts/CommonLayout.astro`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/layouts/PageLayout.astro` & `cityseer-4.9.0/docs/src/layouts/PageLayout.astro`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/attribution.md` & `cityseer-4.9.0/docs/src/pages/attribution.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/examples.md` & `cityseer-4.9.0/docs/src/pages/examples.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/guide.md` & `cityseer-4.9.0/docs/src/pages/guide.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/index.astro` & `cityseer-4.9.0/docs/src/pages/index.astro`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/intro.md` & `cityseer-4.9.0/docs/src/pages/intro.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/metrics/layers.md` & `cityseer-4.9.0/docs/src/pages/metrics/layers.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/metrics/networks.md` & `cityseer-4.9.0/docs/src/pages/metrics/networks.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/metrics/observe.md` & `cityseer-4.9.0/docs/src/pages/metrics/observe.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/metrics/visibility.md` & `cityseer-4.9.0/docs/src/pages/metrics/visibility.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/rustalgos/rustalgos.md` & `cityseer-4.9.0/docs/src/pages/rustalgos/rustalgos.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -2722,30 +2722,30 @@
 </div>
 </div>
 
 </div>
 
  
 
-<span class="name">node_lives</span><span class="annotation">: list[bool]</span>
+<span class="name">node_xs</span><span class="annotation">: list[float]</span>
 
 
  
 
-<span class="name">node_ys</span><span class="annotation">: list[float]</span>
+<span class="name">node_xys</span><span class="annotation">: list[tuple[float, float]]</span>
 
 
  
 
-<span class="name">node_xys</span><span class="annotation">: list[tuple[float, float]]</span>
+<span class="name">node_lives</span><span class="annotation">: list[bool]</span>
 
 
  
 
-<span class="name">node_xs</span><span class="annotation">: list[float]</span>
+<span class="name">node_ys</span><span class="annotation">: list[float]</span>
 
 
  
 </div>
 
 
 <div class="class">
```

### Comparing `cityseer-4.8.1/docs/src/pages/tools/graphs.md` & `cityseer-4.9.0/docs/src/pages/tools/graphs.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/tools/io.md` & `cityseer-4.9.0/docs/src/pages/tools/io.md`

 * *Files 0% similar despite different names*

```diff
@@ -328,15 +328,15 @@
   <span class="pt">(</span>
   <div class="param">
     <span class="pn">poly_geom</span>
     <span class="pc">:</span>
     <span class="pa"> shapely.geometry.polygon.Polygon</span>
   </div>
   <div class="param">
-    <span class="pn">poly_epsg_code</span>
+    <span class="pn">poly_crs_code</span>
     <span class="pc">:</span>
     <span class="pa"> int | str = 4326</span>
   </div>
   <div class="param">
     <span class="pn">to_crs_code</span>
     <span class="pc">:</span>
     <span class="pa"> int | str | None = None</span>
@@ -403,15 +403,15 @@
   <div class="desc">
 
  A shapely Polygon representing the extents for which to fetch the OSM network.</div>
 </div>
 
 <div class="param-set">
   <div class="def">
-    <div class="name">poly_epsg_code</div>
+    <div class="name">poly_crs_code</div>
     <div class="type">int | str</div>
   </div>
   <div class="desc">
 
  An integer representing a valid EPSG code for the provided polygon. For example, [4326](https://epsg.io/4326) if using WGS lng / lat, or [27700](https://epsg.io/27700) if using the British National Grid.</div>
 </div>
```

### Comparing `cityseer-4.8.1/docs/src/pages/tools/mock.md` & `cityseer-4.9.0/docs/src/pages/tools/mock.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/tools/plot.md` & `cityseer-4.9.0/docs/src/pages/tools/plot.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/pages/tools/util.md` & `cityseer-4.9.0/docs/src/pages/tools/util.md`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/styles/tailwind.css` & `cityseer-4.9.0/docs/src/styles/tailwind.css`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/src/styles/yapper.css` & `cityseer-4.9.0/docs/src/styles/yapper.css`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/docs/tailwind.config.cjs` & `cityseer-4.9.0/docs/tailwind.config.cjs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pdm.lock` & `cityseer-4.9.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/config.py` & `cityseer-4.9.0/pysrc/cityseer/config.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/metrics/layers.py` & `cityseer-4.9.0/pysrc/cityseer/metrics/layers.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/metrics/networks.py` & `cityseer-4.9.0/pysrc/cityseer/metrics/networks.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/metrics/observe.py` & `cityseer-4.9.0/pysrc/cityseer/metrics/observe.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/metrics/visibility.py` & `cityseer-4.9.0/pysrc/cityseer/metrics/visibility.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/rustalgos.pyi` & `cityseer-4.9.0/pysrc/cityseer/rustalgos.pyi`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/tools/graphs.py` & `cityseer-4.9.0/pysrc/cityseer/tools/graphs.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/tools/io.py` & `cityseer-4.9.0/pysrc/cityseer/tools/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -212,15 +212,15 @@
         osm_response.raise_for_status()
 
     return osm_response
 
 
 def osm_graph_from_poly(
     poly_geom: geometry.Polygon,
-    poly_epsg_code: int | str = 4326,
+    poly_crs_code: int | str = 4326,
     to_crs_code: int | str | None = None,
     custom_request: str | None = None,
     simplify: bool = True,
     crawl_consolidate_dist: int = 12,
     parallel_consolidate_dist: int = 15,
     contains_buffer_dist: int = 50,
     iron_edges: bool = True,
@@ -234,15 +234,15 @@
     retrieve the OSM response and will automatically unpack this into a `networkX` graph. Simplification will be applied
     by default, but can be disabled.
 
     Parameters
     ----------
     poly_geom: shapely.Polygon
         A shapely Polygon representing the extents for which to fetch the OSM network.
-    poly_epsg_code: int | str
+    poly_crs_code: int | str
         An integer representing a valid EPSG code for the provided polygon. For example, [4326](https://epsg.io/4326) if
         using WGS lng / lat, or [27700](https://epsg.io/27700) if using the British National Grid.
     to_crs_code: int | str
         An optional integer representing a valid EPSG code for the generated network returned from this function. If
         this parameter is provided, then the network will be converted to the specified EPSG coordinate reference
         system. If not provided, then the OSM network will be projected into a local UTM coordinate reference system.
     buffer_dist: int
@@ -301,20 +301,20 @@
     out body;
     >;
     out qt;
     '''
     ```
 
     """
-    if poly_epsg_code is not None and not isinstance(poly_epsg_code, (int, str)):  # type: ignore
-        raise TypeError('Please provide "poly_epsg_code" parameter as int or str')
+    if poly_crs_code is not None and not isinstance(poly_crs_code, (int, str)):  # type: ignore
+        raise TypeError('Please provide "poly_crs_code" parameter as int or str')
     if to_crs_code is not None and not isinstance(to_crs_code, (int, str)):
         raise TypeError('Please provide "to_crs_code" parameter as int or str')
     # format for OSM query
-    in_transformer = Transformer.from_crs(poly_epsg_code, 4326, always_xy=True)
+    in_transformer = Transformer.from_crs(poly_crs_code, 4326, always_xy=True)
     coords = [in_transformer.transform(lng, lat) for lng, lat in poly_geom.exterior.coords]
     geom_osm = str.join(" ", [f"{lat} {lng}" for lng, lat in coords])
     if custom_request is not None:
         if "geom_osm" not in custom_request:
             raise ValueError(
                 'The provided custom_request does not contain an f-string interpolation bracket for "geom_osm". '
                 "This key is required for interpolating the generated geometry into the request."
```

### Comparing `cityseer-4.8.1/pysrc/cityseer/tools/mock.py` & `cityseer-4.9.0/pysrc/cityseer/tools/mock.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/tools/plot.py` & `cityseer-4.9.0/pysrc/cityseer/tools/plot.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pysrc/cityseer/tools/util.py` & `cityseer-4.9.0/pysrc/cityseer/tools/util.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/centrality.rs` & `cityseer-4.9.0/src/centrality.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/common.rs` & `cityseer-4.9.0/src/common.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/data.rs` & `cityseer-4.9.0/src/data.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/diversity.rs` & `cityseer-4.9.0/src/diversity.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/graph.rs` & `cityseer-4.9.0/src/graph.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/lib.rs` & `cityseer-4.9.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/src/viewshed.rs` & `cityseer-4.9.0/src/viewshed.rs`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/test.prof` & `cityseer-4.9.0/test.prof`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/conftest.py` & `cityseer-4.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/metrics/test_layers.py` & `cityseer-4.9.0/tests/metrics/test_layers.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/metrics/test_networks.py` & `cityseer-4.9.0/tests/metrics/test_networks.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/metrics/test_visibility.py` & `cityseer-4.9.0/tests/metrics/test_visibility.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/rustalgos/test_centrality.py` & `cityseer-4.9.0/tests/rustalgos/test_centrality.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/rustalgos/test_common.py` & `cityseer-4.9.0/tests/rustalgos/test_common.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/rustalgos/test_data.py` & `cityseer-4.9.0/tests/rustalgos/test_data.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/rustalgos/test_diversity.py` & `cityseer-4.9.0/tests/rustalgos/test_diversity.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/test_performance.py` & `cityseer-4.9.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/tools/test_graphs.py` & `cityseer-4.9.0/tests/tools/test_graphs.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/tools/test_io.py` & `cityseer-4.9.0/tests/tools/test_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     assert isinstance(network_from_wgs, nx.MultiGraph)
     assert len(network_from_wgs.nodes) > 0
     assert len(network_from_wgs.edges) > 0
     # check that from CRS conversions are working
     # 32630 corresponds to UTM 30N
     poly_utm, utm_epsg = io.buffered_point_poly(LNG, LAT, BUFFER, projected=True)
     assert utm_epsg == 32630
-    network_from_utm = io.osm_graph_from_poly(poly_utm, poly_epsg_code=utm_epsg, simplify=False)
+    network_from_utm = io.osm_graph_from_poly(poly_utm, poly_crs_code=utm_epsg, simplify=False)
     # visual check for debugging
     # plot.plot_nx(network_from_utm)
     assert isinstance(network_from_utm, nx.MultiGraph)
     assert len(network_from_utm.nodes) > 0
     assert len(network_from_utm.edges) > 0
     # check that networks match
     assert list(network_from_utm.nodes) == list(network_from_wgs.nodes)
```

### Comparing `cityseer-4.8.1/tests/tools/test_mock.py` & `cityseer-4.9.0/tests/tools/test_mock.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/tests/tools/test_util.py` & `cityseer-4.9.0/tests/tools/test_util.py`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/Cargo.lock` & `cityseer-4.9.0/Cargo.lock`

 * *Files identical despite different names*

### Comparing `cityseer-4.8.1/pyproject.toml` & `cityseer-4.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cityseer"
-version = '4.8.1'
+version = '4.9.0'
 description = "Computational tools for network-based pedestrian-scale urban analysis"
 readme = "README.md"
 requires-python = ">=3.10, <3.12"
 license = { text = "AGPL-3.0" }
 keywords = [
   "network-topology",
   "numpy",
```

### Comparing `cityseer-4.8.1/PKG-INFO` & `cityseer-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cityseer
-Version: 4.8.1
+Version: 4.9.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Rust
 Requires-Dist: matplotlib >=3.5.1
 Requires-Dist: networkx >=2.8.8
 Requires-Dist: pyproj >=3.3.0
 Requires-Dist: requests >=2.27.1
```

