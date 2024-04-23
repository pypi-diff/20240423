# Comparing `tmp/buildz-0.4.91.tar.gz` & `tmp/buildz-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "buildz-0.4.91.tar", last modified: Tue Apr 16 14:14:44 2024, max compression
+gzip compressed data, was "buildz-0.5.1.tar", last modified: Tue Apr 23 20:20:42 2024, max compression
```

## Comparing `buildz-0.4.91.tar` & `buildz-0.5.1.tar`

### file list

```diff
@@ -1,154 +1,159 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.463063 buildz-0.4.91/
--rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.4.91/LICENSE
--rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.4.91/MANIFEST.in
--rw-rw-rw-   0        0        0     2706 2024-04-16 14:14:44.463063 buildz-0.4.91/PKG-INFO
--rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.4.91/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.897421 buildz-0.4.91/buildz/
--rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.4.91/buildz/__init__.py
--rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.4.91/buildz/__main__.py
--rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.4.91/buildz/argx.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.927921 buildz-0.4.91/buildz/demo/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.937433 buildz-0.4.91/buildz/demo/ioc/
--rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.4.91/buildz/demo/ioc/deal.py
--rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.4.91/buildz/demo/ioc/help.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.945025 buildz-0.4.91/buildz/demo/myers/
--rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.4.91/buildz/demo/myers/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.91/buildz/demo/myers/help.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.960673 buildz-0.4.91/buildz/demo/res/
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.976337 buildz-0.4.91/buildz/demo/res/conf/
--rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.4.91/buildz/demo/res/conf/ioc.js
--rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.4.91/buildz/demo/res/conf/main.js
--rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.4.91/buildz/demo/res/conf/myers.js
--rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.4.91/buildz/demo/res/conf/search.js
--rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.4.91/buildz/demo/res/conf/xf.js
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.006075 buildz-0.4.91/buildz/demo/res/help/
--rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.4.91/buildz/demo/res/help/default.js
--rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.4.91/buildz/demo/res/help/ioc.js
--rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.4.91/buildz/demo/res/help/myers.js
--rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.4.91/buildz/demo/res/help/search.js
--rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.4.91/buildz/demo/res/help/xf.js
--rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.4.91/buildz/demo/res/test.js
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.008084 buildz-0.4.91/buildz/demo/search/
--rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.4.91/buildz/demo/search/deal.py
--rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.4.91/buildz/demo/search/help.py
--rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.4.91/buildz/demo/test.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.008084 buildz-0.4.91/buildz/demo/xf/
--rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.4.91/buildz/demo/xf/deal.py
--rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.4.91/buildz/demo/xf/help.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.024110 buildz-0.4.91/buildz/fz/
--rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.4.91/buildz/fz/__init__.py
--rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.4.91/buildz/fz/dirz.py
--rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.4.91/buildz/fz/fio.py
--rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.4.91/buildz/fz/lsf.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.039740 buildz-0.4.91/buildz/ioc/
--rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.4.91/buildz/ioc/__init__.py
--rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.4.91/buildz/ioc/init.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.055524 buildz-0.4.91/buildz/ioc/ioc/
--rw-rw-rw-   0        0        0     1010 2024-04-02 12:26:00.000000 buildz-0.4.91/buildz/ioc/ioc/base.py
--rw-rw-rw-   0        0        0     5842 2024-04-02 16:11:02.000000 buildz-0.4.91/buildz/ioc/ioc/conf.py
--rw-rw-rw-   0        0        0    12673 2024-04-16 13:23:38.000000 buildz-0.4.91/buildz/ioc/ioc/confs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.134876 buildz-0.4.91/buildz/ioc/ioc_deal/
--rw-rw-rw-   0        0        0     4828 2024-04-02 14:18:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/base.py
--rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.4.91/buildz/ioc/ioc_deal/call.py
--rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.4.91/buildz/ioc/ioc_deal/calls.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.214026 buildz-0.4.91/buildz/ioc/ioc_deal/conf/
--rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/call_defaults.js
--rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/call_lists.js
--rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/calls_defaults.js
--rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/calls_lists.js
--rw-rw-rw-   0        0        0     1843 2024-04-02 15:59:22.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/deals.js
--rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/env_lists.js
--rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ioc_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/join_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/list_lists.js
--rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/map_lists.js
--rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/mcall_defaults.js
--rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/mcall_lists.js
--rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
--rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_defaults.js
--rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_lists.js
--rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_set_lists.js
--rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ovar_lists.js
--rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/ref_lists.js
--rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.4.91/buildz/ioc/ioc_deal/conf/var_lists.js
--rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.4.91/buildz/ioc/ioc_deal/demo.py
--rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.4.91/buildz/ioc/ioc_deal/env.py
--rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ioc.py
--rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.4.91/buildz/ioc/ioc_deal/join.py
--rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.4.91/buildz/ioc/ioc_deal/list.py
--rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.4.91/buildz/ioc/ioc_deal/map.py
--rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.4.91/buildz/ioc/ioc_deal/mcall.py
--rw-rw-rw-   0        0        0     5472 2024-04-02 15:07:54.000000 buildz-0.4.91/buildz/ioc/ioc_deal/obj.py
--rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ovar.py
--rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.4.91/buildz/ioc/ioc_deal/ref.py
--rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.4.91/buildz/ioc/ioc_deal/val.py
--rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.4.91/buildz/ioc/ioc_deal/var.py
--rw-rw-rw-   0        0        0     1931 2024-04-07 18:52:48.000000 buildz-0.4.91/buildz/pyz.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.221451 buildz-0.4.91/buildz/tz/
--rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.4.91/buildz/tz/__init__.py
--rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.4.91/buildz/tz/myers_diff.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.247866 buildz-0.4.91/buildz/xf/
--rw-rw-rw-   0        0        0      210 2024-04-16 13:29:45.000000 buildz-0.4.91/buildz/xf/__init__.py
--rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.4.91/buildz/xf/__main__.py
--rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.4.91/buildz/xf/file.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.280399 buildz-0.4.91/buildz/xf/loader/
--rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.4.91/buildz/xf/loader/base.py
--rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.4.91/buildz/xf/loader/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.318389 buildz-0.4.91/buildz/xf/loader/deal/
--rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.4.91/buildz/xf/loader/deal/listz.py
--rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.4.91/buildz/xf/loader/deal/lr.py
--rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.4.91/buildz/xf/loader/deal/lrval.py
--rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.4.91/buildz/xf/loader/deal/mapz.py
--rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.4.91/buildz/xf/loader/deal/nextz.py
--rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.4.91/buildz/xf/loader/deal/reval.py
--rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.4.91/buildz/xf/loader/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.4.91/buildz/xf/loader/deal/spc.py
--rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.4.91/buildz/xf/loader/deal/spt.py
--rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.4.91/buildz/xf/loader/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.91/buildz/xf/loader/exp.py
--rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.4.91/buildz/xf/loader/item.py
--rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.4.91/buildz/xf/loader/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.4.91/buildz/xf/loader/pos.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.357098 buildz-0.4.91/buildz/xf/loaderz/
--rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.4.91/buildz/xf/loaderz/base.py
--rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.4.91/buildz/xf/loaderz/buffer.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.404072 buildz-0.4.91/buildz/xf/loaderz/deal/
--rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.4.91/buildz/xf/loaderz/deal/listz.py
--rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.4.91/buildz/xf/loaderz/deal/lr.py
--rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.4.91/buildz/xf/loaderz/deal/lrval.py
--rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.4.91/buildz/xf/loaderz/deal/mapz.py
--rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.4.91/buildz/xf/loaderz/deal/nextz.py
--rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.4.91/buildz/xf/loaderz/deal/reval.py
--rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.4.91/buildz/xf/loaderz/deal/setz.py
--rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.4.91/buildz/xf/loaderz/deal/spc.py
--rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.4.91/buildz/xf/loaderz/deal/spt.py
--rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.4.91/buildz/xf/loaderz/deal/strz.py
--rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.4.91/buildz/xf/loaderz/exp.py
--rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.4.91/buildz/xf/loaderz/item.py
--rw-rw-rw-   0        0        0     2838 2024-04-16 10:04:19.000000 buildz-0.4.91/buildz/xf/loaderz/mg.py
--rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.4.91/buildz/xf/loaderz/pos.py
--rw-rw-rw-   0        0        0     1687 2024-04-16 14:12:03.000000 buildz-0.4.91/buildz/xf/loaderz/test.py
--rw-rw-rw-   0        0        0     2009 2024-04-10 16:50:01.000000 buildz-0.4.91/buildz/xf/mapz.py
--rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.4.91/buildz/xf/read.py
--rw-rw-rw-   0        0        0     2525 2024-04-16 13:29:30.000000 buildz-0.4.91/buildz/xf/readz.py
--rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.4.91/buildz/xf/stack.py
--rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.4.91/buildz/xf/write.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.430238 buildz-0.4.91/buildz/xf/writer/
--rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.4.91/buildz/xf/writer/base.py
--rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.4.91/buildz/xf/writer/conf.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:44.461697 buildz-0.4.91/buildz/xf/writer/deal/
--rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.4.91/buildz/xf/writer/deal/jsonval.py
--rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.4.91/buildz/xf/writer/deal/listz.py
--rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.4.91/buildz/xf/writer/deal/mapz.py
--rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.4.91/buildz/xf/writer/deal/reval.py
--rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.4.91/buildz/xf/writer/deal/strz.py
--rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.4.91/buildz/xf/writer/itemz.py
--rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.4.91/buildz/xf/writer/mg.py
--rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.4.91/buildz/xf/xargs.py
-drwxrwxrwx   0        0        0        0 2024-04-16 14:14:43.922962 buildz-0.4.91/buildz.egg-info/
--rw-rw-rw-   0        0        0     2706 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3526 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-16 14:14:43.000000 buildz-0.4.91/buildz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 14:14:44.463063 buildz-0.4.91/setup.cfg
--rw-rw-rw-   0        0        0      771 2024-04-16 13:30:05.000000 buildz-0.4.91/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.875188 buildz-0.5.1/
+-rw-rw-rw-   0        0        0    11558 2023-10-16 14:40:02.000000 buildz-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0       45 2024-02-27 01:25:41.000000 buildz-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2705 2024-04-23 20:20:42.875188 buildz-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2290 2024-04-16 14:12:21.000000 buildz-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.417045 buildz-0.5.1/buildz/
+-rw-rw-rw-   0        0        0      153 2024-04-16 14:04:54.000000 buildz-0.5.1/buildz/__init__.py
+-rw-rw-rw-   0        0        0       90 2024-04-01 15:59:48.000000 buildz-0.5.1/buildz/__main__.py
+-rw-rw-rw-   0        0        0     2944 2024-04-13 11:54:47.000000 buildz-0.5.1/buildz/argx.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.432049 buildz-0.5.1/buildz/demo/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.463809 buildz-0.5.1/buildz/demo/ioc/
+-rw-rw-rw-   0        0        0      548 2024-04-02 17:19:41.000000 buildz-0.5.1/buildz/demo/ioc/deal.py
+-rw-rw-rw-   0        0        0     1401 2024-04-02 17:34:58.000000 buildz-0.5.1/buildz/demo/ioc/help.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.471001 buildz-0.5.1/buildz/demo/myers/
+-rw-rw-rw-   0        0        0     2060 2024-04-07 18:54:16.000000 buildz-0.5.1/buildz/demo/myers/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.1/buildz/demo/myers/help.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.479509 buildz-0.5.1/buildz/demo/res/
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.486432 buildz-0.5.1/buildz/demo/res/conf/
+-rw-rw-rw-   0        0        0      432 2024-04-01 16:28:22.000000 buildz-0.5.1/buildz/demo/res/conf/ioc.js
+-rw-rw-rw-   0        0        0     1930 2024-04-07 16:29:22.000000 buildz-0.5.1/buildz/demo/res/conf/main.js
+-rw-rw-rw-   0        0        0      461 2024-04-07 16:06:55.000000 buildz-0.5.1/buildz/demo/res/conf/myers.js
+-rw-rw-rw-   0        0        0      466 2024-04-02 16:29:25.000000 buildz-0.5.1/buildz/demo/res/conf/search.js
+-rw-rw-rw-   0        0        0      446 2024-04-01 16:28:28.000000 buildz-0.5.1/buildz/demo/res/conf/xf.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.486432 buildz-0.5.1/buildz/demo/res/help/
+-rw-rw-rw-   0        0        0      419 2024-04-07 16:31:32.000000 buildz-0.5.1/buildz/demo/res/help/default.js
+-rw-rw-rw-   0        0        0     1117 2024-04-02 17:27:33.000000 buildz-0.5.1/buildz/demo/res/help/ioc.js
+-rw-rw-rw-   0        0        0     1234 2024-04-07 18:48:53.000000 buildz-0.5.1/buildz/demo/res/help/myers.js
+-rw-rw-rw-   0        0        0      871 2024-04-02 17:27:41.000000 buildz-0.5.1/buildz/demo/res/help/search.js
+-rw-rw-rw-   0        0        0     1547 2024-04-02 17:12:29.000000 buildz-0.5.1/buildz/demo/res/help/xf.js
+-rw-rw-rw-   0        0        0      572 2024-04-16 13:25:08.000000 buildz-0.5.1/buildz/demo/res/test.js
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.495437 buildz-0.5.1/buildz/demo/search/
+-rw-rw-rw-   0        0        0      907 2024-04-02 17:19:49.000000 buildz-0.5.1/buildz/demo/search/deal.py
+-rw-rw-rw-   0        0        0      491 2024-04-02 17:19:57.000000 buildz-0.5.1/buildz/demo/search/help.py
+-rw-rw-rw-   0        0        0     1664 2024-04-02 17:36:05.000000 buildz-0.5.1/buildz/demo/test.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.495437 buildz-0.5.1/buildz/demo/xf/
+-rw-rw-rw-   0        0        0      368 2024-04-02 17:20:04.000000 buildz-0.5.1/buildz/demo/xf/deal.py
+-rw-rw-rw-   0        0        0      502 2024-04-02 17:20:15.000000 buildz-0.5.1/buildz/demo/xf/help.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/fz/
+-rw-rw-rw-   0        0        0      233 2024-04-05 04:01:25.000000 buildz-0.5.1/buildz/fz/__init__.py
+-rw-rw-rw-   0        0        0     1387 2024-04-01 14:39:23.000000 buildz-0.5.1/buildz/fz/dirz.py
+-rw-rw-rw-   0        0        0      629 2024-04-05 10:37:31.000000 buildz-0.5.1/buildz/fz/fio.py
+-rw-rw-rw-   0        0        0     1729 2024-04-02 16:31:56.000000 buildz-0.5.1/buildz/fz/lsf.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/ioc/
+-rw-rw-rw-   0        0        0      124 2024-04-02 15:52:39.000000 buildz-0.5.1/buildz/ioc/__init__.py
+-rw-rw-rw-   0        0        0      297 2024-03-31 08:12:36.000000 buildz-0.5.1/buildz/ioc/init.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.542601 buildz-0.5.1/buildz/ioc/ioc/
+-rw-rw-rw-   0        0        0     2230 2024-04-23 14:05:55.000000 buildz-0.5.1/buildz/ioc/ioc/base.py
+-rw-rw-rw-   0        0        0     6624 2024-04-23 19:13:22.000000 buildz-0.5.1/buildz/ioc/ioc/conf.py
+-rw-rw-rw-   0        0        0    13056 2024-04-23 19:19:25.000000 buildz-0.5.1/buildz/ioc/ioc/confs.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.558233 buildz-0.5.1/buildz/ioc/ioc_deal/
+-rw-rw-rw-   0        0        0     4828 2024-04-23 18:50:39.000000 buildz-0.5.1/buildz/ioc/ioc_deal/base.py
+-rw-rw-rw-   0        0        0     1461 2024-04-02 15:35:04.000000 buildz-0.5.1/buildz/ioc/ioc_deal/call.py
+-rw-rw-rw-   0        0        0     1239 2024-04-02 15:36:13.000000 buildz-0.5.1/buildz/ioc/ioc_deal/calls.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.570451 buildz-0.5.1/buildz/ioc/ioc_deal/conf/
+-rw-rw-rw-   0        0        0       50 2024-03-31 09:25:52.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/call_defaults.js
+-rw-rw-rw-   0        0        0      416 2024-03-31 09:53:23.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/call_lists.js
+-rw-rw-rw-   0        0        0       19 2024-04-01 14:21:19.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/calls_defaults.js
+-rw-rw-rw-   0        0        0      376 2024-04-01 14:21:18.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/calls_lists.js
+-rw-rw-rw-   0        0        0      412 2024-04-23 19:15:09.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/deal_lists.js
+-rw-rw-rw-   0        0        0     2197 2024-04-23 19:17:12.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/deals.js
+-rw-rw-rw-   0        0        0      307 2024-04-01 14:20:24.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/env_lists.js
+-rw-rw-rw-   0        0        0      444 2024-04-01 11:09:33.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ioc_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/join_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/list_lists.js
+-rw-rw-rw-   0        0        0      286 2024-04-01 14:26:46.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/map_lists.js
+-rw-rw-rw-   0        0        0       66 2024-04-02 15:18:35.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/mcall_defaults.js
+-rw-rw-rw-   0        0        0      509 2024-04-02 15:19:12.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/mcall_lists.js
+-rw-rw-rw-   0        0        0      159 2024-03-31 08:48:51.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_cst_lists.js
+-rw-rw-rw-   0        0        0      173 2024-04-02 14:50:55.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_defaults.js
+-rw-rw-rw-   0        0        0      627 2024-04-02 14:51:11.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_lists.js
+-rw-rw-rw-   0        0        0      113 2024-03-31 08:45:47.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_set_lists.js
+-rw-rw-rw-   0        0        0      443 2024-04-02 15:23:34.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ovar_lists.js
+-rw-rw-rw-   0        0        0      488 2024-04-02 15:09:57.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/ref_lists.js
+-rw-rw-rw-   0        0        0      351 2024-03-31 10:05:46.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/var_lists.js
+-rw-rw-rw-   0        0        0        4 2024-04-23 10:50:44.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/xfile_defaults.js
+-rw-rw-rw-   0        0        0      410 2024-04-23 10:50:04.000000 buildz-0.5.1/buildz/ioc/ioc_deal/conf/xfile_lists.js
+-rw-rw-rw-   0        0        0     1356 2024-04-23 19:35:52.000000 buildz-0.5.1/buildz/ioc/ioc_deal/deal.py
+-rw-rw-rw-   0        0        0      365 2024-03-31 09:08:35.000000 buildz-0.5.1/buildz/ioc/ioc_deal/demo.py
+-rw-rw-rw-   0        0        0      824 2024-04-02 15:07:38.000000 buildz-0.5.1/buildz/ioc/ioc_deal/env.py
+-rw-rw-rw-   0        0        0      950 2024-04-02 15:27:47.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ioc.py
+-rw-rw-rw-   0        0        0      928 2024-04-02 15:33:45.000000 buildz-0.5.1/buildz/ioc/ioc_deal/join.py
+-rw-rw-rw-   0        0        0     1086 2024-04-02 17:38:51.000000 buildz-0.5.1/buildz/ioc/ioc_deal/list.py
+-rw-rw-rw-   0        0        0     1017 2024-04-02 15:31:18.000000 buildz-0.5.1/buildz/ioc/ioc_deal/map.py
+-rw-rw-rw-   0        0        0     1972 2024-04-02 15:18:24.000000 buildz-0.5.1/buildz/ioc/ioc_deal/mcall.py
+-rw-rw-rw-   0        0        0     6130 2024-04-23 14:07:16.000000 buildz-0.5.1/buildz/ioc/ioc_deal/obj.py
+-rw-rw-rw-   0        0        0     1558 2024-04-02 15:23:58.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ovar.py
+-rw-rw-rw-   0        0        0     1083 2024-04-02 15:10:34.000000 buildz-0.5.1/buildz/ioc/ioc_deal/ref.py
+-rw-rw-rw-   0        0        0      702 2024-04-02 15:08:11.000000 buildz-0.5.1/buildz/ioc/ioc_deal/val.py
+-rw-rw-rw-   0        0        0     1000 2024-04-02 15:26:02.000000 buildz-0.5.1/buildz/ioc/ioc_deal/var.py
+-rw-rw-rw-   0        0        0     1078 2024-04-23 10:55:49.000000 buildz-0.5.1/buildz/ioc/ioc_deal/xfile.py
+-rw-rw-rw-   0        0        0     1958 2024-04-23 08:58:52.000000 buildz-0.5.1/buildz/pyz.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.589591 buildz-0.5.1/buildz/tz/
+-rw-rw-rw-   0        0        0      324 2024-04-16 14:03:17.000000 buildz-0.5.1/buildz/tz/__init__.py
+-rw-rw-rw-   0        0        0     7543 2024-04-07 19:00:58.000000 buildz-0.5.1/buildz/tz/myers_diff.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.643635 buildz-0.5.1/buildz/xf/
+-rw-rw-rw-   0        0        0      210 2024-04-16 13:29:45.000000 buildz-0.5.1/buildz/xf/__init__.py
+-rw-rw-rw-   0        0        0       86 2024-04-13 11:53:05.000000 buildz-0.5.1/buildz/xf/__main__.py
+-rw-rw-rw-   0        0        0      841 2024-04-01 17:49:56.000000 buildz-0.5.1/buildz/xf/file.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.668493 buildz-0.5.1/buildz/xf/loader/
+-rw-rw-rw-   0        0        0     1782 2024-04-14 12:14:09.000000 buildz-0.5.1/buildz/xf/loader/base.py
+-rw-rw-rw-   0        0        0     3647 2024-04-14 14:34:15.000000 buildz-0.5.1/buildz/xf/loader/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.719803 buildz-0.5.1/buildz/xf/loader/deal/
+-rw-rw-rw-   0        0        0      613 2024-02-22 13:04:58.000000 buildz-0.5.1/buildz/xf/loader/deal/listz.py
+-rw-rw-rw-   0        0        0     2647 2024-04-14 14:34:45.000000 buildz-0.5.1/buildz/xf/loader/deal/lr.py
+-rw-rw-rw-   0        0        0     1583 2024-03-01 16:44:58.000000 buildz-0.5.1/buildz/xf/loader/deal/lrval.py
+-rw-rw-rw-   0        0        0      734 2024-02-22 13:18:57.000000 buildz-0.5.1/buildz/xf/loader/deal/mapz.py
+-rw-rw-rw-   0        0        0      517 2024-02-22 16:24:13.000000 buildz-0.5.1/buildz/xf/loader/deal/nextz.py
+-rw-rw-rw-   0        0        0     1242 2024-04-14 12:03:17.000000 buildz-0.5.1/buildz/xf/loader/deal/reval.py
+-rw-rw-rw-   0        0        0     1134 2024-04-14 12:09:59.000000 buildz-0.5.1/buildz/xf/loader/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.1/buildz/xf/loader/deal/spc.py
+-rw-rw-rw-   0        0        0     1358 2024-02-28 03:19:27.000000 buildz-0.5.1/buildz/xf/loader/deal/spt.py
+-rw-rw-rw-   0        0        0     3180 2024-04-14 14:16:55.000000 buildz-0.5.1/buildz/xf/loader/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.1/buildz/xf/loader/exp.py
+-rw-rw-rw-   0        0        0     1490 2024-04-12 12:01:04.000000 buildz-0.5.1/buildz/xf/loader/item.py
+-rw-rw-rw-   0        0        0     2502 2024-04-16 13:18:40.000000 buildz-0.5.1/buildz/xf/loader/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.1/buildz/xf/loader/pos.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.747437 buildz-0.5.1/buildz/xf/loaderz/
+-rw-rw-rw-   0        0        0      746 2024-04-16 13:01:38.000000 buildz-0.5.1/buildz/xf/loaderz/base.py
+-rw-rw-rw-   0        0        0     3126 2024-04-16 13:11:00.000000 buildz-0.5.1/buildz/xf/loaderz/buffer.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.811401 buildz-0.5.1/buildz/xf/loaderz/deal/
+-rw-rw-rw-   0        0        0      533 2024-04-16 10:23:04.000000 buildz-0.5.1/buildz/xf/loaderz/deal/listz.py
+-rw-rw-rw-   0        0        0     1787 2024-04-16 12:27:38.000000 buildz-0.5.1/buildz/xf/loaderz/deal/lr.py
+-rw-rw-rw-   0        0        0     1094 2024-04-16 13:26:19.000000 buildz-0.5.1/buildz/xf/loaderz/deal/lrval.py
+-rw-rw-rw-   0        0        0      699 2024-04-16 10:17:43.000000 buildz-0.5.1/buildz/xf/loaderz/deal/mapz.py
+-rw-rw-rw-   0        0        0      452 2024-04-16 12:57:03.000000 buildz-0.5.1/buildz/xf/loaderz/deal/nextz.py
+-rw-rw-rw-   0        0        0      691 2024-04-16 13:02:05.000000 buildz-0.5.1/buildz/xf/loaderz/deal/reval.py
+-rw-rw-rw-   0        0        0      287 2024-04-16 10:07:28.000000 buildz-0.5.1/buildz/xf/loaderz/deal/setz.py
+-rw-rw-rw-   0        0        0      504 2024-04-14 14:10:33.000000 buildz-0.5.1/buildz/xf/loaderz/deal/spc.py
+-rw-rw-rw-   0        0        0     1147 2024-04-16 12:27:46.000000 buildz-0.5.1/buildz/xf/loaderz/deal/spt.py
+-rw-rw-rw-   0        0        0     3234 2024-04-16 13:34:36.000000 buildz-0.5.1/buildz/xf/loaderz/deal/strz.py
+-rw-rw-rw-   0        0        0      448 2024-02-21 13:35:31.000000 buildz-0.5.1/buildz/xf/loaderz/exp.py
+-rw-rw-rw-   0        0        0     1911 2024-04-16 10:34:17.000000 buildz-0.5.1/buildz/xf/loaderz/item.py
+-rw-rw-rw-   0        0        0     2838 2024-04-16 10:04:19.000000 buildz-0.5.1/buildz/xf/loaderz/mg.py
+-rw-rw-rw-   0        0        0     1339 2024-04-14 12:11:55.000000 buildz-0.5.1/buildz/xf/loaderz/pos.py
+-rw-rw-rw-   0        0        0     1687 2024-04-16 14:12:03.000000 buildz-0.5.1/buildz/xf/loaderz/test.py
+-rw-rw-rw-   0        0        0     2009 2024-04-23 09:07:57.000000 buildz-0.5.1/buildz/xf/mapz.py
+-rw-rw-rw-   0        0        0     2587 2024-04-16 13:17:27.000000 buildz-0.5.1/buildz/xf/read.py
+-rw-rw-rw-   0        0        0     2587 2024-04-22 07:14:54.000000 buildz-0.5.1/buildz/xf/readz.py
+-rw-rw-rw-   0        0        0     1999 2024-04-15 04:06:48.000000 buildz-0.5.1/buildz/xf/stack.py
+-rw-rw-rw-   0        0        0     1230 2024-04-07 17:26:44.000000 buildz-0.5.1/buildz/xf/write.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.844079 buildz-0.5.1/buildz/xf/writer/
+-rw-rw-rw-   0        0        0     1108 2024-02-23 14:38:49.000000 buildz-0.5.1/buildz/xf/writer/base.py
+-rw-rw-rw-   0        0        0     1519 2024-02-23 14:41:57.000000 buildz-0.5.1/buildz/xf/writer/conf.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.875188 buildz-0.5.1/buildz/xf/writer/deal/
+-rw-rw-rw-   0        0        0      461 2024-02-24 09:45:45.000000 buildz-0.5.1/buildz/xf/writer/deal/jsonval.py
+-rw-rw-rw-   0        0        0     1105 2024-02-24 09:40:04.000000 buildz-0.5.1/buildz/xf/writer/deal/listz.py
+-rw-rw-rw-   0        0        0     1252 2024-02-24 09:40:12.000000 buildz-0.5.1/buildz/xf/writer/deal/mapz.py
+-rw-rw-rw-   0        0        0      504 2024-02-24 09:41:59.000000 buildz-0.5.1/buildz/xf/writer/deal/reval.py
+-rw-rw-rw-   0        0        0     1429 2024-04-07 12:04:50.000000 buildz-0.5.1/buildz/xf/writer/deal/strz.py
+-rw-rw-rw-   0        0        0     1152 2024-02-23 09:09:41.000000 buildz-0.5.1/buildz/xf/writer/itemz.py
+-rw-rw-rw-   0        0        0     2038 2024-02-24 09:36:48.000000 buildz-0.5.1/buildz/xf/writer/mg.py
+-rw-rw-rw-   0        0        0      597 2024-04-13 11:53:25.000000 buildz-0.5.1/buildz/xf/xargs.py
+drwxrwxrwx   0        0        0        0 2024-04-23 20:20:42.432049 buildz-0.5.1/buildz.egg-info/
+-rw-rw-rw-   0        0        0     2705 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3705 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-23 20:20:42.000000 buildz-0.5.1/buildz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-23 20:20:42.875188 buildz-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      770 2024-04-23 20:17:27.000000 buildz-0.5.1/setup.py
```

### Comparing `buildz-0.4.91/LICENSE` & `buildz-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/PKG-INFO` & `buildz-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.91
+Version: 0.5.1
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.91/README.md` & `buildz-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/argx.py` & `buildz-0.5.1/buildz/argx.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/ioc/deal.py` & `buildz-0.5.1/buildz/demo/ioc/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/ioc/help.py` & `buildz-0.5.1/buildz/demo/ioc/help.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/myers/deal.py` & `buildz-0.5.1/buildz/demo/myers/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/conf/main.js` & `buildz-0.5.1/buildz/demo/res/conf/main.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/help/ioc.js` & `buildz-0.5.1/buildz/demo/res/help/ioc.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/help/myers.js` & `buildz-0.5.1/buildz/demo/res/help/myers.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/help/search.js` & `buildz-0.5.1/buildz/demo/res/help/search.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/help/xf.js` & `buildz-0.5.1/buildz/demo/res/help/xf.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/res/test.js` & `buildz-0.5.1/buildz/demo/res/test.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/search/deal.py` & `buildz-0.5.1/buildz/demo/search/deal.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/demo/test.py` & `buildz-0.5.1/buildz/demo/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/fz/dirz.py` & `buildz-0.5.1/buildz/fz/dirz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/fz/fio.py` & `buildz-0.5.1/buildz/fz/fio.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/fz/lsf.py` & `buildz-0.5.1/buildz/fz/lsf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc/conf.py` & `buildz-0.5.1/buildz/ioc/ioc/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #coding=utf-8
 from buildz import xf, pyz
 from buildz.xf import g as xg
 import json
-from .base import Base, EncapeData
+from .base import Base, EncapeData,IOCError
 class Conf(Base):
     """
         配置文件格式：
             {
                 id: 配置文件id，默认null
                 //在配置文件配置的环境变量
                 envs: {
@@ -29,14 +29,20 @@
                     ...
                 ]
                 //全局数据配置项
                 datas: [
                     item_conf,
                     ...
                 ]
+                // 初始化，会一个一个get(id)
+                // 其他地方调用该conf.get的时候，会先判断有没有进行init，没有就先调init里的get
+                inits: [
+                    id,
+                    ...
+                ]
             }
         如果只有全局数据配置项，可以只写datas里的东西:
             [
                 //全局数据配置项
                 item_conf,
                 ...
             ]
@@ -59,25 +65,26 @@
                 namespace: default null
                 datas: [{id:val, type: val, ...}]
                 locals: [like datas]
                 default_type: default null
             }
         """
         if type(conf)!=dict:
-            conf = {'data':conf}
+            conf = {'datas':conf}
         id = xf.g(conf, id=None)
         if id is None:
             id = confs.conf_id()
         self.id = id
         self.namespace = xf.g(conf, namespace=None)
         self.conf = conf
         self.confs = confs
         self.locals = self.map(xf.g(conf, locals=[]), self.confs.get_data_id)
         self.datas = self.map(xf.g(conf, datas=[]), self.confs.get_data_id)
         self.deals = self.map(xf.g(conf, deals = []), self.confs.get_deal_type)
+        self.inits = xf.g(conf, inits = [])
         self._default_type = xf.g(conf, default_type = None)
         self.envs = xf.g(conf, envs = {})
         self.confs.flush_env(self.envs)
         for _type in list(self.deals.keys()):
             conf = self.deals[_type]
             if type(conf) in [list, tuple]:
                 maps = {}
@@ -93,14 +100,21 @@
             args = xf.g(conf, args=[])
             maps = xf.g(conf, maps={})
             deal = fc(*args, **maps)
             self.deals[_type] = deal
             aliases = xf.g(conf, aliases = [])
             for alias in aliases:
                 self.deals[alias] = deal
+        self.mark_init = False
+    def do_init(self):
+        if self.mark_init:
+            return
+        self.mark_init = True
+        for id in self.inits:
+            self.get(id)
     def get_env(self, id, search_confs = True):
         if self.confs.global_env and search_confs:
             return self.confs.get_env(id, self.id)
         ids = self.confs.env_ids(id)
         envs = self.envs
         find = None
         for id in ids:
@@ -112,23 +126,27 @@
                 break
             envs = envs[id]
         if envs is not None:
             return envs
         if not search_confs:
             return None
         return self.confs.get_env(id, self.id)
+    def set_deal(self, type, fc):
+        self.deals[type] = fc
+        self.confs.set_deal(type, fc)
     def get_deal(self, type, search_confs = True):
         if self.confs.global_deal and search_confs:
             return self.confs.get_deal(type, self.id)
         if type in self.deals:
             return self.deals[type]
         if not search_confs:
             return None
         return self.confs.get_deal(type, self.id)
     def get_data(self, id, local = True, search_confs = True, src = None, info = None):
+        self.do_init()
         if id in self.datas:
             obj = self.datas[id]
             return EncapeData(obj, self, local = False, src=src, info = info)
         if not local:
             return None
         if id in self.locals:
             obj = self.locals[id]
@@ -144,17 +162,19 @@
         return self._default_type
     def get_obj(self, id, src = None, info=None, remove = False):
         """
             根据data id获取data对象，处理逻辑：根据data id查配置，根据配置的type查deal，返回deal处理过的配置
         """
         conf = self.get_data(id, src = src, info = info)
         if conf is None:
+            raise IOCError(f"can't find conf of {id}")
             return None
         deal = self.get_deal(conf.type)
         if deal is None:
+            raise IOCError(f"can't find deal of {id}, type = {conf.type}")
             return None
         if not remove:
             obj = deal(conf)
         else:
             obj = deal.remove(conf)
         return obj
     def remove(self, id):
```

### Comparing `buildz-0.4.91/buildz/ioc/ioc/confs.py` & `buildz-0.5.1/buildz/ioc/ioc/confs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #coding=utf-8
 from buildz import xf, pyz
 from buildz.xf import g as xg
 from buildz import argx
 import json
-from .base import Base, EncapeData
+from .base import Base, EncapeData,IOCError
 from .conf import Conf
 import os
 class ConfsNode(Base):
     def init(self):
         self.confs = []
         self.ids = {}
 
@@ -216,14 +216,21 @@
         self._conf_id = 0
         self.conf = conf
         self.node = ConfsNode()
         self.confs = {}
         self.deals = {}
         self.envs = {}
         self.envs_args = None
+        self.mark_init = False
+    def do_init(self):
+        if self.mark_init:
+            return
+        self.mark_init = True
+        for id in self.confs:
+            self.confs[id].do_init()
     def get_deal_type(self, obj):
         if type(obj)==dict:
             return obj[self.deal_key_type]
         return obj[self.deal_index_type]
     def get_data_id(self, obj):
         if type(obj)==dict:
             return obj[self.data_key_id]
@@ -302,19 +309,22 @@
         return self.get_obj(*args, **maps)
     def remove(self, *a,**b):
         return self.get_obj(*a, **b, remove=True)
     def get_obj(self, id, sid = None, src = None, info = None, remove = False):
         """
             根据data id获取data对象，处理逻辑：根据data id查配置，根据配置的type查deal，返回deal处理过的配置
         """
+        self.do_init()
         conf = self.get_data(id, sid, src=src, info = info)
         if conf is None:
+            raise IOCError(f"confs: can't find conf of {id}")
             return None
         deal = self.get_deal(conf.type, sid)
         if deal is None:
+            raise IOCError(f"confs: can't find deal of {id}, type = {conf.type}")
             return None
         #print(f"get_obj: {id}({sid}), conf: {conf}, deal: {deal}, type: {conf.type}")
         if not remove:
             obj = deal(conf)
         else:
             obj = deal.remove(conf)
         return obj
```

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/base.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/call.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/call.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/calls.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/calls.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/conf/deals.js` & `buildz-0.5.1/buildz/ioc/ioc_deal/conf/deals.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -3,15 +3,16 @@
         type: val,
         note: 数据, //note是注释，非必须
         build: buildz.ioc.ioc_deal.val.ValDeal,
         aliases: ['default']
     }, {
         type: object,
         note: 对象,
-        build: buildz.ioc.ioc_deal.obj.ObjectDeal
+        build: buildz.ioc.ioc_deal.obj.ObjectDeal,
+        aliases: [obj]
     }, {
         type: env,
         note: 环境变量,
         build: buildz.ioc.ioc_deal.env.EnvDeal
     }, {
         type: ref,
         note: 引用,
@@ -48,9 +49,18 @@
         type: map,
         note: 字典,
         build: buildz.ioc.ioc_deal.map.MapDeal
     }, {
         type: join,
         note: 文件路径拼接,
         build: buildz.ioc.ioc_deal.join.JoinDeal
+    }, {
+        type: xfile,
+        note: xf配置文件读取,
+        build: buildz.ioc.ioc_deal.xfile.XfileDeal,
+        aliases: [xf]
+    }, {
+        type: deal,
+        note: 扩展的自定义deal方法,
+        build: buildz.ioc.ioc_deal.deal.DealDeal
     }]
 }
```

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/conf/obj_lists.js` & `buildz-0.5.1/buildz/ioc/ioc_deal/conf/obj_lists.js`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/env.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/env.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/ioc.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/ioc.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/join.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/join.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/list.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/list.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/map.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/map.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/mcall.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/mcall.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/obj.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/obj.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,33 +1,44 @@
 #
-from ..ioc.base import Base, EncapeData
+from ..ioc.base import Base, EncapeData,IOCError
 from .base import FormatData,BaseDeal
 from buildz import xf, pyz
 import os
 dp = os.path.dirname(__file__)
 join = os.path.join
 class ObjectDeal(BaseDeal):
     """
         对象object:
             {
                 id: id
                 type: object
                 source: 导入路径+调用方法/类
-                single: 1 //是否单例，默认是
+                single: 1 //是否单例，默认是，
+                        //这里的单例是一个id对应一个实例，
+                        //如果两个id用的同一个source，就是同一个source的两个对象
                 // 构造函数
                 construct:{
                     args: [
                         item_conf,
                         ...
                     ]
                     maps: {
                         key1: item_conf,
                         ...
                     }
                 }
+                //construct和args+maps，不能同时存在
+                args: [
+                    item_conf,
+                    ...
+                ]
+                maps: {
+                    key1: item_conf,
+                    ...
+                }
                 // sets之前调用方法
                 prev_call: item_conf
                 // 对象变量设置属性
                 sets: [
                     {key: key1, data: item_conf }
                     ...
                 ]
@@ -94,21 +105,26 @@
             if single:
                 ids = [sid, id]
             else:
                 ids = [sid, id, cid]
         if ids is not None:
             obj = xf.gets(self.singles, ids)
             if obj is not None:
+                #raise IOCError(f"null for {ids}")
                 return obj
         source = xf.g(data, source=0)
         fc = xf.get(self.sources, source, None)
         if fc is None:
             fc = pyz.load(source)
             self.sources[source]=fc
-        cst = xf.g(data, construct = [])
+        cst = xf.g(data, construct = None)
+        if cst is None:
+            _args = xf.g(data, args = [])
+            _maps = xf.g(data, maps = {})
+            cst = [_args, _maps]
         cst = self.fmt_cst(cst)
         args = xf.g(cst, args=[])
         maps = xf.g(cst, maps={})
         args = [self.get_obj(v, conf) for v in args]
         maps = {k:self.get_obj(maps[k], conf) for k in maps}
         obj = fc(*args, **maps)
         if ids is not None:
```

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/ovar.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/ovar.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/ref.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/ref.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/val.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/val.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/ioc/ioc_deal/var.py` & `buildz-0.5.1/buildz/ioc/ioc_deal/var.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/pyz.py` & `buildz-0.5.1/buildz/pyz.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     """
     mds = md.split(".")
     arr = mds[1:]
     while len(mds)>0:
         try:
             md = __import__(".".join(mds))
             break
-        except:
+        except ModuleNotFoundError as exp:
             mds = mds[:-1]
     if len(mds)==0:
         raise Exception("can't import package from "+md)
     for k in arr:
         md = getattr(md, k)
     if fc is not None:
         fc = getattr(md, fc)
```

### Comparing `buildz-0.4.91/buildz/tz/myers_diff.py` & `buildz-0.5.1/buildz/tz/myers_diff.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/file.py` & `buildz-0.5.1/buildz/xf/file.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/base.py` & `buildz-0.5.1/buildz/xf/loader/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/buffer.py` & `buildz-0.5.1/buildz/xf/loader/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/listz.py` & `buildz-0.5.1/buildz/xf/loader/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/lr.py` & `buildz-0.5.1/buildz/xf/loader/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/lrval.py` & `buildz-0.5.1/buildz/xf/loader/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/mapz.py` & `buildz-0.5.1/buildz/xf/loader/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/nextz.py` & `buildz-0.5.1/buildz/xf/loader/deal/nextz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/reval.py` & `buildz-0.5.1/buildz/xf/loader/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/setz.py` & `buildz-0.5.1/buildz/xf/loader/deal/setz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/spt.py` & `buildz-0.5.1/buildz/xf/loader/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/deal/strz.py` & `buildz-0.5.1/buildz/xf/loader/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/item.py` & `buildz-0.5.1/buildz/xf/loader/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/mg.py` & `buildz-0.5.1/buildz/xf/loader/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loader/pos.py` & `buildz-0.5.1/buildz/xf/loader/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/base.py` & `buildz-0.5.1/buildz/xf/loaderz/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/buffer.py` & `buildz-0.5.1/buildz/xf/loaderz/buffer.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/listz.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/lr.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/lr.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/lrval.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/lrval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/mapz.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/reval.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/reval.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/spt.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/spt.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/deal/strz.py` & `buildz-0.5.1/buildz/xf/loaderz/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/item.py` & `buildz-0.5.1/buildz/xf/loaderz/item.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/mg.py` & `buildz-0.5.1/buildz/xf/loaderz/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/pos.py` & `buildz-0.5.1/buildz/xf/loaderz/pos.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/loaderz/test.py` & `buildz-0.5.1/buildz/xf/loaderz/test.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/mapz.py` & `buildz-0.5.1/buildz/xf/mapz.py`

 * *Files 9% similar despite different names*

```diff
@@ -84,13 +84,13 @@
     for k in src:
         val = src[k]
         if k not in target:
             target[k] = val
             continue
         mval = target[k]
         if type(mval) == dict and type(val)==dict:
-            update_maps(mval, val, replace)
+            deep_update(mval, val, replace)
         else:
             if replace:
                 target[k] = val
 
 pass
```

### Comparing `buildz-0.4.91/buildz/xf/read.py` & `buildz-0.5.1/buildz/xf/read.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/readz.py` & `buildz-0.5.1/buildz/xf/readz.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     mgs.add(reval.ValDeal("[\+\-]?\d*\.\d+", float))
     mgs.add(reval.ValDeal("[\+\-]?\d+e[\+\-]?\d+", float))
     mgs.add(reval.ValDeal("null", lambda x:None))
     mgs.add(reval.ValDeal("true", lambda x:True))
     mgs.add(reval.ValDeal("false", lambda x:False))
 
 pass
-def build():
-    mgs = mg.Manager()
+def build(as_bytes=False):
+    mgs = mg.Manager(as_bytes)
     build_val(mgs)
     mgs.add(strz.PrevStrDeal("r'''","'''",0,0,0))
     mgs.add(strz.PrevStrDeal('r"""','"""',0,0,0))
     mgs.add(strz.PrevStrDeal("r'","'",1,0,0))
     mgs.add(strz.PrevStrDeal('r"','"',1,0,0))
     mgs.add(strz.PrevStrDeal("###","###",0,1))
     mgs.add(strz.PrevStrDeal("/*","*/",0,1))
@@ -67,16 +67,16 @@
     mgs.add(listz.ListDeal("(", ")"))
     mgs.add(listz.ListDeal("[", "]"))
     mgs.add(mapz.MapDeal("{", "}"))
     mgs.add(nextz.PrevNextDeal())
     return mgs
 
 pass
-def load(read):
-    mgs = build()
+def load(read, as_bytes = False):
+    mgs = build(as_bytes)
     return msg.loads(read)
 def loads(s):
-    mgs = build()
+    mgs = build(type(s)==bytes)
     input = buffer.BufferInput(s)
     return mgs.loads(s)
 
 pass
```

### Comparing `buildz-0.4.91/buildz/xf/stack.py` & `buildz-0.5.1/buildz/xf/stack.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/write.py` & `buildz-0.5.1/buildz/xf/write.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/base.py` & `buildz-0.5.1/buildz/xf/writer/base.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/conf.py` & `buildz-0.5.1/buildz/xf/writer/conf.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/deal/listz.py` & `buildz-0.5.1/buildz/xf/writer/deal/listz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/deal/mapz.py` & `buildz-0.5.1/buildz/xf/writer/deal/mapz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/deal/strz.py` & `buildz-0.5.1/buildz/xf/writer/deal/strz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/itemz.py` & `buildz-0.5.1/buildz/xf/writer/itemz.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/writer/mg.py` & `buildz-0.5.1/buildz/xf/writer/mg.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz/xf/xargs.py` & `buildz-0.5.1/buildz/xf/xargs.py`

 * *Files identical despite different names*

### Comparing `buildz-0.4.91/buildz.egg-info/PKG-INFO` & `buildz-0.5.1/buildz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: buildz
-Version: 0.4.91
+Version: 0.5.1
 Summary: a json-base file format's read and write code by python, and codes to read and product object from configure file in such format
 Home-page: https://github.com/buildCodeZ/buildz
 Author: Zzz
 Author-email: 1309458652@qq.com
 License: Apache License 2.0
 Keywords: buildz
 Platform: any
```

### Comparing `buildz-0.4.91/buildz.egg-info/SOURCES.txt` & `buildz-0.5.1/buildz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -38,30 +38,33 @@
 buildz/ioc/init.py
 buildz/ioc/ioc/base.py
 buildz/ioc/ioc/conf.py
 buildz/ioc/ioc/confs.py
 buildz/ioc/ioc_deal/base.py
 buildz/ioc/ioc_deal/call.py
 buildz/ioc/ioc_deal/calls.py
+buildz/ioc/ioc_deal/deal.py
 buildz/ioc/ioc_deal/demo.py
 buildz/ioc/ioc_deal/env.py
 buildz/ioc/ioc_deal/ioc.py
 buildz/ioc/ioc_deal/join.py
 buildz/ioc/ioc_deal/list.py
 buildz/ioc/ioc_deal/map.py
 buildz/ioc/ioc_deal/mcall.py
 buildz/ioc/ioc_deal/obj.py
 buildz/ioc/ioc_deal/ovar.py
 buildz/ioc/ioc_deal/ref.py
 buildz/ioc/ioc_deal/val.py
 buildz/ioc/ioc_deal/var.py
+buildz/ioc/ioc_deal/xfile.py
 buildz/ioc/ioc_deal/conf/call_defaults.js
 buildz/ioc/ioc_deal/conf/call_lists.js
 buildz/ioc/ioc_deal/conf/calls_defaults.js
 buildz/ioc/ioc_deal/conf/calls_lists.js
+buildz/ioc/ioc_deal/conf/deal_lists.js
 buildz/ioc/ioc_deal/conf/deals.js
 buildz/ioc/ioc_deal/conf/env_lists.js
 buildz/ioc/ioc_deal/conf/ioc_lists.js
 buildz/ioc/ioc_deal/conf/join_lists.js
 buildz/ioc/ioc_deal/conf/list_lists.js
 buildz/ioc/ioc_deal/conf/map_lists.js
 buildz/ioc/ioc_deal/conf/mcall_defaults.js
@@ -69,14 +72,16 @@
 buildz/ioc/ioc_deal/conf/obj_cst_lists.js
 buildz/ioc/ioc_deal/conf/obj_defaults.js
 buildz/ioc/ioc_deal/conf/obj_lists.js
 buildz/ioc/ioc_deal/conf/obj_set_lists.js
 buildz/ioc/ioc_deal/conf/ovar_lists.js
 buildz/ioc/ioc_deal/conf/ref_lists.js
 buildz/ioc/ioc_deal/conf/var_lists.js
+buildz/ioc/ioc_deal/conf/xfile_defaults.js
+buildz/ioc/ioc_deal/conf/xfile_lists.js
 buildz/tz/__init__.py
 buildz/tz/myers_diff.py
 buildz/xf/__init__.py
 buildz/xf/__main__.py
 buildz/xf/file.py
 buildz/xf/mapz.py
 buildz/xf/read.py
```

### Comparing `buildz-0.4.91/setup.py` & `buildz-0.5.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Author: Zzz(1309458652@qq.com)
 # Description:
 
 from setuptools import setup, find_packages
 
 setup(
     name = 'buildz',
-    version = '0.4.91',
+    version = '0.5.1',
     keywords='buildz',
     long_description=open('README.md', 'r', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     description = "a json-base file format's read and write code by python, and codes to read and product object from configure file in such format",
     license = 'Apache License 2.0',
     url = 'https://github.com/buildCodeZ/buildz',
     author = 'Zzz',
```

