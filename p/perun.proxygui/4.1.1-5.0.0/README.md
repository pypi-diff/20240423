# Comparing `tmp/perun.proxygui-4.1.1.tar.gz` & `tmp/perun.proxygui-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-4.1.1.tar", last modified: Tue Apr 23 07:33:26 2024, max compression
+gzip compressed data, was "perun.proxygui-5.0.0.tar", last modified: Tue Apr 23 07:38:19 2024, max compression
```

## Comparing `perun.proxygui-4.1.1.tar` & `perun.proxygui-5.0.0.tar`

### file list

```diff
@@ -1,289 +1,289 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/LICENSE
--rw-rw-rw-   0     1001 root         (0)       46 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/MANIFEST.in
--rw-r--r--   0     1001 root         (0)     9393 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     8072 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun/proxygui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun/proxygui/api/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/__init__.py
--rw-rw-rw-   0     1001 root         (0)     2389 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0     1001 root         (0)     4476 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0     1001 root         (0)     4825 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0     1001 root         (0)    10175 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/heuristic_api.py
--rw-rw-rw-   0     1001 root         (0)     3037 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/api/kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)     6008 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/app.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun/proxygui/gui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0     1001 root         (0)    19806 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/gui.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun/proxygui/gui/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0     1001 root         (0)   141520 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)       99 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0     1001 root         (0)      612 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0     1001 root         (0)       67 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0     1001 root         (0)      688 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0     1001 root         (0)       19 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)      949 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0     1001 root         (0)     1663 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0     1001 root         (0)      477 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0     1001 root         (0)      631 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0     1001 root         (0)     1451 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)     3089 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0     1001 root         (0)     1617 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0     1001 root         (0)     1776 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0     1001 root         (0)      437 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0     1001 root         (0)      387 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0     1001 root         (0)     2945 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0     1001 root         (0)     2624 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0     1001 root         (0)      713 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0     1001 root         (0)     1899 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0     1001 root         (0)      815 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0     1001 root         (0)      571 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0     1001 root         (0)      421 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0     1001 root         (0)      403 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0     1001 root         (0)     2758 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.314116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0     1001 root         (0)      198 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0     1001 root         (0)      684 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0     1001 root         (0)    29997 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0     1001 root         (0)      244 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.318116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0     1001 root         (0)    22637 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0     1001 root         (0)    21057 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0     1001 root         (0)    22481 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0     1001 root         (0)    35533 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0     1001 root         (0)    34805 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0     1001 root         (0)    28733 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0     1001 root         (0)    20267 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28025 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0     1001 root         (0)    25884 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0     1001 root         (0)   363233 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0     1001 root         (0)    27013 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0     1001 root         (0)    33321 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0     1001 root         (0)    31511 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0     1001 root         (0)    34010 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28152 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0     1001 root         (0)    36726 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0     1001 root         (0)    28663 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0     1001 root         (0)    22030 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.322116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.338116 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0     1001 root         (0)   125046 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0     1001 root         (0)   252563 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0     1001 root         (0)  1052500 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0     1001 root         (0)  1125125 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0     1001 root         (0)  1125144 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0     1001 root         (0)  1125123 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0     1001 root         (0)  1125119 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0     1001 root         (0)  1125120 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0     1001 root         (0)  1125147 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0     1001 root         (0)  1125545 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0     1001 root         (0)  1126098 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)   139176 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0     1001 root         (0)     2596 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0     1001 root         (0)    48080 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.342115 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0     1001 root         (0)     2596 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0     1001 root         (0)    46987 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0     1001 root         (0)   303728 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   332353 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   332557 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0     1001 root         (0)     5778 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0     1001 root         (0)   312236 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   341456 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   341664 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0     1001 root         (0)     5772 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.342115 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0     1001 root         (0)    87048 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    74284 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)   208892 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0     1001 root         (0)   159376 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0     1001 root         (0)     1632 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0     1001 root         (0)     1837 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0     1001 root         (0)     1484 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0     1001 root         (0)      988 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0     1001 root         (0)    12252 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0     1001 root         (0)     9596 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.342115 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.346115 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0     1001 root         (0)    70841 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0     1001 root         (0)     4348 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0     1001 root         (0)      151 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0     1001 root         (0)      281 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0     1001 root         (0)      149 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0     1001 root         (0)      304 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0     1001 root         (0)     7406 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0     1001 root         (0)     4426 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0     1001 root         (0)      443 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.350115 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0     1001 root         (0)   218591 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0     1001 root         (0)   659454 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0     1001 root         (0)   337945 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0     1001 root         (0)     2707 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0     1001 root         (0)     8806 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0     1001 root         (0)    26171 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0     1001 root         (0)     4075 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0     1001 root         (0)   284394 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0     1001 root         (0)   610160 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.350115 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0     1001 root         (0)   155845 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0     1001 root         (0)   431289 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.350115 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0     1001 root         (0)    78743 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0     1001 root         (0)   325834 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0     1001 root         (0)       78 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0     1001 root         (0)     7336 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0     1001 root         (0)     4859 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.354115 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0     1001 root         (0)    73577 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0     1001 root         (0)    59305 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0     1001 root         (0)   134294 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0     1001 root         (0)   747927 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0     1001 root         (0)   133988 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0     1001 root         (0)    89988 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    76736 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)    34034 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0     1001 root         (0)   144714 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0     1001 root         (0)    33736 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0     1001 root         (0)    16276 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0     1001 root         (0)    13224 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0     1001 root         (0)   203030 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0     1001 root         (0)   918991 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0     1001 root         (0)   202744 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0     1001 root         (0)   101648 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0     1001 root         (0)    78268 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/
--rw-rw-rw-   0     1001 root         (0)      490 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/check.svg
--rw-rw-rw-   0     1001 root         (0)      536 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/circle-check-regular.svg
--rw-rw-rw-   0     1001 root         (0)      483 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
--rw-rw-rw-   0     1001 root         (0)      730 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/questionmark.svg
--rw-rw-rw-   0     1001 root         (0)      625 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/images/spinner.svg
--rw-rw-rw-   0     1001 root         (0)    89501 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/jquery-3.6.0.min.js
--rw-rw-rw-   0     1001 root         (0)      627 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/proxygui.css
--rw-rw-rw-   0     1001 root         (0)     1427 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/proxygui.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0     1001 root         (0)    15836 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0     1001 root         (0)     8266 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0     1001 root         (0)     8862 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0     1001 root         (0)     8873 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0     1001 root         (0)     7692 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0     1001 root         (0)     8344 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0     1001 root         (0)    11438 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0     1001 root         (0)    64906 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/templates/
--rw-rw-rw-   0     1001 root         (0)    15205 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0     1001 root         (0)     9192 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/HeuristicData.html
--rw-rw-rw-   0     1001 root         (0)      747 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0     1001 root         (0)     3091 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/Logout.html
--rw-rw-rw-   0     1001 root         (0)     1131 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetEmailSent.html
--rw-rw-rw-   0     1001 root         (0)     1942 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetInitiated.html
--rw-rw-rw-   0     1001 root         (0)     1133 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
--rw-rw-rw-   0     1001 root         (0)     1021 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResult.html
--rw-rw-rw-   0     1001 root         (0)      795 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/MissingAuth.html
--rw-rw-rw-   0     1001 root         (0)     1019 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/OidcError.html
--rw-rw-rw-   0     1001 root         (0)     1223 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/Post-logout.html
--rw-rw-rw-   0     1001 root         (0)      907 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0     1001 root         (0)     2490 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0     1001 root         (0)     8103 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0     1001 root         (0)     1175 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0     1001 root         (0)     3477 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/base.html
--rw-rw-rw-   0     1001 root         (0)      561 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/logout-iframe.html
--rw-rw-rw-   0     1001 root         (0)     3769 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/templates/logout-state.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/translations/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.266116 perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0     1001 root         (0)     2973 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0     1001 root         (0)     8108 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0     1001 root         (0)     5372 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/jwt.py
--rw-rw-rw-   0     1001 root         (0)    20220 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/logout_manager.py
--rw-rw-rw-   0     1001 root         (0)     2480 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/oauth.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.358115 perun.proxygui-4.1.1/perun/proxygui/openapi/
--rw-rw-rw-   0     1001 root         (0)     6107 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/openapi/openapi.py
--rw-rw-rw-   0     1001 root         (0)    12933 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/openapi/openapi_data.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/perun/proxygui/openapi/schemas/
--rw-rw-rw-   0     1001 root         (0)      997 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/openapi/schemas/arguments_schemas.py
--rw-rw-rw-   0     1001 root         (0)     1446 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/openapi/schemas/response_schemas.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/perun/proxygui/tests/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1816 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0     1001 root         (0)     6409 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0     1001 root         (0)     6635 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0     1001 root         (0)     4713 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2160 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0     1001 root         (0)     6826 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0     1001 root         (0)     1111 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/tests/test_kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)    21918 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/proxygui/user_manager.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/perun/utils/
--rw-rw-rw-   0     1001 root         (0)     2496 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/ConfigStore.py
--rw-rw-rw-   0     1001 root         (0)       43 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/CustomExceptions.py
--rw-rw-rw-   0     1001 root         (0)     2555 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/CustomRPHandler.py
--rw-rw-rw-   0     1001 root         (0)     1354 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/DatabaseService.py
--rw-rw-rw-   0     1001 root         (0)     4414 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/EmailService.py
--rw-rw-rw-   0     1001 root         (0)       96 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/Notification.py
--rw-rw-rw-   0     1001 root         (0)      816 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/Utils.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/perun/utils/consent_framework/
--rw-rw-rw-   0     1001 root         (0)     1241 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0     1001 root         (0)     2226 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2274 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0     1001 root         (0)      730 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0     1001 root         (0)     1371 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.362115 perun.proxygui-4.1.1/perun/utils/logout_requests/
--rw-rw-rw-   0     1001 root         (0)     2001 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/logout_requests/BackchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)      832 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     3841 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/logout_requests/GraphLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     1361 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/logout_requests/LogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     2229 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/perun/utils/logout_requests/SamlLogoutRequest.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:33:26.270116 perun.proxygui-4.1.1/perun.proxygui.egg-info/
--rw-r--r--   0     1001 root         (0)     9393 2024-04-23 07:33:26.000000 perun.proxygui-4.1.1/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)    12784 2024-04-23 07:33:26.000000 perun.proxygui-4.1.1/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-04-23 07:33:26.000000 perun.proxygui-4.1.1/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      584 2024-04-23 07:33:26.000000 perun.proxygui-4.1.1/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-04-23 07:33:26.000000 perun.proxygui-4.1.1/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-04-23 07:33:26.366115 perun.proxygui-4.1.1/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1523 2024-04-23 07:32:48.000000 perun.proxygui-4.1.1/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.169565 perun.proxygui-5.0.0/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       46 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)     9393 2024-04-23 07:38:19.169565 perun.proxygui-5.0.0/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     8072 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/api/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     2478 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0     1001 root         (0)     4517 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     4900 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0     1001 root         (0)    10193 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/heuristic_api.py
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/api/kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)     6876 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/app.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    22314 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/gui.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.117566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   141520 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)       99 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0     1001 root         (0)      612 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0     1001 root         (0)       67 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0     1001 root         (0)      688 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0     1001 root         (0)       19 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)      949 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0     1001 root         (0)     1663 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0     1001 root         (0)      477 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.117566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0     1001 root         (0)      631 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0     1001 root         (0)     1451 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0     1001 root         (0)     1617 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0     1001 root         (0)     1776 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0     1001 root         (0)      437 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0     1001 root         (0)      387 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0     1001 root         (0)     2945 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0     1001 root         (0)     2624 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0     1001 root         (0)      713 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0     1001 root         (0)     1899 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0     1001 root         (0)      815 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0     1001 root         (0)      571 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.125566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0     1001 root         (0)      421 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0     1001 root         (0)      403 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0     1001 root         (0)     2758 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.129566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0     1001 root         (0)      198 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0     1001 root         (0)      684 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0     1001 root         (0)    29997 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0     1001 root         (0)      244 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.117566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.129566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0     1001 root         (0)    22637 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    21057 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    22481 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0     1001 root         (0)    35533 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    34805 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    28733 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    20267 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28025 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    25884 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0     1001 root         (0)   363233 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0     1001 root         (0)    27013 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    33321 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    31511 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    34010 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28152 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    36726 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0     1001 root         (0)    28663 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0     1001 root         (0)    22030 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.133566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.145566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   125046 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0     1001 root         (0)   252563 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0     1001 root         (0)  1052500 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125125 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125144 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125123 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125119 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125120 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125147 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125545 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0     1001 root         (0)  1126098 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)   139176 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    48080 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.149566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    46987 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0     1001 root         (0)   303728 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   332353 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   332557 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0     1001 root         (0)     5778 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0     1001 root         (0)   312236 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   341456 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   341664 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0     1001 root         (0)     5772 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.149566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0     1001 root         (0)    87048 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    74284 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   208892 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0     1001 root         (0)   159376 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0     1001 root         (0)     1632 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0     1001 root         (0)     1837 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0     1001 root         (0)     1484 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0     1001 root         (0)      988 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0     1001 root         (0)    12252 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0     1001 root         (0)     9596 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.149566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.153566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0     1001 root         (0)    70841 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0     1001 root         (0)     4348 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0     1001 root         (0)      151 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0     1001 root         (0)      281 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0     1001 root         (0)      149 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0     1001 root         (0)      304 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0     1001 root         (0)     7406 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0     1001 root         (0)     4426 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0     1001 root         (0)      443 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.153566 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0     1001 root         (0)   218591 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0     1001 root         (0)   659454 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0     1001 root         (0)   337945 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0     1001 root         (0)     2707 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0     1001 root         (0)     8806 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0     1001 root         (0)    26171 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0     1001 root         (0)     4075 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0     1001 root         (0)   284394 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0     1001 root         (0)   610160 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.157565 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0     1001 root         (0)   155845 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0     1001 root         (0)   431289 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.157565 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0     1001 root         (0)    78743 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0     1001 root         (0)   325834 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0     1001 root         (0)       78 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0     1001 root         (0)     7336 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0     1001 root         (0)     4859 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.157565 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0     1001 root         (0)    73577 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0     1001 root         (0)    59305 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.161565 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0     1001 root         (0)   134294 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0     1001 root         (0)   747927 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0     1001 root         (0)   133988 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    89988 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    76736 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)    34034 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0     1001 root         (0)   144714 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0     1001 root         (0)    33736 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    16276 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0     1001 root         (0)    13224 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   203030 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0     1001 root         (0)   918991 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0     1001 root         (0)   202744 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0     1001 root         (0)   101648 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0     1001 root         (0)    78268 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.161565 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/
+-rw-rw-rw-   0     1001 root         (0)      490 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/check.svg
+-rw-rw-rw-   0     1001 root         (0)      536 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg
+-rw-rw-rw-   0     1001 root         (0)      483 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/questionmark.svg
+-rw-rw-rw-   0     1001 root         (0)      625 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/images/spinner.svg
+-rw-rw-rw-   0     1001 root         (0)    89501 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
+-rw-rw-rw-   0     1001 root         (0)      627 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/proxygui.css
+-rw-rw-rw-   0     1001 root         (0)     1427 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/proxygui.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.161565 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0     1001 root         (0)    15836 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0     1001 root         (0)     8266 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0     1001 root         (0)     8862 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0     1001 root         (0)     8873 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0     1001 root         (0)     7692 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0     1001 root         (0)     8344 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0     1001 root         (0)    11438 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.161565 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0     1001 root         (0)    64906 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/proxygui/gui/templates/
+-rw-rw-rw-   0     1001 root         (0)    15205 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0     1001 root         (0)     9192 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/HeuristicData.html
+-rw-rw-rw-   0     1001 root         (0)      747 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0     1001 root         (0)     3091 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/Logout.html
+-rw-rw-rw-   0     1001 root         (0)     1131 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
+-rw-rw-rw-   0     1001 root         (0)     1942 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html
+-rw-rw-rw-   0     1001 root         (0)     1133 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
+-rw-rw-rw-   0     1001 root         (0)     1021 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResult.html
+-rw-rw-rw-   0     1001 root         (0)      795 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/MissingAuth.html
+-rw-rw-rw-   0     1001 root         (0)     1019 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/OidcError.html
+-rw-rw-rw-   0     1001 root         (0)     1223 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/Post-logout.html
+-rw-rw-rw-   0     1001 root         (0)      907 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0     1001 root         (0)     2490 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0     1001 root         (0)     8103 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0     1001 root         (0)     1175 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0     1001 root         (0)     3477 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)      561 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/logout-iframe.html
+-rw-rw-rw-   0     1001 root         (0)     3769 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/templates/logout-state.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/translations/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0     1001 root         (0)     2973 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0     1001 root         (0)     8108 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0     1001 root         (0)     5372 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/jwt.py
+-rw-rw-rw-   0     1001 root         (0)    20220 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/logout_manager.py
+-rw-rw-rw-   0     1001 root         (0)     2480 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/oauth.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/proxygui/openapi/
+-rw-rw-rw-   0     1001 root         (0)     6107 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/openapi/openapi.py
+-rw-rw-rw-   0     1001 root         (0)    12933 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/openapi/openapi_data.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/proxygui/openapi/schemas/
+-rw-rw-rw-   0     1001 root         (0)      997 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py
+-rw-rw-rw-   0     1001 root         (0)     1446 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/openapi/schemas/response_schemas.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/proxygui/tests/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1816 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0     1001 root         (0)     6409 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     6635 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0     1001 root         (0)     4713 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2160 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0     1001 root         (0)     6826 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0     1001 root         (0)     1111 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/tests/test_kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)    22361 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/proxygui/user_manager.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/utils/
+-rw-rw-rw-   0     1001 root         (0)     2496 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/ConfigStore.py
+-rw-rw-rw-   0     1001 root         (0)       43 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/CustomExceptions.py
+-rw-rw-rw-   0     1001 root         (0)     2555 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/CustomRPHandler.py
+-rw-rw-rw-   0     1001 root         (0)     1354 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/DatabaseService.py
+-rw-rw-rw-   0     1001 root         (0)     4414 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/EmailService.py
+-rw-rw-rw-   0     1001 root         (0)       96 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/Notification.py
+-rw-rw-rw-   0     1001 root         (0)      816 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/Utils.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.165565 perun.proxygui-5.0.0/perun/utils/consent_framework/
+-rw-rw-rw-   0     1001 root         (0)     1241 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0     1001 root         (0)     2226 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2274 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0     1001 root         (0)     1371 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.169565 perun.proxygui-5.0.0/perun/utils/logout_requests/
+-rw-rw-rw-   0     1001 root         (0)     2001 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)      832 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     3841 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/logout_requests/GraphLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     1361 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/logout_requests/LogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     2229 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/perun/utils/logout_requests/SamlLogoutRequest.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 07:38:19.121566 perun.proxygui-5.0.0/perun.proxygui.egg-info/
+-rw-r--r--   0     1001 root         (0)     9393 2024-04-23 07:38:19.000000 perun.proxygui-5.0.0/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)    12784 2024-04-23 07:38:19.000000 perun.proxygui-5.0.0/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-04-23 07:38:19.000000 perun.proxygui-5.0.0/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      584 2024-04-23 07:38:19.000000 perun.proxygui-5.0.0/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-04-23 07:38:19.000000 perun.proxygui-5.0.0/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-04-23 07:38:19.169565 perun.proxygui-5.0.0/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1523 2024-04-23 07:37:48.000000 perun.proxygui-5.0.0/setup.py
```

### Comparing `perun.proxygui-4.1.1/LICENSE` & `perun.proxygui-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/PKG-INFO` & `perun.proxygui-5.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 4.1.1
+Version: 5.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
```

### Comparing `perun.proxygui-4.1.1/README.md` & `perun.proxygui-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-5.0.0/perun/proxygui/api/backchannel_logout_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,17 @@
     backchannel_logout_openapi_api = fs.Blueprint(
         "Backchannel logout API",
         __name__,
         url_prefix="/proxygui",
         description=apis_desc.get("backchannel_logout", ""),
     )
 
-    user_manager = UserManager(cfg)
+    BACKCHANEL_LOGOUT_API_CFG = cfg.get("backchannel_logout_api")
+
+    user_manager = UserManager(BACKCHANEL_LOGOUT_API_CFG)
 
     @openapi_route("/backchannel-logout", backchannel_logout_openapi_api)
     def perform_backchannel_logout() -> Response:
         try:
             client = get_client(logout_cfg)
         except Exception as ex:
             error_message = f"Error happened while getting client: {ex}"
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/api/ban_api.py` & `perun.proxygui-5.0.0/perun/proxygui/api/ban_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,17 +32,18 @@
 def construct_ban_api_blueprint(cfg):
     ban_openapi_api = fs.Blueprint(
         "Ban API",
         __name__,
         url_prefix="/proxygui",
         description=apis_desc.get("ban", ""),
     )
+    BAN_CFG = cfg.get("ban_api")
 
-    USER_MANAGER = UserManager(cfg)
-    UPLOAD_FILE_MAX_SIZE = int(cfg.get("max_ban_upload_filesize"))
+    USER_MANAGER = UserManager(BAN_CFG)
+    UPLOAD_FILE_MAX_SIZE = int(BAN_CFG.get("max_ban_upload_filesize"))
 
     # Endpoints
     @openapi_route("/banned-users/", ban_openapi_api)
     def update_banned_users() -> Response:
         process_update(request.get_json())
 
         response = flask.Response()
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/api/consent_api.py` & `perun.proxygui-5.0.0/perun/proxygui/api/consent_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,22 @@
 def construct_consent_api(cfg):
     consent_openapi_api = fs.Blueprint(
         "Consent API",
         __name__,
         url_prefix="/proxygui",
         description=apis_desc.get("consent", ""),
     )
-    db_manager = ConsentManager(cfg)
-    user_manager = UserManager(cfg)
+
+    CONSENT_CFG = cfg.get("consent_api")
+
+    db_manager = ConsentManager(CONSENT_CFG)
+    user_manager = UserManager(CONSENT_CFG)
     jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
 
-    oauth_cfg = cfg["oidc_provider"]
+    oauth_cfg = CONSENT_CFG["oidc_provider"]
 
     @openapi_route("/verify/<string:consent_id>", consent_openapi_api)
     def verify(consent_id):
         attrs = db_manager.fetch_consented_attributes(consent_id)
         if attrs:
             return jsonify(attrs)
         logger.debug("no consent found for id '%s'", consent_id)
@@ -102,15 +105,15 @@
     required_scopes = [" ".join(oauth_cfg["scopes"])]
 
     @openapi_route("/users/me/consents", consent_openapi_api)
     @require_oauth(required_scopes)
     def consents():
         scopes = current_token.scopes
         sub = scopes.get("sub")
-        issuer = cfg["oidc_provider"]["issuer"]
+        issuer = CONSENT_CFG["oidc_provider"]["issuer"]
         user_id = user_manager.sub_to_user_id(sub, issuer)
         if not user_id:
             error_message = f"Could not fetch user ID for subject ID '{sub}'"
             return Response(error_message, HTTPStatus.INTERNAL_SERVER_ERROR)
 
         user_consents = db_manager.fetch_all_user_consents(user_id)
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/api/heuristic_api.py` & `perun.proxygui-5.0.0/perun/proxygui/api/heuristic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         self.user_agents = None  # User agents and upstream logs
         self.time_result = None  # Many AuthEvent logs
         # Nunbers of retrieved rows from DB for various data
         self.few_time_logs = cfg["heuristic_page"]["few_time_logs"]
         self.some_time_logs = cfg["heuristic_page"]["some_time_logs"]
         self.many_time_logs = cfg["heuristic_page"]["many_time_logs"]
         # DB connect string
-        self.logging_db = cfg["auth_event_logging"]["logging_db"]
+        self.logging_db = cfg["heuristic_page"]["auth_event_logging"]["logging_db"]
         # REFEDS profile for MFA.
         self.REFEDS_MFA = "https://refeds.org/profile/mfa"
         # Microsoft authentication context for MFA.
         self.MS_MFA = "http://schemas.microsoft.com/claims/multipleauthn"
         # Contexts trusted as multifactor authentication, in the order of
         # preference (for replies).
         self.MFA_CONTEXTS = [self.REFEDS_MFA, self.MS_MFA]
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/api/kerberos_auth_api.py` & `perun.proxygui-5.0.0/perun/proxygui/api/kerberos_auth_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 def construct_kerberos_auth_api_blueprint(cfg):
     kerberos_openapi_auth_api = fs.Blueprint(
         "Kerberos API",
         __name__,
         url_prefix="/proxygui",
         description=apis_desc.get("kerberos", ""),
     )
+    KERBEROS_CFG = cfg.get("kerberos_api")
 
     @openapi_route("/AuthenticateKerberosTicket", kerberos_openapi_auth_api)
     def authenticate_kerberos_ticket():
         """
         Import done here to prevent other endpoints from being dependent on
         the kerberos
         module. Flask blueprints are assembled in one file and this process
@@ -50,15 +51,15 @@
                 "'Negotiate'. Incorrect format was provided in "
                 "authorization header."
             }, HTTPStatus.BAD_REQUEST
 
         b64_client_token = auth_header.removeprefix(required_prefix)
         client_token = base64.b64decode(b64_client_token).decode()
 
-        service_name = cfg["kerberos_service_name"]
+        service_name = KERBEROS_CFG["kerberos_service_name"]
         result, context = kerberos.authGSSServerInit(service_name)
         if result != kerberos.AUTH_GSS_COMPLETE:
             return {
                 "_text": "Error initializing Kerberos server context"
             }, HTTPStatus.INTERNAL_SERVER_ERROR
 
         result = kerberos.authGSSServerStep(context, client_token)
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/app.py` & `perun.proxygui-5.0.0/perun/proxygui/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         entity_conf=[{"class": RPHConfiguration, "attr": "rp"}],
         filename=cfg_path,
     )
 
 
 def get_oidc_auth(cfg, app: Flask):
     oidc_cfg = cfg["oidc_provider"]
+
     app.config.update(OIDC_REDIRECT_URI=oidc_cfg["oidc_redirect_uri"])
 
     client_metadata = ClientMetadata(
         client_id=oidc_cfg["client_id"],
         client_secret=oidc_cfg["client_secret"],
         post_logout_redirect_uris=oidc_cfg["post_logout_redirect_uris"],
     )
@@ -121,44 +122,63 @@
         app.config["SESSION_MONGODB_COLLECT"] = cfg["session_database"][
             "collection_name"
         ]
         Session(app)
 
     app, api = api_setup(app, openapi_version)
 
-    @app.context_processor
-    def inject_conf_var():
-        return dict(cfg=cfg, lang=get_locale())
-
-    # initialize OIDC
-    auth = get_oidc_auth(cfg, app)
-
-    # Register GUI component
-    app.register_blueprint(construct_gui_blueprint(cfg, auth))
-
-    # Register API endpoints
-    api.register_blueprint(construct_ban_api_blueprint(cfg))
-
-    api.register_blueprint(construct_kerberos_auth_api_blueprint(cfg))
-    # to avoid breaking change
-
-    if "consent" in cfg:
-        oauth_cfg = cfg["oidc_provider"]
+    # Optional GUI
+    if isinstance(cfg.get("gui", None), dict):
+        # initialize OIDC
+        auth = get_oidc_auth(cfg.get("gui", None), app)
+
+        @app.context_processor
+        def inject_conf_var():
+            gui_cfg = cfg.get("gui")
+            html_dict = gui_cfg.get("html")
+            all_html_dict = {
+                **html_dict,
+                "general_translations": gui_cfg.get("general_translations"),
+                "mfa_reset_translations": gui_cfg.get("mfa_reset").get(
+                    "mfa_reset_translations"
+                ),
+            }
+
+            return dict(cfg=all_html_dict, lang=get_locale())
+
+        # Register GUI component
+        app.register_blueprint(construct_gui_blueprint(cfg, auth))
+
+    # Optional Ban API
+    if isinstance(cfg.get("ban_api", None), dict):
+        # Register API endpoints
+        api.register_blueprint(construct_ban_api_blueprint(cfg))
+
+    # Optional Kerberos API
+    if isinstance(cfg.get("kerberos_api", None), dict):
+        api.register_blueprint(construct_kerberos_auth_api_blueprint(cfg))
+        # to avoid breaking change
+
+    # Optional Consent API
+    if isinstance(cfg.get("consent_api", None), dict):
+        oauth_cfg = cfg["consent_api"]["oidc_provider"]
         configure_resource_protector(oauth_cfg)
 
         api.register_blueprint(construct_consent_api(cfg))
 
-    logout_cfg = ConfigStore.get_config(BACKCHANNEL_LOGOUT_CFG, False)
-    if logout_cfg:
-        api.register_blueprint(
-            construct_backchannel_logout_api_blueprint(cfg, logout_cfg)
-        )
+    # Optional Backchannel logout API
+    if isinstance(cfg.get("backchannel_logout_api", None), dict):
+        logout_cfg = ConfigStore.get_config(BACKCHANNEL_LOGOUT_CFG, False)
+        if logout_cfg:
+            api.register_blueprint(
+                construct_backchannel_logout_api_blueprint(cfg, logout_cfg)
+            )
 
-        # Initialize the oidc_provider after views to be able to set correct urls
-        app.rp_handler = init_oidc_rp_handler()
+            # Initialize the oidc_provider after views to be able to set correct urls
+            app.rp_handler = init_oidc_rp_handler()
 
     if return_with_api:
         return app, api
     return app
 
 
 # for uWSGI
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/gui.py` & `perun.proxygui-5.0.0/perun/proxygui/gui/gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,24 +71,27 @@
     gui = Blueprint(
         "gui",
         __name__,
         template_folder="templates",
         url_prefix="/proxygui",
         static_folder="static",
     )
-    consent_db_manager = ConsentManager(cfg)
-    user_manager = UserManager(cfg)
-    jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
-    logout_manager = LogoutManager(cfg)
-    auth_event = AuthEventLoggingQueries(cfg)
 
-    REDIRECT_URL = cfg["redirect_url"]
+    GUI_CFG = cfg.get("gui")
+    REDIRECT_URL = GUI_CFG["redirect_url"]
     COLOR = cfg["bootstrap_color"]
-    OIDC_CFG = cfg["oidc_provider"]
-    MFA_CFG = cfg["mfa_provider"]
+    OIDC_CFG = GUI_CFG["oidc_provider"]
+    MFA_CFG = GUI_CFG["mfa_provider"]
+
+    consent_db_manager = ConsentManager(GUI_CFG)
+    user_manager = UserManager(GUI_CFG)
+
+    jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
+    logout_manager = LogoutManager(GUI_CFG)
+    auth_event = AuthEventLoggingQueries(GUI_CFG)
 
     @gui.route("/authorization/<token>")
     def authorization(token):
         try:
             message = jwt_service.verify_jwt(token)
         except InvalidJWTError as e:
             return make_response(
@@ -127,412 +130,444 @@
             "SPAuthorization.html",
             email=email,
             service=service,
             registration_url=registration_url,
             bootstrap_color=COLOR,
         )
 
-    @gui.route("/logout", methods=["POST", "GET"])
-    def logout():
-        ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
-
-        logger.debug(f"Logout call for SimpleSAMLSessionID: {ssp_session_id}")
-        # todo - dbs will contain user_id and won't need to be converted in the future
-        sub = user_manager.get_user_id_by_ssp_session_id(ssp_session_id)
-
-        if ssp_session_id is None or sub is None:
-            return render_template("MissingAuth.html")
-
-        (
-            valid_request,
-            client_id,
-            rp_sid,
-            issuer,
-            logout_params,
-        ) = logout_manager.validate_request_and_extract_params(ssp_session_id, request)
-
-        if valid_request:
-            user_manager.logout_from_service_op(sub, ssp_session_id, client_id)
-
-        device_active_clients = user_manager.get_active_client_ids_for_user(sub)
-        session_active_clients = user_manager.get_active_client_ids_for_session(
-            request.cookies.get("SimpleSAMLSessionID")
-        )
+    # Logout ==================================================================================
+    if GUI_CFG.get("logout", None):
 
-        rp_names = user_manager.get_all_rp_names()
-        logged_out_service = (
-            {
-                "from_devices": rp_sid is None,
-                # user might have been logged out for all devices
-                "labels": rp_names.get(client_id, client_id),
-                "client_id": client_id,
-            }
-            if client_id is not None
-            else {}
-        )
+        @gui.route("/logout", methods=["POST", "GET"])
+        def logout():
+            ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
+
+            logger.debug(f"Logout call for SimpleSAMLSessionID: {ssp_session_id}")
+            # todo - dbs will contain user_id and won't need to be converted in the future
+            sub = user_manager.get_user_id_by_ssp_session_id(ssp_session_id)
 
-        session_services = logout_manager.complete_service_names(
-            session_active_clients, rp_names
-        )
-        device_services = logout_manager.complete_service_names(
-            device_active_clients, rp_names
-        )
-        session["logout_params"] = logout_params if logout_params else {}
-        session["init_logged_out_service"] = logged_out_service
-        session["init_issuer"] = issuer  # todo - we probably don't need to save it
-
-        resp = make_response(
-            render_template(
-                "Logout.html",
-                logged_out_service=logged_out_service,
-                session_services=session_services,
-                device_services=device_services,
-                default_postlogout_uri=cfg.get("default_postlogout_uri"),
-                bootstrap_color=COLOR,
-            )
-        )
-        return resp
+            if ssp_session_id is None or sub is None:
+                return render_template("MissingAuth.html")
 
-    @gui.route("/logout_state", methods=["GET"])
-    def logout_state():
-        if session.get("logout_params") is None:
-            # at least empty dict should be set, or logout endpoint was not visited
-            return redirect(url_for("gui.logout", _external=True))
-
-        ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
-        # todo - dbs will contain user_id and won't need to be converted in the future
-        sub = user_manager.get_user_id_by_ssp_session_id(ssp_session_id)
-
-        if ssp_session_id is None or sub is None:
-            return render_template("MissingAuth.html")
-
-        include_all_devices = request.args.get("from_devices", False)
-        include_all_devices = include_all_devices in ["True", True, "true"]
-
-        if include_all_devices:
-            active_clients = user_manager.get_active_client_ids_for_user(sub)
-            unique_client_issuer_clients = []
-            for client_id, sid, issuer in active_clients:
-                found = next(
-                    filter(
-                        lambda x: x[0] == client_id and x[2] == issuer,
-                        unique_client_issuer_clients,
-                    ),
-                    None,
-                )
-                (
-                    unique_client_issuer_clients.append((client_id, sid, issuer))
-                    if not found
-                    else None
-                )
-                active_clients = unique_client_issuer_clients
-        else:
-            active_clients = user_manager.get_active_client_ids_for_session(
-                ssp_session_id
-            )
-
-        rp_names = user_manager.get_all_rp_names()
-        # todo - jazyky brát z config option languages - brát průnik,
-        #  issuer bude mapa {issuer: pretty_name}
-        # todo - pěkná funkce na vyčítání (fallback když je jenom japonská verze atd...)
-        service_configs = logout_manager.services_configuration
-        logout_requests = [
-            logout_manager.prepare_logout_request(
-                service_configs,
+            (
+                valid_request,
                 client_id,
-                sub,
-                rp_names.get(client_id, {"en": client_id, "cs": client_id}),
+                rp_sid,
                 issuer,
-                rp_sid if include_all_devices else None,
-            ).to_dict()
-            for (client_id, rp_sid, issuer) in active_clients
-        ]
-
-        session["logout_requests"] = logout_requests
-        init_logged_out_client_id = session["init_logged_out_service"].get("client_id")
-        session["init_logged_out_service"]["logback_url"] = (
-            service_configs.get("RPS", {})
-            .get(init_logged_out_client_id, {})
-            .get("logback_url")
-        )
-
-        main_issuer = cfg.get("issuers", [{}])[0].get("issuer")
-        if not main_issuer:
-            logger.error("Main issuer not set!")
-            return make_response(
-                jsonify({gettext("fail"): "Invalid endpoint configuration."}),
-                400,
+                logout_params,
+            ) = logout_manager.validate_request_and_extract_params(
+                ssp_session_id, request
+            )
+
+            if valid_request:
+                user_manager.logout_from_service_op(sub, ssp_session_id, client_id)
+
+            device_active_clients = user_manager.get_active_client_ids_for_user(sub)
+            session_active_clients = user_manager.get_active_client_ids_for_session(
+                request.cookies.get("SimpleSAMLSessionID")
+            )
+
+            rp_names = user_manager.get_all_rp_names()
+            logged_out_service = (
+                {
+                    "from_devices": rp_sid is None,
+                    # user might have been logged out for all devices
+                    "labels": rp_names.get(client_id, client_id),
+                    "client_id": client_id,
+                }
+                if client_id is not None
+                else {}
+            )
+
+            session_services = logout_manager.complete_service_names(
+                session_active_clients, rp_names
+            )
+            device_services = logout_manager.complete_service_names(
+                device_active_clients, rp_names
+            )
+            session["logout_params"] = logout_params if logout_params else {}
+            session["init_logged_out_service"] = logged_out_service
+            session["init_issuer"] = issuer  # todo - we probably don't need to save it
+
+            resp = make_response(
+                render_template(
+                    "Logout.html",
+                    logged_out_service=logged_out_service,
+                    session_services=session_services,
+                    device_services=device_services,
+                    default_postlogout_uri=cfg.get("logout", {}).get(
+                        "default_postlogout_uri"
+                    ),
+                    bootstrap_color=COLOR,
+                )
             )
-        user_id = user_manager.sub_to_user_id(sub, main_issuer)
-        if not user_id:
-            return render_template("MissingAuth.html")
-        user_manager.logout(
-            user_id=user_id,
-            session_id=ssp_session_id if include_all_devices else None,
-            include_refresh_tokens=include_all_devices,
-        )
+            return resp
 
-        resp = make_response(
-            render_template(
-                "logout-state.html",
-                session_services=logout_requests if not include_all_devices else [],
-                device_services=logout_requests if include_all_devices else [],
-                bootstrap_color=COLOR,
+        @gui.route("/logout_state", methods=["GET"])
+        def logout_state():
+            if session.get("logout_params") is None:
+                # at least empty dict should be set, or logout endpoint was not visited
+                return redirect(url_for("gui.logout", _external=True))
+
+            ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
+            # todo - dbs will contain user_id and won't need to be converted in the future
+            sub = user_manager.get_user_id_by_ssp_session_id(ssp_session_id)
+
+            if ssp_session_id is None or sub is None:
+                return render_template("MissingAuth.html")
+
+            include_all_devices = request.args.get("from_devices", False)
+            include_all_devices = include_all_devices in ["True", True, "true"]
+
+            if include_all_devices:
+                active_clients = user_manager.get_active_client_ids_for_user(sub)
+                unique_client_issuer_clients = []
+                for client_id, sid, issuer in active_clients:
+                    found = next(
+                        filter(
+                            lambda x: x[0] == client_id and x[2] == issuer,
+                            unique_client_issuer_clients,
+                        ),
+                        None,
+                    )
+                    (
+                        unique_client_issuer_clients.append((client_id, sid, issuer))
+                        if not found
+                        else None
+                    )
+                    active_clients = unique_client_issuer_clients
+            else:
+                active_clients = user_manager.get_active_client_ids_for_session(
+                    ssp_session_id
+                )
+
+            rp_names = user_manager.get_all_rp_names()
+            # todo - jazyky brát z config option languages - brát průnik,
+            #  issuer bude mapa {issuer: pretty_name}
+            # todo - pěkná funkce na vyčítání (fallback když je jenom japonská verze atd...)
+            service_configs = logout_manager.services_configuration
+            logout_requests = [
+                logout_manager.prepare_logout_request(
+                    service_configs,
+                    client_id,
+                    sub,
+                    rp_names.get(client_id, {"en": client_id, "cs": client_id}),
+                    issuer,
+                    rp_sid if include_all_devices else None,
+                ).to_dict()
+                for (client_id, rp_sid, issuer) in active_clients
+            ]
+
+            session["logout_requests"] = logout_requests
+            init_logged_out_client_id = session["init_logged_out_service"].get(
+                "client_id"
+            )
+            session["init_logged_out_service"]["logback_url"] = (
+                service_configs.get("RPS", {})
+                .get(init_logged_out_client_id, {})
+                .get("logback_url")
+            )
+
+            main_issuer = cfg.get("issuers", [{}])[0].get("issuer")
+            if not main_issuer:
+                logger.error("Main issuer not set!")
+                return make_response(
+                    jsonify({gettext("fail"): "Invalid endpoint configuration."}),
+                    400,
+                )
+            user_id = user_manager.sub_to_user_id(sub, main_issuer)
+            if not user_id:
+                return render_template("MissingAuth.html")
+            user_manager.logout(
+                user_id=user_id,
+                session_id=ssp_session_id if include_all_devices else None,
+                include_refresh_tokens=include_all_devices,
             )
-        )
-        resp.delete_cookie("SimpleSAMLSessionID")
-        return resp
 
-    @gui.route("/post_logout")
-    def post_logout():
-        logout_params = session.get("logout_params")
-        init_logged_out_service = session.get("init_logged_out_service")
-        session.clear()
-
-        if (
-            logout_params is None or init_logged_out_service is None
-        ):  # can be {} but not None (wrong flow then)
-            return render_template("MissingAuth.html")
-
-        if "post_logout_redirect_uri" in logout_params:
-            url = logout_params["post_logout_redirect_uri"]
-            if "state" in logout_params:
-                state = parse.quote(logout_params["state"])
-                url = f"{url}?{state}" if "?" not in url else f"{url}&{state}"
-            return redirect(url)
+            resp = make_response(
+                render_template(
+                    "logout-state.html",
+                    session_services=logout_requests if not include_all_devices else [],
+                    device_services=logout_requests if include_all_devices else [],
+                    bootstrap_color=COLOR,
+                )
+            )
+            resp.delete_cookie("SimpleSAMLSessionID")
+            return resp
 
-        return render_template(
-            "Post-logout.html",
-            init_logged_out_service=init_logged_out_service,
-            bootstrap_color=COLOR,
-        )
+        @gui.route("/post_logout")
+        def post_logout():
+            logout_params = session.get("logout_params")
+            init_logged_out_service = session.get("init_logged_out_service")
+            session.clear()
+
+            if (
+                logout_params is None or init_logged_out_service is None
+            ):  # can be {} but not None (wrong flow then)
+                return render_template("MissingAuth.html")
+
+            if "post_logout_redirect_uri" in logout_params:
+                url = logout_params["post_logout_redirect_uri"]
+                if "state" in logout_params:
+                    state = parse.quote(logout_params["state"])
+                    url = f"{url}?{state}" if "?" not in url else f"{url}&{state}"
+                return redirect(url)
 
-    @gui.route("/logout_iframe_callback", methods=["GET"])
-    def logout_iframe_callback():
-        request_id = request.args.get("request_id")
-        logout_requests = session["logout_requests"]
+            return render_template(
+                "Post-logout.html",
+                init_logged_out_service=init_logged_out_service,
+                bootstrap_color=COLOR,
+            )
 
-        current_request = next(
-            (r for r in logout_requests if str(r["id"]) == request_id), None
-        )
+        @gui.route("/logout_iframe_callback", methods=["GET"])
+        def logout_iframe_callback():
+            request_id = request.args.get("request_id")
+            logout_requests = session["logout_requests"]
+
+            current_request = next(
+                (r for r in logout_requests if str(r["id"]) == request_id), None
+            )
 
-        if current_request is None:
-            response = False
-        else:
-            req = logout_manager.deserialize_request(current_request)
-            response = req.logout()
-        return render_template(
-            "logout-iframe.html",
-            result="success" if response else response,
-        )
+            if current_request is None:
+                response = False
+            else:
+                req = logout_manager.deserialize_request(current_request)
+                response = req.logout()
+            return render_template(
+                "logout-iframe.html",
+                result="success" if response else response,
+            )
 
-    @gui.route("/logout_saml_callback/<issuer_id>", methods=["GET"])
-    def logout_saml_callback(issuer_id):
-        request_ok = logout_manager.check_saml_callback(request, issuer_id)
+        @gui.route("/logout_saml_callback/<issuer_id>", methods=["GET"])
+        def logout_saml_callback(issuer_id):
+            request_ok = logout_manager.check_saml_callback(request, issuer_id)
 
-        return render_template(
-            "logout-iframe.html",
-            result="success" if request_ok else "request invalid",
-        )
+            return render_template(
+                "logout-iframe.html",
+                result="success" if request_ok else "request invalid",
+            )
 
-    @gui.route("/IsTestingSP")
-    def is_testing_sp():
-        return render_template(
-            "IsTestingSP.html",
-            redirect_url=REDIRECT_URL,
-            bootstrap_color=COLOR,
-        )
+    # Testing ==================================================================================
+    if GUI_CFG.get("is_testing_sp", None):
 
-    @gui.route("/consent/<token>")
-    def consent(token):
-        try:
-            ticket = jwt_service.verify_jwt(token)
-        except InvalidJWTError as e:
-            return make_response(
-                jsonify({gettext("fail"): f"JWT validation failed with error: '{e}'"}),
-                400,
-            )
-        data = consent_db_manager.fetch_consent_request(ticket)
-        if not ticket:
-            return make_response(
-                jsonify({gettext("fail"): gettext("received invalid ticket")}),
-                400,
+        @gui.route("/IsTestingSP")
+        def is_testing_sp():
+            return render_template(
+                "IsTestingSP.html",
+                redirect_url=REDIRECT_URL,
+                bootstrap_color=COLOR,
             )
 
-        months_valid = cfg["consent"]["months_valid"]
-        session["id"] = data["id"]
-        session["state"] = uuid4().urn
-        session["redirect_endpoint"] = data["redirect_endpoint"]
-        session["attr"] = ignore_claims(cfg["consent"]["ignored_claims"], data["attr"])
-        session["user_id"] = data["user_id"]
-        session["locked_attrs"] = data.get("locked_attrs")
-        session["requester_name"] = data["requester_name"]
-        session["month"] = months_valid
-
-        warning = cfg["consent"].get("warning", None)
-        with open(
-            cfg["consent"]["attribute_config_path"],
-            "r",
-            encoding="utf8",
-        ) as ymlfile:
-            attr_config = yaml.safe_load(ymlfile)
+    # Consent ==================================================================================
+    if GUI_CFG.get("consent", None):
 
-        return render_template(
-            "ConsentRegistration.html",
-            bootstrap_color=COLOR,
-            cfg=cfg,
-            attr_config=attr_config,
-            released_claims=copy.deepcopy(session["attr"]),
-            locked_claims=session["locked_attrs"],
-            requester_name=session["requester_name"],
-            months=months_valid,
-            data_protection_redirect=data["data_protection_redirect"],
-            warning=warning,
-        )
+        @gui.route("/consent/<token>")
+        def consent(token):
+            try:
+                ticket = jwt_service.verify_jwt(token)
+            except InvalidJWTError as e:
+                return make_response(
+                    jsonify(
+                        {gettext("fail"): f"JWT validation failed with error: '{e}'"}
+                    ),
+                    400,
+                )
+            data = consent_db_manager.fetch_consent_request(ticket)
+            if not ticket:
+                return make_response(
+                    jsonify({gettext("fail"): gettext("received invalid ticket")}),
+                    400,
+                )
+
+            months_valid = GUI_CFG["consent"]["months_valid"]
+            session["id"] = data["id"]
+            session["state"] = uuid4().urn
+            session["redirect_endpoint"] = data["redirect_endpoint"]
+            session["attr"] = ignore_claims(
+                GUI_CFG["consent"]["ignored_claims"], data["attr"]
+            )
+            session["user_id"] = data["user_id"]
+            session["locked_attrs"] = data.get("locked_attrs")
+            session["requester_name"] = data["requester_name"]
+            session["month"] = months_valid
+
+            warning = GUI_CFG["consent"].get("warning", None)
+            with open(
+                GUI_CFG["consent"]["attribute_config_path"],
+                "r",
+                encoding="utf8",
+            ) as ymlfile:
+                attr_config = yaml.safe_load(ymlfile)
 
-    @gui.route("/mfa-reset-verify/<token>")
-    @auth.oidc_auth(OIDC_CFG["provider_name"])
-    def mfa_reset_verify(token):
-        try:
-            reset_request = jwt_service.verify_jwt(token)
-        except InvalidJWTError:
             return render_template(
-                "MfaResult.html", title="request_fail_title", info="request_fail_info"
+                "ConsentRegistration.html",
+                bootstrap_color=COLOR,
+                cfg=cfg,
+                attr_config=attr_config,
+                released_claims=copy.deepcopy(session["attr"]),
+                locked_claims=session["locked_attrs"],
+                requester_name=session["requester_name"],
+                months=months_valid,
+                data_protection_redirect=data["data_protection_redirect"],
+                warning=warning,
+            )
+
+    # MFA ==================================================================================
+    if GUI_CFG.get("mfa_reset", None):
+
+        @gui.route("/mfa-reset-verify/<token>")
+        @auth.oidc_auth(OIDC_CFG["provider_name"])
+        def mfa_reset_verify(token):
+            try:
+                reset_request = jwt_service.verify_jwt(token)
+            except InvalidJWTError:
+                return render_template(
+                    "MfaResult.html",
+                    title="request_fail_title",
+                    info="request_fail_info",
+                )
+            requester_email = reset_request.get("requester_email")
+            user_manager.forward_mfa_reset_request(requester_email)
+            return render_template(
+                "MfaResult.html",
+                title="request_success_title",
+                info="request_success_info",
             )
-        requester_email = reset_request.get("requester_email")
-        user_manager.forward_mfa_reset_request(requester_email)
-        return render_template(
-            "MfaResult.html", title="request_success_title", info="request_success_info"
-        )
 
-    @gui.route("/send-mfa-reset-emails")
-    @auth.oidc_auth(OIDC_CFG["provider_name"])
-    def send_mfa_reset_emails():
-        user_session = UserSession(flask.session, OIDC_CFG["provider_name"])
-        sub = user_session.userinfo.get("sub")
-        issuer = OIDC_CFG["issuer"]
-        user_id = user_manager.sub_to_user_id(sub, issuer)
-        if not user_id:
-            return f"No corresponding user found for sub: '{sub}'", HTTPStatus.NOT_FOUND
-
-        locale = get_locale().language
-        preferred_email = user_manager.handle_mfa_reset(
-            user_id,
-            locale,
-            url_for("gui.mfa_reset_verify", token=jwt_service.get_jwt()),
-            NotificationType.VERIFICATION,
-        )
-        return render_template(
-            "MfaResetEmailSent.html",
-            email=preferred_email,
-        )
-
-    @gui.route("/mfa-reset")
-    @auth.oidc_auth(OIDC_CFG["provider_name"])
-    def mfa_reset():
-        return render_template(
-            "MfaResetInitiated.html",
-            redirect_url=REDIRECT_URL,
-            bootstrap_color=COLOR,
-            referrer=request.referrer or "/",
-            next_action=url_for("gui.send_mfa_reset_emails"),
-        )
+        @gui.route("/send-mfa-reset-emails")
+        @auth.oidc_auth(OIDC_CFG["provider_name"])
+        def send_mfa_reset_emails():
+            user_session = UserSession(flask.session, OIDC_CFG["provider_name"])
+            sub = user_session.userinfo.get("sub")
+            issuer = OIDC_CFG["issuer"]
+            user_id = user_manager.sub_to_user_id(sub, issuer)
+            if not user_id:
+                return (
+                    f"No corresponding user found for sub: '{sub}'",
+                    HTTPStatus.NOT_FOUND,
+                )
 
-    @gui.route("/mfa-perform-delegated-reset")
-    @auth.oidc_auth(MFA_CFG["provider_name"])
-    def mfa_perform_delegated_reset():
-        if not session.get("mfa_reset_visited"):
-            # force user to confirm this action
-            return redirect(url_for("gui.mfa_delegated_reset"))
-        user_session = UserSession(flask.session, MFA_CFG["provider_name"])
-        username = user_session.id_token.get("sub")
-        locale = get_locale().language
-        tokens = logout_manager.remove_mfa_tokens(username)
-
-        if tokens > 0:
-            issuer = MFA_CFG["issuer"]
-            user_id = user_manager.sub_to_user_id(username, issuer)
-            user_manager.handle_mfa_reset(
+            locale = get_locale().language
+            preferred_email = user_manager.handle_mfa_reset(
                 user_id,
                 locale,
-                None,
-                NotificationType.CONFIRMATION,
+                url_for("gui.mfa_reset_verify", token=jwt_service.get_jwt()),
+                NotificationType.VERIFICATION,
             )
             return render_template(
-                "MfaResult.html",
-                title="delegated_successful_title",
-                info="delegated_successful_info",
+                "MfaResetEmailSent.html",
+                email=preferred_email,
             )
-        else:
-            session["mfa_reset_success"] = True
+
+        @gui.route("/mfa-reset")
+        @auth.oidc_auth(OIDC_CFG["provider_name"])
+        def mfa_reset():
             return render_template(
-                "MfaResult.html",
-                title="delegated_failed_title",
-                info="delegated_failed_info",
+                "MfaResetInitiated.html",
+                redirect_url=REDIRECT_URL,
+                bootstrap_color=COLOR,
+                referrer=request.referrer or "/",
+                next_action=url_for("gui.send_mfa_reset_emails"),
             )
 
-    @gui.route("/mfa-delegated-reset")
-    @auth.oidc_auth(MFA_CFG["provider_name"])
-    def mfa_delegated_reset():
-        session["mfa_reset_visited"] = True
-        return render_template(
-            "MfaResetInitiated.html",
-            redirect_url=REDIRECT_URL,
-            bootstrap_color=COLOR,
-            referrer=request.referrer or "/",
-            next_action=url_for("gui.mfa_perform_delegated_reset"),
-        )
+        @gui.route("/mfa-perform-delegated-reset")
+        @auth.oidc_auth(MFA_CFG["provider_name"])
+        def mfa_perform_delegated_reset():
+            if not session.get("mfa_reset_visited"):
+                # force user to confirm this action
+                return redirect(url_for("gui.mfa_delegated_reset"))
+            user_session = UserSession(flask.session, MFA_CFG["provider_name"])
+            username = user_session.id_token.get("sub")
+            locale = get_locale().language
+            tokens = logout_manager.remove_mfa_tokens(username)
+
+            if tokens > 0:
+                issuer = MFA_CFG["issuer"]
+                user_id = user_manager.sub_to_user_id(username, issuer)
+                user_manager.handle_mfa_reset(
+                    user_id,
+                    locale,
+                    None,
+                    NotificationType.CONFIRMATION,
+                )
+                return render_template(
+                    "MfaResult.html",
+                    title="delegated_successful_title",
+                    info="delegated_successful_info",
+                )
+            else:
+                session["mfa_reset_success"] = True
+                return render_template(
+                    "MfaResult.html",
+                    title="delegated_failed_title",
+                    info="delegated_failed_info",
+                )
 
-    @gui.route("/HeuristicGetID")
-    @auth.oidc_auth(OIDC_CFG["provider_name"])
-    def heuristic_get_id():
-        if not check_scope_claim("heuristic_pages", OIDC_CFG):
-            return "User does not have access to this page", HTTPStatus.FORBIDDEN
+        @gui.route("/mfa-delegated-reset")
+        @auth.oidc_auth(MFA_CFG["provider_name"])
+        def mfa_delegated_reset():
+            session["mfa_reset_visited"] = True
+            return render_template(
+                "MfaResetInitiated.html",
+                redirect_url=REDIRECT_URL,
+                bootstrap_color=COLOR,
+                referrer=request.referrer or "/",
+                next_action=url_for("gui.mfa_perform_delegated_reset"),
+            )
 
-        return render_template(
-            "HeuristicData.html",
-            redirect_url=REDIRECT_URL,
-            bootstrap_color=COLOR,
-            selected=False,
-        )
+    # Heuristic ==================================================================================
+    if GUI_CFG.get("heuristic_page", None):
 
-    @gui.route("/GetHeuristic", methods=["GET"])
-    @auth.oidc_auth(OIDC_CFG["provider_name"])
-    def get_heuristic():
-        user_id = request.args.get("user")
-        if not user_id:
-            return "User ID not provided in the request", HTTPStatus.BAD_REQUEST
+        @gui.route("/HeuristicGetID")
+        @auth.oidc_auth(OIDC_CFG["provider_name"])
+        def heuristic_get_id():
+            if not check_scope_claim("heuristic_pages", OIDC_CFG):
+                return "User does not have access to this page", HTTPStatus.FORBIDDEN
 
-        if not check_scope_claim("heuristic_pages", OIDC_CFG):
-            return "User does not have access to this page", HTTPStatus.FORBIDDEN
+            return render_template(
+                "HeuristicData.html",
+                redirect_url=REDIRECT_URL,
+                bootstrap_color=COLOR,
+                selected=False,
+            )
 
-        try:
-            user_id = int(user_id)
-        except ValueError:
-            return (
-                f"Provided user ID: '{user_id}' could not be converted to an "
-                f"integer"
-            ), HTTPStatus.BAD_REQUEST
+        @gui.route("/GetHeuristic", methods=["GET"])
+        @auth.oidc_auth(OIDC_CFG["provider_name"])
+        def get_heuristic():
+            user_id = request.args.get("user")
+            if not user_id:
+                return "User ID not provided in the request", HTTPStatus.BAD_REQUEST
+
+            if not check_scope_claim("heuristic_pages", OIDC_CFG):
+                return "User does not have access to this page", HTTPStatus.FORBIDDEN
+
+            try:
+                user_id = int(user_id)
+            except ValueError:
+                return (
+                    f"Provided user ID: '{user_id}' could not be converted to an "
+                    f"integer"
+                ), HTTPStatus.BAD_REQUEST
 
-        name = user_manager.get_user_name(user_id)
-        auth_event.get_auth_logs(user_id)
+            name = user_manager.get_user_name(user_id)
+            auth_event.get_auth_logs(user_id)
 
-        return render_template(
-            "HeuristicData.html",
-            redirect_url=REDIRECT_URL,
-            bootstrap_color=COLOR,
-            selected=True,
-            user=user_id,
-            name=name,
-            last_n_times=auth_event.get_last_n_times(),
-            user_agents=auth_event.get_unique_user_agents(),
-            last_n_cities=auth_event.get_last_n_cities(),
-            sps=auth_event.get_last_n_services(),
-            ips=auth_event.get_last_n_ips(),
-        )
+            return render_template(
+                "HeuristicData.html",
+                redirect_url=REDIRECT_URL,
+                bootstrap_color=COLOR,
+                selected=True,
+                user=user_id,
+                name=name,
+                last_n_times=auth_event.get_last_n_times(),
+                user_agents=auth_event.get_unique_user_agents(),
+                last_n_cities=auth_event.get_last_n_cities(),
+                sps=auth_event.get_last_n_services(),
+                ips=auth_event.get_last_n_ips(),
+            )
 
     @gui.route("/oidc-error")
     def display_oidc_error_screen():
         return render_template(
             "OidcError.html",
             title="oidc_error_title",
             info="oidc_error_info",
```

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/images/circle-check-regular.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/images/circle-check-regular.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/images/questionmark.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/images/questionmark.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/images/spinner.svg` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/images/spinner.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/proxygui.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/proxygui.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/proxygui.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/proxygui.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-5.0.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/HeuristicData.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/HeuristicData.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/Logout.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/Logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetEmailSent.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetEmailSent.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetInitiated.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetInitiated.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/MfaResult.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/MfaResult.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/MissingAuth.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/MissingAuth.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/OidcError.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/OidcError.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/Post-logout.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/Post-logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/base.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/logout-iframe.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/logout-iframe.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/templates/logout-state.html` & `perun.proxygui-5.0.0/perun/proxygui/gui/templates/logout-state.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-5.0.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/jwt.py` & `perun.proxygui-5.0.0/perun/proxygui/jwt.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/logout_manager.py` & `perun.proxygui-5.0.0/perun/proxygui/logout_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/oauth.py` & `perun.proxygui-5.0.0/perun/proxygui/oauth.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/openapi/openapi.py` & `perun.proxygui-5.0.0/perun/proxygui/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/openapi/openapi_data.py` & `perun.proxygui-5.0.0/perun/proxygui/openapi/openapi_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/openapi/schemas/arguments_schemas.py` & `perun.proxygui-5.0.0/perun/proxygui/openapi/schemas/arguments_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/openapi/schemas/response_schemas.py` & `perun.proxygui-5.0.0/perun/proxygui/openapi/schemas/response_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/shared_test_data.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/shared_test_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_gui.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/tests/test_kerberos_auth_api.py` & `perun.proxygui-5.0.0/perun/proxygui/tests/test_kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/proxygui/user_manager.py` & `perun.proxygui-5.0.0/perun/proxygui/user_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,47 @@
 from perun.utils.DatabaseService import DatabaseService
 from perun.utils.EmailService import EmailService
 from perun.utils.Notification import NotificationType
 
 
 class UserManager:
     def __init__(self, cfg):
-        GLOBAL_CONFIG = ConfigStore.get_global_cfg(cfg.get("global_cfg_filepath"))
+        USER_MANAGER_CFG = cfg.get("user_manager", {})
+        GLOBAL_CONFIG = ConfigStore.get_global_cfg(
+            USER_MANAGER_CFG.get("global_cfg_filepath")
+        )
         ADAPTERS_MANAGER_CFG = GLOBAL_CONFIG["adapters_manager"]
         ATTRS_MAP = ConfigStore.get_attributes_map(GLOBAL_CONFIG["attrs_cfg_path"])
 
         self._ADAPTERS_MANAGER = AdaptersManager(ADAPTERS_MANAGER_CFG, ATTRS_MAP)
-        self._SUBJECT_ATTRIBUTE = cfg.get("perun_person_principal_names_attribute")
-        self._PREFERRED_MAIL_ATTRIBUTE = cfg["mfa_reset"]["preferred_mail_attribute"]
-        self._ALL_MAILS_ATTRIBUTE = cfg.get("mfa_reset", {}).get("all_mails_attribute")
-        self._NAME_ATTRIBUTE = cfg.get("perun_user_name_attribute")
-        self.email_service = EmailService(cfg)
+        self._SUBJECT_ATTRIBUTE = USER_MANAGER_CFG.get(
+            "perun_person_principal_names_attribute"
+        )
+        self._KEY_ID = USER_MANAGER_CFG["key_id"]
+        self._KEYSTORE = USER_MANAGER_CFG["keystore"]
+
+        if isinstance(cfg.get("heuristic_page", None), dict):
+            self._NAME_ATTRIBUTE = USER_MANAGER_CFG.get("heuristic_page", {}).get(
+                "perun_user_name_attribute"
+            )
+
+        if isinstance(cfg.get("mfa_reset", None), dict):
+            self.email_service = EmailService(cfg)
+            self._PREFERRED_MAIL_ATTRIBUTE = cfg.get("mfa_reset", {}).get(
+                "preferred_mail_attribute"
+            )
+            self._ALL_MAILS_ATTRIBUTE = cfg.get("mfa_reset", {}).get(
+                "all_mails_attribute"
+            )
+
         self.database_service = DatabaseService(cfg)
         self.jwt_service = SingletonJWTServiceProvider.get_provider().get_service()
-        self._KEY_ID = cfg["key_id"]
-        self._KEYSTORE = cfg["keystore"]
 
         self.logger = Logger.get_logger(__name__)
-        self._cfg = cfg
+        self._cfg = USER_MANAGER_CFG
 
     def extract_user_attribute(self, attr_name: str, user_id: int) -> Any:
         user_attrs = self._ADAPTERS_MANAGER.get_user_attributes(user_id, [attr_name])
         attr_value_candidates = user_attrs.get(attr_name, [])
         attr_value = attr_value_candidates[0] if attr_value_candidates else None
 
         return attr_value
```

### Comparing `perun.proxygui-4.1.1/perun/utils/ConfigStore.py` & `perun.proxygui-5.0.0/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/CustomRPHandler.py` & `perun.proxygui-5.0.0/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/DatabaseService.py` & `perun.proxygui-5.0.0/perun/utils/DatabaseService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/EmailService.py` & `perun.proxygui-5.0.0/perun/utils/EmailService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/Utils.py` & `perun.proxygui-5.0.0/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/consent_framework/consent.py` & `perun.proxygui-5.0.0/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-5.0.0/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-5.0.0/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-5.0.0/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-5.0.0/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/logout_requests/BackchannelLogoutRequest.py` & `perun.proxygui-5.0.0/perun/utils/logout_requests/BackchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py` & `perun.proxygui-5.0.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/logout_requests/GraphLogoutRequest.py` & `perun.proxygui-5.0.0/perun/utils/logout_requests/GraphLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/logout_requests/LogoutRequest.py` & `perun.proxygui-5.0.0/perun/utils/logout_requests/LogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun/utils/logout_requests/SamlLogoutRequest.py` & `perun.proxygui-5.0.0/perun/utils/logout_requests/SamlLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun.proxygui.egg-info/PKG-INFO` & `perun.proxygui-5.0.0/perun.proxygui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 4.1.1
+Version: 5.0.0
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
```

### Comparing `perun.proxygui-4.1.1/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-5.0.0/perun.proxygui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/perun.proxygui.egg-info/requires.txt` & `perun.proxygui-5.0.0/perun.proxygui.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `perun.proxygui-4.1.1/setup.py` & `perun.proxygui-5.0.0/setup.py`

 * *Files identical despite different names*

