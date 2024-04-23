# Comparing `tmp/kk-0.9.8.tar.gz` & `tmp/kk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kk-0.9.8.tar", last modified: Sun Mar 31 15:33:58 2024, max compression
+gzip compressed data, was "kk-0.9.9.tar", last modified: Tue Apr 23 10:29:30 2024, max compression
```

## Comparing `kk-0.9.8.tar` & `kk-0.9.9.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.838435 kk-0.9.8/
--rw-r--r--   0 root         (0) root         (0)      589 2024-03-31 15:33:58.838435 kk-0.9.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.826435 kk-0.9.8/kk/
--rw-r--r--   0 root         (0) root         (0)      129 2024-03-31 15:33:55.000000 kk-0.9.8/kk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35462 2024-03-27 04:36:35.000000 kk-0.9.8/kk/handler.py
--rwxr-xr-x   0 root         (0) root         (0)     3686 2024-03-27 04:41:37.000000 kk-0.9.8/kk/index.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.826435 kk-0.9.8/kk/static/
--rw-r--r--   0 root         (0) root         (0)     4286 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.830435 kk-0.9.8/kk/static/img/
--rw-r--r--   0 root         (0) root         (0)     3397 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/apk.png
--rw-r--r--   0 root         (0) root         (0)     3105 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/audio.png
--rw-r--r--   0 root         (0) root         (0)     4154 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/c.png
--rw-r--r--   0 root         (0) root         (0)     3638 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/cpp.png
--rw-r--r--   0 root         (0) root         (0)     5479 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/css.png
--rw-r--r--   0 root         (0) root         (0)     4934 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/database.png
--rw-r--r--   0 root         (0) root         (0)     3229 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/dmg.png
--rw-r--r--   0 root         (0) root         (0)     4321 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/docx.png
--rw-r--r--   0 root         (0) root         (0)     4436 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/exe.png
--rw-r--r--   0 root         (0) root         (0)     3409 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/file.png
--rw-r--r--   0 root         (0) root         (0)     1595 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/folder.png
--rw-r--r--   0 root         (0) root         (0)     6366 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/golang.png
--rw-r--r--   0 root         (0) root         (0)     3457 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/html.png
--rw-r--r--   0 root         (0) root         (0)     3494 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/image.png
--rw-r--r--   0 root         (0) root         (0)     5324 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/ini.png
--rw-r--r--   0 root         (0) root         (0)     5633 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/iso.png
--rw-r--r--   0 root         (0) root         (0)     5994 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/java.png
--rw-r--r--   0 root         (0) root         (0)     5472 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/javascript.png
--rw-r--r--   0 root         (0) root         (0)     4946 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/json.png
--rw-r--r--   0 root         (0) root         (0)    11198 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/kindle.png
--rw-r--r--   0 root         (0) root         (0)     3968 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/markdown.png
--rw-r--r--   0 root         (0) root         (0)     4285 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/pdf.png
--rw-r--r--   0 root         (0) root         (0)     3158 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/pptx.png
--rw-r--r--   0 root         (0) root         (0)     3859 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/python.png
--rw-r--r--   0 root         (0) root         (0)     2114 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/rar.png
--rw-r--r--   0 root         (0) root         (0)     1394 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/shell.png
--rw-r--r--   0 root         (0) root         (0)     3806 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/txt.png
--rw-r--r--   0 root         (0) root         (0)     2448 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/video.png
--rw-r--r--   0 root         (0) root         (0)     3623 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/vue.png
--rw-r--r--   0 root         (0) root         (0)     3406 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/xlsx.png
--rw-r--r--   0 root         (0) root         (0)     3446 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/xml.png
--rw-r--r--   0 root         (0) root         (0)     4812 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/yaml.png
--rw-r--r--   0 root         (0) root         (0)     1930 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img/zip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.830435 kk-0.9.8/kk/static/img2/
--rw-r--r--   0 root         (0) root         (0)     5153 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/apk.png
--rw-r--r--   0 root         (0) root         (0)    17071 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/audio.png
--rw-r--r--   0 root         (0) root         (0)     6382 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/c.png
--rw-r--r--   0 root         (0) root         (0)     6673 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/cpp.png
--rw-r--r--   0 root         (0) root         (0)     5635 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/css.png
--rw-r--r--   0 root         (0) root         (0)    16755 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/database.png
--rw-r--r--   0 root         (0) root         (0)     4006 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/dmg.png
--rw-r--r--   0 root         (0) root         (0)     7904 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/docx.png
--rw-r--r--   0 root         (0) root         (0)     2245 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/exe.png
--rw-r--r--   0 root         (0) root         (0)     2822 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/file.png
--rw-r--r--   0 root         (0) root         (0)     3688 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/folder.png
--rw-r--r--   0 root         (0) root         (0)    12494 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/golang.png
--rw-r--r--   0 root         (0) root         (0)     8140 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/html.png
--rw-r--r--   0 root         (0) root         (0)     7301 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/image.png
--rw-r--r--   0 root         (0) root         (0)     8962 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/ini.png
--rw-r--r--   0 root         (0) root         (0)     7287 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/iso.png
--rw-r--r--   0 root         (0) root         (0)    15616 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/java.png
--rw-r--r--   0 root         (0) root         (0)    10518 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/javascript.png
--rw-r--r--   0 root         (0) root         (0)     3847 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/json.png
--rw-r--r--   0 root         (0) root         (0)     2997 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/kindle.png
--rw-r--r--   0 root         (0) root         (0)     2901 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/markdown.png
--rw-r--r--   0 root         (0) root         (0)    12717 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/pdf.png
--rw-r--r--   0 root         (0) root         (0)    12577 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/php.png
--rw-r--r--   0 root         (0) root         (0)     3574 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/pptx.png
--rw-r--r--   0 root         (0) root         (0)     9024 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/python.png
--rw-r--r--   0 root         (0) root         (0)     7434 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/shell.png
--rw-r--r--   0 root         (0) root         (0)     2901 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/txt.png
--rw-r--r--   0 root         (0) root         (0)    15897 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/video.png
--rw-r--r--   0 root         (0) root         (0)    13413 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/vue.png
--rw-r--r--   0 root         (0) root         (0)     8139 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/xlsx.png
--rw-r--r--   0 root         (0) root         (0)     3449 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/xml.png
--rw-r--r--   0 root         (0) root         (0)    11355 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/yaml.png
--rw-r--r--   0 root         (0) root         (0)     3509 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/img2/zip.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.822435 kk-0.9.8/kk/static/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.834435 kk-0.9.8/kk/static/src/css/
--rw-r--r--   0 root         (0) root         (0)    45250 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/DPlayer.min.css
--rw-r--r--   0 root         (0) root         (0)     5254 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.css
--rw-r--r--   0 root         (0) root         (0)     5572 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.eot
--rw-r--r--   0 root         (0) root         (0)    15798 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.svg
--rw-r--r--   0 root         (0) root         (0)     5404 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.ttf
--rw-r--r--   0 root         (0) root         (0)     3536 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.woff
--rw-r--r--   0 root         (0) root         (0)     2904 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/iconfont.woff2
--rw-r--r--   0 root         (0) root         (0)     3584 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/markdown.css
--rw-r--r--   0 root         (0) root         (0)     2477 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/css/monokai_sublime.css
--rw-r--r--   0 root         (0) root         (0)     9940 2024-03-26 09:19:54.000000 kk-0.9.8/kk/static/src/css/style.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.834435 kk-0.9.8/kk/static/src/js/
--rw-r--r--   0 root         (0) root         (0)   116781 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/DPlayer.min.js
--rw-r--r--   0 root         (0) root         (0)    10453 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/clipboard.min.js
--rw-r--r--   0 root         (0) root         (0)   173418 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/flv.min.js
--rw-r--r--   0 root         (0) root         (0)    80655 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/highcharts-more.js
--rw-r--r--   0 root         (0) root         (0)   254576 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/highcharts.js
--rw-r--r--   0 root         (0) root         (0)   749330 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/highlight.pack.min.js
--rw-r--r--   0 root         (0) root         (0)   231552 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/hls.min.js
--rw-r--r--   0 root         (0) root         (0)     5595 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/imagesloaded.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    88145 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/jquery.min.js
--rw-r--r--   0 root         (0) root         (0)    24104 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/masonry.pkgd.min.js
--rw-r--r--   0 root         (0) root         (0)    21347 2024-03-26 09:50:34.000000 kk-0.9.8/kk/static/src/js/page.js
--rw-r--r--   0 root         (0) root         (0)     2221 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/utils.js
--rw-r--r--   0 root         (0) root         (0)    70754 2024-03-24 07:25:29.000000 kk-0.9.8/kk/static/src/js/webuploader.nolog.min.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.834435 kk-0.9.8/kk/static/src/layui/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.834435 kk-0.9.8/kk/static/src/layui/css/
--rw-rw-rw-   0 root         (0) root         (0)   123804 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/css/layui.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.834435 kk-0.9.8/kk/static/src/layui/font/
--rw-rw-rw-   0 root         (0) root         (0)    54172 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/font/iconfont.eot
--rw-rw-rw-   0 root         (0) root         (0)   329481 2024-03-24 08:06:30.000000 kk-0.9.8/kk/static/src/layui/font/iconfont.svg
--rw-rw-rw-   0 root         (0) root         (0)    53996 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/font/iconfont.ttf
--rw-rw-rw-   0 root         (0) root         (0)    34624 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/font/iconfont.woff
--rw-rw-rw-   0 root         (0) root         (0)    29736 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/font/iconfont.woff2
--rw-rw-rw-   0 root         (0) root         (0)   352265 2024-02-28 01:16:52.000000 kk-0.9.8/kk/static/src/layui/layui.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.838435 kk-0.9.8/kk/templates/
--rw-r--r--   0 root         (0) root         (0)     3786 2024-03-26 10:46:28.000000 kk-0.9.8/kk/templates/admin.html
--rw-r--r--   0 root         (0) root         (0)     4289 2024-03-27 04:41:45.000000 kk-0.9.8/kk/templates/base.html
--rw-r--r--   0 root         (0) root         (0)     4032 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/chart.html
--rw-r--r--   0 root         (0) root         (0)    14157 2024-03-27 05:01:08.000000 kk-0.9.8/kk/templates/index.html
--rw-r--r--   0 root         (0) root         (0)     1772 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/manage.html
--rw-r--r--   0 root         (0) root         (0)     1461 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/reset.html
--rw-r--r--   0 root         (0) root         (0)     2995 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/search.html
--rw-r--r--   0 root         (0) root         (0)     1052 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/signin.html
--rw-r--r--   0 root         (0) root         (0)     1849 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/signup.html
--rw-r--r--   0 root         (0) root         (0)     5934 2024-03-24 07:25:29.000000 kk-0.9.8/kk/templates/table.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-31 15:33:58.826435 kk-0.9.8/kk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      589 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3060 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        3 2024-03-31 15:33:58.000000 kk-0.9.8/kk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-31 15:33:58.838435 kk-0.9.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1326 2024-03-24 10:57:40.000000 kk-0.9.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.326228 kk-0.9.9/
+-rw-r--r--   0 root         (0) root         (0)      589 2024-04-23 10:29:30.326228 kk-0.9.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3203 2022-07-14 13:13:22.000000 kk-0.9.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.306228 kk-0.9.9/kk/
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-23 10:29:22.000000 kk-0.9.9/kk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35462 2024-03-27 04:36:35.000000 kk-0.9.9/kk/handler.py
+-rwxr-xr-x   0 root         (0) root         (0)     3686 2024-03-27 04:41:37.000000 kk-0.9.9/kk/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.306228 kk-0.9.9/kk/static/
+-rw-r--r--   0 root         (0) root         (0)     4286 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.314228 kk-0.9.9/kk/static/img/
+-rw-r--r--   0 root         (0) root         (0)     3397 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/apk.png
+-rw-r--r--   0 root         (0) root         (0)     3105 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/audio.png
+-rw-r--r--   0 root         (0) root         (0)     4154 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/c.png
+-rw-r--r--   0 root         (0) root         (0)     3638 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/cpp.png
+-rw-r--r--   0 root         (0) root         (0)     5479 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/css.png
+-rw-r--r--   0 root         (0) root         (0)     4934 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/database.png
+-rw-r--r--   0 root         (0) root         (0)     3229 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/dmg.png
+-rw-r--r--   0 root         (0) root         (0)     4321 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/docx.png
+-rw-r--r--   0 root         (0) root         (0)     4436 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/exe.png
+-rw-r--r--   0 root         (0) root         (0)     3409 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/file.png
+-rw-r--r--   0 root         (0) root         (0)     1595 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/folder.png
+-rw-r--r--   0 root         (0) root         (0)     6366 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/golang.png
+-rw-r--r--   0 root         (0) root         (0)     3457 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/html.png
+-rw-r--r--   0 root         (0) root         (0)     3494 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/image.png
+-rw-r--r--   0 root         (0) root         (0)     5324 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/ini.png
+-rw-r--r--   0 root         (0) root         (0)     5633 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/iso.png
+-rw-r--r--   0 root         (0) root         (0)     5994 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/java.png
+-rw-r--r--   0 root         (0) root         (0)     5472 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/javascript.png
+-rw-r--r--   0 root         (0) root         (0)     4946 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/json.png
+-rw-r--r--   0 root         (0) root         (0)    11198 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/kindle.png
+-rw-r--r--   0 root         (0) root         (0)     3968 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/markdown.png
+-rw-r--r--   0 root         (0) root         (0)     4285 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/pdf.png
+-rw-r--r--   0 root         (0) root         (0)     3158 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/pptx.png
+-rw-r--r--   0 root         (0) root         (0)     3859 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/python.png
+-rw-r--r--   0 root         (0) root         (0)     2114 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/rar.png
+-rw-r--r--   0 root         (0) root         (0)     1394 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/shell.png
+-rw-r--r--   0 root         (0) root         (0)     3806 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/txt.png
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/video.png
+-rw-r--r--   0 root         (0) root         (0)     3623 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/vue.png
+-rw-r--r--   0 root         (0) root         (0)     3406 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/xlsx.png
+-rw-r--r--   0 root         (0) root         (0)     3446 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/xml.png
+-rw-r--r--   0 root         (0) root         (0)     4812 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/yaml.png
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img/zip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.318228 kk-0.9.9/kk/static/img2/
+-rw-r--r--   0 root         (0) root         (0)     5153 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/apk.png
+-rw-r--r--   0 root         (0) root         (0)    17071 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/audio.png
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/c.png
+-rw-r--r--   0 root         (0) root         (0)     6673 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/cpp.png
+-rw-r--r--   0 root         (0) root         (0)     5635 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/css.png
+-rw-r--r--   0 root         (0) root         (0)    16755 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/database.png
+-rw-r--r--   0 root         (0) root         (0)     4006 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/dmg.png
+-rw-r--r--   0 root         (0) root         (0)     7904 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/docx.png
+-rw-r--r--   0 root         (0) root         (0)     2245 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/exe.png
+-rw-r--r--   0 root         (0) root         (0)     2822 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/file.png
+-rw-r--r--   0 root         (0) root         (0)     3688 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/folder.png
+-rw-r--r--   0 root         (0) root         (0)    12494 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/golang.png
+-rw-r--r--   0 root         (0) root         (0)     8140 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/html.png
+-rw-r--r--   0 root         (0) root         (0)     7301 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/image.png
+-rw-r--r--   0 root         (0) root         (0)     8962 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/ini.png
+-rw-r--r--   0 root         (0) root         (0)     7287 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/iso.png
+-rw-r--r--   0 root         (0) root         (0)    15616 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/java.png
+-rw-r--r--   0 root         (0) root         (0)    10518 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/javascript.png
+-rw-r--r--   0 root         (0) root         (0)     3847 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/json.png
+-rw-r--r--   0 root         (0) root         (0)     2997 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/kindle.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/markdown.png
+-rw-r--r--   0 root         (0) root         (0)    12717 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/pdf.png
+-rw-r--r--   0 root         (0) root         (0)    12577 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/php.png
+-rw-r--r--   0 root         (0) root         (0)     3574 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/pptx.png
+-rw-r--r--   0 root         (0) root         (0)     9024 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/python.png
+-rw-r--r--   0 root         (0) root         (0)     7434 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/shell.png
+-rw-r--r--   0 root         (0) root         (0)     2901 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/txt.png
+-rw-r--r--   0 root         (0) root         (0)    15897 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/video.png
+-rw-r--r--   0 root         (0) root         (0)    13413 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/vue.png
+-rw-r--r--   0 root         (0) root         (0)     8139 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/xlsx.png
+-rw-r--r--   0 root         (0) root         (0)     3449 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/xml.png
+-rw-r--r--   0 root         (0) root         (0)    11355 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/yaml.png
+-rw-r--r--   0 root         (0) root         (0)     3509 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/img2/zip.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.306228 kk-0.9.9/kk/static/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.322228 kk-0.9.9/kk/static/src/css/
+-rw-r--r--   0 root         (0) root         (0)    45250 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/DPlayer.min.css
+-rw-r--r--   0 root         (0) root         (0)     5254 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.css
+-rw-r--r--   0 root         (0) root         (0)     5572 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.eot
+-rw-r--r--   0 root         (0) root         (0)    15798 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.svg
+-rw-r--r--   0 root         (0) root         (0)     5404 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.ttf
+-rw-r--r--   0 root         (0) root         (0)     3536 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.woff
+-rw-r--r--   0 root         (0) root         (0)     2904 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/iconfont.woff2
+-rw-r--r--   0 root         (0) root         (0)     3584 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/markdown.css
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/css/monokai_sublime.css
+-rw-r--r--   0 root         (0) root         (0)     9940 2024-03-26 09:19:54.000000 kk-0.9.9/kk/static/src/css/style.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.322228 kk-0.9.9/kk/static/src/js/
+-rw-r--r--   0 root         (0) root         (0)   116781 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/DPlayer.min.js
+-rw-r--r--   0 root         (0) root         (0)    10453 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/clipboard.min.js
+-rw-r--r--   0 root         (0) root         (0)   173418 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/flv.min.js
+-rw-r--r--   0 root         (0) root         (0)    80655 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/highcharts-more.js
+-rw-r--r--   0 root         (0) root         (0)   254576 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/highcharts.js
+-rw-r--r--   0 root         (0) root         (0)   749330 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/highlight.pack.min.js
+-rw-r--r--   0 root         (0) root         (0)   231552 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/hls.min.js
+-rw-r--r--   0 root         (0) root         (0)     5595 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/imagesloaded.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    88145 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/jquery.min.js
+-rw-r--r--   0 root         (0) root         (0)    24104 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/masonry.pkgd.min.js
+-rw-r--r--   0 root         (0) root         (0)    21347 2024-03-26 09:50:34.000000 kk-0.9.9/kk/static/src/js/page.js
+-rw-r--r--   0 root         (0) root         (0)     2221 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/utils.js
+-rw-r--r--   0 root         (0) root         (0)    70754 2024-03-24 07:25:29.000000 kk-0.9.9/kk/static/src/js/webuploader.nolog.min.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.322228 kk-0.9.9/kk/static/src/layui/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.326228 kk-0.9.9/kk/static/src/layui/css/
+-rw-rw-rw-   0 root         (0) root         (0)   123804 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/css/layui.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.326228 kk-0.9.9/kk/static/src/layui/font/
+-rw-rw-rw-   0 root         (0) root         (0)    54172 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/font/iconfont.eot
+-rw-rw-rw-   0 root         (0) root         (0)   329481 2024-03-24 08:06:30.000000 kk-0.9.9/kk/static/src/layui/font/iconfont.svg
+-rw-rw-rw-   0 root         (0) root         (0)    53996 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/font/iconfont.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    34624 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/font/iconfont.woff
+-rw-rw-rw-   0 root         (0) root         (0)    29736 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/font/iconfont.woff2
+-rw-rw-rw-   0 root         (0) root         (0)   352265 2024-02-28 01:16:52.000000 kk-0.9.9/kk/static/src/layui/layui.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.326228 kk-0.9.9/kk/templates/
+-rw-r--r--   0 root         (0) root         (0)     3786 2024-03-26 10:46:28.000000 kk-0.9.9/kk/templates/admin.html
+-rw-r--r--   0 root         (0) root         (0)     4289 2024-03-27 04:41:45.000000 kk-0.9.9/kk/templates/base.html
+-rw-r--r--   0 root         (0) root         (0)     4032 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/chart.html
+-rw-r--r--   0 root         (0) root         (0)    14223 2024-04-23 10:27:57.000000 kk-0.9.9/kk/templates/index.html
+-rw-r--r--   0 root         (0) root         (0)     1772 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/manage.html
+-rw-r--r--   0 root         (0) root         (0)     1461 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/reset.html
+-rw-r--r--   0 root         (0) root         (0)     2995 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/search.html
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/signin.html
+-rw-r--r--   0 root         (0) root         (0)     1849 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/signup.html
+-rw-r--r--   0 root         (0) root         (0)     5934 2024-03-24 07:25:29.000000 kk-0.9.9/kk/templates/table.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 10:29:30.306228 kk-0.9.9/kk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      589 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3060 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        3 2024-04-23 10:29:30.000000 kk-0.9.9/kk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 10:29:30.326228 kk-0.9.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-03-24 10:57:40.000000 kk-0.9.9/setup.py
```

### Comparing `kk-0.9.8/PKG-INFO` & `kk-0.9.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk
-Version: 0.9.8
+Version: 0.9.9
 Summary: a simple file server
 Home-page: https://github.com/zkdfbb/kk
 Author: digua
 Author-email: zkdfbb@qq.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kk-0.9.8/README.md` & `kk-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/handler.py` & `kk-0.9.9/kk/handler.py`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/index.py` & `kk-0.9.9/kk/index.py`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/favicon.ico` & `kk-0.9.9/kk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/apk.png` & `kk-0.9.9/kk/static/img/apk.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/audio.png` & `kk-0.9.9/kk/static/img/audio.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/c.png` & `kk-0.9.9/kk/static/img/c.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/cpp.png` & `kk-0.9.9/kk/static/img/cpp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/css.png` & `kk-0.9.9/kk/static/img/css.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/database.png` & `kk-0.9.9/kk/static/img/database.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/dmg.png` & `kk-0.9.9/kk/static/img/dmg.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/docx.png` & `kk-0.9.9/kk/static/img/docx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/exe.png` & `kk-0.9.9/kk/static/img/exe.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/file.png` & `kk-0.9.9/kk/static/img/file.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/folder.png` & `kk-0.9.9/kk/static/img/folder.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/golang.png` & `kk-0.9.9/kk/static/img/golang.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/html.png` & `kk-0.9.9/kk/static/img/html.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/image.png` & `kk-0.9.9/kk/static/img/image.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/ini.png` & `kk-0.9.9/kk/static/img/ini.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/iso.png` & `kk-0.9.9/kk/static/img/iso.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/java.png` & `kk-0.9.9/kk/static/img/java.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/javascript.png` & `kk-0.9.9/kk/static/img/javascript.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/json.png` & `kk-0.9.9/kk/static/img/json.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/kindle.png` & `kk-0.9.9/kk/static/img/kindle.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/markdown.png` & `kk-0.9.9/kk/static/img/markdown.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/pdf.png` & `kk-0.9.9/kk/static/img/pdf.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/pptx.png` & `kk-0.9.9/kk/static/img/pptx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/python.png` & `kk-0.9.9/kk/static/img/python.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/rar.png` & `kk-0.9.9/kk/static/img/rar.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/shell.png` & `kk-0.9.9/kk/static/img/shell.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/txt.png` & `kk-0.9.9/kk/static/img/txt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/video.png` & `kk-0.9.9/kk/static/img/video.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/vue.png` & `kk-0.9.9/kk/static/img/vue.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/xlsx.png` & `kk-0.9.9/kk/static/img/xlsx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/xml.png` & `kk-0.9.9/kk/static/img/xml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/yaml.png` & `kk-0.9.9/kk/static/img/yaml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img/zip.png` & `kk-0.9.9/kk/static/img/zip.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/apk.png` & `kk-0.9.9/kk/static/img2/apk.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/audio.png` & `kk-0.9.9/kk/static/img2/audio.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/c.png` & `kk-0.9.9/kk/static/img2/c.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/cpp.png` & `kk-0.9.9/kk/static/img2/cpp.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/css.png` & `kk-0.9.9/kk/static/img2/css.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/database.png` & `kk-0.9.9/kk/static/img2/database.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/dmg.png` & `kk-0.9.9/kk/static/img2/dmg.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/docx.png` & `kk-0.9.9/kk/static/img2/docx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/exe.png` & `kk-0.9.9/kk/static/img2/exe.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/file.png` & `kk-0.9.9/kk/static/img2/file.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/folder.png` & `kk-0.9.9/kk/static/img2/folder.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/golang.png` & `kk-0.9.9/kk/static/img2/golang.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/html.png` & `kk-0.9.9/kk/static/img2/html.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/image.png` & `kk-0.9.9/kk/static/img2/image.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/ini.png` & `kk-0.9.9/kk/static/img2/ini.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/iso.png` & `kk-0.9.9/kk/static/img2/iso.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/java.png` & `kk-0.9.9/kk/static/img2/java.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/javascript.png` & `kk-0.9.9/kk/static/img2/javascript.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/json.png` & `kk-0.9.9/kk/static/img2/json.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/kindle.png` & `kk-0.9.9/kk/static/img2/kindle.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/markdown.png` & `kk-0.9.9/kk/static/img2/markdown.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/pdf.png` & `kk-0.9.9/kk/static/img2/pdf.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/php.png` & `kk-0.9.9/kk/static/img2/php.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/pptx.png` & `kk-0.9.9/kk/static/img2/pptx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/python.png` & `kk-0.9.9/kk/static/img2/python.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/shell.png` & `kk-0.9.9/kk/static/img2/shell.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/txt.png` & `kk-0.9.9/kk/static/img2/txt.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/video.png` & `kk-0.9.9/kk/static/img2/video.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/vue.png` & `kk-0.9.9/kk/static/img2/vue.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/xlsx.png` & `kk-0.9.9/kk/static/img2/xlsx.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/xml.png` & `kk-0.9.9/kk/static/img2/xml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/yaml.png` & `kk-0.9.9/kk/static/img2/yaml.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/img2/zip.png` & `kk-0.9.9/kk/static/img2/zip.png`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/DPlayer.min.css` & `kk-0.9.9/kk/static/src/css/DPlayer.min.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.css` & `kk-0.9.9/kk/static/src/css/iconfont.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.eot` & `kk-0.9.9/kk/static/src/css/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.svg` & `kk-0.9.9/kk/static/src/css/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.ttf` & `kk-0.9.9/kk/static/src/css/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.woff` & `kk-0.9.9/kk/static/src/css/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/iconfont.woff2` & `kk-0.9.9/kk/static/src/css/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/markdown.css` & `kk-0.9.9/kk/static/src/css/markdown.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/monokai_sublime.css` & `kk-0.9.9/kk/static/src/css/monokai_sublime.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/css/style.css` & `kk-0.9.9/kk/static/src/css/style.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/DPlayer.min.js` & `kk-0.9.9/kk/static/src/js/DPlayer.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/clipboard.min.js` & `kk-0.9.9/kk/static/src/js/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/flv.min.js` & `kk-0.9.9/kk/static/src/js/flv.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/highcharts-more.js` & `kk-0.9.9/kk/static/src/js/highcharts-more.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/highcharts.js` & `kk-0.9.9/kk/static/src/js/highcharts.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/highlight.pack.min.js` & `kk-0.9.9/kk/static/src/js/highlight.pack.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/hls.min.js` & `kk-0.9.9/kk/static/src/js/hls.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/imagesloaded.pkgd.min.js` & `kk-0.9.9/kk/static/src/js/imagesloaded.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/jquery.min.js` & `kk-0.9.9/kk/static/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/masonry.pkgd.min.js` & `kk-0.9.9/kk/static/src/js/masonry.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/page.js` & `kk-0.9.9/kk/static/src/js/page.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/utils.js` & `kk-0.9.9/kk/static/src/js/utils.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/js/webuploader.nolog.min.js` & `kk-0.9.9/kk/static/src/js/webuploader.nolog.min.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/css/layui.css` & `kk-0.9.9/kk/static/src/layui/css/layui.css`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/font/iconfont.eot` & `kk-0.9.9/kk/static/src/layui/font/iconfont.eot`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/font/iconfont.svg` & `kk-0.9.9/kk/static/src/layui/font/iconfont.svg`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/font/iconfont.ttf` & `kk-0.9.9/kk/static/src/layui/font/iconfont.ttf`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/font/iconfont.woff` & `kk-0.9.9/kk/static/src/layui/font/iconfont.woff`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/font/iconfont.woff2` & `kk-0.9.9/kk/static/src/layui/font/iconfont.woff2`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/static/src/layui/layui.js` & `kk-0.9.9/kk/static/src/layui/layui.js`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/admin.html` & `kk-0.9.9/kk/templates/admin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/base.html` & `kk-0.9.9/kk/templates/base.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/chart.html` & `kk-0.9.9/kk/templates/chart.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/index.html` & `kk-0.9.9/kk/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -156,26 +156,28 @@
             </button>
             <a class="layui-btn layui-btn-radius layui-btn-primary layui-btn-xs" href="/download/{{ doc.path }}{% if (doc.key and doc.is_dir) or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}">
               <i class="icon iconfont icon-clouddownload layui-tips" tips="下载"></i>
             </a>
             <button class="layui-btn layui-btn-radius layui-btn-primary layui-btn-xs btn-copy" add-host data-clipboard-text="/disk/{{ doc.path }}{% if (doc.key and doc.is_dir) or handler.args.key %}?key={{ doc.key or handler.args.key }}{% end %}">
               <i class="icon iconfont icon-copy layui-tips" tips="复制"></i>
             </button>
-              {% if handler.app.options.delete and not (handler.request.path.startswith('/share') or (handler.app.options.auth and handler.request.path.startswith("/disk/public") and not current_user.admin)) %}
+            {% if handler.app.options.delete and not (handler.request.path.startswith('/share') or (handler.app.options.auth and handler.request.path.startswith("/disk/public") and not current_user.admin)) %}
             <button class="layui-btn layui-btn-radius layui-btn-primary layui-btn-xs btn-delete">
               <i class="icon iconfont icon-delete layui-tips" tips="删除"></i>
             </button>
             {% end %}
+            {% if handler.app.options.auth %}
             <button class="layui-btn layui-btn-radius layui-btn-primary layui-btn-xs btn-share" {% if doc.share %}data-share="true"{% end %}>
               {% if doc.share %}
               <i class="layui-icon layui-icon-unlink layui-tips" tips="取消分享"></i>
               {% else %}
               <i class="layui-icon layui-icon-share layui-tips" tips="分享"></i>
               {% end %}
             </button>
+            {% end %}
 
             {% if False and handler.app.options.auth %}
             <ul class="layui-nav layui-btn-menu layui-btn-radius layui-btn-primary layui-btn-xs">
               <li class="layui-nav-item">
                 <a class="btn-menu layui-btn layui-btn-radius layui-btn-primary layui-btn-xs" href="javascript:;" style="width: 30px;">
                   <i class="layui-icon layui-icon-more"></i>
                 </a>
```

#### html2text {}

```diff
@@ -61,22 +61,22 @@
   ('preview') and                                                                 and not
   doc.path.suffix.lower                                                           (handler.request.path.startswith
   () in ['.mp3', '.amr',                                                          ('/share') or
   '.ogg', '.wav'] %} {%                                                           (handler.app.options.auth and
   elif not               {              {                    {                    handler.request.path.startswith
 ?? handler.get_cookie     {              {                    {                    ("/disk/public") and not
   ('preview') and        doc.expired_at handler.convert_time handler.convert_size current_user.admin)) %} {% end
-  doc.path.suffix.lower  or '' }}       (doc.mtime) }}       (doc.size) }}        %}
-  () in ['.mp4', 'mkv']                                                           % if doc.share %}data-
-  %} {% else %} {% set                                                            share="true"{% end %}> {% if
-  icon = 'folder.png' if                                                          doc.share %} {% else %} {% end
-  doc.is_dir else                                                                 %} {% if False and
-  handler.icon.get                                                                handler.app.options.auth %}
-  (doc.path.suffix.lower                                                          {% end %}
-  (), 'file.png') %}
+  doc.path.suffix.lower  or '' }}       (doc.mtime) }}       (doc.size) }}        %} {% if
+  () in ['.mp4', 'mkv']                                                           handler.app.options.auth %}
+  %} {% else %} {% set                                                            % if doc.share %}data-
+  icon = 'folder.png' if                                                          share="true"{% end %}> {% if
+  doc.is_dir else                                                                 doc.share %} {% else %} {% end
+  handler.icon.get                                                                %} {% end %} {% if False and
+  (doc.path.suffix.lower                                                          handler.app.options.auth %}
+  (), 'file.png') %}                                                              {% end %}
   % if icon in
   ['folder.png']
   %}style="width:
   22px;height:22px"{%
   elif icon in
   ['pdf.png',
   'audio.png',
```

### Comparing `kk-0.9.8/kk/templates/manage.html` & `kk-0.9.9/kk/templates/manage.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/reset.html` & `kk-0.9.9/kk/templates/reset.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/search.html` & `kk-0.9.9/kk/templates/search.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/signin.html` & `kk-0.9.9/kk/templates/signin.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/signup.html` & `kk-0.9.9/kk/templates/signup.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk/templates/table.html` & `kk-0.9.9/kk/templates/table.html`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/kk.egg-info/PKG-INFO` & `kk-0.9.9/kk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kk
-Version: 0.9.8
+Version: 0.9.9
 Summary: a simple file server
 Home-page: https://github.com/zkdfbb/kk
 Author: digua
 Author-email: zkdfbb@qq.com
 License: GPL
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `kk-0.9.8/kk.egg-info/SOURCES.txt` & `kk-0.9.9/kk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kk-0.9.8/setup.py` & `kk-0.9.9/setup.py`

 * *Files identical despite different names*

