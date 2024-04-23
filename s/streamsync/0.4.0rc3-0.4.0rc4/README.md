# Comparing `tmp/streamsync-0.4.0rc3.tar.gz` & `tmp/streamsync-0.4.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamsync-0.4.0rc3.tar", max compression
+gzip compressed data, was "streamsync-0.4.0rc4.tar", max compression
```

## Comparing `streamsync-0.4.0rc3.tar` & `streamsync-0.4.0rc4.tar`

### file list

```diff
@@ -1,151 +1,151 @@
--rw-r--r--   0        0        0    11323 2024-03-21 18:52:51.360674 streamsync-0.4.0rc3/LICENSE.txt
--rw-r--r--   0        0        0     3981 2024-03-21 18:52:51.360674 streamsync-0.4.0rc3/README.md
--rw-r--r--   0        0        0     1766 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/pyproject.toml
--rw-r--r--   0        0        0     2763 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/__init__.py
--rw-r--r--   0        0        0    29945 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_runner.py
--rw-r--r--   0        0        0     1035 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/default/main.py
--rw-r--r--   0        0        0      416 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/default/static/README.md
--rw-r--r--   0        0        0     3780 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/default/static/favicon.png
--rw-r--r--   0        0        0     4848 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/default/ui.json
--rw-r--r--   0        0        0      475 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/Dockerfile
--rw-r--r--   0        0        0     1250 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/assets/main_df.csv
--rw-r--r--   0        0        0     2818 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/assets/story.txt
--rw-r--r--   0        0        0     4775 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/main.py
--rw-r--r--   0        0        0        0 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/requirements.txt
--rw-r--r--   0        0        0      628 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/README.md
--rw-r--r--   0        0        0     3780 2024-03-21 18:52:51.468675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/favicon.png
--rw-r--r--   0        0        0   179279 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/pigeon1.jpg
--rw-r--r--   0        0        0     1460 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/test_app.py
--rw-r--r--   0        0        0    36666 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/app_templates/hello/ui.json
--rw-r--r--   0        0        0     4381 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/command_line.py
--rw-r--r--   0        0        0    48455 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/core.py
--rw-r--r--   0        0        0     7230 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/core_ui.py
--rw-r--r--   0        0        0       30 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/mypy.ini
--rw-r--r--   0        0        0        0 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/py.typed
--rw-r--r--   0        0        0    17879 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/serve.py
--rw-r--r--   0        0        0     3585 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/ss_types.py
--rw-r--r--   0        0        0     8966 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/Arrow.dom-d8f7f33e.js
--rw-r--r--   0        0        0  3206609 2024-03-21 18:54:27.801066 streamsync-0.4.0rc3/src/streamsync/static/assets/BuilderApp-6c29fc91.js
--rw-r--r--   0        0        0   263851 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/BuilderApp-9cf67088.css
--rw-r--r--   0        0        0     7530 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/ComponentRenderer-82ebfa88.js
--rw-r--r--   0        0        0    14970 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/ComponentRenderer-a2494844.css
--rw-r--r--   0        0        0   309828 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/Inter-Regular-41ab0f70.ttf
--rw-r--r--   0        0        0    98868 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/Inter-Regular-d612f121.woff2
--rw-r--r--   0        0        0    14409 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/abap-b029dff1.js
--rw-r--r--   0        0        0     4198 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/apex-3c83662c.js
--rw-r--r--   0        0        0     1094 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/azcli-f1f7c576.js
--rw-r--r--   0        0        0     2091 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/bat-86aea46a.js
--rw-r--r--   0        0        0     2782 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/bicep-75c0c4d5.js
--rw-r--r--   0        0        0     2431 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/cameligo-8043f913.js
--rw-r--r--   0        0        0     9889 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/clojure-73642b02.js
--rw-r--r--   0        0        0    73464 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/codicon-79f233d0.ttf
--rw-r--r--   0        0        0     3836 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/coffee-a18badcf.js
--rw-r--r--   0        0        0     5724 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/cpp-4034161e.js
--rw-r--r--   0        0        0     4770 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/csharp-49cbf0d2.js
--rw-r--r--   0        0        0     1665 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/csp-d207cac4.js
--rw-r--r--   0        0        0     4756 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/css-74326df0.js
--rw-r--r--   0        0        0    33820 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/cssMode-dc15036c.js
--rw-r--r--   0        0        0     3631 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/cypher-49f5f839.js
--rw-r--r--   0        0        0     4496 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/dart-84b7c6b4.js
--rw-r--r--   0        0        0     2115 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/dockerfile-bbf114b2.js
--rw-r--r--   0        0        0     5588 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/ecl-15840f49.js
--rw-r--r--   0        0        0    10503 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/elixir-e479e18e.js
--rw-r--r--   0        0        0     2056 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/flow9-42a61225.js
--rw-r--r--   0        0        0    16478 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/freemarker2-c56b9d61.js
--rw-r--r--   0        0        0     3229 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/fsharp-8abe6da0.js
--rw-r--r--   0        0        0     2903 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/go-8759e9f7.js
--rw-r--r--   0        0        0     2506 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/graphql-387d549c.js
--rw-r--r--   0        0        0     7156 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/handlebars-1fc6855b.js
--rw-r--r--   0        0        0     3836 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/hcl-a88f331a.js
--rw-r--r--   0        0        0     5396 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/html-1e46783a.js
--rw-r--r--   0        0        0    34371 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/htmlMode-82eab562.js
--rw-r--r--   0        0        0  1733993 2024-03-21 18:54:27.801066 streamsync-0.4.0rc3/src/streamsync/static/assets/index-165490a0.js
--rw-r--r--   0        0        0   201777 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/index-59f5827a.js
--rw-r--r--   0        0        0   306642 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/index-b222671e.js
--rw-r--r--   0        0        0   330649 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/index-b7043f95.css
--rw-r--r--   0        0        0     5725 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/index.esm-1f2a7de3.js
--rw-r--r--   0        0        0     1347 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/ini-18bf1153.js
--rw-r--r--   0        0        0     3467 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/java-000a6283.js
--rw-r--r--   0        0        0     1292 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/javascript-a891c4c5.js
--rw-r--r--   0        0        0    39861 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/jsonMode-7dc8e9c5.js
--rw-r--r--   0        0        0     7395 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/julia-0026391c.js
--rw-r--r--   0        0        0     3685 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/kotlin-06ee8898.js
--rw-r--r--   0        0        0     4144 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/less-dd86a68c.js
--rw-r--r--   0        0        0     2683 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/lexon-8d4b0444.js
--rw-r--r--   0        0        0     4342 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/liquid-79207f1f.js
--rw-r--r--   0        0        0      312 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/logo-38e5451f.svg
--rw-r--r--   0        0        0     2369 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/lua-9adddcd9.js
--rw-r--r--   0        0        0     3063 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/m3-aa2dcf72.js
--rw-r--r--   0        0        0  1267743 2024-03-21 18:54:27.801066 streamsync-0.4.0rc3/src/streamsync/static/assets/mapbox-gl-6d4978b5.js
--rw-r--r--   0        0        0     4034 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/markdown-0f073a3a.js
--rw-r--r--   0        0        0    41341 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/marked.esm-0bd9b835.js
--rw-r--r--   0        0        0     5247 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/mdx-d684260e.js
--rw-r--r--   0        0        0     2825 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/mips-bdd96c5a.js
--rw-r--r--   0        0        0     5158 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/msdax-1ac55115.js
--rw-r--r--   0        0        0    11520 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/mysql-b530c105.js
--rw-r--r--   0        0        0     2648 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/objective-c-951ded7b.js
--rw-r--r--   0        0        0      383 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-4-side-5ad25975.svg
--rw-r--r--   0        0        0      218 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-bottom-side-af43d05a.svg
--rw-r--r--   0        0        0      218 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-left-side-92febd90.svg
--rw-r--r--   0        0        0      218 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-right-side-520b5d5f.svg
--rw-r--r--   0        0        0      218 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-top-side-a82fabbc.svg
--rw-r--r--   0        0        0      273 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-x-side-6ca00bcf.svg
--rw-r--r--   0        0        0      273 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/padding-y-side-278dc262.svg
--rw-r--r--   0        0        0     3241 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/pascal-7442fd46.js
--rw-r--r--   0        0        0     2246 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/pascaligo-385edc0e.js
--rw-r--r--   0        0        0     8501 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/perl-d5fb326c.js
--rw-r--r--   0        0        0    13710 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/pgsql-2d7db25a.js
--rw-r--r--   0        0        0     8273 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/php-1daff147.js
--rw-r--r--   0        0        0     1929 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/pla-1b3e1614.js
--rw-r--r--   0        0        0  3704150 2024-03-21 18:54:27.801066 streamsync-0.4.0rc3/src/streamsync/static/assets/plotly.min-95fb3915.js
--rw-r--r--   0        0        0     8102 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/postiats-9db13649.js
--rw-r--r--   0        0        0    17185 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/powerquery-4c428232.js
--rw-r--r--   0        0        0     3515 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/powershell-d3380668.js
--rw-r--r--   0        0        0     9292 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/protobuf-941cf3e8.js
--rw-r--r--   0        0        0     5074 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/pug-cfe384ef.js
--rw-r--r--   0        0        0     3999 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/python-bbfdef2a.js
--rw-r--r--   0        0        0     3181 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/qsharp-e125d03f.js
--rw-r--r--   0        0        0     3377 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/r-e0a01d4f.js
--rw-r--r--   0        0        0     9160 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/razor-edf02117.js
--rw-r--r--   0        0        0     3802 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/redis-d0a12fea.js
--rw-r--r--   0        0        0    12046 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/redshift-a163b94a.js
--rw-r--r--   0        0        0   525744 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-3d7b8a45.eot
--rw-r--r--   0        0        0   224116 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-793349c8.woff
--rw-r--r--   0        0        0   163200 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-7c1b0867.woff2
--rw-r--r--   0        0        0  2460531 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-931f98fd.svg
--rw-r--r--   0        0        0   525572 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-b074b4f2.ttf
--rw-r--r--   0        0        0     4139 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/restructuredtext-5a906e1a.js
--rw-r--r--   0        0        0     8750 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/ruby-05b021bf.js
--rw-r--r--   0        0        0     4406 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/rust-3d80982c.js
--rw-r--r--   0        0        0     2075 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/sb-2020a5af.js
--rw-r--r--   0        0        0     7564 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/scala-54469b4b.js
--rw-r--r--   0        0        0     2013 2024-03-21 18:54:27.761066 streamsync-0.4.0rc3/src/streamsync/static/assets/scheme-ff6e5671.js
--rw-r--r--   0        0        0     6655 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/scss-77902feb.js
--rw-r--r--   0        0        0   202279 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/serialization-0c0131b6.js
--rw-r--r--   0        0        0     3319 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/shell-3c06def6.js
--rw-r--r--   0        0        0    18843 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/solidity-3d59d6a7.js
--rw-r--r--   0        0        0     3010 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/sophia-12eb7ba8.js
--rw-r--r--   0        0        0     2798 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/sparql-e42fb28a.js
--rw-r--r--   0        0        0    10543 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/sql-d30fd9fd.js
--rw-r--r--   0        0        0     7645 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/st-0857f583.js
--rw-r--r--   0        0        0     5417 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/swift-f0a706dd.js
--rw-r--r--   0        0        0     7849 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/systemverilog-0cfd4211.js
--rw-r--r--   0        0        0     3817 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/tcl-7df3c0c5.js
--rw-r--r--   0        0        0    23320 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/tsMode-d172b673.js
--rw-r--r--   0        0        0     6219 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/twig-f894aab2.js
--rw-r--r--   0        0        0     5789 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/typescript-31544fa1.js
--rw-r--r--   0        0        0     6037 2024-03-21 18:54:27.765066 streamsync-0.4.0rc3/src/streamsync/static/assets/vb-39a025f4.js
--rw-r--r--   0        0        0   839593 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/assets/vega-embed.module-ab6e1af3.js
--rw-r--r--   0        0        0     7575 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/wgsl-afa2396f.js
--rw-r--r--   0        0        0     2790 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/xml-1904b31e.js
--rw-r--r--   0        0        0     4397 2024-03-21 18:54:27.769066 streamsync-0.4.0rc3/src/streamsync/static/assets/yaml-ea97fa90.js
--rw-r--r--   0        0        0     3780 2024-03-21 18:54:24.837054 streamsync-0.4.0rc3/src/streamsync/static/favicon.png
--rw-r--r--   0        0        0     3342 2024-03-21 18:54:27.797066 streamsync-0.4.0rc3/src/streamsync/static/index.html
--rw-r--r--   0        0        0  1784530 2024-03-21 18:54:27.973067 streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/css.worker.bundle.js
--rw-r--r--   0        0        0   482889 2024-03-21 18:54:27.893067 streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/editor.worker.bundle.js
--rw-r--r--   0        0        0  1184272 2024-03-21 18:54:28.037067 streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/html.worker.bundle.js
--rw-r--r--   0        0        0   762716 2024-03-21 18:54:28.077067 streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/json.worker.bundle.js
--rw-r--r--   0        0        0  9667054 2024-03-21 18:54:28.605069 streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/ts.worker.bundle.js
--rw-r--r--   0        0        0    58171 2024-03-21 18:54:34.373093 streamsync-0.4.0rc3/src/streamsync/ui.py
--rw-r--r--   0        0        0     5853 2024-03-21 18:52:51.472675 streamsync-0.4.0rc3/src/streamsync/ui_manager.py
--rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 streamsync-0.4.0rc3/PKG-INFO
+-rw-r--r--   0        0        0    11323 2024-03-27 20:08:36.781568 streamsync-0.4.0rc4/LICENSE.txt
+-rw-r--r--   0        0        0     3981 2024-03-27 20:08:36.781568 streamsync-0.4.0rc4/README.md
+-rw-r--r--   0        0        0     1766 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     2792 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/__init__.py
+-rw-r--r--   0        0        0    29945 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_runner.py
+-rw-r--r--   0        0        0     1035 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/default/main.py
+-rw-r--r--   0        0        0      416 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/default/static/README.md
+-rw-r--r--   0        0        0     3780 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/default/static/favicon.png
+-rw-r--r--   0        0        0     4848 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/default/ui.json
+-rw-r--r--   0        0        0      475 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/Dockerfile
+-rw-r--r--   0        0        0     1250 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/assets/main_df.csv
+-rw-r--r--   0        0        0     2818 2024-03-27 20:08:36.889569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/assets/story.txt
+-rw-r--r--   0        0        0     4775 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/main.py
+-rw-r--r--   0        0        0        0 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/requirements.txt
+-rw-r--r--   0        0        0      628 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/README.md
+-rw-r--r--   0        0        0     3780 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/favicon.png
+-rw-r--r--   0        0        0   179279 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/pigeon1.jpg
+-rw-r--r--   0        0        0     1460 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/test_app.py
+-rw-r--r--   0        0        0    36666 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/app_templates/hello/ui.json
+-rw-r--r--   0        0        0     4381 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/command_line.py
+-rw-r--r--   0        0        0    48554 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/core.py
+-rw-r--r--   0        0        0     9052 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/core_ui.py
+-rw-r--r--   0        0        0       30 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/mypy.ini
+-rw-r--r--   0        0        0        0 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/py.typed
+-rw-r--r--   0        0        0    17879 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/serve.py
+-rw-r--r--   0        0        0     3585 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/ss_types.py
+-rw-r--r--   0        0        0     8966 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/Arrow.dom-d8f7f33e.js
+-rw-r--r--   0        0        0  3206657 2024-03-27 20:10:14.154514 streamsync-0.4.0rc4/src/streamsync/static/assets/BuilderApp-82d844f6.js
+-rw-r--r--   0        0        0   263851 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/BuilderApp-f68489e4.css
+-rw-r--r--   0        0        0     7561 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/ComponentRenderer-007280fe.js
+-rw-r--r--   0        0        0    14970 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/ComponentRenderer-08d5f1dc.css
+-rw-r--r--   0        0        0   309828 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/Inter-Regular-41ab0f70.ttf
+-rw-r--r--   0        0        0    98868 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/Inter-Regular-d612f121.woff2
+-rw-r--r--   0        0        0    14409 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/abap-b029dff1.js
+-rw-r--r--   0        0        0     4198 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/apex-3c83662c.js
+-rw-r--r--   0        0        0     1094 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/azcli-f1f7c576.js
+-rw-r--r--   0        0        0     2091 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/bat-86aea46a.js
+-rw-r--r--   0        0        0     2782 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/bicep-75c0c4d5.js
+-rw-r--r--   0        0        0     2431 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/cameligo-8043f913.js
+-rw-r--r--   0        0        0     9889 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/clojure-73642b02.js
+-rw-r--r--   0        0        0    73464 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/codicon-79f233d0.ttf
+-rw-r--r--   0        0        0     3836 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/coffee-a18badcf.js
+-rw-r--r--   0        0        0     5724 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/cpp-4034161e.js
+-rw-r--r--   0        0        0     4770 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/csharp-49cbf0d2.js
+-rw-r--r--   0        0        0     1665 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/csp-d207cac4.js
+-rw-r--r--   0        0        0     4756 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/css-74326df0.js
+-rw-r--r--   0        0        0    33820 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/cssMode-40a421b7.js
+-rw-r--r--   0        0        0     3631 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/cypher-49f5f839.js
+-rw-r--r--   0        0        0     4496 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/dart-84b7c6b4.js
+-rw-r--r--   0        0        0     2115 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/dockerfile-bbf114b2.js
+-rw-r--r--   0        0        0     5588 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/ecl-15840f49.js
+-rw-r--r--   0        0        0    10503 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/elixir-e479e18e.js
+-rw-r--r--   0        0        0     2056 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/flow9-42a61225.js
+-rw-r--r--   0        0        0    16478 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/freemarker2-ab7f8d00.js
+-rw-r--r--   0        0        0     3229 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/fsharp-8abe6da0.js
+-rw-r--r--   0        0        0     2903 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/go-8759e9f7.js
+-rw-r--r--   0        0        0     2506 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/graphql-387d549c.js
+-rw-r--r--   0        0        0     7156 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/handlebars-b7cc84e9.js
+-rw-r--r--   0        0        0     3836 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/hcl-a88f331a.js
+-rw-r--r--   0        0        0     5396 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/html-14f46deb.js
+-rw-r--r--   0        0        0    34371 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/htmlMode-4adc2b6d.js
+-rw-r--r--   0        0        0   306642 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/index-0d669be8.js
+-rw-r--r--   0        0        0  1733993 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/index-3137b44e.js
+-rw-r--r--   0        0        0   201777 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/index-59f5827a.js
+-rw-r--r--   0        0        0   330649 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/index-b7043f95.css
+-rw-r--r--   0        0        0     5725 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/index.esm-1f2a7de3.js
+-rw-r--r--   0        0        0     1347 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/ini-18bf1153.js
+-rw-r--r--   0        0        0     3467 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/java-000a6283.js
+-rw-r--r--   0        0        0     1292 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/javascript-18f19bfc.js
+-rw-r--r--   0        0        0    39861 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/jsonMode-be63eb4c.js
+-rw-r--r--   0        0        0     7395 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/julia-0026391c.js
+-rw-r--r--   0        0        0     3685 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/kotlin-06ee8898.js
+-rw-r--r--   0        0        0     4144 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/less-dd86a68c.js
+-rw-r--r--   0        0        0     2683 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/lexon-8d4b0444.js
+-rw-r--r--   0        0        0     4342 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/liquid-d7e3f977.js
+-rw-r--r--   0        0        0      312 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/logo-38e5451f.svg
+-rw-r--r--   0        0        0     2369 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/lua-9adddcd9.js
+-rw-r--r--   0        0        0     3063 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/m3-aa2dcf72.js
+-rw-r--r--   0        0        0  1267743 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/mapbox-gl-572acb0e.js
+-rw-r--r--   0        0        0     4034 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/markdown-0f073a3a.js
+-rw-r--r--   0        0        0    41341 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/marked.esm-0bd9b835.js
+-rw-r--r--   0        0        0     5247 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/mdx-2b91f7f9.js
+-rw-r--r--   0        0        0     2825 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/mips-bdd96c5a.js
+-rw-r--r--   0        0        0     5158 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/msdax-1ac55115.js
+-rw-r--r--   0        0        0    11520 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/mysql-b530c105.js
+-rw-r--r--   0        0        0     2648 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/objective-c-951ded7b.js
+-rw-r--r--   0        0        0      383 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-4-side-5ad25975.svg
+-rw-r--r--   0        0        0      218 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-bottom-side-af43d05a.svg
+-rw-r--r--   0        0        0      218 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-left-side-92febd90.svg
+-rw-r--r--   0        0        0      218 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-right-side-520b5d5f.svg
+-rw-r--r--   0        0        0      218 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-top-side-a82fabbc.svg
+-rw-r--r--   0        0        0      273 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-x-side-6ca00bcf.svg
+-rw-r--r--   0        0        0      273 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/padding-y-side-278dc262.svg
+-rw-r--r--   0        0        0     3241 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/pascal-7442fd46.js
+-rw-r--r--   0        0        0     2246 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/pascaligo-385edc0e.js
+-rw-r--r--   0        0        0     8501 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/perl-d5fb326c.js
+-rw-r--r--   0        0        0    13710 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/pgsql-2d7db25a.js
+-rw-r--r--   0        0        0     8273 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/php-1daff147.js
+-rw-r--r--   0        0        0     1929 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/pla-1b3e1614.js
+-rw-r--r--   0        0        0  3704150 2024-03-27 20:10:14.154514 streamsync-0.4.0rc4/src/streamsync/static/assets/plotly.min-d27e0f8d.js
+-rw-r--r--   0        0        0     8102 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/postiats-9db13649.js
+-rw-r--r--   0        0        0    17185 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/powerquery-4c428232.js
+-rw-r--r--   0        0        0     3515 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/powershell-d3380668.js
+-rw-r--r--   0        0        0     9292 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/protobuf-941cf3e8.js
+-rw-r--r--   0        0        0     5074 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/pug-cfe384ef.js
+-rw-r--r--   0        0        0     3999 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/python-a79eb30c.js
+-rw-r--r--   0        0        0     3181 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/qsharp-e125d03f.js
+-rw-r--r--   0        0        0     3377 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/r-e0a01d4f.js
+-rw-r--r--   0        0        0     9160 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/razor-673842c1.js
+-rw-r--r--   0        0        0     3802 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/redis-d0a12fea.js
+-rw-r--r--   0        0        0    12046 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/redshift-a163b94a.js
+-rw-r--r--   0        0        0   525744 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-3d7b8a45.eot
+-rw-r--r--   0        0        0   224116 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-793349c8.woff
+-rw-r--r--   0        0        0   163200 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-7c1b0867.woff2
+-rw-r--r--   0        0        0  2460531 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-931f98fd.svg
+-rw-r--r--   0        0        0   525572 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-b074b4f2.ttf
+-rw-r--r--   0        0        0     4139 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/restructuredtext-5a906e1a.js
+-rw-r--r--   0        0        0     8750 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/ruby-05b021bf.js
+-rw-r--r--   0        0        0     4406 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/rust-3d80982c.js
+-rw-r--r--   0        0        0     2075 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/sb-2020a5af.js
+-rw-r--r--   0        0        0     7564 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/scala-54469b4b.js
+-rw-r--r--   0        0        0     2013 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/scheme-ff6e5671.js
+-rw-r--r--   0        0        0     6655 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/scss-77902feb.js
+-rw-r--r--   0        0        0   202279 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/serialization-0c0131b6.js
+-rw-r--r--   0        0        0     3319 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/shell-3c06def6.js
+-rw-r--r--   0        0        0    18843 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/solidity-3d59d6a7.js
+-rw-r--r--   0        0        0     3010 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/sophia-12eb7ba8.js
+-rw-r--r--   0        0        0     2798 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/sparql-e42fb28a.js
+-rw-r--r--   0        0        0    10543 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/sql-d30fd9fd.js
+-rw-r--r--   0        0        0     7645 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/st-0857f583.js
+-rw-r--r--   0        0        0     5417 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/swift-f0a706dd.js
+-rw-r--r--   0        0        0     7849 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/systemverilog-0cfd4211.js
+-rw-r--r--   0        0        0     3817 2024-03-27 20:10:14.122514 streamsync-0.4.0rc4/src/streamsync/static/assets/tcl-7df3c0c5.js
+-rw-r--r--   0        0        0    23320 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/tsMode-27474ecc.js
+-rw-r--r--   0        0        0     6219 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/twig-f894aab2.js
+-rw-r--r--   0        0        0     5789 2024-03-27 20:10:14.114514 streamsync-0.4.0rc4/src/streamsync/static/assets/typescript-a67a867f.js
+-rw-r--r--   0        0        0     6037 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/vb-39a025f4.js
+-rw-r--r--   0        0        0   839593 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/vega-embed.module-3d202f0a.js
+-rw-r--r--   0        0        0     7575 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/wgsl-afa2396f.js
+-rw-r--r--   0        0        0     2790 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/assets/xml-f0bf815b.js
+-rw-r--r--   0        0        0     4397 2024-03-27 20:10:14.118514 streamsync-0.4.0rc4/src/streamsync/static/assets/yaml-d6c7a4c1.js
+-rw-r--r--   0        0        0     3780 2024-03-27 20:10:11.370487 streamsync-0.4.0rc4/src/streamsync/static/favicon.png
+-rw-r--r--   0        0        0     3342 2024-03-27 20:10:14.150514 streamsync-0.4.0rc4/src/streamsync/static/index.html
+-rw-r--r--   0        0        0  1784530 2024-03-27 20:10:14.326516 streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/css.worker.bundle.js
+-rw-r--r--   0        0        0   482889 2024-03-27 20:10:14.242515 streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/editor.worker.bundle.js
+-rw-r--r--   0        0        0  1184272 2024-03-27 20:10:14.386517 streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/html.worker.bundle.js
+-rw-r--r--   0        0        0   762716 2024-03-27 20:10:14.426517 streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/json.worker.bundle.js
+-rw-r--r--   0        0        0  9667054 2024-03-27 20:10:14.942522 streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/ts.worker.bundle.js
+-rw-r--r--   0        0        0    58171 2024-03-27 20:10:20.074571 streamsync-0.4.0rc4/src/streamsync/ui.py
+-rw-r--r--   0        0        0     5885 2024-03-27 20:08:36.893569 streamsync-0.4.0rc4/src/streamsync/ui_manager.py
+-rw-r--r--   0        0        0     5231 1970-01-01 00:00:00.000000 streamsync-0.4.0rc4/PKG-INFO
```

### Comparing `streamsync-0.4.0rc3/LICENSE.txt` & `streamsync-0.4.0rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/README.md` & `streamsync-0.4.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/pyproject.toml` & `streamsync-0.4.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "streamsync"
-version = "0.4.0rc3"
+version = "0.4.0rc4"
 description = "Streamsync helps you create performant data apps, via Python code and its built-in visual UI editor."
 authors = ["Ramiro Medina <ramiro.a.medina@gmail.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://www.streamsync.cloud"
 repository = "https://www.github.com/streamsync-cloud/streamsync"
 documentation = "https://www.streamsync.cloud/getting-started.html"
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/__init__.py` & `streamsync-0.4.0rc4/src/streamsync/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import importlib.metadata
 from typing import Union, Optional, Dict, Any, Type, TypeVar, cast
 
 from streamsync.core import (BytesWrapper, Config, FileWrapper, Readable,
-                             base_component_tree, initial_state,
+                             base_component_tree, base_cmc_tree, initial_state,
                              session_manager, session_verifier)
 from streamsync.core import Readable, FileWrapper, BytesWrapper, Config, StreamsyncState
 from streamsync.core import new_initial_state, base_component_tree, session_manager, session_verifier
 from streamsync.ui import StreamsyncUIManager
 
 VERSION = importlib.metadata.version("streamsync")
 
 base_component_tree
+base_cmc_tree
 session_manager
 Config
 session_verifier
 
 
 def pack_file(file: Union[Readable, str], mime_type: Optional[str] = None):
     """
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_runner.py` & `streamsync-0.4.0rc4/src/streamsync/app_runner.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/default/main.py` & `streamsync-0.4.0rc4/src/streamsync/app_templates/default/main.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/default/static/favicon.png` & `streamsync-0.4.0rc4/src/streamsync/app_templates/default/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/default/ui.json` & `streamsync-0.4.0rc4/src/streamsync/app_templates/default/ui.json`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/assets/main_df.csv` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/assets/main_df.csv`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/assets/story.txt` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/assets/story.txt`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/main.py` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/main.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/README.md` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/README.md`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/favicon.png` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/static/pigeon1.jpg` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/static/pigeon1.jpg`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/test_app.py` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/test_app.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/app_templates/hello/ui.json` & `streamsync-0.4.0rc4/src/streamsync/app_templates/hello/ui.json`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/command_line.py` & `streamsync-0.4.0rc4/src/streamsync/command_line.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/core.py` & `streamsync-0.4.0rc4/src/streamsync/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import urllib.request
 import base64
 import io
 import re
 import json
 import math
 from streamsync.ss_types import Readable, InstancePath, StreamsyncEvent, StreamsyncEventResult, StreamsyncFileItem
-from streamsync.core_ui import ComponentTree, SessionComponentTree, use_component_tree
+from streamsync.core_ui import ComponentTree, DependentComponentTree, SessionComponentTree, use_component_tree
 
 
 class Config:
 
     is_mail_enabled_for_log: bool = False
     mode: str = "run"
     logger: Optional[logging.Logger] = None
@@ -1049,15 +1049,15 @@
         self.session_id = session_id
         self.cookies = cookies
         self.headers = headers
         self.last_active_timestamp: int = int(time.time())
         new_state = StreamsyncState.get_new()
         new_state.user_state.mutated = set()
         self.session_state = new_state
-        self.session_component_tree = SessionComponentTree(base_component_tree)
+        self.session_component_tree = SessionComponentTree(base_component_tree, base_cmc_tree)
         self.event_handler = EventHandler(self)
 
     def update_last_active_timestamp(self) -> None:
         self.last_active_timestamp = int(time.time())
 
 
 class SessionManager:
@@ -1352,8 +1352,9 @@
 
 
 
 
 state_serialiser = StateSerialiser()
 initial_state = StreamsyncState()
 base_component_tree = ComponentTree()
+base_cmc_tree = DependentComponentTree(base_component_tree)
 session_manager = SessionManager()
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/core_ui.py` & `streamsync-0.4.0rc4/src/streamsync/core_ui.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from contextvars import ContextVar
 from typing import Any, Dict, List, Optional, Union
 import uuid
 
 from pydantic import BaseModel, Field
 
 
-current_parent_container: ContextVar[Union["Component", None]] = ContextVar("current_parent_container")
-_current_component_tree: ContextVar[Union["ComponentTree", None]] = ContextVar("current_component_tree", default=None)
+current_parent_container: ContextVar[Union["Component", None]] = \
+    ContextVar("current_parent_container")
+_current_component_tree: ContextVar[Union["DependentComponentTree", None]] = \
+    ContextVar("current_component_tree", default=None)
 # This variable is thread safe and context safe
 
 
 def generate_component_id():
     return str(uuid.uuid4())
 
 
@@ -39,17 +41,16 @@
     def __exit__(self, *_):
         current_parent_container.reset(self._token)
 
 
 class ComponentTree:
 
     def __init__(self, attach_root=True) -> None:
-        self.counter: int = 0
-        self.page_counter: int = 0
         self.components: Dict[str, Component] = {}
+
         if attach_root:
             root_component = Component(
                 id="root", type="root", content={}
             )
             self.attach(root_component)
 
     def get_component(self, component_id: str) -> Optional[Component]:
@@ -71,114 +72,165 @@
     def determine_position(self, parent_id: str, is_positionless: bool = False):
         if is_positionless:
             return -2
 
         children = self.get_direct_descendents(parent_id)
         cmc_children = list(filter(lambda c: c.isCodeManaged is True, children))
         if len(cmc_children) > 0:
-            position = max([0, max([child.position for child in cmc_children]) + 1])
+            position = \
+                max([0, max([child.position for child in cmc_children]) + 1])
             return position
         else:
             return 0
 
     def attach(self, component: Component, override=False) -> None:
-        self.counter += 1
-        if component.type == "page":
-            self.page_counter += 1
+        """
+        Attaches a component to the main components dictionary of the instance.
+
+        :param component: The component to be attached.
+        :type component: Component
+        :param override: If True, an existing component with the same ID will
+                         be overridden. Defaults to False.
+        :type override: bool, optional
+        """
         if (component.id in self.components) and (override is False):
-            raise RuntimeWarning(f"Component with ID {component.id} already exists")
+            raise RuntimeWarning(
+                f"Component with ID {component.id} already exists"
+                )
         self.components[component.id] = component
 
     def ingest(self, serialised_components: Dict[str, Any]) -> None:
         removed_ids = [
-            key for key, value in self.components.items()
-            if key not in serialised_components.keys()
-            and value.isCodeManaged is False
+            key for key in self.components
+            if key not in serialised_components
         ]
 
         for component_id in removed_ids:
             if component_id == "root":
                 continue
             self.components.pop(component_id)
         for component_id, sc in serialised_components.items():
             component = Component(**sc)
-            if component.type == "page" and component_id not in self.components:
-                self.page_counter += 1
             self.components[component_id] = component
 
     def to_dict(self) -> Dict:
         active_components = {}
         for id, component in self.components.items():
             active_components[id] = component.to_dict()
         return active_components
 
 
-class SessionComponentTree(ComponentTree):
+class DependentComponentTree(ComponentTree):
 
-    def __init__(self, base_component_tree: ComponentTree):
-        super().__init__(attach_root=False)
+    def __init__(self, base_component_tree: ComponentTree, attach_root=False):
+        super().__init__(attach_root)
         self.base_component_tree = base_component_tree
-        self.updated = False
-        self.page_counter = self.base_component_tree.page_counter
 
-    def determine_position(self, parent_id: str, is_positionless: bool = False):
-        session_component_present = parent_id in self.components
-        if session_component_present:
-            # If present, use ComponentTree method
-            # for determining position directly from this class
-            return super().determine_position(parent_id, is_positionless)
-        else:
-            # Otherwise, invoke it on base component tree
-            return self.base_component_tree.determine_position(parent_id, is_positionless)
+        # Page counter is required to set
+        # predefined IDs & keys for code-managed pages
+        self.page_counter = 0
 
-    def get_component(self, component_id: str) -> Optional[Component]:
-        # Check if session component tree contains requested key
-        session_component_present = component_id in self.components
+    def attach(self, component: Component, override=False) -> None:
+        if component.type == "page" and component.id not in self.components:
+            self.page_counter += 1
+        return super().attach(component, override)
 
-        if session_component_present:
-            # If present, return session component (even if it's None)
-            session_component = self.components.get(component_id)
-            return session_component
+    def get_component(self, component_id: str) -> Optional[Component]:
+        own_component_present = component_id in self.components
+        if own_component_present:
+            # If present, return own component
+            own_component = self.components.get(component_id)
+            return own_component
 
         # Otherwise, try to obtain the base tree component
         return self.base_component_tree.get_component(component_id)
 
-    def attach(self, component: Component, override=False) -> None:
-        self.updated = True
-        return super().attach(component, override)
+    def delete_component(self, component_id: str) -> None:
+        if component_id in self.components:
+            self.components.pop(component_id, None)
+            return
+        if component_id in self.base_component_tree.components:
+            raise UIError(
+                f"Component with ID '{component_id}' " +
+                "is builder-managed and cannot be removed by app"
+                )
+        raise KeyError(
+            f"Failed to delete component with ID {component_id}: " +
+            "no such component"
+            )
 
-    def ingest(self, serialised_components: Dict[str, Any]) -> None:
-        self.updated = True
-        return super().ingest(serialised_components)
+    def clear_children(self, component_id: str) -> None:
+        children = self.get_descendents(component_id)
+        for child in children:
+            try:
+                self.delete_component(child.id)
+            except UIError:
+                raise UIError("Failed to clear children of component " +
+                              f"with ID '{component_id}': {child.id} " +
+                              "is a builder-managed component.")
+
+    def get_direct_descendents(self, parent_id: str) -> List[Component]:
+        base_children = self.base_component_tree.get_direct_descendents(parent_id)
+        own_children = list(filter(lambda c: c.parentId == parent_id, self.components.values()))
+        return base_children + own_children
 
     def to_dict(self) -> Dict:
         active_components = {
             # Collecting serialized base tree components
             component_id: base_component.to_dict()
             for component_id, base_component
             in self.base_component_tree.components.items()
         }
-        for component_id, session_component in self.components.items():
-            # Overriding base tree components with session-specific ones
-            active_components[component_id] = session_component.to_dict()
+        for component_id, own_component in self.components.items():
+            # Overriding base tree components with ones that belong to dependent tree
+            active_components[component_id] = own_component.to_dict()
         return active_components
 
+
+class SessionComponentTree(DependentComponentTree):
+
+    def __init__(self, base_component_tree: ComponentTree, base_cmc_tree: ComponentTree):
+        super().__init__(base_component_tree, attach_root=False)
+
+        # Initialize SessionComponentTree with components from the base
+        # CMC pool, added during app initialization
+        preinitialized_components = base_cmc_tree.to_dict()
+        self.ingest(preinitialized_components)
+
+        preinitialized_pages = \
+            filter(lambda c: c.type == "page", self.components.values())
+        self.page_counter = len(list(preinitialized_pages))
+
+        self.updated = False
+
+    def attach(self, component: Component, override=False) -> None:
+        self.updated = True
+        return super().attach(component, override)
+
+    def ingest(self, serialised_components: Dict[str, Any]) -> None:
+        self.updated = True
+        return super().ingest(serialised_components)
+
+    def delete_component(self, component_id: str) -> None:
+        self.updated = True
+        return super().delete_component(component_id)
+
     def fetch_updates(self):
         if self.updated:
             self.updated = False
             return self.to_dict()
         return
 
 
 class UIError(Exception):
     ...
 
 
 @contextlib.contextmanager
-def use_component_tree(component_tree: ComponentTree):
+def use_component_tree(component_tree: DependentComponentTree):
     """
     Declares the component tree that will be manipulated during a context.
 
     The declared tree can be retrieved with the `current_component_tree` method.
 
     >>> with use_component_tree(component_tree):
     >>>     ui_manager = StreamsyncUIManager()
@@ -187,20 +239,20 @@
     :param component_tree:
     """
     token = _current_component_tree.set(component_tree)
     yield
     _current_component_tree.reset(token)
 
 
-def current_component_tree() -> ComponentTree:
+def current_component_tree() -> DependentComponentTree:
     """
     Retrieves the component tree of the current context or the base
     one if no context has been declared.
 
     :return:
     """
     tree = _current_component_tree.get()
     if tree is None:
         import streamsync.core
-        return streamsync.core.base_component_tree
+        return streamsync.core.base_cmc_tree
 
     return tree
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/serve.py` & `streamsync-0.4.0rc4/src/streamsync/serve.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/ss_types.py` & `streamsync-0.4.0rc4/src/streamsync/ss_types.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/Arrow.dom-d8f7f33e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/Arrow.dom-d8f7f33e.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/BuilderApp-6c29fc91.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/BuilderApp-82d844f6.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -49,19 +49,19 @@
     L as Bb,
     M as WA,
     N as $g,
     O as Yr,
     P as n9,
     Q as qz,
     R as s9
-} from "./index-b222671e.js";
+} from "./index-0d669be8.js";
 import {
     marked as Gz
 } from "./marked.esm-0bd9b835.js";
-import Zz from "./ComponentRenderer-82ebfa88.js";
+import Zz from "./ComponentRenderer-007280fe.js";
 const Yz = 30,
     Xz = /^application\/json;streamsync=(?<componentType>\w+),(?<componentId>[\w\-]*)$/,
     Nm = Je(null),
     Wl = Je(null),
     O0 = Je(!1);
 let ex = null,
     F0 = null;
@@ -19406,15 +19406,15 @@
         order: 1
     }]
 }));
 Yb(new Y7(J7, {
     id: "default:undo",
     precondition: void 0
 }));
-const eB = Yb(new hm({
+const e8 = Yb(new hm({
     id: "redo",
     precondition: void 0,
     kbOpts: {
         weight: 0,
         primary: 2103,
         secondary: [3128],
         mac: {
@@ -19432,15 +19432,15 @@
     }, {
         menuId: R.CommandPalette,
         group: "",
         title: p("redo", "Redo"),
         order: 1
     }]
 }));
-Yb(new Y7(eB, {
+Yb(new Y7(e8, {
     id: "default:redo",
     precondition: void 0
 }));
 const mY = Yb(new hm({
     id: "editor.action.selectAll",
     precondition: void 0,
     kbOpts: {
@@ -20063,15 +20063,15 @@
 function ve(o) {
     return `var(${J2(o)})`
 }
 
 function EY(o, e) {
     return `var(${J2(o)}, ${e})`
 }
-const tB = {
+const t8 = {
     ColorContribution: "base.contributions.colors"
 };
 class TY {
     constructor() {
         this._onDidChangeSchema = new W, this.onDidChangeSchema = this._onDidChangeSchema.event, this.colorSchema = {
             type: "object",
             properties: {}
@@ -20120,15 +20120,15 @@
             return n !== s ? n - s : t.localeCompare(i)
         };
         return Object.keys(this.colorsById).sort(e).map(t => `- \`${t}\`: ${this.colorsById[t].description}`).join(`
 `)
     }
 }
 const my = new TY;
-xi.add(tB.ColorContribution, my);
+xi.add(t8.ColorContribution, my);
 
 function A(o, e, t, i, n) {
     return my.registerColor(o, e, t, i, n)
 }
 const ce = A("foreground", {
     dark: "#CCCCCC",
     light: "#616161",
@@ -20233,27 +20233,27 @@
     }, p("widgetShadow", "Shadow color of widgets such as find/replace inside the editor.")),
     eR = A("widget.border", {
         dark: null,
         light: null,
         hcDark: gt,
         hcLight: gt
     }, p("widgetBorder", "Border color of widgets such as find/replace inside the editor.")),
-    iB = A("input.background", {
+    i8 = A("input.background", {
         dark: "#3C3C3C",
         light: U.white,
         hcDark: U.black,
         hcLight: U.white
     }, p("inputBoxBackground", "Input box background.")),
-    nB = A("input.foreground", {
+    n8 = A("input.foreground", {
         dark: ce,
         light: ce,
         hcDark: ce,
         hcLight: ce
     }, p("inputBoxForeground", "Input box foreground.")),
-    sB = A("input.border", {
+    s8 = A("input.border", {
         dark: null,
         light: null,
         hcDark: gt,
         hcLight: gt
     }, p("inputBoxBorder", "Input box border.")),
     tR = A("inputOption.activeBorder", {
         dark: "#007ACC",
@@ -20413,15 +20413,15 @@
     }, p("buttonSecondaryHoverBackground", "Secondary button background color when hovering.")),
     g1 = A("badge.background", {
         dark: "#4D4D4D",
         light: "#C4C4C4",
         hcDark: U.black,
         hcLight: "#0F4A85"
     }, p("badgeBackground", "Badge background color. Badges are small information labels, e.g. for search results count.")),
-    oB = A("badge.foreground", {
+    o8 = A("badge.foreground", {
         dark: U.white,
         light: "#333",
         hcDark: U.white,
         hcLight: U.white
     }, p("badgeForeground", "Badge foreground color. Badges are small information labels, e.g. for search results count.")),
     GY = A("scrollbar.shadow", {
         dark: "#000000",
@@ -20587,15 +20587,15 @@
     }, p("pickerForeground", "Quick picker foreground color. The quick picker widget is the container for pickers like the command palette.")),
     eX = A("quickInputTitle.background", {
         dark: new U(new pt(255, 255, 255, .105)),
         light: new U(new pt(0, 0, 0, .06)),
         hcDark: "#000000",
         hcLight: U.white
     }, p("pickerTitleBackground", "Quick picker title background color. The quick picker widget is the container for pickers like the command palette.")),
-    rB = A("pickerGroup.foreground", {
+    r8 = A("pickerGroup.foreground", {
         dark: "#3794FF",
         light: "#0066BF",
         hcDark: U.white,
         hcLight: "#0F4A85"
     }, p("pickerGroupForeground", "Quick picker color for grouping labels.")),
     tX = A("pickerGroup.border", {
         dark: "#3F3F46",
@@ -20635,15 +20635,15 @@
     }, p("editorSelectionBackground", "Color of the editor selection.")),
     rX = A("editor.selectionForeground", {
         light: null,
         dark: null,
         hcDark: "#000000",
         hcLight: U.white
     }, p("editorSelectionForeground", "Color of the selected text for high contrast.")),
-    aB = A("editor.inactiveSelectionBackground", {
+    a8 = A("editor.inactiveSelectionBackground", {
         light: Me(bc, .5),
         dark: Me(bc, .5),
         hcDark: Me(bc, .7),
         hcLight: Me(bc, .5)
     }, p("editorInactiveSelection", "Color of the selection in an inactive editor. The color must not be opaque so as not to hide underlying decorations."), !0),
     sR = A("editor.selectionHighlightBackground", {
         light: CO(bc, an, .3, .6),
@@ -20747,15 +20747,15 @@
         hcDark: U.cyan,
         hcLight: "#292929"
     }, p("activeLinkForeground", "Color of active links.")),
     bd = A("editorInlayHint.foreground", {
         dark: ce,
         light: ce,
         hcDark: U.black,
-        hcLight: oB
+        hcLight: o8
     }, p("editorInlayHintForeground", "Foreground color of inline hints")),
     Cd = A("editorInlayHint.background", {
         dark: Me(g1, .25),
         light: Me(g1, .3),
         hcDark: "#f38518",
         hcLight: g1
     }, p("editorInlayHintBackground", "Background color of inline hints")),
@@ -20793,21 +20793,21 @@
     dark: "#75BEFF",
     light: "#007ACC",
     hcDark: "#75BEFF",
     hcLight: "#007ACC"
 }, p("editorLightBulbAutoFixForeground", "The color used for the lightbulb auto fix actions icon."));
 const uw = new U(new pt(155, 185, 85, .2)),
     gw = new U(new pt(255, 0, 0, .2)),
-    lB = A("diffEditor.insertedTextBackground", {
+    l8 = A("diffEditor.insertedTextBackground", {
         dark: "#9ccc2c33",
         light: "#9ccc2c40",
         hcDark: null,
         hcLight: null
     }, p("diffEditorInserted", "Background color for text that got inserted. The color must not be opaque so as not to hide underlying decorations."), !0),
-    dB = A("diffEditor.removedTextBackground", {
+    d8 = A("diffEditor.removedTextBackground", {
         dark: "#ff000033",
         light: "#ff000033",
         hcDark: null,
         hcLight: null
     }, p("diffEditorRemoved", "Background color for text that got removed. The color must not be opaque so as not to hide underlying decorations."), !0);
 A("diffEditor.insertedLineBackground", {
     dark: uw,
@@ -20829,21 +20829,21 @@
 }, p("diffEditorInsertedLineGutter", "Background color for the margin where lines got inserted."));
 A("diffEditorGutter.removedLineBackground", {
     dark: null,
     light: null,
     hcDark: null,
     hcLight: null
 }, p("diffEditorRemovedLineGutter", "Background color for the margin where lines got removed."));
-const cB = A("diffEditorOverview.insertedForeground", {
+const c8 = A("diffEditorOverview.insertedForeground", {
         dark: null,
         light: null,
         hcDark: null,
         hcLight: null
     }, p("diffEditorOverviewInserted", "Diff overview ruler foreground for inserted content.")),
-    hB = A("diffEditorOverview.removedForeground", {
+    h8 = A("diffEditorOverview.removedForeground", {
         dark: null,
         light: null,
         hcDark: null,
         hcLight: null
     }, p("diffEditorOverviewRemoved", "Diff overview ruler foreground for removed content."));
 A("diffEditor.insertedTextBorder", {
     dark: null,
@@ -20955,21 +20955,21 @@
     }, p("listInactiveFocusBackground", "List/Tree background color for the focused item when the list/tree is inactive. An active list/tree has keyboard focus, an inactive does not.")),
     DX = A("list.inactiveFocusOutline", {
         dark: null,
         light: null,
         hcDark: null,
         hcLight: null
     }, p("listInactiveFocusOutline", "List/Tree outline color for the focused item when the list/tree is inactive. An active list/tree has keyboard focus, an inactive does not.")),
-    uB = A("list.hoverBackground", {
+    u8 = A("list.hoverBackground", {
         dark: "#2A2D2E",
         light: "#F0F0F0",
         hcDark: U.white.transparent(.1),
         hcLight: U.fromHex("#0F4A85").transparent(.1)
     }, p("listHoverBackground", "List/Tree background when hovering over items using the mouse.")),
-    gB = A("list.hoverForeground", {
+    g8 = A("list.hoverForeground", {
         dark: null,
         light: null,
         hcDark: null,
         hcLight: null
     }, p("listHoverForeground", "List/Tree foreground when hovering over items using the mouse.")),
     kX = A("list.dropBackground", {
         dark: "#062F4A",
@@ -21237,17 +21237,17 @@
     }, p("breadcrumbsSelectedForeground", "Color of selected breadcrumb items."));
 A("breadcrumbPicker.background", {
     light: yi,
     dark: yi,
     hcDark: yi,
     hcLight: yi
 }, p("breadcrumbsSelectedBackground", "Background color of breadcrumb item picker."));
-const fB = .5,
-    mO = U.fromHex("#40C8AE").transparent(fB),
-    _O = U.fromHex("#40A6FF").transparent(fB),
+const f8 = .5,
+    mO = U.fromHex("#40C8AE").transparent(f8),
+    _O = U.fromHex("#40A6FF").transparent(f8),
     vO = U.fromHex("#606060").transparent(.4),
     Nr = .4,
     Lp = 1,
     Df = A("merge.currentHeaderBackground", {
         dark: mO,
         light: mO,
         hcDark: null,
@@ -21531,30 +21531,30 @@
 function Jr(o, e) {
     if (o !== null) {
         if (typeof o == "string") return o[0] === "#" ? U.fromHex(o) : e.getColor(o);
         if (o instanceof U) return o;
         if (typeof o == "object") return tQ(o, e)
     }
 }
-const pB = "vscode://schemas/workbench-colors",
-    mB = xi.as(ry.JSONContribution);
-mB.registerSchema(pB, my.getColorSchema());
-const wO = new zt(() => mB.notifySchemaChanged(pB), 200);
+const p8 = "vscode://schemas/workbench-colors",
+    m8 = xi.as(ry.JSONContribution);
+m8.registerSchema(p8, my.getColorSchema());
+const wO = new zt(() => m8.notifySchemaChanged(p8), 200);
 my.onDidChangeSchema(() => {
     wO.isScheduled() || wO.schedule()
 });
 class vy {
     constructor(e, t) {
         this.x = e, this.y = t, this._pageCoordinatesBrand = void 0
     }
     toClientCoordinates() {
-        return new _B(this.x - window.scrollX, this.y - window.scrollY)
+        return new _8(this.x - window.scrollX, this.y - window.scrollY)
     }
 }
-class _B {
+class _8 {
     constructor(e, t) {
         this.clientX = e, this.clientY = t, this._clientCoordinatesBrand = void 0
     }
     toPageCoordinates() {
         return new vy(this.clientX + window.scrollX, this.clientY + window.scrollY)
     }
 }
@@ -22087,15 +22087,15 @@
         }
         const d = new Rl(r.useMonospaceOptimizations, r.canUseHalfwidthRightwardsArrow, s.content, s.continuesWithWrappedLine, s.isBasicASCII, s.containsRTL, s.minColumn - 1, s.tokens, a, s.tabSize, s.startVisibleColumn, r.spaceWidth, r.middotWidth, r.wsmiddotWidth, r.stopRenderingLineAfter, r.renderWhitespace, r.renderControlCharacters, r.fontLigatures !== Ks.OFF, l);
         if (this._renderedViewLine && this._renderedViewLine.input.equals(d)) return !1;
         n.appendString('<div style="top:'), n.appendString(String(t)), n.appendString("px;height:"), n.appendString(String(this._options.lineHeight)), n.appendString('px;" class="'), n.appendString(Qa.CLASS_NAME), n.appendString('">');
         const c = dm(d, n);
         n.appendString("</div>");
         let h = null;
-        return Qf && fQ && s.isBasicASCII && r.useMonospaceOptimizations && c.containsForeignElements === 0 && (h = new Y0(this._renderedViewLine ? this._renderedViewLine.domNode : null, d, c.characterMapping)), h || (h = bB(this._renderedViewLine ? this._renderedViewLine.domNode : null, d, c.characterMapping, c.containsRTL, c.containsForeignElements)), this._renderedViewLine = h, !0
+        return Qf && fQ && s.isBasicASCII && r.useMonospaceOptimizations && c.containsForeignElements === 0 && (h = new Y0(this._renderedViewLine ? this._renderedViewLine.domNode : null, d, c.characterMapping)), h || (h = b8(this._renderedViewLine ? this._renderedViewLine.domNode : null, d, c.characterMapping, c.containsRTL, c.containsForeignElements)), this._renderedViewLine = h, !0
     }
     layoutLine(e, t) {
         this._renderedViewLine && this._renderedViewLine.domNode && (this._renderedViewLine.domNode.setTop(t), this._renderedViewLine.domNode.setHeight(this._options.lineHeight))
     }
     getWidth(e) {
         return this._renderedViewLine ? this._renderedViewLine.getWidth(e) : 0
     }
@@ -22151,15 +22151,15 @@
             const e = this.getWidth(null),
                 t = this.domNode.domNode.firstChild.offsetWidth;
             Math.abs(e - t) >= 2 && (console.warn("monospace assumptions have been violated, therefore disabling monospace optimizations!"), Qf = !1)
         }
         return Qf
     }
     toSlowRenderedLine() {
-        return bB(this.domNode, this.input, this._characterMapping, !1, 0)
+        return b8(this.domNode, this.input, this._characterMapping, !1, 0)
     }
     getVisibleRangesForRange(e, t, i, n) {
         const s = this._getColumnPixelOffset(e, t, n),
             r = this._getColumnPixelOffset(e, i, n);
         return [new Iu(s, r - s)]
     }
     _getColumnPixelOffset(e, t, i) {
@@ -22190,15 +22190,15 @@
     getColumnOfNodeOffset(e, t, i) {
         const n = t.textContent.length;
         let s = -1;
         for (; t;) t = t.previousSibling, s++;
         return this._characterMapping.getColumn(new j2(s, i), n)
     }
 }
-class vB {
+class v8 {
     constructor(e, t, i, n, s) {
         if (this.domNode = e, this.input = t, this._characterMapping = i, this._isWhitespaceOnly = /^\s*$/.test(t.lineContent), this._containsForeignElements = s, this._cachedWidth = -1, this._pixelOffsetCache = null, !n || this._characterMapping.length === 0) {
             this._pixelOffsetCache = new Float32Array(Math.max(2, this._characterMapping.length + 1));
             for (let r = 0, a = this._characterMapping.length; r <= a; r++) this._pixelOffsetCache[r] = -1
         }
     }
     _getReadingTarget(e) {
@@ -22267,38 +22267,38 @@
     getColumnOfNodeOffset(e, t, i) {
         const n = t.textContent.length;
         let s = -1;
         for (; t;) t = t.previousSibling, s++;
         return this._characterMapping.getColumn(new j2(s, i), n)
     }
 }
-class pQ extends vB {
+class pQ extends v8 {
     _readVisibleRangesForRange(e, t, i, n, s) {
         const r = super._readVisibleRangesForRange(e, t, i, n, s);
         if (!r || r.length === 0 || i === n || i === 1 && n === this._characterMapping.length) return r;
         if (!this.input.containsRTL) {
             const a = this._readPixelOffset(e, t, n, s);
             if (a !== -1) {
                 const l = r[r.length - 1];
                 l.left < a && (l.width = a - l.left)
             }
         }
         return r
     }
 }
-const bB = function() {
+const b8 = function() {
     return yu ? mQ : _Q
 }();
 
 function mQ(o, e, t, i, n) {
     return new pQ(o, e, t, i, n)
 }
 
 function _Q(o, e, t, i, n) {
-    return new vB(o, e, t, i, n)
+    return new v8(o, e, t, i, n)
 }
 class Ji {
     static _nextVisibleColumn(e, t, i) {
         return e === 9 ? Ji.nextRenderTabStop(t, i) : Xc(e) || N2(e) ? t + 2 : t + 1
     }
     static visibleColumnFromColumn(e, t, i) {
         const n = Math.min(t - 1, e.length),
@@ -22418,24 +22418,24 @@
     }
 }
 class oc {
     constructor(e = null) {
         this.hitTarget = e, this.type = 0
     }
 }
-class CB {
+class C8 {
     constructor(e, t, i) {
         this.position = e, this.spanNode = t, this.injectedText = i, this.type = 1
     }
 }
 var su;
 (function(o) {
     function e(t, i, n) {
         const s = t.getPositionFromDOMInfo(i, n);
-        return s ? new CB(s, i, null) : new oc(i)
+        return s ? new C8(s, i, null) : new oc(i)
     }
     o.createFromDOMInfo = e
 })(su || (su = {}));
 class vQ {
     constructor(e, t) {
         this.lastViewCursorsRenderData = e, this.lastTextareaPosition = t
     }
@@ -22997,15 +22997,15 @@
         return s !== -1 ? new V(e.lineNumber, s + 1) : e
     }
     static _doHitTest(e, t) {
         let i = new oc;
         if (typeof document.caretRangeFromPoint == "function" ? i = this._doHitTestWithCaretRangeFromPoint(e, t) : document.caretPositionFromPoint && (i = this._doHitTestWithCaretPositionFromPoint(e, t.pos.toClientCoordinates())), i.type === 1) {
             const n = e.viewModel.getInjectedTextAt(i.position),
                 s = e.viewModel.normalizePosition(i.position, 2);
-            (n || !s.equals(i.position)) && (i = new CB(s, i.spanNode, n))
+            (n || !s.equals(i.position)) && (i = new C8(s, i.spanNode, n))
         }
         return i
     }
 }
 
 function CQ(o, e, t) {
     const i = document.createRange();
@@ -23141,15 +23141,15 @@
     }
     _hide(e) {
         var t;
         this._revealTimer.cancel(), this._isVisible && (this._isVisible = !1, (t = this._domNode) === null || t === void 0 || t.setClassName(this._invisibleClassName + (e ? " fade" : "")))
     }
 }
 const yQ = 140;
-class wB extends Ur {
+class w8 extends Ur {
     constructor(e) {
         super(), this._lazyRender = e.lazyRender, this._host = e.host, this._scrollable = e.scrollable, this._scrollByPage = e.scrollByPage, this._scrollbarState = e.scrollbarState, this._visibilityController = this._register(new SQ(e.visibility, "visible scrollbar " + e.extraScrollbarClassName, "invisible scrollbar " + e.extraScrollbarClassName)), this._visibilityController.setIsNeeded(this._scrollbarState.isNeeded()), this._pointerMoveMonitor = this._register(new um), this._shouldRender = !0, this.domNode = wt(document.createElement("div")), this.domNode.setAttribute("role", "presentation"), this.domNode.setAttribute("aria-hidden", "true"), this._visibilityController.setDomNode(this.domNode), this.domNode.setPosition("absolute"), this._register(G(this.domNode.domNode, me.POINTER_DOWN, t => this._domNodePointerDown(t)))
     }
     _createArrow(e) {
         const t = this._register(new wQ(e));
         this.domNode.domNode.appendChild(t.bgDomNode), this.domNode.domNode.appendChild(t.domNode)
     }
@@ -23313,15 +23313,15 @@
     }
     getDesiredScrollPositionFromDelta(e) {
         if (!this._computedIsNeeded) return 0;
         const t = this._computedSliderPosition + e;
         return Math.round(t / this._computedSliderRatio)
     }
 }
-class xQ extends wB {
+class xQ extends w8 {
     constructor(e, t, i) {
         const n = e.getScrollDimensions(),
             s = e.getCurrentScrollPosition();
         if (super({
                 lazyRender: t.lazyRender,
                 host: i,
                 scrollbarState: new Ep(t.horizontalHasArrows ? t.arrowSize : 0, t.horizontal === 2 ? 0 : t.horizontalScrollbarSize, t.vertical === 2 ? 0 : t.verticalScrollbarSize, n.width, n.scrollWidth, s.scrollLeft),
@@ -23380,15 +23380,15 @@
     writeScrollPosition(e, t) {
         e.scrollLeft = t
     }
     updateOptions(e) {
         this.updateScrollbarSize(e.horizontal === 2 ? 0 : e.horizontalScrollbarSize), this._scrollbarState.setOppositeScrollbarSize(e.vertical === 2 ? 0 : e.verticalScrollbarSize), this._visibilityController.setVisibility(e.horizontal), this._scrollByPage = e.scrollByPage
     }
 }
-class DQ extends wB {
+class DQ extends w8 {
     constructor(e, t, i) {
         const n = e.getScrollDimensions(),
             s = e.getCurrentScrollPosition();
         if (super({
                 lazyRender: t.lazyRender,
                 host: i,
                 scrollbarState: new Ep(t.verticalHasArrows ? t.arrowSize : 0, t.vertical === 2 ? 0 : t.verticalScrollbarSize, 0, n.height, n.scrollHeight, s.scrollTop),
@@ -23795,15 +23795,15 @@
     _hide() {
         !this._mouseIsOver && !this._isDragging && (this._verticalScrollbar.beginHide(), this._horizontalScrollbar.beginHide())
     }
     _scheduleHide() {
         !this._mouseIsOver && !this._isDragging && this._hideTimeout.cancelAndSet(() => this._hide(), TQ)
     }
 }
-class SB extends dR {
+class S8 extends dR {
     constructor(e, t) {
         t = t || {}, t.mouseWheelSmoothScroll = !1;
         const i = new Jb({
             forceIntegerValues: !0,
             smoothScrollDuration: 0,
             scheduleAtNextAnimationFrame: n => hr(n)
         });
@@ -23938,15 +23938,15 @@
     onCursorStateChanged(e) {
         return this._mouseDownOperation.onCursorStateChanged(e), !1
     }
     onFocusChanged(e) {
         return !1
     }
     getTargetAtClientPoint(e, t) {
-        const n = new _B(e, t).toPageCoordinates(),
+        const n = new _8(e, t).toPageCoordinates(),
             s = rR(this.viewHelper.viewDomNode);
         if (n.y < s.y || n.y > s.y + s.height || n.x < s.x || n.x > s.x + s.width) return null;
         const r = aR(this.viewHelper.viewDomNode, s, n);
         return this.mouseTargetFactory.createMouseTarget(this.viewHelper.getLastRenderData(), s, n, r, null)
     }
     _createMouseTarget(e, t) {
         let i = e.target;
@@ -24811,15 +24811,15 @@
             return "hc-black";
         case nr.HIGH_CONTRAST_LIGHT:
             return "hc-light";
         default:
             return "vs"
     }
 }
-const yB = {
+const y8 = {
     ThemingContribution: "base.contributions.theming"
 };
 class zQ {
     constructor() {
         this.themingParticipants = [], this.themingParticipants = [], this.onThemingParticipantAddedEmitter = new W
     }
     onColorThemeChange(e) {
@@ -24828,30 +24828,30 @@
             this.themingParticipants.splice(t, 1)
         })
     }
     getThemingParticipants() {
         return this.themingParticipants
     }
 }
-const LB = new zQ;
-xi.add(yB.ThemingContribution, LB);
+const L8 = new zQ;
+xi.add(y8.ThemingContribution, L8);
 
 function jr(o) {
-    return LB.onColorThemeChange(o)
+    return L8.onColorThemeChange(o)
 }
 class $Q extends z {
     constructor(e) {
         super(), this.themeService = e, this.theme = e.getColorTheme(), this._register(this.themeService.onDidColorThemeChange(t => this.onThemeChange(t)))
     }
     onThemeChange(e) {
         this.theme = e, this.updateStyles()
     }
     updateStyles() {}
 }
-const xB = A("editor.lineHighlightBackground", {
+const x8 = A("editor.lineHighlightBackground", {
         dark: null,
         light: null,
         hcDark: null,
         hcLight: null
     }, p("lineHighlight", "Background color for the highlight of line at the cursor position.")),
     kO = A("editor.lineHighlightBorder", {
         dark: "#282828",
@@ -24879,15 +24879,15 @@
 }, p("symbolHighlight", "Background color of highlighted symbol, like for go to definition or go next/previous symbol. The color must not be opaque so as not to hide underlying decorations."), !0);
 A("editor.symbolHighlightBorder", {
     dark: null,
     light: null,
     hcDark: ni,
     hcLight: ni
 }, p("symbolHighlightBorder", "Background color of the border around highlighted symbols."), !0);
-const DB = A("editorCursor.foreground", {
+const D8 = A("editorCursor.foreground", {
         dark: "#AEAFAD",
         light: U.black,
         hcDark: U.white,
         hcLight: "#0F4A85"
     }, p("caret", "Color of the editor cursor.")),
     UQ = A("editorCursor.background", null, p("editorCursorBackground", "The background color of the editor cursor. Allows customizing the color of a character overlapped by a block cursor.")),
     Sd = A("editorWhitespace.foreground", {
@@ -25068,15 +25068,15 @@
 A("editorGhostText.background", {
     dark: null,
     light: null,
     hcDark: null,
     hcLight: null
 }, p("editorGhostTextBackground", "Background color of the ghost text in the editor."));
 const eC = new U(new pt(0, 122, 204, .6)),
-    kB = A("editorOverviewRuler.rangeHighlightForeground", {
+    k8 = A("editorOverviewRuler.rangeHighlightForeground", {
         dark: eC,
         light: eC,
         hcDark: eC,
         hcLight: eC
     }, p("overviewRulerRangeHighlight", "Overview ruler marker color for range highlights. The color must not be opaque so as not to hide underlying decorations."), !0),
     rJ = A("editorOverviewRuler.errorForeground", {
         dark: new U(new pt(255, 18, 18, .7)),
@@ -25092,45 +25092,45 @@
     }, p("overviewRuleWarning", "Overview ruler marker color for warnings.")),
     lJ = A("editorOverviewRuler.infoForeground", {
         dark: No,
         light: No,
         hcDark: $I,
         hcLight: $I
     }, p("overviewRuleInfo", "Overview ruler marker color for infos.")),
-    IB = A("editorBracketHighlight.foreground1", {
+    I8 = A("editorBracketHighlight.foreground1", {
         dark: "#FFD700",
         light: "#0431FAFF",
         hcDark: "#FFD700",
         hcLight: "#0431FAFF"
     }, p("editorBracketHighlightForeground1", "Foreground color of brackets (1). Requires enabling bracket pair colorization.")),
-    EB = A("editorBracketHighlight.foreground2", {
+    E8 = A("editorBracketHighlight.foreground2", {
         dark: "#DA70D6",
         light: "#319331FF",
         hcDark: "#DA70D6",
         hcLight: "#319331FF"
     }, p("editorBracketHighlightForeground2", "Foreground color of brackets (2). Requires enabling bracket pair colorization.")),
-    TB = A("editorBracketHighlight.foreground3", {
+    T8 = A("editorBracketHighlight.foreground3", {
         dark: "#179FFF",
         light: "#7B3814FF",
         hcDark: "#87CEFA",
         hcLight: "#7B3814FF"
     }, p("editorBracketHighlightForeground3", "Foreground color of brackets (3). Requires enabling bracket pair colorization.")),
-    NB = A("editorBracketHighlight.foreground4", {
+    N8 = A("editorBracketHighlight.foreground4", {
         dark: "#00000000",
         light: "#00000000",
         hcDark: "#00000000",
         hcLight: "#00000000"
     }, p("editorBracketHighlightForeground4", "Foreground color of brackets (4). Requires enabling bracket pair colorization.")),
-    RB = A("editorBracketHighlight.foreground5", {
+    R8 = A("editorBracketHighlight.foreground5", {
         dark: "#00000000",
         light: "#00000000",
         hcDark: "#00000000",
         hcLight: "#00000000"
     }, p("editorBracketHighlightForeground5", "Foreground color of brackets (5). Requires enabling bracket pair colorization.")),
-    MB = A("editorBracketHighlight.foreground6", {
+    M8 = A("editorBracketHighlight.foreground6", {
         dark: "#00000000",
         light: "#00000000",
         hcDark: "#00000000",
         hcLight: "#00000000"
     }, p("editorBracketHighlightForeground6", "Foreground color of brackets (6). Requires enabling bracket pair colorization.")),
     dJ = A("editorBracketHighlight.unexpectedBracket.foreground", {
         dark: new U(new pt(255, 18, 18, .8)),
@@ -25220,15 +25220,15 @@
     dark: "#bd9b0326",
     light: "#cea33d14",
     hcDark: "#00000000",
     hcLight: "#cea33d14"
 }, p("editorUnicodeHighlight.background", "Background color used to highlight unicode characters."));
 jr((o, e) => {
     const t = o.getColor(an),
-        i = o.getColor(xB),
+        i = o.getColor(x8),
         n = i && !i.isTransparent() ? i : t;
     n && e.addRule(`.monaco-editor .inputarea.ime-input { background-color: ${n}; }`)
 });
 class i0 extends kg {
     constructor(e) {
         super(), this._context = e, this._readConfig(), this._lastCursorModelPosition = new V(1, 1), this._renderResult = null, this._activeLineNumber = 1, this._context.addEventHandler(this)
     }
@@ -25867,25 +25867,25 @@
         const n = Ji.columnFromVisibleColumn(e.getLineContent(t), i, this.tabSize),
             s = e.getLineMinColumn(t);
         if (n < s) return s;
         const r = e.getLineMaxColumn(t);
         return n > r ? r : n
     }
 }
-let Ct = class AB {
+let Ct = class A8 {
     static fromModelState(e) {
         return new NJ(e)
     }
     static fromViewState(e) {
         return new RJ(e)
     }
     static fromModelSelection(e) {
         const t = Ie.liftSelection(e),
             i = new Dn(I.fromPositions(t.getSelectionStart()), 0, 0, t.getPosition(), 0);
-        return AB.fromModelState(i)
+        return A8.fromModelState(i)
     }
     static fromModelSelections(e) {
         const t = [];
         for (let i = 0, n = e.length; i < n; i++) t[i] = this.fromModelSelection(e[i]);
         return t
     }
     constructor(e, t) {
@@ -27461,15 +27461,15 @@
         if (!h) return null;
         let u = h.indentation;
         return h.action !== $i.Indent && (u = n.unshiftIndent(u)), u
     }
     return null
 }
 
-function PB(o, e, t) {
+function P8(o, e, t) {
     const i = t.getLanguageConfiguration(o.getLanguageId()).indentRulesSupport;
     return !i || e < 1 || e > o.getLineCount() ? null : i.getIndentMetadata(o.getLineContent(e))
 }
 class ci {
     static indent(e, t, i) {
         if (t === null || i === null) return [];
         const n = [];
@@ -27814,15 +27814,15 @@
         }
         return g ? c.close.substring(0, c.close.length - u.length) : c.close
     }
     static _runAutoClosingOpenCharType(e, t, i, n, s, r, a) {
         const l = [];
         for (let d = 0, c = n.length; d < c; d++) {
             const h = n[d];
-            l[d] = new OB(h, s, !r, a)
+            l[d] = new O8(h, s, !r, a)
         }
         return new Vs(4, l, {
             shouldPushStackElementBefore: !0,
             shouldPushStackElementAfter: !1
         })
     }
     static _shouldSurroundChar(e, t) {
@@ -28021,15 +28021,15 @@
     }
     static lineBreakInsert(e, t, i) {
         const n = [];
         for (let s = 0, r = i.length; s < r; s++) n[s] = this._enter(e, t, !0, i[s]);
         return n
     }
 }
-class OB extends p1 {
+class O8 extends p1 {
     constructor(e, t, i, n) {
         super(e, (i ? t : "") + n, 0, -n.length), this._openCharacter = t, this._closeCharacter = n, this.closeCharacterRange = null, this.enclosingRange = null
     }
     computeCursorState(e, t) {
         const n = t.getInverseEditOperations()[0].range;
         return this.closeCharacterRange = new I(n.startLineNumber, n.endColumn - this._closeCharacter.length, n.endLineNumber, n.endColumn), this.enclosingRange = new I(n.startLineNumber, n.endColumn - this._openCharacter.length - this._closeCharacter.length, n.endLineNumber, n.endColumn), super.computeCursorState(e, t)
     }
@@ -29458,15 +29458,15 @@
             document.execCommand("undo")
         }
         runEditorCommand(t, i, n) {
             if (!(!i.hasModel() || i.getOption(89) === !0)) return i.getModel().undo()
         }
     }, o.Redo = new class extends ZI {
         constructor() {
-            super(eB)
+            super(e8)
         }
         runDOMCommand() {
             document.execCommand("redo")
         }
         runEditorCommand(t, i, n) {
             if (!(!i.hasModel() || i.getOption(89) === !0)) return i.getModel().redo()
         }
@@ -29736,15 +29736,15 @@
             positionBefore: e.positionBefore ? t.convertViewPositionToModelPosition(e.positionBefore) : e.positionBefore,
             positionAfter: e.positionAfter ? t.convertViewPositionToModelPosition(e.positionAfter) : e.positionAfter,
             position: t.convertViewPositionToModelPosition(e.position),
             afterLineNumber: t.convertViewPositionToModelPosition(new V(e.afterLineNumber, 1)).lineNumber
         }
     }
 }
-class FB {
+class F8 {
     constructor(e) {
         this._createLine = e, this._set(1, [])
     }
     flush() {
         this._set(1, [])
     }
     _set(e, t) {
@@ -29830,17 +29830,17 @@
                 const h = c - this._rendLineNumberStart;
                 this._lines[h].onTokensChanged(), n = !0
             }
         }
         return n
     }
 }
-class BB {
+class B8 {
     constructor(e) {
-        this._host = e, this.domNode = this._createDomNode(), this._linesCollection = new FB(() => this._host.createVisibleLine())
+        this._host = e, this.domNode = this._createDomNode(), this._linesCollection = new F8(() => this._host.createVisibleLine())
     }
     _createDomNode() {
         const e = wt(document.createElement("div"));
         return e.setClassName("view-layer"), e.setPosition("absolute"), e.domNode.setAttribute("role", "presentation"), e.domNode.setAttribute("aria-hidden", "true"), e
     }
     onConfigurationChanged(e) {
         return !!e.hasChanged(142)
@@ -30016,17 +30016,17 @@
         }
     }
 }
 cd._ttPolicy = Hd("editorViewLayer", {
     createHTML: o => o
 });
 cd._sb = new yg(1e5);
-class WB extends po {
+class W8 extends po {
     constructor(e) {
-        super(e), this._visibleLines = new BB(this), this.domNode = this._visibleLines.domNode;
+        super(e), this._visibleLines = new B8(this), this.domNode = this._visibleLines.domNode;
         const i = this._context.configuration.options.get(49);
         ln(this.domNode, i), this._dynamicOverlays = [], this._isFocused = !1, this.domNode.setClassName("view-overlays")
     }
     shouldRender() {
         if (super.shouldRender()) return !0;
         for (let e = 0, t = this._dynamicOverlays.length; e < t; e++)
             if (this._dynamicOverlays[e].shouldRender()) return !0;
@@ -30115,15 +30115,15 @@
         }
         return this._renderedContent === s ? !1 : (this._renderedContent = s, n.appendString('<div style="position:absolute;top:'), n.appendString(String(t)), n.appendString("px;width:100%;height:"), n.appendString(String(this._lineHeight)), n.appendString('px;">'), n.appendString(s), n.appendString("</div>"), !0)
     }
     layoutLine(e, t) {
         this._domNode && (this._domNode.setTop(t), this._domNode.setHeight(this._lineHeight))
     }
 }
-class jJ extends WB {
+class jJ extends W8 {
     constructor(e) {
         super(e);
         const i = this._context.configuration.options.get(142);
         this._contentWidth = i.contentWidth, this.domNode.setHeight(0)
     }
     onConfigurationChanged(e) {
         const i = this._context.configuration.options.get(142);
@@ -30132,15 +30132,15 @@
     onScrollChanged(e) {
         return super.onScrollChanged(e) || e.scrollWidthChanged
     }
     _viewOverlaysRender(e) {
         super._viewOverlaysRender(e), this.domNode.setWidth(Math.max(e.scrollWidth, this._contentWidth))
     }
 }
-class KJ extends WB {
+class KJ extends W8 {
     constructor(e) {
         super(e);
         const t = this._context.configuration.options,
             i = t.get(142);
         this._contentLeft = i.contentLeft, this.domNode.setClassName("margin-view-overlays"), this.domNode.setWidth(1), ln(this.domNode, t.get(49))
     }
     onConfigurationChanged(e) {
@@ -30426,15 +30426,15 @@
 function Fx(o, e, ...t) {
     try {
         return o.call(e, ...t)
     } catch {
         return null
     }
 }
-class VB extends kg {
+class V8 extends kg {
     constructor(e) {
         super(), this._context = e;
         const t = this._context.configuration.options,
             i = t.get(142);
         this._lineHeight = t.get(65), this._renderLineHighlight = t.get(94), this._renderLineHighlightOnlyWhenFocus = t.get(95), this._contentLeft = i.contentLeft, this._contentWidth = i.contentWidth, this._selectionIsEmpty = !0, this._focused = !1, this._cursorLineNumbers = [1], this._selections = [new Ie(1, 1, 1, 1)], this._renderData = null, this._context.addEventHandler(this)
     }
     dispose() {
@@ -30502,38 +30502,38 @@
     _shouldRenderInMargin() {
         return (this._renderLineHighlight === "gutter" || this._renderLineHighlight === "all") && (!this._renderLineHighlightOnlyWhenFocus || this._focused)
     }
     _shouldRenderInContent() {
         return (this._renderLineHighlight === "line" || this._renderLineHighlight === "all") && this._selectionIsEmpty && (!this._renderLineHighlightOnlyWhenFocus || this._focused)
     }
 }
-class ZJ extends VB {
+class ZJ extends V8 {
     _renderOne(e) {
         return `<div class="${"current-line"+(this._shouldRenderOther()?" current-line-both":"")}" style="width:${Math.max(e.scrollWidth,this._contentWidth)}px; height:${this._lineHeight}px;"></div>`
     }
     _shouldRenderThis() {
         return this._shouldRenderInContent()
     }
     _shouldRenderOther() {
         return this._shouldRenderInMargin()
     }
 }
-class YJ extends VB {
+class YJ extends V8 {
     _renderOne(e) {
         return `<div class="${"current-line"+(this._shouldRenderInMargin()?" current-line-margin":"")+(this._shouldRenderOther()?" current-line-margin-both":"")}" style="width:${this._contentLeft}px; height:${this._lineHeight}px;"></div>`
     }
     _shouldRenderThis() {
         return !0
     }
     _shouldRenderOther() {
         return this._shouldRenderInContent()
     }
 }
 jr((o, e) => {
-    const t = o.getColor(xB);
+    const t = o.getColor(x8);
     if (t && (e.addRule(`.monaco-editor .view-overlays .current-line { background-color: ${t}; }`), e.addRule(`.monaco-editor .margin-view-overlays .current-line-margin { background-color: ${t}; border: none; }`)), !t || t.isTransparent() || o.defines(kO)) {
         const i = o.getColor(kO);
         i && (e.addRule(`.monaco-editor .view-overlays .current-line { border: 2px solid ${i}; }`), e.addRule(`.monaco-editor .margin-view-overlays .current-line-margin { border: 2px solid ${i}; }`), ml(o.type) && (e.addRule(".monaco-editor .view-overlays .current-line { border-width: 1px; }"), e.addRule(".monaco-editor .margin-view-overlays .current-line-margin { border-width: 1px; }")))
     }
 });
 class XJ extends kg {
     constructor(e) {
@@ -30753,15 +30753,15 @@
         return this.scrollbar.updateClassName("editor-scrollable " + _w(this._context.theme.type)), !0
     }
     prepareRender(e) {}
     render(e) {
         this.scrollbar.renderNow()
     }
 }
-class HB extends z {
+class H8 extends z {
     constructor() {
         super(...arguments), this._isDisposed = !1
     }
     dispose() {
         super.dispose(), this._isDisposed = !0
     }
     assertNotDisposed() {
@@ -30792,15 +30792,15 @@
     }
 }
 class W_ {
     constructor(e, t) {
         this.top = e, this.endColumn = t
     }
 }
-class JJ extends HB {
+class JJ extends H8 {
     constructor(e, t) {
         super(), this.textModel = e, this.languageConfigurationService = t
     }
     getLanguageConfiguration(e) {
         return this.languageConfigurationService.getLanguageConfiguration(e)
     }
     _computeIndentLevel(e) {
@@ -30919,15 +30919,15 @@
             l = this.textModel.bracketPairs.getBracketPairsInRangeWithMinIndentation(new I(e, 1, t, this.textModel.getLineMaxColumn(t))).toArray();
         let d;
         if (i && l.length > 0) {
             const u = (e <= i.lineNumber && i.lineNumber <= t ? l : this.textModel.bracketPairs.getBracketPairsInRange(I.fromPositions(i)).toArray()).filter(g => I.strictContainsPosition(g.range, i));
             d = (s = a9(u, g => a)) === null || s === void 0 ? void 0 : s.range
         }
         const c = this.textModel.getOptions().bracketPairColorizationOptions.independentColorPoolPerBracketType,
-            h = new zB;
+            h = new z8;
         for (const u of l) {
             if (!u.closingBracketRange) continue;
             const g = d && u.range.equalsRange(d);
             if (!g && !n.includeInactive) continue;
             const f = h.getInlineClassName(u.nestingLevel, u.nestingLevelOfEqualBracketType, c) + (n.highlightActive && g ? " " + h.activeClassName : ""),
                 m = u.openingBracketRange.getStartPosition(),
                 _ = u.closingBracketRange.getStartPosition(),
@@ -30998,15 +30998,15 @@
         return a
     }
     _getIndentLevelForWhitespaceLine(e, t, i) {
         const n = this.textModel.getOptions();
         return t === -1 || i === -1 ? 0 : t < i ? 1 + Math.floor(t / n.indentSize) : t === i || e ? Math.ceil(i / n.indentSize) : 1 + Math.floor(i / n.indentSize)
     }
 }
-class zB {
+class z8 {
     constructor() {
         this.activeClassName = "indent-active"
     }
     getInlineClassName(e, t, i) {
         return this.getInlineClassNameOfLevel(i ? t : e)
     }
     getInlineClassNameOfLevel(e) {
@@ -31130,39 +31130,39 @@
 }
 
 function Zg(o) {
     if (!(o && o.isTransparent())) return o
 }
 jr((o, e) => {
     const t = [{
-            bracketColor: IB,
+            bracketColor: I8,
             guideColor: cJ,
             guideColorActive: mJ
         }, {
-            bracketColor: EB,
+            bracketColor: E8,
             guideColor: hJ,
             guideColorActive: _J
         }, {
-            bracketColor: TB,
+            bracketColor: T8,
             guideColor: uJ,
             guideColorActive: vJ
         }, {
-            bracketColor: NB,
+            bracketColor: N8,
             guideColor: gJ,
             guideColorActive: bJ
         }, {
-            bracketColor: RB,
+            bracketColor: R8,
             guideColor: fJ,
             guideColorActive: CJ
         }, {
-            bracketColor: MB,
+            bracketColor: M8,
             guideColor: pJ,
             guideColorActive: wJ
         }],
-        i = new zB,
+        i = new z8,
         n = [{
             indentColor: e0,
             indentColorActive: t0
         }, {
             indentColor: KQ,
             indentColorActive: XQ
         }, {
@@ -31265,15 +31265,15 @@
             r = Math.min(r, c.startLineNumber), a = Math.max(a, c.endLineNumber)
         }
         this.minLineNumber = r, this.maxLineNumber = a
     }
 }
 class xy extends po {
     constructor(e, t) {
-        super(e), this._linesContent = t, this._textRangeRestingSpot = document.createElement("div"), this._visibleLines = new BB(this), this.domNode = this._visibleLines.domNode;
+        super(e), this._linesContent = t, this._textRangeRestingSpot = document.createElement("div"), this._visibleLines = new B8(this), this.domNode = this._visibleLines.domNode;
         const i = this._context.configuration,
             n = this._context.configuration.options,
             s = n.get(49),
             r = n.get(143);
         this._lineHeight = n.get(65), this._typicalHalfwidthCharacterWidth = s.typicalHalfwidthCharacterWidth, this._isViewportWrapping = r.isViewportWrapping, this._revealHorizontalRightPadding = n.get(98), this._cursorSurroundingLines = n.get(28), this._cursorSurroundingLinesStyle = n.get(29), this._canUseLayerHinting = !n.get(31), this._viewLineOptions = new yO(i, this._context.theme.type), Ll.write(this.domNode, 7), this.domNode.setClassName(`view-lines ${Eu}`), ln(this.domNode, s), this._maxLineWidth = 0, this._asyncUpdateLineWidths = new zt(() => {
             this._updateLineWidthsSlow()
         }, 200), this._asyncCheckMonospaceFontAssumptions = new zt(() => {
@@ -31612,15 +31612,15 @@
     add(e) {
         this.decorations.push(e)
     }
     getDecorations() {
         return this.decorations
     }
 }
-class $B extends kg {
+class $8 extends kg {
     _render(e, t, i) {
         const n = [];
         for (let a = e; a <= t; a++) {
             const l = a - e;
             n[l] = new oee
         }
         if (i.length === 0) return n;
@@ -31800,15 +31800,15 @@
     }
 }
 class dee {
     constructor(e, t, i) {
         this.lineNumber = e, this.lane = t, this.combinedClassName = i
     }
 }
-class cee extends $B {
+class cee extends $8 {
     constructor(e) {
         super(), this._context = e;
         const i = this._context.configuration.options.get(142);
         this._decorationsLeft = i.decorationsLeft, this._decorationsWidth = i.decorationsWidth, this._renderResult = null, this._context.addEventHandler(this)
     }
     dispose() {
         this._context.removeEventHandler(this), this._renderResult = null, super.dispose()
@@ -31869,15 +31869,15 @@
         }
         this._renderResult = l
     }
     render(e, t) {
         return this._renderResult ? this._renderResult[t - e] : ""
     }
 }
-class hee extends $B {
+class hee extends $8 {
     constructor(e) {
         super(), this._context = e, this._renderResult = null, this._context.addEventHandler(this)
     }
     dispose() {
         this._context.removeEventHandler(this), this._renderResult = null, super.dispose()
     }
     onConfigurationChanged(e) {
@@ -32247,15 +32247,15 @@
     onTokensChanged() {
         this.dy = -1
     }
 }
 Cw.INVALID = new Cw(-1);
 class OO {
     constructor(e, t, i) {
-        this.renderedLayout = e, this._imageData = t, this._renderedLines = new FB(() => Cw.INVALID), this._renderedLines._set(e.startLineNumber, i)
+        this.renderedLayout = e, this._imageData = t, this._renderedLines = new F8(() => Cw.INVALID), this._renderedLines._set(e.startLineNumber, i)
     }
     linesEquals(e) {
         if (!this.scrollEquals(e)) return !1;
         const i = this._renderedLines._get().lines;
         for (let n = 0, s = i.length; n < s; n++)
             if (i[n].dy === -1) return !1;
         return !0
@@ -32976,15 +32976,15 @@
 }
 class vee {
     constructor(e, t) {
         const i = e.options;
         this.lineHeight = i.get(65), this.pixelRatio = i.get(140), this.overviewRulerLanes = i.get(81), this.renderBorder = i.get(80);
         const n = t.getColor(nJ);
         this.borderColor = n ? n.toString() : null, this.hideCursor = i.get(58);
-        const s = t.getColor(DB);
+        const s = t.getColor(D8);
         this.cursorColor = s ? s.transparent(.7).toString() : null, this.themeType = t.type;
         const r = i.get(71),
             a = r.enabled,
             l = r.side,
             d = t.getColor(sJ),
             c = fi.getDefaultBackground();
         d ? this.backgroundColor = d : a && l === "right" ? this.backgroundColor = c : this.backgroundColor = null;
@@ -33803,15 +33803,15 @@
     }
     getLastRenderData() {
         return this._renderData
     }
 }
 Fv.BLINK_INTERVAL = 500;
 jr((o, e) => {
-    const t = o.getColor(DB);
+    const t = o.getColor(D8);
     if (t) {
         let i = o.getColor(UQ);
         i || (i = t.opposite()), e.addRule(`.monaco-editor .cursors-layer .cursor { background-color: ${t}; border-color: ${t}; color: ${i}; }`), ml(o.type) && e.addRule(`.monaco-editor .cursors-layer.has-selection .cursor { border-left: 1px solid ${i}; border-right: 1px solid ${i}; }`)
     }
 });
 const Wx = () => {
     throw new Error("Invalid change accessor")
@@ -34496,15 +34496,15 @@
 function Fee(o) {
     try {
         return o()
     } catch (e) {
         Xe(e)
     }
 }
-class UB {
+class U8 {
     constructor(e, t, i, n, s, r) {
         this.id = e, this.label = t, this.alias = i, this._precondition = n, this._run = s, this._contextKeyService = r
     }
     isSupported() {
         return this._contextKeyService.contextMatchesRules(this._precondition)
     }
     run(e) {
@@ -34584,15 +34584,15 @@
     return e >= qs && (t = t - o % qs), t
 }
 
 function Hee(o, e) {
     return o.reduce((t, i) => li(t, e(i)), is)
 }
 
-function jB(o, e) {
+function j8(o, e) {
     return o === e
 }
 
 function Np(o, e) {
     const t = o,
         i = e;
     if (i - t <= 0) return is;
@@ -34753,15 +34753,15 @@
 ji.cache = new Array(129);
 ji.empty = ji.create(0, _1);
 const $O = {
     getKey(o) {
         return o
     }
 };
-class KB {
+class K8 {
     constructor() {
         this.items = new Map
     }
     getKey(e) {
         let t = this.items.get(e);
         return t === void 0 && (t = this.items.size, this.items.set(e, t)), t
     }
@@ -35098,15 +35098,15 @@
     }
 }
 let gc = class {
     constructor(e, t, i, n, s) {
         this.length = e, this.kind = t, this.bracketId = i, this.bracketIds = n, this.astNode = s
     }
 };
-class qB {
+class q8 {
     constructor(e, t) {
         this.textModel = e, this.bracketTokens = t, this.reader = new Zee(this.textModel, this.bracketTokens), this._offset = is, this.didPeek = !1, this.peeked = null, this.textBufferLineCount = e.getLineCount(), this.textBufferLastLineLength = e.getLineLength(this.textBufferLineCount)
     }
     get offset() {
         return this._offset
     }
     get length() {
@@ -35292,15 +35292,15 @@
     }
 }
 
 function Xee(o) {
     let e = Oo(o);
     return /^[\w ]+/.test(o) && (e = `\\b${e}`), /[\w ]+$/.test(o) && (e = `${e}\\b`), e
 }
-class GB {
+class G8 {
     constructor(e, t) {
         this.denseKeyProvider = e, this.getLanguageConfiguration = t, this.languageIdToBracketTokens = new Map
     }
     didLanguageChange(e) {
         return this.languageIdToBracketTokens.has(e)
     }
     getSingleLanguageBracketTokens(e) {
@@ -35315,24 +35315,24 @@
     let e = 0;
 
     function t() {
         if (e >= o.length) return null;
         const r = e,
             a = o[r].listHeight;
         for (e++; e < o.length && o[e].listHeight === a;) e++;
-        return e - r >= 2 ? ZB(r === 0 && e === o.length ? o : o.slice(r, e), !1) : o[r]
+        return e - r >= 2 ? Z8(r === 0 && e === o.length ? o : o.slice(r, e), !1) : o[r]
     }
     let i = t(),
         n = t();
     if (!n) return i;
     for (let r = t(); r; r = t()) UO(i, n) <= UO(n, r) ? (i = Vx(i, n), n = r) : n = Vx(n, r);
     return Vx(i, n)
 }
 
-function ZB(o, e = !1) {
+function Z8(o, e = !1) {
     if (o.length === 0) return null;
     if (o.length === 1) return o[0];
     let t = o.length;
     for (; t > 3;) {
         const i = t >> 1;
         for (let n = 0; n < i; n++) {
             const s = n << 1;
@@ -35461,15 +35461,15 @@
             if (!s) {
                 const r = this.tokenizer.peek();
                 if (!r || r.kind === 2 && r.bracketIds.intersects(e)) break;
                 s = this.parseChild(e, t + 1)
             }
             s.kind === 4 && s.childrenLength === 0 || i.push(s)
         }
-        return this.oldNodeReader ? Qee(i) : ZB(i, this.createImmutableLists)
+        return this.oldNodeReader ? Qee(i) : Z8(i, this.createImmutableLists)
     }
     tryReadChildFromCache(e) {
         if (this.oldNodeReader) {
             const t = this.positionMapper.getDistanceToNextChange(this.tokenizer.offset);
             if (t === null || !Sw(t)) {
                 const i = this.oldNodeReader.readLongestNodeAt(this.positionMapper.getOffsetBeforeChange(this.tokenizer.offset), n => t !== null && !tp(n.length, t) ? !1 : n.canBeReused(e));
                 if (i) return this._itemsFromCache++, this.tokenizer.skip(i.length), i
@@ -35520,15 +35520,15 @@
             c.push(h), d = Np(h.lengthAfter, d), n = u ?? t.dequeue()
         }
         return Sw(d) || c.push(new Sc(!1, d, d)), c
     }
     const r = [];
 
     function a(d, c, h) {
-        if (r.length > 0 && jB(r[r.length - 1].endOffset, d)) {
+        if (r.length > 0 && j8(r[r.length - 1].endOffset, d)) {
             const u = r[r.length - 1];
             r[r.length - 1] = new hl(u.startOffset, c, li(u.newLength, h))
         } else r.push({
             startOffset: d,
             endOffset: c,
             newLength: h
         })
@@ -35550,15 +35550,15 @@
 }
 class Sc {
     constructor(e, t, i) {
         this.modified = e, this.lengthBefore = t, this.lengthAfter = i
     }
     splitAt(e) {
         const t = Np(e, this.lengthAfter);
-        return jB(t, is) ? [this, void 0] : this.modified ? [new Sc(this.modified, this.lengthBefore, e), new Sc(this.modified, is, t)] : [new Sc(this.modified, e, e), new Sc(this.modified, t, t)]
+        return j8(t, is) ? [this, void 0] : this.modified ? [new Sc(this.modified, this.lengthBefore, e), new Sc(this.modified, is, t)] : [new Sc(this.modified, e, e), new Sc(this.modified, t, t)]
     }
     toString() {
         return `${this.modified?"M":"U"}:${ar(this.lengthBefore)} -> ${ar(this.lengthAfter)}`
     }
 }
 
 function jO(o) {
@@ -35573,15 +35573,15 @@
     return e
 }
 class nte extends z {
     didLanguageChange(e) {
         return this.brackets.didLanguageChange(e)
     }
     constructor(e, t) {
-        if (super(), this.textModel = e, this.getLanguageConfiguration = t, this.didChangeEmitter = new W, this.denseKeyProvider = new KB, this.brackets = new GB(this.denseKeyProvider, this.getLanguageConfiguration), this.onDidChange = this.didChangeEmitter.event, this.queuedTextEditsForInitialAstWithoutTokens = [], this.queuedTextEdits = [], e.tokenization.hasTokens) e.tokenization.backgroundTokenizationState === 2 ? (this.initialAstWithoutTokens = void 0, this.astWithTokens = this.parseDocumentFromTextBuffer([], void 0, !1)) : (this.initialAstWithoutTokens = this.parseDocumentFromTextBuffer([], void 0, !0), this.astWithTokens = this.initialAstWithoutTokens);
+        if (super(), this.textModel = e, this.getLanguageConfiguration = t, this.didChangeEmitter = new W, this.denseKeyProvider = new K8, this.brackets = new G8(this.denseKeyProvider, this.getLanguageConfiguration), this.onDidChange = this.didChangeEmitter.event, this.queuedTextEditsForInitialAstWithoutTokens = [], this.queuedTextEdits = [], e.tokenization.hasTokens) e.tokenization.backgroundTokenizationState === 2 ? (this.initialAstWithoutTokens = void 0, this.astWithTokens = this.parseDocumentFromTextBuffer([], void 0, !1)) : (this.initialAstWithoutTokens = this.parseDocumentFromTextBuffer([], void 0, !0), this.astWithTokens = this.initialAstWithoutTokens);
         else {
             const i = this.brackets.getSingleLanguageBracketTokens(this.textModel.getLanguageId()),
                 n = new Yee(this.textModel.getValue(), i);
             this.initialAstWithoutTokens = QI(n, [], void 0, !0), this.astWithTokens = this.initialAstWithoutTokens
         }
     }
     handleDidChangeBackgroundTokenizationState() {
@@ -35605,15 +35605,15 @@
         this.queuedTextEdits = i, this.initialAstWithoutTokens && !t && (this.queuedTextEditsForInitialAstWithoutTokens = Hv(this.queuedTextEditsForInitialAstWithoutTokens, e))
     }
     flushQueue() {
         this.queuedTextEdits.length > 0 && (this.astWithTokens = this.parseDocumentFromTextBuffer(this.queuedTextEdits, this.astWithTokens, !1), this.queuedTextEdits = []), this.queuedTextEditsForInitialAstWithoutTokens.length > 0 && (this.initialAstWithoutTokens && (this.initialAstWithoutTokens = this.parseDocumentFromTextBuffer(this.queuedTextEditsForInitialAstWithoutTokens, this.initialAstWithoutTokens, !1)), this.queuedTextEditsForInitialAstWithoutTokens = [])
     }
     parseDocumentFromTextBuffer(e, t, i) {
         const n = t,
-            s = new qB(this.textModel, this.brackets);
+            s = new q8(this.textModel, this.brackets);
         return QI(s, e, n, i)
     }
     getBracketsInRange(e, t) {
         this.flushQueue();
         const i = Ri(e.startLineNumber - 1, e.startColumn - 1),
             n = Ri(e.endLineNumber - 1, e.endColumn - 1);
         return new gl(s => {
@@ -35630,37 +35630,37 @@
                 a = new ste(s, t, this.textModel);
             eE(r, is, r.length, i, n, a, 0, new Map)
         })
     }
     getFirstBracketAfter(e) {
         this.flushQueue();
         const t = this.initialAstWithoutTokens || this.astWithTokens;
-        return XB(t, is, t.length, wc(e))
+        return X8(t, is, t.length, wc(e))
     }
     getFirstBracketBefore(e) {
         this.flushQueue();
         const t = this.initialAstWithoutTokens || this.astWithTokens;
-        return YB(t, is, t.length, wc(e))
+        return Y8(t, is, t.length, wc(e))
     }
 }
 
-function YB(o, e, t, i) {
+function Y8(o, e, t, i) {
     if (o.kind === 4 || o.kind === 2) {
         const n = [];
         for (const s of o.children) t = li(e, s.length), n.push({
             nodeOffsetStart: e,
             nodeOffsetEnd: t
         }), e = t;
         for (let s = n.length - 1; s >= 0; s--) {
             const {
                 nodeOffsetStart: r,
                 nodeOffsetEnd: a
             } = n[s];
             if (tp(r, i)) {
-                const l = YB(o.children[s], r, a, i);
+                const l = Y8(o.children[s], r, a, i);
                 if (l) return l
             }
         }
         return null
     } else {
         if (o.kind === 3) return null;
         if (o.kind === 1) {
@@ -35670,19 +35670,19 @@
                 range: n
             }
         }
     }
     return null
 }
 
-function XB(o, e, t, i) {
+function X8(o, e, t, i) {
     if (o.kind === 4 || o.kind === 2) {
         for (const n of o.children) {
             if (t = li(e, n.length), tp(i, t)) {
-                const s = XB(n, e, t, i);
+                const s = X8(n, e, t, i);
                 if (s) return s
             }
             e = t
         }
         return null
     } else {
         if (o.kind === 3) return null;
@@ -36212,15 +36212,15 @@
 nd.INSTANCE = new nd;
 
 function rC(o) {
     return o instanceof nd ? null : o
 }
 class ate extends z {
     constructor(e) {
-        super(), this.textModel = e, this.colorProvider = new QB, this.onDidChangeEmitter = new W, this.onDidChange = this.onDidChangeEmitter.event, this.colorizationOptions = e.getOptions().bracketPairColorizationOptions, this._register(e.bracketPairs.onDidChange(t => {
+        super(), this.textModel = e, this.colorProvider = new Q8, this.onDidChangeEmitter = new W, this.onDidChange = this.onDidChangeEmitter.event, this.colorizationOptions = e.getOptions().bracketPairColorizationOptions, this._register(e.bracketPairs.onDidChange(t => {
             this.onDidChangeEmitter.fire()
         }))
     }
     handleDidChangeOptions(e) {
         this.colorizationOptions = this.textModel.getOptions().bracketPairColorizationOptions
     }
     getDecorationsInRange(e, t, i, n) {
@@ -36234,28 +36234,28 @@
             range: r.range
         })).toArray() : []
     }
     getAllDecorations(e, t) {
         return e === void 0 ? [] : this.colorizationOptions.enabled ? this.getDecorationsInRange(new I(1, 1, this.textModel.getLineCount(), 1), e, t) : []
     }
 }
-class QB {
+class Q8 {
     constructor() {
         this.unexpectedClosingBracketClassName = "unexpected-closing-bracket"
     }
     getInlineClassName(e, t) {
         return e.isInvalid ? this.unexpectedClosingBracketClassName : this.getInlineClassNameOfLevel(t ? e.nestingLevelOfEqualBracketType : e.nestingLevel)
     }
     getInlineClassNameOfLevel(e) {
         return `bracket-highlighting-${e%30}`
     }
 }
 jr((o, e) => {
-    const t = [IB, EB, TB, NB, RB, MB],
-        i = new QB;
+    const t = [I8, E8, T8, N8, R8, M8],
+        i = new Q8;
     e.addRule(`.monaco-editor .${i.unexpectedClosingBracketClassName} { color: ${o.getColor(dJ)}; }`);
     const n = t.map(s => o.getColor(s)).filter(s => !!s).filter(s => !s.isTransparent());
     for (let s = 0; s < 30; s++) {
         const r = n[s % n.length];
         e.addRule(`.monaco-editor .${i.getInlineClassNameOfLevel(s)} { color: ${r}; }`)
     }
 });
@@ -36417,20 +36417,20 @@
     }
 }
 
 function Qd(o) {
     return o === 47 || o === 92
 }
 
-function JB(o) {
+function J8(o) {
     return o.replace(/[\\/]/g, Ki.sep)
 }
 
 function dte(o) {
-    return o.indexOf("/") === -1 && (o = JB(o)), /^[a-zA-Z]:(\/|$)/.test(o) && (o = "/" + o), o
+    return o.indexOf("/") === -1 && (o = J8(o)), /^[a-zA-Z]:(\/|$)/.test(o) && (o = "/" + o), o
 }
 
 function KO(o, e = Ki.sep) {
     if (!o) return "";
     const t = o.length,
         i = o.charCodeAt(0);
     if (Qd(i)) {
@@ -36440,15 +36440,15 @@
             for (; s < t && !Qd(o.charCodeAt(s)); s++);
             if (r !== s && !Qd(o.charCodeAt(s + 1))) {
                 for (s += 1; s < t; s++)
                     if (Qd(o.charCodeAt(s))) return o.slice(0, s + 1).replace(/[\\/]/g, e)
             }
         }
         return e
-    } else if (e8(i) && o.charCodeAt(1) === 58) return Qd(o.charCodeAt(2)) ? o.slice(0, 2) + e : o.slice(0, 2);
+    } else if (eB(i) && o.charCodeAt(1) === 58) return Qd(o.charCodeAt(2)) ? o.slice(0, 2) + e : o.slice(0, 2);
     let n = o.indexOf("://");
     if (n !== -1) {
         for (n += 3; n < t; n++)
             if (Qd(o.charCodeAt(n))) return o.slice(0, n + 1)
     }
     return ""
 }
@@ -36461,20 +36461,20 @@
         if (e.length === o.length) return !0;
         let s = e.length;
         return e.charAt(e.length - 1) === i && s--, o.charAt(s) === i
     }
     return e.charAt(e.length - 1) !== i && (e += i), o.indexOf(e) === 0
 }
 
-function e8(o) {
+function eB(o) {
     return o >= 65 && o <= 90 || o >= 97 && o <= 122
 }
 
 function cte(o, e = Zn) {
-    return e ? e8(o.charCodeAt(0)) && o.charCodeAt(1) === 58 : !1
+    return e ? eB(o.charCodeAt(0)) && o.charCodeAt(1) === 58 : !1
 }
 
 function Va(o) {
     return j1(o, !0)
 }
 class hte {
     constructor(e) {
@@ -36525,15 +36525,15 @@
             path: t
         })
     }
     relativePath(e, t) {
         if (e.scheme !== t.scheme || !GO(e.authority, t.authority)) return;
         if (e.scheme === it.file) {
             const s = Aj(Va(e), Va(t));
-            return Zn ? JB(s) : s
+            return Zn ? J8(s) : s
         }
         let i = e.path || "/";
         const n = t.path || "/";
         if (this._ignorePathCasing(e)) {
             let s = 0;
             for (const r = Math.min(i.length, n.length); s < r && !(i.charCodeAt(s) !== n.charCodeAt(s) && i.charAt(s).toLowerCase() !== n.charAt(s).toLowerCase()); s++);
             i = n.substr(0, s) + i.substr(s)
@@ -36685,15 +36685,15 @@
         const c = ta(t, i);
         i += 4;
         const h = [];
         for (let u = 0; u < c; u++) i = Wn.read(t, i, h);
         return new un(n, s, r, a, l, d, h)
     }
 }
-class t8 {
+class tB {
     get type() {
         return 0
     }
     get resource() {
         return Oe.isUri(this.model) ? this.model : this.model.uri
     }
     constructor(e, t, i, n) {
@@ -36795,15 +36795,15 @@
 
 function iE(o) {
     return o.getEOL() === `
 ` ? 0 : 1
 }
 
 function sd(o) {
-    return o ? o instanceof t8 || o instanceof _te : !1
+    return o ? o instanceof tB || o instanceof _te : !1
 }
 class vR {
     constructor(e, t) {
         this._model = e, this._undoRedoService = t
     }
     pushStackElement() {
         const e = this._undoRedoService.getLastElement(this._model.uri);
@@ -36815,15 +36815,15 @@
     }
     clear() {
         this._undoRedoService.removeElements(this._model.uri)
     }
     _getOrCreateEditStackElement(e, t) {
         const i = this._undoRedoService.getLastElement(this._model.uri);
         if (sd(i) && i.canAppend(this._model)) return i;
-        const n = new t8(p("edit", "Typing"), "undoredo.textBufferEdit", this._model, e);
+        const n = new tB(p("edit", "Typing"), "undoredo.textBufferEdit", this._model, e);
         return this._undoRedoService.pushElement(n, t), n
     }
     pushEOL(e) {
         const t = this._getOrCreateEditStackElement(null, void 0);
         this._model.setEOL(e), t.append(this._model, [], iE(this._model), this._model.getAlternativeVersionId(), null)
     }
     pushEditOperation(e, t, i, n) {
@@ -36936,23 +36936,23 @@
     return (o.metadata & 2) >>> 1 === 1
 }
 
 function Jt(o, e) {
     o.metadata = o.metadata & 253 | (e ? 1 : 0) << 1
 }
 
-function i8(o) {
+function iB(o) {
     return (o.metadata & 4) >>> 2 === 1
 }
 
 function XO(o, e) {
     o.metadata = o.metadata & 251 | (e ? 1 : 0) << 2
 }
 
-function n8(o) {
+function nB(o) {
     return (o.metadata & 64) >>> 6 === 1
 }
 
 function QO(o, e) {
     o.metadata = o.metadata & 191 | (e ? 1 : 0) << 6
 }
 
@@ -36967,15 +36967,15 @@
 function wte(o) {
     return (o.metadata & 32) >>> 5 === 1
 }
 
 function e4(o, e) {
     o.metadata = o.metadata & 223 | (e ? 1 : 0) << 5
 }
-class s8 {
+class sB {
     constructor(e, t, i) {
         this.metadata = 0, this.parent = this, this.left = this, this.right = this, ti(this, 1), this.start = t, this.end = i, this.delta = 0, this.maxEnd = i, this.id = e, this.ownerId = 0, this.options = null, XO(this, !1), QO(this, !1), JO(this, 1), e4(this, !1), this.cachedVersionId = 0, this.cachedAbsoluteStart = t, this.cachedAbsoluteEnd = i, this.range = null, Jt(this, !1)
     }
     reset(e, t, i, n) {
         this.start = t, this.end = i, this.maxEnd = i, this.cachedVersionId = e, this.cachedAbsoluteStart = t, this.cachedAbsoluteEnd = i, this.range = n
     }
     setOptions(e) {
@@ -36986,15 +36986,15 @@
     setCachedOffsets(e, t, i) {
         this.cachedVersionId !== i && (this.range = null), this.cachedVersionId = i, this.cachedAbsoluteStart = e, this.cachedAbsoluteEnd = t
     }
     detach() {
         this.parent = null, this.left = null, this.right = null
     }
 }
-const rt = new s8(null, 0, 0);
+const rt = new sB(null, 0, 0);
 rt.parent = rt;
 rt.left = rt;
 rt.right = rt;
 ti(rt, 0);
 class $x {
     constructor() {
         this.root = rt, this.requestNormalizeDelta = !1
@@ -37216,15 +37216,15 @@
         }
         if (s.left !== rt && !Gn(s.left)) {
             s = s.left;
             continue
         }
         a = r + s.start, l = r + s.end, s.setCachedOffsets(a, l, i);
         let h = !0;
-        if (e && s.ownerId && s.ownerId !== e && (h = !1), t && i8(s) && (h = !1), n && !n8(s) && (h = !1), h && (d[c++] = s), Jt(s, !0), s.right !== rt && !Gn(s.right)) {
+        if (e && s.ownerId && s.ownerId !== e && (h = !1), t && iB(s) && (h = !1), n && !nB(s) && (h = !1), h && (d[c++] = s), Jt(s, !0), s.right !== rt && !Gn(s.right)) {
             r += s.delta, s = s.right;
             continue
         }
     }
     return Jt(o.root, !1), d
 }
 
@@ -37254,15 +37254,15 @@
         if (c = l + a.start, c > t) {
             Jt(a, !0);
             continue
         }
         if (h = l + a.end, h >= e) {
             a.setCachedOffsets(c, h, s);
             let f = !0;
-            i && a.ownerId && a.ownerId !== i && (f = !1), n && i8(a) && (f = !1), r && !n8(a) && (f = !1), f && (u[g++] = a)
+            i && a.ownerId && a.ownerId !== i && (f = !1), n && iB(a) && (f = !1), r && !nB(a) && (f = !1), f && (u[g++] = a)
         }
         if (Jt(a, !0), a.right !== rt && !Gn(a.right)) {
             l += a.delta, a = a.right;
             continue
         }
     }
     return Jt(o.root, !1), u
@@ -37332,34 +37332,34 @@
 }
 
 function $_(o, e) {
     const t = e.left;
     e.delta -= t.delta, (e.delta < -1073741824 || e.delta > 1073741824) && (o.requestNormalizeDelta = !0), e.start -= t.delta, e.end -= t.delta, e.left = t.right, t.right !== rt && (t.right.parent = e), t.parent = e.parent, e.parent === rt ? o.root = t : e === e.parent.right ? e.parent.right = t : e.parent.left = t, t.right = e, e.parent = t, oh(e), oh(t)
 }
 
-function o8(o) {
+function oB(o) {
     let e = o.end;
     if (o.left !== rt) {
         const t = o.left.maxEnd;
         t > e && (e = t)
     }
     if (o.right !== rt) {
         const t = o.right.maxEnd + o.delta;
         t > e && (e = t)
     }
     return e
 }
 
 function oh(o) {
-    o.maxEnd = o8(o)
+    o.maxEnd = oB(o)
 }
 
 function ac(o) {
     for (; o !== rt;) {
-        const e = o8(o);
+        const e = oB(o);
         if (o.maxEnd === e) return;
         o.maxEnd = e, o = o.parent
     }
 }
 
 function Rte(o, e, t, i) {
     return o === t ? e - i : o - t
@@ -37371,15 +37371,15 @@
     next() {
         if (this.right !== Ye) return bR(this.right);
         let e = this;
         for (; e.parent !== Ye && e.parent.left !== e;) e = e.parent;
         return e.parent === Ye ? Ye : e.parent
     }
     prev() {
-        if (this.left !== Ye) return r8(this.left);
+        if (this.left !== Ye) return rB(this.left);
         let e = this;
         for (; e.parent !== Ye && e.parent.right !== e;) e = e.parent;
         return e.parent === Ye ? Ye : e.parent
     }
     detach() {
         this.parent = null, this.left = null, this.right = null
     }
@@ -37391,15 +37391,15 @@
 Ye.color = 0;
 
 function bR(o) {
     for (; o.left !== Ye;) o = o.left;
     return o
 }
 
-function r8(o) {
+function rB(o) {
     for (; o.right !== Ye;) o = o.right;
     return o
 }
 
 function CR(o) {
     return o === Ye ? 0 : o.size_left + o.piece.length + CR(o.right)
 }
@@ -37469,15 +37469,15 @@
         for (; e !== o.root && e === e.parent.right;) e = e.parent;
         if (e !== o.root)
             for (e = e.parent, t = CR(e.left) - e.size_left, i = wR(e.left) - e.lf_left, e.size_left += t, e.lf_left += i; e !== o.root && (t !== 0 || i !== 0);) e.parent.left === e && (e.parent.size_left += t, e.parent.lf_left += i), e = e.parent
     }
 }
 const Hl = 65535;
 
-function a8(o) {
+function aB(o) {
     let e;
     return o[o.length - 1] < 65536 ? e = new Uint16Array(o.length) : e = new Uint32Array(o.length), e.set(o, 0), e
 }
 class Mte {
     constructor(e, t, i, n, s) {
         this.lineStarts = e, this.cr = t, this.lf = i, this.crlf = n, this.isBasicASCII = s
     }
@@ -37486,29 +37486,29 @@
 function Ql(o, e = !0) {
     const t = [0];
     let i = 1;
     for (let n = 0, s = o.length; n < s; n++) {
         const r = o.charCodeAt(n);
         r === 13 ? n + 1 < s && o.charCodeAt(n + 1) === 10 ? (t[i++] = n + 2, n++) : t[i++] = n + 1 : r === 10 && (t[i++] = n + 1)
     }
-    return e ? a8(t) : t
+    return e ? aB(t) : t
 }
 
 function Ate(o, e) {
     o.length = 0, o[0] = 0;
     let t = 1,
         i = 0,
         n = 0,
         s = 0,
         r = !0;
     for (let l = 0, d = e.length; l < d; l++) {
         const c = e.charCodeAt(l);
         c === 13 ? l + 1 < d && e.charCodeAt(l + 1) === 10 ? (s++, o[t++] = l + 2, l++) : (i++, o[t++] = l + 1) : c === 10 ? (n++, o[t++] = l + 1) : r && c !== 9 && (c < 32 || c > 126) && (r = !1)
     }
-    const a = new Mte(a8(o), i, n, s, r);
+    const a = new Mte(aB(o), i, n, s, r);
     return o.length = 0, a
 }
 class to {
     constructor(e, t, i, n, s) {
         this.bufferIndex = e, this.start = t, this.end = i, this.lineFeedCnt = n, this.length = s
     }
 }
@@ -38333,15 +38333,15 @@
         return n4(this, i), i
     }
     rbInsertLeft(e, t) {
         const i = new nE(t, 1);
         if (i.left = Ye, i.right = Ye, i.parent = Ye, i.size_left = 0, i.lf_left = 0, this.root === Ye) this.root = i, i.color = 0;
         else if (e.left === Ye) e.left = i, i.parent = e;
         else {
-            const n = r8(e.left);
+            const n = rB(e.left);
             n.right = i, i.parent = n
         }
         return n4(this, i), i
     }
 }
 class np extends z {
     constructor(e, t, i, n, s, r, a) {
@@ -38668,15 +38668,15 @@
         const n = new np(i, this._bom, t, this._containsRTL, this._containsUnusualLineTerminators, this._isBasicASCII, this._normalizeEOL);
         return {
             textBuffer: n,
             disposable: n
         }
     }
 }
-class l8 {
+class lB {
     constructor() {
         this.chunks = [], this.BOM = "", this._hasPreviousChar = !1, this._previousChar = 0, this._tmpLineStarts = [], this.cr = 0, this.lf = 0, this.crlf = 0, this.containsRTL = !1, this.containsUnusualLineTerminators = !1, this.isBasicASCII = !0
     }
     acceptChunk(e) {
         if (e.length === 0) return;
         this.chunks.length === 0 && R2(e) && (this.BOM = rK, e = e.substr(1));
         const t = e.charCodeAt(e.length - 1);
@@ -39298,15 +39298,15 @@
         }
         return i
     }
     acceptEdit(e, t, i, n, s) {
         for (const r of this._pieces) r.acceptEdit(e, t, i, n, s)
     }
 }
-class xw extends HB {
+class xw extends H8 {
     constructor(e, t, i, n, s, r) {
         super(), this._languageService = e, this._languageConfigurationService = t, this._textModel = i, this._bracketPairsTextModelPart = n, this._languageId = s, this._attachedViews = r, this._semanticTokens = new SR(this._languageService.languageIdCodec), this._onDidChangeLanguage = this._register(new W), this.onDidChangeLanguage = this._onDidChangeLanguage.event, this._onDidChangeLanguageConfiguration = this._register(new W), this.onDidChangeLanguageConfiguration = this._onDidChangeLanguageConfiguration.event, this._onDidChangeTokens = this._register(new W), this.onDidChangeTokens = this._onDidChangeTokens.event, this.grammarTokens = this._register(new qte(this._languageService.languageIdCodec, this._textModel, () => this._languageId, this._attachedViews)), this._register(this._languageConfigurationService.onDidChange(a => {
             a.affects(this._languageId) && this._onDidChangeLanguageConfiguration.fire({})
         })), this._register(this.grammarTokens.onDidChangeTokens(a => {
             this._emitModelTokensChangedEvent(a)
         })), this._register(this.grammarTokens.onDidChangeBackgroundTokenizationState(a => {
             this._bracketPairsTextModelPart.handleDidChangeBackgroundTokenizationState()
@@ -39661,15 +39661,15 @@
         const i = [].concat(e.changes).concat(t.changes),
             n = t.versionId,
             s = e.isUndoing || t.isUndoing,
             r = e.isRedoing || t.isRedoing;
         return new sp(i, n, s, r)
     }
 }
-class d8 {
+class dB {
     constructor(e) {
         this.changes = e
     }
 }
 class Ru {
     constructor(e, t) {
         this.rawContentChangedEvent = e, this.contentChangedEvent = t
@@ -39695,15 +39695,15 @@
             isUndoing: r,
             isRedoing: a,
             isFlush: l
         }
     }
 }
 const Iy = ht("undoRedoService");
-class c8 {
+class cB {
     constructor(e, t) {
         this.resource = e, this.elements = t
     }
 }
 class Rp {
     constructor() {
         this.id = Rp._ID++, this.order = 1
@@ -39736,20 +39736,20 @@
     Kx = globalThis && globalThis.__param || function(o, e) {
         return function(t, i) {
             e(t, i, o)
         }
     };
 
 function eie(o) {
-    const e = new l8;
+    const e = new lB;
     return e.acceptChunk(o), e.finish()
 }
 
 function tie(o) {
-    const e = new l8;
+    const e = new lB;
     let t;
     for (; typeof(t = o.read()) == "string";) e.acceptChunk(t);
     return e.finish()
 }
 
 function r4(o, e) {
     let t;
@@ -40416,15 +40416,15 @@
     }
     canRedo() {
         return this._undoRedoService.canRedo(this.uri)
     }
     handleBeforeFireDecorationsChangedEvent(e) {
         if (e === null || e.size === 0) return;
         const i = Array.from(e).map(n => new o4(n, this.getLineContent(n), this._getInjectedTextInLine(n)));
-        this._onDidChangeInjectedText.fire(new d8(i))
+        this._onDidChangeInjectedText.fire(new dB(i))
     }
     changeDecorations(e, t = 0) {
         this._assertNotDisposed();
         try {
             return this._onDidChangeDecorations.beginDeferredEmit(), this._changeDecorations(t, e)
         } finally {
             this._onDidChangeDecorations.endDeferredEmit()
@@ -40594,15 +40594,15 @@
                         this._decorationsTree.delete(h), n || this._onDidChangeDecorations.checkAffectedAndFire(h.options)
                     }
                 }
                 if (d < l) {
                     if (!h) {
                         const v = ++this._lastDecorationId,
                             b = `${this._instanceId};${v}`;
-                        h = new s8(b, 0, 0), this._decorations[b] = h
+                        h = new sB(b, 0, 0), this._decorations[b] = h
                     }
                     const u = i[d],
                         g = this._validateRangeRelaxedNoAllocations(u.range),
                         f = d4(u.options),
                         m = this._buffer.getOffsetAt(g.startLineNumber, g.startColumn),
                         _ = this._buffer.getOffsetAt(g.endLineNumber, g.endColumn);
                     h.ownerId = e, h.reset(s, m, _, g), h.setOptions(f), h.options.after && this._onDidChangeDecorations.recordLineAffectedByInjectedText(g.endLineNumber), h.options.before && this._onDidChangeDecorations.recordLineAffectedByInjectedText(g.startLineNumber), n || this._onDidChangeDecorations.checkAffectedAndFire(f), this._decorationsTree.insert(h), c[d] = h.id, d++
@@ -40744,20 +40744,20 @@
         this._decorationsTree0.acceptReplace(e, t, i, n), this._decorationsTree1.acceptReplace(e, t, i, n), this._injectedTextDecorationsTree.acceptReplace(e, t, i, n)
     }
 }
 
 function zl(o) {
     return o.replace(/[^a-z0-9\-_]/gi, " ")
 }
-class h8 {
+class hB {
     constructor(e) {
         this.color = e.color || "", this.darkColor = e.darkColor || ""
     }
 }
-class rie extends h8 {
+class rie extends hB {
     constructor(e) {
         super(e), this._resolvedColor = null, this.position = typeof e.position == "number" ? e.position : Fo.Center
     }
     getColor(e) {
         return this._resolvedColor || (e.type !== "light" && this.darkColor ? this._resolvedColor = this._resolveColor(this.darkColor, e) : this._resolvedColor = this._resolveColor(this.color, e)), this._resolvedColor
     }
     invalidateCachedColor() {
@@ -40771,15 +40771,15 @@
 }
 class aie {
     constructor(e) {
         var t;
         this.position = (t = e == null ? void 0 : e.position) !== null && t !== void 0 ? t : jf.Left
     }
 }
-class lie extends h8 {
+class lie extends hB {
     constructor(e) {
         super(e), this.position = e.position
     }
     getColor(e) {
         return this._resolvedColor || (e.type !== "light" && this.darkColor ? this._resolvedColor = this._resolveColor(this.darkColor, e) : this._resolvedColor = this._resolveColor(this.color, e)), this._resolvedColor
     }
     invalidateCachedColor() {
@@ -41149,15 +41149,15 @@
     }
 }
 class hC {
     constructor() {
         this.type = 8
     }
 }
-class u8 {
+class uB {
     constructor(e, t) {
         this.fromLineNumber = e, this.count = t, this.type = 9
     }
 }
 class rE {
     constructor(e, t) {
         this.type = 10, this.fromLineNumber = e, this.toLineNumber = t
@@ -41520,15 +41520,15 @@
                 positionLineNumber: a,
                 positionColumn: l
             })
         }
         this.setStates(e, "restoreState", 0, Ct.fromModelSelections(i)), this.revealPrimary(e, "restoreState", !1, 0, !0, 1)
     }
     onModelContentChanged(e, t) {
-        if (t instanceof d8) {
+        if (t instanceof dB) {
             if (this._isHandling) return;
             this._isHandling = !0;
             try {
                 this.setStates(e, "modelChange", 0, this.getCursorStates())
             } finally {
                 this._isHandling = !1
             }
@@ -41607,15 +41607,15 @@
         const t = Oie.executeCommands(this._model, this._cursors.getSelections(), e.commands);
         if (t) {
             this._interpretCommandResult(t);
             const i = [],
                 n = [];
             for (let s = 0; s < e.commands.length; s++) {
                 const r = e.commands[s];
-                r instanceof OB && r.enclosingRange && r.closeCharacterRange && (i.push(r.closeCharacterRange), n.push(r.enclosingRange))
+                r instanceof O8 && r.enclosingRange && r.closeCharacterRange && (i.push(r.closeCharacterRange), n.push(r.enclosingRange))
             }
             i.length > 0 && this._pushAutoClosedAction(i, n), this._prevEditOperationType = e.type
         }
         e.shouldPushStackElementAfter && this._model.pushStackElement()
     }
     _interpretCommandResult(e) {
         (!e || e.length === 0) && (e = this._cursors.readSelectionFromMarkers()), this._columnSelectData = null, this._cursors.setSelections(e), this._cursors.normalize()
@@ -42746,22 +42746,22 @@
 }
 
 function DR(o, e) {
     return !(e.options.hideInCommentTokens && kR(o, e) || e.options.hideInStringTokens && IR(o, e))
 }
 
 function kR(o, e) {
-    return g8(o, e.range, t => t === 1)
+    return gB(o, e.range, t => t === 1)
 }
 
 function IR(o, e) {
-    return g8(o, e.range, t => t === 2)
+    return gB(o, e.range, t => t === 2)
 }
 
-function g8(o, e, t) {
+function gB(o, e, t) {
     for (let i = e.startLineNumber; i <= e.endLineNumber; i++) {
         const n = o.tokenization.getLineTokens(i),
             s = i === e.startLineNumber,
             r = i === e.endLineNumber;
         let a = s ? n.findTokenIndexAtOffset(e.startColumn - 1) : 0;
         for (; a < n.getCount() && !(r && n.getStartOffset(a) > e.endColumn - 1);) {
             if (!t(n.getStandardTokenType(a))) return !1;
@@ -43158,15 +43158,15 @@
             c = 0,
             h = -1,
             u = 0,
             g = -1,
             f = 0,
             m = -1;
         s > l ? (c = this.projectedModelLineLineCounts.getPrefixSum(t - 1) + 1, h = c + l - 1, f = h + 1, m = f + (s - l) - 1, d = !0) : s < l ? (c = this.projectedModelLineLineCounts.getPrefixSum(t - 1) + 1, h = c + s - 1, u = h + 1, g = u + (l - s) - 1, d = !0) : (c = this.projectedModelLineLineCounts.getPrefixSum(t - 1) + 1, h = c + l - 1), this.projectedModelLineLineCounts.setValue(n, l);
-        const _ = c <= h ? new u8(c, h - c + 1) : null,
+        const _ = c <= h ? new uB(c, h - c + 1) : null,
             v = u <= g ? new aE(u, g) : null,
             b = f <= m ? new rE(f, m) : null;
         return [d, _, v, b]
     }
     acceptVersionId(e) {
         this._validModelVersionId = e, this.modelLineProjections.length === 1 && !this.modelLineProjections[0].isVisible() && this.setHiddenAreas([])
     }
@@ -43531,15 +43531,15 @@
     onModelLinesDeleted(e, t, i) {
         return new rE(t, i)
     }
     onModelLinesInserted(e, t, i, n) {
         return new aE(t, i)
     }
     onModelLineChanged(e, t, i) {
-        return [!1, new u8(t, 1), null, null]
+        return [!1, new uB(t, 1), null, null]
     }
     acceptVersionId(e) {}
     getViewLineCount() {
         return this.model.getLineCount()
     }
     getActiveIndentGuide(e, t, i) {
         return {
@@ -44544,15 +44544,15 @@
 function rne(o, e, t, i, n, s, r, a) {
     if (n === -1) return null;
     const l = t.length;
     if (l <= 1) return null;
     const d = a === "keepAll",
         c = e.breakOffsets,
         h = e.breakOffsetsVisibleColumn,
-        u = f8(t, i, n, s, r),
+        u = fB(t, i, n, s, r),
         g = n - u,
         f = lE,
         m = dE;
     let _ = 0,
         v = 0,
         b = 0,
         C = n;
@@ -44647,15 +44647,15 @@
 function ane(o, e, t, i, n, s, r, a) {
     const l = La.applyInjectedText(e, t);
     let d, c;
     if (t && t.length > 0 ? (d = t.map(L => L.options), c = t.map(L => L.column - 1)) : (d = null, c = null), n === -1) return d ? new G_(c, d, [l.length], [], 0) : null;
     const h = l.length;
     if (h <= 1) return d ? new G_(c, d, [l.length], [], 0) : null;
     const u = a === "keepAll",
-        g = f8(l, i, n, s, r),
+        g = fB(l, i, n, s, r),
         f = n - g,
         m = [],
         _ = [];
     let v = 0,
         b = 0,
         C = 0,
         w = n,
@@ -44681,15 +44681,15 @@
     return e - o % e
 }
 
 function cE(o, e, t, i, n) {
     return t !== 32 && (e === 2 && i !== 2 || e !== 1 && i === 1 || !n && e === 3 && i !== 2 || !n && i === 3 && e !== 1)
 }
 
-function f8(o, e, t, i, n) {
+function fB(o, e, t, i, n) {
     let s = 0;
     if (n !== 0) {
         const r = ms(o);
         if (r !== -1) {
             for (let l = 0; l < r; l++) {
                 const d = o.charCodeAt(l) === 9 ? S4(s, e) : 1;
                 s += d
@@ -44872,37 +44872,37 @@
         d = Qx(o, e, t[l], t[l + 1]);
     hE(o, e, t, i, n, l, d, a), hE(o, e, t, l, d, s, r, a)
 }
 
 function Qx(o, e, t, i) {
     return o.setStart(e[t / 16384 | 0].firstChild, t % 16384), o.setEnd(e[i / 16384 | 0].firstChild, i % 16384), o.getClientRects()
 }
-const p8 = {
+const pB = {
     value: p("accessibleDiffViewer", "Accessible Diff Viewer"),
     original: "Accessible Diff Viewer"
 };
 class pm extends Ta {
     constructor() {
         super({
             id: pm.id,
             title: {
                 value: p("editor.action.accessibleDiffViewer.next", "Go to Next Difference"),
                 original: "Go to Next Difference"
             },
-            category: p8,
+            category: pB,
             precondition: te.has("isInDiffEditor"),
             keybinding: {
                 primary: 65,
                 weight: 100
             },
             f1: !0
         })
     }
     run(e) {
-        const t = m8(e);
+        const t = mB(e);
         t == null || t.accessibleDiffViewerNext()
     }
 }
 pm.id = "editor.action.accessibleDiffViewer.next";
 ts.appendMenuItem(R.EditorTitle, {
     command: {
         id: pm.id,
@@ -44916,31 +44916,31 @@
     constructor() {
         super({
             id: o0.id,
             title: {
                 value: p("editor.action.accessibleDiffViewer.prev", "Go to Previous Difference"),
                 original: "Go to Previous Difference"
             },
-            category: p8,
+            category: pB,
             precondition: te.has("isInDiffEditor"),
             keybinding: {
                 primary: 1089,
                 weight: 100
             },
             f1: !0
         })
     }
     run(e) {
-        const t = m8(e);
+        const t = mB(e);
         t == null || t.accessibleDiffViewerPrev()
     }
 }
 o0.id = "editor.action.accessibleDiffViewer.prev";
 
-function m8(o) {
+function mB(o) {
     var e;
     const t = o.get(St),
         i = t.listDiffEditors(),
         n = (e = t.getFocusedCodeEditor()) !== null && e !== void 0 ? e : t.getActiveCodeEditor();
     if (!n) return null;
     for (let s = 0, r = i.length; s < r; s++) {
         const a = i[s];
@@ -45136,15 +45136,15 @@
             let f;
             Array.isArray(i.contributions) ? f = i.contributions : f = Du.getEditorContributions(), this._contributions.initialize(this, f, this._instantiationService);
             for (const _ of Du.getEditorActions()) {
                 if (this._actions.has(_.id)) {
                     Xe(new Error(`Cannot have two actions with the same id ${_.id}`));
                     continue
                 }
-                const v = new UB(_.id, _.label, _.alias, jn(_.precondition), () => this._instantiationService.invokeFunction(b => Promise.resolve(_.runEditorCommand(b, this, null))), this._contextKeyService);
+                const v = new U8(_.id, _.label, _.alias, jn(_.precondition), () => this._instantiationService.invokeFunction(b => Promise.resolve(_.runEditorCommand(b, this, null))), this._contextKeyService);
                 this._actions.set(v.id, v)
             }
             const m = () => !this._configuration.options.get(89) && this._configuration.options.get(35).enabled;
             this._register(new rY(this._domElement, {
                 onDragEnter: () => {},
                 onDragOver: _ => {
                     if (!m()) return;
@@ -46572,35 +46572,35 @@
         for (let i = 0, n = o.length; i < n; i++) {
             const s = o[i](e, t);
             if (s) return s
         }
         return null
     }
 }
-_8.bind(void 0, !1);
-const Ty = _8.bind(void 0, !0);
+_B.bind(void 0, !1);
+const Ty = _B.bind(void 0, !0);
 
-function _8(o, e, t) {
+function _B(o, e, t) {
     if (!t || t.length < e.length) return null;
     let i;
     return o ? i = k2(t, e) : i = t.indexOf(e) === 0, i ? e.length > 0 ? [{
         start: 0,
         end: e.length
     }] : [] : null
 }
 
-function v8(o, e) {
+function vB(o, e) {
     const t = e.toLowerCase().indexOf(o.toLowerCase());
     return t === -1 ? null : [{
         start: t,
         end: t + o.length
     }]
 }
 
-function b8(o, e) {
+function bB(o, e) {
     return uE(o.toLowerCase(), e.toLowerCase(), 0, 0)
 }
 
 function uE(o, e, t, i) {
     if (t === o.length) return [];
     if (i === e.length) return null;
     if (o[t] === e[i]) {
@@ -46621,66 +46621,66 @@
     return 65 <= o && o <= 90
 }
 
 function OR(o) {
     return 48 <= o && o <= 57
 }
 
-function C8(o) {
+function CB(o) {
     return o === 32 || o === 9 || o === 10 || o === 13
 }
-const w8 = new Set;
-"()[]{}<>`'\"-/;:,.?!".split("").forEach(o => w8.add(o.charCodeAt(0)));
+const wB = new Set;
+"()[]{}<>`'\"-/;:,.?!".split("").forEach(o => wB.add(o.charCodeAt(0)));
 
 function Rw(o) {
-    return C8(o) || w8.has(o)
+    return CB(o) || wB.has(o)
 }
 
 function Mne(o, e) {
     return o === e || Rw(o) && Rw(e)
 }
 
-function S8(o) {
+function SB(o) {
     return PR(o) || Ny(o) || OR(o)
 }
 
 function FR(o, e) {
     return e.length === 0 ? e = [o] : o.end === e[0].start ? e[0].start = o.start : e.unshift(o), e
 }
 
-function y8(o, e) {
+function yB(o, e) {
     for (let t = e; t < o.length; t++) {
         const i = o.charCodeAt(t);
-        if (Ny(i) || OR(i) || t > 0 && !S8(o.charCodeAt(t - 1))) return t
+        if (Ny(i) || OR(i) || t > 0 && !SB(o.charCodeAt(t - 1))) return t
     }
     return o.length
 }
 
 function gE(o, e, t, i) {
     if (t === o.length) return [];
     if (i === e.length) return null;
     if (o[t] !== e[i].toLowerCase()) return null;
     {
         let n = null,
             s = i + 1;
-        for (n = gE(o, e, t + 1, i + 1); !n && (s = y8(e, s)) < e.length;) n = gE(o, e, t + 1, s), s++;
+        for (n = gE(o, e, t + 1, i + 1); !n && (s = yB(e, s)) < e.length;) n = gE(o, e, t + 1, s), s++;
         return n === null ? null : FR({
             start: i,
             end: i + 1
         }, n)
     }
 }
 
 function Ane(o) {
     let e = 0,
         t = 0,
         i = 0,
         n = 0,
         s = 0;
-    for (let c = 0; c < o.length; c++) s = o.charCodeAt(c), Ny(s) && e++, PR(s) && t++, S8(s) && i++, OR(s) && n++;
+    for (let c = 0; c < o.length; c++) s = o.charCodeAt(c), Ny(s) && e++, PR(s) && t++, SB(s) && i++, OR(s) && n++;
     const r = e / o.length,
         a = t / o.length,
         l = i / o.length,
         d = n / o.length;
     return {
         upperPercent: r,
         lowerPercent: a,
@@ -46708,61 +46708,61 @@
 }
 
 function Fne(o) {
     let e = 0,
         t = 0,
         i = 0,
         n = 0;
-    for (let s = 0; s < o.length; s++) i = o.charCodeAt(s), Ny(i) && e++, PR(i) && t++, C8(i) && n++;
+    for (let s = 0; s < o.length; s++) i = o.charCodeAt(s), Ny(i) && e++, PR(i) && t++, CB(i) && n++;
     return (e === 0 || t === 0) && n === 0 ? o.length <= 30 : e <= 5
 }
 
-function L8(o, e) {
+function LB(o, e) {
     if (!e || (e = e.trim(), e.length === 0) || !Fne(o) || e.length > 60) return null;
     const t = Ane(e);
     if (!One(t)) {
         if (!Pne(t)) return null;
         e = e.toLowerCase()
     }
     let i = null,
         n = 0;
-    for (o = o.toLowerCase(); n < e.length && (i = gE(o, e, 0, n)) === null;) n = y8(e, n + 1);
+    for (o = o.toLowerCase(); n < e.length && (i = gE(o, e, 0, n)) === null;) n = yB(e, n + 1);
     return i
 }
 
 function Bne(o, e, t = !1) {
     if (!e || e.length === 0) return null;
     let i = null,
         n = 0;
-    for (o = o.toLowerCase(), e = e.toLowerCase(); n < e.length && (i = fE(o, e, 0, n, t)) === null;) n = x8(e, n + 1);
+    for (o = o.toLowerCase(), e = e.toLowerCase(); n < e.length && (i = fE(o, e, 0, n, t)) === null;) n = xB(e, n + 1);
     return i
 }
 
 function fE(o, e, t, i, n) {
     if (t === o.length) return [];
     if (i === e.length) return null;
     if (Mne(o.charCodeAt(t), e.charCodeAt(i))) {
         let s = null,
             r = i + 1;
         if (s = fE(o, e, t + 1, i + 1, n), !n)
-            for (; !s && (r = x8(e, r)) < e.length;) s = fE(o, e, t + 1, r, n), r++;
+            for (; !s && (r = xB(e, r)) < e.length;) s = fE(o, e, t + 1, r, n), r++;
         return s ? o.charCodeAt(t) !== e.charCodeAt(i) ? s : FR({
             start: i,
             end: i + 1
         }, s) : null
     } else return null
 }
 
-function x8(o, e) {
+function xB(o, e) {
     for (let t = e; t < o.length; t++)
         if (Rw(o.charCodeAt(t)) || t > 0 && Rw(o.charCodeAt(t - 1))) return t;
     return o.length
 }
-const Wne = AR(Ty, L8, v8),
-    Vne = AR(Ty, L8, b8),
+const Wne = AR(Ty, LB, vB),
+    Vne = AR(Ty, LB, bB),
     k4 = new xh(1e4);
 
 function I4(o, e, t = !1) {
     if (typeof o != "string" || typeof e != "string") return null;
     let i = k4.get(o);
     i || (i = new RegExp(Jj(o), "i"), k4.set(o, i));
     const n = i.exec(e);
@@ -46804,21 +46804,21 @@
     const o = [],
         e = [];
     for (let t = 0; t <= yc; t++) e[t] = 0;
     for (let t = 0; t <= yc; t++) o.push(e.slice(0));
     return o
 }
 
-function D8(o) {
+function DB(o) {
     const e = [];
     for (let t = 0; t <= o; t++) e[t] = 0;
     return e
 }
-const k8 = D8(2 * yc),
-    pE = D8(2 * yc),
+const kB = DB(2 * yc),
+    pE = DB(2 * yc),
     Ul = BR(),
     Vh = BR(),
     gC = BR();
 
 function fC(o, e) {
     if (e < 0 || e >= o.length) return !1;
     const t = o.codePointAt(e);
@@ -46861,15 +46861,15 @@
 }
 
 function b1(o, e, t) {
     return e[o] !== t[o]
 }
 
 function zne(o, e, t, i, n, s, r = !1) {
-    for (; e < t && n < s;) o[e] === i[n] && (r && (k8[e] = n), e += 1), n += 1;
+    for (; e < t && n < s;) o[e] === i[n] && (r && (kB[e] = n), e += 1), n += 1;
     return e === t
 }
 var wa;
 (function(o) {
     o.Default = [-100, 0];
 
     function e(t) {
@@ -46894,15 +46894,15 @@
     $ne(a, l, t, s, e, n);
     let d = 1,
         c = 1,
         h = t,
         u = s;
     const g = [!1];
     for (d = 1, h = t; h < a; d++, h++) {
-        const b = k8[h],
+        const b = kB[h],
             C = pE[h],
             w = h + 1 < a ? pE[h + 1] : l;
         for (c = b - s + 1, u = b; u < w; c++, u++) {
             let S = Number.MIN_SAFE_INTEGER,
                 k = !1;
             u <= C && (S = Une(o, e, h, t, i, n, u, l, s, Ul[d - 1][c - 1] === 0, g));
             let y = 0;
@@ -47220,15 +47220,15 @@
     }
     dispose() {
         var e, t;
         (e = this._hoverWidget) === null || e === void 0 || e.dispose(), (t = this._cancellationTokenSource) === null || t === void 0 || t.dispose(!0), this._cancellationTokenSource = void 0
     }
 }
 
-function I8(o, e, t, i) {
+function IB(o, e, t, i) {
     let n, s;
     const r = (h, u) => {
             var g;
             const f = s !== void 0;
             h && (s == null || s.dispose(), s = void 0), u && (n == null || n.dispose(), n = void 0), f && ((g = o.onDidHideHover) === null || g === void 0 || g.call(o))
         },
         a = (h, u, g) => new $r(() => mE(this, void 0, void 0, function*() {
@@ -47273,15 +47273,15 @@
 function rse(o, e = {}) {
     const t = HR(e);
     return t.textContent = o, t
 }
 
 function ase(o, e = {}) {
     const t = HR(e);
-    return E8(t, dse(o, !!e.renderCodeSegments), e.actionHandler, e.renderCodeSegments), t
+    return EB(t, dse(o, !!e.renderCodeSegments), e.actionHandler, e.renderCodeSegments), t
 }
 
 function HR(o) {
     const e = o.inline ? "span" : "div",
         t = document.createElement(e);
     return o.className && (t.className = o.className), t
 }
@@ -47300,28 +47300,28 @@
         return this.source[this.index]
     }
     advance() {
         this.index++
     }
 }
 
-function E8(o, e, t, i) {
+function EB(o, e, t, i) {
     let n;
     if (e.type === 2) n = document.createTextNode(e.content || "");
     else if (e.type === 3) n = document.createElement("b");
     else if (e.type === 4) n = document.createElement("i");
     else if (e.type === 7 && i) n = document.createElement("code");
     else if (e.type === 5 && t) {
         const s = document.createElement("a");
         t.disposables.add(Ai(s, "click", r => {
             t.callback(String(e.index), r)
         })), n = s
     } else e.type === 8 ? n = document.createElement("br") : e.type === 1 && (n = o);
     n && o !== n && o.appendChild(n), n && Array.isArray(e.children) && e.children.forEach(s => {
-        E8(n, s, t, i)
+        EB(n, s, t, i)
     })
 }
 
 function dse(o, e) {
     const t = {
         type: 1,
         children: []
@@ -49181,15 +49181,15 @@
         this.spliceables.forEach(n => n.splice(e, t, i))
     }
 }
 
 function so(o, e, t) {
     return Math.min(Math.max(o, e), t)
 }
-class T8 {
+class TB {
     constructor() {
         this._n = 1, this._val = 0
     }
     update(e) {
         return this._val = this._val + (e - this._val) / this._n, this._n += 1, this._val
     }
     get value() {
@@ -50230,18 +50230,18 @@
     return o.tagName === "INPUT" || o.tagName === "TEXTAREA"
 }
 
 function Rf(o) {
     return o.classList.contains("monaco-editor") ? !0 : o.classList.contains("monaco-list") || !o.parentElement ? !1 : Rf(o.parentElement)
 }
 
-function N8(o) {
-    return o.tagName === "A" && o.classList.contains("monaco-button") || o.tagName === "DIV" && o.classList.contains("monaco-button-dropdown") ? !0 : o.classList.contains("monaco-list") || !o.parentElement ? !1 : N8(o.parentElement)
+function NB(o) {
+    return o.tagName === "A" && o.classList.contains("monaco-button") || o.tagName === "DIV" && o.classList.contains("monaco-button-dropdown") ? !0 : o.classList.contains("monaco-list") || !o.parentElement ? !1 : NB(o.parentElement)
 }
-class R8 {
+class RB {
     get onKeyDown() {
         return this.disposables.add(De.chain(this.disposables.add(new dt(this.view.domNode, "keydown")).event).filter(e => !Vc(e.target)).map(e => new qt(e)))
     }
     constructor(e, t, i) {
         this.list = e, this.view = t, this.disposables = new ee, this.multipleSelectionDisposables = new ee, this.onKeyDown.filter(n => n.keyCode === 3).on(this.onEnter, this, this.disposables), this.onKeyDown.filter(n => n.keyCode === 16).on(this.onUpArrow, this, this.disposables), this.onKeyDown.filter(n => n.keyCode === 18).on(this.onDownArrow, this, this.disposables), this.onKeyDown.filter(n => n.keyCode === 11).on(this.onPageUpArrow, this, this.disposables), this.onKeyDown.filter(n => n.keyCode === 12).on(this.onPageDownArrow, this, this.disposables), this.onKeyDown.filter(n => n.keyCode === 9).on(this.onEscape, this, this.disposables), i.multipleSelectionSupport !== !1 && this.onKeyDown.filter(n => (ft ? n.metaKey : n.ctrlKey) && n.keyCode === 31).on(this.onCtrlA, this, this.multipleSelectionDisposables)
     }
     updateOptions(e) {
@@ -50276,15 +50276,15 @@
     onEscape(e) {
         this.list.getSelection().length && (e.preventDefault(), e.stopPropagation(), this.list.setSelection([], e.browserEvent), this.list.setAnchor(void 0), this.view.domNode.focus())
     }
     dispose() {
         this.disposables.dispose(), this.multipleSelectionDisposables.dispose()
     }
 }
-Tg([Vi], R8.prototype, "onKeyDown", null);
+Tg([Vi], RB.prototype, "onKeyDown", null);
 var tl;
 (function(o) {
     o[o.Automatic = 0] = "Automatic", o[o.Trigger = 1] = "Trigger"
 })(tl || (tl = {}));
 var Mf;
 (function(o) {
     o[o.Idle = 0] = "Idle", o[o.Typing = 1] = "Typing"
@@ -50360,30 +50360,30 @@
         s.visibility === "hidden" || s.display === "none" || (e.preventDefault(), e.stopPropagation(), n.focus())
     }
     dispose() {
         this.disposables.dispose()
     }
 }
 
-function M8(o) {
+function MB(o) {
     return ft ? o.browserEvent.metaKey : o.browserEvent.ctrlKey
 }
 
-function A8(o) {
+function AB(o) {
     return o.browserEvent.shiftKey
 }
 
 function qse(o) {
     return o instanceof MouseEvent && o.button === 2
 }
 const A4 = {
-    isSelectionSingleChangeEvent: M8,
-    isSelectionRangeChangeEvent: A8
+    isSelectionSingleChangeEvent: MB,
+    isSelectionRangeChangeEvent: AB
 };
-class P8 {
+class PB {
     constructor(e) {
         this.list = e, this.disposables = new ee, this._onPointer = new W, this.onPointer = this._onPointer.event, e.options.multipleSelectionSupport !== !1 && (this.multipleSelectionController = this.list.options.multipleSelectionController || A4), this.mouseSupport = typeof e.options.mouseSupport > "u" || !!e.options.mouseSupport, this.mouseSupport && (e.onMouseDown(this.onMouseDown, this, this.disposables), e.onContextMenu(this.onContextMenu, this, this.disposables), e.onMouseDblClick(this.onDoubleClick, this, this.disposables), e.onTouchStart(this.onMouseDown, this, this.disposables), this.disposables.add(jt.addTarget(e.getHTMLElement()))), De.any(e.onMouseClick, e.onMouseMiddleClick, e.onTap)(this.onViewPointer, this, this.disposables)
     }
     updateOptions(e) {
         e.multipleSelectionSupport !== void 0 && (this.multipleSelectionController = void 0, e.multipleSelectionSupport && (this.multipleSelectionController = this.list.options.multipleSelectionController || A4))
     }
     isSelectionSingleChangeEvent(e) {
@@ -50443,15 +50443,15 @@
             this.list.setFocus([t]), this.list.setAnchor(t), n.length === s.length ? this.list.setSelection([...s, t], e.browserEvent) : this.list.setSelection(s, e.browserEvent)
         }
     }
     dispose() {
         this.disposables.dispose()
     }
 }
-class O8 {
+class OB {
     constructor(e, t) {
         this.styleElement = e, this.selectorSuffix = t
     }
     style(e) {
         var t, i;
         const n = this.selectorSuffix && `.${this.selectorSuffix}`,
             s = [];
@@ -50732,27 +50732,27 @@
         this.accessibilityProvider = s.accessibilityProvider, this.accessibilityProvider && (h.push(new Jse(this.accessibilityProvider)), (l = (a = this.accessibilityProvider).onDidChangeActiveDescendant) === null || l === void 0 || l.call(a, this.onDidChangeActiveDescendant, this, this.disposables)), n = n.map(g => new Qse(g.templateId, [...h, g]));
         const u = Object.assign(Object.assign({}, s), {
             dnd: s.dnd && new eoe(this, s.dnd)
         });
         if (this.view = this.createListView(t, i, n, u), this.view.domNode.setAttribute("role", c), s.styleController) this.styleController = s.styleController(this.view.domId);
         else {
             const g = ur(this.view.domNode);
-            this.styleController = new O8(g, this.view.domId)
+            this.styleController = new OB(g, this.view.domId)
         }
-        if (this.spliceable = new Rse([new oD(this.focus, this.view, s.identityProvider), new oD(this.selection, this.view, s.identityProvider), new oD(this.anchor, this.view, s.identityProvider), this.view]), this.disposables.add(this.focus), this.disposables.add(this.selection), this.disposables.add(this.anchor), this.disposables.add(this.view), this.disposables.add(this._onDidDispose), this.disposables.add(new Kse(this, this.view)), (typeof s.keyboardSupport != "boolean" || s.keyboardSupport) && (this.keyboardController = new R8(this, this.view, s), this.disposables.add(this.keyboardController)), s.keyboardNavigationLabelProvider) {
+        if (this.spliceable = new Rse([new oD(this.focus, this.view, s.identityProvider), new oD(this.selection, this.view, s.identityProvider), new oD(this.anchor, this.view, s.identityProvider), this.view]), this.disposables.add(this.focus), this.disposables.add(this.selection), this.disposables.add(this.anchor), this.disposables.add(this.view), this.disposables.add(this._onDidDispose), this.disposables.add(new Kse(this, this.view)), (typeof s.keyboardSupport != "boolean" || s.keyboardSupport) && (this.keyboardController = new RB(this, this.view, s), this.disposables.add(this.keyboardController)), s.keyboardNavigationLabelProvider) {
             const g = s.keyboardNavigationDelegate || Use;
             this.typeNavigationController = new jse(this, this.view, s.keyboardNavigationLabelProvider, (d = s.keyboardNavigationEventFilter) !== null && d !== void 0 ? d : () => !0, g), this.disposables.add(this.typeNavigationController)
         }
         this.mouseController = this.createMouseController(s), this.disposables.add(this.mouseController), this.onDidChangeFocus(this._onFocusChange, this, this.disposables), this.onDidChangeSelection(this._onSelectionChange, this, this.disposables), this.accessibilityProvider && (this.ariaLabel = this.accessibilityProvider.getWidgetAriaLabel()), this._options.multipleSelectionSupport !== !1 && this.view.domNode.setAttribute("aria-multiselectable", "true")
     }
     createListView(e, t, i, n) {
         return new mr(e, t, i, n)
     }
     createMouseController(e) {
-        return new P8(this)
+        return new PB(this)
     }
     updateOptions(e = {}) {
         var t, i;
         this._options = Object.assign(Object.assign({}, this._options), e), (t = this.typeNavigationController) === null || t === void 0 || t.updateOptions(this._options), this._options.multipleSelectionController !== void 0 && (this._options.multipleSelectionSupport ? this.view.domNode.setAttribute("aria-multiselectable", "true") : this.view.domNode.removeAttribute("aria-multiselectable")), this.mouseController.updateOptions(e), (i = this.keyboardController) === null || i === void 0 || i.updateOptions(e), this.view.updateOptions(e)
     }
     get options() {
         return this._options
@@ -50966,18 +50966,18 @@
 }
 Tg([Vi], Kr.prototype, "onDidChangeFocus", null);
 Tg([Vi], Kr.prototype, "onDidChangeSelection", null);
 Tg([Vi], Kr.prototype, "onContextMenu", null);
 Tg([Vi], Kr.prototype, "onKeyDown", null);
 Tg([Vi], Kr.prototype, "onDidFocus", null);
 const Cu = ae,
-    F8 = "selectOption.entry.template";
+    FB = "selectOption.entry.template";
 class toe {
     get templateId() {
-        return F8
+        return FB
     }
     renderTemplate(e) {
         const t = Object.create(null);
         return t.root = e, t.text = Q(e, Cu(".option-text")), t.detail = Q(e, Cu(".option-detail")), t.decoratorRight = Q(e, Cu(".option-decorator-right")), t
     }
     renderElement(e, t, i) {
         const n = i,
@@ -50993,15 +50993,15 @@
     constructor(e, t, i, n, s) {
         super(), this.options = [], this._currentSelection = 0, this._hasDetails = !1, this._skipLayout = !1, this._sticky = !1, this._isVisible = !1, this.styles = n, this.selectBoxOptions = s || Object.create(null), typeof this.selectBoxOptions.minBottomMargin != "number" ? this.selectBoxOptions.minBottomMargin = il.DEFAULT_DROPDOWN_MINIMUM_BOTTOM_MARGIN : this.selectBoxOptions.minBottomMargin < 0 && (this.selectBoxOptions.minBottomMargin = 0), this.selectElement = document.createElement("select"), this.selectElement.className = "monaco-select-box monaco-select-box-dropdown-padding", typeof this.selectBoxOptions.ariaLabel == "string" && this.selectElement.setAttribute("aria-label", this.selectBoxOptions.ariaLabel), typeof this.selectBoxOptions.ariaDescription == "string" && this.selectElement.setAttribute("aria-description", this.selectBoxOptions.ariaDescription), this._onDidSelect = new W, this._register(this._onDidSelect), this.registerListeners(), this.constructSelectDropDown(i), this.selected = t || 0, e && this.setOptions(e, t), this.initStyleSheet()
     }
     getHeight() {
         return 22
     }
     getTemplateId() {
-        return F8
+        return FB
     }
     constructSelectDropDown(e) {
         this.contextViewProvider = e, this.selectDropDownContainer = ae(".monaco-select-box-dropdown-container"), this.selectDropDownContainer.classList.add("monaco-select-box-dropdown-padding"), this.selectionDetailsPane = Q(this.selectDropDownContainer, Cu(".select-box-details-pane"));
         const t = Q(this.selectDropDownContainer, Cu(".select-box-dropdown-container-width-control")),
             i = Q(t, Cu(".width-control-div"));
         this.widthControlElement = document.createElement("span"), this.widthControlElement.className = "option-text-width-control", Q(i, this.widthControlElement), this._dropDownPosition = 0, this.styleElement = ur(this.selectDropDownContainer), this.selectDropDownContainer.setAttribute("draggable", "true"), this._register(G(this.selectDropDownContainer, me.DRAG_START, n => {
             tt.stop(n, !0)
@@ -51442,15 +51442,15 @@
     getTooltip() {
         return this.action.tooltip
     }
     updateTooltip() {
         var e;
         if (!this.element) return;
         const t = (e = this.getTooltip()) !== null && e !== void 0 ? e : "";
-        this.updateAriaLabel(), this.options.hoverDelegate ? (this.element.title = "", this.customHover ? this.customHover.update(t) : (this.customHover = I8(this.options.hoverDelegate, this.element, t), this._store.add(this.customHover))) : this.element.title = t
+        this.updateAriaLabel(), this.options.hoverDelegate ? (this.element.title = "", this.customHover ? this.customHover.update(t) : (this.customHover = IB(this.options.hoverDelegate, this.element, t), this._store.add(this.customHover))) : this.element.title = t
     }
     updateAriaLabel() {
         var e;
         if (this.element) {
             const t = (e = this.getTooltip()) !== null && e !== void 0 ? e : "";
             this.element.setAttribute("aria-label", t)
         }
@@ -51873,36 +51873,36 @@
 const Ng = new aoe;
 xi.add(roe.IconContribution, Ng);
 
 function ri(o, e, t, i) {
     return Ng.registerIcon(o, e, t, i)
 }
 
-function B8() {
+function BB() {
     return Ng
 }
 
 function loe() {
     const o = B9();
     for (const e in o) {
         const t = "\\" + o[e].toString(16);
         Ng.registerIcon(e, {
             fontCharacter: t
         })
     }
 }
 loe();
-const W8 = "vscode://schemas/icons",
-    V8 = xi.as(ry.JSONContribution);
-V8.registerSchema(W8, Ng.getIconSchema());
-const B4 = new zt(() => V8.notifySchemaChanged(W8), 200);
+const WB = "vscode://schemas/icons",
+    VB = xi.as(ry.JSONContribution);
+VB.registerSchema(WB, Ng.getIconSchema());
+const B4 = new zt(() => VB.notifySchemaChanged(WB), 200);
 Ng.onDidChange(() => {
     B4.isScheduled() || B4.schedule()
 });
-const H8 = ri("widget-close", ue.close, p("widgetClose", "Icon for the close action in widgets."));
+const HB = ri("widget-close", ue.close, p("widgetClose", "Icon for the close action in widgets."));
 ri("goto-previous-location", ue.arrowUp, p("previousChangeIcon", "Icon for goto previous editor location."));
 ri("goto-next-location", ue.arrowDown, p("nextChangeIcon", "Icon for goto next editor location."));
 Ne.modify(ue.sync, "spin");
 Ne.modify(ue.loading, "spin");
 var doe = globalThis && globalThis.__decorate || function(o, e, t, i) {
         var n = arguments.length,
             s = n < 3 ? e : i === null ? i = Object.getOwnPropertyDescriptor(e, t) : i,
@@ -52486,15 +52486,15 @@
     }
 };
 qv.diffCache = new Map;
 qv = poe([W4(1, qr), W4(2, $o)], qv);
 const Na = ht("clipboardService"),
     $d = ht("contextViewService"),
     Uo = ht("contextMenuService"),
-    z8 = ht("progressService");
+    zB = ht("progressService");
 class Rg {
     constructor(e, t) {
         this.callback = e, this.report = t != null && t.async ? this._reportAsync.bind(this) : this._reportSync.bind(this)
     }
     _reportSync(e) {
         this._value = e, this.callback(this._value)
     }
@@ -52583,15 +52583,15 @@
         }), s == null || s.restore(e), e.changeDecorations(r => {
             this._decorations = r.deltaDecorations(this._decorations, i.decorations)
         }), t == null || t.setZones(i.overviewZones)
     }
 }
 let boe = 0;
 const Coe = ri("diff-insert", ue.add, p("diffInsertIcon", "Line decoration for inserts in the diff editor.")),
-    $8 = ri("diff-remove", ue.remove, p("diffRemoveIcon", "Line decoration for removals in the diff editor.")),
+    $B = ri("diff-remove", ue.remove, p("diffRemoveIcon", "Line decoration for removals in the diff editor.")),
     LE = Hd("diffEditorWidget", {
         createHTML: o => o
     }),
     H4 = p("diff-aria-navigation-tip", " use Shift + F7 to navigate changes");
 let ah = class An extends z {
     constructor(e, t, i, n, s, r, a, l, d, c, h) {
         super(), this._editorProgressService = h, this._onDidDispose = this._register(new W), this.onDidDispose = this._onDidDispose.event, this._onDidChangeModel = this._register(new W), this.onDidChangeModel = this._onDidChangeModel.event, this._onDidUpdateDiff = this._register(new W), this.onDidUpdateDiff = this._onDidUpdateDiff.event, this._onDidContentSizeChange = this._register(new W), this._lastOriginalWarning = null, this._lastModifiedWarning = null, a.willCreateDiffEditor(), this._documentDiffProvider = this._register(r.createInstance(qv, t)), this._register(this._documentDiffProvider.onDidChange(g => this._beginUpdateDecorationsSoon())), this._codeEditorService = a, this._contextKeyService = this._register(s.createScoped(e)), this._instantiationService = r.createChild(new s0([He, this._contextKeyService])), this._contextKeyService.createKey("isInDiffEditor", !0), this._themeService = l, this._notificationService = d, this._id = ++boe, this._state = 0, this._updatingDiffProgress = null, this._domElement = e, t = t || {}, this._options = U4(t, {
@@ -53089,21 +53089,21 @@
         (t = this._strategy) === null || t === void 0 || t.dispose(), this._strategy = e, this._boundarySashes && e.setBoundarySashes(this._boundarySashes), e.applyColors(this._themeService.getColorTheme()), this._diffComputationResult && this._updateDecorations(), this._doLayout()
     }
 };
 ah.ONE_OVERVIEW_WIDTH = 15;
 ah.ENTIRE_DIFF_OVERVIEW_WIDTH = 30;
 ah.UPDATE_DIFF_DECORATIONS_DELAY = 200;
 ah = _oe([Jd(3, Na), Jd(4, He), Jd(5, $e), Jd(6, St), Jd(7, nn), Jd(8, Oi), Jd(9, Uo), Jd(10, Ud)], ah);
-class U8 extends z {
+class UB extends z {
     constructor(e) {
         super(), this._dataSource = e, this._insertColor = null, this._removeColor = null
     }
     applyColors(e) {
-        const t = e.getColor(cB) || (e.getColor(lB) || uw).transparent(2),
-            i = e.getColor(hB) || (e.getColor(dB) || gw).transparent(2),
+        const t = e.getColor(c8) || (e.getColor(l8) || uw).transparent(2),
+            i = e.getColor(h8) || (e.getColor(d8) || gw).transparent(2),
             n = !t.equals(this._insertColor) || !i.equals(this._removeColor);
         return this._insertColor = t, this._removeColor = i, n
     }
     getEditorsDiffDecorations(e, t, i, n, s, r) {
         r = r.sort((c, h) => c.afterLineNumber - h.afterLineNumber), s = s.sort((c, h) => c.afterLineNumber - h.afterLineNumber);
         const a = this._getViewZones(e, s, r, i),
             l = this._getOriginalEditorDecorations(a, e, t, i),
@@ -53246,15 +53246,15 @@
         }
         return {
             original: wu._ensureDomNodes(d.original),
             modified: wu._ensureDomNodes(d.modified)
         }
     }
     static _ensureDomNodes(e) {
-        return e.map(t => (t.domNode || (t.domNode = q8()), t))
+        return e.map(t => (t.domNode || (t.domNode = qB()), t))
     }
 }
 
 function od(o, e, t, i, n) {
     return {
         range: new I(o, e, t, i),
         options: n
@@ -53306,24 +53306,24 @@
         className: "line-delete",
         marginClassName: "gutter-delete",
         isWholeLine: !0
     }),
     lineDeleteWithSign: ze.register({
         description: "diff-editor-line-delete-with-sign",
         className: "line-delete",
-        linesDecorationsClassName: "delete-sign " + Ne.asClassName($8),
+        linesDecorationsClassName: "delete-sign " + Ne.asClassName($B),
         marginClassName: "gutter-delete",
         isWholeLine: !0
     }),
     lineDeleteMargin: ze.register({
         description: "diff-editor-line-delete-margin",
         marginClassName: "gutter-delete"
     })
 };
-class ud extends U8 {
+class ud extends UB {
     constructor(e, t, i) {
         super(e), this._disableSash = t === !1, this._defaultRatio = i, this._sashRatio = null, this._sashPosition = null, this._startSashPosition = null, this._sash = this._register(new Vn(this._dataSource.getContainerDomNode(), this, {
             orientation: 0
         })), this._disableSash && (this._sash.state = 0), this._sash.onDidStart(() => this._onSashDragStart()), this._sash.onDidChange(n => this._onSashDrag(n)), this._sash.onDidEnd(() => this._onSashDragEnd()), this._sash.onDidReset(() => this._onSashReset())
     }
     setEnableSplitViewResizing(e, t) {
         this._defaultRatio = t;
@@ -53381,15 +53381,15 @@
                 a.decorations.push({
                     range: new I(c.originalStartLineNumber, 1, c.originalEndLineNumber, 1073741824),
                     options: n ? ws.lineDeleteWithSign : ws.lineDelete
                 }), (!Aw(c) || !c.charChanges) && a.decorations.push(od(c.originalStartLineNumber, 1, c.originalEndLineNumber, 1073741824, ws.charDeleteWholeLine));
                 const h = Gv(l, d, c.originalStartLineNumber, c.originalEndLineNumber);
                 if (a.overviewZones.push(new Tp(h.startLineNumber, h.endLineNumber, 0, r)), c.charChanges) {
                     for (const u of c.charChanges)
-                        if (K8(u))
+                        if (KB(u))
                             if (i)
                                 for (let g = u.originalStartLineNumber; g <= u.originalEndLineNumber; g++) {
                                     let f, m;
                                     g === u.originalStartLineNumber ? f = u.originalStartColumn : f = l.getLineFirstNonWhitespaceColumn(g), g === u.originalEndLineNumber ? m = u.originalEndColumn : m = l.getLineLastNonWhitespaceColumn(g), a.decorations.push(od(g, f, g, m, ws.charDelete))
                                 } else a.decorations.push(od(u.originalStartLineNumber, u.originalStartColumn, u.originalEndLineNumber, u.originalEndColumn, ws.charDelete))
                 }
             } return a
@@ -53416,15 +53416,15 @@
                 l.decorations.push({
                     range: new I(h.modifiedStartLineNumber, 1, h.modifiedEndLineNumber, 1073741824),
                     options: n ? ws.lineInsertWithSign : ws.lineInsert
                 }), (!Pw(h) || !h.charChanges) && l.decorations.push(od(h.modifiedStartLineNumber, 1, h.modifiedEndLineNumber, 1073741824, ws.charInsertWholeLine));
                 const u = Gv(d, c, h.modifiedStartLineNumber, h.modifiedEndLineNumber);
                 if (l.overviewZones.push(new Tp(u.startLineNumber, u.endLineNumber, 0, a)), h.charChanges) {
                     for (const g of h.charChanges)
-                        if (j8(g))
+                        if (jB(g))
                             if (i)
                                 for (let f = g.modifiedStartLineNumber; f <= g.modifiedEndLineNumber; f++) {
                                     let m, _;
                                     f === g.modifiedStartLineNumber ? m = g.modifiedStartColumn : m = d.getLineFirstNonWhitespaceColumn(f), f === g.modifiedEndLineNumber ? _ = g.modifiedEndColumn : _ = d.getLineLastNonWhitespaceColumn(f), l.decorations.push(od(f, m, f, _, ws.charInsert))
                                 } else l.decorations.push(od(g.modifiedStartLineNumber, g.modifiedStartColumn, g.modifiedEndLineNumber, g.modifiedEndColumn, ws.charInsert))
                 }
             }
@@ -53451,15 +53451,15 @@
         return t > i ? {
             afterLineNumber: Math.max(e.modifiedStartLineNumber, e.modifiedEndLineNumber),
             heightInLines: t - i,
             domNode: null
         } : null
     }
 }
-class $4 extends U8 {
+class $4 extends UB {
     constructor(e, t) {
         super(e), this._decorationsLeft = e.getOriginalEditor().getLayoutInfo().decorationsLeft, this._register(e.getOriginalEditor().onDidLayoutChange(i => {
             this._decorationsLeft !== i.decorationsLeft && (this._decorationsLeft = i.decorationsLeft, e.relayoutEditors())
         }))
     }
     setEnableSplitViewResizing(e) {}
     _getViewZones(e, t, i, n) {
@@ -53510,15 +53510,15 @@
                 l.decorations.push({
                     range: new I(h.modifiedStartLineNumber, 1, h.modifiedEndLineNumber, 1073741824),
                     options: n ? ws.lineInsertWithSign : ws.lineInsert
                 });
                 const u = Gv(d, c, h.modifiedStartLineNumber, h.modifiedEndLineNumber);
                 if (l.overviewZones.push(new Tp(u.startLineNumber, u.endLineNumber, 0, a)), h.charChanges) {
                     for (const g of h.charChanges)
-                        if (j8(g))
+                        if (jB(g))
                             if (i)
                                 for (let f = g.modifiedStartLineNumber; f <= g.modifiedEndLineNumber; f++) {
                                     let m, _;
                                     f === g.modifiedStartLineNumber ? m = g.modifiedStartColumn : m = d.getLineFirstNonWhitespaceColumn(f), f === g.modifiedEndLineNumber ? _ = g.modifiedEndColumn : _ = d.getLineLastNonWhitespaceColumn(f), l.decorations.push(od(f, m, f, _, ws.charInsert))
                                 } else l.decorations.push(od(g.modifiedStartLineNumber, g.modifiedStartColumn, g.modifiedEndLineNumber, g.modifiedEndColumn, ws.charInsert))
                 } else l.decorations.push(od(h.modifiedStartLineNumber, 1, h.modifiedEndLineNumber, 1073741824, ws.charInsertWholeLine))
             } return l
@@ -53594,15 +53594,15 @@
                 S = this._pendingViewZones[C],
                 k = S.domNode;
             ln(k, n);
             const y = S.marginDomNode;
             ln(y, n);
             const x = [];
             if (w.charChanges)
-                for (const ye of w.charChanges) K8(ye) && x.push(new Zf(new I(ye.originalStartLineNumber, ye.originalStartColumn, ye.originalEndLineNumber, ye.originalEndColumn), "char-delete", 0));
+                for (const ye of w.charChanges) KB(ye) && x.push(new Zf(new I(ye.originalStartLineNumber, ye.originalStartColumn, ye.originalEndLineNumber, ye.originalEndColumn), "char-delete", 0));
             const L = x.length > 0,
                 E = new yg(1e4);
             let T = 0,
                 M = 0,
                 B = null;
             for (let ye = w.originalStartLineNumber; ye <= w.originalEndLineNumber; ye++) {
                 const Re = ye - w.originalStartLineNumber,
@@ -53620,15 +53620,15 @@
                     for (B || (B = []); B.length < Re;) B[B.length] = 1;
                     B[Re] = Le.breakOffsets.length, S.heightInLines += Le.breakOffsets.length - 1;
                     const K = document.createElement("div");
                     K.className = "gutter-delete", e.original.push({
                         afterLineNumber: ye,
                         afterColumn: 0,
                         heightInLines: Le.breakOffsets.length - 1,
-                        domNode: q8(),
+                        domNode: qB(),
                         marginDomNode: K
                     })
                 } else T = Math.max(T, this._renderOriginalLine(M++, pe, ne, Se, L, l, d, n, s, c, u, g, f, m, _, i, E, y))
             }
             T += a;
             const q = E.build(),
                 X = LE ? LE.createHTML(q) : q;
@@ -53643,15 +53643,15 @@
     _renderOriginalLine(e, t, i, n, s, r, a, l, d, c, h, u, g, f, m, _, v, b) {
         v.appendString('<div class="view-line'), s || v.appendString(" char-delete"), v.appendString('" style="top:'), v.appendString(String(e * c)), v.appendString('px;width:1000000px;">');
         const C = vs.isBasicASCII(t, r),
             w = vs.containsRTL(t, C, a),
             S = dm(new Rl(l.isMonospace && !d, l.canUseHalfwidthRightwardsArrow, t, !1, C, w, 0, i, n, _, 0, l.spaceWidth, l.middotWidth, l.wsmiddotWidth, u, g, f, m !== Ks.OFF, null), v);
         if (v.appendString("</div>"), this._renderIndicators) {
             const k = document.createElement("div");
-            k.className = `delete-sign ${Ne.asClassName($8)}`, k.setAttribute("style", `position:absolute;top:${e*c}px;width:${h}px;height:${c}px;right:0;`), b.appendChild(k)
+            k.className = `delete-sign ${Ne.asClassName($B)}`, k.setAttribute("style", `position:absolute;top:${e*c}px;width:${h}px;height:${c}px;right:0;`), b.appendChild(k)
         }
         return S.characterMapping.getHorizontalOffset(S.characterMapping.length)
     }
 }
 
 function yoe(o, e) {
     return Si(o, e, ["off", "on", "inherit"])
@@ -53661,23 +53661,23 @@
     return o.modifiedEndLineNumber > 0
 }
 
 function Pw(o) {
     return o.originalEndLineNumber > 0
 }
 
-function j8(o) {
+function jB(o) {
     return o.modifiedStartLineNumber === o.modifiedEndLineNumber ? o.modifiedEndColumn - o.modifiedStartColumn > 0 : o.modifiedEndLineNumber - o.modifiedStartLineNumber > 0
 }
 
-function K8(o) {
+function KB(o) {
     return o.originalStartLineNumber === o.originalEndLineNumber ? o.originalEndColumn - o.originalStartColumn > 0 : o.originalEndLineNumber - o.originalStartLineNumber > 0
 }
 
-function q8() {
+function qB() {
     const o = document.createElement("div");
     return o.className = "diagonal-fill", o
 }
 
 function Loe() {
     const o = document.createElement("div");
     return o.className = "arrow-revert-change " + Ne.asClassName(ue.arrowRight), ae("div", {}, o)
@@ -53941,24 +53941,24 @@
         const i = e.getModel();
         return i && i.uri.toString() !== t.toString() ? null : i
     }
 };
 Ow = Eoe([j4(0, He), j4(1, nn)], Ow);
 vt(St, Ow, 0);
 const _m = ht("layoutService");
-var G8 = globalThis && globalThis.__decorate || function(o, e, t, i) {
+var GB = globalThis && globalThis.__decorate || function(o, e, t, i) {
         var n = arguments.length,
             s = n < 3 ? e : i === null ? i = Object.getOwnPropertyDescriptor(e, t) : i,
             r;
         if (typeof Reflect == "object" && typeof Reflect.decorate == "function") s = Reflect.decorate(o, e, t, i);
         else
             for (var a = o.length - 1; a >= 0; a--)(r = o[a]) && (s = (n < 3 ? r(s) : n > 3 ? r(e, t, s) : r(e, t)) || s);
         return n > 3 && s && Object.defineProperty(e, t, s), s
     },
-    Z8 = globalThis && globalThis.__param || function(o, e) {
+    ZB = globalThis && globalThis.__param || function(o, e) {
         return function(t, i) {
             e(t, i, o)
         }
     };
 let Fw = class {
     get dimension() {
         return this._dimension || (this._dimension = cm(window.document.body)), this._dimension
@@ -53976,27 +53976,27 @@
     constructor(e) {
         this._codeEditorService = e, this.onDidLayout = De.None, this.offset = {
             top: 0,
             quickPickTop: 0
         }
     }
 };
-Fw = G8([Z8(0, St)], Fw);
+Fw = GB([ZB(0, St)], Fw);
 let DE = class extends Fw {
     get hasContainer() {
         return !1
     }
     get container() {
         return this._container
     }
     constructor(e, t) {
         super(t), this._container = e
     }
 };
-DE = G8([Z8(1, St)], DE);
+DE = GB([ZB(1, St)], DE);
 vt(_m, Fw, 1);
 const a0 = ht("dialogService");
 var Noe = globalThis && globalThis.__decorate || function(o, e, t, i) {
         var n = arguments.length,
             s = n < 3 ? e : i === null ? i = Object.getOwnPropertyDescriptor(e, t) : i,
             r;
         if (typeof Reflect == "object" && typeof Reflect.decorate == "function") s = Reflect.decorate(o, e, t, i);
@@ -54038,18 +54038,18 @@
             d((i = i.apply(o, e || [])).next())
         })
     };
 
 function vC(o) {
     return o.scheme === it.file ? o.fsPath : o.path
 }
-let Y8 = 0;
+let YB = 0;
 class bC {
     constructor(e, t, i, n, s, r, a) {
-        this.id = ++Y8, this.type = 0, this.actual = e, this.label = e.label, this.confirmBeforeUndo = e.confirmBeforeUndo || !1, this.resourceLabel = t, this.strResource = i, this.resourceLabels = [this.resourceLabel], this.strResources = [this.strResource], this.groupId = n, this.groupOrder = s, this.sourceId = r, this.sourceOrder = a, this.isValid = !0
+        this.id = ++YB, this.type = 0, this.actual = e, this.label = e.label, this.confirmBeforeUndo = e.confirmBeforeUndo || !1, this.resourceLabel = t, this.strResource = i, this.resourceLabels = [this.resourceLabel], this.strResources = [this.strResource], this.groupId = n, this.groupOrder = s, this.sourceId = r, this.sourceOrder = a, this.isValid = !0
     }
     setValid(e) {
         this.isValid = e
     }
     toString() {
         return `[id:${this.id}] [group:${this.groupId}] [${this.isValid?"  VALID":"INVALID"}] ${this.actual.constructor.name} - ${this.actual}`
     }
@@ -54088,30 +54088,30 @@
     }
     delete(e) {
         return this.elements.delete(e)
     }
 }
 class Roe {
     constructor(e, t, i, n, s, r, a) {
-        this.id = ++Y8, this.type = 1, this.actual = e, this.label = e.label, this.confirmBeforeUndo = e.confirmBeforeUndo || !1, this.resourceLabels = t, this.strResources = i, this.groupId = n, this.groupOrder = s, this.sourceId = r, this.sourceOrder = a, this.removedResources = null, this.invalidatedResources = null
+        this.id = ++YB, this.type = 1, this.actual = e, this.label = e.label, this.confirmBeforeUndo = e.confirmBeforeUndo || !1, this.resourceLabels = t, this.strResources = i, this.groupId = n, this.groupOrder = s, this.sourceId = r, this.sourceOrder = a, this.removedResources = null, this.invalidatedResources = null
     }
     canSplit() {
         return typeof this.actual.split == "function"
     }
     removeResource(e, t, i) {
         this.removedResources || (this.removedResources = new G4), this.removedResources.has(t) || this.removedResources.set(t, new q4(e, i))
     }
     setValid(e, t, i) {
         i ? this.invalidatedResources && (this.invalidatedResources.delete(t), this.invalidatedResources.size === 0 && (this.invalidatedResources = null)) : (this.invalidatedResources || (this.invalidatedResources = new G4), this.invalidatedResources.has(t) || this.invalidatedResources.set(t, new q4(e, 0)))
     }
     toString() {
         return `[id:${this.id}] [group:${this.groupId}] [${this.invalidatedResources?"INVALID":"  VALID"}] ${this.actual.constructor.name} - ${this.actual}`
     }
 }
-class X8 {
+class XB {
     constructor(e, t) {
         this.resourceLabel = e, this.strResource = t, this._past = [], this._future = [], this.locked = !1, this.versionId = 1
     }
     dispose() {
         for (const e of this._past) e.type === 1 && e.removeResource(this.resourceLabel, this.strResource, 0);
         for (const e of this._future) e.type === 1 && e.removeResource(this.resourceLabel, this.strResource, 0);
         this.versionId++
@@ -54138,15 +54138,15 @@
         for (const t of this._future) t.type === 1 && t.removeResource(this.resourceLabel, this.strResource, 1);
         this._future = [], this._past.push(e), this.versionId++
     }
     createSnapshot(e) {
         const t = [];
         for (let i = 0, n = this._past.length; i < n; i++) t.push(this._past[i].id);
         for (let i = this._future.length - 1; i >= 0; i--) t.push(this._future[i].id);
-        return new c8(e, t)
+        return new cB(e, t)
     }
     restoreSnapshot(e) {
         const t = e.elements.length;
         let i = !0,
             n = 0,
             s = -1;
         for (let a = 0, l = this._past.length; a < l; a++, n++) {
@@ -54213,16 +54213,16 @@
     }
     isValid() {
         for (let e = 0, t = this.editStacks.length; e < t; e++)
             if (this._versionIds[e] !== this.editStacks[e].versionId) return !1;
         return !0
     }
 }
-const Q8 = new X8("", "");
-Q8.locked = !0;
+const QB = new XB("", "");
+QB.locked = !0;
 let kE = class {
     constructor(e, t) {
         this._dialogService = e, this._notificationService = t, this._editStacks = new Map, this._uriComparisonKeyComputers = []
     }
     getUriComparisonKey(e) {
         for (const t of this._uriComparisonKeyComputers)
             if (t[0] === e.scheme) return t[1].getComparisonKey(e);
@@ -54253,15 +54253,15 @@
         }
     }
     _pushElement(e) {
         for (let t = 0, i = e.strResources.length; t < i; t++) {
             const n = e.resourceLabels[t],
                 s = e.strResources[t];
             let r;
-            this._editStacks.has(s) ? r = this._editStacks.get(s) : (r = new X8(n, s), this._editStacks.set(s, r)), r.pushElement(e)
+            this._editStacks.has(s) ? r = this._editStacks.get(s) : (r = new XB(n, s), this._editStacks.set(s, r)), r.pushElement(e)
         }
     }
     getLastElement(e) {
         const t = this.getUriComparisonKey(e);
         if (this._editStacks.has(t)) {
             const i = this._editStacks.get(t);
             if (i.hasFutureElements()) return null;
@@ -54304,15 +54304,15 @@
     }
     setElementsValidFlag(e, t, i) {
         const n = this.getUriComparisonKey(e);
         this._editStacks.has(n) && this._editStacks.get(n).setElementsValidFlag(t, i)
     }
     createSnapshot(e) {
         const t = this.getUriComparisonKey(e);
-        return this._editStacks.has(t) ? this._editStacks.get(t).createSnapshot(e) : new c8(e, [])
+        return this._editStacks.has(t) ? this._editStacks.get(t).createSnapshot(e) : new cB(e, [])
     }
     restoreSnapshot(e) {
         const t = this.getUriComparisonKey(e.resource);
         if (this._editStacks.has(t)) {
             const i = this._editStacks.get(t);
             i.restoreSnapshot(e), !i.hasPastElements() && !i.hasFutureElements() && (i.dispose(), this._editStacks.delete(t))
         }
@@ -54375,15 +54375,15 @@
     _invokeResourcePrepare(e, t) {
         if (e.actual.type !== 1 || typeof e.actual.prepareUndoRedo > "u") return t(z.None);
         const i = e.actual.prepareUndoRedo();
         return i ? b2(i) ? t(i) : i.then(n => t(n)) : t(z.None)
     }
     _getAffectedEditStacks(e) {
         const t = [];
-        for (const i of e.strResources) t.push(this._editStacks.get(i) || Q8);
+        for (const i of e.strResources) t.push(this._editStacks.get(i) || QB);
         return new dD(t)
     }
     _tryToSplitAndUndo(e, t, i, n) {
         if (t.canSplit()) return this._splitPastWorkspaceElement(t, i), this._notificationService.warn(n), new CC(this._undo(e, 0, !0));
         for (const s of t.strResources) this.removeElements(s);
         return this._notificationService.warn(n), new CC
     }
@@ -54749,15 +54749,15 @@
         const i = this._key(e);
         let n = this._cache.get(i);
         n || (n = new Mse(6), this._cache.set(i, n));
         const s = so(n.update(t), this._min, this._max);
         return jR(e.uri, "output") || this._logService.trace(`[DEBOUNCE: ${this._name}] for ${e.uri.toString()} is ${s}ms`), s
     }
     _overall() {
-        const e = new T8;
+        const e = new TB;
         for (const [, t] of this._cache) e.update(t.value);
         return e.value
     }
     default () {
         const e = this._overall() | 0 || this._default;
         return so(e, this._min, this._max)
     }
@@ -54772,15 +54772,15 @@
             l = (s = i == null ? void 0 : i.max) !== null && s !== void 0 ? s : Math.pow(a, 2),
             d = (r = i == null ? void 0 : i.key) !== null && r !== void 0 ? r : void 0,
             c = `${Bw.of(e)},${a}${d?","+d:""}`;
         let h = this._data.get(c);
         return h || (this._isDev ? h = new Ooe(this._logService, t, e, this._overallAverage() | 0 || a * 1.5, a, l) : (this._logService.debug(`[DEBOUNCE: ${t}] is disabled in developed mode`), h = new Poe(a * 1.5)), this._data.set(c, h)), h
     }
     _overallAverage() {
-        const e = new T8;
+        const e = new TB;
         for (const t of this._data.values()) e.update(t.default());
         return e.value
     }
 };
 IE = Aoe([Y4(0, zo), Y4(1, UR)], IE);
 vt(_r, IE, 1);
 class Y_ {
@@ -55119,15 +55119,15 @@
     }
     warnInvalidEditStart(e, t, i, n, s) {
         this._hasWarnedInvalidEditStart || (this._hasWarnedInvalidEditStart = !0, console.warn(`Invalid semantic tokens edit detected (previousResultId: ${e}, resultId: ${t}) at edit #${i}: The provided start offset ${n} is outside the previous data (length ${s}).`))
     }
 };
 EE = Foe([cD(1, nn), cD(2, oi), cD(3, zo)], EE);
 
-function J8(o, e, t) {
+function JB(o, e, t) {
     const i = o.data,
         n = o.data.length / 5 | 0,
         s = Math.max(Math.ceil(n / 1024), 400),
         r = [];
     let a = 0,
         l = 1,
         d = 0;
@@ -58434,17 +58434,17 @@
         inputActiveOptionBorder: ve(tR),
         inputActiveOptionForeground: ve(nR),
         inputActiveOptionBackground: ve(iR)
     };
 ve(PX), ve(FX), ve(OX);
 ve(yi), ve(ll), ve(ol), ve(gt), ve(QX), ve(JX), ve(eQ), ve(RY);
 const Gw = {
-        inputBackground: ve(iB),
-        inputForeground: ve(nB),
-        inputBorder: ve(sB),
+        inputBackground: ve(i8),
+        inputForeground: ve(n8),
+        inputBorder: ve(s8),
         inputValidationInfoBorder: ve(PY),
         inputValidationInfoBackground: ve(MY),
         inputValidationInfoForeground: ve(AY),
         inputValidationWarningBorder: ve(BY),
         inputValidationWarningBackground: ve(OY),
         inputValidationWarningForeground: ve(FY),
         inputValidationErrorBorder: ve(HY),
@@ -58457,15 +58457,15 @@
         listFilterWidgetNoMatchesOutline: ve(TX),
         listFilterWidgetShadow: ve(NX),
         inputBoxStyles: Gw,
         toggleStyles: qw
     },
     c6 = {
         badgeBackground: ve(g1),
-        badgeForeground: ve(oB),
+        badgeForeground: ve(o8),
         badgeBorder: ve(gt)
     };
 ve(KX), ve(jX), ve(pO), ve(pO), ve(qX);
 const Mg = {
     listBackground: void 0,
     listInactiveFocusForeground: void 0,
     listFocusBackground: ve(vX),
@@ -58478,16 +58478,16 @@
     listFocusAndSelectionBackground: ve(wd),
     listFocusAndSelectionForeground: ve(cl),
     listInactiveSelectionBackground: ve(SX),
     listInactiveSelectionIconForeground: ve(LX),
     listInactiveSelectionForeground: ve(yX),
     listInactiveFocusBackground: ve(xX),
     listInactiveFocusOutline: ve(DX),
-    listHoverBackground: ve(uB),
-    listHoverForeground: ve(gB),
+    listHoverBackground: ve(u8),
+    listHoverForeground: ve(g8),
     listDropBackground: ve(kX),
     listSelectionOutline: ve(ni),
     listHoverOutline: ve(ni),
     treeIndentGuidesStroke: ve(m_),
     treeInactiveIndentGuidesStroke: ve(RX),
     tableColumnsBorder: ve(MX),
     tableOddRowsBackgroundColor: ve(AX)
@@ -58496,23 +58496,23 @@
 function vm(o) {
     return jre(o, Mg)
 }
 const Yre = {
         selectBackground: ve(rl),
         selectListBackground: ve(zY),
         selectForeground: ve(_d),
-        decoratorRightForeground: ve(rB),
+        decoratorRightForeground: ve(r8),
         selectBorder: ve(Lf),
         focusBorder: ve(Eo),
         listFocusBackground: ve(_u),
         listInactiveSelectionIconForeground: ve(xf),
         listFocusForeground: ve(mu),
         listFocusOutline: EY(ni, U.transparent.toString()),
-        listHoverBackground: ve(uB),
-        listHoverForeground: ve(gB),
+        listHoverBackground: ve(u8),
+        listHoverForeground: ve(g8),
         listHoverOutline: ve(ni),
         selectListBorder: ve(dl),
         listBackground: void 0,
         listActiveSelectionBackground: void 0,
         listActiveSelectionForeground: void 0,
         listActiveSelectionIconForeground: void 0,
         listFocusAndSelectionBackground: void 0,
@@ -61267,15 +61267,15 @@
 let Lae = class extends Ur {
     constructor(e, t, i) {
         var n;
         super(), this.state = "idle", this.maxHeight = Number.POSITIVE_INFINITY, this._onDidChange = this._register(new W), this.onDidChange = this._onDidChange.event, this._onDidHeightChange = this._register(new W), this.onDidHeightChange = this._onDidHeightChange.event, this.contextViewProvider = t, this.options = i, this.message = null, this.placeholder = this.options.placeholder || "", this.tooltip = (n = this.options.tooltip) !== null && n !== void 0 ? n : this.placeholder || "", this.ariaLabel = this.options.ariaLabel || "", this.options.validationOptions && (this.validation = this.options.validationOptions.validation), this.element = Q(e, Gm(".monaco-inputbox.idle"));
         const s = this.options.flexibleHeight ? "textarea" : "input",
             r = Q(this.element, Gm(".ibwrapper"));
         if (this.input = Q(r, Gm(s + ".input.empty")), this.input.setAttribute("autocorrect", "off"), this.input.setAttribute("autocapitalize", "off"), this.input.setAttribute("spellcheck", "false"), this.onfocus(this.input, () => this.element.classList.add("synthetic-focus")), this.onblur(this.input, () => this.element.classList.remove("synthetic-focus")), this.options.flexibleHeight) {
-            this.maxHeight = typeof this.options.flexibleMaxHeight == "number" ? this.options.flexibleMaxHeight : Number.POSITIVE_INFINITY, this.mirror = Q(r, Gm("div.mirror")), this.mirror.innerText = " ", this.scrollableElement = new SB(this.element, {
+            this.maxHeight = typeof this.options.flexibleMaxHeight == "number" ? this.options.flexibleMaxHeight : Number.POSITIVE_INFINITY, this.mirror = Q(r, Gm("div.mirror")), this.mirror.innerText = " ", this.scrollableElement = new S8(this.element, {
                 vertical: 1
             }), this.options.flexibleWidth && (this.input.setAttribute("wrap", "off"), this.mirror.style.whiteSpace = "pre", this.mirror.style.wordWrap = "initial"), Q(e, this.scrollableElement.getDomNode()), this._register(this.scrollableElement), this._register(this.scrollableElement.onScroll(d => this.input.scrollTop = d.scrollTop));
             const a = this._register(new dt(document, "selectionchange")),
                 l = De.filter(a.event, () => {
                     const d = document.getSelection();
                     return (d == null ? void 0 : d.anchorNode) === r
                 });
@@ -62500,20 +62500,20 @@
     }
     createNodeSet() {
         const e = new Set;
         for (const t of this.nodes) e.add(t);
         return e
     }
 }
-class Mae extends P8 {
+class Mae extends PB {
     constructor(e, t) {
         super(e), this.tree = t
     }
     onViewPointer(e) {
-        if (N8(e.browserEvent.target) || Vc(e.browserEvent.target) || Rf(e.browserEvent.target) || e.browserEvent.isHandledByList) return;
+        if (NB(e.browserEvent.target) || Vc(e.browserEvent.target) || Rf(e.browserEvent.target) || e.browserEvent.isHandledByList) return;
         const t = e.element;
         if (!t) return super.onViewPointer(e);
         if (this.isSelectionRangeChangeEvent(e) || this.isSelectionSingleChangeEvent(e)) return super.onViewPointer(e);
         const i = e.browserEvent.target,
             n = i.classList.contains("monaco-tl-twistie") || i.classList.contains("monaco-icon-label") && i.classList.contains("folder-icon") && e.browserEvent.offsetX < 16;
         let s = !1;
         if (typeof this.tree.expandOnlyOnTwistieClick == "function" ? s = this.tree.expandOnlyOnTwistieClick(t.element) : s = !!this.tree.expandOnlyOnTwistieClick, s && !n && e.browserEvent.detail !== 2) return super.onViewPointer(e);
@@ -64038,15 +64038,15 @@
         this.disposables = new ee, this.lists = [], this._lastFocusedWidget = void 0, this._hasCreatedStyleController = !1
     }
     setLastFocusedList(e) {
         var t, i;
         e !== this._lastFocusedWidget && ((t = this._lastFocusedWidget) === null || t === void 0 || t.getHTMLElement().classList.remove("last-focused"), this._lastFocusedWidget = e, (i = this._lastFocusedWidget) === null || i === void 0 || i.getHTMLElement().classList.add("last-focused"))
     }
     register(e, t) {
-        if (this._hasCreatedStyleController || (this._hasCreatedStyleController = !0, new O8(ur(), "").style(Mg)), this.lists.some(n => n.widget === e)) throw new Error("Cannot register the same widget multiple times");
+        if (this._hasCreatedStyleController || (this._hasCreatedStyleController = !0, new OB(ur(), "").style(Mg)), this.lists.some(n => n.widget === e)) throw new Error("Cannot register the same widget multiple times");
         const i = {
             widget: e,
             extraContextKeys: t
         };
         return this.lists.push(i), e.getHTMLElement() === document.activeElement && this.setLastFocusedList(e), Ar(e.onDidFocus(() => this.setLastFocusedList(e)), Ze(() => this.lists.splice(this.lists.indexOf(i), 1)), e.onDidDispose(() => {
             this.lists = this.lists.filter(n => n !== i), this._lastFocusedWidget === e && this.setLastFocusedList(void 0)
         }))
@@ -64112,18 +64112,18 @@
     }
     registerListeners() {
         this._register(this.configurationService.onDidChangeConfiguration(e => {
             e.affectsConfiguration(Ag) && (this.useAltAsMultipleSelectionModifier = Il(this.configurationService))
         }))
     }
     isSelectionSingleChangeEvent(e) {
-        return this.useAltAsMultipleSelectionModifier ? e.browserEvent.altKey : M8(e)
+        return this.useAltAsMultipleSelectionModifier ? e.browserEvent.altKey : MB(e)
     }
     isSelectionRangeChangeEvent(e) {
-        return A8(e)
+        return AB(e)
     }
 }
 
 function Ky(o, e) {
     var t;
     const i = o.get(_t),
         n = o.get(Yt),
@@ -65144,15 +65144,15 @@
         const i = this.customHovers.get(e);
         if (i && (i.dispose(), this.customHovers.delete(e)), !t) {
             e.removeAttribute("title");
             return
         }
         if (!this.hoverDelegate) sse(e, t);
         else {
-            const n = I8(this.hoverDelegate, e, t);
+            const n = IB(this.hoverDelegate, e, t);
             n && this.customHovers.set(e, n)
         }
     }
     dispose() {
         super.dispose();
         for (const e of this.customHovers.values()) e.dispose();
         this.customHovers.clear()
@@ -66863,15 +66863,15 @@
                 listInactiveSelectionIconForeground: xf,
                 listInactiveFocusBackground: _u,
                 listFocusOutline: ni,
                 listInactiveFocusOutline: ni
             }),
             pickerGroup: {
                 pickerGroupBorder: ve(tX),
-                pickerGroupForeground: ve(rB)
+                pickerGroupForeground: ve(r8)
             },
             colorScheme: this.themeService.getColorTheme().type
         }
     }
 };
 rT = Nle([kC(0, $e), kC(1, He), kC(2, nn), kC(3, _m)], rT);
 var V6 = globalThis && globalThis.__decorate || function(o, e, t, i) {
@@ -67298,15 +67298,15 @@
         }, {
             token: "predefined.sql",
             foreground: "C700C7"
         }],
         colors: {
             [an]: "#FFFFFE",
             [Er]: "#000000",
-            [aB]: "#E5EBF1",
+            [a8]: "#E5EBF1",
             [e0]: "#D3D3D3",
             [t0]: "#939393",
             [sR]: "#ADD6FF4D"
         }
     },
     zle = {
         base: "vs-dark",
@@ -67447,15 +67447,15 @@
         }, {
             token: "predefined.sql",
             foreground: "FF00FF"
         }],
         colors: {
             [an]: "#1E1E1E",
             [Er]: "#D4D4D4",
-            [aB]: "#3A3D41",
+            [a8]: "#3A3D41",
             [e0]: "#404040",
             [t0]: "#707070",
             [sR]: "#ADD6FF26"
         }
     },
     $le = {
         base: "hc-black",
@@ -67696,15 +67696,15 @@
             [e0]: "#292929",
             [t0]: "#292929"
         }
     };
 
 function jle(o) {
     const e = new W,
-        t = B8();
+        t = BB();
     return t.onDidChange(() => e.fire()), o == null || o.onDidProductIconThemeChange(() => e.fire()), {
         onDidChange: e.event,
         getCSS() {
             const i = o ? o.getProductIconTheme() : new z6,
                 n = {},
                 s = a => {
                     const l = i.getIcon(a);
@@ -67727,30 +67727,30 @@
             return r.join(`
 `)
         }
     }
 }
 class z6 {
     getIcon(e) {
-        const t = B8();
+        const t = BB();
         let i = e.defaults;
         for (; Ne.isThemeIcon(i);) {
             const n = t.getIcon(i.id);
             if (!n) return;
             i = n.defaults
         }
         return i
     }
 }
 const gd = "vs",
     dp = "vs-dark",
     Mu = "hc-black",
     Au = "hc-light",
-    $6 = xi.as(tB.ColorContribution),
-    Kle = xi.as(yB.ThemingContribution);
+    $6 = xi.as(t8.ColorContribution),
+    Kle = xi.as(y8.ThemingContribution);
 class U6 {
     constructor(e, t) {
         this.semanticHighlighting = !1, this.themeData = t;
         const i = t.base;
         e.length > 0 ? (k1(e) ? this.id = e : this.id = i + " " + e, this.themeName = e) : (this.id = i, this.themeName = i), this.colors = null, this.defaultColors = Object.create(null), this._tokenTheme = null
     }
     get base() {
@@ -69692,15 +69692,15 @@
 vt(Ol, lc, 0);
 vt(oi, Sde, 0);
 vt(_o, qle, 0);
 vt(zo, yde, 0);
 vt(di, Jw, 0);
 vt(Y2, GE, 0);
 vt(He, pT, 0);
-vt(z8, pde, 0);
+vt(zB, pde, 0);
 vt(Ud, Qy, 0);
 vt(Gr, Ure, 0);
 vt(qr, RI, 0);
 vt(l0, CT, 0);
 vt(l6, wde, 0);
 vt(eo, mT, 0);
 vt(Nl, cT, 0);
@@ -71421,16 +71421,16 @@
     };
 let vl = class Yl extends z {
     constructor(e, t, i, n, s, r, a, l) {
         super(), this._editors = e, this._rootElement = t, this._diffModel = i, this._rootWidth = n, this._rootHeight = s, this._modifiedEditorLayoutInfo = r, this._options = a, this._themeService = l;
         const d = Ts(this._themeService.onDidColorThemeChange, () => this._themeService.getColorTheme()),
             c = Lt("colors", g => {
                 const f = d.read(g),
-                    m = f.getColor(cB) || (f.getColor(lB) || uw).transparent(2),
-                    _ = f.getColor(hB) || (f.getColor(dB) || gw).transparent(2);
+                    m = f.getColor(c8) || (f.getColor(l8) || uw).transparent(2),
+                    _ = f.getColor(h8) || (f.getColor(d8) || gw).transparent(2);
                 return {
                     insertColor: m,
                     removeColor: _
                 }
             }),
             h = Ts(this._editors.modified.onDidScrollChange, () => this._editors.modified.getScrollTop()),
             u = Ts(this._editors.modified.onDidScrollChange, () => this._editors.modified.getScrollHeight());
@@ -72626,15 +72626,15 @@
                 group: a,
                 order: l
             };
             c.add(ts.appendMenuItem(R.EditorContext, g))
         }
         if (Array.isArray(s))
             for (const g of s) c.add(this._standaloneKeybindingService.addDynamicKeybinding(h, g, d, r));
-        const u = new UB(h, i, i, n, (...g) => Promise.resolve(e.run(this, ...g)), this._contextKeyService);
+        const u = new U8(h, i, i, n, (...g) => Promise.resolve(e.run(this, ...g)), this._contextKeyService);
         return this._actions.set(t, u), c.add(Ze(() => {
             this._actions.delete(t)
         })), c
     }
     _triggerCommand(e, t) {
         if (this._codeEditorService instanceof Ow) try {
             this._codeEditorService.setActiveCodeEditor(this), super._triggerCommand(e, t)
@@ -74368,45 +74368,45 @@
     aliases: ["F#", "FSharp", "fsharp"],
     loader: () => Ee(() => import("./fsharp-8abe6da0.js"), [], import.meta.url)
 });
 Ae({
     id: "freemarker2",
     extensions: [".ftl", ".ftlh", ".ftlx"],
     aliases: ["FreeMarker2", "Apache FreeMarker2"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagAutoInterpolationDollar)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagAutoInterpolationDollar)
 });
 Ae({
     id: "freemarker2.tag-angle.interpolation-dollar",
     aliases: ["FreeMarker2 (Angle/Dollar)", "Apache FreeMarker2 (Angle/Dollar)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagAngleInterpolationDollar)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagAngleInterpolationDollar)
 });
 Ae({
     id: "freemarker2.tag-bracket.interpolation-dollar",
     aliases: ["FreeMarker2 (Bracket/Dollar)", "Apache FreeMarker2 (Bracket/Dollar)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagBracketInterpolationDollar)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagBracketInterpolationDollar)
 });
 Ae({
     id: "freemarker2.tag-angle.interpolation-bracket",
     aliases: ["FreeMarker2 (Angle/Bracket)", "Apache FreeMarker2 (Angle/Bracket)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagAngleInterpolationBracket)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagAngleInterpolationBracket)
 });
 Ae({
     id: "freemarker2.tag-bracket.interpolation-bracket",
     aliases: ["FreeMarker2 (Bracket/Bracket)", "Apache FreeMarker2 (Bracket/Bracket)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagBracketInterpolationBracket)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagBracketInterpolationBracket)
 });
 Ae({
     id: "freemarker2.tag-auto.interpolation-dollar",
     aliases: ["FreeMarker2 (Auto/Dollar)", "Apache FreeMarker2 (Auto/Dollar)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagAutoInterpolationDollar)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagAutoInterpolationDollar)
 });
 Ae({
     id: "freemarker2.tag-auto.interpolation-bracket",
     aliases: ["FreeMarker2 (Auto/Bracket)", "Apache FreeMarker2 (Auto/Bracket)"],
-    loader: () => Ee(() => import("./freemarker2-c56b9d61.js"), ["./freemarker2-c56b9d61.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url).then(o => o.TagAutoInterpolationBracket)
+    loader: () => Ee(() => import("./freemarker2-ab7f8d00.js"), ["./freemarker2-ab7f8d00.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url).then(o => o.TagAutoInterpolationBracket)
 });
 Ae({
     id: "go",
     extensions: [".go"],
     aliases: ["Go"],
     loader: () => Ee(() => import("./go-8759e9f7.js"), [], import.meta.url)
 });
@@ -74418,28 +74418,28 @@
     loader: () => Ee(() => import("./graphql-387d549c.js"), [], import.meta.url)
 });
 Ae({
     id: "handlebars",
     extensions: [".handlebars", ".hbs"],
     aliases: ["Handlebars", "handlebars", "hbs"],
     mimetypes: ["text/x-handlebars-template"],
-    loader: () => Ee(() => import("./handlebars-1fc6855b.js"), ["./handlebars-1fc6855b.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./handlebars-b7cc84e9.js"), ["./handlebars-b7cc84e9.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "hcl",
     extensions: [".tf", ".tfvars", ".hcl"],
     aliases: ["Terraform", "tf", "HCL", "hcl"],
     loader: () => Ee(() => import("./hcl-a88f331a.js"), [], import.meta.url)
 });
 Ae({
     id: "html",
     extensions: [".html", ".htm", ".shtml", ".xhtml", ".mdoc", ".jsp", ".asp", ".aspx", ".jshtm"],
     aliases: ["HTML", "htm", "html", "xhtml"],
     mimetypes: ["text/html", "text/x-jshtm", "text/template", "text/ng-template"],
-    loader: () => Ee(() => import("./html-1e46783a.js"), ["./html-1e46783a.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./html-14f46deb.js"), ["./html-14f46deb.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "ini",
     extensions: [".ini", ".properties", ".gitconfig"],
     filenames: ["config", ".gitattributes", ".gitconfig", ".editorconfig"],
     aliases: ["Ini", "ini"],
     loader: () => Ee(() => import("./ini-18bf1153.js"), [], import.meta.url)
@@ -74454,15 +74454,15 @@
 Ae({
     id: "javascript",
     extensions: [".js", ".es6", ".jsx", ".mjs", ".cjs"],
     firstLine: "^#!.*\\bnode",
     filenames: ["jakefile"],
     aliases: ["JavaScript", "javascript", "js"],
     mimetypes: ["text/javascript"],
-    loader: () => Ee(() => import("./javascript-a891c4c5.js"), ["./javascript-a891c4c5.js", "./typescript-31544fa1.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./javascript-18f19bfc.js"), ["./javascript-18f19bfc.js", "./typescript-a67a867f.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "julia",
     extensions: [".jl"],
     aliases: ["julia", "Julia"],
     loader: () => Ee(() => import("./julia-0026391c.js"), [], import.meta.url)
 });
@@ -74493,15 +74493,15 @@
     loader: () => Ee(() => import("./lua-9adddcd9.js"), [], import.meta.url)
 });
 Ae({
     id: "liquid",
     extensions: [".liquid", ".html.liquid"],
     aliases: ["Liquid", "liquid"],
     mimetypes: ["application/liquid"],
-    loader: () => Ee(() => import("./liquid-79207f1f.js"), ["./liquid-79207f1f.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./liquid-d7e3f977.js"), ["./liquid-d7e3f977.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "m3",
     extensions: [".m3", ".i3", ".mg", ".ig"],
     aliases: ["Modula-3", "Modula3", "modula3", "m3"],
     loader: () => Ee(() => import("./m3-aa2dcf72.js"), [], import.meta.url)
 });
@@ -74511,15 +74511,15 @@
     aliases: ["Markdown", "markdown"],
     loader: () => Ee(() => import("./markdown-0f073a3a.js"), [], import.meta.url)
 });
 Ae({
     id: "mdx",
     extensions: [".mdx"],
     aliases: ["MDX", "mdx"],
-    loader: () => Ee(() => import("./mdx-d684260e.js"), ["./mdx-d684260e.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./mdx-2b91f7f9.js"), ["./mdx-2b91f7f9.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "mips",
     extensions: [".s"],
     aliases: ["MIPS", "MIPS-V"],
     mimetypes: ["text/x-mips", "text/mips", "text/plaintext"],
     loader: () => Ee(() => import("./mips-bdd96c5a.js"), [], import.meta.url)
@@ -74610,15 +74610,15 @@
     loader: () => Ee(() => import("./pug-cfe384ef.js"), [], import.meta.url)
 });
 Ae({
     id: "python",
     extensions: [".py", ".rpy", ".pyw", ".cpy", ".gyp", ".gypi"],
     aliases: ["Python", "py"],
     firstLine: "^#!/.*\\bpython[0-9.-]*\\b",
-    loader: () => Ee(() => import("./python-bbfdef2a.js"), ["./python-bbfdef2a.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./python-a79eb30c.js"), ["./python-a79eb30c.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "qsharp",
     extensions: [".qs"],
     aliases: ["Q#", "qsharp"],
     loader: () => Ee(() => import("./qsharp-e125d03f.js"), [], import.meta.url)
 });
@@ -74629,15 +74629,15 @@
     loader: () => Ee(() => import("./r-e0a01d4f.js"), [], import.meta.url)
 });
 Ae({
     id: "razor",
     extensions: [".cshtml"],
     aliases: ["Razor", "razor"],
     mimetypes: ["text/x-cshtml"],
-    loader: () => Ee(() => import("./razor-edf02117.js"), ["./razor-edf02117.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./razor-673842c1.js"), ["./razor-673842c1.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "redis",
     extensions: [".redis"],
     aliases: ["redis"],
     loader: () => Ee(() => import("./redis-d0a12fea.js"), [], import.meta.url)
 });
@@ -74761,15 +74761,15 @@
     loader: () => Ee(() => import("./twig-f894aab2.js"), [], import.meta.url)
 });
 Ae({
     id: "typescript",
     extensions: [".ts", ".tsx", ".cts", ".mts"],
     aliases: ["TypeScript", "ts", "typescript"],
     mimetypes: ["text/typescript"],
-    loader: () => Ee(() => import("./typescript-31544fa1.js"), ["./typescript-31544fa1.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./typescript-a67a867f.js"), ["./typescript-a67a867f.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "vb",
     extensions: [".vb"],
     aliases: ["Visual Basic", "vb"],
     loader: () => Ee(() => import("./vb-39a025f4.js"), [], import.meta.url)
 });
@@ -74781,22 +74781,22 @@
 });
 Ae({
     id: "xml",
     extensions: [".xml", ".xsd", ".dtd", ".ascx", ".csproj", ".config", ".props", ".targets", ".wxi", ".wxl", ".wxs", ".xaml", ".svg", ".svgz", ".opf", ".xslt", ".xsl"],
     firstLine: "(\\<\\?xml.*)|(\\<svg)|(\\<\\!doctype\\s+svg)",
     aliases: ["XML", "xml"],
     mimetypes: ["text/xml", "application/xml", "application/xaml+xml", "application/xml-dtd"],
-    loader: () => Ee(() => import("./xml-1904b31e.js"), ["./xml-1904b31e.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./xml-f0bf815b.js"), ["./xml-f0bf815b.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 Ae({
     id: "yaml",
     extensions: [".yaml", ".yml"],
     aliases: ["YAML", "yaml", "YML", "yml"],
     mimetypes: ["application/x-yaml", "text/x-yaml"],
-    loader: () => Ee(() => import("./yaml-ea97fa90.js"), ["./yaml-ea97fa90.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    loader: () => Ee(() => import("./yaml-d6c7a4c1.js"), ["./yaml-d6c7a4c1.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 });
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
@@ -74903,15 +74903,15 @@
 Cm.languages.css = {
     cssDefaults: vW,
     lessDefaults: CW,
     scssDefaults: bW
 };
 
 function AM() {
-    return Ee(() => import("./cssMode-dc15036c.js"), ["./cssMode-dc15036c.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    return Ee(() => import("./cssMode-40a421b7.js"), ["./cssMode-40a421b7.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 }
 Cm.languages.onLanguage("less", () => {
     AM().then(o => o.setupMode(CW))
 });
 Cm.languages.onLanguage("scss", () => {
     AM().then(o => o.setupMode(bW))
 });
@@ -75020,15 +75020,15 @@
     htmlLanguageService: wW,
     handlebarLanguageService: SW,
     razorLanguageService: yW,
     registerHTMLLanguageService: oL
 };
 
 function Mue() {
-    return Ee(() => import("./htmlMode-82eab562.js"), ["./htmlMode-82eab562.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    return Ee(() => import("./htmlMode-4adc2b6d.js"), ["./htmlMode-4adc2b6d.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 }
 
 function oL(o, e = nL, t = sL(o)) {
     const i = new Iue(o, e, t);
     let n;
     const s = iL.languages.onLanguage(o, async () => {
         n = (await Mue()).setupMode(i)
@@ -75112,15 +75112,15 @@
     },
     LW = new Wue("json", Vue, Hue);
 m0.languages.json = {
     jsonDefaults: LW
 };
 
 function zue() {
-    return Ee(() => import("./jsonMode-7dc8e9c5.js"), ["./jsonMode-7dc8e9c5.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    return Ee(() => import("./jsonMode-be63eb4c.js"), ["./jsonMode-be63eb4c.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 }
 m0.languages.register({
     id: "json",
     extensions: [".json", ".bowerrc", ".jshintrc", ".jscsrc", ".eslintrc", ".babelrc", ".har"],
     aliases: ["JSON", "json"],
     mimetypes: ["application/json"]
 });
@@ -75296,15 +75296,15 @@
     typescriptDefaults: RW,
     javascriptDefaults: MW,
     getTypeScriptWorker: Yue,
     getJavaScriptWorker: Xue
 };
 
 function rL() {
-    return Ee(() => import("./tsMode-d172b673.js"), ["./tsMode-d172b673.js", "./index-b222671e.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url)
+    return Ee(() => import("./tsMode-27474ecc.js"), ["./tsMode-27474ecc.js", "./index-0d669be8.js", "./index-b7043f95.css", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url)
 }
 $p.languages.onLanguage("typescript", () => rL().then(o => o.setupTypeScript(RW)));
 $p.languages.onLanguage("javascript", () => rL().then(o => o.setupJavaScript(MW)));
 var Que = globalThis && globalThis.__decorate || function(o, e, t, i) {
         var n = arguments.length,
             s = n < 3 ? e : i === null ? i = Object.getOwnPropertyDescriptor(e, t) : i,
             r;
@@ -83146,15 +83146,15 @@
     constructor(e, t, i, n, s) {
         this._openerService = n, this._labelService = s, this._lines = 0, this._longestLineLength = 0, this._relatedDiagnostics = new WeakMap, this._disposables = new ee, this._editor = t;
         const r = document.createElement("div");
         r.className = "descriptioncontainer", this._messageBlock = document.createElement("div"), this._messageBlock.classList.add("message"), this._messageBlock.setAttribute("aria-live", "assertive"), this._messageBlock.setAttribute("role", "alert"), r.appendChild(this._messageBlock), this._relatedBlock = document.createElement("div"), r.appendChild(this._relatedBlock), this._disposables.add(Ai(this._relatedBlock, "click", a => {
             a.preventDefault();
             const l = this._relatedDiagnostics.get(a.target);
             l && i(l)
-        })), this._scrollable = new SB(r, {
+        })), this._scrollable = new S8(r, {
             horizontal: 1,
             vertical: 1,
             useShadows: !1,
             horizontalScrollbarSize: 6,
             verticalScrollbarSize: 6
         }), e.appendChild(this._scrollable.getDomNode()), this._disposables.add(this._scrollable.onScroll(a => {
             r.style.left = `-${a.scrollLeft}px`, r.style.top = `-${a.scrollTop}px`
@@ -86410,15 +86410,15 @@
                 mode: null
             };
             this._editor.trigger("keyboard", "paste", d)
         })
     }
 };
 lg.ID = "editor.contrib.copyPasteActionController";
-lg = lme([of(1, $e), of(2, l0), of(3, Na), of(4, xe), of(5, Ra), of(6, z8)], lg);
+lg = lme([of(1, $e), of(2, l0), of(3, Na), of(4, xe), of(5, Ra), of(6, zB)], lg);
 
 function Y5(o, e) {
     var t;
     return !!(!((t = o.pasteMimeTypes) === null || t === void 0) && t.some(i => e.matches(i)))
 }
 var QM = globalThis && globalThis.__decorate || function(o, e, t, i) {
         var n = arguments.length,
@@ -88249,15 +88249,15 @@
                     }, !0)
                 }
             } else this._state.change({
                 searchScope: null
             }, !0)
         })), n.appendChild(this._toggleSelectionFind.domNode), this._closeBtn = this._register(new rf({
             label: Mme + this._keybindingLabelFor(Qt.CloseFindWidgetCommand),
-            icon: H8,
+            icon: HB,
             onTrigger: () => {
                 this._state.change({
                     isRevealed: !1,
                     searchScope: null
                 }, !1)
             },
             onKeyDown: l => {
@@ -88960,15 +88960,15 @@
                     isWholeLine: !0
                 }
             }, {
                 range: t,
                 options: {
                     description: "find-match-quick-access-range-highlight-overview",
                     overviewRuler: {
-                        color: wi(kB),
+                        color: wi(k8),
                         position: Fo.Full
                     }
                 }
             }])
         })
     }
 }
@@ -91877,17 +91877,17 @@
         getElements: () => a
     }, {
         getElements: () => l
     }).ComputeDiff(!1).changes
 }
 
 function dve(o, e) {
-    const t = new KB,
-        i = new GB(t, d => e.getLanguageConfiguration(d)),
-        n = new qB(new cve([o]), i),
+    const t = new K8,
+        i = new G8(t, d => e.getLanguageConfiguration(d)),
+        n = new q8(new cve([o]), i),
         s = QI(n, [], void 0, !0);
     let r = "";
     const a = o.getLineContent();
 
     function l(d, c) {
         if (d.kind === 2)
             if (l(d.openingBracket, c), c = li(c, d.openingBracket.length), d.child && (l(d.child, c), c = li(c, d.child.length)), d.closingBracket) l(d.closingBracket, c), c = li(c, d.closingBracket.length);
@@ -92754,15 +92754,15 @@
             r = n.text.toLowerCase(),
             a = Math.max(0, t.column - n.range.startColumn);
         let l = r.substring(0, a),
             d = r.substring(a),
             c = s.substring(0, a),
             h = s.substring(a);
         const u = e.getLineIndentColumn(n.range.startLineNumber);
-        return n.range.startColumn <= u && (c = c.trimStart(), c.length === 0 && (h = h.trimStart()), l = l.trimStart(), l.length === 0 && (d = d.trimStart())), l.startsWith(c) && !!b8(h, d)
+        return n.range.startColumn <= u && (c = c.trimStart(), c.length === 0 && (h = h.trimStart()), l = l.trimStart(), l.length === 0 && (d = d.trimStart())), l.startsWith(c) && !!bB(h, d)
     }
     canBeReused(e, t) {
         return this._isValid && this._getUpdatedRange(void 0).containsPosition(t) && this.isVisible(e, t, void 0) && !this._isSmallerThanOriginal(void 0)
     }
     _toFilterTextReplacement(e) {
         return new Qp(this._getUpdatedRange(e), this.inlineCompletion.filterText)
     }
@@ -97540,15 +97540,15 @@
                 if (m !== _) {
                     const v = rv(m, s, a);
                     l.push({
                         range: new I(c, 1, c, f.length + 1),
                         text: v
                     }), h = v + h.substr(f.length)
                 } else {
-                    const v = PB(i, c, this._languageConfigurationService);
+                    const v = P8(i, c, this._languageConfigurationService);
                     if (v === 0 || v === 8) return
                 }
             }
         }
         const u = c;
         for (; c < e.endLineNumber;) {
             if (!/\S/.test(i.getLineContent(c + 1))) {
@@ -98707,15 +98707,15 @@
         if (s) {
             let r = s.indentation;
             s.indentAction === $i.None || s.indentAction === $i.Indent ? r = s.indentation + s.appendText : s.indentAction === $i.IndentOutdent ? r = s.indentation : s.indentAction === $i.Outdent && (r = t.unshiftIndent(s.indentation) + s.appendText);
             const a = e.getLineContent(n);
             if (this.trimLeft(a).indexOf(this.trimLeft(r)) >= 0) {
                 const l = $t(e.getLineContent(n));
                 let d = $t(r);
-                const c = PB(e, n, this._languageConfigurationService);
+                const c = P8(e, n, this._languageConfigurationService);
                 c !== null && c & 2 && (d = t.unshiftIndent(d));
                 const h = no(d, i),
                     u = no(l, i);
                 return h - u
             }
         }
         return null
@@ -101576,16 +101576,16 @@
         return this._domNode || (this._domNode = document.createElement("div"), this._domNode.className = "monaco-editor rename-box", this._input = document.createElement("input"), this._input.className = "rename-input", this._input.type = "text", this._input.setAttribute("aria-label", p("renameAriaLabel", "Rename input. Type new name and press Enter to commit.")), this._domNode.appendChild(this._input), this._label = document.createElement("div"), this._label.className = "rename-label", this._domNode.appendChild(this._label), this._updateFont(), this._updateStyles(this._themeService.getColorTheme())), this._domNode
     }
     _updateStyles(e) {
         var t, i, n, s;
         if (!this._input || !this._domNode) return;
         const r = e.getColor(ol),
             a = e.getColor(eR);
-        this._domNode.style.backgroundColor = String((t = e.getColor(yi)) !== null && t !== void 0 ? t : ""), this._domNode.style.boxShadow = r ? ` 0 0 8px 2px ${r}` : "", this._domNode.style.border = a ? `1px solid ${a}` : "", this._domNode.style.color = String((i = e.getColor(nB)) !== null && i !== void 0 ? i : ""), this._input.style.backgroundColor = String((n = e.getColor(iB)) !== null && n !== void 0 ? n : "");
-        const l = e.getColor(sB);
+        this._domNode.style.backgroundColor = String((t = e.getColor(yi)) !== null && t !== void 0 ? t : ""), this._domNode.style.boxShadow = r ? ` 0 0 8px 2px ${r}` : "", this._domNode.style.border = a ? `1px solid ${a}` : "", this._domNode.style.color = String((i = e.getColor(n8)) !== null && i !== void 0 ? i : ""), this._input.style.backgroundColor = String((n = e.getColor(i8)) !== null && n !== void 0 ? n : "");
+        const l = e.getColor(s8);
         this._input.style.borderWidth = l ? "1px" : "0px", this._input.style.borderStyle = l ? "solid" : "none", this._input.style.borderColor = (s = l == null ? void 0 : l.toString()) !== null && s !== void 0 ? s : "none"
     }
     _updateFont() {
         if (!this._input || !this._label) return;
         const e = this._editor.getOption(49);
         this._input.style.fontFamily = e.fontFamily, this._input.style.fontWeight = e.fontWeight, this._input.style.fontSize = `${e.fontSize}px`, this._label.style.fontSize = `${e.fontSize*.8}px`
     }
@@ -102299,15 +102299,15 @@
                     resultId: t.resultId,
                     data: d
                 }
             }
         }
         if ($L(t)) {
             this._currentDocumentResponse = new uCe(e, t.resultId, t.data);
-            const a = J8(t, i, this._model.getLanguageId());
+            const a = JB(t, i, this._model.getLanguageId());
             if (n.length > 0)
                 for (const l of n)
                     for (const d of a)
                         for (const c of l.changes) d.applyEdit(c.range, c.text);
             this._model.tokenization.setSemanticTokens(a, !0)
         } else this._model.tokenization.setSemanticTokens(null, !0);
         r()
@@ -102394,15 +102394,15 @@
             s = new os(!1);
         return n.then(r => {
             if (this._debounceInformation.update(e, s.elapsed()), !r || !r.tokens || e.isDisposed() || e.getVersionId() !== i) return;
             const {
                 provider: a,
                 tokens: l
             } = r, d = this._semanticTokensStylingService.getStyling(a);
-            e.tokenization.setPartialSemanticTokens(t, J8(l, d, e.getLanguageId()))
+            e.tokenization.setPartialSemanticTokens(t, JB(l, d, e.getLanguageId()))
         }).then(() => this._removeOutstandingRequest(n), () => this._removeOutstandingRequest(n)), n
     }
 };
 Rb.ID = "editor.contrib.viewportSemanticTokens";
 Rb = gCe([s_(1, Py), s_(2, nn), s_(3, _t), s_(4, _r), s_(5, xe)], Rb);
 yt(Rb.ID, Rb, 1);
 class fCe {
@@ -103880,15 +103880,15 @@
         i.setAttribute("aria-hidden", "true"), e.icon && i.appendChild(ae(`div${Ne.asCSSSelector(e.icon)}`));
         const n = Q(this.element, ae("div.message-container"));
         if (n.setAttribute("aria-hidden", "true"), n.appendChild(this.getBannerMessage(e.message)), this.messageActionsContainer = Q(this.element, ae("div.message-actions-container")), e.actions)
             for (const r of e.actions) this._register(this.instantiationService.createInstance(QN, this.messageActionsContainer, Object.assign(Object.assign({}, r), {
                 tabIndex: -1
             }), {}));
         const s = Q(this.element, ae("div.action-container"));
-        this.actionBar = this._register(new Bo(s)), this.actionBar.push(this._register(new ss("banner.close", "Close Banner", Ne.asClassName(H8), !0, () => {
+        this.actionBar = this._register(new Bo(s)), this.actionBar.push(this._register(new ss("banner.close", "Close Banner", Ne.asClassName(HB), !0, () => {
             typeof e.onClose == "function" && e.onClose()
         })), {
             icon: !0,
             label: !1
         }), this.actionBar.setFocusable(!1)
     }
 };
@@ -105704,15 +105704,15 @@
                         isWholeLine: !0
                     }
                 }, {
                     range: t,
                     options: {
                         description: "quick-access-range-highlight-overview",
                         overviewRuler: {
-                            color: wi(kB),
+                            color: wi(k8),
                             position: Fo.Full
                         }
                     }
                 }],
                 [r, a] = i.deltaDecorations(n, s);
             this.rangeHighlightDecorationId = {
                 rangeHighlightId: r,
@@ -106585,15 +106585,15 @@
                     Ea(a) || this.dialogService.error(p("canNotRun", "Command '{0}' resulted in an error", e.label), Oz(a))
                 }
             })
         })
     }
 };
 Ob.PREFIX = ">";
-Ob.WORD_FILTER = AR(Ty, Bne, v8);
+Ob.WORD_FILTER = AR(Ty, Bne, vB);
 Ob = Fz([cu(1, $e), cu(2, Yt), cu(3, Di), cu(4, $o), cu(5, a0)], Ob);
 let vg = class cn extends z {
     constructor(e, t) {
         super(), this.storageService = e, this.configurationService = t, this.configuredCommandsHistoryLength = 0, this.updateConfiguration(), this.load(), this.registerListeners()
     }
     registerListeners() {
         this._register(this.configurationService.onDidChangeConfiguration(e => this.updateConfiguration(e)))
@@ -107269,31 +107269,32 @@
                 "field-key": _e(r)
             }, null, 8, ["component-id", "field-key"])) : Te("", !0)], 512))
         }
     });
 const $we = Li(zwe, [
         ["__scopeId", "data-v-4e8d9316"]
     ]),
-    Uwe = {
+    Uwe = ["data-key"],
+    jwe = {
         class: "chipStackContainer"
     },
-    jwe = {
+    Kwe = {
         class: "chipStack"
     },
-    Kwe = {
+    qwe = {
         key: 0,
         class: "main"
     },
-    qwe = {
+    Gwe = {
         key: 0,
         class: "pickerContainer"
     },
-    Gwe = ["value"],
     Zwe = ["value"],
-    Ywe = Pi({
+    Ywe = ["value"],
+    Xwe = Pi({
         __name: "BuilderFieldsColor",
         props: {
             componentId: {},
             fieldKey: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -107331,16 +107332,17 @@
                 n.value.addEventListener("focus", f)
             }), Bb(() => {
                 n.value.removeEventListener("focus", f)
             }), (v, b) => (J(), he("div", {
                 ref_key: "rootEl",
                 ref: n,
                 class: "BuilderFieldsColor",
-                tabindex: "-1"
-            }, [F("div", Uwe, [F("div", jwe, [F("button", {
+                tabindex: "-1",
+                "data-key": _e(c)
+            }, [F("div", jwe, [F("div", Kwe, [F("button", {
                 class: xt(["chip", {
                     active: g.value == "default"
                 }]),
                 tabindex: "0",
                 onClick: b[0] || (b[0] = () => {
                     m("default"), _e(i)(h.value.id, _e(c), void 0)
                 })
@@ -107352,99 +107354,99 @@
                 onClick: b[1] || (b[1] = C => m("css"))
             }, " CSS ", 2), F("button", {
                 class: xt(["chip", {
                     active: g.value == "pick"
                 }]),
                 tabindex: "0",
                 onClick: b[2] || (b[2] = C => m("pick"))
-            }, " Pick ", 2)])]), g.value == "pick" || g.value == "css" ? (J(), he("div", Kwe, [g.value == "pick" ? (J(), he("div", qwe, [F("input", {
+            }, " Pick ", 2)])]), g.value == "pick" || g.value == "css" ? (J(), he("div", qwe, [g.value == "pick" ? (J(), he("div", Gwe, [F("input", {
                 ref_key: "pickerEl",
                 ref: s,
                 type: "color",
                 value: h.value.content[_e(c)],
                 onInput: _
-            }, null, 40, Gwe)])) : Te("", !0), g.value == "css" ? (J(), he("input", {
+            }, null, 40, Zwe)])) : Te("", !0), g.value == "css" ? (J(), he("input", {
                 key: 1,
                 ref_key: "freehandInputEl",
                 ref: r,
                 type: "text",
                 value: h.value.content[_e(c)],
                 onInput: _
-            }, null, 40, Zwe)) : Te("", !0)])) : Te("", !0)], 512))
+            }, null, 40, Ywe)) : Te("", !0)])) : Te("", !0)], 8, Uwe))
         }
     });
-const Xwe = Li(Ywe, [
-        ["__scopeId", "data-v-0ef3b82c"]
+const Qwe = Li(Xwe, [
+        ["__scopeId", "data-v-7672140e"]
     ]),
     E0 = o => (Nn("data-v-c164aacf"), o = o(), Rn(), o),
-    Qwe = {
+    Jwe = {
         class: "chipStackContainer"
     },
-    Jwe = {
+    eSe = {
         class: "chipStack"
     },
-    eSe = {
+    tSe = {
         key: 0,
         class: "main"
     },
-    tSe = {
+    iSe = {
         key: 0,
         class: "pickerContainer"
     },
-    iSe = {
+    nSe = {
         class: "param"
     },
-    nSe = {
+    sSe = {
         class: "header"
     },
-    sSe = E0(() => F("div", {
+    oSe = E0(() => F("div", {
         class: "name"
     }, "Offset X", -1)),
-    oSe = ["value"],
-    rSe = {
+    rSe = ["value"],
+    aSe = {
         class: "param"
     },
-    aSe = {
+    lSe = {
         class: "header"
     },
-    lSe = E0(() => F("div", {
+    dSe = E0(() => F("div", {
         class: "name"
     }, "Offset Y", -1)),
-    dSe = ["value"],
-    cSe = {
+    cSe = ["value"],
+    hSe = {
         class: "param"
     },
-    hSe = {
+    uSe = {
         class: "header"
     },
-    uSe = E0(() => F("div", {
+    gSe = E0(() => F("div", {
         class: "name"
     }, "Blur radius", -1)),
-    gSe = ["value"],
-    fSe = {
+    fSe = ["value"],
+    pSe = {
         class: "param"
     },
-    pSe = {
+    mSe = {
         class: "header"
     },
-    mSe = E0(() => F("div", {
+    _Se = E0(() => F("div", {
         class: "name"
     }, "Spread radius", -1)),
-    _Se = ["value"],
-    vSe = {
+    vSe = ["value"],
+    bSe = {
         class: "param"
     },
-    bSe = E0(() => F("div", {
+    CSe = E0(() => F("div", {
         class: "header"
     }, [F("div", {
         class: "name"
     }, "Color")], -1)),
-    CSe = ["value"],
     wSe = ["value"],
-    SSe = Pi({
+    SSe = ["value"],
+    ySe = Pi({
         __name: "BuilderFieldsShadow",
         props: {
             componentId: {},
             fieldKey: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -107504,15 +107506,15 @@
             }), (x, L) => {
                 var E, T, M, B, q, X, ye, Re, ne, pe, Le, Se, $;
                 return J(), he("div", {
                     ref_key: "rootEl",
                     ref: n,
                     class: "BuilderFieldsShadow",
                     tabindex: "-1"
-                }, [F("div", Qwe, [F("div", Jwe, [F("button", {
+                }, [F("div", Jwe, [F("div", eSe, [F("button", {
                     class: xt(["chip", {
                         active: b.value == "default"
                     }]),
                     tabindex: "0",
                     onClick: L[0] || (L[0] = () => {
                         w("default"), _e(i)(m.value.id, _e(f), void 0)
                     })
@@ -107524,88 +107526,88 @@
                     onClick: L[1] || (L[1] = K => w("css"))
                 }, " CSS ", 2), F("button", {
                     class: xt(["chip", {
                         active: b.value == "pick"
                     }]),
                     tabindex: "0",
                     onClick: L[2] || (L[2] = K => w("pick"))
-                }, " Pick ", 2)])]), b.value == "pick" || b.value == "css" ? (J(), he("div", eSe, [b.value == "pick" ? (J(), he("div", tSe, [F("div", iSe, [F("div", nSe, [sSe, Un(F("div", {
+                }, " Pick ", 2)])]), b.value == "pick" || b.value == "css" ? (J(), he("div", tSe, [b.value == "pick" ? (J(), he("div", iSe, [F("div", nSe, [F("div", sSe, [oSe, Un(F("div", {
                     class: "value"
                 }, kt((E = y.value) == null ? void 0 : E.offsetX) + "px ", 513), [
                     [ga, (T = y.value) == null ? void 0 : T.offsetX]
                 ])]), F("input", {
                     ref_key: "paramOffsetXEl",
                     ref: r,
                     type: "range",
                     min: "0",
                     max: "32",
                     value: (M = y.value) == null ? void 0 : M.offsetX,
                     onInput: S
-                }, null, 40, oSe)]), F("div", rSe, [F("div", aSe, [lSe, Un(F("div", {
+                }, null, 40, rSe)]), F("div", aSe, [F("div", lSe, [dSe, Un(F("div", {
                     class: "value"
                 }, kt((B = y.value) == null ? void 0 : B.offsetY) + "px ", 513), [
                     [ga, (q = y.value) == null ? void 0 : q.offsetY]
                 ])]), F("input", {
                     ref_key: "paramOffsetYEl",
                     ref: a,
                     type: "range",
                     min: "0",
                     max: "32",
                     value: (X = y.value) == null ? void 0 : X.offsetY,
                     onInput: S
-                }, null, 40, dSe)]), F("div", cSe, [F("div", hSe, [uSe, Un(F("div", {
+                }, null, 40, cSe)]), F("div", hSe, [F("div", uSe, [gSe, Un(F("div", {
                     class: "value"
                 }, kt((ye = y.value) == null ? void 0 : ye.blurRadius) + "px ", 513), [
                     [ga, (Re = y.value) == null ? void 0 : Re.blurRadius]
                 ])]), F("input", {
                     ref_key: "paramBlurRadiusEl",
                     ref: l,
                     type: "range",
                     min: "0",
                     max: "32",
                     value: (ne = y.value) == null ? void 0 : ne.blurRadius,
                     onInput: S
-                }, null, 40, gSe)]), F("div", fSe, [F("div", pSe, [mSe, Un(F("div", {
+                }, null, 40, fSe)]), F("div", pSe, [F("div", mSe, [_Se, Un(F("div", {
                     class: "value"
                 }, kt((pe = y.value) == null ? void 0 : pe.spreadRadius) + "px ", 513), [
                     [ga, (Le = y.value) == null ? void 0 : Le.spreadRadius]
                 ])]), F("input", {
                     ref_key: "paramSpreadRadiusEl",
                     ref: d,
                     type: "range",
                     min: "-16",
                     max: "32",
                     value: (Se = y.value) == null ? void 0 : Se.spreadRadius,
                     onInput: S
-                }, null, 40, _Se)]), F("div", vSe, [bSe, F("input", {
+                }, null, 40, vSe)]), F("div", bSe, [CSe, F("input", {
                     ref_key: "paramColorEl",
                     ref: c,
                     type: "color",
                     value: ($ = y.value) == null ? void 0 : $.color,
                     onInput: S
-                }, null, 40, CSe)])])) : Te("", !0), b.value == "css" ? (J(), he("input", {
+                }, null, 40, wSe)])])) : Te("", !0), b.value == "css" ? (J(), he("input", {
                     key: 1,
                     ref_key: "freehandInputEl",
                     ref: s,
                     type: "text",
                     value: m.value.content[_e(f)],
                     onInput: k
-                }, null, 40, wSe)) : Te("", !0)])) : Te("", !0)], 512)
+                }, null, 40, SSe)) : Te("", !0)])) : Te("", !0)], 512)
             }
         }
     });
-const ySe = Li(SSe, [
+const LSe = Li(ySe, [
         ["__scopeId", "data-v-c164aacf"]
     ]),
-    LSe = ["data-key"],
-    xSe = ["value", "placeholder", "list"],
-    DSe = ["id"],
-    kSe = ["value"],
-    ISe = ["value", "placeholder"],
-    ESe = Pi({
+    xSe = ["data-key"],
+    DSe = ["value", "placeholder", "list"],
+    kSe = ["id"],
+    ISe = ["value"],
+    ESe = ["value", "placeholder"],
+    TSe = Pi({
         __name: "BuilderFieldsText",
         props: {
             componentId: {},
             fieldKey: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -107646,65 +107648,65 @@
                     class: "content",
                     autocorrect: "off",
                     autocomplete: "off",
                     spellcheck: "false",
                     placeholder: (f = l.value) == null ? void 0 : f.default,
                     list: l.value.options ? `list-${_e(s)}-${_e(r)}` : void 0,
                     onInput: c
-                }, null, 40, xSe), l.value.options ? (J(), he("datalist", {
+                }, null, 40, DSe), l.value.options ? (J(), he("datalist", {
                     key: 0,
                     id: `list-${_e(s)}-${_e(r)}`
                 }, [(J(!0), he(hi, null, Hn(d.value, (_, v) => (J(), he("option", {
                     key: v,
                     value: v
                 }, [_.toLowerCase() !== v.toLowerCase() ? (J(), he(hi, {
                     key: 0
-                }, [Gi(kt(_), 1)], 64)) : Te("", !0)], 8, kSe))), 128))], 8, DSe)) : Te("", !0)], 64)) : l.value.control == _e(WA).Textarea ? Un((J(), he("textarea", {
+                }, [Gi(kt(_), 1)], 64)) : Te("", !0)], 8, ISe))), 128))], 8, kSe)) : Te("", !0)], 64)) : l.value.control == _e(WA).Textarea ? Un((J(), he("textarea", {
                     key: 1,
                     class: "content",
                     value: a.value.content[_e(r)],
                     placeholder: (m = l.value) == null ? void 0 : m.default,
                     autocorrect: "off",
                     autocomplete: "off",
                     spellcheck: "false",
                     onInput: c
                 }, [Gi(`
-			`)], 40, ISe)), [
+			`)], 40, ESe)), [
                     [g]
-                ]) : Te("", !0)], 8, LSe)
+                ]) : Te("", !0)], 8, xSe)
             }
         }
     });
-const pk = Li(ESe, [
+const pk = Li(TSe, [
         ["__scopeId", "data-v-460413c0"]
     ]),
-    TSe = o => (Nn("data-v-510f1335"), o = o(), Rn(), o),
-    NSe = {
+    NSe = o => (Nn("data-v-510f1335"), o = o(), Rn(), o),
+    RSe = {
         class: "selectTrigger"
     },
-    RSe = {
+    MSe = {
         class: "selectContent"
     },
-    MSe = {
+    ASe = {
         key: 0,
         class: "flexRow"
     },
-    ASe = TSe(() => F("div", {
+    PSe = NSe(() => F("div", {
         class: "selectArrow"
     }, [F("i", {
         class: "ri-arrow-down-s-fill"
     })], -1)),
-    PSe = {
+    OSe = {
         class: "selectOptions"
     },
-    OSe = ["data-value"],
-    FSe = {
+    FSe = ["data-value"],
+    BSe = {
         class: "flexRow"
     },
-    BSe = Pi({
+    WSe = Pi({
         __name: "BuilderSelect",
         props: {
             options: {},
             defaultValue: {},
             defaultIcon: {}
         },
         emits: ["select"],
@@ -107741,52 +107743,52 @@
             return (h, u) => (J(), he("div", {
                 class: "selectWrapper",
                 onClick: d
             }, [F("div", {
                 ref_key: "selectEl",
                 ref: t,
                 class: "select"
-            }, [F("div", NSe, [F("div", RSe, [s.value != null ? (J(), he("div", MSe, [F("div", null, [F("i", {
+            }, [F("div", RSe, [F("div", MSe, [s.value != null ? (J(), he("div", ASe, [F("div", null, [F("i", {
                 class: xt(r.value)
-            }, null, 2)]), F("div", null, kt(s.value), 1)])) : Te("", !0)]), ASe]), F("div", PSe, [(J(!0), he(hi, null, Hn(_e(l), g => (J(), he("div", {
+            }, null, 2)]), F("div", null, kt(s.value), 1)])) : Te("", !0)]), PSe]), F("div", OSe, [(J(!0), he(hi, null, Hn(_e(l), g => (J(), he("div", {
                 key: g.value,
                 class: xt(["selectOption", g.class]),
                 "data-value": g.value,
                 onClick: c
-            }, [F("div", FSe, [F("div", null, [F("i", {
+            }, [F("div", BSe, [F("div", null, [F("i", {
                 class: xt(g.icon)
-            }, null, 2)]), F("div", null, kt(g.label), 1)])], 10, OSe))), 128))])], 512)]))
+            }, null, 2)]), F("div", null, kt(g.label), 1)])], 10, FSe))), 128))])], 512)]))
         }
     });
-const MA = Li(BSe, [
+const MA = Li(WSe, [
         ["__scopeId", "data-v-510f1335"]
     ]),
-    WSe = o => (Nn("data-v-75b5ce4b"), o = o(), Rn(), o),
-    VSe = {
+    VSe = o => (Nn("data-v-75b5ce4b"), o = o(), Rn(), o),
+    HSe = {
         class: "chipStackContainer"
     },
-    HSe = {
+    zSe = {
         class: "chipStack"
     },
-    zSe = {
+    $Se = {
         key: 0,
         class: "main"
     },
-    $Se = {
+    USe = {
         key: 0,
         class: "pickerContainer"
     },
-    USe = {
+    jSe = {
         key: 0,
         class: "fixedContainer"
     },
-    jSe = ["value"],
-    KSe = WSe(() => F("div", null, "px", -1)),
-    qSe = ["value"],
-    GSe = Pi({
+    KSe = ["value"],
+    qSe = VSe(() => F("div", null, "px", -1)),
+    GSe = ["value"],
+    ZSe = Pi({
         __name: "BuilderFieldsWidth",
         props: {
             componentId: {},
             fieldKey: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -107878,15 +107880,15 @@
             }), Bb(() => {
                 n.value.removeEventListener("focus", w)
             }), (L, E) => (J(), he("div", {
                 ref_key: "rootEl",
                 ref: n,
                 class: "BuilderFieldsWidth",
                 tabindex: "-1"
-            }, [F("div", VSe, [F("div", HSe, [F("button", {
+            }, [F("div", HSe, [F("div", zSe, [F("button", {
                 class: xt(["chip", {
                     active: C.value == "default"
                 }]),
                 tabindex: "0",
                 onClick: E[0] || (E[0] = () => {
                     S("default"), _e(i)(g.value.id, _e(u), void 0)
                 })
@@ -107898,53 +107900,53 @@
                 onClick: E[1] || (E[1] = T => S("css"))
             }, " CSS ", 2), F("button", {
                 class: xt(["chip", {
                     active: C.value == "pick"
                 }]),
                 tabindex: "0",
                 onClick: E[2] || (E[2] = T => S("pick"))
-            }, " Pick ", 2)])]), C.value == "pick" || C.value == "css" ? (J(), he("div", zSe, [C.value == "pick" ? (J(), he("div", $Se, [on(MA, {
+            }, " Pick ", 2)])]), C.value == "pick" || C.value == "css" ? (J(), he("div", $Se, [C.value == "pick" ? (J(), he("div", USe, [on(MA, {
                 "default-value": m.value,
                 options: f.value,
                 onSelect: k
-            }, null, 8, ["default-value", "options"]), m.value == "fixed" ? (J(), he("div", USe, [F("input", {
+            }, null, 8, ["default-value", "options"]), m.value == "fixed" ? (J(), he("div", jSe, [F("input", {
                 ref_key: "fixedEl",
                 ref: r,
                 type: "text",
                 value: v.value,
                 onInput: x
-            }, null, 40, jSe), KSe])) : Te("", !0)])) : Te("", !0), C.value == "css" ? (J(), he("input", {
+            }, null, 40, KSe), qSe])) : Te("", !0)])) : Te("", !0), C.value == "css" ? (J(), he("input", {
                 key: 1,
                 ref_key: "freehandInputEl",
                 ref: a,
                 type: "text",
                 value: g.value.content[_e(u)],
                 onInput: y
-            }, null, 40, qSe)) : Te("", !0)])) : Te("", !0)], 512))
+            }, null, 40, GSe)) : Te("", !0)])) : Te("", !0)], 512))
         }
     });
-const ZSe = Li(GSe, [
+const YSe = Li(ZSe, [
         ["__scopeId", "data-v-75b5ce4b"]
     ]),
-    YSe = {
+    XSe = {
         class: "chipStackContainer"
     },
-    XSe = {
+    QSe = {
         class: "chipStack"
     },
-    QSe = {
+    JSe = {
         key: 0,
         class: "main"
     },
-    JSe = {
+    eye = {
         key: 0,
         class: "pickerContainer"
     },
-    eye = ["value"],
-    tye = Pi({
+    tye = ["value"],
+    iye = Pi({
         __name: "BuilderFieldsAlign",
         props: {
             componentId: {},
             fieldKey: {},
             direction: {}
         },
         setup(o) {
@@ -108049,15 +108051,15 @@
             }), Bb(() => {
                 n.value.removeEventListener("focus", S)
             }), (L, E) => (J(), he("div", {
                 ref_key: "rootEl",
                 ref: n,
                 class: "BuilderFieldsAlign",
                 tabindex: "-1"
-            }, [F("div", YSe, [F("div", XSe, [F("button", {
+            }, [F("div", XSe, [F("div", QSe, [F("button", {
                 class: xt(["chip", {
                     active: w.value == "default"
                 }]),
                 tabindex: "0",
                 onClick: E[0] || (E[0] = () => {
                     k("default"), _e(i)(f.value.id, _e(u), void 0)
                 })
@@ -108069,111 +108071,111 @@
                 onClick: E[1] || (E[1] = T => k("css"))
             }, " CSS ", 2), F("button", {
                 class: xt(["chip", {
                     active: w.value == "pick"
                 }]),
                 tabindex: "0",
                 onClick: E[2] || (E[2] = T => k("pick"))
-            }, " Pick ", 2)])]), w.value == "pick" || w.value == "css" ? (J(), he("div", QSe, [w.value == "pick" ? (J(), he("div", JSe, [on(MA, {
+            }, " Pick ", 2)])]), w.value == "pick" || w.value == "css" ? (J(), he("div", JSe, [w.value == "pick" ? (J(), he("div", eye, [on(MA, {
                 "default-value": v.value,
                 options: _.value,
                 onSelect: y
             }, null, 8, ["default-value", "options"])])) : Te("", !0), w.value == "css" ? (J(), he("input", {
                 key: 1,
                 ref_key: "freehandInputEl",
                 ref: r,
                 type: "text",
                 value: f.value.content[_e(u)],
                 onInput: x
-            }, null, 40, eye)) : Te("", !0)])) : Te("", !0)], 512))
+            }, null, 40, tye)) : Te("", !0)])) : Te("", !0)], 512))
         }
     });
-const e9 = Li(tye, [
+const e9 = Li(iye, [
         ["__scopeId", "data-v-5309ecc1"]
     ]),
     jo = o => (Nn("data-v-2078a3cf"), o = o(), Rn(), o),
-    iye = {
+    nye = {
         class: "chipStackContainer"
     },
-    nye = {
+    sye = {
         class: "chipStack"
     },
-    sye = {
+    oye = {
         key: 0,
         class: "main"
     },
-    oye = {
+    rye = {
         key: 0,
         class: "pickerContainer"
     },
-    rye = {
+    aye = {
         key: 0,
         class: "row"
     },
-    aye = jo(() => F("i", {
+    lye = jo(() => F("i", {
         class: "ico ico-padding-4-side"
     }, null, -1)),
-    lye = ["value"],
-    dye = jo(() => F("div", null, "px", -1)),
-    cye = {
+    dye = ["value"],
+    cye = jo(() => F("div", null, "px", -1)),
+    hye = {
         key: 1
     },
-    hye = {
+    uye = {
         class: "row"
     },
-    uye = jo(() => F("i", {
+    gye = jo(() => F("i", {
         class: "ico ico-padding-x-side"
     }, null, -1)),
-    gye = ["value"],
-    fye = jo(() => F("div", null, "px", -1)),
-    pye = {
+    fye = ["value"],
+    pye = jo(() => F("div", null, "px", -1)),
+    mye = {
         class: "row"
     },
-    mye = jo(() => F("i", {
+    _ye = jo(() => F("i", {
         class: "ico ico-padding-y-side"
     }, null, -1)),
-    _ye = ["value"],
-    vye = jo(() => F("div", null, "px", -1)),
-    bye = {
+    vye = ["value"],
+    bye = jo(() => F("div", null, "px", -1)),
+    Cye = {
         key: 2
     },
-    Cye = {
+    wye = {
         class: "row"
     },
-    wye = jo(() => F("i", {
+    Sye = jo(() => F("i", {
         class: "ico ico-padding-left-side"
     }, null, -1)),
-    Sye = ["value"],
-    yye = jo(() => F("div", null, "px", -1)),
-    Lye = {
+    yye = ["value"],
+    Lye = jo(() => F("div", null, "px", -1)),
+    xye = {
         class: "row"
     },
-    xye = jo(() => F("i", {
+    Dye = jo(() => F("i", {
         class: "ico ico-padding-right-side"
     }, null, -1)),
-    Dye = ["value"],
-    kye = jo(() => F("div", null, "px", -1)),
-    Iye = {
+    kye = ["value"],
+    Iye = jo(() => F("div", null, "px", -1)),
+    Eye = {
         class: "row"
     },
-    Eye = jo(() => F("i", {
+    Tye = jo(() => F("i", {
         class: "ico ico-padding-top-side"
     }, null, -1)),
-    Tye = ["value"],
-    Nye = jo(() => F("div", null, "px", -1)),
-    Rye = {
+    Nye = ["value"],
+    Rye = jo(() => F("div", null, "px", -1)),
+    Mye = {
         class: "row"
     },
-    Mye = jo(() => F("i", {
+    Aye = jo(() => F("i", {
         class: "ico ico-padding-bottom-side"
     }, null, -1)),
-    Aye = ["value"],
-    Pye = jo(() => F("div", null, "px", -1)),
-    Oye = ["value"],
-    Fye = Pi({
+    Pye = ["value"],
+    Oye = jo(() => F("div", null, "px", -1)),
+    Fye = ["value"],
+    Bye = Pi({
         __name: "BuilderFieldsPadding",
         props: {
             componentId: {},
             fieldKey: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -108281,15 +108283,15 @@
             }), Bb(() => {
                 n.value.removeEventListener("focus", S)
             }), (E, T) => (J(), he("div", {
                 ref_key: "rootEl",
                 ref: n,
                 class: "BuilderFieldsPadding",
                 tabindex: "-1"
-            }, [F("div", iye, [F("div", nye, [F("button", {
+            }, [F("div", nye, [F("div", sye, [F("button", {
                 class: xt(["chip", {
                     active: w.value == "default"
                 }]),
                 tabindex: "0",
                 onClick: T[0] || (T[0] = () => {
                     k("default"), _e(i)(g.value.id, _e(u), void 0)
                 })
@@ -108301,93 +108303,93 @@
                 onClick: T[1] || (T[1] = M => k("css"))
             }, " CSS ", 2), F("button", {
                 class: xt(["chip", {
                     active: w.value == "pick"
                 }]),
                 tabindex: "0",
                 onClick: T[2] || (T[2] = M => k("pick"))
-            }, " Pick ", 2)])]), w.value == "pick" || w.value == "css" ? (J(), he("div", sye, [w.value == "pick" ? (J(), he("div", oye, [on(MA, {
+            }, " Pick ", 2)])]), w.value == "pick" || w.value == "css" ? (J(), he("div", oye, [w.value == "pick" ? (J(), he("div", rye, [on(MA, {
                 "default-value": m.value,
                 options: f.value,
                 onSelect: y
-            }, null, 8, ["default-value", "options"]), m.value == "all_sides" ? (J(), he("div", rye, [aye, F("input", {
+            }, null, 8, ["default-value", "options"]), m.value == "all_sides" ? (J(), he("div", aye, [lye, F("input", {
                 ref_key: "fixedEl",
                 ref: r,
                 type: "text",
                 value: v.value[0],
                 onInput: T[3] || (T[3] = M => L(M, m.value))
-            }, null, 40, lye), dye])) : Te("", !0), m.value == "XY sides" ? (J(), he("div", cye, [F("div", hye, [uye, F("input", {
+            }, null, 40, dye), cye])) : Te("", !0), m.value == "XY sides" ? (J(), he("div", hye, [F("div", uye, [gye, F("input", {
                 ref_key: "fixedEl",
                 ref: r,
                 type: "text",
                 value: v.value[0],
                 onInput: T[4] || (T[4] = M => L(M, m.value, "x"))
-            }, null, 40, gye), fye]), F("div", pye, [mye, F("input", {
+            }, null, 40, fye), pye]), F("div", mye, [_ye, F("input", {
                 type: "text",
                 value: v.value[2],
                 onInput: T[5] || (T[5] = M => L(M, m.value, "y"))
-            }, null, 40, _ye), vye])])) : Te("", !0), m.value == "Per side" ? (J(), he("div", bye, [F("div", Cye, [wye, F("input", {
+            }, null, 40, vye), bye])])) : Te("", !0), m.value == "Per side" ? (J(), he("div", Cye, [F("div", wye, [Sye, F("input", {
                 ref_key: "fixedEl",
                 ref: r,
                 type: "text",
                 value: v.value[0],
                 onInput: T[6] || (T[6] = M => L(M, m.value, "left"))
-            }, null, 40, Sye), yye]), F("div", Lye, [xye, F("input", {
+            }, null, 40, yye), Lye]), F("div", xye, [Dye, F("input", {
                 type: "text",
                 value: v.value[1],
                 onInput: T[7] || (T[7] = M => L(M, m.value, "right"))
-            }, null, 40, Dye), kye]), F("div", Iye, [Eye, F("input", {
+            }, null, 40, kye), Iye]), F("div", Eye, [Tye, F("input", {
                 type: "text",
                 value: v.value[2],
                 onInput: T[8] || (T[8] = M => L(M, m.value, "top"))
-            }, null, 40, Tye), Nye]), F("div", Rye, [Mye, F("input", {
+            }, null, 40, Nye), Rye]), F("div", Mye, [Aye, F("input", {
                 type: "text",
                 value: v.value[3],
                 onInput: T[9] || (T[9] = M => L(M, m.value, "bottom"))
-            }, null, 40, Aye), Pye])])) : Te("", !0)])) : Te("", !0), w.value == "css" ? (J(), he("input", {
+            }, null, 40, Pye), Oye])])) : Te("", !0)])) : Te("", !0), w.value == "css" ? (J(), he("input", {
                 key: 1,
                 ref_key: "freehandInputEl",
                 ref: a,
                 type: "text",
                 value: g.value.content[_e(u)],
                 onInput: x
-            }, null, 40, Oye)) : Te("", !0)])) : Te("", !0)], 512))
+            }, null, 40, Fye)) : Te("", !0)])) : Te("", !0)], 512))
         }
     });
-const Bye = Li(Fye, [
+const Wye = Li(Bye, [
         ["__scopeId", "data-v-2078a3cf"]
     ]),
-    Wye = o => (Nn("data-v-8ed4dc9e"), o = o(), Rn(), o),
-    Vye = {
+    Vye = o => (Nn("data-v-8ed4dc9e"), o = o(), Rn(), o),
+    Hye = {
         key: 0,
         class: "BuilderSettingsProperties"
     },
-    Hye = Wye(() => F("div", {
+    zye = Vye(() => F("div", {
         class: "sectionTitle"
     }, [F("i", {
         class: "ri-equalizer-line ri-xl"
     }), F("h3", null, "Properties")], -1)),
-    zye = {
+    $ye = {
         key: 0,
         class: "title"
     },
-    $ye = {
+    Uye = {
         class: "fieldWrapper"
     },
-    Uye = {
+    jye = {
         class: "name"
     },
-    jye = {
+    Kye = {
         class: "type"
     },
-    Kye = {
+    qye = {
         key: 11,
         class: "desc"
     },
-    qye = Pi({
+    Gye = Pi({
         __name: "BuilderSettingsProperties",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 i = Ue(() => e.getComponentById(t.getSelectedId())),
                 n = Ue(() => {
                     const {
@@ -108399,25 +108401,25 @@
                 r = Ue(() => {
                     const a = Object.entries(n.value);
                     return {
                         [$g.General]: a.filter(([d, c]) => !c.category || c.category == $g.General),
                         [$g.Style]: a.filter(([d, c]) => c.category == $g.Style)
                     }
                 });
-            return (a, l) => _e(t).isSelectionActive() && n.value ? (J(), he("div", Vye, [Hye, F("div", null, [(J(), he(hi, null, Hn(s, d => F("div", {
+            return (a, l) => _e(t).isSelectionActive() && n.value ? (J(), he("div", Hye, [zye, F("div", null, [(J(), he(hi, null, Hn(s, d => F("div", {
                 key: d,
                 class: "propertyCategory"
-            }, [r.value[d].length > 0 ? (J(), he("div", zye, [F("h4", null, kt(d), 1)])) : Te("", !0), (J(!0), he(hi, null, Hn(r.value[d], ([c, h]) => (J(), he("div", {
+            }, [r.value[d].length > 0 ? (J(), he("div", $ye, [F("h4", null, kt(d), 1)])) : Te("", !0), (J(!0), he(hi, null, Hn(r.value[d], ([c, h]) => (J(), he("div", {
                 key: c
-            }, [F("div", $ye, [F("div", Uye, [Gi(kt(h.name ?? c), 1), F("span", jye, " : " + kt(h.type), 1)]), h.type == _e(Yr).Color ? (J(), Fn(Xwe, {
+            }, [F("div", Uye, [F("div", jye, [Gi(kt(h.name ?? c), 1), F("span", Kye, " : " + kt(h.type), 1)]), h.type == _e(Yr).Color ? (J(), Fn(Qwe, {
                 key: 0,
                 class: "content",
                 "field-key": c,
                 "component-id": i.value.id
-            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Shadow ? (J(), Fn(ySe, {
+            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Shadow ? (J(), Fn(LSe, {
                 key: 1,
                 class: "content",
                 "field-key": c,
                 "component-id": i.value.id
             }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).KeyValue ? (J(), Fn($we, {
                 key: 2,
                 class: "content",
@@ -108436,15 +108438,15 @@
                 "field-key": c,
                 "component-id": i.value.id
             }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Object ? (J(), Fn(Bz, {
                 key: 6,
                 class: "content",
                 "field-key": c,
                 "component-id": i.value.id
-            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Width ? (J(), Fn(ZSe, {
+            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Width ? (J(), Fn(YSe, {
                 key: 7,
                 class: "content",
                 "field-key": c,
                 "component-id": i.value.id
             }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).HAlign ? (J(), Fn(e9, {
                 key: 8,
                 class: "content",
@@ -108453,192 +108455,192 @@
                 "component-id": i.value.id
             }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).VAlign ? (J(), Fn(e9, {
                 key: 9,
                 class: "content",
                 direction: "vertical",
                 "field-key": c,
                 "component-id": i.value.id
-            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Padding ? (J(), Fn(Bye, {
+            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.type == _e(Yr).Padding ? (J(), Fn(Wye, {
                 key: 10,
                 class: "content",
                 "field-key": c,
                 "component-id": i.value.id
-            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.desc ? (J(), he("div", Kye, kt(h.desc), 1)) : Te("", !0)])]))), 128))])), 64))])])) : Te("", !0)
+            }, null, 8, ["field-key", "component-id"])) : Te("", !0), h.desc ? (J(), he("div", qye, kt(h.desc), 1)) : Te("", !0)])]))), 128))])), 64))])])) : Te("", !0)
         }
     });
-const Gye = Li(qye, [
+const Zye = Li(Gye, [
         ["__scopeId", "data-v-8ed4dc9e"]
     ]),
     AA = o => (Nn("data-v-968a15bf"), o = o(), Rn(), o),
-    Zye = {
+    Yye = {
         key: 0,
         class: "BuilderSettingsBinding"
     },
-    Yye = AA(() => F("div", {
+    Xye = AA(() => F("div", {
         class: "sectionTitle"
     }, [F("i", {
         class: "ri-links-line ri-xl"
     }), F("h3", null, "Binding")], -1)),
-    Xye = {
+    Qye = {
         class: "main"
     },
-    Qye = {
+    Jye = {
         class: "fieldWrapper"
     },
-    Jye = AA(() => F("span", {
+    eLe = AA(() => F("span", {
         class: "name"
     }, "State element", -1)),
-    eLe = ["value"],
-    tLe = AA(() => F("div", {
+    tLe = ["value"],
+    iLe = AA(() => F("div", {
         class: "desc"
     }, ' Links this component to a state element, in a two-way fashion. Reference the state element directly, i.e. use "my_var" instead of "@{my_var}". ', -1)),
-    iLe = Pi({
+    nLe = Pi({
         __name: "BuilderSettingsBinding",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 {
                     setBinding: i
                 } = Js(e, t),
                 n = Ue(() => e.getComponentById(t.getSelectedId()));
             return (s, r) => {
                 var a;
-                return _e(t).isSelectionActive() ? (J(), he("div", Zye, [Yye, F("div", Xye, [F("div", Qye, [Jye, F("input", {
+                return _e(t).isSelectionActive() ? (J(), he("div", Yye, [Xye, F("div", Qye, [F("div", Jye, [eLe, F("input", {
                     value: (a = n.value.binding) == null ? void 0 : a.stateRef,
                     type: "text",
                     class: "content",
                     placeholder: "my_var",
                     onInput: r[0] || (r[0] = l => _e(i)(n.value.id, l.target.value))
-                }, null, 40, eLe), tLe])])])) : Te("", !0)
+                }, null, 40, tLe), iLe])])])) : Te("", !0)
             }
         }
     });
-const nLe = Li(iLe, [
+const sLe = Li(nLe, [
         ["__scopeId", "data-v-968a15bf"]
     ]),
     PA = o => (Nn("data-v-ec4f56f8"), o = o(), Rn(), o),
-    sLe = {
+    oLe = {
         key: 0,
         class: "BuilderSettingsVisibility"
     },
-    oLe = PA(() => F("div", {
+    rLe = PA(() => F("div", {
         class: "sectionTitle"
     }, [F("i", {
         class: "ri-eye-line ri-xl"
     }), F("h3", null, "Visibility")], -1)),
-    rLe = {
+    aLe = {
         class: "main"
     },
-    aLe = {
+    lLe = {
         class: "chipStack"
     },
-    lLe = {
+    dLe = {
         key: 0,
         class: "fieldWrapper"
     },
-    dLe = PA(() => F("span", {
+    cLe = PA(() => F("span", {
         class: "name"
     }, "Visibility value", -1)),
-    cLe = ["value"],
-    hLe = PA(() => F("div", {
+    hLe = ["value"],
+    uLe = PA(() => F("div", {
         class: "desc"
     }, ' Reference a state or context element that will evaluate to true or false. Reference the element directly, i.e. use "my_var" instead of "@{my_var}". ', -1)),
-    uLe = Pi({
+    gLe = Pi({
         __name: "BuilderSettingsVisibility",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 {
                     setVisibleValue: i
                 } = Js(e, t),
                 n = Ue(() => e.getComponentById(t.getSelectedId()));
-            return (s, r) => _e(t).isSelectionActive() ? (J(), he("div", sLe, [oLe, F("div", rLe, [F("div", aLe, [F("div", {
+            return (s, r) => _e(t).isSelectionActive() ? (J(), he("div", oLe, [rLe, F("div", aLe, [F("div", lLe, [F("div", {
                 class: xt(["chip", {
                     active: typeof n.value.visible > "u" || n.value.visible === !0
                 }]),
                 onClick: r[0] || (r[0] = () => _e(i)(n.value.id, !0))
             }, " Yes ", 2), F("div", {
                 class: xt(["chip", {
                     active: n.value.visible === !1
                 }]),
                 onClick: r[1] || (r[1] = () => _e(i)(n.value.id, !1))
             }, " No ", 2), F("div", {
                 class: xt(["chip", {
                     active: typeof n.value.visible == "string"
                 }]),
                 onClick: r[2] || (r[2] = () => _e(i)(n.value.id, ""))
-            }, " Custom ", 2)]), typeof n.value.visible == "string" ? (J(), he("div", lLe, [dLe, F("input", {
+            }, " Custom ", 2)]), typeof n.value.visible == "string" ? (J(), he("div", dLe, [cLe, F("input", {
                 value: n.value.visible,
                 type: "text",
                 class: "content",
                 placeholder: "my_visibility_state_value",
                 onInput: r[3] || (r[3] = a => _e(i)(n.value.id, a.target.value))
-            }, null, 40, cLe), hLe])) : Te("", !0)])])) : Te("", !0)
+            }, null, 40, hLe), uLe])) : Te("", !0)])])) : Te("", !0)
         }
     });
-const gLe = Li(uLe, [
+const fLe = Li(gLe, [
         ["__scopeId", "data-v-ec4f56f8"]
     ]),
-    T0 = o => (Nn("data-v-5e4004d6"), o = o(), Rn(), o),
-    fLe = {
+    T0 = o => (Nn("data-v-e803ab69"), o = o(), Rn(), o),
+    pLe = {
         key: 0,
         class: "BuilderSettings"
     },
-    pLe = {
+    mLe = {
         class: "windowBar"
     },
-    mLe = T0(() => F("div", {
+    _Le = T0(() => F("div", {
         class: "icon"
     }, [F("i", {
         class: "ri-settings-3-line ri-lg"
     })], -1)),
-    _Le = {
+    vLe = {
         class: "title"
     },
-    vLe = ["title"],
-    bLe = T0(() => F("i", {
+    bLe = ["title"],
+    CLe = T0(() => F("i", {
         class: "ri-question-line ri-lg"
     }, null, -1)),
-    CLe = {
+    wLe = {
         key: 0,
         class: "ri-arrow-drop-up-line ri-lg"
     },
-    wLe = {
+    SLe = {
         key: 1,
         class: "ri-arrow-drop-down-line ri-lg"
     },
-    SLe = T0(() => F("i", {
+    yLe = T0(() => F("i", {
         class: "ri-close-line ri-lg"
     }, null, -1)),
-    yLe = [SLe],
-    LLe = {
+    LLe = [yLe],
+    xLe = {
         key: 0,
         class: "docs"
     },
-    xLe = {
+    DLe = {
         key: 0
     },
-    DLe = {
+    kLe = {
         key: 1,
         class: "markdown"
     },
-    kLe = {
+    ILe = {
         key: 1,
-        class: "warning"
+        class: "warning cmc-warning"
     },
-    ILe = T0(() => F("i", {
+    ELe = T0(() => F("i", {
         class: "ri-error-warning-line ri-xl"
     }, null, -1)),
-    ELe = T0(() => F("span", null, " This component is instantiated in code. All settings in this panel are read-only and cannot be edited. ", -1)),
-    TLe = [ILe, ELe],
-    NLe = ["inert"],
-    RLe = {
+    TLe = T0(() => F("span", null, " This component is instantiated in code. All settings in this panel are read-only and cannot be edited. ", -1)),
+    NLe = [ELe, TLe],
+    RLe = ["inert"],
+    MLe = {
         class: "debug"
     },
-    MLe = Pi({
+    ALe = Pi({
         __name: "BuilderSettings",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 i = Je(!1),
                 n = Ue(() => e.getComponentById(t.getSelectedId())),
                 s = Ue(() => n.value.isCodeManaged),
@@ -108668,157 +108670,157 @@
                 h = Ue(() => {
                     var g;
                     if ((g = r.value) != null && g.docs) return r.value.docs.trim()
                 }),
                 u = () => Gz.parse(h.value);
             return (g, f) => {
                 const m = zS("dompurify-html");
-                return _e(t).isSelectionActive() ? (J(), he("div", fLe, [F("div", pLe, [mLe, F("div", _Le, kt(r.value.name), 1), c.value || h.value ? (J(), he("button", {
+                return _e(t).isSelectionActive() ? (J(), he("div", pLe, [F("div", mLe, [_Le, F("div", vLe, kt(r.value.name), 1), c.value || h.value ? (J(), he("button", {
                     key: 0,
                     class: "windowAction",
                     tabindex: "0",
                     title: (i.value ? "Hide" : "Show") + " inline docs",
                     onClick: l
-                }, [bLe, i.value ? (J(), he("i", CLe)) : (J(), he("i", wLe))], 8, vLe)) : Te("", !0), F("button", {
+                }, [CLe, i.value ? (J(), he("i", wLe)) : (J(), he("i", SLe))], 8, bLe)) : Te("", !0), F("button", {
                     class: "windowAction",
                     tabindex: "0",
                     title: "Close (Esc)",
                     onClick: a
-                }, yLe)]), i.value ? (J(), he("div", LLe, [c.value ? (J(), he("div", xLe, kt(c.value), 1)) : Te("", !0), h.value ? Un((J(), he("div", DLe, null, 512)), [
+                }, LLe)]), i.value ? (J(), he("div", xLe, [c.value ? (J(), he("div", DLe, kt(c.value), 1)) : Te("", !0), h.value ? Un((J(), he("div", kLe, null, 512)), [
                     [m, u()]
-                ]) : Te("", !0)])) : Te("", !0), s.value ? (J(), he("div", kLe, TLe)) : Te("", !0), F("div", {
+                ]) : Te("", !0)])) : Te("", !0), s.value ? (J(), he("div", ILe, NLe)) : Te("", !0), F("div", {
                     class: "sections",
                     inert: s.value
-                }, [on(Gye), d.value ? (J(), Fn(nLe, {
+                }, [on(Zye), d.value ? (J(), Fn(sLe, {
                     key: 0
-                })) : Te("", !0), on(Nwe), on(gLe)], 8, NLe), F("div", RLe, " Component id: " + kt(_e(t).getSelectedId()), 1)])) : Te("", !0)
+                })) : Te("", !0), on(Nwe), on(fLe)], 8, RLe), F("div", MLe, " Component id: " + kt(_e(t).getSelectedId()), 1)])) : Te("", !0)
             }
         }
     });
-const ALe = Li(MLe, [
-    ["__scopeId", "data-v-5e4004d6"]
+const PLe = Li(ALe, [
+    ["__scopeId", "data-v-e803ab69"]
 ]);
 
-function PLe() {
+function OLe() {
     var e;
     return ((e = navigator == null ? void 0 : navigator.userAgentData) == null ? void 0 : e.platform) || (navigator == null ? void 0 : navigator.platform)
 }
 
 function HS() {
-    return PLe().toLowerCase().indexOf("mac") != -1
+    return OLe().toLowerCase().indexOf("mac") != -1
 }
 const Rh = o => (Nn("data-v-caebba71"), o = o(), Rn(), o),
-    OLe = {
+    FLe = {
         class: "editor"
     },
-    FLe = {
+    BLe = {
         class: "windowBar"
     },
-    BLe = Rh(() => F("div", {
+    WLe = Rh(() => F("div", {
         class: "icon"
     }, [F("i", {
         class: "ri-code-line ri-lg"
     })], -1)),
-    WLe = Rh(() => F("div", {
+    VLe = Rh(() => F("div", {
         class: "title"
     }, "Code Editor", -1)),
-    VLe = ["title"],
-    HLe = {
+    HLe = ["title"],
+    zLe = {
         class: "ri-sun-line ri-lg"
     },
-    zLe = {
+    $Le = {
         class: "ri-moon-line ri-lg"
     },
-    $Le = {
+    ULe = {
         class: "codeActions"
     },
-    ULe = ["disabled", "title"],
-    jLe = Rh(() => F("i", {
+    jLe = ["disabled", "title"],
+    KLe = Rh(() => F("i", {
         class: "ri-save-line"
     }, null, -1)),
-    KLe = {
+    qLe = {
         key: 0,
         class: "statusMessage"
     },
-    qLe = {
+    GLe = {
         key: 0,
         class: "statusOk ok"
     },
-    GLe = Rh(() => F("i", {
+    ZLe = Rh(() => F("i", {
         class: "ri-check-line"
     }, null, -1)),
-    ZLe = [GLe],
-    YLe = {
+    YLe = [ZLe],
+    XLe = {
         key: 1,
         class: "statusOk notOk"
     },
-    XLe = Rh(() => F("i", {
+    QLe = Rh(() => F("i", {
         class: "ri-error-warning-line"
     }, null, -1)),
-    QLe = [XLe],
-    JLe = {
+    JLe = [QLe],
+    exe = {
         key: 2,
         class: "statusOk processing"
     },
-    exe = Rh(() => F("i", {
+    txe = Rh(() => F("i", {
         class: "ri-loader-3-line"
     }, null, -1)),
-    txe = [exe],
-    ixe = {
+    ixe = [txe],
+    nxe = {
         class: "log"
     },
-    nxe = {
+    sxe = {
         class: "windowBar"
     },
-    sxe = Rh(() => F("div", {
+    oxe = Rh(() => F("div", {
         class: "icon"
     }, [F("i", {
         class: "ri-booklet-line"
     })], -1)),
-    oxe = {
+    rxe = {
         class: "title"
     },
-    rxe = {
+    axe = {
         class: "countLabel"
     },
-    axe = Rh(() => F("i", {
+    lxe = Rh(() => F("i", {
         class: "ri-delete-bin-line"
     }, null, -1)),
-    lxe = [axe],
-    dxe = ["title"],
-    cxe = {
+    dxe = [lxe],
+    cxe = ["title"],
+    hxe = {
         class: "ri-arrow-drop-up-line ri-lg"
     },
-    hxe = {
+    uxe = {
         class: "ri-arrow-drop-down-line ri-lg"
     },
-    uxe = {
+    gxe = {
         key: 0,
         class: "entryContainer"
     },
-    gxe = {
+    fxe = {
         class: "content"
     },
-    fxe = {
+    pxe = {
         class: "header"
     },
-    pxe = {
+    mxe = {
         class: "title"
     },
-    mxe = {
+    _xe = {
         class: "time"
     },
-    _xe = {
+    vxe = {
         class: "message"
     },
-    vxe = {
+    bxe = {
         key: 0,
         class: "codeContainer"
     },
-    bxe = Pi({
+    Cxe = Pi({
         __name: "BuilderEditor",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 i = Je(null),
                 n = Je(null),
                 s = Je(!1);
@@ -108910,88 +108912,88 @@
                 ref_key: "builderEditor",
                 ref: i,
                 class: xt(["BuilderEditor", {
                     dark: l.value == "vs-dark",
                     light: l.value == "vs-light",
                     activeLog: d.value
                 }])
-            }, [F("div", OLe, [F("div", FLe, [BLe, WLe, F("button", {
+            }, [F("div", FLe, [F("div", BLe, [WLe, VLe, F("button", {
                 class: "windowAction",
                 tabindex: "0",
                 title: (l.value == "vs-light" ? "Dark" : "Light") + " theme",
                 onClick: w
-            }, [Un(F("i", HLe, null, 512), [
+            }, [Un(F("i", zLe, null, 512), [
                 [ga, l.value == "vs-dark"]
-            ]), Un(F("i", zLe, null, 512), [
+            ]), Un(F("i", $Le, null, 512), [
                 [ga, l.value == "vs-light"]
-            ])], 8, VLe)]), F("div", $Le, [F("button", {
+            ])], 8, HLe)]), F("div", ULe, [F("button", {
                 disabled: s.value,
                 title: `Save and run (${_e(a)}+s)`,
                 onClick: b
-            }, [jLe, Gi(kt("Save and run"))], 8, ULe), h.value ? (J(), he("div", KLe, [h.value.ok === !0 ? (J(), he("div", qLe, ZLe)) : h.value.ok === !1 ? (J(), he("div", YLe, QLe)) : h.value.ok === "processing" ? (J(), he("div", JLe, txe)) : Te("", !0), Gi(" " + kt(h.value.message), 1)])) : Te("", !0)]), F("div", {
+            }, [KLe, Gi(kt("Save and run"))], 8, jLe), h.value ? (J(), he("div", qLe, [h.value.ok === !0 ? (J(), he("div", GLe, YLe)) : h.value.ok === !1 ? (J(), he("div", XLe, JLe)) : h.value.ok === "processing" ? (J(), he("div", exe, ixe)) : Te("", !0), Gi(" " + kt(h.value.message), 1)])) : Te("", !0)]), F("div", {
                 ref_key: "editorContainer",
                 ref: n,
                 class: "editorContainer"
-            }, null, 512)]), F("div", ixe, [F("div", nxe, [sxe, F("div", oxe, [Gi(" Log "), F("span", rxe, kt(g.value.length), 1)]), F("button", {
+            }, null, 512)]), F("div", nxe, [F("div", sxe, [oxe, F("div", rxe, [Gi(" Log "), F("span", axe, kt(g.value.length), 1)]), F("button", {
                 class: "windowAction",
                 tabindex: "0",
                 title: "Clear log",
                 onClick: y[0] || (y[0] = (...x) => _e(t).clearLogEntries && _e(t).clearLogEntries(...x))
-            }, lxe), F("button", {
+            }, dxe), F("button", {
                 class: "windowAction",
                 tabindex: "0",
                 title: (d.value ? "Hide" : "Show") + ` log (${_e(a)}+j)`,
                 onClick: C
-            }, [Un(F("i", cxe, null, 512), [
+            }, [Un(F("i", hxe, null, 512), [
                 [ga, !d.value]
-            ]), Un(F("i", hxe, null, 512), [
+            ]), Un(F("i", uxe, null, 512), [
                 [ga, d.value]
-            ])], 8, dxe)]), d.value ? (J(), he("div", uxe, [(J(!0), he(hi, null, Hn(g.value, (x, L) => (J(), he("div", {
+            ])], 8, cxe)]), d.value ? (J(), he("div", gxe, [(J(!0), he(hi, null, Hn(g.value, (x, L) => (J(), he("div", {
                 key: L,
                 class: "entry"
             }, [F("div", {
                 class: xt(["icon", x.type])
             }, [F("i", {
                 class: xt([u[x.type], "ri-xl"])
-            }, null, 2)], 2), F("div", gxe, [F("div", fxe, [F("span", pxe, kt(x.title) + kt(x.repeated > 0 ? ` · Repeated ${x.repeated} times` : ""), 1), F("span", mxe, kt(x.timestampReceived.toLocaleTimeString()), 1)]), F("div", _xe, [Gi(kt(x.message) + " ", 1), x.code ? (J(), he("div", vxe, [F("code", null, kt(x.code), 1)])) : Te("", !0)])])]))), 128))])) : Te("", !0)])], 2))
+            }, null, 2)], 2), F("div", fxe, [F("div", pxe, [F("span", mxe, kt(x.title) + kt(x.repeated > 0 ? ` · Repeated ${x.repeated} times` : ""), 1), F("span", _xe, kt(x.timestampReceived.toLocaleTimeString()), 1)]), F("div", vxe, [Gi(kt(x.message) + " ", 1), x.code ? (J(), he("div", bxe, [F("code", null, kt(x.code), 1)])) : Te("", !0)])])]))), 128))])) : Te("", !0)])], 2))
         }
     });
-const Cxe = Li(bxe, [
+const wxe = Li(Cxe, [
         ["__scopeId", "data-v-caebba71"]
     ]),
-    wxe = o => (Nn("data-v-cb9a267f"), o = o(), Rn(), o),
-    Sxe = {
+    Sxe = o => (Nn("data-v-cb9a267f"), o = o(), Rn(), o),
+    yxe = {
         class: "BuilderSidebarToolbar"
     },
-    yxe = wxe(() => F("div", {
+    Lxe = Sxe(() => F("div", {
         class: "sectionTitle"
     }, [F("i", {
         class: "ri-tools-line ri-xl"
     }), F("h3", null, "Toolkit")], -1)),
-    Lxe = {
+    xxe = {
         class: "categories"
     },
-    xxe = {
+    Dxe = {
         key: 0,
         class: "category"
     },
-    Dxe = {
+    kxe = {
         class: "title"
     },
-    kxe = ["onClick"],
-    Ixe = {
+    Ixe = ["onClick"],
+    Exe = {
         class: "components"
     },
-    Exe = ["title", "data-component-type", "onDragstart"],
-    Txe = {
+    Txe = ["title", "data-component-type", "onDragstart"],
+    Nxe = {
         key: 0,
         class: "ri-collage-line ri-lg",
         title: "(Custom component template)"
     },
-    Nxe = Pi({
+    Rxe = Pi({
         __name: "BuilderSidebarToolbar",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 {
                     removeInsertionCandidacy: i
                 } = h2(e),
@@ -109037,73 +109039,73 @@
                 }),
                 a = (d, c) => {
                     t.setSelection(null), d.dataTransfer.setData(`application/json;streamsync=${c},`, "{}")
                 },
                 l = d => {
                     i(d)
                 };
-            return (d, c) => (J(), he("div", Sxe, [yxe, F("div", Lxe, [(J(!0), he(hi, null, Hn(n.value, (h, u) => (J(), he(hi, {
+            return (d, c) => (J(), he("div", yxe, [Lxe, F("div", xxe, [(J(!0), he(hi, null, Hn(n.value, (h, u) => (J(), he(hi, {
                 key: u
-            }, [h.isVisible !== !1 ? (J(), he("div", xxe, [F("div", Dxe, [F("i", {
+            }, [h.isVisible !== !1 ? (J(), he("div", Dxe, [F("div", kxe, [F("i", {
                 class: xt(h.icon ?? "ri-question-line")
             }, null, 2), F("h4", null, kt(u), 1), F("div", {
                 class: "drop-arrow",
                 onClick: g => s(u)
             }, [F("i", {
                 class: xt(["ri-xl", h.isCollapsed ? "ri-arrow-drop-down-line" : "ri-arrow-drop-up-line"])
-            }, null, 2)], 8, kxe)]), Un(F("div", Ixe, [(J(!0), he(hi, null, Hn(r.value[u], (g, f) => (J(), he("div", {
+            }, null, 2)], 8, Ixe)]), Un(F("div", Exe, [(J(!0), he(hi, null, Hn(r.value[u], (g, f) => (J(), he("div", {
                 key: f,
                 class: "component button",
                 title: g.description,
                 draggable: "true",
                 "data-component-type": f,
                 onDragend: c[0] || (c[0] = m => l(m)),
                 onDragstart: m => a(m, f)
-            }, [Gi(kt(g.name ?? f) + " ", 1), f.startsWith("custom_") ? (J(), he("i", Txe)) : Te("", !0)], 40, Exe))), 128))], 512), [
+            }, [Gi(kt(g.name ?? f) + " ", 1), f.startsWith("custom_") ? (J(), he("i", Nxe)) : Te("", !0)], 40, Txe))), 128))], 512), [
                 [ga, !h.isCollapsed]
             ])])) : Te("", !0)], 64))), 128))])]))
         }
     });
-const Rxe = Li(Nxe, [
+const Mxe = Li(Rxe, [
         ["__scopeId", "data-v-cb9a267f"]
     ]),
     OA = o => (Nn("data-v-d2a3534e"), o = o(), Rn(), o),
-    Mxe = {
+    Axe = {
         class: "BuilderTreeBranch"
     },
-    Axe = ["title", "data-branch-component-id", "draggable"],
-    Pxe = {
+    Pxe = ["title", "data-branch-component-id", "draggable"],
+    Oxe = {
         key: 0,
         class: "ri-arrow-drop-up-line ri-lg"
     },
-    Oxe = {
+    Fxe = {
         key: 1,
         class: "ri-arrow-drop-down-line ri-lg"
     },
-    Fxe = {
+    Bxe = {
         class: "type"
     },
-    Bxe = OA(() => F("i", {
+    Wxe = OA(() => F("i", {
         class: "ri-flashlight-line ri-lg"
     }, null, -1)),
-    Wxe = OA(() => F("i", {
+    Vxe = OA(() => F("i", {
         class: "ri-eye-off-line ri-lg"
     }, null, -1)),
-    Vxe = OA(() => F("i", {
+    Hxe = OA(() => F("i", {
         class: "ri-terminal-box-line ri-lg"
     }, null, -1)),
-    Hxe = {
+    zxe = {
         key: 4,
         class: "preview"
     },
-    zxe = {
+    $xe = {
         key: 0,
         class: "children"
     },
-    $xe = Pi({
+    Uxe = Pi({
         __name: "BuilderTreeBranch",
         props: {
             componentId: {},
             matchingComponents: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -109227,15 +109229,15 @@
                     } = pe;
                     Se ? n(Se, f.value.id) : i(Le, f.value.id), l(ne)
                 };
             return Ia(() => {
                 M.value && B()
             }), (ne, pe) => {
                 const Le = i9("BuilderTreeBranch", !0);
-                return J(), he("div", Mxe, [F("div", {
+                return J(), he("div", Axe, [F("div", {
                     ref_key: "rootEl",
                     ref: _,
                     class: xt(["main", {
                         selected: M.value,
                         childless: C.value,
                         matching: w.value
                     }]),
@@ -109249,21 +109251,21 @@
                     onDragstart: q,
                     onDragend: X,
                     onDrop: Re
                 }, [C.value ? Te("", !0) : (J(), he("div", {
                     key: 0,
                     class: "toggleChildren",
                     onClick: L
-                }, [x.value ? (J(), he("i", Pxe)) : Te("", !0), x.value ? Te("", !0) : (J(), he("i", Oxe))])), F("span", Fxe, kt(b.value), 1), Object.keys(f.value.handlers ?? {}).length > 0 ? (J(), he(hi, {
+                }, [x.value ? (J(), he("i", Oxe)) : Te("", !0), x.value ? Te("", !0) : (J(), he("i", Fxe))])), F("span", Bxe, kt(b.value), 1), Object.keys(f.value.handlers ?? {}).length > 0 ? (J(), he(hi, {
                     key: 1
-                }, [Gi("  · "), Bxe], 64)) : Te("", !0), _e(c)(f.value.id) ? Te("", !0) : (J(), he(hi, {
+                }, [Gi("  · "), Wxe], 64)) : Te("", !0), _e(c)(f.value.id) ? Te("", !0) : (J(), he(hi, {
                     key: 2
-                }, [Gi("  · "), Wxe], 64)), f.value.isCodeManaged ? (J(), he(hi, {
+                }, [Gi("  · "), Vxe], 64)), f.value.isCodeManaged ? (J(), he(hi, {
                     key: 3
-                }, [Gi("  · "), Vxe], 64)) : Te("", !0), S.value ? (J(), he("span", Hxe, "  · " + kt(S.value), 1)) : Te("", !0)], 42, Axe), x.value && !C.value ? (J(), he("div", zxe, [(J(!0), he(hi, null, Hn(y.value.filter(Se => !Se.isCodeManaged), Se => (J(), he("div", {
+                }, [Gi("  · "), Hxe], 64)) : Te("", !0), S.value ? (J(), he("span", zxe, "  · " + kt(S.value), 1)) : Te("", !0)], 42, Pxe), x.value && !C.value ? (J(), he("div", $xe, [(J(!0), he(hi, null, Hn(y.value.filter(Se => !Se.isCodeManaged), Se => (J(), he("div", {
                     key: Se.id,
                     class: "child"
                 }, [on(Le, {
                     "component-id": Se.id,
                     "matching-components": _e(g)
                 }, null, 8, ["component-id", "matching-components"])]))), 128)), (J(!0), he(hi, null, Hn(y.value.filter(Se => Se.isCodeManaged), Se => (J(), he("div", {
                     key: Se.id,
@@ -109271,43 +109273,43 @@
                 }, [on(Le, {
                     "component-id": Se.id,
                     "matching-components": _e(g)
                 }, null, 8, ["component-id", "matching-components"])]))), 128))])) : Te("", !0)])
             }
         }
     });
-const Uxe = Li($xe, [
+const jxe = Li(Uxe, [
         ["__scopeId", "data-v-d2a3534e"]
     ]),
     FA = o => (Nn("data-v-b4d7d19e"), o = o(), Rn(), o),
-    jxe = {
+    Kxe = {
         class: "BuilderSidebarTree"
     },
-    Kxe = {
+    qxe = {
         key: 0,
         class: "sectionTitle"
     },
-    qxe = FA(() => F("i", {
+    Gxe = FA(() => F("i", {
         class: "ri-node-tree ri-xl"
     }, null, -1)),
-    Gxe = FA(() => F("h3", null, "Component Tree", -1)),
-    Zxe = {
+    Zxe = FA(() => F("h3", null, "Component Tree", -1)),
+    Yxe = {
         key: 1,
         class: "sectionTitle"
     },
-    Yxe = ["title"],
     Xxe = ["title"],
-    Qxe = {
+    Qxe = ["title"],
+    Jxe = {
         ref: "componentTree",
         class: "components"
     },
-    Jxe = FA(() => F("i", {
+    eDe = FA(() => F("i", {
         class: "ri-add-line"
     }, null, -1)),
-    eDe = Pi({
+    tDe = Pi({
         __name: "BuilderSidebarTree",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 {
                     createAndInsertComponent: i,
                     goToComponentParentPage: n
@@ -109368,126 +109370,126 @@
                 var w;
                 return ((w = v.value) == null ? void 0 : w.length) > 0
             });
             async function C() {
                 const w = i("page", "root");
                 e.setActivePageId(w), await co(), t.setSelection(w)
             }
-            return (w, S) => (J(), he("div", jxe, [r.value ? Te("", !0) : (J(), he("div", Kxe, [qxe, Gxe, F("i", {
+            return (w, S) => (J(), he("div", Kxe, [r.value ? Te("", !0) : (J(), he("div", qxe, [Gxe, Zxe, F("i", {
                 class: "ri-search-line ri-xl searchIcon",
                 title: "Search",
                 onClick: c
-            })])), r.value ? (J(), he("div", Zxe, [Un(F("input", {
+            })])), r.value ? (J(), he("div", Yxe, [Un(F("input", {
                 ref_key: "searchInput",
                 ref: s,
                 "onUpdate:modelValue": S[0] || (S[0] = k => a.value = k),
                 type: "text",
                 placeholder: "Search..."
             }, null, 512), [
                 [B1, a.value]
             ]), F("i", {
                 class: xt(["ri-arrow-left-s-line ri-xl searchIcon", {
                     disabled: !b.value
                 }]),
                 title: b.value ? `Go to match ${g.value+1} of ${v.value.length}` : "Previous match",
                 onClick: m
-            }, null, 10, Yxe), F("i", {
+            }, null, 10, Xxe), F("i", {
                 class: xt(["ri-arrow-right-s-line ri-xl searchIcon", {
                     disabled: !b.value
                 }]),
                 title: b.value ? `Go to match ${f.value+1} of ${v.value.length}` : "Next match",
                 onClick: _
-            }, null, 10, Xxe), F("i", {
+            }, null, 10, Qxe), F("i", {
                 class: "ri-close-line ri-xl searchIcon",
                 title: "Close",
                 onClick: c
-            })])) : Te("", !0), F("div", Qxe, [(J(!0), he(hi, null, Hn(d.value, k => (J(), he("div", {
+            })])) : Te("", !0), F("div", Jxe, [(J(!0), he(hi, null, Hn(d.value, k => (J(), he("div", {
                 key: k.id,
                 class: "selector"
-            }, [on(Uxe, {
+            }, [on(jxe, {
                 "component-id": k.id,
                 "matching-components": v.value
             }, null, 8, ["component-id", "matching-components"])]))), 128))], 512), F("div", {
                 class: "addPage"
             }, [F("button", {
                 onClick: C
-            }, [Jxe, Gi("Add Page ")])])]))
+            }, [eDe, Gi("Add Page ")])])]))
         }
     });
-const tDe = Li(eDe, [
+const iDe = Li(tDe, [
         ["__scopeId", "data-v-b4d7d19e"]
     ]),
-    iDe = {
+    nDe = {
         class: "BuilderSidebar"
     },
-    nDe = Pi({
+    sDe = Pi({
         __name: "BuilderSidebar",
         setup(o) {
-            return (e, t) => (J(), he("div", iDe, [on(Rxe, {
+            return (e, t) => (J(), he("div", nDe, [on(Mxe, {
                 class: "toolbar"
-            }), on(tDe, {
+            }), on(iDe, {
                 class: "tree"
             })]))
         }
     });
-const sDe = Li(nDe, [
+const oDe = Li(sDe, [
         ["__scopeId", "data-v-e1a5c7b9"]
     ]),
     Mh = o => (Nn("data-v-973b5178"), o = o(), Rn(), o),
-    oDe = ["draggable", "data-streamsync-id"],
-    rDe = {
+    rDe = ["draggable", "data-streamsync-id"],
+    aDe = {
         class: "type"
     },
-    aDe = Mh(() => F("i", {
+    lDe = Mh(() => F("i", {
         class: "ri-add-line"
     }, null, -1)),
-    lDe = [aDe],
-    dDe = ["title"],
-    cDe = Mh(() => F("i", {
+    dDe = [lDe],
+    cDe = ["title"],
+    hDe = Mh(() => F("i", {
         class: "ri-arrow-up-line"
     }, null, -1)),
-    hDe = [cDe],
-    uDe = ["title"],
-    gDe = Mh(() => F("i", {
+    uDe = [hDe],
+    gDe = ["title"],
+    fDe = Mh(() => F("i", {
         class: "ri-arrow-down-line"
     }, null, -1)),
-    fDe = [gDe],
-    pDe = ["title"],
-    mDe = Mh(() => F("i", {
+    pDe = [fDe],
+    mDe = ["title"],
+    _De = Mh(() => F("i", {
         class: "ri-scissors-line"
     }, null, -1)),
-    _De = [mDe],
-    vDe = ["title"],
-    bDe = Mh(() => F("i", {
+    vDe = [_De],
+    bDe = ["title"],
+    CDe = Mh(() => F("i", {
         class: "ri-file-copy-line"
     }, null, -1)),
-    CDe = [bDe],
-    wDe = ["title"],
-    SDe = Mh(() => F("i", {
+    wDe = [CDe],
+    SDe = ["title"],
+    yDe = Mh(() => F("i", {
         class: "ri-clipboard-line"
     }, null, -1)),
-    yDe = [SDe],
-    LDe = ["title"],
-    xDe = Mh(() => F("i", {
+    LDe = [yDe],
+    xDe = ["title"],
+    DDe = Mh(() => F("i", {
         class: "ri-parent-line"
     }, null, -1)),
-    DDe = [xDe],
-    kDe = Mh(() => F("i", {
+    kDe = [DDe],
+    IDe = Mh(() => F("i", {
         class: "ri-delete-bin-line"
     }, null, -1)),
-    IDe = [kDe],
-    EDe = {
+    EDe = [IDe],
+    TDe = {
         key: 1,
         class: "addDialog"
     },
-    TDe = {
+    NDe = {
         id: "validChildrenTypes"
     },
-    NDe = ["value"],
-    RDe = Pi({
+    RDe = ["value"],
+    MDe = Pi({
         __name: "BuilderComponentShortcuts",
         props: {
             componentId: {},
             instancePath: {}
         },
         setup(o) {
             const e = Pt(Ot.core),
@@ -109569,107 +109571,107 @@
             }), (M, B) => {
                 var q, X, ye, Re, ne, pe, Le, Se, $, K;
                 return y.value ? (J(), he("div", {
                     key: 0,
                     draggable: (q = y.value) == null ? void 0 : q.isDraggable,
                     class: "BuilderComponentShortcuts",
                     "data-streamsync-id": _e(w)
-                }, [F("div", rDe, kt((X = y.value) == null ? void 0 : X.componentTypeName), 1), k.value ? Te("", !0) : (J(), he(hi, {
+                }, [F("div", aDe, kt((X = y.value) == null ? void 0 : X.componentTypeName), 1), k.value ? Te("", !0) : (J(), he(hi, {
                     key: 0
                 }, [F("div", {
                     class: xt(["actionButton", {
                         enabled: (ye = y.value) == null ? void 0 : ye.isAddEnabled
                     }]),
                     title: "Add child",
                     onClick: B[0] || (B[0] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isAddEnabled ? k.value = !k.value : void 0
                     })
-                }, lDe, 2), F("div", {
+                }, dDe, 2), F("div", {
                     class: xt(["actionButton", {
                         enabled: (Re = y.value) == null ? void 0 : Re.isMoveUpEnabled
                     }]),
                     title: `Move up (${_e(T)}+↑)`,
                     onClick: B[1] || (B[1] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isMoveUpEnabled ? _e(n)(_e(w)) : void 0
                     })
-                }, hDe, 10, dDe), F("div", {
+                }, uDe, 10, cDe), F("div", {
                     class: xt(["actionButton", {
                         enabled: (ne = y.value) == null ? void 0 : ne.isMoveDownEnabled
                     }]),
                     title: `Move down (${_e(T)}+↓)`,
                     onClick: B[2] || (B[2] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isMoveDownEnabled ? _e(s)(_e(w)) : void 0
                     })
-                }, fDe, 10, uDe), F("div", {
+                }, pDe, 10, gDe), F("div", {
                     class: xt(["actionButton", {
                         enabled: (pe = y.value) == null ? void 0 : pe.isCutEnabled
                     }]),
                     title: `Cut (${_e(T)}+X)`,
                     onClick: B[3] || (B[3] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isCutEnabled ? _e(r)(_e(w)) : void 0
                     })
-                }, _De, 10, pDe), F("div", {
+                }, vDe, 10, mDe), F("div", {
                     class: xt(["actionButton", {
                         enabled: (Le = y.value) == null ? void 0 : Le.isCopyEnabled
                     }]),
                     title: `Copy (${_e(T)}+C)`,
                     onClick: B[4] || (B[4] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isCopyEnabled ? _e(l)(_e(w)) : void 0
                     })
-                }, CDe, 10, vDe), F("div", {
+                }, wDe, 10, bDe), F("div", {
                     class: xt(["actionButton", {
                         enabled: (Se = y.value) == null ? void 0 : Se.isPasteEnabled
                     }]),
                     title: `Paste (${_e(T)}+V)`,
                     onClick: B[5] || (B[5] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isPasteEnabled ? _e(a)(_e(w)) : void 0
                     })
-                }, yDe, 10, wDe), F("div", {
+                }, LDe, 10, SDe), F("div", {
                     class: xt(["actionButton", {
                         enabled: ($ = y.value) == null ? void 0 : $.isGoToParentEnabled
                     }]),
                     title: `Go to parent (${_e(T)}+Shift+↑)`,
                     onClick: B[6] || (B[6] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isGoToParentEnabled ? _e(b)(_e(w), _e(S)) : void 0
                     })
-                }, DDe, 10, LDe), F("div", {
+                }, kDe, 10, xDe), F("div", {
                     class: xt(["actionButton delete", {
                         enabled: (K = y.value) == null ? void 0 : K.isDeleteEnabled
                     }]),
                     "data-automation-action": "delete",
                     title: "Delete (Del)",
                     onClick: B[7] || (B[7] = se => {
                         var fe;
                         return (fe = y.value) != null && fe.isDeleteEnabled ? _e(v)(_e(w)) : void 0
                     })
-                }, IDe, 2)], 64)), k.value ? (J(), he("div", EDe, [F("input", {
+                }, EDe, 2)], 64)), k.value ? (J(), he("div", TDe, [F("input", {
                     type: "text",
                     list: "validChildrenTypes",
                     placeholder: "Component...",
                     onChange: L
-                }, null, 32), F("datalist", TDe, [(J(!0), he(hi, null, Hn(x.value, (se, fe) => (J(), he("option", {
+                }, null, 32), F("datalist", NDe, [(J(!0), he(hi, null, Hn(x.value, (se, fe) => (J(), he("option", {
                     key: fe,
                     value: se.name
-                }, kt(se.name), 9, NDe))), 128))])])) : Te("", !0)], 8, oDe)) : Te("", !0)
+                }, kt(se.name), 9, RDe))), 128))])])) : Te("", !0)], 8, rDe)) : Te("", !0)
             }
         }
     });
-const MDe = Li(RDe, [
+const ADe = Li(MDe, [
         ["__scopeId", "data-v-973b5178"]
     ]),
-    ADe = 200,
-    PDe = 36,
-    ODe = Pi({
+    PDe = 200,
+    ODe = 36,
+    FDe = Pi({
         __name: "BuilderInstanceTracker",
         props: {
             instancePath: {},
             matchSize: {
                 type: Boolean
             },
             verticalOffsetPixels: {},
@@ -109721,15 +109723,15 @@
                         } = (w == null ? void 0 : w.getBoundingClientRect()) || {
                             left: 1 / 0
                         };
                     let {
                         clientHeight: E,
                         clientWidth: T
                     } = i != null && i.value ? g : d.value, M = n != null && n.value ? n.value : 0, B = _, q = m + M;
-                    if (s.value || (B = Math.max(C, B), B = Math.min(C + b - T, B), q = Math.max(PDe, q), q = Math.min(v - E, q)), r.value) {
+                    if (s.value || (B = Math.max(C, B), B = Math.min(C + b - T, B), q = Math.max(ODe, q), q = Math.min(v - E, q)), r.value) {
                         let X = 0;
                         if (L < C + b) {
                             const ye = B + T,
                                 Re = C + b,
                                 ne = Math.max(Re - ye, 0);
                             X = Math.max(x - ne, 0)
                         }
@@ -109745,104 +109747,104 @@
                 h = () => {
                     let g = document.querySelector(`.ComponentRenderer [data-streamsync-instance-path="${t.value}"]`);
                     if (u(), !g) return;
                     const f = getComputedStyle(g);
                     f && (f.display == "contents" && (g = g.querySelector("[data-streamsync-id]")), g && c(g))
                 },
                 u = () => {
-                    l.value = setTimeout(h, ADe)
+                    l.value = setTimeout(h, PDe)
                 };
             return Ia(async () => {
                 await co(), h()
             }), n9(() => {
                 clearTimeout(l.value)
             }), (g, f) => (J(), he("div", {
                 ref_key: "rootEl",
                 ref: d,
                 class: "BuilderInstanceTracker",
                 style: s9(a.value)
             }, [c2(g.$slots, "default", {}, void 0, !0)], 4))
         }
     });
-const mk = Li(ODe, [
+const mk = Li(FDe, [
         ["__scopeId", "data-v-0704f28a"]
     ]),
-    FDe = o => (Nn("data-v-0c332d4f"), o = o(), Rn(), o),
-    BDe = {
+    BDe = o => (Nn("data-v-0c332d4f"), o = o(), Rn(), o),
+    WDe = {
         class: "BuilderInsertionOverlay"
     },
-    WDe = FDe(() => F("div", {
+    VDe = BDe(() => F("div", {
         class: "overlay"
     }, null, -1)),
-    VDe = {
+    HDe = {
         class: "progressBar"
     },
-    HDe = Pi({
+    zDe = Pi({
         __name: "BuilderInsertionOverlay",
         setup(o) {
             const e = Ue(() => ({
                 "animation-duration": `${t9}ms`
             }));
-            return (t, i) => (J(), he("div", BDe, [WDe, F("div", VDe, [F("div", {
+            return (t, i) => (J(), he("div", WDe, [VDe, F("div", HDe, [F("div", {
                 class: "elapsed",
                 style: s9(e.value)
             }, null, 4)])]))
         }
     });
-const zDe = Li(HDe, [
+const $De = Li(zDe, [
     ["__scopeId", "data-v-0c332d4f"]
 ]);
-const $De = {},
-    UDe = {
+const UDe = {},
+    jDe = {
         class: "BuilderInsertionLabel"
     };
 
-function jDe(o, e) {
-    return J(), he("div", UDe, [c2(o.$slots, "default", {}, void 0, !0)])
+function KDe(o, e) {
+    return J(), he("div", jDe, [c2(o.$slots, "default", {}, void 0, !0)])
 }
-const KDe = Li($De, [
-        ["render", jDe],
+const qDe = Li(UDe, [
+        ["render", KDe],
         ["__scopeId", "data-v-9cd536ed"]
     ]),
-    qDe = o => (Nn("data-v-c5323e29"), o = o(), Rn(), o),
-    GDe = {
+    GDe = o => (Nn("data-v-c5323e29"), o = o(), Rn(), o),
+    ZDe = {
         class: "BuilderApp",
         tabindex: "-1"
     },
-    ZDe = {
+    YDe = {
         class: "mainGrid"
     },
-    YDe = {
+    XDe = {
         key: 0,
         class: "sidebar"
     },
-    XDe = {
+    QDe = {
         class: "rendererWrapper"
     },
-    QDe = {
+    JDe = {
         class: "floatingContainer"
     },
-    JDe = {
+    eke = {
         class: "floatingSticky"
     },
-    eke = {
+    tke = {
         key: 0,
         class: "ri-settings-3-line ri-lg"
     },
-    tke = {
+    ike = {
         key: 1,
         class: "ri-arrow-drop-right-line ri-lg"
     },
-    ike = {
+    nke = {
         class: "codeBar"
     },
-    nke = qDe(() => F("div", {
+    ske = GDe(() => F("div", {
         id: "modal"
     }, null, -1)),
-    ske = Pi({
+    oke = Pi({
         __name: "BuilderApp",
         setup(o) {
             const e = Pt(Ot.core),
                 t = Pt(Ot.builderManager),
                 {
                     candidateId: i,
                     candidateInstancePath: n,
@@ -109969,88 +109971,88 @@
                     ne.dataTransfer.setData(`application/json;streamsync=${Se},${Le}`, "{}")
                 },
                 Re = ne => {
                     t.setSelection(null), l(ne)
                 };
             return Ia(() => {
                 document.addEventListener("keydown", ne => M(ne))
-            }), (ne, pe) => (J(), he("div", GDe, [F("div", ZDe, [on(q$, {
+            }), (ne, pe) => (J(), he("div", ZDe, [F("div", YDe, [on(q$, {
                 class: "builderHeader"
-            }), L.value !== "preview" ? (J(), he("div", YDe, [on(sDe)])) : Te("", !0), F("div", {
+            }), L.value !== "preview" ? (J(), he("div", XDe, [on(oDe)])) : Te("", !0), F("div", {
                 class: xt(["builderMain", {
                     buildMode: L.value !== "preview",
                     previewMode: L.value === "preview"
                 }])
-            }, [F("div", XDe, [on(Zz, {
+            }, [F("div", QDe, [on(Zz, {
                 class: xt(["componentRenderer", {
                     settingsOpen: _e(t).isSelectionActive() && !_e(t).isSettingsBarCollapsed()
                 }]),
                 onDragover: B,
                 onDragstart: ye,
                 onDragend: Re,
                 onDrop: q,
                 onClickCapture: X
-            }, null, 8, ["class"])]), F("div", QDe, [F("div", JDe, [_e(t).isSelectionActive() ? (J(), he("div", {
+            }, null, 8, ["class"])]), F("div", JDe, [F("div", eke, [_e(t).isSelectionActive() ? (J(), he("div", {
                 key: 0,
                 class: "settingsHiderTab",
                 onClick: pe[0] || (pe[0] = Le => _e(t).setSettingsBarCollapsed(!_e(t).isSettingsBarCollapsed()))
-            }, [_e(t).isSettingsBarCollapsed() ? (J(), he("i", eke)) : Te("", !0), _e(t).isSettingsBarCollapsed() ? Te("", !0) : (J(), he("i", tke))])) : Te("", !0), _e(t).isSelectionActive() ? (J(), he("div", {
+            }, [_e(t).isSettingsBarCollapsed() ? (J(), he("i", tke)) : Te("", !0), _e(t).isSettingsBarCollapsed() ? Te("", !0) : (J(), he("i", ike))])) : Te("", !0), _e(t).isSelectionActive() ? (J(), he("div", {
                 key: E.value ?? "noneSelected",
                 class: xt(["settingsBar", {
                     collapsed: _e(t).isSettingsBarCollapsed()
                 }])
-            }, [on(ALe)], 2)) : Te("", !0), Un(F("div", ike, [on(Cxe)], 512), [
+            }, [on(PLe)], 2)) : Te("", !0), Un(F("div", nke, [on(wxe)], 512), [
                 [ga, L.value == "code"]
             ])])])], 2)]), L.value !== "preview" ? (J(), he(hi, {
                 key: 0
             }, [_e(t).isSelectionActive() ? (J(), Fn(mk, {
                 key: T.value,
                 class: "shortcutsTracker",
                 "prevent-settings-bar-overlap": !0,
                 "instance-path": T.value,
                 "vertical-offset-pixels": -48,
                 "data-streamsync-cage": "",
                 onDragstart: ye,
                 onDragend: Re
             }, {
-                default: hu(() => [on(MDe, {
+                default: hu(() => [on(ADe, {
                     "component-id": E.value,
                     "instance-path": T.value
                 }, null, 8, ["component-id", "instance-path"])]),
                 _: 1
             }, 8, ["instance-path"])) : Te("", !0), _e(i) && !_e(s) ? (J(), he(hi, {
                 key: 1
             }, [(J(), Fn(mk, {
                 key: _e(n),
                 class: "insertionOverlayTracker",
                 "is-off-bounds-allowed": !0,
                 "instance-path": _e(n),
                 "match-size": !0
             }, {
-                default: hu(() => [on(zDe)]),
+                default: hu(() => [on($De)]),
                 _: 1
             }, 8, ["instance-path"])), (J(), Fn(mk, {
                 key: _e(n),
                 class: "insertionLabelTracker",
                 "instance-path": _e(n),
                 "vertical-offset-pixels": -48
             }, {
-                default: hu(() => [on(KDe, null, {
+                default: hu(() => [on(qDe, null, {
                     default: hu(() => [Gi(kt(_e(e).getComponentDefinition(_e(e).getComponentById(_e(i)).type).name), 1)]),
                     _: 1
                 })]),
                 _: 1
-            }, 8, ["instance-path"]))], 64)) : Te("", !0)], 64)) : Te("", !0), nke]))
+            }, 8, ["instance-path"]))], 64)) : Te("", !0)], 64)) : Te("", !0), ske]))
         }
     });
-const oke = Li(ske, [
+const rke = Li(oke, [
         ["__scopeId", "data-v-c5323e29"]
     ]),
-    hTe = Object.freeze(Object.defineProperty({
+    uTe = Object.freeze(Object.defineProperty({
         __proto__: null,
-        default: oke
+        default: rke
     }, Symbol.toStringTag, {
         value: "Module"
     }));
 export {
-    hTe as B, p0 as m, RW as t
+    uTe as B, p0 as m, RW as t
 };
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/BuilderApp-9cf67088.css` & `streamsync-0.4.0rc4/src/streamsync/static/assets/BuilderApp-f68489e4.css`

 * *Files 1% similar despite different names*

```diff
@@ -9807,15 +9807,15 @@
 000264e0: 7465 722d 5265 6775 6c61 722d 6436 3132  ter-Regular-d612
 000264f0: 6631 3231 2e77 6f66 6632 2920 666f 726d  f121.woff2) form
 00026500: 6174 2822 776f 6666 3222 292c 7572 6c28  at("woff2"),url(
 00026510: 2e2f 496e 7465 722d 5265 6775 6c61 722d  ./Inter-Regular-
 00026520: 3431 6162 3066 3730 2e74 7466 2920 666f  41ab0f70.ttf) fo
 00026530: 726d 6174 2822 7472 7565 7479 7065 2229  rmat("truetype")
 00026540: 7d2e 4275 696c 6465 7241 7070 5b64 6174  }.BuilderApp[dat
-00026550: 612d 762d 3065 6633 6238 3263 5d7b 2d2d  a-v-0ef3b82c]{--
+00026550: 612d 762d 3736 3732 3134 3065 5d7b 2d2d  a-v-7672140e]{--
 00026560: 6275 696c 6465 7242 6163 6b67 726f 756e  builderBackgroun
 00026570: 6443 6f6c 6f72 3a20 2366 6666 6666 663b  dColor: #ffffff;
 00026580: 2d2d 6275 696c 6465 7241 6363 656e 7443  --builderAccentC
 00026590: 6f6c 6f72 3a20 2332 3963 6630 303b 2d2d  olor: #29cf00;--
 000265a0: 6275 696c 6465 7253 7563 6365 7373 436f  builderSuccessCo
 000265b0: 6c6f 723a 2023 3239 6366 3030 3b2d 2d62  lor: #29cf00;--b
 000265c0: 7569 6c64 6572 4572 726f 7243 6f6c 6f72  uilderErrorColor
@@ -9861,136 +9861,136 @@
 00026840: 6178 2832 3635 7078 2c20 3237 7668 293b  ax(265px, 27vh);
 00026850: 2d2d 6275 696c 6465 7253 6574 7469 6e67  --builderSetting
 00026860: 7357 6964 7468 3a20 6d61 7828 3236 3570  sWidth: max(265p
 00026870: 782c 2032 3776 6829 3b2d 2d62 7569 6c64  x, 27vh);--build
 00026880: 6572 4163 7469 6f6e 4f6e 676f 696e 6743  erActionOngoingC
 00026890: 6f6c 6f72 3a20 7267 6261 2830 2c20 302c  olor: rgba(0, 0,
 000268a0: 2030 2c20 2e37 297d 6831 5b64 6174 612d   0, .7)}h1[data-
-000268b0: 762d 3065 6633 6238 3263 5d2c 6832 5b64  v-0ef3b82c],h2[d
-000268c0: 6174 612d 762d 3065 6633 6238 3263 5d2c  ata-v-0ef3b82c],
-000268d0: 6833 5b64 6174 612d 762d 3065 6633 6238  h3[data-v-0ef3b8
-000268e0: 3263 5d7b 666f 6e74 2d77 6569 6768 743a  2c]{font-weight:
+000268b0: 762d 3736 3732 3134 3065 5d2c 6832 5b64  v-7672140e],h2[d
+000268c0: 6174 612d 762d 3736 3732 3134 3065 5d2c  ata-v-7672140e],
+000268d0: 6833 5b64 6174 612d 762d 3736 3732 3134  h3[data-v-767214
+000268e0: 3065 5d7b 666f 6e74 2d77 6569 6768 743a  0e]{font-weight:
 000268f0: 3330 303b 6d61 7267 696e 3a30 7d68 315b  300;margin:0}h1[
-00026900: 6461 7461 2d76 2d30 6566 3362 3832 635d  data-v-0ef3b82c]
+00026900: 6461 7461 2d76 2d37 3637 3231 3430 655d  data-v-7672140e]
 00026910: 7b66 6f6e 742d 7369 7a65 3a31 2e33 7265  {font-size:1.3re
-00026920: 6d7d 6832 5b64 6174 612d 762d 3065 6633  m}h2[data-v-0ef3
-00026930: 6238 3263 5d7b 666f 6e74 2d73 697a 653a  b82c]{font-size:
-00026940: 3172 656d 7d68 335b 6461 7461 2d76 2d30  1rem}h3[data-v-0
-00026950: 6566 3362 3832 635d 7b66 6f6e 742d 7369  ef3b82c]{font-si
+00026920: 6d7d 6832 5b64 6174 612d 762d 3736 3732  m}h2[data-v-7672
+00026930: 3134 3065 5d7b 666f 6e74 2d73 697a 653a  140e]{font-size:
+00026940: 3172 656d 7d68 335b 6461 7461 2d76 2d37  1rem}h3[data-v-7
+00026950: 3637 3231 3430 655d 7b66 6f6e 742d 7369  672140e]{font-si
 00026960: 7a65 3a2e 3872 656d 7d68 345b 6461 7461  ze:.8rem}h4[data
-00026970: 2d76 2d30 6566 3362 3832 635d 7b74 6578  -v-0ef3b82c]{tex
+00026970: 2d76 2d37 3637 3231 3430 655d 7b74 6578  -v-7672140e]{tex
 00026980: 742d 7472 616e 7366 6f72 6d3a 7570 7065  t-transform:uppe
 00026990: 7263 6173 653b 666f 6e74 2d77 6569 6768  rcase;font-weigh
 000269a0: 743a 3730 303b 666f 6e74 2d73 697a 653a  t:700;font-size:
 000269b0: 2e36 3572 656d 3b6c 6574 7465 722d 7370  .65rem;letter-sp
 000269c0: 6163 696e 673a 2e32 6368 7d2e 696e 7365  acing:.2ch}.inse
 000269d0: 7274 696f 6e4f 7665 726c 6179 5b64 6174  rtionOverlay[dat
-000269e0: 612d 762d 3065 6633 6238 3263 5d7b 6261  a-v-0ef3b82c]{ba
+000269e0: 612d 762d 3736 3732 3134 3065 5d7b 6261  a-v-7672140e]{ba
 000269f0: 636b 6772 6f75 6e64 3a72 6762 6128 3231  ckground:rgba(21
 00026a00: 302c 3233 342c 3234 342c 2e35 293b 706f  0,234,244,.5);po
 00026a10: 696e 7465 722d 6576 656e 7473 3a6e 6f6e  inter-events:non
 00026a20: 653b 706f 7369 7469 6f6e 3a61 6273 6f6c  e;position:absol
 00026a30: 7574 653b 746f 703a 303b 6c65 6674 3a30  ute;top:0;left:0
 00026a40: 3b6d 6178 2d68 6569 6768 743a 3130 3025  ;max-height:100%
 00026a50: 3b6d 6178 2d77 6964 7468 3a31 3030 257d  ;max-width:100%}
 00026a60: 2e69 6e73 6572 7469 6f6e 4f76 6572 6c61  .insertionOverla
 00026a70: 7920 2e6c 6162 656c 5b64 6174 612d 762d  y .label[data-v-
-00026a80: 3065 6633 6238 3263 5d7b 626f 7264 6572  0ef3b82c]{border
+00026a80: 3736 3732 3134 3065 5d7b 626f 7264 6572  7672140e]{border
 00026a90: 2d72 6164 6975 733a 3136 7078 3b62 6f78  -radius:16px;box
 00026aa0: 2d73 6861 646f 773a 3020 3020 3870 7820  -shadow:0 0 8px 
 00026ab0: 2d31 7078 2023 3030 3036 3b70 6f73 6974  -1px #0006;posit
 00026ac0: 696f 6e3a 6162 736f 6c75 7465 3b72 6967  ion:absolute;rig
 00026ad0: 6874 3a30 3b68 6569 6768 743a 3234 7078  ht:0;height:24px
 00026ae0: 3b70 6164 6469 6e67 3a34 7078 2031 3670  ;padding:4px 16p
 00026af0: 7820 303b 746f 703a 2d32 3470 783b 636f  x 0;top:-24px;co
 00026b00: 6c6f 723a 2366 6666 3b62 6163 6b67 726f  lor:#fff;backgro
 00026b10: 756e 643a 7661 7228 2d2d 6275 696c 6465  und:var(--builde
 00026b20: 7241 6374 696f 6e4f 6e67 6f69 6e67 436f  rActionOngoingCo
 00026b30: 6c6f 7229 7d62 7574 746f 6e5b 6461 7461  lor)}button[data
-00026b40: 2d76 2d30 6566 3362 3832 635d 7b62 6f72  -v-0ef3b82c]{bor
+00026b40: 2d76 2d37 3637 3231 3430 655d 7b62 6f72  -v-7672140e]{bor
 00026b50: 6465 723a 6e6f 6e65 3b62 6163 6b67 726f  der:none;backgro
 00026b60: 756e 643a 7661 7228 2d2d 6275 696c 6465  und:var(--builde
 00026b70: 7253 7562 746c 6553 6570 6172 6174 6f72  rSubtleSeparator
 00026b80: 436f 6c6f 7229 3b6f 7574 6c69 6e65 3a6e  Color);outline:n
 00026b90: 6f6e 653b 636f 6c6f 723a 7661 7228 2d2d  one;color:var(--
 00026ba0: 6275 696c 6465 7250 7269 6d61 7279 5465  builderPrimaryTe
 00026bb0: 7874 436f 6c6f 7229 3b70 6164 6469 6e67  xtColor);padding
 00026bc0: 3a31 3070 7820 3132 7078 3b62 6f72 6465  :10px 12px;borde
 00026bd0: 722d 7261 6469 7573 3a34 7078 3b66 6f6e  r-radius:4px;fon
 00026be0: 742d 7369 7a65 3a2e 3735 7265 6d3b 6375  t-size:.75rem;cu
 00026bf0: 7273 6f72 3a70 6f69 6e74 6572 3b64 6973  rsor:pointer;dis
 00026c00: 706c 6179 3a66 6c65 783b 6761 703a 3870  play:flex;gap:8p
 00026c10: 783b 616c 6967 6e2d 6974 656d 733a 6365  x;align-items:ce
 00026c20: 6e74 6572 7d62 7574 746f 6e5b 6461 7461  nter}button[data
-00026c30: 2d76 2d30 6566 3362 3832 635d 3a66 6f63  -v-0ef3b82c]:foc
+00026c30: 2d76 2d37 3637 3231 3430 655d 3a66 6f63  -v-7672140e]:foc
 00026c40: 7573 2c62 7574 746f 6e5b 6461 7461 2d76  us,button[data-v
-00026c50: 2d30 6566 3362 3832 635d 3a68 6f76 6572  -0ef3b82c]:hover
+00026c50: 2d37 3637 3231 3430 655d 3a68 6f76 6572  -7672140e]:hover
 00026c60: 7b62 6163 6b67 726f 756e 643a 7661 7228  {background:var(
 00026c70: 2d2d 6275 696c 6465 7241 6374 696f 6e4f  --builderActionO
 00026c80: 6e67 6f69 6e67 436f 6c6f 7229 3b63 6f6c  ngoingColor);col
 00026c90: 6f72 3a76 6172 282d 2d62 7569 6c64 6572  or:var(--builder
 00026ca0: 4261 636b 6772 6f75 6e64 436f 6c6f 7229  BackgroundColor)
-00026cb0: 7d62 7574 746f 6e5b 6461 7461 2d76 2d30  }button[data-v-0
-00026cc0: 6566 3362 3832 635d 3a68 6173 2869 2b69  ef3b82c]:has(i+i
+00026cb0: 7d62 7574 746f 6e5b 6461 7461 2d76 2d37  }button[data-v-7
+00026cc0: 3637 3231 3430 655d 3a68 6173 2869 2b69  672140e]:has(i+i
 00026cd0: 297b 6761 703a 307d 6275 7474 6f6e 5b76  ){gap:0}button[v
 00026ce0: 6172 6961 6e74 3d73 7562 746c 655d 5b64  ariant=subtle][d
-00026cf0: 6174 612d 762d 3065 6633 6238 3263 5d7b  ata-v-0ef3b82c]{
+00026cf0: 6174 612d 762d 3736 3732 3134 3065 5d7b  ata-v-7672140e]{
 00026d00: 6261 636b 6772 6f75 6e64 3a75 6e73 6574  background:unset
 00026d10: 7d62 7574 746f 6e5b 7661 7269 616e 743d  }button[variant=
-00026d20: 7375 6274 6c65 5d5b 6461 7461 2d76 2d30  subtle][data-v-0
-00026d30: 6566 3362 3832 635d 3a68 6f76 6572 2c62  ef3b82c]:hover,b
+00026d20: 7375 6274 6c65 5d5b 6461 7461 2d76 2d37  subtle][data-v-7
+00026d30: 3637 3231 3430 655d 3a68 6f76 6572 2c62  672140e]:hover,b
 00026d40: 7574 746f 6e5b 7661 7269 616e 743d 7375  utton[variant=su
-00026d50: 6274 6c65 5d5b 6461 7461 2d76 2d30 6566  btle][data-v-0ef
-00026d60: 3362 3832 635d 3a66 6f63 7573 7b62 6163  3b82c]:focus{bac
+00026d50: 6274 6c65 5d5b 6461 7461 2d76 2d37 3637  btle][data-v-767
+00026d60: 3231 3430 655d 3a66 6f63 7573 7b62 6163  2140e]:focus{bac
 00026d70: 6b67 726f 756e 643a 7661 7228 2d2d 6275  kground:var(--bu
 00026d80: 696c 6465 7241 6374 696f 6e4f 6e67 6f69  ilderActionOngoi
 00026d90: 6e67 436f 6c6f 7229 3b63 6f6c 6f72 3a76  ngColor);color:v
 00026da0: 6172 282d 2d62 7569 6c64 6572 4261 636b  ar(--builderBack
 00026db0: 6772 6f75 6e64 436f 6c6f 7229 7d74 6578  groundColor)}tex
 00026dc0: 7461 7265 615b 7661 7269 616e 743d 636f  tarea[variant=co
-00026dd0: 6465 5d5b 6461 7461 2d76 2d30 6566 3362  de][data-v-0ef3b
-00026de0: 3832 635d 7b66 6f6e 742d 6661 6d69 6c79  82c]{font-family
+00026dd0: 6465 5d5b 6461 7461 2d76 2d37 3637 3231  de][data-v-76721
+00026de0: 3430 655d 7b66 6f6e 742d 6661 6d69 6c79  40e]{font-family
 00026df0: 3a43 6f6e 736f 6c61 732c 6d6f 6e6f 7370  :Consolas,monosp
 00026e00: 6163 657d 636f 6465 5b64 6174 612d 762d  ace}code[data-v-
-00026e10: 3065 6633 6238 3263 5d7b 666f 6e74 2d66  0ef3b82c]{font-f
+00026e10: 3736 3732 3134 3065 5d7b 666f 6e74 2d66  7672140e]{font-f
 00026e20: 616d 696c 793a 6d6f 6e6f 7370 6163 657d  amily:monospace}
 00026e30: 2e6d 6172 6b64 6f77 6e20 636f 6465 5b64  .markdown code[d
-00026e40: 6174 612d 762d 3065 6633 6238 3263 5d7b  ata-v-0ef3b82c]{
+00026e40: 6174 612d 762d 3736 3732 3134 3065 5d7b  ata-v-7672140e]{
 00026e50: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
 00026e60: 3a76 6172 282d 2d62 7569 6c64 6572 5375  :var(--builderSu
 00026e70: 6274 6c65 5365 7061 7261 746f 7243 6f6c  btleSeparatorCol
 00026e80: 6f72 293b 7061 6464 696e 673a 3270 787d  or);padding:2px}
 00026e90: 2e77 696e 646f 7742 6172 5b64 6174 612d  .windowBar[data-
-00026ea0: 762d 3065 6633 6238 3263 5d7b 7061 6464  v-0ef3b82c]{padd
+00026ea0: 762d 3736 3732 3134 3065 5d7b 7061 6464  v-7672140e]{padd
 00026eb0: 696e 673a 3132 7078 2031 3270 7820 3132  ing:12px 12px 12
 00026ec0: 7078 2032 3470 783b 6d69 6e2d 6865 6967  px 24px;min-heig
 00026ed0: 6874 3a34 3870 783b 6469 7370 6c61 793a  ht:48px;display:
 00026ee0: 666c 6578 3b61 6c69 676e 2d69 7465 6d73  flex;align-items
 00026ef0: 3a63 656e 7465 723b 706f 7369 7469 6f6e  :center;position
 00026f00: 3a73 7469 636b 793b 746f 703a 303b 6261  :sticky;top:0;ba
 00026f10: 636b 6772 6f75 6e64 3a76 6172 282d 2d62  ckground:var(--b
 00026f20: 7569 6c64 6572 5375 6274 6c65 4869 6768  uilderSubtleHigh
 00026f30: 6c69 6768 7443 6f6c 6f72 536f 6c69 6429  lightColorSolid)
 00026f40: 3b7a 2d69 6e64 6578 3a32 3b66 6f6e 742d  ;z-index:2;font-
 00026f50: 7369 7a65 3a2e 3872 656d 7d2e 7769 6e64  size:.8rem}.wind
 00026f60: 6f77 4261 7220 2e69 636f 6e5b 6461 7461  owBar .icon[data
-00026f70: 2d76 2d30 6566 3362 3832 635d 7b6d 6172  -v-0ef3b82c]{mar
+00026f70: 2d76 2d37 3637 3231 3430 655d 7b6d 6172  -v-7672140e]{mar
 00026f80: 6769 6e2d 7269 6768 743a 3870 783b 6469  gin-right:8px;di
 00026f90: 7370 6c61 793a 666c 6578 3b61 6c69 676e  splay:flex;align
 00026fa0: 2d69 7465 6d73 3a63 656e 7465 727d 2e77  -items:center}.w
 00026fb0: 696e 646f 7742 6172 202e 7469 746c 655b  indowBar .title[
-00026fc0: 6461 7461 2d76 2d30 6566 3362 3832 635d  data-v-0ef3b82c]
+00026fc0: 6461 7461 2d76 2d37 3637 3231 3430 655d  data-v-7672140e]
 00026fd0: 7b66 6c65 783a 3120 3120 6175 746f 3b6f  {flex:1 1 auto;o
 00026fe0: 7665 7266 6c6f 773a 6869 6464 656e 3b74  verflow:hidden;t
 00026ff0: 6578 742d 6f76 6572 666c 6f77 3a65 6c6c  ext-overflow:ell
 00027000: 6970 7369 733b 7768 6974 652d 7370 6163  ipsis;white-spac
 00027010: 653a 6e6f 7772 6170 7d2e 7769 6e64 6f77  e:nowrap}.window
 00027020: 4261 7220 2e77 696e 646f 7741 6374 696f  Bar .windowActio
-00027030: 6e5b 6461 7461 2d76 2d30 6566 3362 3832  n[data-v-0ef3b82
-00027040: 635d 7b68 6569 6768 743a 3234 7078 3b6d  c]{height:24px;m
+00027030: 6e5b 6461 7461 2d76 2d37 3637 3231 3430  n[data-v-7672140
+00027040: 655d 7b68 6569 6768 743a 3234 7078 3b6d  e]{height:24px;m
 00027050: 696e 2d77 6964 7468 3a32 3470 783b 7061  in-width:24px;pa
 00027060: 6464 696e 672d 6c65 6674 3a38 7078 3b70  dding-left:8px;p
 00027070: 6164 6469 6e67 2d72 6967 6874 3a38 7078  adding-right:8px
 00027080: 3b66 6c65 783a 3020 3020 6175 746f 3b64  ;flex:0 0 auto;d
 00027090: 6973 706c 6179 3a66 6c65 783b 626f 7264  isplay:flex;bord
 000270a0: 6572 2d72 6164 6975 733a 3132 7078 3b61  er-radius:12px;a
 000270b0: 6c69 676e 2d69 7465 6d73 3a63 656e 7465  lign-items:cente
@@ -9999,54 +9999,54 @@
 000270e0: 756e 643a 7661 7228 2d2d 6275 696c 6465  und:var(--builde
 000270f0: 7253 7562 746c 6548 6967 686c 6967 6874  rSubtleHighlight
 00027100: 436f 6c6f 7229 3b63 7572 736f 723a 706f  Color);cursor:po
 00027110: 696e 7465 723b 6d61 7267 696e 2d6c 6566  inter;margin-lef
 00027120: 743a 3870 783b 6f75 746c 696e 653a 6e6f  t:8px;outline:no
 00027130: 6e65 7d2e 7769 6e64 6f77 4261 7220 2e77  ne}.windowBar .w
 00027140: 696e 646f 7741 6374 696f 6e5b 6461 7461  indowAction[data
-00027150: 2d76 2d30 6566 3362 3832 635d 3a66 6f63  -v-0ef3b82c]:foc
+00027150: 2d76 2d37 3637 3231 3430 655d 3a66 6f63  -v-7672140e]:foc
 00027160: 7573 2c2e 7769 6e64 6f77 4261 7220 2e77  us,.windowBar .w
 00027170: 696e 646f 7741 6374 696f 6e5b 6461 7461  indowAction[data
-00027180: 2d76 2d30 6566 3362 3832 635d 3a68 6f76  -v-0ef3b82c]:hov
+00027180: 2d76 2d37 3637 3231 3430 655d 3a68 6f76  -v-7672140e]:hov
 00027190: 6572 7b63 6f6c 6f72 3a76 6172 282d 2d62  er{color:var(--b
 000271a0: 7569 6c64 6572 4261 636b 6772 6f75 6e64  uilderBackground
 000271b0: 436f 6c6f 7229 3b62 6163 6b67 726f 756e  Color);backgroun
 000271c0: 643a 7661 7228 2d2d 6275 696c 6465 7241  d:var(--builderA
 000271d0: 6374 696f 6e4f 6e67 6f69 6e67 436f 6c6f  ctionOngoingColo
 000271e0: 7229 7d2e 7365 6374 696f 6e54 6974 6c65  r)}.sectionTitle
-000271f0: 5b64 6174 612d 762d 3065 6633 6238 3263  [data-v-0ef3b82c
+000271f0: 5b64 6174 612d 762d 3736 3732 3134 3065  [data-v-7672140e
 00027200: 5d7b 6469 7370 6c61 793a 666c 6578 3b67  ]{display:flex;g
 00027210: 6170 3a38 7078 3b61 6c69 676e 2d69 7465  ap:8px;align-ite
 00027220: 6d73 3a63 656e 7465 727d 2e66 6965 6c64  ms:center}.field
-00027230: 5772 6170 7065 725b 6461 7461 2d76 2d30  Wrapper[data-v-0
-00027240: 6566 3362 3832 635d 7b70 6f73 6974 696f  ef3b82c]{positio
+00027230: 5772 6170 7065 725b 6461 7461 2d76 2d37  Wrapper[data-v-7
+00027240: 3637 3231 3430 655d 7b70 6f73 6974 696f  672140e]{positio
 00027250: 6e3a 7265 6c61 7469 7665 3b77 6964 7468  n:relative;width
 00027260: 3a31 3030 253b 6d61 7267 696e 2d74 6f70  :100%;margin-top
 00027270: 3a31 3670 787d 3a69 7328 2e66 6965 6c64  :16px}:is(.field
 00027280: 5772 6170 7065 722c 2e66 6965 6c64 5772  Wrapper,.fieldWr
 00027290: 6170 7065 724d 6169 6e29 3e2e 6e61 6d65  apperMain)>.name
-000272a0: 5b64 6174 612d 762d 3065 6633 6238 3263  [data-v-0ef3b82c
+000272a0: 5b64 6174 612d 762d 3736 3732 3134 3065  [data-v-7672140e
 000272b0: 5d7b 706f 7369 7469 6f6e 3a61 6273 6f6c  ]{position:absol
 000272c0: 7574 653b 746f 703a 303b 6c65 6674 3a38  ute;top:0;left:8
 000272d0: 7078 3b62 6163 6b67 726f 756e 643a 7661  px;background:va
 000272e0: 7228 2d2d 6275 696c 6465 7242 6163 6b67  r(--builderBackg
 000272f0: 726f 756e 6443 6f6c 6f72 293b 7061 6464  roundColor);padd
 00027300: 696e 673a 3020 3470 7820 3470 783b 666f  ing:0 4px 4px;fo
 00027310: 6e74 2d73 697a 653a 2e37 7265 6d3b 7a2d  nt-size:.7rem;z-
 00027320: 696e 6465 783a 317d 3a69 7328 2e66 6965  index:1}:is(.fie
 00027330: 6c64 5772 6170 7065 722c 2e66 6965 6c64  ldWrapper,.field
 00027340: 5772 6170 7065 724d 6169 6e29 202e 6e61  WrapperMain) .na
 00027350: 6d65 202e 7479 7065 5b64 6174 612d 762d  me .type[data-v-
-00027360: 3065 6633 6238 3263 5d7b 636f 6c6f 723a  0ef3b82c]{color:
+00027360: 3736 3732 3134 3065 5d7b 636f 6c6f 723a  7672140e]{color:
 00027370: 7661 7228 2d2d 6275 696c 6465 7253 6563  var(--builderSec
 00027380: 6f6e 6461 7279 5465 7874 436f 6c6f 7229  ondaryTextColor)
 00027390: 7d3a 6973 282e 6669 656c 6457 7261 7070  }:is(.fieldWrapp
 000273a0: 6572 2c2e 6669 656c 6457 7261 7070 6572  er,.fieldWrapper
 000273b0: 4d61 696e 2920 2e63 6f6e 7465 6e74 5b64  Main) .content[d
-000273c0: 6174 612d 762d 3065 6633 6238 3263 5d7b  ata-v-0ef3b82c]{
+000273c0: 6174 612d 762d 3736 3732 3134 3065 5d7b  ata-v-7672140e]{
 000273d0: 706f 7369 7469 6f6e 3a72 656c 6174 6976  position:relativ
 000273e0: 653b 746f 703a 3670 783b 6d61 7267 696e  e;top:6px;margin
 000273f0: 2d62 6f74 746f 6d3a 3134 7078 3b77 6964  -bottom:14px;wid
 00027400: 7468 3a31 3030 253b 626f 7264 6572 2d72  th:100%;border-r
 00027410: 6164 6975 733a 3470 783b 626f 7264 6572  adius:4px;border
 00027420: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
 00027430: 2d62 7569 6c64 6572 5365 7061 7261 746f  -builderSeparato
@@ -10054,70 +10054,70 @@
 00027450: 653a 2e37 3572 656d 3b62 6163 6b67 726f  e:.75rem;backgro
 00027460: 756e 643a 7661 7228 2d2d 6275 696c 6465  und:var(--builde
 00027470: 7242 6163 6b67 726f 756e 6443 6f6c 6f72  rBackgroundColor
 00027480: 293b 6f75 746c 696e 653a 6e6f 6e65 7d3a  );outline:none}:
 00027490: 6973 282e 6669 656c 6457 7261 7070 6572  is(.fieldWrapper
 000274a0: 2c2e 6669 656c 6457 7261 7070 6572 4d61  ,.fieldWrapperMa
 000274b0: 696e 2920 2e63 6f6e 7465 6e74 5b64 6174  in) .content[dat
-000274c0: 612d 762d 3065 6633 6238 3263 5d3a 666f  a-v-0ef3b82c]:fo
+000274c0: 612d 762d 3736 3732 3134 3065 5d3a 666f  a-v-7672140e]:fo
 000274d0: 6375 732d 7769 7468 696e 7b62 6f72 6465  cus-within{borde
 000274e0: 723a 3170 7820 736f 6c69 6420 7661 7228  r:1px solid var(
 000274f0: 2d2d 6275 696c 6465 7250 7269 6d61 7279  --builderPrimary
 00027500: 5465 7874 436f 6c6f 7229 7d3a 6973 282e  TextColor)}:is(.
 00027510: 6669 656c 6457 7261 7070 6572 2c2e 6669  fieldWrapper,.fi
 00027520: 656c 6457 7261 7070 6572 4d61 696e 2920  eldWrapperMain) 
 00027530: 2e63 6f6e 7465 6e74 2074 6578 7461 7265  .content textare
-00027540: 615b 6461 7461 2d76 2d30 6566 3362 3832  a[data-v-0ef3b82
-00027550: 635d 2c3a 6973 282e 6669 656c 6457 7261  c],:is(.fieldWra
+00027540: 615b 6461 7461 2d76 2d37 3637 3231 3430  a[data-v-7672140
+00027550: 655d 2c3a 6973 282e 6669 656c 6457 7261  e],:is(.fieldWra
 00027560: 7070 6572 2c2e 6669 656c 6457 7261 7070  pper,.fieldWrapp
 00027570: 6572 4d61 696e 2920 2e63 6f6e 7465 6e74  erMain) .content
-00027580: 2069 6e70 7574 5b64 6174 612d 762d 3065   input[data-v-0e
-00027590: 6633 6238 3263 5d7b 626f 7264 6572 3a30  f3b82c]{border:0
+00027580: 2069 6e70 7574 5b64 6174 612d 762d 3736   input[data-v-76
+00027590: 3732 3134 3065 5d7b 626f 7264 6572 3a30  72140e]{border:0
 000275a0: 3b6f 7574 6c69 6e65 3a6e 6f6e 653b 7769  ;outline:none;wi
 000275b0: 6474 683a 3130 3025 7d2e 6669 656c 6457  dth:100%}.fieldW
 000275c0: 7261 7070 6572 3e2e 6465 7363 5b64 6174  rapper>.desc[dat
-000275d0: 612d 762d 3065 6633 6238 3263 5d7b 636f  a-v-0ef3b82c]{co
+000275d0: 612d 762d 3736 3732 3134 3065 5d7b 636f  a-v-7672140e]{co
 000275e0: 6c6f 723a 7661 7228 2d2d 6275 696c 6465  lor:var(--builde
 000275f0: 7253 6563 6f6e 6461 7279 5465 7874 436f  rSecondaryTextCo
 00027600: 6c6f 7229 3b66 6f6e 742d 7369 7a65 3a2e  lor);font-size:.
 00027610: 3772 656d 7d2e 6368 6970 5374 6163 6b5b  7rem}.chipStack[
-00027620: 6461 7461 2d76 2d30 6566 3362 3832 635d  data-v-0ef3b82c]
+00027620: 6461 7461 2d76 2d37 3637 3231 3430 655d  data-v-7672140e]
 00027630: 7b64 6973 706c 6179 3a66 6c65 783b 666c  {display:flex;fl
 00027640: 6578 2d64 6972 6563 7469 6f6e 3a72 6f77  ex-direction:row
 00027650: 3b66 6c65 782d 7772 6170 3a77 7261 703b  ;flex-wrap:wrap;
 00027660: 6761 703a 3470 787d 2e63 6869 705b 6461  gap:4px}.chip[da
-00027670: 7461 2d76 2d30 6566 3362 3832 635d 7b66  ta-v-0ef3b82c]{f
+00027670: 7461 2d76 2d37 3637 3231 3430 655d 7b66  ta-v-7672140e]{f
 00027680: 6f6e 742d 7369 7a65 3a2e 3735 7265 6d3b  ont-size:.75rem;
 00027690: 626f 7264 6572 2d72 6164 6975 733a 3136  border-radius:16
 000276a0: 7078 3b70 6164 6469 6e67 3a38 7078 2031  px;padding:8px 1
 000276b0: 3270 783b 6375 7273 6f72 3a70 6f69 6e74  2px;cursor:point
 000276c0: 6572 3b6f 7574 6c69 6e65 3a6e 6f6e 653b  er;outline:none;
 000276d0: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
 000276e0: 2d62 7569 6c64 6572 4261 636b 6772 6f75  -builderBackgrou
 000276f0: 6e64 436f 6c6f 7229 7d2e 6368 6970 5b64  ndColor)}.chip[d
-00027700: 6174 612d 762d 3065 6633 6238 3263 5d3a  ata-v-0ef3b82c]:
+00027700: 6174 612d 762d 3736 3732 3134 3065 5d3a  ata-v-7672140e]:
 00027710: 666f 6375 732c 2e63 6869 702e 6163 7469  focus,.chip.acti
-00027720: 7665 5b64 6174 612d 762d 3065 6633 6238  ve[data-v-0ef3b8
-00027730: 3263 5d3a 666f 6375 732c 2e63 6869 705b  2c]:focus,.chip[
-00027740: 6461 7461 2d76 2d30 6566 3362 3832 635d  data-v-0ef3b82c]
+00027720: 7665 5b64 6174 612d 762d 3736 3732 3134  ve[data-v-767214
+00027730: 3065 5d3a 666f 6375 732c 2e63 6869 705b  0e]:focus,.chip[
+00027740: 6461 7461 2d76 2d37 3637 3231 3430 655d  data-v-7672140e]
 00027750: 3a68 6f76 6572 2c2e 6368 6970 2e61 6374  :hover,.chip.act
-00027760: 6976 655b 6461 7461 2d76 2d30 6566 3362  ive[data-v-0ef3b
-00027770: 3832 635d 3a68 6f76 6572 7b63 6f6c 6f72  82c]:hover{color
+00027760: 6976 655b 6461 7461 2d76 2d37 3637 3231  ive[data-v-76721
+00027770: 3430 655d 3a68 6f76 6572 7b63 6f6c 6f72  40e]:hover{color
 00027780: 3a76 6172 282d 2d62 7569 6c64 6572 4261  :var(--builderBa
 00027790: 636b 6772 6f75 6e64 436f 6c6f 7229 3b62  ckgroundColor);b
 000277a0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
 000277b0: 6275 696c 6465 7241 6374 696f 6e4f 6e67  builderActionOng
 000277c0: 6f69 6e67 436f 6c6f 7229 7d2e 6368 6970  oingColor)}.chip
-000277d0: 2e61 6374 6976 655b 6461 7461 2d76 2d30  .active[data-v-0
-000277e0: 6566 3362 3832 635d 7b62 6163 6b67 726f  ef3b82c]{backgro
+000277d0: 2e61 6374 6976 655b 6461 7461 2d76 2d37  .active[data-v-7
+000277e0: 3637 3231 3430 655d 7b62 6163 6b67 726f  672140e]{backgro
 000277f0: 756e 643a 7661 7228 2d2d 6275 696c 6465  und:var(--builde
 00027800: 7253 7562 746c 6553 6570 6172 6174 6f72  rSubtleSeparator
 00027810: 436f 6c6f 7229 7d2e 636f 756e 744c 6162  Color)}.countLab
-00027820: 656c 5b64 6174 612d 762d 3065 6633 6238  el[data-v-0ef3b8
-00027830: 3263 5d7b 6261 636b 6772 6f75 6e64 3a76  2c]{background:v
+00027820: 656c 5b64 6174 612d 762d 3736 3732 3134  el[data-v-767214
+00027830: 3065 5d7b 6261 636b 6772 6f75 6e64 3a76  0e]{background:v
 00027840: 6172 282d 2d62 7569 6c64 6572 496e 7465  ar(--builderInte
 00027850: 6e73 6553 656c 6563 7465 6443 6f6c 6f72  nseSelectedColor
 00027860: 293b 6469 7370 6c61 793a 696e 6c69 6e65  );display:inline
 00027870: 2d66 6c65 783b 636f 6c6f 723a 7661 7228  -flex;color:var(
 00027880: 2d2d 6275 696c 6465 7242 6163 6b67 726f  --builderBackgro
 00027890: 756e 6443 6f6c 6f72 293b 616c 6967 6e2d  undColor);align-
 000278a0: 6974 656d 733a 6365 6e74 6572 3b6a 7573  items:center;jus
@@ -10127,18 +10127,18 @@
 000278e0: 6874 3a34 7078 3b6d 696e 2d77 6964 7468  ht:4px;min-width
 000278f0: 3a32 3070 783b 6865 6967 6874 3a32 3070  :20px;height:20p
 00027900: 783b 626f 7264 6572 2d72 6164 6975 733a  x;border-radius:
 00027910: 3130 7078 3b6d 6172 6769 6e2d 6c65 6674  10px;margin-left
 00027920: 3a38 7078 3b66 6f6e 742d 7369 7a65 3a2e  :8px;font-size:.
 00027930: 3772 656d 7d2e 6368 6970 5374 6163 6b43  7rem}.chipStackC
 00027940: 6f6e 7461 696e 6572 5b64 6174 612d 762d  ontainer[data-v-
-00027950: 3065 6633 6238 3263 5d7b 7061 6464 696e  0ef3b82c]{paddin
+00027950: 3736 3732 3134 3065 5d7b 7061 6464 696e  7672140e]{paddin
 00027960: 673a 3132 7078 3b6d 6172 6769 6e2d 746f  g:12px;margin-to
 00027970: 703a 3470 787d 2e6d 6169 6e5b 6461 7461  p:4px}.main[data
-00027980: 2d76 2d30 6566 3362 3832 635d 7b62 6f72  -v-0ef3b82c]{bor
+00027980: 2d76 2d37 3637 3231 3430 655d 7b62 6f72  -v-7672140e]{bor
 00027990: 6465 722d 746f 703a 3170 7820 736f 6c69  der-top:1px soli
 000279a0: 6420 7661 7228 2d2d 6275 696c 6465 7253  d var(--builderS
 000279b0: 6570 6172 6174 6f72 436f 6c6f 7229 3b70  eparatorColor);p
 000279c0: 6164 6469 6e67 3a31 3270 787d 4066 6f6e  adding:12px}@fon
 000279d0: 742d 6661 6365 7b66 6f6e 742d 6661 6d69  t-face{font-fami
 000279e0: 6c79 3a49 6e74 6572 3b73 7263 3a75 726c  ly:Inter;src:url
 000279f0: 282e 2f49 6e74 6572 2d52 6567 756c 6172  (./Inter-Regular
@@ -13038,15 +13038,15 @@
 00032ed0: 6572 2d52 6567 756c 6172 2d64 3631 3266  er-Regular-d612f
 00032ee0: 3132 312e 776f 6666 3229 2066 6f72 6d61  121.woff2) forma
 00032ef0: 7428 2277 6f66 6632 2229 2c75 726c 282e  t("woff2"),url(.
 00032f00: 2f49 6e74 6572 2d52 6567 756c 6172 2d34  /Inter-Regular-4
 00032f10: 3161 6230 6637 302e 7474 6629 2066 6f72  1ab0f70.ttf) for
 00032f20: 6d61 7428 2274 7275 6574 7970 6522 297d  mat("truetype")}
 00032f30: 2e42 7569 6c64 6572 4170 705b 6461 7461  .BuilderApp[data
-00032f40: 2d76 2d35 6534 3030 3464 365d 7b2d 2d62  -v-5e4004d6]{--b
+00032f40: 2d76 2d65 3830 3361 6236 395d 7b2d 2d62  -v-e803ab69]{--b
 00032f50: 7569 6c64 6572 4261 636b 6772 6f75 6e64  uilderBackground
 00032f60: 436f 6c6f 723a 2023 6666 6666 6666 3b2d  Color: #ffffff;-
 00032f70: 2d62 7569 6c64 6572 4163 6365 6e74 436f  -builderAccentCo
 00032f80: 6c6f 723a 2023 3239 6366 3030 3b2d 2d62  lor: #29cf00;--b
 00032f90: 7569 6c64 6572 5375 6363 6573 7343 6f6c  uilderSuccessCol
 00032fa0: 6f72 3a20 2332 3963 6630 303b 2d2d 6275  or: #29cf00;--bu
 00032fb0: 696c 6465 7245 7272 6f72 436f 6c6f 723a  ilderErrorColor:
@@ -13092,135 +13092,135 @@
 00033230: 7828 3236 3570 782c 2032 3776 6829 3b2d  x(265px, 27vh);-
 00033240: 2d62 7569 6c64 6572 5365 7474 696e 6773  -builderSettings
 00033250: 5769 6474 683a 206d 6178 2832 3635 7078  Width: max(265px
 00033260: 2c20 3237 7668 293b 2d2d 6275 696c 6465  , 27vh);--builde
 00033270: 7241 6374 696f 6e4f 6e67 6f69 6e67 436f  rActionOngoingCo
 00033280: 6c6f 723a 2072 6762 6128 302c 2030 2c20  lor: rgba(0, 0, 
 00033290: 302c 202e 3729 7d68 315b 6461 7461 2d76  0, .7)}h1[data-v
-000332a0: 2d35 6534 3030 3464 365d 2c68 325b 6461  -5e4004d6],h2[da
-000332b0: 7461 2d76 2d35 6534 3030 3464 365d 2c68  ta-v-5e4004d6],h
-000332c0: 335b 6461 7461 2d76 2d35 6534 3030 3464  3[data-v-5e4004d
-000332d0: 365d 7b66 6f6e 742d 7765 6967 6874 3a33  6]{font-weight:3
+000332a0: 2d65 3830 3361 6236 395d 2c68 325b 6461  -e803ab69],h2[da
+000332b0: 7461 2d76 2d65 3830 3361 6236 395d 2c68  ta-v-e803ab69],h
+000332c0: 335b 6461 7461 2d76 2d65 3830 3361 6236  3[data-v-e803ab6
+000332d0: 395d 7b66 6f6e 742d 7765 6967 6874 3a33  9]{font-weight:3
 000332e0: 3030 3b6d 6172 6769 6e3a 307d 6831 5b64  00;margin:0}h1[d
-000332f0: 6174 612d 762d 3565 3430 3034 6436 5d7b  ata-v-5e4004d6]{
+000332f0: 6174 612d 762d 6538 3033 6162 3639 5d7b  ata-v-e803ab69]{
 00033300: 666f 6e74 2d73 697a 653a 312e 3372 656d  font-size:1.3rem
-00033310: 7d68 325b 6461 7461 2d76 2d35 6534 3030  }h2[data-v-5e400
-00033320: 3464 365d 7b66 6f6e 742d 7369 7a65 3a31  4d6]{font-size:1
-00033330: 7265 6d7d 6833 5b64 6174 612d 762d 3565  rem}h3[data-v-5e
-00033340: 3430 3034 6436 5d7b 666f 6e74 2d73 697a  4004d6]{font-siz
+00033310: 7d68 325b 6461 7461 2d76 2d65 3830 3361  }h2[data-v-e803a
+00033320: 6236 395d 7b66 6f6e 742d 7369 7a65 3a31  b69]{font-size:1
+00033330: 7265 6d7d 6833 5b64 6174 612d 762d 6538  rem}h3[data-v-e8
+00033340: 3033 6162 3639 5d7b 666f 6e74 2d73 697a  03ab69]{font-siz
 00033350: 653a 2e38 7265 6d7d 6834 5b64 6174 612d  e:.8rem}h4[data-
-00033360: 762d 3565 3430 3034 6436 5d7b 7465 7874  v-5e4004d6]{text
+00033360: 762d 6538 3033 6162 3639 5d7b 7465 7874  v-e803ab69]{text
 00033370: 2d74 7261 6e73 666f 726d 3a75 7070 6572  -transform:upper
 00033380: 6361 7365 3b66 6f6e 742d 7765 6967 6874  case;font-weight
 00033390: 3a37 3030 3b66 6f6e 742d 7369 7a65 3a2e  :700;font-size:.
 000333a0: 3635 7265 6d3b 6c65 7474 6572 2d73 7061  65rem;letter-spa
 000333b0: 6369 6e67 3a2e 3263 687d 2e69 6e73 6572  cing:.2ch}.inser
 000333c0: 7469 6f6e 4f76 6572 6c61 795b 6461 7461  tionOverlay[data
-000333d0: 2d76 2d35 6534 3030 3464 365d 7b62 6163  -v-5e4004d6]{bac
+000333d0: 2d76 2d65 3830 3361 6236 395d 7b62 6163  -v-e803ab69]{bac
 000333e0: 6b67 726f 756e 643a 7267 6261 2832 3130  kground:rgba(210
 000333f0: 2c32 3334 2c32 3434 2c2e 3529 3b70 6f69  ,234,244,.5);poi
 00033400: 6e74 6572 2d65 7665 6e74 733a 6e6f 6e65  nter-events:none
 00033410: 3b70 6f73 6974 696f 6e3a 6162 736f 6c75  ;position:absolu
 00033420: 7465 3b74 6f70 3a30 3b6c 6566 743a 303b  te;top:0;left:0;
 00033430: 6d61 782d 6865 6967 6874 3a31 3030 253b  max-height:100%;
 00033440: 6d61 782d 7769 6474 683a 3130 3025 7d2e  max-width:100%}.
 00033450: 696e 7365 7274 696f 6e4f 7665 726c 6179  insertionOverlay
-00033460: 202e 6c61 6265 6c5b 6461 7461 2d76 2d35   .label[data-v-5
-00033470: 6534 3030 3464 365d 7b62 6f72 6465 722d  e4004d6]{border-
+00033460: 202e 6c61 6265 6c5b 6461 7461 2d76 2d65   .label[data-v-e
+00033470: 3830 3361 6236 395d 7b62 6f72 6465 722d  803ab69]{border-
 00033480: 7261 6469 7573 3a31 3670 783b 626f 782d  radius:16px;box-
 00033490: 7368 6164 6f77 3a30 2030 2038 7078 202d  shadow:0 0 8px -
 000334a0: 3170 7820 2330 3030 363b 706f 7369 7469  1px #0006;positi
 000334b0: 6f6e 3a61 6273 6f6c 7574 653b 7269 6768  on:absolute;righ
 000334c0: 743a 303b 6865 6967 6874 3a32 3470 783b  t:0;height:24px;
 000334d0: 7061 6464 696e 673a 3470 7820 3136 7078  padding:4px 16px
 000334e0: 2030 3b74 6f70 3a2d 3234 7078 3b63 6f6c   0;top:-24px;col
 000334f0: 6f72 3a23 6666 663b 6261 636b 6772 6f75  or:#fff;backgrou
 00033500: 6e64 3a76 6172 282d 2d62 7569 6c64 6572  nd:var(--builder
 00033510: 4163 7469 6f6e 4f6e 676f 696e 6743 6f6c  ActionOngoingCol
 00033520: 6f72 297d 6275 7474 6f6e 5b64 6174 612d  or)}button[data-
-00033530: 762d 3565 3430 3034 6436 5d7b 626f 7264  v-5e4004d6]{bord
+00033530: 762d 6538 3033 6162 3639 5d7b 626f 7264  v-e803ab69]{bord
 00033540: 6572 3a6e 6f6e 653b 6261 636b 6772 6f75  er:none;backgrou
 00033550: 6e64 3a76 6172 282d 2d62 7569 6c64 6572  nd:var(--builder
 00033560: 5375 6274 6c65 5365 7061 7261 746f 7243  SubtleSeparatorC
 00033570: 6f6c 6f72 293b 6f75 746c 696e 653a 6e6f  olor);outline:no
 00033580: 6e65 3b63 6f6c 6f72 3a76 6172 282d 2d62  ne;color:var(--b
 00033590: 7569 6c64 6572 5072 696d 6172 7954 6578  uilderPrimaryTex
 000335a0: 7443 6f6c 6f72 293b 7061 6464 696e 673a  tColor);padding:
 000335b0: 3130 7078 2031 3270 783b 626f 7264 6572  10px 12px;border
 000335c0: 2d72 6164 6975 733a 3470 783b 666f 6e74  -radius:4px;font
 000335d0: 2d73 697a 653a 2e37 3572 656d 3b63 7572  -size:.75rem;cur
 000335e0: 736f 723a 706f 696e 7465 723b 6469 7370  sor:pointer;disp
 000335f0: 6c61 793a 666c 6578 3b67 6170 3a38 7078  lay:flex;gap:8px
 00033600: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
 00033610: 7465 727d 6275 7474 6f6e 5b64 6174 612d  ter}button[data-
-00033620: 762d 3565 3430 3034 6436 5d3a 666f 6375  v-5e4004d6]:focu
+00033620: 762d 6538 3033 6162 3639 5d3a 666f 6375  v-e803ab69]:focu
 00033630: 732c 6275 7474 6f6e 5b64 6174 612d 762d  s,button[data-v-
-00033640: 3565 3430 3034 6436 5d3a 686f 7665 727b  5e4004d6]:hover{
+00033640: 6538 3033 6162 3639 5d3a 686f 7665 727b  e803ab69]:hover{
 00033650: 6261 636b 6772 6f75 6e64 3a76 6172 282d  background:var(-
 00033660: 2d62 7569 6c64 6572 4163 7469 6f6e 4f6e  -builderActionOn
 00033670: 676f 696e 6743 6f6c 6f72 293b 636f 6c6f  goingColor);colo
 00033680: 723a 7661 7228 2d2d 6275 696c 6465 7242  r:var(--builderB
 00033690: 6163 6b67 726f 756e 6443 6f6c 6f72 297d  ackgroundColor)}
-000336a0: 6275 7474 6f6e 5b64 6174 612d 762d 3565  button[data-v-5e
-000336b0: 3430 3034 6436 5d3a 6861 7328 692b 6929  4004d6]:has(i+i)
+000336a0: 6275 7474 6f6e 5b64 6174 612d 762d 6538  button[data-v-e8
+000336b0: 3033 6162 3639 5d3a 6861 7328 692b 6929  03ab69]:has(i+i)
 000336c0: 7b67 6170 3a30 7d62 7574 746f 6e5b 7661  {gap:0}button[va
 000336d0: 7269 616e 743d 7375 6274 6c65 5d5b 6461  riant=subtle][da
-000336e0: 7461 2d76 2d35 6534 3030 3464 365d 7b62  ta-v-5e4004d6]{b
+000336e0: 7461 2d76 2d65 3830 3361 6236 395d 7b62  ta-v-e803ab69]{b
 000336f0: 6163 6b67 726f 756e 643a 756e 7365 747d  ackground:unset}
 00033700: 6275 7474 6f6e 5b76 6172 6961 6e74 3d73  button[variant=s
-00033710: 7562 746c 655d 5b64 6174 612d 762d 3565  ubtle][data-v-5e
-00033720: 3430 3034 6436 5d3a 686f 7665 722c 6275  4004d6]:hover,bu
+00033710: 7562 746c 655d 5b64 6174 612d 762d 6538  ubtle][data-v-e8
+00033720: 3033 6162 3639 5d3a 686f 7665 722c 6275  03ab69]:hover,bu
 00033730: 7474 6f6e 5b76 6172 6961 6e74 3d73 7562  tton[variant=sub
-00033740: 746c 655d 5b64 6174 612d 762d 3565 3430  tle][data-v-5e40
-00033750: 3034 6436 5d3a 666f 6375 737b 6261 636b  04d6]:focus{back
+00033740: 746c 655d 5b64 6174 612d 762d 6538 3033  tle][data-v-e803
+00033750: 6162 3639 5d3a 666f 6375 737b 6261 636b  ab69]:focus{back
 00033760: 6772 6f75 6e64 3a76 6172 282d 2d62 7569  ground:var(--bui
 00033770: 6c64 6572 4163 7469 6f6e 4f6e 676f 696e  lderActionOngoin
 00033780: 6743 6f6c 6f72 293b 636f 6c6f 723a 7661  gColor);color:va
 00033790: 7228 2d2d 6275 696c 6465 7242 6163 6b67  r(--builderBackg
 000337a0: 726f 756e 6443 6f6c 6f72 297d 7465 7874  roundColor)}text
 000337b0: 6172 6561 5b76 6172 6961 6e74 3d63 6f64  area[variant=cod
-000337c0: 655d 5b64 6174 612d 762d 3565 3430 3034  e][data-v-5e4004
-000337d0: 6436 5d7b 666f 6e74 2d66 616d 696c 793a  d6]{font-family:
+000337c0: 655d 5b64 6174 612d 762d 6538 3033 6162  e][data-v-e803ab
+000337d0: 3639 5d7b 666f 6e74 2d66 616d 696c 793a  69]{font-family:
 000337e0: 436f 6e73 6f6c 6173 2c6d 6f6e 6f73 7061  Consolas,monospa
-000337f0: 6365 7d63 6f64 655b 6461 7461 2d76 2d35  ce}code[data-v-5
-00033800: 6534 3030 3464 365d 7b66 6f6e 742d 6661  e4004d6]{font-fa
+000337f0: 6365 7d63 6f64 655b 6461 7461 2d76 2d65  ce}code[data-v-e
+00033800: 3830 3361 6236 395d 7b66 6f6e 742d 6661  803ab69]{font-fa
 00033810: 6d69 6c79 3a6d 6f6e 6f73 7061 6365 7d2e  mily:monospace}.
 00033820: 6d61 726b 646f 776e 2063 6f64 655b 6461  markdown code[da
-00033830: 7461 2d76 2d35 6534 3030 3464 365d 7b62  ta-v-5e4004d6]{b
+00033830: 7461 2d76 2d65 3830 3361 6236 395d 7b62  ta-v-e803ab69]{b
 00033840: 6163 6b67 726f 756e 642d 636f 6c6f 723a  ackground-color:
 00033850: 7661 7228 2d2d 6275 696c 6465 7253 7562  var(--builderSub
 00033860: 746c 6553 6570 6172 6174 6f72 436f 6c6f  tleSeparatorColo
 00033870: 7229 3b70 6164 6469 6e67 3a32 7078 7d2e  r);padding:2px}.
 00033880: 7769 6e64 6f77 4261 725b 6461 7461 2d76  windowBar[data-v
-00033890: 2d35 6534 3030 3464 365d 7b70 6164 6469  -5e4004d6]{paddi
+00033890: 2d65 3830 3361 6236 395d 7b70 6164 6469  -e803ab69]{paddi
 000338a0: 6e67 3a31 3270 7820 3132 7078 2031 3270  ng:12px 12px 12p
 000338b0: 7820 3234 7078 3b6d 696e 2d68 6569 6768  x 24px;min-heigh
 000338c0: 743a 3438 7078 3b64 6973 706c 6179 3a66  t:48px;display:f
 000338d0: 6c65 783b 616c 6967 6e2d 6974 656d 733a  lex;align-items:
 000338e0: 6365 6e74 6572 3b70 6f73 6974 696f 6e3a  center;position:
 000338f0: 7374 6963 6b79 3b74 6f70 3a30 3b62 6163  sticky;top:0;bac
 00033900: 6b67 726f 756e 643a 7661 7228 2d2d 6275  kground:var(--bu
 00033910: 696c 6465 7253 7562 746c 6548 6967 686c  ilderSubtleHighl
 00033920: 6967 6874 436f 6c6f 7253 6f6c 6964 293b  ightColorSolid);
 00033930: 7a2d 696e 6465 783a 323b 666f 6e74 2d73  z-index:2;font-s
 00033940: 697a 653a 2e38 7265 6d7d 2e77 696e 646f  ize:.8rem}.windo
 00033950: 7742 6172 202e 6963 6f6e 5b64 6174 612d  wBar .icon[data-
-00033960: 762d 3565 3430 3034 6436 5d7b 6d61 7267  v-5e4004d6]{marg
+00033960: 762d 6538 3033 6162 3639 5d7b 6d61 7267  v-e803ab69]{marg
 00033970: 696e 2d72 6967 6874 3a38 7078 3b64 6973  in-right:8px;dis
 00033980: 706c 6179 3a66 6c65 783b 616c 6967 6e2d  play:flex;align-
 00033990: 6974 656d 733a 6365 6e74 6572 7d2e 7769  items:center}.wi
 000339a0: 6e64 6f77 4261 7220 2e74 6974 6c65 5b64  ndowBar .title[d
-000339b0: 6174 612d 762d 3565 3430 3034 6436 5d7b  ata-v-5e4004d6]{
+000339b0: 6174 612d 762d 6538 3033 6162 3639 5d7b  ata-v-e803ab69]{
 000339c0: 666c 6578 3a31 2031 2061 7574 6f3b 6f76  flex:1 1 auto;ov
 000339d0: 6572 666c 6f77 3a68 6964 6465 6e3b 7465  erflow:hidden;te
 000339e0: 7874 2d6f 7665 7266 6c6f 773a 656c 6c69  xt-overflow:elli
 000339f0: 7073 6973 3b77 6869 7465 2d73 7061 6365  psis;white-space
 00033a00: 3a6e 6f77 7261 707d 2e77 696e 646f 7742  :nowrap}.windowB
 00033a10: 6172 202e 7769 6e64 6f77 4163 7469 6f6e  ar .windowAction
-00033a20: 5b64 6174 612d 762d 3565 3430 3034 6436  [data-v-5e4004d6
+00033a20: 5b64 6174 612d 762d 6538 3033 6162 3639  [data-v-e803ab69
 00033a30: 5d7b 6865 6967 6874 3a32 3470 783b 6d69  ]{height:24px;mi
 00033a40: 6e2d 7769 6474 683a 3234 7078 3b70 6164  n-width:24px;pad
 00033a50: 6469 6e67 2d6c 6566 743a 3870 783b 7061  ding-left:8px;pa
 00033a60: 6464 696e 672d 7269 6768 743a 3870 783b  dding-right:8px;
 00033a70: 666c 6578 3a30 2030 2061 7574 6f3b 6469  flex:0 0 auto;di
 00033a80: 7370 6c61 793a 666c 6578 3b62 6f72 6465  splay:flex;borde
 00033a90: 722d 7261 6469 7573 3a31 3270 783b 616c  r-radius:12px;al
@@ -13230,54 +13230,54 @@
 00033ad0: 6e64 3a76 6172 282d 2d62 7569 6c64 6572  nd:var(--builder
 00033ae0: 5375 6274 6c65 4869 6768 6c69 6768 7443  SubtleHighlightC
 00033af0: 6f6c 6f72 293b 6375 7273 6f72 3a70 6f69  olor);cursor:poi
 00033b00: 6e74 6572 3b6d 6172 6769 6e2d 6c65 6674  nter;margin-left
 00033b10: 3a38 7078 3b6f 7574 6c69 6e65 3a6e 6f6e  :8px;outline:non
 00033b20: 657d 2e77 696e 646f 7742 6172 202e 7769  e}.windowBar .wi
 00033b30: 6e64 6f77 4163 7469 6f6e 5b64 6174 612d  ndowAction[data-
-00033b40: 762d 3565 3430 3034 6436 5d3a 666f 6375  v-5e4004d6]:focu
+00033b40: 762d 6538 3033 6162 3639 5d3a 666f 6375  v-e803ab69]:focu
 00033b50: 732c 2e77 696e 646f 7742 6172 202e 7769  s,.windowBar .wi
 00033b60: 6e64 6f77 4163 7469 6f6e 5b64 6174 612d  ndowAction[data-
-00033b70: 762d 3565 3430 3034 6436 5d3a 686f 7665  v-5e4004d6]:hove
+00033b70: 762d 6538 3033 6162 3639 5d3a 686f 7665  v-e803ab69]:hove
 00033b80: 727b 636f 6c6f 723a 7661 7228 2d2d 6275  r{color:var(--bu
 00033b90: 696c 6465 7242 6163 6b67 726f 756e 6443  ilderBackgroundC
 00033ba0: 6f6c 6f72 293b 6261 636b 6772 6f75 6e64  olor);background
 00033bb0: 3a76 6172 282d 2d62 7569 6c64 6572 4163  :var(--builderAc
 00033bc0: 7469 6f6e 4f6e 676f 696e 6743 6f6c 6f72  tionOngoingColor
 00033bd0: 297d 2e73 6563 7469 6f6e 5469 746c 655b  )}.sectionTitle[
-00033be0: 6461 7461 2d76 2d35 6534 3030 3464 365d  data-v-5e4004d6]
+00033be0: 6461 7461 2d76 2d65 3830 3361 6236 395d  data-v-e803ab69]
 00033bf0: 7b64 6973 706c 6179 3a66 6c65 783b 6761  {display:flex;ga
 00033c00: 703a 3870 783b 616c 6967 6e2d 6974 656d  p:8px;align-item
 00033c10: 733a 6365 6e74 6572 7d2e 6669 656c 6457  s:center}.fieldW
-00033c20: 7261 7070 6572 5b64 6174 612d 762d 3565  rapper[data-v-5e
-00033c30: 3430 3034 6436 5d7b 706f 7369 7469 6f6e  4004d6]{position
+00033c20: 7261 7070 6572 5b64 6174 612d 762d 6538  rapper[data-v-e8
+00033c30: 3033 6162 3639 5d7b 706f 7369 7469 6f6e  03ab69]{position
 00033c40: 3a72 656c 6174 6976 653b 7769 6474 683a  :relative;width:
 00033c50: 3130 3025 3b6d 6172 6769 6e2d 746f 703a  100%;margin-top:
 00033c60: 3136 7078 7d3a 6973 282e 6669 656c 6457  16px}:is(.fieldW
 00033c70: 7261 7070 6572 2c2e 6669 656c 6457 7261  rapper,.fieldWra
 00033c80: 7070 6572 4d61 696e 293e 2e6e 616d 655b  pperMain)>.name[
-00033c90: 6461 7461 2d76 2d35 6534 3030 3464 365d  data-v-5e4004d6]
+00033c90: 6461 7461 2d76 2d65 3830 3361 6236 395d  data-v-e803ab69]
 00033ca0: 7b70 6f73 6974 696f 6e3a 6162 736f 6c75  {position:absolu
 00033cb0: 7465 3b74 6f70 3a30 3b6c 6566 743a 3870  te;top:0;left:8p
 00033cc0: 783b 6261 636b 6772 6f75 6e64 3a76 6172  x;background:var
 00033cd0: 282d 2d62 7569 6c64 6572 4261 636b 6772  (--builderBackgr
 00033ce0: 6f75 6e64 436f 6c6f 7229 3b70 6164 6469  oundColor);paddi
 00033cf0: 6e67 3a30 2034 7078 2034 7078 3b66 6f6e  ng:0 4px 4px;fon
 00033d00: 742d 7369 7a65 3a2e 3772 656d 3b7a 2d69  t-size:.7rem;z-i
 00033d10: 6e64 6578 3a31 7d3a 6973 282e 6669 656c  ndex:1}:is(.fiel
 00033d20: 6457 7261 7070 6572 2c2e 6669 656c 6457  dWrapper,.fieldW
 00033d30: 7261 7070 6572 4d61 696e 2920 2e6e 616d  rapperMain) .nam
-00033d40: 6520 2e74 7970 655b 6461 7461 2d76 2d35  e .type[data-v-5
-00033d50: 6534 3030 3464 365d 7b63 6f6c 6f72 3a76  e4004d6]{color:v
+00033d40: 6520 2e74 7970 655b 6461 7461 2d76 2d65  e .type[data-v-e
+00033d50: 3830 3361 6236 395d 7b63 6f6c 6f72 3a76  803ab69]{color:v
 00033d60: 6172 282d 2d62 7569 6c64 6572 5365 636f  ar(--builderSeco
 00033d70: 6e64 6172 7954 6578 7443 6f6c 6f72 297d  ndaryTextColor)}
 00033d80: 3a69 7328 2e66 6965 6c64 5772 6170 7065  :is(.fieldWrappe
 00033d90: 722c 2e66 6965 6c64 5772 6170 7065 724d  r,.fieldWrapperM
 00033da0: 6169 6e29 202e 636f 6e74 656e 745b 6461  ain) .content[da
-00033db0: 7461 2d76 2d35 6534 3030 3464 365d 7b70  ta-v-5e4004d6]{p
+00033db0: 7461 2d76 2d65 3830 3361 6236 395d 7b70  ta-v-e803ab69]{p
 00033dc0: 6f73 6974 696f 6e3a 7265 6c61 7469 7665  osition:relative
 00033dd0: 3b74 6f70 3a36 7078 3b6d 6172 6769 6e2d  ;top:6px;margin-
 00033de0: 626f 7474 6f6d 3a31 3470 783b 7769 6474  bottom:14px;widt
 00033df0: 683a 3130 3025 3b62 6f72 6465 722d 7261  h:100%;border-ra
 00033e00: 6469 7573 3a34 7078 3b62 6f72 6465 723a  dius:4px;border:
 00033e10: 3170 7820 736f 6c69 6420 7661 7228 2d2d  1px solid var(--
 00033e20: 6275 696c 6465 7253 6570 6172 6174 6f72  builderSeparator
@@ -13285,70 +13285,70 @@
 00033e40: 3a2e 3735 7265 6d3b 6261 636b 6772 6f75  :.75rem;backgrou
 00033e50: 6e64 3a76 6172 282d 2d62 7569 6c64 6572  nd:var(--builder
 00033e60: 4261 636b 6772 6f75 6e64 436f 6c6f 7229  BackgroundColor)
 00033e70: 3b6f 7574 6c69 6e65 3a6e 6f6e 657d 3a69  ;outline:none}:i
 00033e80: 7328 2e66 6965 6c64 5772 6170 7065 722c  s(.fieldWrapper,
 00033e90: 2e66 6965 6c64 5772 6170 7065 724d 6169  .fieldWrapperMai
 00033ea0: 6e29 202e 636f 6e74 656e 745b 6461 7461  n) .content[data
-00033eb0: 2d76 2d35 6534 3030 3464 365d 3a66 6f63  -v-5e4004d6]:foc
+00033eb0: 2d76 2d65 3830 3361 6236 395d 3a66 6f63  -v-e803ab69]:foc
 00033ec0: 7573 2d77 6974 6869 6e7b 626f 7264 6572  us-within{border
 00033ed0: 3a31 7078 2073 6f6c 6964 2076 6172 282d  :1px solid var(-
 00033ee0: 2d62 7569 6c64 6572 5072 696d 6172 7954  -builderPrimaryT
 00033ef0: 6578 7443 6f6c 6f72 297d 3a69 7328 2e66  extColor)}:is(.f
 00033f00: 6965 6c64 5772 6170 7065 722c 2e66 6965  ieldWrapper,.fie
 00033f10: 6c64 5772 6170 7065 724d 6169 6e29 202e  ldWrapperMain) .
 00033f20: 636f 6e74 656e 7420 7465 7874 6172 6561  content textarea
-00033f30: 5b64 6174 612d 762d 3565 3430 3034 6436  [data-v-5e4004d6
+00033f30: 5b64 6174 612d 762d 6538 3033 6162 3639  [data-v-e803ab69
 00033f40: 5d2c 3a69 7328 2e66 6965 6c64 5772 6170  ],:is(.fieldWrap
 00033f50: 7065 722c 2e66 6965 6c64 5772 6170 7065  per,.fieldWrappe
 00033f60: 724d 6169 6e29 202e 636f 6e74 656e 7420  rMain) .content 
-00033f70: 696e 7075 745b 6461 7461 2d76 2d35 6534  input[data-v-5e4
-00033f80: 3030 3464 365d 7b62 6f72 6465 723a 303b  004d6]{border:0;
+00033f70: 696e 7075 745b 6461 7461 2d76 2d65 3830  input[data-v-e80
+00033f80: 3361 6236 395d 7b62 6f72 6465 723a 303b  3ab69]{border:0;
 00033f90: 6f75 746c 696e 653a 6e6f 6e65 3b77 6964  outline:none;wid
 00033fa0: 7468 3a31 3030 257d 2e66 6965 6c64 5772  th:100%}.fieldWr
 00033fb0: 6170 7065 723e 2e64 6573 635b 6461 7461  apper>.desc[data
-00033fc0: 2d76 2d35 6534 3030 3464 365d 7b63 6f6c  -v-5e4004d6]{col
+00033fc0: 2d76 2d65 3830 3361 6236 395d 7b63 6f6c  -v-e803ab69]{col
 00033fd0: 6f72 3a76 6172 282d 2d62 7569 6c64 6572  or:var(--builder
 00033fe0: 5365 636f 6e64 6172 7954 6578 7443 6f6c  SecondaryTextCol
 00033ff0: 6f72 293b 666f 6e74 2d73 697a 653a 2e37  or);font-size:.7
 00034000: 7265 6d7d 2e63 6869 7053 7461 636b 5b64  rem}.chipStack[d
-00034010: 6174 612d 762d 3565 3430 3034 6436 5d7b  ata-v-5e4004d6]{
+00034010: 6174 612d 762d 6538 3033 6162 3639 5d7b  ata-v-e803ab69]{
 00034020: 6469 7370 6c61 793a 666c 6578 3b66 6c65  display:flex;fle
 00034030: 782d 6469 7265 6374 696f 6e3a 726f 773b  x-direction:row;
 00034040: 666c 6578 2d77 7261 703a 7772 6170 3b67  flex-wrap:wrap;g
 00034050: 6170 3a34 7078 7d2e 6368 6970 5b64 6174  ap:4px}.chip[dat
-00034060: 612d 762d 3565 3430 3034 6436 5d7b 666f  a-v-5e4004d6]{fo
+00034060: 612d 762d 6538 3033 6162 3639 5d7b 666f  a-v-e803ab69]{fo
 00034070: 6e74 2d73 697a 653a 2e37 3572 656d 3b62  nt-size:.75rem;b
 00034080: 6f72 6465 722d 7261 6469 7573 3a31 3670  order-radius:16p
 00034090: 783b 7061 6464 696e 673a 3870 7820 3132  x;padding:8px 12
 000340a0: 7078 3b63 7572 736f 723a 706f 696e 7465  px;cursor:pointe
 000340b0: 723b 6f75 746c 696e 653a 6e6f 6e65 3b62  r;outline:none;b
 000340c0: 6163 6b67 726f 756e 643a 7661 7228 2d2d  ackground:var(--
 000340d0: 6275 696c 6465 7242 6163 6b67 726f 756e  builderBackgroun
 000340e0: 6443 6f6c 6f72 297d 2e63 6869 705b 6461  dColor)}.chip[da
-000340f0: 7461 2d76 2d35 6534 3030 3464 365d 3a66  ta-v-5e4004d6]:f
+000340f0: 7461 2d76 2d65 3830 3361 6236 395d 3a66  ta-v-e803ab69]:f
 00034100: 6f63 7573 2c2e 6368 6970 2e61 6374 6976  ocus,.chip.activ
-00034110: 655b 6461 7461 2d76 2d35 6534 3030 3464  e[data-v-5e4004d
-00034120: 365d 3a66 6f63 7573 2c2e 6368 6970 5b64  6]:focus,.chip[d
-00034130: 6174 612d 762d 3565 3430 3034 6436 5d3a  ata-v-5e4004d6]:
+00034110: 655b 6461 7461 2d76 2d65 3830 3361 6236  e[data-v-e803ab6
+00034120: 395d 3a66 6f63 7573 2c2e 6368 6970 5b64  9]:focus,.chip[d
+00034130: 6174 612d 762d 6538 3033 6162 3639 5d3a  ata-v-e803ab69]:
 00034140: 686f 7665 722c 2e63 6869 702e 6163 7469  hover,.chip.acti
-00034150: 7665 5b64 6174 612d 762d 3565 3430 3034  ve[data-v-5e4004
-00034160: 6436 5d3a 686f 7665 727b 636f 6c6f 723a  d6]:hover{color:
+00034150: 7665 5b64 6174 612d 762d 6538 3033 6162  ve[data-v-e803ab
+00034160: 3639 5d3a 686f 7665 727b 636f 6c6f 723a  69]:hover{color:
 00034170: 7661 7228 2d2d 6275 696c 6465 7242 6163  var(--builderBac
 00034180: 6b67 726f 756e 6443 6f6c 6f72 293b 6261  kgroundColor);ba
 00034190: 636b 6772 6f75 6e64 3a76 6172 282d 2d62  ckground:var(--b
 000341a0: 7569 6c64 6572 4163 7469 6f6e 4f6e 676f  uilderActionOngo
 000341b0: 696e 6743 6f6c 6f72 297d 2e63 6869 702e  ingColor)}.chip.
-000341c0: 6163 7469 7665 5b64 6174 612d 762d 3565  active[data-v-5e
-000341d0: 3430 3034 6436 5d7b 6261 636b 6772 6f75  4004d6]{backgrou
+000341c0: 6163 7469 7665 5b64 6174 612d 762d 6538  active[data-v-e8
+000341d0: 3033 6162 3639 5d7b 6261 636b 6772 6f75  03ab69]{backgrou
 000341e0: 6e64 3a76 6172 282d 2d62 7569 6c64 6572  nd:var(--builder
 000341f0: 5375 6274 6c65 5365 7061 7261 746f 7243  SubtleSeparatorC
 00034200: 6f6c 6f72 297d 2e63 6f75 6e74 4c61 6265  olor)}.countLabe
-00034210: 6c5b 6461 7461 2d76 2d35 6534 3030 3464  l[data-v-5e4004d
-00034220: 365d 7b62 6163 6b67 726f 756e 643a 7661  6]{background:va
+00034210: 6c5b 6461 7461 2d76 2d65 3830 3361 6236  l[data-v-e803ab6
+00034220: 395d 7b62 6163 6b67 726f 756e 643a 7661  9]{background:va
 00034230: 7228 2d2d 6275 696c 6465 7249 6e74 656e  r(--builderInten
 00034240: 7365 5365 6c65 6374 6564 436f 6c6f 7229  seSelectedColor)
 00034250: 3b64 6973 706c 6179 3a69 6e6c 696e 652d  ;display:inline-
 00034260: 666c 6578 3b63 6f6c 6f72 3a76 6172 282d  flex;color:var(-
 00034270: 2d62 7569 6c64 6572 4261 636b 6772 6f75  -builderBackgrou
 00034280: 6e64 436f 6c6f 7229 3b61 6c69 676e 2d69  ndColor);align-i
 00034290: 7465 6d73 3a63 656e 7465 723b 6a75 7374  tems:center;just
@@ -13357,90 +13357,90 @@
 000342c0: 3470 783b 7061 6464 696e 672d 7269 6768  4px;padding-righ
 000342d0: 743a 3470 783b 6d69 6e2d 7769 6474 683a  t:4px;min-width:
 000342e0: 3230 7078 3b68 6569 6768 743a 3230 7078  20px;height:20px
 000342f0: 3b62 6f72 6465 722d 7261 6469 7573 3a31  ;border-radius:1
 00034300: 3070 783b 6d61 7267 696e 2d6c 6566 743a  0px;margin-left:
 00034310: 3870 783b 666f 6e74 2d73 697a 653a 2e37  8px;font-size:.7
 00034320: 7265 6d7d 2e42 7569 6c64 6572 5365 7474  rem}.BuilderSett
-00034330: 696e 6773 5b64 6174 612d 762d 3565 3430  ings[data-v-5e40
-00034340: 3034 6436 5d7b 666f 6e74 2d73 697a 653a  04d6]{font-size:
+00034330: 696e 6773 5b64 6174 612d 762d 6538 3033  ings[data-v-e803
+00034340: 6162 3639 5d7b 666f 6e74 2d73 697a 653a  ab69]{font-size:
 00034350: 2e37 7265 6d3b 6261 636b 6772 6f75 6e64  .7rem;background
 00034360: 3a76 6172 282d 2d62 7569 6c64 6572 4261  :var(--builderBa
 00034370: 636b 6772 6f75 6e64 436f 6c6f 7229 7d2e  ckgroundColor)}.
-00034380: 646f 6373 5b64 6174 612d 762d 3565 3430  docs[data-v-5e40
-00034390: 3034 6436 5d7b 666f 6e74 2d73 697a 653a  04d6]{font-size:
+00034380: 646f 6373 5b64 6174 612d 762d 6538 3033  docs[data-v-e803
+00034390: 6162 3639 5d7b 666f 6e74 2d73 697a 653a  ab69]{font-size:
 000343a0: 2e37 3572 656d 3b70 6164 6469 6e67 3a32  .75rem;padding:2
 000343b0: 3470 783b 6c69 6e65 2d68 6569 6768 743a  4px;line-height:
 000343c0: 312e 353b 6261 636b 6772 6f75 6e64 3a76  1.5;background:v
 000343d0: 6172 282d 2d62 7569 6c64 6572 5375 6274  ar(--builderSubt
 000343e0: 6c65 4869 6768 6c69 6768 7443 6f6c 6f72  leHighlightColor
 000343f0: 536f 6c69 6429 3b62 6f72 6465 722d 746f  Solid);border-to
 00034400: 703a 3170 7820 736f 6c69 6420 7661 7228  p:1px solid var(
 00034410: 2d2d 6275 696c 6465 7253 7562 746c 6553  --builderSubtleS
 00034420: 6570 6172 6174 6f72 436f 6c6f 7229 3b77  eparatorColor);w
 00034430: 6869 7465 2d73 7061 6365 3a70 7265 2d77  hite-space:pre-w
 00034440: 7261 707d 2e64 6f63 7320 6469 765b 6461  rap}.docs div[da
-00034450: 7461 2d76 2d35 6534 3030 3464 365d 3a6e  ta-v-5e4004d6]:n
+00034450: 7461 2d76 2d65 3830 3361 6236 395d 3a6e  ta-v-e803ab69]:n
 00034460: 6f74 283a 6669 7273 742d 6368 696c 6429  ot(:first-child)
 00034470: 7b6d 6172 6769 6e2d 746f 703a 3136 7078  {margin-top:16px
 00034480: 3b62 6f72 6465 722d 746f 703a 3170 7820  ;border-top:1px 
 00034490: 736f 6c69 6420 7661 7228 2d2d 6275 696c  solid var(--buil
 000344a0: 6465 7253 7562 746c 6553 6570 6172 6174  derSubtleSeparat
 000344b0: 6f72 436f 6c6f 7229 3b70 6164 6469 6e67  orColor);padding
 000344c0: 2d74 6f70 3a31 3670 787d 2e73 6563 7469  -top:16px}.secti
-000344d0: 6f6e 735b 6461 7461 2d76 2d35 6534 3030  ons[data-v-5e400
-000344e0: 3464 365d 7b62 6163 6b67 726f 756e 643a  4d6]{background:
+000344d0: 6f6e 735b 6461 7461 2d76 2d65 3830 3361  ons[data-v-e803a
+000344e0: 6236 395d 7b62 6163 6b67 726f 756e 643a  b69]{background:
 000344f0: 7661 7228 2d2d 6275 696c 6465 7242 6163  var(--builderBac
 00034500: 6b67 726f 756e 6443 6f6c 6f72 297d 2e73  kgroundColor)}.s
 00034510: 6563 7469 6f6e 735b 696e 6572 745d 5b64  ections[inert][d
-00034520: 6174 612d 762d 3565 3430 3034 6436 5d7b  ata-v-5e4004d6]{
+00034520: 6174 612d 762d 6538 3033 6162 3639 5d7b  ata-v-e803ab69]{
 00034530: 6f70 6163 6974 793a 2e37 7d2e 7365 6374  opacity:.7}.sect
-00034540: 696f 6e73 3e2a 5b64 6174 612d 762d 3565  ions>*[data-v-5e
-00034550: 3430 3034 6436 5d3a 6e6f 7428 3a66 6972  4004d6]:not(:fir
+00034540: 696f 6e73 3e2a 5b64 6174 612d 762d 6538  ions>*[data-v-e8
+00034550: 3033 6162 3639 5d3a 6e6f 7428 3a66 6972  03ab69]:not(:fir
 00034560: 7374 2d63 6869 6c64 297b 626f 7264 6572  st-child){border
 00034570: 2d74 6f70 3a31 7078 2073 6f6c 6964 2076  -top:1px solid v
 00034580: 6172 282d 2d62 7569 6c64 6572 5365 7061  ar(--builderSepa
 00034590: 7261 746f 7243 6f6c 6f72 297d 2e64 6562  ratorColor)}.deb
-000345a0: 7567 5b64 6174 612d 762d 3565 3430 3034  ug[data-v-5e4004
-000345b0: 6436 5d7b 636f 6c6f 723a 7661 7228 2d2d  d6]{color:var(--
+000345a0: 7567 5b64 6174 612d 762d 6538 3033 6162  ug[data-v-e803ab
+000345b0: 3639 5d7b 636f 6c6f 723a 7661 7228 2d2d  69]{color:var(--
 000345c0: 6275 696c 6465 7253 6563 6f6e 6461 7279  builderSecondary
 000345d0: 5465 7874 436f 6c6f 7229 3b62 6f72 6465  TextColor);borde
 000345e0: 722d 746f 703a 3170 7820 736f 6c69 6420  r-top:1px solid 
 000345f0: 7661 7228 2d2d 6275 696c 6465 7253 6570  var(--builderSep
 00034600: 6172 6174 6f72 436f 6c6f 7229 3b70 6164  aratorColor);pad
 00034610: 6469 6e67 3a32 3470 787d 2e77 6172 6e69  ding:24px}.warni
-00034620: 6e67 5b64 6174 612d 762d 3565 3430 3034  ng[data-v-5e4004
-00034630: 6436 5d7b 6469 7370 6c61 793a 666c 6578  d6]{display:flex
+00034620: 6e67 5b64 6174 612d 762d 6538 3033 6162  ng[data-v-e803ab
+00034630: 3639 5d7b 6469 7370 6c61 793a 666c 6578  69]{display:flex
 00034640: 3b61 6c69 676e 2d69 7465 6d73 3a63 656e  ;align-items:cen
 00034650: 7465 723b 6261 636b 6772 6f75 6e64 3a76  ter;background:v
 00034660: 6172 282d 2d62 7569 6c64 6572 5761 726e  ar(--builderWarn
 00034670: 696e 6743 6f6c 6f72 293b 636f 6c6f 723a  ingColor);color:
 00034680: 7661 7228 2d2d 6275 696c 6465 7257 6172  var(--builderWar
 00034690: 6e69 6e67 5465 7874 436f 6c6f 7229 3b62  ningTextColor);b
 000346a0: 6f72 6465 722d 7261 6469 7573 3a34 7078  order-radius:4px
 000346b0: 3b67 6170 3a31 3270 783b 6d61 7267 696e  ;gap:12px;margin
 000346c0: 3a31 3270 7820 3132 7078 2030 3b70 6164  :12px 12px 0;pad
 000346d0: 6469 6e67 3a31 3270 787d 2e6d 6172 6b64  ding:12px}.markd
-000346e0: 6f77 6e5b 6461 7461 2d76 2d35 6534 3030  own[data-v-5e400
-000346f0: 3464 365d 2070 7265 7b62 6163 6b67 726f  4d6] pre{backgro
+000346e0: 6f77 6e5b 6461 7461 2d76 2d65 3830 3361  own[data-v-e803a
+000346f0: 6236 395d 2070 7265 7b62 6163 6b67 726f  b69] pre{backgro
 00034700: 756e 642d 636f 6c6f 723a 7661 7228 2d2d  und-color:var(--
 00034710: 6275 696c 6465 7253 7562 746c 6553 6570  builderSubtleSep
 00034720: 6172 6174 6f72 436f 6c6f 7229 3b66 6f6e  aratorColor);fon
 00034730: 742d 6661 6d69 6c79 3a6d 6f6e 6f73 7061  t-family:monospa
 00034740: 6365 3b70 6164 6469 6e67 3a38 7078 3b62  ce;padding:8px;b
 00034750: 6f72 6465 722d 7261 6469 7573 3a34 7078  order-radius:4px
 00034760: 7d2e 6d61 726b 646f 776e 5b64 6174 612d  }.markdown[data-
-00034770: 762d 3565 3430 3034 6436 5d20 636f 6465  v-5e4004d6] code
+00034770: 762d 6538 3033 6162 3639 5d20 636f 6465  v-e803ab69] code
 00034780: 7b62 6163 6b67 726f 756e 642d 636f 6c6f  {background-colo
 00034790: 723a 7661 7228 2d2d 6275 696c 6465 7253  r:var(--builderS
 000347a0: 7562 746c 6553 6570 6172 6174 6f72 436f  ubtleSeparatorCo
 000347b0: 6c6f 7229 3b66 6f6e 742d 6661 6d69 6c79  lor);font-family
 000347c0: 3a6d 6f6e 6f73 7061 6365 3b70 6164 6469  :monospace;paddi
 000347d0: 6e67 3a32 7078 7d2e 6d61 726b 646f 776e  ng:2px}.markdown
-000347e0: 5b64 6174 612d 762d 3565 3430 3034 6436  [data-v-5e4004d6
+000347e0: 5b64 6174 612d 762d 6538 3033 6162 3639  [data-v-e803ab69
 000347f0: 5d20 7072 653e 636f 6465 7b62 6163 6b67  ] pre>code{backg
 00034800: 726f 756e 642d 636f 6c6f 723a 756e 7365  round-color:unse
 00034810: 747d 4066 6f6e 742d 6661 6365 7b66 6f6e  t}@font-face{fon
 00034820: 742d 6661 6d69 6c79 3a49 6e74 6572 3b73  t-family:Inter;s
 00034830: 7263 3a75 726c 282e 2f49 6e74 6572 2d52  rc:url(./Inter-R
 00034840: 6567 756c 6172 2d64 3631 3266 3132 312e  egular-d612f121.
 00034850: 776f 6666 3229 2066 6f72 6d61 7428 2277  woff2) format("w
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/ComponentRenderer-82ebfa88.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/ComponentRenderer-007280fe.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -25,17 +25,17 @@
     s as he,
     n as J,
     p as Z,
     j as ee,
     z as ye,
     u as q,
     l as Ce,
-    q as Ie,
-    R as be
-} from "./index-b222671e.js";
+    q as be,
+    R as Ie
+} from "./index-0d669be8.js";
 const Pe = {
         class: "ChildlessPlaceholder"
     },
     $e = {
         class: "content"
     },
     Ee = {
@@ -56,23 +56,23 @@
                 _ = d,
                 {
                     componentId: l
                 } = pe(_),
                 s = m(() => n.getComponentById(l.value)),
                 T = m(() => n.getComponentDefinition(s.value.type)),
                 r = (h, y) => {
-                    const c = h.map(I => n.getComponentDefinition(I)).map(I => I == null ? void 0 : I.name);
+                    const c = h.map(b => n.getComponentDefinition(b)).map(b => b == null ? void 0 : b.name);
                     return `${c.slice(0,-1).join(", ")} ${c.length>1?y:""} ${c.at(-1)}`
                 },
-                b = m(() => {
+                I = m(() => {
                     const h = n.getContainableTypes(l.value);
                     let y;
                     return h.length <= Te && (y = `You can add ${r(h,"and")} components`), y
                 });
-            return (h, y) => (S(), x("div", Pe, [o("div", $e, [o("div", Ee, [o("h2", null, "Empty " + E(T.value.name), 1)]), b.value ? (S(), x("div", Se, E(b.value), 1)) : G("", !0)])]))
+            return (h, y) => (S(), x("div", Pe, [o("div", $e, [o("div", Ee, [o("h2", null, "Empty " + E(T.value.name), 1)]), I.value ? (S(), x("div", Se, E(I.value), 1)) : G("", !0)])]))
         }
     });
 const Me = F(xe, [
         ["__scopeId", "data-v-7f547886"]
     ]),
     Be = {
         class: "RenderError"
@@ -99,53 +99,53 @@
         setup(d) {
             const n = w(g.core),
                 _ = w(g.builderManager),
                 l = d.componentId,
                 s = m(() => n.getComponentById(l)),
                 T = _e(s.value.type),
                 r = d.instancePath,
-                b = d.instanceData,
+                I = d.instanceData,
                 {
                     getEvaluatedFields: h,
                     isComponentVisible: y
                 } = Q(n),
                 e = h(r),
                 c = m(() => n.getComponents(l, {
                     sortedByPosition: !0
                 })),
                 i = m(() => !!_ && _.getMode() != "preview"),
-                I = m(() => i.value && !s.value.isCodeManaged && s.value.type !== "root"),
+                b = m(() => i.value && !s.value.isCodeManaged && s.value.type !== "root"),
                 M = D(!1),
                 V = m(() => n.getUserFunctions()),
                 se = () => {
                     if (!(c.value.length > 0)) return B(Me, {
                         componentId: s.value.id
                     })
                 },
                 L = (t, a = 0) => B(te, {
                     componentId: t,
                     key: `${t}:${a}`,
                     instancePath: [...r, {
                         componentId: t,
                         instanceNumber: a
                     }],
-                    instanceData: [...b, D(null)]
+                    instanceData: [...I, D(null)]
                 }),
                 K = (t = 0, a = () => !0, v = !1) => {
                     const u = f => !i.value || v ? [] : [B("div", {
                             "data-streamsync-slot-of-id": l,
                             "data-streamsync-position": f
                         })],
                         p = c.value.filter(a),
                         C = p.filter(f => !f.isCodeManaged).map(f => L(f.id, t)),
                         P = p.filter(f => f.isCodeManaged).map(f => L(f.id, t));
                     return [...u(0), ...C.map((f, R) => [f, u(R + 1)]).flat(), ...P]
                 },
                 W = (t => t.map(a => `${a.componentId}:${a.instanceNumber}`).join(","))(r);
-            $(g.evaluatedFields, e), $(g.componentId, l), $(g.isBeingEdited, i), $(g.isDisabled, M), $(g.instancePath, r), $(g.instanceData, b), $(g.renderProxiedComponent, L), $(g.getChildrenVNodes, K), $(g.flattenedInstancePath, W);
+            $(g.evaluatedFields, e), $(g.componentId, l), $(g.isBeingEdited, i), $(g.isDisabled, M), $(g.instancePath, r), $(g.instanceData, I), $(g.renderProxiedComponent, L), $(g.getChildrenVNodes, K), $(g.flattenedInstancePath, W);
             const ne = {
                     "data-streamsync-id": l,
                     "data-streamsync-instance-path": W
                 },
                 N = D(!1);
             j(() => (_ == null ? void 0 : _.getSelectedId()) == l, t => {
                 N.value = t
@@ -203,14 +203,15 @@
                     return u.forEach(P => {
                         p[P] = !0
                     }), p
                 }),
                 ie = function() {
                     return {
                         class: {
+                            [`ss-type-${s.value.type}`]: !0,
                             component: !0,
                             childless: z.value,
                             selected: N.value,
                             disabled: M.value,
                             beingEdited: i.value,
                             ...re.value
                         },
@@ -218,15 +219,15 @@
                             ...ce.value,
                             ...oe.value ? {} : {
                                 display: "none"
                             }
                         },
                         ...ne,
                         ...M.value ? [] : le.value,
-                        draggable: I.value
+                        draggable: b.value
                     }
                 },
                 de = () => (s.value.parentId ? n.getContainableTypes(s.value.parentId) : ["root"]).includes(s.value.type),
                 ue = (t, a) => i.value ? B(Ve, {
                     ...t,
                     componentType: s.value.type,
                     message: a
@@ -244,15 +245,15 @@
                 return de() ? B(T, v, {
                     default: a
                 }) : ue(v, "Parent is not suitable for this component")
             }
         }
     };
 const te = F(Re, [
-        ["__scopeId", "data-v-f812114a"]
+        ["__scopeId", "data-v-a731db34"]
     ]),
     k = d => (Z("data-v-54d2c60b"), d = d(), ee(), d),
     Ae = k(() => o("i", {
         class: "ri-notification-2-line ri-xl"
     }, null, -1)),
     Fe = {
         class: "counter"
@@ -307,29 +308,29 @@
                 };
             me(() => {
                 n.addMailSubscription("notification", T)
             });
             const r = () => {
                     s.length != 0 && (_.value = !_.value)
                 },
-                b = () => {
+                I = () => {
                     s.splice(0), _.value = !1
                 };
             return (h, y) => X((S(), x("div", {
                 class: "RendererNotifications",
                 onClick: r
             }, [o("div", {
                 ref_key: "balloon",
                 ref: l,
                 class: "balloon",
                 title: "Toggle notifications"
             }, [Ae, o("div", Fe, E(s.length), 1)], 512), ke, X(o("div", Le, [o("div", {
                 class: "clearContainer"
             }, [o("button", {
-                onClick: b
+                onClick: I
             }, [Ne, fe(" Clear all ")])]), (S(!0), x(ge, null, he(s, (e, c) => (S(), x("div", {
                 key: c,
                 class: "notification"
             }, [o("div", {
                 class: J(["icon", e.type])
             }, Ke, 2), o("div", We, [o("header", null, [o("strong", ze, E(e.title), 1), o("span", He, E(e.timestampReceived.toLocaleTimeString()), 1)]), o("div", Oe, E(e.message), 1)])]))), 128))], 512), [
                 [Y, _.value]
@@ -357,21 +358,21 @@
             l || console.error("No root component found.");
             const s = [{
                     componentId: "root",
                     instanceNumber: 0
                 }],
                 T = [D(null)],
                 r = _.getEvaluatedFields(s),
-                b = m(() => {
-                    var e, c, i, I, M, V;
+                I = m(() => {
+                    var e, c, i, b, M, V;
                     return {
                         "--accentColor": (e = r.accentColor) == null ? void 0 : e.value,
                         "--emptinessColor": (c = r.emptinessColor) == null ? void 0 : c.value,
                         "--containerBackgroundColor": (i = r.parentIdBackgroundColor) == null ? void 0 : i.value,
-                        "--primaryTextColor": (I = r.primaryTextColor) == null ? void 0 : I.value,
+                        "--primaryTextColor": (b = r.primaryTextColor) == null ? void 0 : b.value,
                         "--secondaryTextColor": (M = r.secondaryTextColor) == null ? void 0 : M.value,
                         "--separatorColor": (V = r.separatorColor) == null ? void 0 : V.value
                     }
                 }),
                 h = m(() => n.getFrontendMessageMap().size > 0);
             j(() => {
                 var e;
@@ -388,23 +389,23 @@
                 e && c == "edit" ? i = `${e} | Streamsync Builder` : !e && c == "edit" ? i = "Streamsync Builder" : e && c == "run" ? i = `${e}` : !e && c == "run" && (i = "Streamsync App"), document.title = i
             }
             return (e, c) => (S(), x("main", {
                 class: J(["ComponentRenderer", {
                     loadingActive: h.value
                 }]),
                 tabindex: "-1",
-                style: be(b.value)
+                style: Ie(I.value)
             }, [ye(Ye, {
                 class: "notifications"
             }), Ge, o("div", Qe, [q(l) ? (S(), Ce(te, {
                 key: 0,
                 "component-id": q(l).id,
                 "instance-path": s,
                 "instance-data": T
-            }, null, 8, ["component-id"])) : G("", !0), Ie(e.$slots, "default", {}, void 0, !0)])], 6))
+            }, null, 8, ["component-id"])) : G("", !0), be(e.$slots, "default", {}, void 0, !0)])], 6))
         }
     });
 const tt = F(Je, [
     ["__scopeId", "data-v-7f4207e0"]
 ]);
 export {
     tt as
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/ComponentRenderer-a2494844.css` & `streamsync-0.4.0rc4/src/streamsync/static/assets/ComponentRenderer-08d5f1dc.css`

 * *Files 8% similar despite different names*

```diff
@@ -1 +1 @@
-@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-7f547886],button[data-v-7f547886],textarea[data-v-7f547886],select[data-v-7f547886]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-7f547886]:focus,textarea[data-v-7f547886]:focus,select[data-v-7f547886]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-7f547886],h2[data-v-7f547886],h3[data-v-7f547886],h4[data-v-7f547886]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-7f547886]{font-size:1.3rem}h2[data-v-7f547886]{font-size:1rem}h3[data-v-7f547886]{font-size:.9rem}h4[data-v-7f547886]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-7f547886],ol[data-v-7f547886]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-7f547886]{margin:0 0 0 32px}hr[data-v-7f547886]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-7f547886]{color:var(--primaryTextColor)}code[data-v-7f547886]{background-color:var(--separatorColor)}button[data-v-7f547886]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-7f547886]:focus,button[data-v-7f547886]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-7f547886]{font-size:.8rem}.component.selected[data-v-7f547886]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-7f547886]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-7f547886]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-7f547886]{display:flex;gap:16px}[data-streamsync-container][data-v-7f547886]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-7f547886]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-7f547886]{animation:appearVertical-7f547886 .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-7f547886]{animation:appearHorizontal-7f547886 .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-7f547886{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-7f547886{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.ChildlessPlaceholder[data-v-7f547886]{background:rgba(0,0,0,.05);color:var(--primaryTextColor);padding:16px;display:flex;align-items:center;justify-content:center;width:100%;min-height:100%}.content[data-v-7f547886]{text-align:center}.title>h2[data-v-7f547886]{color:var(--primaryTextColor);opacity:.8}.message[data-v-7f547886]{opacity:.5;margin-top:8px}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-f812114a],button[data-v-f812114a],textarea[data-v-f812114a],select[data-v-f812114a]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-f812114a]:focus,textarea[data-v-f812114a]:focus,select[data-v-f812114a]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-f812114a],h2[data-v-f812114a],h3[data-v-f812114a],h4[data-v-f812114a]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-f812114a]{font-size:1.3rem}h2[data-v-f812114a]{font-size:1rem}h3[data-v-f812114a]{font-size:.9rem}h4[data-v-f812114a]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-f812114a],ol[data-v-f812114a]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-f812114a]{margin:0 0 0 32px}hr[data-v-f812114a]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-f812114a]{color:var(--primaryTextColor)}code[data-v-f812114a]{background-color:var(--separatorColor)}button[data-v-f812114a]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-f812114a]:focus,button[data-v-f812114a]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-f812114a]{font-size:.8rem}.component.selected[data-v-f812114a]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-f812114a]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-f812114a]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-f812114a]{display:flex;gap:16px}[data-streamsync-container][data-v-f812114a]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-f812114a]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-f812114a]{animation:appearVertical-f812114a .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-f812114a]{animation:appearHorizontal-f812114a .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-f812114a{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-f812114a{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-54d2c60b],button[data-v-54d2c60b],textarea[data-v-54d2c60b],select[data-v-54d2c60b]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-54d2c60b]:focus,textarea[data-v-54d2c60b]:focus,select[data-v-54d2c60b]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-54d2c60b],h2[data-v-54d2c60b],h3[data-v-54d2c60b],h4[data-v-54d2c60b]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-54d2c60b]{font-size:1.3rem}h2[data-v-54d2c60b]{font-size:1rem}h3[data-v-54d2c60b]{font-size:.9rem}h4[data-v-54d2c60b]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-54d2c60b],ol[data-v-54d2c60b]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-54d2c60b]{margin:0 0 0 32px}hr[data-v-54d2c60b]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-54d2c60b]{color:var(--primaryTextColor)}code[data-v-54d2c60b]{background-color:var(--separatorColor)}button[data-v-54d2c60b]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-54d2c60b]:focus,button[data-v-54d2c60b]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-54d2c60b]{font-size:.8rem}.component.selected[data-v-54d2c60b]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-54d2c60b]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-54d2c60b]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-54d2c60b]{display:flex;gap:16px}[data-streamsync-container][data-v-54d2c60b]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-54d2c60b]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-54d2c60b]{animation:appearVertical-54d2c60b .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-54d2c60b]{animation:appearHorizontal-54d2c60b .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-54d2c60b{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-54d2c60b{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.RendererNotifications[data-v-54d2c60b]{position:sticky;top:24px;margin-left:auto;margin-right:24px;max-width:70ch;width:40vw;z-index:3}.balloonFlash[data-v-54d2c60b]{right:0;position:absolute;opacity:.8;background:var(--accentColor);width:52px;height:52px;border-radius:50%}.balloon.alert+.balloonFlash[data-v-54d2c60b]{animation-name:alert-54d2c60b;animation-duration:1s;animation-timing-function:ease-in-out}.balloon[data-v-54d2c60b]{z-index:2;position:absolute;-webkit-user-select:none;user-select:none;right:0;font-size:.7rem;border-radius:50%;background:var(--accentColor);width:52px;height:52px;color:var(--emptinessColor);display:flex;align-items:center;justify-content:center;cursor:pointer;box-shadow:0 0 8px 2px #0003;flex-direction:column}.balloon.alert i[data-v-54d2c60b]{animation-name:ring-54d2c60b;animation-duration:.3s;animation-iteration-count:4;animation-timing-function:ease-in-out}.balloon .counter[data-v-54d2c60b]{position:absolute;top:40px;right:0;background:var(--containerBackgroundColor);padding:4px 8px;border-radius:16px;color:var(--primaryTextColor);border:1px solid var(--separatorColor)}@keyframes alert-54d2c60b{0%{transform:scale(1)}50%{transform:scale(1.7)}to{transform:scale(1)}}@keyframes ring-54d2c60b{0%{transform:rotate(0)}25%{transform:rotate(-25deg)}75%{transform:rotate(25deg)}to{transform:rotate(0)}}.main[data-v-54d2c60b]{position:absolute;max-height:75vh;overflow-y:auto;overflow-x:hidden;right:0;width:100%;max-width:100%;top:72px;color:var(--primaryTextColor);background:var(--containerBackgroundColor);border-radius:8px;box-shadow:0 0 8px #0003}.clearContainer[data-v-54d2c60b]{padding:16px}.clearContainer button[data-v-54d2c60b]{margin-left:auto;margin-right:0}.notification[data-v-54d2c60b]{border-top:1px solid var(--separatorColor);padding:16px 16px 16px 0;font-size:.8rem;display:grid;grid-template-rows:1fr;grid-template-columns:72px 1fr;align-items:center}.notification .icon[data-v-54d2c60b]{grid-area:1/1;text-align:center}.notification .icon.error[data-v-54d2c60b]{color:#fb0000}.notification .icon.warning[data-v-54d2c60b]{color:#fb9600}.notification .icon.info[data-v-54d2c60b]{color:#00adb8}.notification .icon.success[data-v-54d2c60b]{color:#00b800}.notification .content[data-v-54d2c60b]{grid-area:1/2;max-width:100%;overflow:hidden}.notification header[data-v-54d2c60b]{display:flex}.notification header .title[data-v-54d2c60b]{flex:1 0 auto}.notification header .time[data-v-54d2c60b]{flex:0 0 auto;color:var(--secondaryTextColor)}.message[data-v-54d2c60b]{margin-top:12px}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-7f4207e0],button[data-v-7f4207e0],textarea[data-v-7f4207e0],select[data-v-7f4207e0]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-7f4207e0]:focus,textarea[data-v-7f4207e0]:focus,select[data-v-7f4207e0]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-7f4207e0],h2[data-v-7f4207e0],h3[data-v-7f4207e0],h4[data-v-7f4207e0]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-7f4207e0]{font-size:1.3rem}h2[data-v-7f4207e0]{font-size:1rem}h3[data-v-7f4207e0]{font-size:.9rem}h4[data-v-7f4207e0]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-7f4207e0],ol[data-v-7f4207e0]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-7f4207e0]{margin:0 0 0 32px}hr[data-v-7f4207e0]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-7f4207e0]{color:var(--primaryTextColor)}code[data-v-7f4207e0]{background-color:var(--separatorColor)}button[data-v-7f4207e0]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-7f4207e0]:focus,button[data-v-7f4207e0]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-7f4207e0]{font-size:.8rem}.component.selected[data-v-7f4207e0]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-7f4207e0]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-7f4207e0]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-7f4207e0]{display:flex;gap:16px}[data-streamsync-container][data-v-7f4207e0]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-7f4207e0]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-7f4207e0]{animation:appearVertical-7f4207e0 .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-7f4207e0]{animation:appearHorizontal-7f4207e0 .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-7f4207e0{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-7f4207e0{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.ComponentRenderer[data-v-7f4207e0]{--accentColor: #29cf00;--buttonColor: #ffffff;--emptinessColor: #e9eef1;--separatorColor: rgba(0, 0, 0, .07);--primaryTextColor: #202829;--buttonTextColor: #202829;--secondaryTextColor: #5d7275;--containerBackgroundColor: #ffffff;width:100%;outline:none;--notificationsDisplacement: 0;font-family:Inter,sans-serif;font-size:.8rem;color:var(--primaryTextColor);background:var(--emptinessColor);display:flex;flex-direction:column;min-height:100%;isolation:isolate;flex:1 0 auto}.notifications[data-v-7f4207e0]{right:var(--notificationsDisplacement)}.loadingBar[data-v-7f4207e0]{width:100%;height:4px;margin-bottom:-4px;position:sticky;top:0;pointer-events:none;z-index:4;transition-delay:.2s;transition-property:opacity;transition-duration:.2s;opacity:0}.loadingActive .loadingBar[data-v-7f4207e0]{background-size:200% 200%;opacity:1;animation:loadingAnimation-7f4207e0 ease-in-out 1s infinite;animation-delay:.2s;background-image:linear-gradient(270deg,var(--emptinessColor),var(--accentColor),var(--emptinessColor))}@keyframes loadingAnimation-7f4207e0{0%{background-position:0% 0%}50%{background-position:100% 100%}to{background-position:0% 0%}}.rootComponentArea[data-v-7f4207e0]{display:flex;flex:1 0 auto}
+@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-7f547886],button[data-v-7f547886],textarea[data-v-7f547886],select[data-v-7f547886]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-7f547886]:focus,textarea[data-v-7f547886]:focus,select[data-v-7f547886]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-7f547886],h2[data-v-7f547886],h3[data-v-7f547886],h4[data-v-7f547886]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-7f547886]{font-size:1.3rem}h2[data-v-7f547886]{font-size:1rem}h3[data-v-7f547886]{font-size:.9rem}h4[data-v-7f547886]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-7f547886],ol[data-v-7f547886]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-7f547886]{margin:0 0 0 32px}hr[data-v-7f547886]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-7f547886]{color:var(--primaryTextColor)}code[data-v-7f547886]{background-color:var(--separatorColor)}button[data-v-7f547886]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-7f547886]:focus,button[data-v-7f547886]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-7f547886]{font-size:.8rem}.component.selected[data-v-7f547886]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-7f547886]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-7f547886]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-7f547886]{display:flex;gap:16px}[data-streamsync-container][data-v-7f547886]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-7f547886]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-7f547886]{animation:appearVertical-7f547886 .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-7f547886]{animation:appearHorizontal-7f547886 .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-7f547886{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-7f547886{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.ChildlessPlaceholder[data-v-7f547886]{background:rgba(0,0,0,.05);color:var(--primaryTextColor);padding:16px;display:flex;align-items:center;justify-content:center;width:100%;min-height:100%}.content[data-v-7f547886]{text-align:center}.title>h2[data-v-7f547886]{color:var(--primaryTextColor);opacity:.8}.message[data-v-7f547886]{opacity:.5;margin-top:8px}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-a731db34],button[data-v-a731db34],textarea[data-v-a731db34],select[data-v-a731db34]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-a731db34]:focus,textarea[data-v-a731db34]:focus,select[data-v-a731db34]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-a731db34],h2[data-v-a731db34],h3[data-v-a731db34],h4[data-v-a731db34]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-a731db34]{font-size:1.3rem}h2[data-v-a731db34]{font-size:1rem}h3[data-v-a731db34]{font-size:.9rem}h4[data-v-a731db34]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-a731db34],ol[data-v-a731db34]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-a731db34]{margin:0 0 0 32px}hr[data-v-a731db34]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-a731db34]{color:var(--primaryTextColor)}code[data-v-a731db34]{background-color:var(--separatorColor)}button[data-v-a731db34]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-a731db34]:focus,button[data-v-a731db34]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-a731db34]{font-size:.8rem}.component.selected[data-v-a731db34]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-a731db34]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-a731db34]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-a731db34]{display:flex;gap:16px}[data-streamsync-container][data-v-a731db34]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-a731db34]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-a731db34]{animation:appearVertical-a731db34 .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-a731db34]{animation:appearHorizontal-a731db34 .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-a731db34{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-a731db34{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-54d2c60b],button[data-v-54d2c60b],textarea[data-v-54d2c60b],select[data-v-54d2c60b]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-54d2c60b]:focus,textarea[data-v-54d2c60b]:focus,select[data-v-54d2c60b]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-54d2c60b],h2[data-v-54d2c60b],h3[data-v-54d2c60b],h4[data-v-54d2c60b]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-54d2c60b]{font-size:1.3rem}h2[data-v-54d2c60b]{font-size:1rem}h3[data-v-54d2c60b]{font-size:.9rem}h4[data-v-54d2c60b]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-54d2c60b],ol[data-v-54d2c60b]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-54d2c60b]{margin:0 0 0 32px}hr[data-v-54d2c60b]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-54d2c60b]{color:var(--primaryTextColor)}code[data-v-54d2c60b]{background-color:var(--separatorColor)}button[data-v-54d2c60b]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-54d2c60b]:focus,button[data-v-54d2c60b]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-54d2c60b]{font-size:.8rem}.component.selected[data-v-54d2c60b]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-54d2c60b]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-54d2c60b]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-54d2c60b]{display:flex;gap:16px}[data-streamsync-container][data-v-54d2c60b]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-54d2c60b]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-54d2c60b]{animation:appearVertical-54d2c60b .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-54d2c60b]{animation:appearHorizontal-54d2c60b .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-54d2c60b{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-54d2c60b{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.RendererNotifications[data-v-54d2c60b]{position:sticky;top:24px;margin-left:auto;margin-right:24px;max-width:70ch;width:40vw;z-index:3}.balloonFlash[data-v-54d2c60b]{right:0;position:absolute;opacity:.8;background:var(--accentColor);width:52px;height:52px;border-radius:50%}.balloon.alert+.balloonFlash[data-v-54d2c60b]{animation-name:alert-54d2c60b;animation-duration:1s;animation-timing-function:ease-in-out}.balloon[data-v-54d2c60b]{z-index:2;position:absolute;-webkit-user-select:none;user-select:none;right:0;font-size:.7rem;border-radius:50%;background:var(--accentColor);width:52px;height:52px;color:var(--emptinessColor);display:flex;align-items:center;justify-content:center;cursor:pointer;box-shadow:0 0 8px 2px #0003;flex-direction:column}.balloon.alert i[data-v-54d2c60b]{animation-name:ring-54d2c60b;animation-duration:.3s;animation-iteration-count:4;animation-timing-function:ease-in-out}.balloon .counter[data-v-54d2c60b]{position:absolute;top:40px;right:0;background:var(--containerBackgroundColor);padding:4px 8px;border-radius:16px;color:var(--primaryTextColor);border:1px solid var(--separatorColor)}@keyframes alert-54d2c60b{0%{transform:scale(1)}50%{transform:scale(1.7)}to{transform:scale(1)}}@keyframes ring-54d2c60b{0%{transform:rotate(0)}25%{transform:rotate(-25deg)}75%{transform:rotate(25deg)}to{transform:rotate(0)}}.main[data-v-54d2c60b]{position:absolute;max-height:75vh;overflow-y:auto;overflow-x:hidden;right:0;width:100%;max-width:100%;top:72px;color:var(--primaryTextColor);background:var(--containerBackgroundColor);border-radius:8px;box-shadow:0 0 8px #0003}.clearContainer[data-v-54d2c60b]{padding:16px}.clearContainer button[data-v-54d2c60b]{margin-left:auto;margin-right:0}.notification[data-v-54d2c60b]{border-top:1px solid var(--separatorColor);padding:16px 16px 16px 0;font-size:.8rem;display:grid;grid-template-rows:1fr;grid-template-columns:72px 1fr;align-items:center}.notification .icon[data-v-54d2c60b]{grid-area:1/1;text-align:center}.notification .icon.error[data-v-54d2c60b]{color:#fb0000}.notification .icon.warning[data-v-54d2c60b]{color:#fb9600}.notification .icon.info[data-v-54d2c60b]{color:#00adb8}.notification .icon.success[data-v-54d2c60b]{color:#00b800}.notification .content[data-v-54d2c60b]{grid-area:1/2;max-width:100%;overflow:hidden}.notification header[data-v-54d2c60b]{display:flex}.notification header .title[data-v-54d2c60b]{flex:1 0 auto}.notification header .time[data-v-54d2c60b]{flex:0 0 auto;color:var(--secondaryTextColor)}.message[data-v-54d2c60b]{margin-top:12px}@font-face{font-family:Inter;src:url(./Inter-Regular-41ab0f70.ttf) format("truetype"),url(./Inter-Regular-d612f121.woff2) format("woff2")}input[data-v-7f4207e0],button[data-v-7f4207e0],textarea[data-v-7f4207e0],select[data-v-7f4207e0]{outline:none;border:1px solid var(--separatorColor);font-size:.75rem;padding:4px}input[data-v-7f4207e0]:focus,textarea[data-v-7f4207e0]:focus,select[data-v-7f4207e0]:focus{border:1px solid var(--primaryTextColor)}h1[data-v-7f4207e0],h2[data-v-7f4207e0],h3[data-v-7f4207e0],h4[data-v-7f4207e0]{font-weight:300;margin:0;color:var(--primaryTextColor)}h1[data-v-7f4207e0]{font-size:1.3rem}h2[data-v-7f4207e0]{font-size:1rem}h3[data-v-7f4207e0]{font-size:.9rem}h4[data-v-7f4207e0]{text-transform:uppercase;font-weight:700;font-size:.65rem;letter-spacing:.2ch}ul[data-v-7f4207e0],ol[data-v-7f4207e0]{padding:0;padding-inline-start:0;margin-block-start:0}li[data-v-7f4207e0]{margin:0 0 0 32px}hr[data-v-7f4207e0]{border:none;border-top:1px solid var(--separatorColor)}label[data-v-7f4207e0]{color:var(--primaryTextColor)}code[data-v-7f4207e0]{background-color:var(--separatorColor)}button[data-v-7f4207e0]{background:var(--buttonColor);font-size:.8rem;border-radius:8px;padding:12px;display:block;cursor:pointer;color:var(--buttonTextColor);box-shadow:var(--buttonShadow)}button[data-v-7f4207e0]:focus,button[data-v-7f4207e0]:hover{border:1px solid var(--buttonTextColor)}.component[data-v-7f4207e0]{font-size:.8rem}.component.selected[data-v-7f4207e0]{background-color:var(--builderSelectedColor)}[data-streamsync-slot-of-id][data-v-7f4207e0]{display:none;opacity:0;border-radius:2px;border:1px solid var(--separatorColor);box-shadow:0 0 3px 0 var(--separatorColor) inset;min-height:0px;min-width:0px;overflow:hidden;animation:appear .2s reverse}[data-streamsync-slot-of-id].highlighted[data-v-7f4207e0]{background:var(--builderIntenseSelectedColor)}[data-streamsync-container][data-v-7f4207e0]{display:flex;gap:16px}[data-streamsync-container][data-v-7f4207e0]:not(.horizontal){flex-direction:column}[data-streamsync-container].horizontal[data-v-7f4207e0]{flex-direction:row}[data-streamsync-container].crackedContainer>[data-streamsync-slot-of-id][data-v-7f4207e0]{animation:appearVertical-7f4207e0 .2s forwards;display:block}[data-streamsync-container].crackedContainer.horizontal>[data-streamsync-slot-of-id][data-v-7f4207e0]{animation:appearHorizontal-7f4207e0 .2s forwards;align-self:center;display:block}@keyframes appearHorizontal-7f4207e0{0%{min-height:0px;min-width:0px;opacity:0}to{height:100%;min-height:24px;min-width:4px;opacity:1}}@keyframes appearVertical-7f4207e0{0%{min-height:0px;min-width:0px;opacity:0}to{width:100%;min-height:4px;min-width:24px;opacity:1}}.ComponentRenderer[data-v-7f4207e0]{--accentColor: #29cf00;--buttonColor: #ffffff;--emptinessColor: #e9eef1;--separatorColor: rgba(0, 0, 0, .07);--primaryTextColor: #202829;--buttonTextColor: #202829;--secondaryTextColor: #5d7275;--containerBackgroundColor: #ffffff;width:100%;outline:none;--notificationsDisplacement: 0;font-family:Inter,sans-serif;font-size:.8rem;color:var(--primaryTextColor);background:var(--emptinessColor);display:flex;flex-direction:column;min-height:100%;isolation:isolate;flex:1 0 auto}.notifications[data-v-7f4207e0]{right:var(--notificationsDisplacement)}.loadingBar[data-v-7f4207e0]{width:100%;height:4px;margin-bottom:-4px;position:sticky;top:0;pointer-events:none;z-index:4;transition-delay:.2s;transition-property:opacity;transition-duration:.2s;opacity:0}.loadingActive .loadingBar[data-v-7f4207e0]{background-size:200% 200%;opacity:1;animation:loadingAnimation-7f4207e0 ease-in-out 1s infinite;animation-delay:.2s;background-image:linear-gradient(270deg,var(--emptinessColor),var(--accentColor),var(--emptinessColor))}@keyframes loadingAnimation-7f4207e0{0%{background-position:0% 0%}50%{background-position:100% 100%}to{background-position:0% 0%}}.rootComponentArea[data-v-7f4207e0]{display:flex;flex:1 0 auto}
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/Inter-Regular-41ab0f70.ttf` & `streamsync-0.4.0rc4/src/streamsync/static/assets/Inter-Regular-41ab0f70.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/Inter-Regular-d612f121.woff2` & `streamsync-0.4.0rc4/src/streamsync/static/assets/Inter-Regular-d612f121.woff2`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/abap-b029dff1.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/abap-b029dff1.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/apex-3c83662c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/apex-3c83662c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/azcli-f1f7c576.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/azcli-f1f7c576.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/bat-86aea46a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/bat-86aea46a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/bicep-75c0c4d5.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/bicep-75c0c4d5.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/cameligo-8043f913.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/cameligo-8043f913.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/clojure-73642b02.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/clojure-73642b02.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/codicon-79f233d0.ttf` & `streamsync-0.4.0rc4/src/streamsync/static/assets/codicon-79f233d0.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/coffee-a18badcf.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/coffee-a18badcf.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/cpp-4034161e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/cpp-4034161e.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/csharp-49cbf0d2.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/csharp-49cbf0d2.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/csp-d207cac4.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/csp-d207cac4.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/css-74326df0.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/css-74326df0.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/cssMode-dc15036c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/cssMode-40a421b7.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
     configurable: !0,
     writable: !0,
     value: i
 }) : e[n] = i;
 var k = (e, n, i) => (je(e, typeof n != "symbol" ? n + "" : n, i), i);
 import {
     m as Ne
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var We = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/cypher-49f5f839.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/cypher-49f5f839.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/dart-84b7c6b4.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/dart-84b7c6b4.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/dockerfile-bbf114b2.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/dockerfile-bbf114b2.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/ecl-15840f49.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/ecl-15840f49.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/elixir-e479e18e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/elixir-e479e18e.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/flow9-42a61225.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/flow9-42a61225.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/freemarker2-c56b9d61.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/freemarker2-ab7f8d00.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as F
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var b = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/fsharp-8abe6da0.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/fsharp-8abe6da0.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/go-8759e9f7.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/go-8759e9f7.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/graphql-387d549c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/graphql-387d549c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/handlebars-1fc6855b.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/handlebars-b7cc84e9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as l
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var s = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/hcl-a88f331a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/hcl-a88f331a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/html-1e46783a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/html-14f46deb.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as p
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var d = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/htmlMode-82eab562.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/htmlMode-4adc2b6d.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
     configurable: !0,
     writable: !0,
     value: i
 }) : e[n] = i;
 var k = (e, n, i) => (qe(e, typeof n != "symbol" ? n + "" : n, i), i);
 import {
     m as Qe
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var Ge = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/index-165490a0.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/index-3137b44e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -42,15 +42,15 @@
     w as withDirectives,
     v as vShow,
     f as createBaseVNode,
     q as renderSlot,
     a1 as shallowRef,
     a2 as isRef,
     a3 as toRaw
-} from "./index-b222671e.js";
+} from "./index-0d669be8.js";
 
 function commonjsRequire(E) {
     throw new Error('Could not dynamically require "' + E + '". Please configure the dynamicRequireTargets or/and ignoreDynamicRequires option of @rollup/plugin-commonjs appropriately for this require call to work.')
 }
 var pdf = {
     exports: {}
 };
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/index-59f5827a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/index-59f5827a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/index-b222671e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/index-0d669be8.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -6539,15 +6539,15 @@
             const t = re(null),
                 n = re(null),
                 a = K(X.evaluatedFields),
                 r = pe(() => a.spec.value),
                 o = async () => {
                     var h, g;
                     if (!r.value || !n.value) return;
-                    const f = await Zt(() => import("./plotly.min-95fb3915.js").then(E => E.p), [], import.meta.url);
+                    const f = await Zt(() => import("./plotly.min-d27e0f8d.js").then(E => E.p), [], import.meta.url);
                     !t.value || t.value.clientHeight == 0 || (f.newPlot(n.value, r.value), c(), (g = (h = r.value) == null ? void 0 : h.layout) != null && g.autosize && i())
                 };
 
             function i() {
                 const f = t.value.parentElement;
                 f != null && f.clientHeight && (t.value.style.height = "100%", n.value.style.height = "100%")
             }
@@ -6794,15 +6794,15 @@
             const t = re(null),
                 n = re(null),
                 a = K(X.evaluatedFields),
                 r = async () => {
                     if (!a.spec.value || !n.value) return;
                     const {
                         default: o
-                    } = await Zt(() => import("./vega-embed.module-ab6e1af3.js"), [], import.meta.url);
+                    } = await Zt(() => import("./vega-embed.module-3d202f0a.js"), [], import.meta.url);
                     await o(n.value, a.spec.value)
                 };
             return Le(() => a.spec.value, o => {
                 o && r()
             }), Yt(() => {
                 r(), new ResizeObserver(r).observe(t.value, {
                     box: "border-box"
@@ -9805,15 +9805,15 @@
             componentId: h
         } = p.at(-1), g = e.getComponentById(h);
         if (!g) return;
         const {
             fields: E
         } = e.getComponentDefinition(g.type), A = (T = g.content) == null ? void 0 : T[f], y = E[f].default, k = o(A, p), Y = E[f].type, B = typeof k > "u" || k === null || k === "";
         if (Y == L.Object || Y == L.KeyValue) {
-            if (!k) return JSON.parse(y) ?? null;
+            if (!k) return JSON.parse(y ?? null);
             if (typeof k != "string") return k;
             let C;
             try {
                 C = JSON.parse(k)
             } catch {
                 return JSON.parse(y) ?? null
             }
@@ -13142,15 +13142,15 @@
                 f = re(0),
                 h = re(null),
                 g = re(null),
                 E = re(!1),
                 A = re(0),
                 y = re([]);
             Yt(async () => {
-                const G = await Zt(() => import("./index-165490a0.js"), [], import.meta.url);
+                const G = await Zt(() => import("./index-3137b44e.js"), [], import.meta.url);
                 r = G.VuePDF;
                 const ue = G.usePDF;
                 ({
                     pdf: n,
                     pages: a
                 } = ue(t.source)), k()
             });
@@ -13933,15 +13933,15 @@
                 a = re(null),
                 r = pe(() => [t.lng.value, t.lat.value]),
                 o = re(null);
             let i = [],
                 c = null;
             const u = async () => {
                 if (!a.value || !t.accessToken.value) return;
-                const f = await Zt(() => import("./mapbox-gl-6d4978b5.js").then(h => h.m), [], import.meta.url);
+                const f = await Zt(() => import("./mapbox-gl-572acb0e.js").then(h => h.m), [], import.meta.url);
                 try {
                     f.accessToken = t.accessToken.value, f.default && (f.default.accessToken = t.accessToken.value), o.value = new f.Map({
                         container: a.value,
                         style: t.mapStyle.value,
                         center: r.value,
                         zoom: t.zoom.value
                     }), o.value.on("click", h => {
@@ -13957,15 +13957,15 @@
                     }), c = new f.NavigationControl, t.controls.value === "yes" && o.value.addControl(c), t.markers.value && o.value.on("load", p)
                 } catch (h) {
                     console.error(h)
                 }
             }, p = async () => {
                 var h, g;
                 if (!o.value) return;
-                const f = await Zt(() => import("./mapbox-gl-6d4978b5.js").then(E => E.m), [], import.meta.url);
+                const f = await Zt(() => import("./mapbox-gl-572acb0e.js").then(E => E.m), [], import.meta.url);
                 i.forEach(E => E.remove()), i = [], (g = (h = t.markers) == null ? void 0 : h.value) == null || g.forEach(E => {
                     const A = new f.Marker().setLngLat([E.lng, E.lat]).addTo(o.value).setPopup(new f.Popup().setText(E.name));
                     i.push(A), A.getElement().addEventListener("click", y => {
                         const k = new CustomEvent("mapbox-marker-click", {
                             detail: {
                                 payload: E
                             }
@@ -15312,17 +15312,17 @@
 async function hI() {
     await Lr.init();
     const e = Lr.getMode(),
         t = e == "edit" ? jE() : void 0;
     t && Lr.addMailSubscription("logEntry", t.handleLogEntry), console.log(`Mounting app in mode ${e}...`);
     const {
         default: n
-    } = e === "run" && await Zt(() => import("./ComponentRenderer-82ebfa88.js"), ["./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css"], import.meta.url), {
+    } = e === "run" && await Zt(() => import("./ComponentRenderer-007280fe.js"), ["./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css"], import.meta.url), {
         default: a
-    } = e === "edit" && await Zt(() => import("./BuilderApp-6c29fc91.js").then(o => o.B), ["./BuilderApp-6c29fc91.js", "./marked.esm-0bd9b835.js", "./ComponentRenderer-82ebfa88.js", "./ComponentRenderer-a2494844.css", "./BuilderApp-9cf67088.css"], import.meta.url), r = bf(n || a);
+    } = e === "edit" && await Zt(() => import("./BuilderApp-82d844f6.js").then(o => o.B), ["./BuilderApp-82d844f6.js", "./marked.esm-0bd9b835.js", "./ComponentRenderer-007280fe.js", "./ComponentRenderer-08d5f1dc.css", "./BuilderApp-f68489e4.css"], import.meta.url), r = bf(n || a);
     r.use(fI), r.provide(X.core, Lr), r.provide(X.builderManager, t), pI(r), r.mount("#app")
 }
 console.log("Initialising Streamsync core...");
 hI().then(async () => {
     console.log("Core initialised.")
 }).catch(e => {
     console.error("Core initialisation failed.", e), document.write(e)
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/index-b7043f95.css` & `streamsync-0.4.0rc4/src/streamsync/static/assets/index-b7043f95.css`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/index.esm-1f2a7de3.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/index.esm-1f2a7de3.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/ini-18bf1153.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/ini-18bf1153.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/java-000a6283.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/java-000a6283.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/javascript-a891c4c5.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/javascript-18f19bfc.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 import {
     conf as t,
     language as e
-} from "./typescript-31544fa1.js";
-import "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./typescript-a67a867f.js";
+import "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var n = t,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/jsonMode-7dc8e9c5.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/jsonMode-be63eb4c.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -4,18 +4,18 @@
     configurable: !0,
     writable: !0,
     value: i
 }) : e[n] = i;
 var C = (e, n, i) => (Qe(e, typeof n != "symbol" ? n + "" : n, i), i);
 import {
     m as Ze
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var Ke = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/julia-0026391c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/julia-0026391c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/kotlin-06ee8898.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/kotlin-06ee8898.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/less-dd86a68c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/less-dd86a68c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/lexon-8d4b0444.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/lexon-8d4b0444.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/liquid-79207f1f.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/liquid-d7e3f977.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as d
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var s = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/lua-9adddcd9.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/lua-9adddcd9.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/m3-aa2dcf72.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/m3-aa2dcf72.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/mapbox-gl-6d4978b5.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/mapbox-gl-572acb0e.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 import {
     X as yA,
     a4 as xA
-} from "./index-b222671e.js";
+} from "./index-0d669be8.js";
 
 function vA(Cs, oh) {
     for (var qr = 0; qr < oh.length; qr++) {
         const fr = oh[qr];
         if (typeof fr != "string" && !Array.isArray(fr)) {
             for (const $r in fr)
                 if ($r !== "default" && !($r in Cs)) {
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/markdown-0f073a3a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/markdown-0f073a3a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/marked.esm-0bd9b835.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/marked.esm-0bd9b835.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/mdx-d684260e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/mdx-2b91f7f9.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as p
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var d = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/mips-bdd96c5a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/mips-bdd96c5a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/msdax-1ac55115.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/msdax-1ac55115.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/mysql-b530c105.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/mysql-b530c105.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/objective-c-951ded7b.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/objective-c-951ded7b.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/pascal-7442fd46.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/pascal-7442fd46.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/pascaligo-385edc0e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/pascaligo-385edc0e.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/perl-d5fb326c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/perl-d5fb326c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/pgsql-2d7db25a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/pgsql-2d7db25a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/php-1daff147.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/php-1daff147.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/pla-1b3e1614.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/pla-1b3e1614.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/plotly.min-95fb3915.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/plotly.min-d27e0f8d.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     X as Ld
-} from "./index-b222671e.js";
+} from "./index-0d669be8.js";
 
 function Cd(au, xc) {
     for (var Rl = 0; Rl < xc.length; Rl++) {
         const Is = xc[Rl];
         if (typeof Is != "string" && !Array.isArray(Is)) {
             for (const Ha in Is)
                 if (Ha !== "default" && !(Ha in au)) {
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/postiats-9db13649.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/postiats-9db13649.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/powerquery-4c428232.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/powerquery-4c428232.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/powershell-d3380668.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/powershell-d3380668.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/protobuf-941cf3e8.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/protobuf-941cf3e8.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/pug-cfe384ef.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/pug-cfe384ef.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/python-bbfdef2a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/python-a79eb30c.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as a
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var l = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/qsharp-e125d03f.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/qsharp-e125d03f.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/r-e0a01d4f.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/r-e0a01d4f.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/razor-edf02117.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/razor-673842c1.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as s
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var c = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/redis-d0a12fea.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/redis-d0a12fea.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/redshift-a163b94a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/redshift-a163b94a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-3d7b8a45.eot` & `streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-3d7b8a45.eot`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-793349c8.woff` & `streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-793349c8.woff`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-7c1b0867.woff2` & `streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-7c1b0867.woff2`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-931f98fd.svg` & `streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-931f98fd.svg`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/remixicon-b074b4f2.ttf` & `streamsync-0.4.0rc4/src/streamsync/static/assets/remixicon-b074b4f2.ttf`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/restructuredtext-5a906e1a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/restructuredtext-5a906e1a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/ruby-05b021bf.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/ruby-05b021bf.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/rust-3d80982c.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/rust-3d80982c.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/sb-2020a5af.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/sb-2020a5af.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/scala-54469b4b.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/scala-54469b4b.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/scheme-ff6e5671.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/scheme-ff6e5671.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/scss-77902feb.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/scss-77902feb.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/serialization-0c0131b6.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/serialization-0c0131b6.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/shell-3c06def6.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/shell-3c06def6.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/solidity-3d59d6a7.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/solidity-3d59d6a7.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/sophia-12eb7ba8.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/sophia-12eb7ba8.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/sparql-e42fb28a.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/sparql-e42fb28a.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/sql-d30fd9fd.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/sql-d30fd9fd.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/st-0857f583.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/st-0857f583.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/swift-f0a706dd.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/swift-f0a706dd.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/systemverilog-0cfd4211.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/systemverilog-0cfd4211.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/tcl-7df3c0c5.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/tcl-7df3c0c5.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/tsMode-d172b673.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/tsMode-27474ecc.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -5,18 +5,18 @@
     writable: !0,
     value: r
 }) : e[t] = r;
 var _ = (e, t, r) => (R(e, typeof t != "symbol" ? t + "" : t, r), r);
 import {
     t as K,
     m as E
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var L = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/twig-f894aab2.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/twig-f894aab2.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/typescript-31544fa1.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/typescript-a67a867f.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as a
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var c = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/vb-39a025f4.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/vb-39a025f4.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/vega-embed.module-ab6e1af3.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/vega-embed.module-3d202f0a.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     X as TL
-} from "./index-b222671e.js";
+} from "./index-0d669be8.js";
 /*!
  * https://github.com/Starcounter-Jack/JSON-Patch
  * (c) 2017-2022 Joachim Wester
  * MIT licensed
  */
 var DL = globalThis && globalThis.__extends || function() {
         var e = function(t, n) {
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/wgsl-afa2396f.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/wgsl-afa2396f.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/xml-1904b31e.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/xml-f0bf815b.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var c = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/assets/yaml-ea97fa90.js` & `streamsync-0.4.0rc4/src/streamsync/static/assets/yaml-d6c7a4c1.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
 import {
     m as i
-} from "./BuilderApp-6c29fc91.js";
-import "./index-b222671e.js";
+} from "./BuilderApp-82d844f6.js";
+import "./index-0d669be8.js";
 import "./marked.esm-0bd9b835.js";
-import "./ComponentRenderer-82ebfa88.js";
+import "./ComponentRenderer-007280fe.js";
 /*!-----------------------------------------------------------------------------
  * Copyright (c) Microsoft Corporation. All rights reserved.
  * Version: 0.41.0(38e1e3d097f84e336c311d071a9ffb5191d4ffd1)
  * Released under the MIT license
  * https://github.com/microsoft/monaco-editor/blob/main/LICENSE.txt
  *-----------------------------------------------------------------------------*/
 var c = Object.defineProperty,
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/favicon.png` & `streamsync-0.4.0rc4/src/streamsync/static/favicon.png`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/index.html` & `streamsync-0.4.0rc4/src/streamsync/static/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 				}
 				100% {
 					x: 0;
 					y: 45.3478;
 				}
 			}
 		</style>
-		<script type="module" crossorigin src="./assets/index-b222671e.js"></script>
+		<script type="module" crossorigin src="./assets/index-0d669be8.js"></script>
 		<link rel="stylesheet" href="./assets/index-b7043f95.css">
 	</head>
 	<body>
 		<div id="app">
 			<div id="loading">
 				<svg
 					width="60"
```

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/css.worker.bundle.js` & `streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/css.worker.bundle.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/editor.worker.bundle.js` & `streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/editor.worker.bundle.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/html.worker.bundle.js` & `streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/html.worker.bundle.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/json.worker.bundle.js` & `streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/json.worker.bundle.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/static/monacoeditorwork/ts.worker.bundle.js` & `streamsync-0.4.0rc4/src/streamsync/static/monacoeditorwork/ts.worker.bundle.js`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/ui.py` & `streamsync-0.4.0rc4/src/streamsync/ui.py`

 * *Files identical despite different names*

### Comparing `streamsync-0.4.0rc3/src/streamsync/ui_manager.py` & `streamsync-0.4.0rc4/src/streamsync/ui_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from json import dumps as json_dumps
 from typing import Optional
 
 from streamsync.core_ui import (Component, UIError,
-                                current_parent_container, current_component_tree, ComponentTree)
+                                current_parent_container, current_component_tree, ComponentTree, DependentComponentTree)
 
 
 class StreamsyncUI:
     """Provides mechanisms to manage and manipulate UI components within a
     Streamsync session.
 
     This class offers context managers and methods to dynamically create, find,
@@ -78,15 +78,14 @@
 
     @staticmethod
     def create_component(component_type: str, **kwargs) -> Component:
         StreamsyncUI.assert_in_container()
         component_tree = current_component_tree()
         component = _create_component(component_tree, component_type, **kwargs)
         component_tree.attach(component)
-
         return component
 
 
 def _prepare_handlers(raw_handlers: Optional[dict]):
     handlers = {}
     if raw_handlers is not None:
         for event, handler in raw_handlers.items():
@@ -111,15 +110,15 @@
 
 def _prepare_value(value):
     if isinstance(value, dict):
         return json_dumps(value)
     return str(value)
 
 
-def _create_component(component_tree: ComponentTree,  component_type: str, **kwargs) -> Component:
+def _create_component(component_tree: DependentComponentTree,  component_type: str, **kwargs) -> Component:
 
     parent_container = current_parent_container.get(None)
     if kwargs.get("id", False) is None:
         kwargs.pop("id")
 
     if kwargs.get("position", False) is None:
         kwargs.pop("position")
```

### Comparing `streamsync-0.4.0rc3/PKG-INFO` & `streamsync-0.4.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamsync
-Version: 0.4.0rc3
+Version: 0.4.0rc4
 Summary: Streamsync helps you create performant data apps, via Python code and its built-in visual UI editor.
 Home-page: https://www.streamsync.cloud
 License: Apache 2.0
 Keywords: data apps,gui,ui
 Author: Ramiro Medina
 Author-email: ramiro.a.medina@gmail.com
 Requires-Python: >=3.9.2,<4.0
```

