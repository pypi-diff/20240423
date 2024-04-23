# Comparing `tmp/mapdata-3.5.0.tar.gz` & `tmp/mapdata-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapdata-3.5.0.tar", last modified: Sun Apr  7 23:48:42 2024, max compression
+gzip compressed data, was "mapdata-3.6.0.tar", last modified: Tue Apr 23 00:16:32 2024, max compression
```

## Comparing `mapdata-3.5.0.tar` & `mapdata-3.6.0.tar`

### file list

```diff
@@ -1,216 +1,216 @@
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.455303 mapdata-3.5.0/
--rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.5.0/LICENSE.txt
--rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.5.0/MANIFEST.in
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-07 23:48:42.451303 mapdata-3.5.0/PKG-INFO
--rw-r--r--   0 dreas     (1000) dreas     (1000)     6306 2024-04-04 16:58:57.000000 mapdata-3.5.0/README.md
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/configfile/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.5.0/mapdata/configfile/mapdata.conf
--rwxrwxr-x   0 dreas     (1000) dreas     (1000)   657069 2024-04-07 23:40:24.000000 mapdata-3.5.0/mapdata/mapdata.py
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.403303 mapdata-3.5.0/mapdata/symbols/
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/16x16/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/0.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.5.0/mapdata/symbols/16x16/2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/5.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.5.0/mapdata/symbols/16x16/6.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/7.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.5.0/mapdata/symbols/16x16/9.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/A.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.5.0/mapdata/symbols/16x16/B.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/C.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/D.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/E.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/F.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/G.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/H.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.5.0/mapdata/symbols/16x16/I.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/J.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/K.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/L.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.5.0/mapdata/symbols/16x16/M.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/N.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/O.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/P.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.5.0/mapdata/symbols/16x16/Q.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/R.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.5.0/mapdata/symbols/16x16/S.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/T.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/U.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/V.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/W.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/X.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/Y.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/Z.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/airplane.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/anchor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/ball.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/ball_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.5.0/mapdata/symbols/16x16/bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/bars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/binoculars.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/bird.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/block.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.5.0/mapdata/symbols/16x16/block_small.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/bookmark.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.5.0/mapdata/symbols/16x16/box_stack.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/camera.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/cancel.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/car.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/car2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/center8.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/check.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/check_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/checkbox.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/checkerboard.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/chevrons.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_bar.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.5.0/mapdata/symbols/16x16/circle_x.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/clock.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/columns.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/contract.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.5.0/mapdata/symbols/16x16/cross.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/darkeye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.5.0/mapdata/symbols/16x16/decrease.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/deposition.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ll.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_lr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ul.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/diag_ur.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/dialog.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/diamond.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/donkey.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/dot.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.5.0/mapdata/symbols/16x16/down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.5.0/mapdata/symbols/16x16/drop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/elephant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/expand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.5.0/mapdata/symbols/16x16/eye.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.5.0/mapdata/symbols/16x16/fire.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/fish.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.5.0/mapdata/symbols/16x16/flag.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.5.0/mapdata/symbols/16x16/flag2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/four_arrows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.5.0/mapdata/symbols/16x16/graph.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/hand.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/hash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.5.0/mapdata/symbols/16x16/heart.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/hidden.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/hourglass.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/house.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/increase.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/info.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/leaf.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightbulb.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.5.0/mapdata/symbols/16x16/lightning2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/location_ptr.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/mine.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/nested_boxes.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.5.0/mapdata/symbols/16x16/pennant.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/pennant2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.5.0/mapdata/symbols/16x16/people.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/person.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/person2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/person3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.5.0/mapdata/symbols/16x16/phone.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/photo.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/picnic.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.5.0/mapdata/symbols/16x16/plus.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_down.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_left.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/point_up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_ne.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_nw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_se.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/pointer_sw.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.5.0/mapdata/symbols/16x16/puzzle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/q1.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.5.0/mapdata/symbols/16x16/q1_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.5.0/mapdata/symbols/16x16/q2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.5.0/mapdata/symbols/16x16/q2_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.5.0/mapdata/symbols/16x16/q3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.5.0/mapdata/symbols/16x16/q3_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/q4.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/q4_notch.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.5.0/mapdata/symbols/16x16/qmark_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/qmark_circle2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/raincloud.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/right.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/rocket.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/rocket2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.5.0/mapdata/symbols/16x16/rose.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/rows.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/scales.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/search.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.5.0/mapdata/symbols/16x16/search2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.5.0/mapdata/symbols/16x16/skull.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/square.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.5.0/mapdata/symbols/16x16/star.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.5.0/mapdata/symbols/16x16/stipple.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/stop.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/surprise_circle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.5.0/mapdata/symbols/16x16/swamp.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/target.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.5.0/mapdata/symbols/16x16/target2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/ten.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.5.0/mapdata/symbols/16x16/trash.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.5.0/mapdata/symbols/16x16/tree3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle_open.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.5.0/mapdata/symbols/16x16/triangle_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.5.0/mapdata/symbols/16x16/up.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.5.0/mapdata/symbols/16x16/vapor.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.5.0/mapdata/symbols/16x16/warning.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.5.0/mapdata/symbols/16x16/wave3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/weather.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedge.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedge_sm.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.5.0/mapdata/symbols/16x16/wedges_3.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.5.0/mapdata/symbols/16x16/well.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.5.0/mapdata/symbols/16x16/whale.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.5.0/mapdata/symbols/16x16/whale2.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.5.0/mapdata/symbols/16x16/wheelchair.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.5.0/mapdata/symbols/16x16/zigzags.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.5.0/mapdata/symbols/16x16/zigzags2.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/20x20/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.5.0/mapdata/symbols/20x20/ball20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.5.0/mapdata/symbols/20x20/block20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.5.0/mapdata/symbols/20x20/circle20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.5.0/mapdata/symbols/20x20/q1_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.5.0/mapdata/symbols/20x20/q2_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.5.0/mapdata/symbols/20x20/q3_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.5.0/mapdata/symbols/20x20/q4_20.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.5.0/mapdata/symbols/20x20/square20.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/24x24/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.5.0/mapdata/symbols/24x24/ball24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.5.0/mapdata/symbols/24x24/block24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.5.0/mapdata/symbols/24x24/circle24.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.5.0/mapdata/symbols/24x24/square24.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata/symbols/28x28/
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.5.0/mapdata/symbols/28x28/ball28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.5.0/mapdata/symbols/28x28/block28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.5.0/mapdata/symbols/28x28/circle28.xbm
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.5.0/mapdata/symbols/28x28/square28.xbm
-drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-07 23:48:42.451303 mapdata-3.5.0/mapdata.egg-info/
--rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/PKG-INFO
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/SOURCES.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/dependency_links.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/requires.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-04-07 23:48:42.000000 mapdata-3.5.0/mapdata.egg-info/top_level.txt
--rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-04-07 23:48:42.455303 mapdata-3.5.0/setup.cfg
--rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-04-04 00:31:55.000000 mapdata-3.5.0/setup.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.412721 mapdata-3.6.0/
+-rw-------   0 dreas     (1000) dreas     (1000)      614 2023-05-10 02:52:31.000000 mapdata-3.6.0/LICENSE.txt
+-rw-------   0 dreas     (1000) dreas     (1000)       88 2022-01-15 18:16:09.000000 mapdata-3.6.0/MANIFEST.in
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-23 00:16:32.412721 mapdata-3.6.0/PKG-INFO
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     6306 2024-04-04 16:58:57.000000 mapdata-3.6.0/README.md
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.372720 mapdata-3.6.0/mapdata/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.372720 mapdata-3.6.0/mapdata/configfile/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     9002 2024-03-04 21:04:24.000000 mapdata-3.6.0/mapdata/configfile/mapdata.conf
+-rwxrwxr-x   0 dreas     (1000) dreas     (1000)   672633 2024-04-22 23:37:52.000000 mapdata-3.6.0/mapdata/mapdata.py
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.372720 mapdata-3.6.0/mapdata/symbols/
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.408721 mapdata-3.6.0/mapdata/symbols/16x16/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:04:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/0.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:16.000000 mapdata-3.6.0/mapdata/symbols/16x16/1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:29.000000 mapdata-3.6.0/mapdata/symbols/16x16/2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:05:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:05:52.000000 mapdata-3.6.0/mapdata/symbols/16x16/4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:06:03.000000 mapdata-3.6.0/mapdata/symbols/16x16/5.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:28:02.000000 mapdata-3.6.0/mapdata/symbols/16x16/6.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:27.000000 mapdata-3.6.0/mapdata/symbols/16x16/7.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-05-16 14:06:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2024-01-31 04:26:59.000000 mapdata-3.6.0/mapdata/symbols/16x16/9.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:04:26.000000 mapdata-3.6.0/mapdata/symbols/16x16/A.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:07:30.000000 mapdata-3.6.0/mapdata/symbols/16x16/B.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:10:14.000000 mapdata-3.6.0/mapdata/symbols/16x16/C.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:13:27.000000 mapdata-3.6.0/mapdata/symbols/16x16/D.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-15 16:14:22.000000 mapdata-3.6.0/mapdata/symbols/16x16/E.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-15 16:15:26.000000 mapdata-3.6.0/mapdata/symbols/16x16/F.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 00:14:24.000000 mapdata-3.6.0/mapdata/symbols/16x16/G.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:15:07.000000 mapdata-3.6.0/mapdata/symbols/16x16/H.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:16:00.000000 mapdata-3.6.0/mapdata/symbols/16x16/I.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:18:38.000000 mapdata-3.6.0/mapdata/symbols/16x16/J.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:21:25.000000 mapdata-3.6.0/mapdata/symbols/16x16/K.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:22:10.000000 mapdata-3.6.0/mapdata/symbols/16x16/L.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:24:58.000000 mapdata-3.6.0/mapdata/symbols/16x16/M.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 00:27:42.000000 mapdata-3.6.0/mapdata/symbols/16x16/N.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 14:04:25.000000 mapdata-3.6.0/mapdata/symbols/16x16/O.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:28:05.000000 mapdata-3.6.0/mapdata/symbols/16x16/P.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:29:12.000000 mapdata-3.6.0/mapdata/symbols/16x16/Q.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:30:16.000000 mapdata-3.6.0/mapdata/symbols/16x16/R.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:34:31.000000 mapdata-3.6.0/mapdata/symbols/16x16/S.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:35:37.000000 mapdata-3.6.0/mapdata/symbols/16x16/T.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:37:27.000000 mapdata-3.6.0/mapdata/symbols/16x16/U.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:40:22.000000 mapdata-3.6.0/mapdata/symbols/16x16/V.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:44:48.000000 mapdata-3.6.0/mapdata/symbols/16x16/W.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:46:24.000000 mapdata-3.6.0/mapdata/symbols/16x16/X.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-05-16 03:47:50.000000 mapdata-3.6.0/mapdata/symbols/16x16/Y.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-16 03:49:43.000000 mapdata-3.6.0/mapdata/symbols/16x16/Z.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-21 14:55:41.000000 mapdata-3.6.0/mapdata/symbols/16x16/airplane.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-06-24 15:22:11.000000 mapdata-3.6.0/mapdata/symbols/16x16/anchor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:00:25.000000 mapdata-3.6.0/mapdata/symbols/16x16/ball.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2024-01-24 20:44:54.000000 mapdata-3.6.0/mapdata/symbols/16x16/ball_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-16 13:39:00.000000 mapdata-3.6.0/mapdata/symbols/16x16/bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-07-04 17:04:48.000000 mapdata-3.6.0/mapdata/symbols/16x16/bars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:43:55.000000 mapdata-3.6.0/mapdata/symbols/16x16/binoculars.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:29:19.000000 mapdata-3.6.0/mapdata/symbols/16x16/bird.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      288 2023-04-24 16:37:43.000000 mapdata-3.6.0/mapdata/symbols/16x16/block.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2024-01-26 04:36:33.000000 mapdata-3.6.0/mapdata/symbols/16x16/block_small.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-16 18:31:20.000000 mapdata-3.6.0/mapdata/symbols/16x16/bookmark.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:29:01.000000 mapdata-3.6.0/mapdata/symbols/16x16/box_stack.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-04-30 14:46:15.000000 mapdata-3.6.0/mapdata/symbols/16x16/camera.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 16:51:47.000000 mapdata-3.6.0/mapdata/symbols/16x16/cancel.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-05-21 15:05:05.000000 mapdata-3.6.0/mapdata/symbols/16x16/car.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-21 15:04:37.000000 mapdata-3.6.0/mapdata/symbols/16x16/car2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-24 01:00:13.000000 mapdata-3.6.0/mapdata/symbols/16x16/center8.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:35:37.000000 mapdata-3.6.0/mapdata/symbols/16x16/check.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 14:51:14.000000 mapdata-3.6.0/mapdata/symbols/16x16/check_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-16 14:20:03.000000 mapdata-3.6.0/mapdata/symbols/16x16/checkbox.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-04-28 13:31:04.000000 mapdata-3.6.0/mapdata/symbols/16x16/checkerboard.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:29:46.000000 mapdata-3.6.0/mapdata/symbols/16x16/chevrons.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:12:28.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 14:22:20.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_bar.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 14:58:14.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:09:20.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 14:29:15.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-25 14:40:36.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-06-24 14:56:37.000000 mapdata-3.6.0/mapdata/symbols/16x16/circle_x.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-07-04 17:10:15.000000 mapdata-3.6.0/mapdata/symbols/16x16/clock.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 14:05:41.000000 mapdata-3.6.0/mapdata/symbols/16x16/columns.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:50:11.000000 mapdata-3.6.0/mapdata/symbols/16x16/contract.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      275 2023-04-16 17:48:39.000000 mapdata-3.6.0/mapdata/symbols/16x16/cross.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-23 18:45:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/darkeye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:32.000000 mapdata-3.6.0/mapdata/symbols/16x16/decrease.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-30 12:46:46.000000 mapdata-3.6.0/mapdata/symbols/16x16/deposition.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:47.000000 mapdata-3.6.0/mapdata/symbols/16x16/diag_ll.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:26.000000 mapdata-3.6.0/mapdata/symbols/16x16/diag_lr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:16:05.000000 mapdata-3.6.0/mapdata/symbols/16x16/diag_ul.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2024-01-30 23:17:04.000000 mapdata-3.6.0/mapdata/symbols/16x16/diag_ur.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-20 18:41:19.000000 mapdata-3.6.0/mapdata/symbols/16x16/dialog.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-16 17:38:10.000000 mapdata-3.6.0/mapdata/symbols/16x16/diamond.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-05-16 13:47:24.000000 mapdata-3.6.0/mapdata/symbols/16x16/donkey.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 16:45:55.000000 mapdata-3.6.0/mapdata/symbols/16x16/dot.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:00:44.000000 mapdata-3.6.0/mapdata/symbols/16x16/down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:38:22.000000 mapdata-3.6.0/mapdata/symbols/16x16/drop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-03 02:15:55.000000 mapdata-3.6.0/mapdata/symbols/16x16/elephant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-25 14:33:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/expand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-04-30 15:03:32.000000 mapdata-3.6.0/mapdata/symbols/16x16/eye.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 13:59:48.000000 mapdata-3.6.0/mapdata/symbols/16x16/fire.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 22:13:54.000000 mapdata-3.6.0/mapdata/symbols/16x16/fish.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:36:11.000000 mapdata-3.6.0/mapdata/symbols/16x16/flag.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-30 15:04:58.000000 mapdata-3.6.0/mapdata/symbols/16x16/flag2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-06-24 15:06:07.000000 mapdata-3.6.0/mapdata/symbols/16x16/four_arrows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:25:14.000000 mapdata-3.6.0/mapdata/symbols/16x16/graph.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-06-24 15:18:19.000000 mapdata-3.6.0/mapdata/symbols/16x16/hand.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:04:09.000000 mapdata-3.6.0/mapdata/symbols/16x16/hash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-03 01:53:41.000000 mapdata-3.6.0/mapdata/symbols/16x16/heart.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2024-01-31 04:51:54.000000 mapdata-3.6.0/mapdata/symbols/16x16/hidden.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-24 15:40:09.000000 mapdata-3.6.0/mapdata/symbols/16x16/hourglass.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 22:31:53.000000 mapdata-3.6.0/mapdata/symbols/16x16/house.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 13:18:05.000000 mapdata-3.6.0/mapdata/symbols/16x16/increase.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-24 23:05:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/info.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-30 14:51:36.000000 mapdata-3.6.0/mapdata/symbols/16x16/leaf.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:02:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-06-23 13:36:40.000000 mapdata-3.6.0/mapdata/symbols/16x16/lightbulb.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 16:38:25.000000 mapdata-3.6.0/mapdata/symbols/16x16/lightning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      314 2023-04-28 13:14:23.000000 mapdata-3.6.0/mapdata/symbols/16x16/lightning2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-07-04 16:58:13.000000 mapdata-3.6.0/mapdata/symbols/16x16/location_ptr.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:06:42.000000 mapdata-3.6.0/mapdata/symbols/16x16/mine.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-06-24 15:07:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/nested_boxes.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-28 14:07:35.000000 mapdata-3.6.0/mapdata/symbols/16x16/pennant.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:16:09.000000 mapdata-3.6.0/mapdata/symbols/16x16/pennant2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-18 19:04:36.000000 mapdata-3.6.0/mapdata/symbols/16x16/people.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:26:34.000000 mapdata-3.6.0/mapdata/symbols/16x16/person.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-16 14:30:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/person2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 18:43:50.000000 mapdata-3.6.0/mapdata/symbols/16x16/person3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 15:37:42.000000 mapdata-3.6.0/mapdata/symbols/16x16/phone.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:18:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/photo.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-19 22:48:26.000000 mapdata-3.6.0/mapdata/symbols/16x16/picnic.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-19 03:57:15.000000 mapdata-3.6.0/mapdata/symbols/16x16/plus.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:16.000000 mapdata-3.6.0/mapdata/symbols/16x16/point_down.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:58:03.000000 mapdata-3.6.0/mapdata/symbols/16x16/point_left.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      362 2023-05-03 01:57:47.000000 mapdata-3.6.0/mapdata/symbols/16x16/point_right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      347 2023-05-03 01:56:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/point_up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:58:38.000000 mapdata-3.6.0/mapdata/symbols/16x16/pointer_ne.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      356 2023-05-03 01:59:20.000000 mapdata-3.6.0/mapdata/symbols/16x16/pointer_nw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      358 2023-05-03 01:58:54.000000 mapdata-3.6.0/mapdata/symbols/16x16/pointer_se.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      357 2023-05-03 01:59:07.000000 mapdata-3.6.0/mapdata/symbols/16x16/pointer_sw.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 18:51:06.000000 mapdata-3.6.0/mapdata/symbols/16x16/puzzle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:52:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/q1.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:57:59.000000 mapdata-3.6.0/mapdata/symbols/16x16/q1_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:25.000000 mapdata-3.6.0/mapdata/symbols/16x16/q2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:55.000000 mapdata-3.6.0/mapdata/symbols/16x16/q2_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:46.000000 mapdata-3.6.0/mapdata/symbols/16x16/q3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:28.000000 mapdata-3.6.0/mapdata/symbols/16x16/q3_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2024-01-24 00:53:57.000000 mapdata-3.6.0/mapdata/symbols/16x16/q4.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2024-01-24 00:58:13.000000 mapdata-3.6.0/mapdata/symbols/16x16/q4_notch.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      308 2023-05-20 18:36:19.000000 mapdata-3.6.0/mapdata/symbols/16x16/qmark_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-20 18:37:52.000000 mapdata-3.6.0/mapdata/symbols/16x16/qmark_circle2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 13:43:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/raincloud.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-04-24 16:39:34.000000 mapdata-3.6.0/mapdata/symbols/16x16/right.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-05-20 17:23:57.000000 mapdata-3.6.0/mapdata/symbols/16x16/rocket.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-20 17:25:43.000000 mapdata-3.6.0/mapdata/symbols/16x16/rocket2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-23 16:07:27.000000 mapdata-3.6.0/mapdata/symbols/16x16/rose.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-28 14:05:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/rows.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 14:27:34.000000 mapdata-3.6.0/mapdata/symbols/16x16/scales.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-07-04 17:07:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/search.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-07-04 17:08:06.000000 mapdata-3.6.0/mapdata/symbols/16x16/search2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-01 15:46:45.000000 mapdata-3.6.0/mapdata/symbols/16x16/skull.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-17 02:43:53.000000 mapdata-3.6.0/mapdata/symbols/16x16/square.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 18:26:56.000000 mapdata-3.6.0/mapdata/symbols/16x16/star.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-04-28 13:07:07.000000 mapdata-3.6.0/mapdata/symbols/16x16/stipple.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-03 02:10:57.000000 mapdata-3.6.0/mapdata/symbols/16x16/stop.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      317 2023-06-24 15:31:50.000000 mapdata-3.6.0/mapdata/symbols/16x16/surprise_circle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:22:10.000000 mapdata-3.6.0/mapdata/symbols/16x16/swamp.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-16 18:27:50.000000 mapdata-3.6.0/mapdata/symbols/16x16/target.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:37:09.000000 mapdata-3.6.0/mapdata/symbols/16x16/target2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      281 2023-06-24 15:27:04.000000 mapdata-3.6.0/mapdata/symbols/16x16/ten.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-24 14:54:31.000000 mapdata-3.6.0/mapdata/symbols/16x16/trash.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-09 17:01:43.000000 mapdata-3.6.0/mapdata/symbols/16x16/tree.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-28 12:59:30.000000 mapdata-3.6.0/mapdata/symbols/16x16/tree2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:26:26.000000 mapdata-3.6.0/mapdata/symbols/16x16/tree3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-09 16:59:51.000000 mapdata-3.6.0/mapdata/symbols/16x16/triangle.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      311 2023-05-09 17:08:13.000000 mapdata-3.6.0/mapdata/symbols/16x16/triangle_open.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-05-20 17:46:38.000000 mapdata-3.6.0/mapdata/symbols/16x16/triangle_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      278 2023-04-16 18:01:12.000000 mapdata-3.6.0/mapdata/symbols/16x16/up.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-06-30 12:50:50.000000 mapdata-3.6.0/mapdata/symbols/16x16/vapor.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 03:55:52.000000 mapdata-3.6.0/mapdata/symbols/16x16/warning.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-04-16 20:02:51.000000 mapdata-3.6.0/mapdata/symbols/16x16/wave.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:01.000000 mapdata-3.6.0/mapdata/symbols/16x16/wave2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      287 2023-05-19 04:12:43.000000 mapdata-3.6.0/mapdata/symbols/16x16/wave3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      305 2023-04-30 14:42:04.000000 mapdata-3.6.0/mapdata/symbols/16x16/weather.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-24 16:37:24.000000 mapdata-3.6.0/mapdata/symbols/16x16/wedge.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-25 13:53:34.000000 mapdata-3.6.0/mapdata/symbols/16x16/wedge_sm.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-04-29 15:40:02.000000 mapdata-3.6.0/mapdata/symbols/16x16/wedges_3.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      284 2023-05-20 14:23:44.000000 mapdata-3.6.0/mapdata/symbols/16x16/well.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      299 2023-04-24 22:20:04.000000 mapdata-3.6.0/mapdata/symbols/16x16/whale.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      290 2023-04-28 12:54:47.000000 mapdata-3.6.0/mapdata/symbols/16x16/whale2.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      302 2023-06-24 15:49:53.000000 mapdata-3.6.0/mapdata/symbols/16x16/wheelchair.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      293 2023-05-19 04:04:57.000000 mapdata-3.6.0/mapdata/symbols/16x16/zigzags.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      296 2023-05-19 04:39:05.000000 mapdata-3.6.0/mapdata/symbols/16x16/zigzags2.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.408721 mapdata-3.6.0/mapdata/symbols/20x20/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      464 2023-06-24 14:14:12.000000 mapdata-3.6.0/mapdata/symbols/20x20/ball20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      467 2023-06-24 14:24:29.000000 mapdata-3.6.0/mapdata/symbols/20x20/block20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:13:06.000000 mapdata-3.6.0/mapdata/symbols/20x20/circle20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:11.000000 mapdata-3.6.0/mapdata/symbols/20x20/q1_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:22.000000 mapdata-3.6.0/mapdata/symbols/20x20/q2_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:35.000000 mapdata-3.6.0/mapdata/symbols/20x20/q3_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      461 2024-01-24 00:55:54.000000 mapdata-3.6.0/mapdata/symbols/20x20/q4_20.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      470 2023-06-24 14:24:00.000000 mapdata-3.6.0/mapdata/symbols/20x20/square20.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.412721 mapdata-3.6.0/mapdata/symbols/24x24/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      539 2023-06-24 14:20:48.000000 mapdata-3.6.0/mapdata/symbols/24x24/ball24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      542 2023-06-24 14:25:39.000000 mapdata-3.6.0/mapdata/symbols/24x24/block24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:20:00.000000 mapdata-3.6.0/mapdata/symbols/24x24/circle24.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      545 2023-06-24 14:22:10.000000 mapdata-3.6.0/mapdata/symbols/24x24/square24.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.412721 mapdata-3.6.0/mapdata/symbols/28x28/
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      793 2023-06-24 14:41:23.000000 mapdata-3.6.0/mapdata/symbols/28x28/ball28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      794 2023-06-24 14:42:33.000000 mapdata-3.6.0/mapdata/symbols/28x28/block28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:41:39.000000 mapdata-3.6.0/mapdata/symbols/28x28/circle28.xbm
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      797 2023-06-24 14:42:15.000000 mapdata-3.6.0/mapdata/symbols/28x28/square28.xbm
+drwxrwxr-x   0 dreas     (1000) dreas     (1000)        0 2024-04-23 00:16:32.412721 mapdata-3.6.0/mapdata.egg-info/
+-rw-r--r--   0 dreas     (1000) dreas     (1000)     7783 2024-04-23 00:16:32.000000 mapdata-3.6.0/mapdata.egg-info/PKG-INFO
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     6598 2024-04-23 00:16:32.000000 mapdata-3.6.0/mapdata.egg-info/SOURCES.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        1 2024-04-23 00:16:32.000000 mapdata-3.6.0/mapdata.egg-info/dependency_links.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)      143 2024-04-23 00:16:32.000000 mapdata-3.6.0/mapdata.egg-info/requires.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)        8 2024-04-23 00:16:32.000000 mapdata-3.6.0/mapdata.egg-info/top_level.txt
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)       38 2024-04-23 00:16:32.412721 mapdata-3.6.0/setup.cfg
+-rw-rw-r--   0 dreas     (1000) dreas     (1000)     1813 2024-04-20 16:47:59.000000 mapdata-3.6.0/setup.py
```

### Comparing `mapdata-3.5.0/LICENSE.txt` & `mapdata-3.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/PKG-INFO` & `mapdata-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.5.0
+Version: 3.6.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.5.0/README.md` & `mapdata-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/configfile/mapdata.conf` & `mapdata-3.6.0/mapdata/configfile/mapdata.conf`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/mapdata.py` & `mapdata-3.6.0/mapdata/mapdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 # 	The GNU General Public License is available at <http://www.gnu.org/licenses/>
 #
 # AUTHOR
 #	Dreas Nielsen (RDN)
 #
 # ==================================================================
 
-version = "3.5.0"
-vdate = "2024-04-07"
+version = "3.6.0"
+vdate = "2024-04-22"
 
 copyright = "2023-2024"
 
 
 import sys
 import os.path
 import io
@@ -1235,14 +1235,38 @@
 #		if d_sd == 0.0:
 #			return 1
 #		else:
 #			nd = len(d)
 #			return math.ceil((3.49 * d_sd)/(nd**(1.0/3)))
 
 
+def xicor(X, Y, ties=True):
+	# xi correlation coefficient.  Adapted from https://towardsdatascience.com/a-new-coefficient-of-correlation-64ae4f260310
+    n = len(X)
+    order = np.array([i[0] for i in sorted(enumerate(X), key=lambda x: x[1])])
+    if ties:
+        l = np.array([sum(y >= Y[order]) for y in Y[order]])
+        r = l.copy()
+        for j in range(n):
+            if sum([r[j] == r[i] for i in range(n)]) > 1:
+                tie_index = np.array([r[j] == r[i] for i in range(n)])
+                r[tie_index] = np.random.choice(r[tie_index] - np.arange(0, sum([r[j] == r[i] for i in range(n)])), sum(tie_index), replace=False)
+        return 1 - n*sum( abs(r[1:] - r[:n-1]) ) / (2*sum(l*(n - l)))
+    else:
+        r = np.array([sum(y >= Y[order]) for y in Y[order]])
+        return 1 - 3 * sum( abs(r[1:] - r[:n-1]) ) / (n**2 - 1)
+
+def pearsonstat(x, y):
+	return spstats.pearsonr(x, y).statistic
+def spearmanstat(x, y):
+	return spstats.spearmanr(x, y).statistic
+def kendallstat(x, y):
+	return spstats.kendalltau(x, y).statistic
+
+
 class VScrollFrame(ttk.Frame):
 	# A custom frame with a vertical scrollbar.
 	# Widgets should be added to the embedded 'content_frame'.
 	def __init__(self, parent, height=150, *args, **kwargs):
 		ttk.Frame.__init__(self, parent, *args, **kwargs)
 		self.canvas = tk.Canvas(self, bd=0, highlightthickness=0, height=height)
 		self.canvas.grid(row=0, column=0, sticky=tk.NSEW)
@@ -1360,18 +1384,15 @@
 	# in an enclosing frame.
 	# This does not grid the table frame in its parent widget.
 	# Returns a tuple of 0: the frame containing the table,  and 1: the table widget itself.
 	nrows = range(len(rowset))
 	ncols = range(len(column_headers))
 	hdrwidths = [len(column_headers[j]) for j in ncols]
 	if len(rowset) > 0:
-		if sys.version_info < (3,):
-			datawidthtbl = [[len(rowset[i][j] if isinstance(rowset[i][j], str) else type(u"")(rowset[i][j])) for i in nrows] for j in ncols]
-		else:
-			datawidthtbl = [[len(rowset[i][j] if isinstance(rowset[i][j], str) else str(rowset[i][j])) for i in nrows] for j in ncols]
+		datawidthtbl = [[len(rowset[i][j] if isinstance(rowset[i][j], str) else str(rowset[i][j])) for i in nrows] for j in ncols]
 		datawidths = [max(cwidths) for cwidths in datawidthtbl]
 	else:
 		datawidths = hdrwidths
 	colwidths = [max(hdrwidths[i], datawidths[i]) for i in ncols]
 	# Set the font.
 	ff = tkfont.nametofont("TkFixedFont")
 	tblstyle = ttk.Style()
@@ -1426,18 +1447,23 @@
 	colhdrs.append(column_name)
 	colwidths.append(colwidth*charpixels)
 	tv_table["columns"] = tuple(colhdrs)
 	for i, col in enumerate(colhdrs):
 		tv_table.column(col, width = colwidths[i], stretch=tk.NO)
 	for col in hdr_attrs:
 		tv_table.heading(col, **hdr_attrs[col])
+	allrowids = tv_table.get_children()
+	if len(item_ids) < len(allrowids):
+		for i in range(len(allrowids)):
+			tv_table.set(allrowids[i], column=column_name, value='')
 	for i in range(len(data_strs)):
 		tv_table.set(item_ids[i], column=column_name, value=data_strs[i])
 
 
+
 def export_data_table(headers, rows, sheetname="mapdata_export"):
 	# Exports the selected data to a CSV or ODS file.  Returns the file name or None if canceled.
 	outfile = tkfiledialog.asksaveasfilename(title="File name for saved data rows",
 		filetypes=[('CSV files', '.csv'), ('ODS files', '.ods'), ('TSV files', '.tsv'), ('Plain text', '.txt'), ('LaTeX', '.tex')])
 	if outfile:
 		if outfile[-3:].lower() == 'csv':
 			write_delimited_file(outfile, "csv", headers, rows)
@@ -2695,23 +2721,27 @@
 		res = [[] for _ in column_list]
 		indices = [self.headers.index(c) for c in column_list]
 		for sel_row in self.tbl.get_children():
 			datarow = self.tbl.item(sel_row)["values"]
 			for i, index in enumerate(indices):
 				res[i].append(datarow[index])
 		return res
+	def get_all_rowids(self):
+		return self.tbl.get_children()
 	def get_sel_data(self, column_list):
 		# Plotting and statistics support.  Return data from selected rows for the specified columns, as a list of lists.
 		res = [[] for _ in column_list]
 		indices = [self.headers.index(c) for c in column_list]
 		for sel_row in self.tbl.selection():
 			datarow = self.tbl.item(sel_row)["values"]
 			for i, index in enumerate(indices):
 				res[i].append(datarow[index])
 		return res
+	def get_sel_rowids(self):
+		return self.tbl.selection()
 	def update_plot_data(self, unconditional=False):
 		# Pushes updates to all plots and other dialogs that may use only selected data.
 		# The 'push' is done by calling each dialog's refresh method.
 		for dlg in self.candcol_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc(get_data=True)
 		for plot in self.plot_list:
@@ -2726,15 +2756,15 @@
 		for dlg in self.fitdist_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
 		for dlg in self.tsne_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
 		for dlg in self.umap_list:
-			if unconditional or dlg.sel_only_var.get() == "1":
+			if unconditional or (dlg.sel_only_var.get() == "1" and dlg.auto_update):
 				dlg.q_recalc()
 		for dlg in self.corrmat_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_redraw()
 		for dlg in self.catcorresp_list:
 			if unconditional or dlg.sel_only_var.get() == "1":
 				dlg.q_recalc()
@@ -3428,31 +3458,42 @@
 		def corr_matrix():
 			self.wait_for_data_types()
 			dlg = CorrMatrixDialog(self, self.data_types)
 			self.corrmat_list.append(dlg)
 			dlg.show()
 
 		def tsne_anal():
+			bad_cols = [self.lat_col, self.lon_col]
+			if self.src_lat_col is not None:
+				bad_cols.extend([self.src_lat_col, self.src_lon_col])
+			if self.lat_4326_col is not None:
+				bad_cols.extend([self.lat_4326_col, self.lon_4326_col])
+			self.loading_dlg.hide()
 			self.wait_for_data_types()
-			dlg = TSNEDialog(self, self.data_types)
+			dlg = TSNEDialog(self, self.data_types, bad_cols)
 			self.tsne_list.append(dlg)
 			dlg.show()
 
 		def umap_anal():
 			self.loading_dlg.display("Initializing UMAP")
 			try:
 				import umap
 				from sklearn.preprocessing import StandardScaler
 			except:
 				self.loading_dlg.hide()
 				warning("Libraries required for UMAP analysis are missing.", {'parent': self.win})
 			else:
+				bad_cols = [self.lat_col, self.lon_col]
+				if self.src_lat_col is not None:
+					bad_cols.extend([self.src_lat_col, self.src_lon_col])
+				if self.lat_4326_col is not None:
+					bad_cols.extend([self.lat_4326_col, self.lon_4326_col])
 				self.loading_dlg.hide()
 				self.wait_for_data_types()
-				dlg = UMAPDialog(self, self.data_types)
+				dlg = UMAPDialog(self, self.data_types, bad_cols)
 				self.umap_list.append(dlg)
 				dlg.show()
 
 		def categ_corresp():
 			self.wait_for_data_types()
 			dlg = CategCorrespDialog(self, self.data_types)
 			self.catcorresp_list.append(dlg)
@@ -3532,15 +3573,15 @@
 		stats_menu.add_command(label="Univariate statistics", command = univar_stats, underline=0)
 		stats_menu.add_command(label="Fit univariate distribution", command = fitdist_stats, underline=0)
 		stats_menu.add_command(label="Bivariate statistics", command = bivar_stats, underline=0)
 		stats_menu.add_command(label="Correlation matrix", command = corr_matrix, underline=0)
 		stats_menu.add_command(label="Contingency table", command = cont_table, underline=2)
 		stats_menu.add_command(label="ROC curve", command = roc_curve, underline=0)
 		stats_menu.add_command(label="t-SNE analysis", command = tsne_anal, underline=0)
-		stats_menu.add_command(label="UMAP analysis", command = umap_anal, underline=0)
+		stats_menu.add_command(label="UMAP analysis", command = umap_anal, underline=1)
 		stats_menu.add_command(label="Categorical corresp.", command = categ_corresp, underline=1)
 		help_menu.add_command(label="Online help", command = online_help, underline=7)
 		help_menu.add_command(label="Config files", command = show_config_files, underline=0)
 		help_menu.add_command(label="Hotkeys", command = show_hotkeys, underline=0)
 		help_menu.add_command(label="About", command = show_about, underline=0)
 
 
@@ -5768,16 +5809,16 @@
 					ds = list(zip(self.dataset[1], self.dataset[0]))
 					plot_data = []
 					for g in grp_vals:
 						plot_data.append([d[1] for d in ds if d[0] == g])
 					self.plot_data = plot_data
 					self.plot_data_labels = grp_vals
 				else:
-					self.plot_data = self.dataset
-					self.plot_data_labels = self.data_labels
+					self.plot_data = [self.dataset[0]]
+					self.plot_data_labels = [self.data_labels[0]]
 			elif plot_type == "Breaks groups":
 				x_vals = copy.copy(self.dataset[0])
 				x_vals.sort()
 				oj = optimum_jenks(x_vals, 8)
 				jnb = jenkspy.JenksNaturalBreaks(oj)
 				jnb.fit(x_vals)
 				self.plot_data = [list(x) for x in jnb.groups_]
@@ -6317,15 +6358,14 @@
 				else:
 					self.plot_axes.set_ylabel(self.ylabel or self.y_var.get())
 				if self.flip_y:
 					self.plot_axes.invert_yaxis()
 			elif plot_type == "Box plot":
 				self.dlg.bind("<Alt-r>", self.set_rotated)
 				orient = not self.rotated
-				breakpoint()
 				grplbls = copy.copy(self.plot_data_labels)
 				if wrap_at_underscores:
 					grplbls = [lbl.replace("_", " ") for lbl in grplbls]
 				grplbls = [textwrap.wrap(lbl, width=wrapwidth) for lbl in grplbls]
 				grplbls = ["\n".join(lbl) for lbl in grplbls]
 				self.plot_axes.boxplot(self.plot_data, labels=grplbls, vert=orient)
 				if not self.rotated:
@@ -7478,14 +7518,19 @@
 						kendalltau = spstats.kendalltau(np.array(self.dataset[0]), np.array(self.dataset[1]))
 						self.statdata.append(["Kendall's tau", fp_display(kendalltau.statistic)])
 						ktau = kendalltau.pvalue
 						ktau = fp_display(ktau, 3)
 						self.statdata.append(["p value for Kendall's tau", ktau])
 					except:
 						pass
+					try:
+						xi = xicor(np.array(self.dataset[0]), np.array(self.dataset[1]))
+						self.statdata.append(["Chatterjee's xi", fp_display(xi)])
+					except:
+						pass
 					# Linear regression
 					ols_model = sm.OLS(np.array(self.dataset[1]), sm.add_constant(np.array(self.dataset[0])))
 					ols_fit = ols_model.fit()
 					slope = ols_fit.params[1]
 					regr_run = True
 					self.statdata.append(["OLS Regression slope", fp_display(slope)])
 					self.statdata.append(["OLS Regression intercept", fp_display(ols_fit.params[0])])
@@ -7674,14 +7719,20 @@
 		var_frame.columnconfigure(0, weight=1)
 		frame_panes.add(var_frame, weight=1)
 		# Add multi-select list of variables to the leftmost pane
 		self.column_frame, self.column_table = treeview_table(var_frame, rowset=[[v] for v in self.numeric_columns], \
 				column_headers=['Variable'], select_mode=tk.EXTENDED, nrows=min(10, len(self.numeric_columns)))
 		self.column_frame.grid(row=0, column=0, sticky=tk.NSEW)
 		self.column_table.bind('<ButtonRelease-1>', self.q_redraw)
+		self.corr_type_var = tk.StringVar(var_frame, "Pearson r")
+		ttk.Label(var_frame, text="Correlation type:").grid(row=1, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+		corr_type_sel = ttk.Combobox(var_frame, state="readonly", textvariable=self.corr_type_var, width=24)
+		corr_type_sel["values"] = ["Pearson r", "Spearman rho", "Kendall tau", "Chatterjee xi"]
+		corr_type_sel.grid(row=2, column=0, sticky=tk.E, padx=(6,3), pady=(3,3))
+		corr_type_sel.bind('<<ComboboxSelected>>', self.q_redraw)
 
 		# Content frame for correlation matrix figure
 		self.content_frame = tk.Frame(frame_panes, borderwidth=3, relief=tk.RIDGE)
 		self.content_frame.grid(row=0, column=1, sticky=tk.NSEW)
 		self.content_frame.rowconfigure(0, weight=1)
 		self.content_frame.columnconfigure(0, weight=1)
 		frame_panes.add(self.content_frame, weight=12)
@@ -7794,46 +7845,65 @@
 					clean_data = log_data
 					clean_labels = ["Log10 of " + v for v in clean_labels]
 			#
 			self.dataset = clean_data
 			self.data_labels = clean_labels
 			self.data_btn["state"] = tk.NORMAL
 
+
 	def redraw(self):
 		# (Re)draw the correlation matrix
 		if self.data_labels is not None and len(self.data_labels) > 1:
 			nvar = len(self.data_labels)
+			corrmat = np.eye(nvar)
+			corrtype = self.corr_type_var.get()
+			if corrtype == "Pearson r":
+				corrfn = pearsonstat
+			elif corrtype == "Spearman rho":
+				corrfn = spearmanstat
+			elif corrtype == "Kendall tau":
+				corrfn = kendallstat
+			else:
+				corrfn = xicor
 			dmat = np.asarray(self.dataset)
-			cormat = np.corrcoef(dmat)
-			#caxes = self.plot_axes.matshow(cormat, cmap="PiYG", vmin=-1.0, vmax=1.0)
-			caxes = self.plot_axes.matshow(cormat, cmap="BrBG", vmin=-1.0, vmax=1.0)
+			for i in range(nvar):
+				for j in range(i, nvar):
+					if i != j:
+						corrcoeff = corrfn(dmat[i], dmat[j])
+						corrmat[i][j] = corrcoeff
+						corrmat[j][i] = corrcoeff
+			caxes = self.plot_axes.matshow(corrmat, cmap="BrBG", vmin=-1.0, vmax=1.0)
 			self.plotfig.colorbar(caxes)
 			self.plot_axes.set_xticks(range(nvar), labels=self.data_labels, rotation=25)
 			self.plot_axes.set_yticks(range(nvar), labels=self.data_labels)
 			for i in range(nvar):
 				for j in range(nvar):
-					v = cormat[i,j]
+					v = corrmat[i,j]
 					c = "white" if abs(v) > 0.40 else "black"
-					self.plot_axes.text(j, i, f"{cormat[i,j]:.2f}", ha="center", va="center", color=c)
+					self.plot_axes.text(j, i, f"{corrmat[i,j]:.2f}", ha="center", va="center", color=c)
+			self.plot_axes.set_title(corrtype)
 			self.plotfig_canvas.draw()
 
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
 		self.parent.remove_corrmat(self)
 		try:
 			self.dlg.destroy()
 		except:
 			pass
 
 
 class TSNEDialog(object):
-	def __init__(self, parent, column_specs):
+	def __init__(self, parent, column_specs, prohibited_columns):
 		self.parent = parent
 		self.column_specs = column_specs
+		self.prohibited_columns = prohibited_columns
+		self.string_columns = [c[0] for c in self.column_specs if c[1] == "string" and not (c[1] in prohibited_columns)]
+		self.auto_update = True
 		self.alpha = 0.45
 		self.plot_title = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("t-SNE Analysis")
 		self.loading_dlg = LoadingDialog(self.dlg)
 		self.alpha = 0.45
 		self.tsne_coords = None
@@ -7858,15 +7928,20 @@
 		# Controls
 		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_recalc, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
-		self.sel_only_ck.grid(row=0, column=0, columnspan=2, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
+		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
+				onvalue="1", offvalue="0")
+		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
@@ -7934,19 +8009,27 @@
 		self.plotfig.set_figwidth(3.5)
 		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, plot_frame)
 		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, plot_frame)
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
 		self.plot_nav.update()
 
-		# t-SNE Data Table button
+		# t-SNE Data Table button frame
 		dtbtn_frame = tk.Frame(self.output_frame)
 		dtbtn_frame.pack(side=tk.BOTTOM, fill=tk.X, expand=0)
 		self.dtable_btn = ttk.Button(dtbtn_frame, text="Data Table", command=self.tsne_table, state=tk.DISABLED, underline=8)
-		self.dtable_btn.pack(side=tk.LEFT, fill='none', expand=0, padx=(6,3), pady=(3,3))
+		self.dtable_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(21,3))
+
+		# k-Means clustering options
+		kmeans_lf = tk.LabelFrame(dtbtn_frame, text="k-Means clusters")
+		kmeans_lf.grid(row=0, column=1, padx=(3,3), pady=(3,3))
+		self.cluster_btn = ttk.Button(kmeans_lf, text="Create", command=self.kclusters, state=tk.DISABLED)
+		self.cluster_btn.grid(row=0, column=0, sticky=tk.W, padx=(3,3), pady=(2,2))
+		self.clust_save_btn = ttk.Button(kmeans_lf, text="Add Column", command=self.kcolumn, state=tk.DISABLED)
+		self.clust_save_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(2,2))
 
 		# Buttons
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=0)
 		btn_frame.columnconfigure(1, weight=0)
@@ -7965,24 +8048,30 @@
 		# Initialize output frames
 		self.clear_output()
 
 		center_window(self.dlg)
 		raise_window(self.dlg)
 
 	def do_help(self, *args):
-		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#t-sne-dialog", new=2, autoraise=True)
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#t-sne-analysis-dialog", new=2, autoraise=True)
+
+	def set_autoupdate(self):
+		if self.autoupdate_var.get() == "1":
+			self.auto_update = True
+		else:
+			self.auto_update = False
 
 	def q_recalc(self, *args):
 		# At least three variables must be selected
 		self.clear_output()
 		curr_selections = self.column_table.selection()
 		if len(curr_selections) > 2:
 			self.calc_btn["state"] = tk.NORMAL
 		else:
-			self.calc_btn["state"] = tk.NORMAL
+			self.calc_btn["state"] = tk.DISABLED
 
 	def get_data(self):
 		self.data_btn["state"] = tk.DISABLED
 		self.dataset = None
 		column_list = []
 		for sel_row in self.column_table.selection():
 			datarow = self.column_table.item(sel_row)["values"]
@@ -7997,36 +8086,42 @@
 			self.label_col = None
 		grpbyvar = self.groupby_var.get()
 		if grpbyvar != '':
 			column_list.append(grpbyvar)
 			self.groupby_col = len(column_list)
 		else:
 			self.groupby_col = None
-		# Get either only the selected data or all data.
+		# Get either only the selected data or all data.  Get row IDs in case k-means clustering results
+		# are to be assigned to a column.
 		if self.sel_only_var.get() == "1":
 			dataset = self.parent.get_sel_data(column_list)
+			self.data_rowids = self.parent.get_sel_rowids()
 		else:
 			dataset = self.parent.get_all_data(column_list)
+			self.data_rowids = self.parent.get_all_rowids()
 		if dataset is None or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 		else:
 			# Remove missing data
 			column_indexes = range(len(dataset))
 			clean_data = [[] for _ in dataset]
+			clean_rowids = []
 			for i in range(len(dataset[0])):
 				ok = True
 				for col in column_indexes:
 					if dataset[col][i] is None or dataset[col][i] == '':
 						ok = False
 				if ok:
 					for col in column_indexes:
 						clean_data[col].append(dataset[col][i])
+					clean_rowids.append(self.data_rowids[i])
+			self.data_rowids = clean_rowids
 			dataset = None
 			# Convert to floats for numeric data only
 			for i in range(len(clean_data)):
 				if column_list[i] in self.numeric_columns:
 					clean_data[i] = [conv_float(v) for v in clean_data[i]]
 			#
 			self.dataset = sort_columns(clean_data)
@@ -8046,46 +8141,43 @@
 		self.plotfig_canvas.draw()
 
 	def recalculate(self):
 		self.loading_dlg.display("Calculating t-SNE")
 		self.clear_output()
 		from sklearn.manifold import TSNE
 		self.get_data()
-		#if self.calc_btn["state"] == tk.NORMAL:
 		d = np.array(columns_to_rows(self.dataset[0:self.n_dataset_columns]))
 		perp = self.perp_var.get()
 		if perp > len(self.dataset[0]) - 1:
 			perp = min(50, math.floor(len(self.dataset[0])/2))
 			self.perp_var.set(perp)
 		tsne = TSNE(n_components=2, perplexity=perp)
 		tsne_result = tsne.fit_transform(d)
 		self.tsne_coords = [tsne_result[:,0], tsne_result[:,1]]
 		self.tsne_labels = ["Dimension 1", "Dimension 2"]
 		self.dtable_btn["state"] = tk.NORMAL
-		#self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
 		# Single or grouped scatter plot
 		if self.groupby_col is None:
 			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], alpha=self.alpha)
-			handle_list = []
-			label_list = []
+			self.plot_handle_list = []
+			self.plot_label_list = []
 		else:
 			groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
 			cmap = map_colors(groups)
 			colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
 			splot = self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], c=colors, alpha=self.alpha)
 			# Custom legend handle for grouped scatter plot
 			lbls = list(cmap.keys())
 			if wrap_at_underscores:
 				lbls = [l.replace("_", " ") for l in lbls]
 			lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
 			colkey = list(cmap.values())
 			symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
-			handle_list = symbs
-			label_list = lbls
-		#bbox = self.plot_axes.get_clip_box()
+			self.plot_handle_list = symbs
+			self.plot_label_list = lbls
 		# Hover annotation
 		def update_annot(ind):
 			pos = splot.get_offsets()[ind["ind"][0]]
 			self.annot.xy = pos
 			text = ", ".join([str(self.dataset[self.label_col-1][n]) for n in ind["ind"]])
 			self.annot.set_text(text)
 			self.annot.get_bbox_patch().set_facecolor("wheat")
@@ -8106,24 +8198,113 @@
 					bbox={"boxstyle": "round", "fc": "w"}, arrowprops={"arrowstyle": "->"})
 			self.annot.set_visible(False)
 			self.canvas_conn_id = self.plotfig_canvas.mpl_connect("motion_notify_event", hover)
 		else:
 			if self.canvas_conn_id is not None:
 				self.plotfig_canvas.mpl_disconnect(self.canvas_conn_id)
 		# Legend
-		if len(handle_list) > 0:
-			self.plot_axes.legend(handles=handle_list, labels=label_list)
+		if len(self.plot_handle_list) > 0:
+			self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
 
 		self.plot_axes.set_xlabel(self.tsne_labels[0])
 		self.plot_axes.set_ylabel(self.tsne_labels[1])
 		self.plotfig_canvas.draw()
 		self.plot_nav.update()
 		self.dlg.bind("<Alt-a>", self.set_alpha)
+		self.cluster_btn["state"] = tk.NORMAL
+		self.clust_save_btn["state"] = tk.DISABLED
 		self.loading_dlg.hide()
 
+	def kclusters(self):
+		# Compute and display k-means clusters
+		dlg = OneIntDialog(self.dlg, "k-Means Clusters", "Enter the number of clusters to identify", min_value=2, max_value=min(30, len(self.dataset[0])-1), initial=2)
+		num_clusters = dlg.show()
+		self.loading_dlg.display("Clustering t-SNE output")
+		from sklearn.cluster import KMeans
+		km = KMeans(n_clusters=num_clusters)
+		km.fit(np.array(columns_to_rows([self.tsne_coords[0], self.tsne_coords[1]])))
+		self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
+		self.tsne_coords.append(self.kmlabels)
+		self.tsne_labels.append("k-Means cluster")
+		kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
+		kcmap = map_colors(kgroups)
+		kcolors = [kcmap[str(g)] for g in self.kmlabels]
+		self.plot_axes.scatter(self.tsne_coords[0], self.tsne_coords[1], marker="v", s=15, c=kcolors)
+		klbls = [str(k) for k in kcmap.keys()]
+		kcolkey = list(kcmap.values())
+		ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
+		self.plot_handle_list.extend(ksymbs)
+		self.plot_label_list.extend(klbls)
+		try:
+			self.plot_axes.get_legend().remove()
+		except:
+			pass
+		self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
+		self.plotfig_canvas.draw()
+		# Only allow creation of one set of clusters for each UMAP output.
+		self.cluster_btn["state"] = tk.DISABLED
+		self.clust_save_btn["state"] = tk.NORMAL
+		self.loading_dlg.hide()
+
+	def kcolumn(self):
+		# Save k-means cluster output as a data table column.
+		# Column selection
+		dlg = CustomContentDialog(parent=self.dlg, title="Save Clusters", prompt="Save k-means clusters in a table column.")
+		def ck_col_name(varname, ix, mode):
+			if self.col_var.get() in self.prohibited_columns:
+				self.col_var.set('')
+				dlg.ok_btn["state"] = tk.DISABLED
+			else:
+				if self.col_var.get() == '':
+					dlg.ok_btn["state"] = tk.DISABLED
+				else:
+					dlg.ok_btn["state"] = tk.NORMAL
+		self.col_var = tk.StringVar(dlg.content_frame, "")
+		self.col_var.trace_add("write", ck_col_name)
+		col_lbl = ttk.Label(dlg.content_frame, justify=tk.RIGHT, text="New or existing column name:")
+		col_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,6))
+		self.col_sel = ttk.Combobox(dlg.content_frame, state=tk.NORMAL, textvariable=self.col_var, values=self.string_columns, width=24)
+		self.col_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,6))
+		self.col_sel.focus()
+		ok = dlg.show()
+		if ok:
+			self.loading_dlg.display("Saving clusters")
+			target_col = self.col_var.get()
+			db_col_name = db_colnames([target_col])[0]
+			# Update the database
+			new_column = target_col not in self.parent.headers
+			cur = data_db.cursor()
+			if new_column:
+				cur.execute(f"alter table mapdata add column {db_col_name} TEXT;")
+			for i in range(len(self.kmlabels)):
+				cur.execute(f"update mapdata set {db_col_name} = '{self.kmlabels[i]}' where treeviewid = '{self.data_rowids[i]}';")
+			# Update the Treeview
+			if new_column:
+				add_tv_column(self.parent.tbl, target_col, self.data_rowids, self.kmlabels)
+			else:
+				for rowid in self.parent.tbl.get_children():
+					if rowid in self.data_rowids:
+						clust_index = self.data_rowids.index(rowid)
+						self.parent.tbl.set(rowid, column=target_col, value=self.kmlabels[clust_index])
+					else:
+						self.parent.tbl.set(rowid, column=target_col, value='')
+			# Update the header names and table specs
+			self.parent.headers = self.parent.headers + [target_col]
+			dt = "string"
+			coldata = self.parent.get_all_data([target_col])[0]
+			missing = len([v for v in coldata if v is None or v == ''])
+			unique = len(set([v for v in coldata if v is not None and v != '']))
+			if new_column:
+				self.parent.data_types.append([target_col, dt, missing, unique])
+				self.string_columns.append(target_col)
+			else:
+				col_ix = self.parent.headers.index(target_col)
+				self.parent.data_types[col_ix] = [target_col, dt, missing, unique]
+			self.loading_dlg.hide()
+
 	def show_data(self, *args):
 		if self.dataset is not None:
 			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels, "Data for t-SNE Analysis")
 
 	def tsne_table(self, *args):
 		if self.tsne_coords is not None:
 			dt = copy.copy(self.tsne_coords)
@@ -8151,25 +8332,28 @@
 			self.dlg.destroy()
 		except:
 			pass
 
 
 
 class UMAPDialog(object):
-	def __init__(self, parent, column_specs):
+	def __init__(self, parent, column_specs, prohibited_columns):
 		self.parent = parent
 		self.column_specs = column_specs
+		self.prohibited_columns = prohibited_columns
+		self.string_columns = [c[0] for c in self.column_specs if c[1] == "string" and not (c[1] in prohibited_columns)]
+		self.auto_update = True
 		self.alpha = 0.45
 		self.plot_title = None
 		self.dlg = tk.Toplevel()
 		self.dlg.title("UMAP Analysis")
 		self.loading_dlg = LoadingDialog(self.dlg)
 		self.alpha = 0.45
-		self.tsne_coords = None
-		self.tsne_labels = None
+		self.umap_coords = None
+		self.umap_labels = None
 		# Data
 		self.dataset = None
 		self.data_labels = None
 		self.numeric_columns = [c[0] for c in self.column_specs if c[1] in ("int", "float")]
 		self.numeric_columns.sort()
 		self.categ_columns = [c[0] for c in self.column_specs if c[1] == "string"]
 		self.categ_columns.sort()
@@ -8186,15 +8370,20 @@
 		# Controls
 		ctrl_frame = tk.Frame(self.dlg, borderwidth=5)
 		ctrl_frame.grid(row=1, column=0, sticky=tk.N+tk.EW)
 
 		self.sel_only_var = tk.StringVar(ctrl_frame, "0")
 		self.sel_only_ck = ttk.Checkbutton(ctrl_frame, text="Selected data only", command=self.q_recalc, variable=self.sel_only_var,
 				onvalue="1", offvalue="0")
-		self.sel_only_ck.grid(row=0, column=0, columnspan=2, sticky=tk.W, padx=(6,3), pady=(3,3))
+		self.sel_only_ck.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(3,3))
+
+		self.autoupdate_var = tk.StringVar(ctrl_frame, "1")
+		self.autoupdate_ck = ttk.Checkbutton(ctrl_frame, text="Auto-update", command=self.set_autoupdate, variable=self.autoupdate_var,
+				onvalue="1", offvalue="0")
+		self.autoupdate_ck.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,3))
 
 		# Frame for input selection and output plot
 		self.content_frame = tk.Frame(self.dlg)
 		self.content_frame.grid(row=2, column=0, sticky=tk.NSEW)
 		self.dlg.rowconfigure(2, weight=1)
 		self.dlg.columnconfigure(0, weight=1)
 		self.content_frame.rowconfigure(0, weight=1)
@@ -8269,19 +8458,27 @@
 		self.plotfig.set_figwidth(3.5)
 		self.plotfig_canvas = FigureCanvasTkAgg(self.plotfig, plot_frame)
 		self.plot_nav = NavigationToolbar2Tk(self.plotfig_canvas, plot_frame)
 		self.plot_axes = self.plotfig.add_subplot(111)
 		self.plotfig_canvas.get_tk_widget().pack(side=tk.TOP, fill=tk.BOTH, expand=1)
 		self.plot_nav.update()
 
-		# t-SNE Data Table button
+		# t-SNE Data Table button frame
 		dtbtn_frame = tk.Frame(self.output_frame)
 		dtbtn_frame.pack(side=tk.BOTTOM, fill=tk.X, expand=0)
 		self.dtable_btn = ttk.Button(dtbtn_frame, text="Data Table", command=self.umap_table, state=tk.DISABLED, underline=8)
-		self.dtable_btn.pack(side=tk.LEFT, fill='none', expand=0, padx=(6,3), pady=(3,3))
+		self.dtable_btn.grid(row=0, column=0, sticky=tk.W, padx=(6,3), pady=(21,3))
+
+		# k-Means clustering options
+		kmeans_lf = tk.LabelFrame(dtbtn_frame, text="k-Means clusters")
+		kmeans_lf.grid(row=0, column=1, padx=(3,3), pady=(3,3))
+		self.cluster_btn = ttk.Button(kmeans_lf, text="Create", command=self.kclusters, state=tk.DISABLED)
+		self.cluster_btn.grid(row=0, column=0, sticky=tk.W, padx=(3,3), pady=(2,2))
+		self.clust_save_btn = ttk.Button(kmeans_lf, text="Add Column", command=self.kcolumn, state=tk.DISABLED)
+		self.clust_save_btn.grid(row=0, column=1, sticky=tk.W, padx=(3,6), pady=(2,2))
 
 		# Buttons
 		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
 		btn_frame.columnconfigure(0, weight=1)
 		btn_frame.grid(row=3, column=0, sticky=tk.EW, pady=(3,3))
 		btn_frame.columnconfigure(0, weight=0)
 		btn_frame.columnconfigure(1, weight=0)
@@ -8300,24 +8497,30 @@
 		# Initialize output frames
 		self.clear_output()
 
 		center_window(self.dlg)
 		raise_window(self.dlg)
 
 	def do_help(self, *args):
-		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#umap-dialog", new=2, autoraise=True)
+		webbrowser.open("https://mapdata.readthedocs.io/en/latest/dialogs.html#umap-analysis-dialog", new=2, autoraise=True)
+
+	def set_autoupdate(self):
+		if self.autoupdate_var.get() == "1":
+			self.auto_update = True
+		else:
+			self.auto_update = False
 
 	def q_recalc(self, *args):
 		# At least three variables must be selected
 		self.clear_output()
 		curr_selections = self.column_table.selection()
 		if len(curr_selections) > 2:
 			self.calc_btn["state"] = tk.NORMAL
 		else:
-			self.calc_btn["state"] = tk.NORMAL
+			self.calc_btn["state"] = tk.DISABLED
 
 	def get_data(self):
 		self.data_btn["state"] = tk.DISABLED
 		self.dataset = None
 		column_list = []
 		for sel_row in self.column_table.selection():
 			datarow = self.column_table.item(sel_row)["values"]
@@ -8332,19 +8535,22 @@
 			self.label_col = None
 		grpbyvar = self.groupby_var.get()
 		if grpbyvar != '':
 			column_list.append(grpbyvar)
 			self.groupby_col = len(column_list)
 		else:
 			self.groupby_col = None
-		# Get either only the selected data or all data.
+		# Get either only the selected data or all data.  Get row IDs in case k-means clustering results
+		# are to be assigned to a column.
 		if self.sel_only_var.get() == "1":
 			dataset = self.parent.get_sel_data(column_list)
+			self.data_rowids = self.parent.get_sel_rowids()
 		else:
 			dataset = self.parent.get_all_data(column_list)
+			self.data_rowids = self.parent.get_all_rowids()
 		if dataset is None or len(dataset[0]) < 6:
 			self.dataset = None
 			self.data_labels = None
 			self.data_btn["state"] = tk.DISABLED
 			self.calc_btn["state"] = tk.DISABLED
 		else:
 			# UMAP can operate on sparse arrays, so there's no need to remove missing data
@@ -8392,39 +8598,39 @@
 			# Convert to a LIL array
 			dsm = sparse.lil_matrix(dsa)
 			# Normalize the variables
 			inp_data = StandardScaler(with_mean=False).fit_transform(dsm)
 		else:
 			# Normalize the variables
 			inp_data = StandardScaler().fit_transform(dsa)
-		reducer = umap.UMAP(n_neighbors=self.neighbors_var.get(), min_dist=self.mindist_var.get(), n_components=2,
+		reducer = umap.UMAP(n_neighbors=min(self.neighbors_var.get(), len(self.dataset[0])-1), min_dist=self.mindist_var.get(), n_components=2,
 				metric=self.metric_var.get())
 		umap_result = reducer.fit_transform(inp_data)
 		self.umap_coords = [umap_result[:,0], umap_result[:,1]]
 		self.umap_labels = ["Dimension 1", "Dimension 2"]
 		self.dtable_btn["state"] = tk.NORMAL
 		# Single or grouped scatter plot
 		if self.groupby_col is None:
 			splot = self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], alpha=self.alpha)
-			handle_list = []
-			label_list = []
+			self.plot_handle_list = []
+			self.plot_label_list = []
 		else:
 			groups = sorted([str(x) for x in list(set(self.dataset[self.groupby_col-1]))])
 			cmap = map_colors(groups)
 			colors = [cmap[str(g)] for g in self.dataset[self.groupby_col-1]]
 			splot = self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], c=colors, alpha=self.alpha)
 			# Custom legend handle for grouped scatter plot
 			lbls = list(cmap.keys())
 			if wrap_at_underscores:
 				lbls = [l.replace("_", " ") for l in lbls]
 			lbls = ["\n".join(textwrap.wrap(l, width=wrapwidth)) for l in lbls]
 			colkey = list(cmap.values())
 			symbs = [matplotlib.lines.Line2D([], [], marker='o', color=colkey[i], label=lbls[i], linestyle='None') for i in range(len(lbls))]
-			handle_list = symbs
-			label_list = lbls
+			self.plot_handle_list = symbs
+			self.plot_label_list = lbls
 		# Hover annotation
 		def update_annot(ind):
 			pos = splot.get_offsets()[ind["ind"][0]]
 			self.annot.xy = pos
 			text = ", ".join([str(self.dataset[self.label_col-1][n]) for n in ind["ind"]])
 			self.annot.set_text(text)
 			self.annot.get_bbox_patch().set_facecolor("wheat")
@@ -8445,24 +8651,113 @@
 					bbox={"boxstyle": "round", "fc": "w"}, arrowprops={"arrowstyle": "->"})
 			self.annot.set_visible(False)
 			self.canvas_conn_id = self.plotfig_canvas.mpl_connect("motion_notify_event", hover)
 		else:
 			if self.canvas_conn_id is not None:
 				self.plotfig_canvas.mpl_disconnect(self.canvas_conn_id)
 		# Legend
-		if len(handle_list) > 0:
-			self.plot_axes.legend(handles=handle_list, labels=label_list)
+		if len(self.plot_handle_list) > 0:
+			self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
 
 		self.plot_axes.set_xlabel(self.umap_labels[0])
 		self.plot_axes.set_ylabel(self.umap_labels[1])
 		self.plotfig_canvas.draw()
 		self.plot_nav.update()
 		self.dlg.bind("<Alt-a>", self.set_alpha)
+		self.cluster_btn["state"] = tk.NORMAL
+		self.clust_save_btn["state"] = tk.DISABLED
 		self.loading_dlg.hide()
 
+	def kclusters(self):
+		# Compute and display k-means clusters
+		dlg = OneIntDialog(self.dlg, "k-Means Clusters", "Enter the number of clusters to identify", min_value=2, max_value=min(30, len(self.dataset[0])-1), initial=2)
+		num_clusters = dlg.show()
+		self.loading_dlg.display("Clustering UMAP output")
+		from sklearn.cluster import KMeans
+		km = KMeans(n_clusters=num_clusters)
+		km.fit(np.array(columns_to_rows([self.umap_coords[0], self.umap_coords[1]])))
+		self.kmlabels = ["Cluster "+str(int(lbl)+1) for lbl in km.labels_]
+		self.umap_coords.append(self.kmlabels)
+		self.umap_labels.append("k-Means cluster")
+		kgroups = sorted([str(x) for x in list(set(self.kmlabels))])
+		kcmap = map_colors(kgroups)
+		kcolors = [kcmap[str(g)] for g in self.kmlabels]
+		self.plot_axes.scatter(self.umap_coords[0], self.umap_coords[1], marker="v", s=15, c=kcolors)
+		klbls = [str(k) for k in kcmap.keys()]
+		kcolkey = list(kcmap.values())
+		ksymbs = [matplotlib.lines.Line2D([], [], marker='v', color=kcolkey[i], label=klbls[i], linestyle='None') for i in range(len(klbls))]
+		self.plot_handle_list.extend(ksymbs)
+		self.plot_label_list.extend(klbls)
+		try:
+			self.plot_axes.get_legend().remove()
+		except:
+			pass
+		self.plot_axes.legend(handles=self.plot_handle_list, labels=self.plot_label_list)
+		self.plotfig_canvas.draw()
+		# Only allow creation of one set of clusters for each UMAP output.
+		self.cluster_btn["state"] = tk.DISABLED
+		self.clust_save_btn["state"] = tk.NORMAL
+		self.loading_dlg.hide()
+
+	def kcolumn(self):
+		# Save k-means cluster output as a data table column.
+		# Column selection
+		dlg = CustomContentDialog(parent=self.dlg, title="Save Clusters", prompt="Save k-means clusters in a table column.")
+		def ck_col_name(varname, ix, mode):
+			if self.col_var.get() in self.prohibited_columns:
+				self.col_var.set('')
+				dlg.ok_btn["state"] = tk.DISABLED
+			else:
+				if self.col_var.get() == '':
+					dlg.ok_btn["state"] = tk.DISABLED
+				else:
+					dlg.ok_btn["state"] = tk.NORMAL
+		self.col_var = tk.StringVar(dlg.content_frame, "")
+		self.col_var.trace_add("write", ck_col_name)
+		col_lbl = ttk.Label(dlg.content_frame, justify=tk.RIGHT, text="New or existing column name:")
+		col_lbl.grid(row=0, column=0, sticky=tk.E, padx=(6,3), pady=(3,6))
+		self.col_sel = ttk.Combobox(dlg.content_frame, state=tk.NORMAL, textvariable=self.col_var, values=self.string_columns, width=24)
+		self.col_sel.grid(row=0, column=1, sticky=tk.W, padx=(3,3), pady=(3,6))
+		self.col_sel.focus()
+		ok = dlg.show()
+		if ok:
+			self.loading_dlg.display("Saving clusters")
+			target_col = self.col_var.get()
+			db_col_name = db_colnames([target_col])[0]
+			# Update the database
+			new_column = target_col not in self.parent.headers
+			cur = data_db.cursor()
+			if new_column:
+				cur.execute(f"alter table mapdata add column {db_col_name} TEXT;")
+			for i in range(len(self.data_rowids)):
+				cur.execute(f"update mapdata set {db_col_name} = '{self.kmlabels[i]}' where treeviewid = '{self.data_rowids[i]}';")
+			# Update the Treeview
+			if new_column:
+				add_tv_column(self.parent.tbl, target_col, self.data_rowids, self.kmlabels)
+			else:
+				for rowid in self.parent.tbl.get_children():
+					if rowid in self.data_rowids:
+						clust_index = self.data_rowids.index(rowid)
+						self.parent.tbl.set(rowid, column=target_col, value=self.kmlabels[clust_index])
+					else:
+						self.parent.tbl.set(rowid, column=target_col, value='')
+			# Update the header names and table specs
+			self.parent.headers = self.parent.headers + [target_col]
+			dt = "string"
+			coldata = self.parent.get_all_data([target_col])[0]
+			missing = len([v for v in coldata if v is None or v == ''])
+			unique = len(set([v for v in coldata if v is not None and v != '']))
+			if new_column:
+				self.parent.data_types.append([target_col, dt, missing, unique])
+				self.string_columns.append(target_col)
+			else:
+				col_ix = self.parent.headers.index(target_col)
+				self.parent.data_types[col_ix] = [target_col, dt, missing, unique]
+			self.loading_dlg.hide()
+
 	def show_data(self, *args):
 		if self.dataset is not None:
 			show_columnar_table(self.dlg, "Source Data", "Selected data:", self.dataset, self.data_labels, "Data for UMAP Analysis")
 
 	def umap_table(self, *args):
 		if self.umap_coords is not None:
 			dt = copy.copy(self.umap_coords)
@@ -8481,15 +8776,15 @@
 		if new_alpha is not None:
 			self.alpha = new_alpha
 			self.q_recalc()
 
 	def show(self):
 		self.dlg.wait_window(self.dlg)
 	def do_close(self, *args):
-		self.parent.remove_tsne(self)
+		self.parent.remove_umap(self)
 		try:
 			self.dlg.destroy()
 		except:
 			pass
 
 
 
@@ -10088,14 +10383,61 @@
 	dlg.show(grab=grab)
 
 def show_columnar_table(parent, wintitle, msg, tabledata, tablehdrs, sheetname, grab=False, dlg_args={}, tv_args={}):
 	rowtable = columns_to_rows(tabledata)
 	show_table(parent, wintitle, msg, rowtable, tablehdrs, sheetname, grab, dlg_args, tv_args)
 
 
+class CustomContentDialog(object):
+	def __init__(self, parent, title, prompt):
+		self.dlg = tk.Toplevel(parent)
+		self.dlg.title(title)
+		self.canceled = False
+		prompt_frame = tk.Frame(self.dlg)
+		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
+		prompt_frame.columnconfigure(0, weight=1)
+		msg_lbl = ttk.Label(prompt_frame, text=prompt)
+		msg_lbl.grid(row=0, column=0, sticky=tk.W, padx=(6,6), pady=(6,6))
+		# Content frame, to be filled in by caller
+		self.content_frame = tk.Frame(self.dlg)
+		self.content_frame.grid(row=1, column=0, sticky=tk.NSEW)
+		self.dlg.rowconfigure(1, weight=1)
+		self.dlg.columnconfigure(0, weight=1)
+		# Buttons
+		btn_frame = tk.Frame(self.dlg, borderwidth=3, relief=tk.RIDGE)
+		btn_frame.columnconfigure(0, weight=1)
+		btn_frame.grid(row=2, column=0, sticky=tk.EW, pady=(3,3))
+		btn_frame.columnconfigure(0, weight=1)
+		self.canceled = False
+		self.ok_btn = ttk.Button(btn_frame, text="OK", command=self.do_select, underline=0)
+		self.ok_btn.grid(row=0, column=0, sticky=tk.E, padx=(6,3))
+		self.ok_btn["state"] = tk.DISABLED
+		self.dlg.bind('<Alt-o>', self.do_select)
+		cancel_btn = ttk.Button(btn_frame, text="Cancel", command=self.do_cancel, underline=0)
+		cancel_btn.grid(row=0, column=1, sticky=tk.E, padx=(3,6))
+		self.dlg.bind("<Escape>", self.do_cancel)
+		self.dlg.bind("<Alt-c>", self.do_cancel)
+		self.dlg.bind("<Return>", self.do_select)
+		self.dlg.bind("<Alt-o>", self.do_select)
+	def do_cancel(self, *args):
+		self.canceled = True
+		self.dlg.destroy()
+	def do_select(self, *args):
+		self.canceled = False
+		self.dlg.destroy()
+	def show(self):
+		self.dlg.grab_set()
+		center_window(self.dlg)
+		raise_window(self.dlg)
+		self.dlg.resizable(True, True)
+		self.dlg.attributes('-topmost', 'true')
+		self.dlg.wait_window(self.dlg)
+		return not self.canceled
+
+
 class OneEntryDialog(object):
 	def __init__(self, parent, title, prompt, obscure=False):
 		self.dlg = tk.Toplevel(parent)
 		self.dlg.title(title)
 		prompt_frame = tk.Frame(self.dlg)
 		prompt_frame.grid(row=0, column=0, sticky=tk.NSEW, pady=(3,3))
 		prompt_frame.columnconfigure(0, weight=1)
```

### Comparing `mapdata-3.5.0/mapdata/symbols/24x24/ball24.xbm` & `mapdata-3.6.0/mapdata/symbols/24x24/ball24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/24x24/block24.xbm` & `mapdata-3.6.0/mapdata/symbols/24x24/block24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/24x24/circle24.xbm` & `mapdata-3.6.0/mapdata/symbols/24x24/circle24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/24x24/square24.xbm` & `mapdata-3.6.0/mapdata/symbols/24x24/square24.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/28x28/ball28.xbm` & `mapdata-3.6.0/mapdata/symbols/28x28/ball28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/28x28/block28.xbm` & `mapdata-3.6.0/mapdata/symbols/28x28/block28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/28x28/circle28.xbm` & `mapdata-3.6.0/mapdata/symbols/28x28/circle28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata/symbols/28x28/square28.xbm` & `mapdata-3.6.0/mapdata/symbols/28x28/square28.xbm`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/mapdata.egg-info/PKG-INFO` & `mapdata-3.6.0/mapdata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapdata
-Version: 3.5.0
+Version: 3.6.0
 Summary: An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database
 Home-page: https://osdn.net/project/mapdata/
 Author: Dreas Nielsen
 Author-email: cortice@tutanota.com
 License: GPL
 Keywords: Map,Locations,CRS,CSV,Spreadsheet,Database,PNG,JPG,Postscript
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `mapdata-3.5.0/mapdata.egg-info/SOURCES.txt` & `mapdata-3.6.0/mapdata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mapdata-3.5.0/setup.py` & `mapdata-3.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with io.open('README.md', encoding='utf-8') as f:
 	long_description = f.read()
 
 symbol_files = glob.glob("mapdata/symbols/16x16/*.xbm") + glob.glob("mapdata/symbols/20x20/*.xbm") + \
 			glob.glob("mapdata/symbols/24x24/*.xbm") + glob.glob("mapdata/symbols/28x28/*.xbm")
 
 setuptools.setup(name='mapdata',
-	version='3.5.0',
+	version='3.6.0',
 	description="An interactive map and table explorer for geographic coordinates in a spreadsheet, CSV file, or database",
 	author='Dreas Nielsen',
 	author_email='cortice@tutanota.com',
     url='https://osdn.net/project/mapdata/',
     packages=['mapdata'],
 	scripts=['mapdata/mapdata.py'],
 	data_files=[('symbols', symbol_files), ('config', ['mapdata/configfile/mapdata.conf'])],
```

