# Comparing `tmp/tqsdk-3.5.6.tar.gz` & `tmp/tqsdk-3.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tqsdk-3.5.6.tar", last modified: Thu Apr 11 03:12:13 2024, max compression
+gzip compressed data, was "dist/tqsdk-3.5.7.tar", last modified: Tue Apr 23 02:18:44 2024, max compression
```

## Comparing `tqsdk-3.5.6.tar` & `tqsdk-3.5.7.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-11 03:11:37.000000 tqsdk-3.5.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 03:11:37.000000 tqsdk-3.5.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-11 03:12:13.000000 tqsdk-3.5.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-11 03:11:37.000000 tqsdk-3.5.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-11 03:11:37.000000 tqsdk-3.5.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/baseApi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/js/
--rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/js/app.2c843c86.js
--rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/js/chunk-vendors.d7fceff6.js
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/css/
--rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/css/chunk-vendors.c93e9127.css
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/css/app.d72d8978.css
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/img/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/img/icons/
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/notes
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-76x76.png
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-48x48.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-152x152.png
--rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-72x72.png
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-114x114.png
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-310x310.png
--rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-150x150.png
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-57x57.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-144x144.png
--rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/favicon-96x96.png
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-180x180.png
--rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-60x60.png
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-70x70.png
--rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-11 03:11:39.000000 tqsdk-3.5.6/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-36x36.png
--rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/img/ionicons.a2c4a261.svg
--rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/d3.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/web/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/fonts/ionicons.143146fa.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/fonts/ionicons.d535a25a.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/fonts/ionicons.99ac3308.woff
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-11 03:11:38.000000 tqsdk-3.5.6/tqsdk/web/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/demo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o60.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o74.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o41.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o10.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o73.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o71.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o40.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o30.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o72.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o20.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/option_tutorial/o70.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/ta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/demo/example/
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/fairy_four_price.py
--rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/gridtrading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/turtle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/momentum.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/gridtrading_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/dualthrust.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/doublema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/rbreaker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/aberration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/vwap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/escalator.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/example/rbreaker2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/ta_option.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t41.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/underlying_symbol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t92.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t90.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t30.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t20.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t96.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t80.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t93.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t60.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t95.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t71.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t10.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t72.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t40.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t94.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t91.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/replay2.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/tutorial/t70.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/download_orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/multiaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tafunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/risk_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/sm.py
--rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/ta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/utils_symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)   210161 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/data_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/calendar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/__pyinstaller/
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/__pyinstaller/hook-tqsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/__pyinstaller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23439 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/data_series.py
--rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/objs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/trade_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/symbols.py
--rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tqwebhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/risk_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/time_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/target_pos_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    37335 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/target_pos_task.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/lib/notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/datetime_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tools/dead_ins.lzma
--rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tools/downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/expired_quotes.json.lzma
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/baseModule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/stockprofit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/trading_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/multiaccount.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/backtest/
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/backtest/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/backtest/replay.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/backtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43337 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/backtest/backtest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/channel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/tradeable/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/tqsim.py
--rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/trade_future.py
--rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/tqsim_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/trade_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/basesim.py
--rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/trade_stock.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/tradeable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/tqaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/tqzq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/tqkq.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/base_otg.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/otg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/tradeable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/rangeset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/ins_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 03:12:13.000000 tqsdk-3.5.6/tqsdk/algorithm/
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/algorithm/twap.py
--rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/algorithm/time_table_generater.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-11 03:11:37.000000 tqsdk-3.5.6/tqsdk/objs_not_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-11 03:12:13.000000 tqsdk-3.5.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     6864 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/rangeset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/baseModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/stockprofit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/datetime_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tqwebhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/data_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6925 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/sm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/example/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/aberration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5201 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/rbreaker2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/doublema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/turtle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4153 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/gridtrading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/vwap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/dualthrust.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/gridtrading_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4596 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/rbreaker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/escalator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/fairy_four_price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5493 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/example/random_forest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t30.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t91.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t93.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t80.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/replay2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t71.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t92.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t90.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t96.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t40.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/underlying_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t94.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t95.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/tutorial/t72.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/download_orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/ta_option.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o41.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o72.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o30.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o71.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o40.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o10.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o70.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o74.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o73.py
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/option_tutorial/o60.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/demo/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21994 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20999 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/objs_not_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/trading_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/backtest/
+-rw-r--r--   0 runner    (1001) docker     (127)     6687 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/replay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4837 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43337 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/backtest/backtest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__pyinstaller/hook-tqsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/risk_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (127)    15912 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/time_table_generater.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/algorithm/twap.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7080 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/multiaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5400 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/baseApi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4824 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/risk_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/utils_symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/time_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10767 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/target_pos_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37335 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/lib/target_pos_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52750 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/tafunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37797 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/objs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   210161 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/trade_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)   132245 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/expired_quotes.json.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)     4910 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/channel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)    11283 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13385 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36480 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27585 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/trade_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim_stock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18113 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/sim/basesim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15130 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqkq.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/tqzq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/otg/base_otg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tradeable/tradeable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  1787845 2024-04-23 02:18:10.000000 tqsdk-3.5.7/tqsdk/web/js/chunk-vendors.d7fceff6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62759 2024-04-23 02:18:10.000000 tqsdk-3.5.7/tqsdk/web/js/app.2c843c86.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   555353 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/ionicons.a2c4a261.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/img/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-70x70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-60x60.png
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-76x76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-48x48.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-144x144.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-36x36.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6325 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-152x152.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5930 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/msapplication-icon-144x144.png.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-114x114.png
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-310x310.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-72x72.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-57x57.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/notes
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-96x96.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2024-04-23 02:18:06.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6269 2024-04-23 02:18:09.000000 tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8235 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-precomposed.png
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-23 02:18:08.000000 tqsdk-3.5.7/tqsdk/web/img/icons/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-23 02:18:07.000000 tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-180x180.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   197740 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.99ac3308.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   197664 2024-04-23 02:18:05.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.d535a25a.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    82216 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/fonts/ionicons.143146fa.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)   246120 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/d3.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/service-worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/robots.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/web/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   279508 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/css/chunk-vendors.c93e9127.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-04-23 02:18:04.000000 tqsdk-3.5.7/tqsdk/web/css/app.d72d8978.css
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-23 02:18:03.000000 tqsdk-3.5.7/tqsdk/web/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/dead_ins.lzma
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21845 2024-04-23 02:18:02.000000 tqsdk-3.5.7/tqsdk/tools/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20440 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    91538 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/ta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7136 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21813 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/ins_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23562 2024-04-23 02:18:01.000000 tqsdk-3.5.7/tqsdk/data_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-04-23 02:18:01.000000 tqsdk-3.5.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-04-23 02:18:01.000000 tqsdk-3.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-23 02:18:44.000000 tqsdk-3.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 02:18:01.000000 tqsdk-3.5.7/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5339 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 02:18:44.000000 tqsdk-3.5.7/tqsdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-23 02:18:44.000000 tqsdk-3.5.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-04-23 02:18:01.000000 tqsdk-3.5.7/setup.py
```

### Comparing `tqsdk-3.5.6/setup.py` & `tqsdk-3.5.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", mode="r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='tqsdk',
-    version="3.5.6",
+    version="3.5.7",
     description='TianQin SDK',
     author='TianQin',
     author_email='tianqincn@gmail.com',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://www.shinnytech.com/tqsdk',
     packages=setuptools.find_packages(exclude=["tqsdk.test", "tqsdk.test.*"]),
```

### Comparing `tqsdk-3.5.6/README.md` & `tqsdk-3.5.7/README.md`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/LICENSE` & `tqsdk-3.5.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk.egg-info/SOURCES.txt` & `tqsdk-3.5.7/tqsdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk.egg-info/PKG-INFO` & `tqsdk-3.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.6
+Version: 3.5.7
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tqsdk-3.5.6/tqsdk/baseApi.py` & `tqsdk-3.5.7/tqsdk/baseApi.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/js/app.2c843c86.js` & `tqsdk-3.5.7/tqsdk/web/js/app.2c843c86.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/js/chunk-vendors.d7fceff6.js` & `tqsdk-3.5.7/tqsdk/web/js/chunk-vendors.d7fceff6.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/manifest.json` & `tqsdk-3.5.7/tqsdk/web/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/css/chunk-vendors.c93e9127.css` & `tqsdk-3.5.7/tqsdk/web/css/chunk-vendors.c93e9127.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/css/app.d72d8978.css` & `tqsdk-3.5.7/tqsdk/web/css/app.d72d8978.css`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js` & `tqsdk-3.5.7/tqsdk/web/precache-manifest.7ed60b69dab01cdb0c64836489ab6e0d.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-72x72.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/manifest.json` & `tqsdk-3.5.7/tqsdk/web/img/icons/manifest.json`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/notes` & `tqsdk-3.5.7/tqsdk/web/img/icons/notes`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-76x76.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-76x76.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-144x144.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-48x48.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-48x48.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-192x192.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-120x120.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-120x120.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/mstile-150x150.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/favicon-32x32.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-152x152.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-152x152.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-72x72.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-72x72.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-114x114.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-114x114.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-310x310.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-310x310.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-150x150.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-150x150.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-96x96.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-chrome-192x192.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-192x192.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/favicon-16x16.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/favicon.ico` & `tqsdk-3.5.7/tqsdk/web/img/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-57x57.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-57x57.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-144x144.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-144x144.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/favicon-96x96.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-96x96.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-180x180.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-180x180.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-precomposed.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-precomposed.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/apple-touch-icon-60x60.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/apple-touch-icon-60x60.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/ms-icon-70x70.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/ms-icon-70x70.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/msapplication-icon-144x144.png.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/msapplication-icon-144x144.png.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/icons/android-icon-36x36.png` & `tqsdk-3.5.7/tqsdk/web/img/icons/android-icon-36x36.png`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/img/ionicons.a2c4a261.svg` & `tqsdk-3.5.7/tqsdk/web/img/ionicons.a2c4a261.svg`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/d3.min.js` & `tqsdk-3.5.7/tqsdk/web/d3.min.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/index.html` & `tqsdk-3.5.7/tqsdk/web/index.html`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/service-worker.js` & `tqsdk-3.5.7/tqsdk/web/service-worker.js`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/fonts/ionicons.143146fa.woff2` & `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.143146fa.woff2`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/fonts/ionicons.d535a25a.ttf` & `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.d535a25a.ttf`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/fonts/ionicons.99ac3308.woff` & `tqsdk-3.5.7/tqsdk/web/fonts/ionicons.99ac3308.woff`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/web/favicon.ico` & `tqsdk-3.5.7/tqsdk/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o60.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o74.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o74.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o41.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o73.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o73.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o71.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o40.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o30.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o72.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o20.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/option_tutorial/o70.py` & `tqsdk-3.5.7/tqsdk/demo/option_tutorial/o70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/ta.py` & `tqsdk-3.5.7/tqsdk/demo/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/fairy_four_price.py` & `tqsdk-3.5.7/tqsdk/demo/example/fairy_four_price.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/gridtrading.py` & `tqsdk-3.5.7/tqsdk/demo/example/gridtrading.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/turtle.py` & `tqsdk-3.5.7/tqsdk/demo/example/turtle.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/momentum.py` & `tqsdk-3.5.7/tqsdk/demo/example/momentum.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/gridtrading_async.py` & `tqsdk-3.5.7/tqsdk/demo/example/gridtrading_async.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/dualthrust.py` & `tqsdk-3.5.7/tqsdk/demo/example/dualthrust.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/doublema.py` & `tqsdk-3.5.7/tqsdk/demo/example/doublema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/rbreaker.py` & `tqsdk-3.5.7/tqsdk/demo/example/rbreaker.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/aberration.py` & `tqsdk-3.5.7/tqsdk/demo/example/aberration.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/vwap.py` & `tqsdk-3.5.7/tqsdk/demo/example/vwap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/random_forest.py` & `tqsdk-3.5.7/tqsdk/demo/example/random_forest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/escalator.py` & `tqsdk-3.5.7/tqsdk/demo/example/escalator.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/example/rbreaker2.py` & `tqsdk-3.5.7/tqsdk/demo/example/rbreaker2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/ta_option.py` & `tqsdk-3.5.7/tqsdk/demo/ta_option.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t41.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t41.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t92.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t92.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t90.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t90.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t30.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t30.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/downloader.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t20.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t20.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t96.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t96.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t80.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t80.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/replay.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t93.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t93.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t60.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t60.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t95.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t95.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t71.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t71.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t72.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t72.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t40.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t40.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t94.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t94.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t91.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t91.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/replay2.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/replay2.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/backtest.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/tutorial/t70.py` & `tqsdk-3.5.7/tqsdk/demo/tutorial/t70.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/download_orders.py` & `tqsdk-3.5.7/tqsdk/demo/download_orders.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/demo/multiaccount.py` & `tqsdk-3.5.7/tqsdk/demo/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tafunc.py` & `tqsdk-3.5.7/tqsdk/tafunc.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/utils.py` & `tqsdk-3.5.7/tqsdk/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/log.py` & `tqsdk-3.5.7/tqsdk/log.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/risk_rule.py` & `tqsdk-3.5.7/tqsdk/risk_rule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/sm.py` & `tqsdk-3.5.7/tqsdk/sm.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/report.py` & `tqsdk-3.5.7/tqsdk/report.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/ta.py` & `tqsdk-3.5.7/tqsdk/ta.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/utils_symbols.py` & `tqsdk-3.5.7/tqsdk/utils_symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/exceptions.py` & `tqsdk-3.5.7/tqsdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/api.py` & `tqsdk-3.5.7/tqsdk/api.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/data_extension.py` & `tqsdk-3.5.7/tqsdk/data_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/calendar.py` & `tqsdk-3.5.7/tqsdk/calendar.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/data_series.py` & `tqsdk-3.5.7/tqsdk/data_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                 await self._download_data_series(diff_rangeset)
                 self._merge_rangeset()  # 归并文件
                 rangeset_id = DataSeries._get_rangeset_id(symbol, self._dur_nano)
                 rangeset_dt = DataSeries._get_rangeset_dt(symbol, self._dur_nano, rangeset_id)
                 DataSeries._assert_rangeset_asce_sorted(rangeset_id)
                 DataSeries._assert_rangeset_asce_sorted(rangeset_dt)
 
-            assert len(rangeset_id) == len(rangeset_dt) > 0
+            assert len(rangeset_id) == len(rangeset_dt)  # rangeset_id 和 rangeset_dt 的长度应该相等, 且一一对应，有可能长度都为 0 ，即没有下载任何数据
 
             # 查找用户请求时间段与已有数据时间段的交集
             target_rangeset_dt = _rangeset_intersection([(self._start_dt_nano, self._end_dt_nano)], rangeset_dt)
             assert len(target_rangeset_dt) <= 1  # 用户请求应该落在一个时间段内，或者用户请求的时间段内没有任何数据
             if len(target_rangeset_dt) == 0:  # 用户请求的时间段内没有任何数据
                 return
```

### Comparing `tqsdk-3.5.6/tqsdk/objs.py` & `tqsdk-3.5.7/tqsdk/objs.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/trade_extension.py` & `tqsdk-3.5.7/tqsdk/trade_extension.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/datetime.py` & `tqsdk-3.5.7/tqsdk/datetime.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/symbols.py` & `tqsdk-3.5.7/tqsdk/symbols.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/connect.py` & `tqsdk-3.5.7/tqsdk/connect.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tqwebhelper.py` & `tqsdk-3.5.7/tqsdk/tqwebhelper.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/risk_manager.py` & `tqsdk-3.5.7/tqsdk/risk_manager.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/lib/utils.py` & `tqsdk-3.5.7/tqsdk/lib/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/lib/target_pos_scheduler.py` & `tqsdk-3.5.7/tqsdk/lib/target_pos_scheduler.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/lib/target_pos_task.py` & `tqsdk-3.5.7/tqsdk/lib/target_pos_task.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/lib/notify.py` & `tqsdk-3.5.7/tqsdk/lib/notify.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/datetime_state.py` & `tqsdk-3.5.7/tqsdk/datetime_state.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tools/dead_ins.lzma` & `tqsdk-3.5.7/tqsdk/tools/dead_ins.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tools/downloader.py` & `tqsdk-3.5.7/tqsdk/tools/downloader.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/expired_quotes.json.lzma` & `tqsdk-3.5.7/tqsdk/expired_quotes.json.lzma`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/entity.py` & `tqsdk-3.5.7/tqsdk/entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/baseModule.py` & `tqsdk-3.5.7/tqsdk/baseModule.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/stockprofit.py` & `tqsdk-3.5.7/tqsdk/stockprofit.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/trading_status.py` & `tqsdk-3.5.7/tqsdk/trading_status.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/multiaccount.py` & `tqsdk-3.5.7/tqsdk/multiaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/backtest/utils.py` & `tqsdk-3.5.7/tqsdk/backtest/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/backtest/replay.py` & `tqsdk-3.5.7/tqsdk/backtest/replay.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/backtest/backtest.py` & `tqsdk-3.5.7/tqsdk/backtest/backtest.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/channel.py` & `tqsdk-3.5.7/tqsdk/channel.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/utils.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/utils.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/tqsim.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/trade_future.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_future.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/tqsim_stock.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/tqsim_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/trade_base.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_base.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/basesim.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/basesim.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/sim/trade_stock.py` & `tqsdk-3.5.7/tqsdk/tradeable/sim/trade_stock.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/tradeable.py` & `tqsdk-3.5.7/tqsdk/tradeable/tradeable.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/otg/tqaccount.py` & `tqsdk-3.5.7/tqsdk/tradeable/otg/tqaccount.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/otg/tqzq.py` & `tqsdk-3.5.7/tqsdk/tradeable/otg/tqzq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/otg/tqkq.py` & `tqsdk-3.5.7/tqsdk/tradeable/otg/tqkq.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/otg/base_otg.py` & `tqsdk-3.5.7/tqsdk/tradeable/otg/base_otg.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/tradeable/mixin.py` & `tqsdk-3.5.7/tqsdk/tradeable/mixin.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/rangeset.py` & `tqsdk-3.5.7/tqsdk/rangeset.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/auth.py` & `tqsdk-3.5.7/tqsdk/auth.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/diff.py` & `tqsdk-3.5.7/tqsdk/diff.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/ins_schema.py` & `tqsdk-3.5.7/tqsdk/ins_schema.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/__init__.py` & `tqsdk-3.5.7/tqsdk/__init__.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/algorithm/twap.py` & `tqsdk-3.5.7/tqsdk/algorithm/twap.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/algorithm/time_table_generater.py` & `tqsdk-3.5.7/tqsdk/algorithm/time_table_generater.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/tqsdk/objs_not_entity.py` & `tqsdk-3.5.7/tqsdk/objs_not_entity.py`

 * *Files identical despite different names*

### Comparing `tqsdk-3.5.6/PKG-INFO` & `tqsdk-3.5.7/tqsdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tqsdk
-Version: 3.5.6
+Version: 3.5.7
 Summary: TianQin SDK
 Home-page: https://www.shinnytech.com/tqsdk
 Author: TianQin
 Author-email: tianqincn@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

