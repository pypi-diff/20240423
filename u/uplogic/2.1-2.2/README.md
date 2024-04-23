# Comparing `tmp/uplogic-2.1.tar.gz` & `tmp/uplogic-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uplogic-2.1.tar", last modified: Fri Feb 16 10:11:41 2024, max compression
+gzip compressed data, was "uplogic-2.2.tar", last modified: Tue Apr 23 18:17:52 2024, max compression
```

## Comparing `uplogic-2.1.tar` & `uplogic-2.2.tar`

### file list

```diff
@@ -1,419 +1,426 @@
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.443203 uplogic-2.1/
--rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-2.1/LICENSE.md
--rw-rw-rw-   0        0        0     1045 2024-02-16 10:11:41.442203 uplogic-2.1/PKG-INFO
--rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-2.1/README.md
--rw-rw-rw-   0        0        0       42 2024-02-16 10:11:41.443203 uplogic-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1739 2024-02-16 10:11:22.000000 uplogic-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:40.985328 uplogic-2.1/uplogic/
--rw-rw-rw-   0        0        0     6472 2024-02-05 13:29:43.000000 uplogic-2.1/uplogic/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.019327 uplogic-2.1/uplogic/animation/
--rw-rw-rw-   0        0        0      341 2023-12-07 08:59:05.000000 uplogic-2.1/uplogic/animation/__init__.py
--rw-rw-rw-   0        0        0    14018 2024-01-23 04:24:15.000000 uplogic-2.1/uplogic/animation/action.py
--rw-rw-rw-   0        0        0     4151 2024-01-23 04:26:24.000000 uplogic-2.1/uplogic/animation/actionsystem.py
--rw-rw-rw-   0        0        0     2419 2023-11-10 06:42:05.000000 uplogic-2.1/uplogic/animation/rig.py
--rw-rw-rw-   0        0        0     6935 2023-10-12 17:14:35.000000 uplogic-2.1/uplogic/animation/sequence.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.023328 uplogic-2.1/uplogic/audio/
--rw-rw-rw-   0        0        0      606 2023-12-15 10:12:29.000000 uplogic-2.1/uplogic/audio/__init__.py
--rw-rw-rw-   0        0        0     7747 2024-02-10 14:51:22.000000 uplogic-2.1/uplogic/audio/audiosystem.py
--rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-2.1/uplogic/audio/music.py
--rw-rw-rw-   0        0        0    24472 2024-02-07 15:06:16.000000 uplogic-2.1/uplogic/audio/sound.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.027329 uplogic-2.1/uplogic/data/
--rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-2.1/uplogic/data/__init__.py
--rw-rw-rw-   0        0        0     3161 2024-02-02 14:24:41.000000 uplogic-2.1/uplogic/data/file.py
--rw-rw-rw-   0        0        0     7239 2023-10-14 18:09:43.000000 uplogic-2.1/uplogic/data/globaldb.py
--rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-2.1/uplogic/data/serializers.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.037340 uplogic-2.1/uplogic/decorators/
--rw-rw-rw-   0        0        0    18208 2024-02-16 10:10:51.000000 uplogic-2.1/uplogic/decorators/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.038331 uplogic-2.1/uplogic/events/
--rw-rw-rw-   0        0        0     8364 2024-02-16 10:03:20.000000 uplogic-2.1/uplogic/events/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.043332 uplogic-2.1/uplogic/input/
--rw-rw-rw-   0        0        0     1541 2023-09-30 18:00:52.000000 uplogic-2.1/uplogic/input/__init__.py
--rw-rw-rw-   0        0        0    15782 2024-02-07 12:12:16.000000 uplogic-2.1/uplogic/input/gamepad.py
--rw-rw-rw-   0        0        0    10458 2023-10-10 08:44:42.000000 uplogic-2.1/uplogic/input/keyboard.py
--rw-rw-rw-   0        0        0    15356 2024-02-07 11:49:53.000000 uplogic-2.1/uplogic/input/mouse.py
--rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-2.1/uplogic/input/vr.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.044333 uplogic-2.1/uplogic/logging/
--rw-rw-rw-   0        0        0     6509 2024-02-07 12:01:45.000000 uplogic-2.1/uplogic/logging/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.047332 uplogic-2.1/uplogic/network/
--rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-2.1/uplogic/network/__init__.py
--rw-rw-rw-   0        0        0     2919 2023-07-11 14:56:49.000000 uplogic-2.1/uplogic/network/client.py
--rw-rw-rw-   0        0        0     4687 2023-07-20 06:49:18.000000 uplogic-2.1/uplogic/network/server.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.049333 uplogic-2.1/uplogic/nodes/
--rw-rw-rw-   0        0        0     4119 2024-01-22 11:03:04.000000 uplogic-2.1/uplogic/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.228155 uplogic-2.1/uplogic/nodes/actions/
--rw-rw-rw-   0        0        0     8317 2024-01-16 18:59:56.000000 uplogic-2.1/uplogic/nodes/actions/__init__.py
--rw-rw-rw-   0        0        0     3996 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/addfilter.py
--rw-rw-rw-   0        0        0     1088 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/addobject.py
--rw-rw-rw-   0        0        0     2219 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/addphysicsconstraint.py
--rw-rw-rw-   0        0        0      666 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/adduiwidget.py
--rw-rw-rw-   0        0        0      972 2024-02-16 09:50:28.000000 uplogic-2.1/uplogic/nodes/actions/alignaxistovector.py
--rw-rw-rw-   0        0        0      859 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/appendlistitem.py
--rw-rw-rw-   0        0        0      723 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applyforce.py
--rw-rw-rw-   0        0        0      838 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applyimpulse.py
--rw-rw-rw-   0        0        0      767 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applymovement.py
--rw-rw-rw-   0        0        0      930 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applyrotation.py
--rw-rw-rw-   0        0        0      781 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applytorque.py
--rw-rw-rw-   0        0        0     1540 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/applytransform.py
--rw-rw-rw-   0        0        0     1580 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/cameraraycast.py
--rw-rw-rw-   0        0        0      693 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/characterjump.py
--rw-rw-rw-   0        0        0     1213 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/clampedmodifyproperty.py
--rw-rw-rw-   0        0        0     1510 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/clearvariables.py
--rw-rw-rw-   0        0        0     1061 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/copyproperty.py
--rw-rw-rw-   0        0        0     3503 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuibutton.py
--rw-rw-rw-   0        0        0      773 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuicanvas.py
--rw-rw-rw-   0        0        0     1692 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuiimage.py
--rw-rw-rw-   0        0        0     2485 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuilabel.py
--rw-rw-rw-   0        0        0     2284 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuilayout.py
--rw-rw-rw-   0        0        0     4432 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createuislider.py
--rw-rw-rw-   0        0        0     1657 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/createvehicle.py
--rw-rw-rw-   0        0        0     1326 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/cursorbehavior.py
--rw-rw-rw-   0        0        0      651 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/cursorvisibility.py
--rw-rw-rw-   0        0        0      814 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/dispatchevent.py
--rw-rw-rw-   0        0        0     2342 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/draw.py
--rw-rw-rw-   0        0        0     1162 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/drawbox.py
--rw-rw-rw-   0        0        0     1018 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/drawcube.py
--rw-rw-rw-   0        0        0      961 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/drawline.py
--rw-rw-rw-   0        0        0     3032 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/editbone.py
--rw-rw-rw-   0        0        0      432 2023-10-13 21:24:56.000000 uplogic-2.1/uplogic/nodes/actions/endgame.py
--rw-rw-rw-   0        0        0      729 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/endobject.py
--rw-rw-rw-   0        0        0     1300 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/executesubnetwork.py
--rw-rw-rw-   0        0        0     4798 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/followpath.py
--rw-rw-rw-   0        0        0     2813 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/gamepadlook.py
--rw-rw-rw-   0        0        0     1185 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/gamepadvibration.py
--rw-rw-rw-   0        0        0     2012 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/getperformanceprofile.py
--rw-rw-rw-   0        0        0     1002 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/installsubnetwork.py
--rw-rw-rw-   0        0        0     2044 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/instream.py
--rw-rw-rw-   0        0        0     1136 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/listglobalvalues.py
--rw-rw-rw-   0        0        0     1914 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/listvariables.py
--rw-rw-rw-   0        0        0      634 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/loadblendfile.py
--rw-rw-rw-   0        0        0     1549 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/loadfilecontent.py
--rw-rw-rw-   0        0        0     4078 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/loadgame.py
--rw-rw-rw-   0        0        0     1663 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/loadscene.py
--rw-rw-rw-   0        0        0     2476 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/localclient.py
--rw-rw-rw-   0        0        0     2352 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/localserver.py
--rw-rw-rw-   0        0        0      775 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/makeuniquelight.py
--rw-rw-rw-   0        0        0     1347 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/modifyproperty.py
--rw-rw-rw-   0        0        0     2711 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/mouselook.py
--rw-rw-rw-   0        0        0     1580 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/mouseraycast.py
--rw-rw-rw-   0        0        0      810 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/mousesetposition.py
--rw-rw-rw-   0        0        0     1130 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/moveto.py
--rw-rw-rw-   0        0        0     4621 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/movetowithnavmesh.py
--rw-rw-rw-   0        0        0      608 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/pausesound.py
--rw-rw-rw-   0        0        0     4386 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/playaction.py
--rw-rw-rw-   0        0        0     2276 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/playsequence.py
--rw-rw-rw-   0        0        0     1135 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/popdictkey.py
--rw-rw-rw-   0        0        0      662 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/printvalue.py
--rw-rw-rw-   0        0        0     2986 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/projectileraycast.py
--rw-rw-rw-   0        0        0     3064 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/raycast.py
--rw-rw-rw-   0        0        0      650 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removefilter.py
--rw-rw-rw-   0        0        0      977 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removelistindex.py
--rw-rw-rw-   0        0        0     1010 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removelistvalue.py
--rw-rw-rw-   0        0        0      646 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removeoverlaycollection.py
--rw-rw-rw-   0        0        0      620 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removeparent.py
--rw-rw-rw-   0        0        0      737 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removephysicsconstraint.py
--rw-rw-rw-   0        0        0     1644 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/removevariable.py
--rw-rw-rw-   0        0        0     1064 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/replacemesh.py
--rw-rw-rw-   0        0        0      544 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/restartgame.py
--rw-rw-rw-   0        0        0      560 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/resumesound.py
--rw-rw-rw-   0        0        0     1032 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/rotateto.py
--rw-rw-rw-   0        0        0      949 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/runactuator.py
--rw-rw-rw-   0        0        0     1894 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/runpython.py
--rw-rw-rw-   0        0        0     7788 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/savegame.py
--rw-rw-rw-   0        0        0     1812 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/savevariable.py
--rw-rw-rw-   0        0        0     1551 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/savevariabledict.py
--rw-rw-rw-   0        0        0     1055 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/sendmessage.py
--rw-rw-rw-   0        0        0      705 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/sendnetworkmessage.py
--rw-rw-rw-   0        0        0     2282 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setactionframe.py
--rw-rw-rw-   0        0        0      939 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setactuatorvalue.py
--rw-rw-rw-   0        0        0     1136 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setboneconstraintattr.py
--rw-rw-rw-   0        0        0     1013 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setboneconstraintinfluence.py
--rw-rw-rw-   0        0        0     1009 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setboneconstrainttarget.py
--rw-rw-rw-   0        0        0     1221 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setboneposition.py
--rw-rw-rw-   0        0        0      664 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcamera.py
--rw-rw-rw-   0        0        0      656 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcamerafov.py
--rw-rw-rw-   0        0        0      679 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcameraorthoscale.py
--rw-rw-rw-   0        0        0      868 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcharactergravity.py
--rw-rw-rw-   0        0        0      781 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcharacterjumpspeed.py
--rw-rw-rw-   0        0        0      795 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcharactermaxjumps.py
--rw-rw-rw-   0        0        0      910 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcharactervelocity.py
--rw-rw-rw-   0        0        0     1489 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcharacterwalkdir.py
--rw-rw-rw-   0        0        0      812 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcollisiongroup.py
--rw-rw-rw-   0        0        0      700 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcollisionmask.py
--rw-rw-rw-   0        0        0      890 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setconstraintattribute.py
--rw-rw-rw-   0        0        0     1176 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcurvepoints.py
--rw-rw-rw-   0        0        0     1003 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setcustomcursor.py
--rw-rw-rw-   0        0        0      899 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setdictkey.py
--rw-rw-rw-   0        0        0      859 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setdynamics.py
--rw-rw-rw-   0        0        0      698 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveeao.py
--rw-rw-rw-   0        0        0      702 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveebloom.py
--rw-rw-rw-   0        0        0      631 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveesmaa.py
--rw-rw-rw-   0        0        0      672 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveesmaaquality.py
--rw-rw-rw-   0        0        0      698 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveessr.py
--rw-rw-rw-   0        0        0      744 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/seteeveevolumetrics.py
--rw-rw-rw-   0        0        0      731 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setexposure.py
--rw-rw-rw-   0        0        0      736 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setfilterstate.py
--rw-rw-rw-   0        0        0      660 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setfullscreen.py
--rw-rw-rw-   0        0        0     1720 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setgameobjectattr.py
--rw-rw-rw-   0        0        0      725 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setgamma.py
--rw-rw-rw-   0        0        0      908 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setglobalvalue.py
--rw-rw-rw-   0        0        0      651 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setgravity.py
--rw-rw-rw-   0        0        0      817 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setlightcolor.py
--rw-rw-rw-   0        0        0      763 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setlightenergy.py
--rw-rw-rw-   0        0        0      783 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setlightshadow.py
--rw-rw-rw-   0        0        0      933 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setlistindex.py
--rw-rw-rw-   0        0        0      783 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setlogictreeproperty.py
--rw-rw-rw-   0        0        0     1091 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setmaterial.py
--rw-rw-rw-   0        0        0     1028 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setmatnodesocket.py
--rw-rw-rw-   0        0        0     1221 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setmatnodevalue.py
--rw-rw-rw-   0        0        0      995 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setnodesocket.py
--rw-rw-rw-   0        0        0     1188 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setnodevalue.py
--rw-rw-rw-   0        0        0      842 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setoverlaycollection.py
--rw-rw-rw-   0        0        0      890 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setparent.py
--rw-rw-rw-   0        0        0      876 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setphysics.py
--rw-rw-rw-   0        0        0      643 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setprofile.py
--rw-rw-rw-   0        0        0     1001 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setproperty.py
--rw-rw-rw-   0        0        0      728 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setpyinstanceattr.py
--rw-rw-rw-   0        0        0      702 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setresolution.py
--rw-rw-rw-   0        0        0      785 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setrigidbody.py
--rw-rw-rw-   0        0        0      672 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setscene.py
--rw-rw-rw-   0        0        0     1004 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setsensorvalue.py
--rw-rw-rw-   0        0        0      663 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/settimescale.py
--rw-rw-rw-   0        0        0     2243 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setuiwidgetattr.py
--rw-rw-rw-   0        0        0     2366 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setvisibility.py
--rw-rw-rw-   0        0        0      585 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/setvsync.py
--rw-rw-rw-   0        0        0      656 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/showframerate.py
--rw-rw-rw-   0        0        0     1247 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/slowfollow.py
--rw-rw-rw-   0        0        0     4012 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/spawnpool.py
--rw-rw-rw-   0        0        0     5354 2024-01-24 16:53:28.000000 uplogic-2.1/uplogic/nodes/actions/startsound.py
--rw-rw-rw-   0        0        0     1895 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/startsound2d.py
--rw-rw-rw-   0        0        0     2989 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/startsound3d.py
--rw-rw-rw-   0        0        0     2503 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/startspeaker.py
--rw-rw-rw-   0        0        0     1231 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/startsubnetwork.py
--rw-rw-rw-   0        0        0     1200 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/stopaction.py
--rw-rw-rw-   0        0        0      605 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/stopallsounds.py
--rw-rw-rw-   0        0        0      556 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/stopsound.py
--rw-rw-rw-   0        0        0      925 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/stopsubnetwork.py
--rw-rw-rw-   0        0        0      650 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/togglefilter.py
--rw-rw-rw-   0        0        0      854 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/toggleproperty.py
--rw-rw-rw-   0        0        0      537 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/translate.py
--rw-rw-rw-   0        0        0     1031 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/vectoranglecheck.py
--rw-rw-rw-   0        0        0     1083 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/vehicleapplybraking.py
--rw-rw-rw-   0        0        0     1076 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/vehicleapplyforce.py
--rw-rw-rw-   0        0        0     1084 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/vehicleapplysteering.py
--rw-rw-rw-   0        0        0     3172 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/actions/vehiclesetattributes.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.275166 uplogic-2.1/uplogic/nodes/conditions/
--rw-rw-rw-   0        0        0     2026 2023-10-03 15:16:22.000000 uplogic-2.1/uplogic/nodes/conditions/__init__.py
--rw-rw-rw-   0        0        0      893 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/barrier.py
--rw-rw-rw-   0        0        0      865 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/checkdistance.py
--rw-rw-rw-   0        0        0     4217 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/collision.py
--rw-rw-rw-   0        0        0      862 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/compare.py
--rw-rw-rw-   0        0        0     1204 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/comparevectors.py
--rw-rw-rw-   0        0        0     2086 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/controllerstatus.py
--rw-rw-rw-   0        0        0      937 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/evaluateproperty.py
--rw-rw-rw-   0        0        0      739 2024-02-07 13:13:10.000000 uplogic-2.1/uplogic/nodes/conditions/gamepadactive.py
--rw-rw-rw-   0        0        0      747 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/gamepadbutton.py
--rw-rw-rw-   0        0        0     1291 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/gamepadbuttonup.py
--rw-rw-rw-   0        0        0      850 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/handleevent.py
--rw-rw-rw-   0        0        0      676 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/hasproperty.py
--rw-rw-rw-   0        0        0      324 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/keyboardactive.py
--rw-rw-rw-   0        0        0      654 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/keypressed.py
--rw-rw-rw-   0        0        0      623 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/keyreleased.py
--rw-rw-rw-   0        0        0      987 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicand.py
--rw-rw-rw-   0        0        0      429 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicandnot.py
--rw-rw-rw-   0        0        0     1761 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicgate.py
--rw-rw-rw-   0        0        0      946 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicgatelist.py
--rw-rw-rw-   0        0        0      327 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicnone.py
--rw-rw-rw-   0        0        0      371 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicnot.py
--rw-rw-rw-   0        0        0      336 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicnotnone.py
--rw-rw-rw-   0        0        0     1016 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logicor.py
--rw-rw-rw-   0        0        0     1001 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/logictreestatus.py
--rw-rw-rw-   0        0        0      402 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mousemoved.py
--rw-rw-rw-   0        0        0     2920 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mouseover.py
--rw-rw-rw-   0        0        0      670 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mousepressed.py
--rw-rw-rw-   0        0        0      979 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mousepressedon.py
--rw-rw-rw-   0        0        0      765 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mousereleased.py
--rw-rw-rw-   0        0        0      704 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/mousescroll.py
--rw-rw-rw-   0        0        0      795 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/once.py
--rw-rw-rw-   0        0        0      281 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/oninit.py
--rw-rw-rw-   0        0        0      638 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/onnexttick.py
--rw-rw-rw-   0        0        0      282 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/onupdate.py
--rw-rw-rw-   0        0        0     1013 2024-01-22 11:36:48.000000 uplogic-2.1/uplogic/nodes/conditions/onvaluechanged.py
--rw-rw-rw-   0        0        0      811 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/onvaluechangedto.py
--rw-rw-rw-   0        0        0      867 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/pulsify.py
--rw-rw-rw-   0        0        0      493 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/sensorpositive.py
--rw-rw-rw-   0        0        0      858 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/timedelay.py
--rw-rw-rw-   0        0        0      914 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/timer.py
--rw-rw-rw-   0        0        0      490 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/truefalse.py
--rw-rw-rw-   0        0        0      402 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/valuevalid.py
--rw-rw-rw-   0        0        0     1040 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/conditions/vectoranglecheck.py
--rw-rw-rw-   0        0        0     5389 2024-01-17 17:29:27.000000 uplogic-2.1/uplogic/nodes/logictree.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.384191 uplogic-2.1/uplogic/nodes/parameters/
--rw-rw-rw-   0        0        0     5104 2023-12-15 10:48:20.000000 uplogic-2.1/uplogic/nodes/parameters/__init__.py
--rw-rw-rw-   0        0        0      431 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/absolutevalue.py
--rw-rw-rw-   0        0        0     1431 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/actionstatus.py
--rw-rw-rw-   0        0        0      373 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/activecamera.py
--rw-rw-rw-   0        0        0      500 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/axisvector.py
--rw-rw-rw-   0        0        0     1733 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/bonestatus.py
--rw-rw-rw-   0        0        0     1560 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/characterinfo.py
--rw-rw-rw-   0        0        0      598 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/childbyindex.py
--rw-rw-rw-   0        0        0      592 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/childbyname.py
--rw-rw-rw-   0        0        0      873 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/clamp.py
--rw-rw-rw-   0        0        0      433 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/colorrgb.py
--rw-rw-rw-   0        0        0      434 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/colorrgba.py
--rw-rw-rw-   0        0        0      604 2024-01-26 09:06:04.000000 uplogic-2.1/uplogic/nodes/parameters/dictvalue.py
--rw-rw-rw-   0        0        0      504 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/distance.py
--rw-rw-rw-   0        0        0      641 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/euler.py
--rw-rw-rw-   0        0        0      592 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/eulertomatrix.py
--rw-rw-rw-   0        0        0      771 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/formattedstring.py
--rw-rw-rw-   0        0        0     1958 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/formula.py
--rw-rw-rw-   0        0        0      363 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/fpsfactor.py
--rw-rw-rw-   0        0        0     1969 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/gamepadsticks.py
--rw-rw-rw-   0        0        0     1519 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/gamepadtrigger.py
--rw-rw-rw-   0        0        0      649 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getactuatorvalue.py
--rw-rw-rw-   0        0        0      362 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getcollection.py
--rw-rw-rw-   0        0        0      503 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getcollectionobjectnames.py
--rw-rw-rw-   0        0        0      568 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getcollectionobjects.py
--rw-rw-rw-   0        0        0      621 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getcurvepoints.py
--rw-rw-rw-   0        0        0      334 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getfont.py
--rw-rw-rw-   0        0        0      345 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getfullscreen.py
--rw-rw-rw-   0        0        0      601 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getglobalvalue.py
--rw-rw-rw-   0        0        0      376 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getgravity.py
--rw-rw-rw-   0        0        0      337 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getimage.py
--rw-rw-rw-   0        0        0      437 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getlightcolor.py
--rw-rw-rw-   0        0        0      443 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getlightenergy.py
--rw-rw-rw-   0        0        0      660 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getlogictreeproperty.py
--rw-rw-rw-   0        0        0      844 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getnodeattribute.py
--rw-rw-rw-   0        0        0      698 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getnodesocket.py
--rw-rw-rw-   0        0        0      408 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getobject.py
--rw-rw-rw-   0        0        0      284 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getowner.py
--rw-rw-rw-   0        0        0      361 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getparent.py
--rw-rw-rw-   0        0        0      837 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getproperty.py
--rw-rw-rw-   0        0        0      468 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getpyinstanceattr.py
--rw-rw-rw-   0        0        0      700 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getresolution.py
--rw-rw-rw-   0        0        0      328 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getscene.py
--rw-rw-rw-   0        0        0      639 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getsensorvalue.py
--rw-rw-rw-   0        0        0      335 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getsound.py
--rw-rw-rw-   0        0        0      329 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/gettimescale.py
--rw-rw-rw-   0        0        0      864 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getuiwidgetattr.py
--rw-rw-rw-   0        0        0      325 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/getvsync.py
--rw-rw-rw-   0        0        0      373 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/initemptydict.py
--rw-rw-rw-   0        0        0      453 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/initemptylist.py
--rw-rw-rw-   0        0        0      435 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/initnewdict.py
--rw-rw-rw-   0        0        0      856 2024-02-09 10:13:40.000000 uplogic-2.1/uplogic/nodes/parameters/instream.py
--rw-rw-rw-   0        0        0      517 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/interpolate.py
--rw-rw-rw-   0        0        0      443 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/invertvalue.py
--rw-rw-rw-   0        0        0      312 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/keycode.py
--rw-rw-rw-   0        0        0     1271 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/limitrange.py
--rw-rw-rw-   0        0        0      382 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/listduplicate.py
--rw-rw-rw-   0        0        0      566 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/listextend.py
--rw-rw-rw-   0        0        0      366 2024-01-24 16:53:05.000000 uplogic-2.1/uplogic/nodes/parameters/listfromitems.py
--rw-rw-rw-   0        0        0      500 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/listindex.py
--rw-rw-rw-   0        0        0      486 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/listindexrandom.py
--rw-rw-rw-   0        0        0     1505 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/loadvariable.py
--rw-rw-rw-   0        0        0     1214 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/loadvariabledict.py
--rw-rw-rw-   0        0        0      870 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/maprange.py
--rw-rw-rw-   0        0        0      892 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/materialgetattribute.py
--rw-rw-rw-   0        0        0      595 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/materialgetnode.py
--rw-rw-rw-   0        0        0      732 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/materialgetsocket.py
--rw-rw-rw-   0        0        0     1712 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/math.py
--rw-rw-rw-   0        0        0      607 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/matrixtoxyz.py
--rw-rw-rw-   0        0        0     1084 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/mousedata.py
--rw-rw-rw-   0        0        0      696 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/objectattr.py
--rw-rw-rw-   0        0        0      391 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/objectdataname.py
--rw-rw-rw-   0        0        0      623 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/objectdatavertices.py
--rw-rw-rw-   0        0        0      780 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/randomfloat.py
--rw-rw-rw-   0        0        0      729 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/randomint.py
--rw-rw-rw-   0        0        0     1761 2024-02-16 09:48:53.000000 uplogic-2.1/uplogic/nodes/parameters/randomvalue.py
--rw-rw-rw-   0        0        0      678 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/randomvect.py
--rw-rw-rw-   0        0        0      968 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/rangedthreshold.py
--rw-rw-rw-   0        0        0     1572 2024-01-26 09:20:12.000000 uplogic-2.1/uplogic/nodes/parameters/rebuilddata.py
--rw-rw-rw-   0        0        0      906 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/resizevector.py
--rw-rw-rw-   0        0        0     1627 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/rotatebypoint.py
--rw-rw-rw-   0        0        0      501 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/screenposition.py
--rw-rw-rw-   0        0        0      773 2024-01-26 09:14:21.000000 uplogic-2.1/uplogic/nodes/parameters/serializedata.py
--rw-rw-rw-   0        0        0      361 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/simplevalue.py
--rw-rw-rw-   0        0        0      731 2024-02-16 09:47:25.000000 uplogic-2.1/uplogic/nodes/parameters/storevalue.py
--rw-rw-rw-   0        0        0      797 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/threshold.py
--rw-rw-rw-   0        0        0      924 2024-01-22 11:36:57.000000 uplogic-2.1/uplogic/nodes/parameters/timedata.py
--rw-rw-rw-   0        0        0      724 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/typecastvalue.py
--rw-rw-rw-   0        0        0     4232 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/valueswitch.py
--rw-rw-rw-   0        0        0      541 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorabsolute.py
--rw-rw-rw-   0        0        0      626 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorangle.py
--rw-rw-rw-   0        0        0       60 2023-09-30 12:04:19.000000 uplogic-2.1/uplogic/nodes/parameters/vectoranglecheck.py
--rw-rw-rw-   0        0        0      417 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorlength.py
--rw-rw-rw-   0        0        0     4672 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectormath.py
--rw-rw-rw-   0        0        0      617 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorsplitxy.py
--rw-rw-rw-   0        0        0      725 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorsplitxyz.py
--rw-rw-rw-   0        0        0      478 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorxy.py
--rw-rw-rw-   0        0        0      553 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorxyz.py
--rw-rw-rw-   0        0        0      624 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vectorxyzw.py
--rw-rw-rw-   0        0        0     1312 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vrcontrollervalues.py
--rw-rw-rw-   0        0        0      525 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/vrheadsetvalues.py
--rw-rw-rw-   0        0        0      962 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/withinrange.py
--rw-rw-rw-   0        0        0      770 2024-01-22 11:02:02.000000 uplogic-2.1/uplogic/nodes/parameters/worldposition.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.391191 uplogic-2.1/uplogic/physics/
--rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-2.1/uplogic/physics/__init__.py
--rw-rw-rw-   0        0        0     4196 2023-05-14 08:28:32.000000 uplogic-2.1/uplogic/physics/buoyancy.py
--rw-rw-rw-   0        0        0     4099 2023-10-14 18:29:13.000000 uplogic-2.1/uplogic/physics/character.py
--rw-rw-rw-   0        0        0     3595 2023-11-06 03:14:00.000000 uplogic-2.1/uplogic/physics/collision.py
--rw-rw-rw-   0        0        0     8370 2024-02-06 12:40:32.000000 uplogic-2.1/uplogic/physics/constraints.py
--rw-rw-rw-   0        0        0    10164 2024-01-25 16:38:46.000000 uplogic-2.1/uplogic/physics/vehicle.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.391191 uplogic-2.1/uplogic/serialize/
--rw-rw-rw-   0        0        0     2965 2023-12-11 16:15:51.000000 uplogic-2.1/uplogic/serialize/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.414197 uplogic-2.1/uplogic/shaders/
--rw-rw-rw-   0        0        0      703 2024-02-12 15:24:15.000000 uplogic-2.1/uplogic/shaders/__init__.py
--rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-2.1/uplogic/shaders/adaptivetonemapping.py
--rw-rw-rw-   0        0        0     1631 2023-04-01 06:53:32.000000 uplogic-2.1/uplogic/shaders/blur.py
--rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/brightness.py
--rw-rw-rw-   0        0        0      829 2024-02-15 08:06:02.000000 uplogic-2.1/uplogic/shaders/buffer.py
--rw-rw-rw-   0        0        0     1050 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/chromaticaberration.py
--rw-rw-rw-   0        0        0     8869 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/distort.py
--rw-rw-rw-   0        0        0     9834 2023-10-18 10:42:33.000000 uplogic-2.1/uplogic/shaders/dof.py
--rw-rw-rw-   0        0        0     9106 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/droplets.py
--rw-rw-rw-   0        0        0    33424 2024-01-26 11:25:17.000000 uplogic-2.1/uplogic/shaders/fxaa.py
--rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/grayscale.py
--rw-rw-rw-   0        0        0     9683 2023-07-05 14:45:48.000000 uplogic-2.1/uplogic/shaders/hbao.py
--rw-rw-rw-   0        0        0     1173 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/letterbox.py
--rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/levels.py
--rw-rw-rw-   0        0        0     4209 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/mist.py
--rw-rw-rw-   0        0        0     1779 2024-02-12 11:42:26.000000 uplogic-2.1/uplogic/shaders/rendertoscreen.py
--rw-rw-rw-   0        0        0     5701 2024-02-12 15:06:24.000000 uplogic-2.1/uplogic/shaders/shader.py
--rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-2.1/uplogic/shaders/sharpen.py
--rw-rw-rw-   0        0        0     2898 2024-02-12 11:42:41.000000 uplogic-2.1/uplogic/shaders/splitscreen.py
--rw-rw-rw-   0        0        0     5738 2023-06-20 15:34:55.000000 uplogic-2.1/uplogic/shaders/ssao.py
--rw-rw-rw-   0        0        0     1189 2024-02-12 15:10:32.000000 uplogic-2.1/uplogic/shaders/vignette.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.428200 uplogic-2.1/uplogic/ui/
--rw-rw-rw-   0        0        0      619 2024-02-16 10:06:39.000000 uplogic-2.1/uplogic/ui/__init__.py
--rw-rw-rw-   0        0        0     1712 2024-02-16 10:02:44.000000 uplogic-2.1/uplogic/ui/behaviors.py
--rw-rw-rw-   0        0        0    10061 2024-02-09 14:26:10.000000 uplogic-2.1/uplogic/ui/button.py
--rw-rw-rw-   0        0        0     1722 2023-11-11 20:36:46.000000 uplogic-2.1/uplogic/ui/camera.py
--rw-rw-rw-   0        0        0     3577 2024-02-15 07:30:22.000000 uplogic-2.1/uplogic/ui/canvas.py
--rw-rw-rw-   0        0        0     3765 2024-02-02 15:06:15.000000 uplogic-2.1/uplogic/ui/cursor.py
--rw-rw-rw-   0        0        0     7249 2024-02-12 11:12:11.000000 uplogic-2.1/uplogic/ui/image.py
--rw-rw-rw-   0        0        0     7555 2024-02-11 18:38:42.000000 uplogic-2.1/uplogic/ui/label.py
--rw-rw-rw-   0        0        0    13537 2024-02-07 10:42:42.000000 uplogic-2.1/uplogic/ui/layout.py
--rw-rw-rw-   0        0        0     5166 2024-02-07 10:41:01.000000 uplogic-2.1/uplogic/ui/path.py
--rw-rw-rw-   0        0        0     2041 2024-02-16 10:05:38.000000 uplogic-2.1/uplogic/ui/render.py
--rw-rw-rw-   0        0        0     8061 2024-01-19 14:39:50.000000 uplogic-2.1/uplogic/ui/slider.py
--rw-rw-rw-   0        0        0    15745 2024-02-07 10:41:01.000000 uplogic-2.1/uplogic/ui/widget.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.441203 uplogic-2.1/uplogic/utils/
--rw-rw-rw-   0        0        0     7396 2024-02-04 10:29:55.000000 uplogic-2.1/uplogic/utils/__init__.py
--rw-rw-rw-   0        0        0     1642 2023-11-09 02:27:44.000000 uplogic-2.1/uplogic/utils/constants.py
--rw-rw-rw-   0        0        0     1089 2023-06-20 14:44:01.000000 uplogic-2.1/uplogic/utils/engine.py
--rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-2.1/uplogic/utils/errors.py
--rw-rw-rw-   0        0        0     4650 2023-11-22 09:34:56.000000 uplogic-2.1/uplogic/utils/lights.py
--rw-rw-rw-   0        0        0    10698 2024-02-07 14:58:16.000000 uplogic-2.1/uplogic/utils/math.py
--rw-rw-rw-   0        0        0     4801 2023-12-31 14:36:53.000000 uplogic-2.1/uplogic/utils/nodetrees.py
--rw-rw-rw-   0        0        0    16950 2024-02-05 16:13:33.000000 uplogic-2.1/uplogic/utils/objects.py
--rw-rw-rw-   0        0        0    10075 2023-11-09 14:18:13.000000 uplogic-2.1/uplogic/utils/pooling.py
--rw-rw-rw-   0        0        0    13778 2023-10-13 21:24:56.000000 uplogic-2.1/uplogic/utils/raycasting.py
--rw-rw-rw-   0        0        0     6277 2024-02-11 18:43:32.000000 uplogic-2.1/uplogic/utils/scene.py
--rw-rw-rw-   0        0        0     2943 2024-01-28 12:18:13.000000 uplogic-2.1/uplogic/utils/visualize.py
--rw-rw-rw-   0        0        0     2553 2023-12-11 10:29:42.000000 uplogic-2.1/uplogic/utils/visuals.py
-drwxrwxrwx   0        0        0        0 2024-02-16 10:11:41.014326 uplogic-2.1/uplogic.egg-info/
--rw-rw-rw-   0        0        0     1045 2024-02-16 10:11:40.000000 uplogic-2.1/uplogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    14556 2024-02-16 10:11:40.000000 uplogic-2.1/uplogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-16 10:11:40.000000 uplogic-2.1/uplogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-02-16 10:11:40.000000 uplogic-2.1/uplogic.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-02-16 10:11:40.000000 uplogic-2.1/uplogic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-2.1/uplogic.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.601885 uplogic-2.2/
+-rw-rw-rw-   0        0        0      189 2022-01-15 11:35:38.000000 uplogic-2.2/LICENSE.md
+-rw-rw-rw-   0        0        0     1045 2024-04-23 18:17:52.600888 uplogic-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      262 2022-01-15 11:34:53.000000 uplogic-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-23 18:17:52.601885 uplogic-2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1739 2024-04-23 18:17:43.000000 uplogic-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.442417 uplogic-2.2/uplogic/
+-rw-rw-rw-   0        0        0     6474 2024-03-22 08:56:45.000000 uplogic-2.2/uplogic/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.456371 uplogic-2.2/uplogic/animation/
+-rw-rw-rw-   0        0        0      341 2023-12-07 08:59:05.000000 uplogic-2.2/uplogic/animation/__init__.py
+-rw-rw-rw-   0        0        0    14151 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/animation/action.py
+-rw-rw-rw-   0        0        0     4152 2024-02-18 10:41:26.000000 uplogic-2.2/uplogic/animation/actionsystem.py
+-rw-rw-rw-   0        0        0     2419 2023-11-10 06:42:05.000000 uplogic-2.2/uplogic/animation/rig.py
+-rw-rw-rw-   0        0        0     6893 2024-02-18 10:45:19.000000 uplogic-2.2/uplogic/animation/sequence.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.457368 uplogic-2.2/uplogic/audio/
+-rw-rw-rw-   0        0        0      606 2023-12-15 10:12:29.000000 uplogic-2.2/uplogic/audio/__init__.py
+-rw-rw-rw-   0        0        0     7747 2024-02-10 14:51:22.000000 uplogic-2.2/uplogic/audio/audiosystem.py
+-rw-rw-rw-   0        0        0     6839 2023-05-14 08:47:09.000000 uplogic-2.2/uplogic/audio/music.py
+-rw-rw-rw-   0        0        0    24557 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/audio/sound.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.458364 uplogic-2.2/uplogic/console/
+-rw-rw-rw-   0        0        0    12943 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/console/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.459361 uplogic-2.2/uplogic/data/
+-rw-rw-rw-   0        0        0     1861 2022-10-06 13:43:59.000000 uplogic-2.2/uplogic/data/__init__.py
+-rw-rw-rw-   0        0        0     3161 2024-02-02 14:24:41.000000 uplogic-2.2/uplogic/data/file.py
+-rw-rw-rw-   0        0        0     7457 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/data/globaldb.py
+-rw-rw-rw-   0        0        0     2050 2021-12-21 09:41:07.000000 uplogic-2.2/uplogic/data/serializers.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.464345 uplogic-2.2/uplogic/decorators/
+-rw-rw-rw-   0        0        0    18211 2024-02-18 10:35:16.000000 uplogic-2.2/uplogic/decorators/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.464345 uplogic-2.2/uplogic/events/
+-rw-rw-rw-   0        0        0     8314 2024-02-18 10:46:49.000000 uplogic-2.2/uplogic/events/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.470324 uplogic-2.2/uplogic/input/
+-rw-rw-rw-   0        0        0     1541 2023-09-30 18:00:52.000000 uplogic-2.2/uplogic/input/__init__.py
+-rw-rw-rw-   0        0        0    15973 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/input/gamepad.py
+-rw-rw-rw-   0        0        0    10967 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/input/keyboard.py
+-rw-rw-rw-   0        0        0    15356 2024-03-18 14:27:09.000000 uplogic-2.2/uplogic/input/mouse.py
+-rw-rw-rw-   0        0        0     9131 2023-05-14 08:49:48.000000 uplogic-2.2/uplogic/input/vr.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.471321 uplogic-2.2/uplogic/network/
+-rw-rw-rw-   0        0        0       56 2023-06-05 09:06:00.000000 uplogic-2.2/uplogic/network/__init__.py
+-rw-rw-rw-   0        0        0     2919 2024-03-22 08:56:49.000000 uplogic-2.2/uplogic/network/client.py
+-rw-rw-rw-   0        0        0     4687 2024-03-22 08:56:53.000000 uplogic-2.2/uplogic/network/server.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.472318 uplogic-2.2/uplogic/nodes/
+-rw-rw-rw-   0        0        0     4276 2024-02-19 13:51:02.000000 uplogic-2.2/uplogic/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.522151 uplogic-2.2/uplogic/nodes/actions/
+-rw-rw-rw-   0        0        0     8317 2024-01-16 18:59:56.000000 uplogic-2.2/uplogic/nodes/actions/__init__.py
+-rw-rw-rw-   0        0        0     4259 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addfilter.py
+-rw-rw-rw-   0        0        0     1049 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addobject.py
+-rw-rw-rw-   0        0        0     2180 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/addphysicsconstraint.py
+-rw-rw-rw-   0        0        0      627 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/adduiwidget.py
+-rw-rw-rw-   0        0        0      933 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/alignaxistovector.py
+-rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/appendlistitem.py
+-rw-rw-rw-   0        0        0      684 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyforce.py
+-rw-rw-rw-   0        0        0      799 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyimpulse.py
+-rw-rw-rw-   0        0        0      728 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applymovement.py
+-rw-rw-rw-   0        0        0      891 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applyrotation.py
+-rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applytorque.py
+-rw-rw-rw-   0        0        0     1501 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/applytransform.py
+-rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cameraraycast.py
+-rw-rw-rw-   0        0        0      654 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/characterjump.py
+-rw-rw-rw-   0        0        0     1174 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/clampedmodifyproperty.py
+-rw-rw-rw-   0        0        0     1471 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/clearvariables.py
+-rw-rw-rw-   0        0        0     1022 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/copyproperty.py
+-rw-rw-rw-   0        0        0     3464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuibutton.py
+-rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuicanvas.py
+-rw-rw-rw-   0        0        0     1736 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuiimage.py
+-rw-rw-rw-   0        0        0     2420 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuilabel.py
+-rw-rw-rw-   0        0        0     2245 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuilayout.py
+-rw-rw-rw-   0        0        0     4393 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createuislider.py
+-rw-rw-rw-   0        0        0     1618 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/createvehicle.py
+-rw-rw-rw-   0        0        0     1287 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cursorbehavior.py
+-rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/cursorvisibility.py
+-rw-rw-rw-   0        0        0      775 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/dispatchevent.py
+-rw-rw-rw-   0        0        0     2485 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/draw.py
+-rw-rw-rw-   0        0        0     1123 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawbox.py
+-rw-rw-rw-   0        0        0      979 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawcube.py
+-rw-rw-rw-   0        0        0      922 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/drawline.py
+-rw-rw-rw-   0        0        0     2993 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/editbone.py
+-rw-rw-rw-   0        0        0      432 2023-10-13 21:24:56.000000 uplogic-2.2/uplogic/nodes/actions/endgame.py
+-rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/endobject.py
+-rw-rw-rw-   0        0        0     1261 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/executesubnetwork.py
+-rw-rw-rw-   0        0        0     4759 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/followpath.py
+-rw-rw-rw-   0        0        0     2774 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/gamepadlook.py
+-rw-rw-rw-   0        0        0     1146 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/gamepadvibration.py
+-rw-rw-rw-   0        0        0     1973 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/getperformanceprofile.py
+-rw-rw-rw-   0        0        0      963 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/installsubnetwork.py
+-rw-rw-rw-   0        0        0     2005 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/instream.py
+-rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/listglobalvalues.py
+-rw-rw-rw-   0        0        0     1875 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/listvariables.py
+-rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadblendfile.py
+-rw-rw-rw-   0        0        0     1510 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadfilecontent.py
+-rw-rw-rw-   0        0        0     4039 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadgame.py
+-rw-rw-rw-   0        0        0     1624 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/loadscene.py
+-rw-rw-rw-   0        0        0     2437 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/localclient.py
+-rw-rw-rw-   0        0        0     2313 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/localserver.py
+-rw-rw-rw-   0        0        0      736 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/makeuniquelight.py
+-rw-rw-rw-   0        0        0     1308 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/modifyproperty.py
+-rw-rw-rw-   0        0        0     2711 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mouselook.py
+-rw-rw-rw-   0        0        0     1541 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mouseraycast.py
+-rw-rw-rw-   0        0        0      771 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/mousesetposition.py
+-rw-rw-rw-   0        0        0     1117 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/moveto.py
+-rw-rw-rw-   0        0        0     4608 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/movetowithnavmesh.py
+-rw-rw-rw-   0        0        0      595 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/pausesound.py
+-rw-rw-rw-   0        0        0     4347 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/playaction.py
+-rw-rw-rw-   0        0        0     2237 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/playsequence.py
+-rw-rw-rw-   0        0        0     1096 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/popdictkey.py
+-rw-rw-rw-   0        0        0      623 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/printvalue.py
+-rw-rw-rw-   0        0        0     2947 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/projectileraycast.py
+-rw-rw-rw-   0        0        0     3025 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/raycast.py
+-rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removefilter.py
+-rw-rw-rw-   0        0        0      938 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removelistindex.py
+-rw-rw-rw-   0        0        0      971 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removelistvalue.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removeoverlaycollection.py
+-rw-rw-rw-   0        0        0      581 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removeparent.py
+-rw-rw-rw-   0        0        0      698 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removephysicsconstraint.py
+-rw-rw-rw-   0        0        0     1605 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/removevariable.py
+-rw-rw-rw-   0        0        0     1025 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/replacemesh.py
+-rw-rw-rw-   0        0        0      505 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/restartgame.py
+-rw-rw-rw-   0        0        0      547 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/resumesound.py
+-rw-rw-rw-   0        0        0      993 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/rotateto.py
+-rw-rw-rw-   0        0        0      910 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/runactuator.py
+-rw-rw-rw-   0        0        0     1855 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/runpython.py
+-rw-rw-rw-   0        0        0     7749 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savegame.py
+-rw-rw-rw-   0        0        0     1773 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savevariable.py
+-rw-rw-rw-   0        0        0     1512 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/savevariabledict.py
+-rw-rw-rw-   0        0        0     1016 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/sendmessage.py
+-rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/sendnetworkmessage.py
+-rw-rw-rw-   0        0        0     2243 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setactionframe.py
+-rw-rw-rw-   0        0        0      900 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setactuatorvalue.py
+-rw-rw-rw-   0        0        0     1097 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstraintattr.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstraintinfluence.py
+-rw-rw-rw-   0        0        0      970 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneconstrainttarget.py
+-rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setboneposition.py
+-rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcamera.py
+-rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcamerafov.py
+-rw-rw-rw-   0        0        0      640 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcameraorthoscale.py
+-rw-rw-rw-   0        0        0      829 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactergravity.py
+-rw-rw-rw-   0        0        0      742 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharacterjumpspeed.py
+-rw-rw-rw-   0        0        0      756 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactermaxjumps.py
+-rw-rw-rw-   0        0        0      871 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharactervelocity.py
+-rw-rw-rw-   0        0        0     1450 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcharacterwalkdir.py
+-rw-rw-rw-   0        0        0      773 2024-04-04 13:01:22.000000 uplogic-2.2/uplogic/nodes/actions/setcollisiongroup.py
+-rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcollisionmask.py
+-rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setconstraintattribute.py
+-rw-rw-rw-   0        0        0     1137 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcurvepoints.py
+-rw-rw-rw-   0        0        0      964 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setcustomcursor.py
+-rw-rw-rw-   0        0        0      860 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setdictkey.py
+-rw-rw-rw-   0        0        0      820 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setdynamics.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveeao.py
+-rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveebloom.py
+-rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveesmaa.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveesmaaquality.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveessr.py
+-rw-rw-rw-   0        0        0      705 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/seteeveevolumetrics.py
+-rw-rw-rw-   0        0        0      692 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setexposure.py
+-rw-rw-rw-   0        0        0      697 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setfilterstate.py
+-rw-rw-rw-   0        0        0      621 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setfullscreen.py
+-rw-rw-rw-   0        0        0     1681 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgameobjectattr.py
+-rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgamma.py
+-rw-rw-rw-   0        0        0      869 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setglobalvalue.py
+-rw-rw-rw-   0        0        0      612 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setgravity.py
+-rw-rw-rw-   0        0        0      778 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightcolor.py
+-rw-rw-rw-   0        0        0      724 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightenergy.py
+-rw-rw-rw-   0        0        0      744 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlightshadow.py
+-rw-rw-rw-   0        0        0      894 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setlistindex.py
+-rw-rw-rw-   0        0        0      783 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/actions/setlogictreeproperty.py
+-rw-rw-rw-   0        0        0     1052 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmaterial.py
+-rw-rw-rw-   0        0        0      989 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmatnodesocket.py
+-rw-rw-rw-   0        0        0     1182 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setmatnodevalue.py
+-rw-rw-rw-   0        0        0      956 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setnodesocket.py
+-rw-rw-rw-   0        0        0     1149 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setnodevalue.py
+-rw-rw-rw-   0        0        0      803 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setoverlaycollection.py
+-rw-rw-rw-   0        0        0      851 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setparent.py
+-rw-rw-rw-   0        0        0      837 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setphysics.py
+-rw-rw-rw-   0        0        0      604 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setprofile.py
+-rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setproperty.py
+-rw-rw-rw-   0        0        0      715 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setpyinstanceattr.py
+-rw-rw-rw-   0        0        0      663 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setresolution.py
+-rw-rw-rw-   0        0        0      746 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setrigidbody.py
+-rw-rw-rw-   0        0        0      633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setscene.py
+-rw-rw-rw-   0        0        0      965 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setsensorvalue.py
+-rw-rw-rw-   0        0        0      624 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/settimescale.py
+-rw-rw-rw-   0        0        0     2204 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setuiwidgetattr.py
+-rw-rw-rw-   0        0        0     2327 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setvisibility.py
+-rw-rw-rw-   0        0        0      546 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/setvsync.py
+-rw-rw-rw-   0        0        0      617 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/showframerate.py
+-rw-rw-rw-   0        0        0     1208 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/slowfollow.py
+-rw-rw-rw-   0        0        0     3973 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/spawnpool.py
+-rw-rw-rw-   0        0        0     5315 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound.py
+-rw-rw-rw-   0        0        0     1856 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound2d.py
+-rw-rw-rw-   0        0        0     2950 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsound3d.py
+-rw-rw-rw-   0        0        0     2464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startspeaker.py
+-rw-rw-rw-   0        0        0     1192 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/startsubnetwork.py
+-rw-rw-rw-   0        0        0     1161 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopaction.py
+-rw-rw-rw-   0        0        0      592 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopallsounds.py
+-rw-rw-rw-   0        0        0      543 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopsound.py
+-rw-rw-rw-   0        0        0      886 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/stopsubnetwork.py
+-rw-rw-rw-   0        0        0      611 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/togglefilter.py
+-rw-rw-rw-   0        0        0      815 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/toggleproperty.py
+-rw-rw-rw-   0        0        0      524 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/translate.py
+-rw-rw-rw-   0        0        0      992 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vectoranglecheck.py
+-rw-rw-rw-   0        0        0     1044 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplybraking.py
+-rw-rw-rw-   0        0        0     1037 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplyforce.py
+-rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehicleapplysteering.py
+-rw-rw-rw-   0        0        0     3133 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/actions/vehiclesetattributes.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.534111 uplogic-2.2/uplogic/nodes/conditions/
+-rw-rw-rw-   0        0        0     2026 2023-10-03 15:16:22.000000 uplogic-2.2/uplogic/nodes/conditions/__init__.py
+-rw-rw-rw-   0        0        0      880 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/barrier.py
+-rw-rw-rw-   0        0        0      826 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/checkdistance.py
+-rw-rw-rw-   0        0        0     4178 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/collision.py
+-rw-rw-rw-   0        0        0      823 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/compare.py
+-rw-rw-rw-   0        0        0     1165 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/comparevectors.py
+-rw-rw-rw-   0        0        0     2047 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/controllerstatus.py
+-rw-rw-rw-   0        0        0      898 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/evaluateproperty.py
+-rw-rw-rw-   0        0        0      739 2024-02-07 13:13:10.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadactive.py
+-rw-rw-rw-   0        0        0      708 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadbutton.py
+-rw-rw-rw-   0        0        0     1252 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/gamepadbuttonup.py
+-rw-rw-rw-   0        0        0      811 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/handleevent.py
+-rw-rw-rw-   0        0        0      637 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/hasproperty.py
+-rw-rw-rw-   0        0        0      311 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keyboardactive.py
+-rw-rw-rw-   0        0        0      615 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keypressed.py
+-rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/keyreleased.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicand.py
+-rw-rw-rw-   0        0        0      416 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicandnot.py
+-rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicgate.py
+-rw-rw-rw-   0        0        0      907 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicgatelist.py
+-rw-rw-rw-   0        0        0      314 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnone.py
+-rw-rw-rw-   0        0        0      332 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnot.py
+-rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicnotnone.py
+-rw-rw-rw-   0        0        0     1003 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logicor.py
+-rw-rw-rw-   0        0        0      962 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/logictreestatus.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousemoved.py
+-rw-rw-rw-   0        0        0     2881 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mouseover.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousepressed.py
+-rw-rw-rw-   0        0        0      940 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousepressedon.py
+-rw-rw-rw-   0        0        0      726 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousereleased.py
+-rw-rw-rw-   0        0        0      665 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/mousescroll.py
+-rw-rw-rw-   0        0        0      782 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/once.py
+-rw-rw-rw-   0        0        0      268 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/oninit.py
+-rw-rw-rw-   0        0        0      625 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onnexttick.py
+-rw-rw-rw-   0        0        0      243 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onupdate.py
+-rw-rw-rw-   0        0        0      974 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onvaluechanged.py
+-rw-rw-rw-   0        0        0      772 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/onvaluechangedto.py
+-rw-rw-rw-   0        0        0      854 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/pulsify.py
+-rw-rw-rw-   0        0        0      454 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/sensorpositive.py
+-rw-rw-rw-   0        0        0      845 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/timedelay.py
+-rw-rw-rw-   0        0        0      901 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/timer.py
+-rw-rw-rw-   0        0        0      451 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/truefalse.py
+-rw-rw-rw-   0        0        0      389 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/valuevalid.py
+-rw-rw-rw-   0        0        0     1001 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/conditions/vectoranglecheck.py
+-rw-rw-rw-   0        0        0     5388 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/nodes/logictree.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.563014 uplogic-2.2/uplogic/nodes/parameters/
+-rw-rw-rw-   0        0        0     5254 2024-04-04 13:03:49.000000 uplogic-2.2/uplogic/nodes/parameters/__init__.py
+-rw-rw-rw-   0        0        0      392 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/absolutevalue.py
+-rw-rw-rw-   0        0        0     1392 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/actionstatus.py
+-rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/activecamera.py
+-rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/axisvector.py
+-rw-rw-rw-   0        0        0     1694 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/bonestatus.py
+-rw-rw-rw-   0        0        0     1521 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/characterinfo.py
+-rw-rw-rw-   0        0        0      559 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/childbyindex.py
+-rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/childbyname.py
+-rw-rw-rw-   0        0        0      834 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/clamp.py
+-rw-rw-rw-   0        0        0      394 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/colorrgb.py
+-rw-rw-rw-   0        0        0      395 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/colorrgba.py
+-rw-rw-rw-   0        0        0      437 2024-02-18 16:30:58.000000 uplogic-2.2/uplogic/nodes/parameters/curveinterpolation.py
+-rw-rw-rw-   0        0        0      565 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/dictvalue.py
+-rw-rw-rw-   0        0        0      465 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/distance.py
+-rw-rw-rw-   0        0        0      602 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/euler.py
+-rw-rw-rw-   0        0        0      553 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/eulertomatrix.py
+-rw-rw-rw-   0        0        0      732 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/formattedstring.py
+-rw-rw-rw-   0        0        0     1919 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/formula.py
+-rw-rw-rw-   0        0        0      324 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/fpsfactor.py
+-rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gamepadsticks.py
+-rw-rw-rw-   0        0        0     1480 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gamepadtrigger.py
+-rw-rw-rw-   0        0        0      610 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getactuatorvalue.py
+-rw-rw-rw-   0        0        0      323 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollection.py
+-rw-rw-rw-   0        0        0      464 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollectionobjectnames.py
+-rw-rw-rw-   0        0        0      529 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcollectionobjects.py
+-rw-rw-rw-   0        0        0      434 2024-04-04 13:03:32.000000 uplogic-2.2/uplogic/nodes/parameters/getcollisiongroup.py
+-rw-rw-rw-   0        0        0      582 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getcurvepoints.py
+-rw-rw-rw-   0        0        0      295 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getfont.py
+-rw-rw-rw-   0        0        0      306 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getfullscreen.py
+-rw-rw-rw-   0        0        0      562 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getglobalvalue.py
+-rw-rw-rw-   0        0        0      337 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getgravity.py
+-rw-rw-rw-   0        0        0      298 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getimage.py
+-rw-rw-rw-   0        0        0      398 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getlightcolor.py
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getlightenergy.py
+-rw-rw-rw-   0        0        0      660 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getlogictreeproperty.py
+-rw-rw-rw-   0        0        0      805 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getnodeattribute.py
+-rw-rw-rw-   0        0        0      659 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getnodesocket.py
+-rw-rw-rw-   0        0        0      369 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getobject.py
+-rw-rw-rw-   0        0        0      284 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getowner.py
+-rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getparent.py
+-rw-rw-rw-   0        0        0      837 2024-01-22 11:02:02.000000 uplogic-2.2/uplogic/nodes/parameters/getproperty.py
+-rw-rw-rw-   0        0        0      429 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getpyinstanceattr.py
+-rw-rw-rw-   0        0        0      661 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getresolution.py
+-rw-rw-rw-   0        0        0      289 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getscene.py
+-rw-rw-rw-   0        0        0      600 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getsensorvalue.py
+-rw-rw-rw-   0        0        0      296 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getsound.py
+-rw-rw-rw-   0        0        0      290 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/gettimescale.py
+-rw-rw-rw-   0        0        0      825 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getuiwidgetattr.py
+-rw-rw-rw-   0        0        0      286 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/getvsync.py
+-rw-rw-rw-   0        0        0      334 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initemptydict.py
+-rw-rw-rw-   0        0        0      414 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initemptylist.py
+-rw-rw-rw-   0        0        0      396 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/initnewdict.py
+-rw-rw-rw-   0        0        0      856 2024-02-09 10:13:40.000000 uplogic-2.2/uplogic/nodes/parameters/instream.py
+-rw-rw-rw-   0        0        0      478 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/interpolate.py
+-rw-rw-rw-   0        0        0      404 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/invertvalue.py
+-rw-rw-rw-   0        0        0      299 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/nodes/parameters/keycode.py
+-rw-rw-rw-   0        0        0     1232 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/limitrange.py
+-rw-rw-rw-   0        0        0      343 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listduplicate.py
+-rw-rw-rw-   0        0        0      527 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listextend.py
+-rw-rw-rw-   0        0        0      327 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listfromitems.py
+-rw-rw-rw-   0        0        0      461 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listindex.py
+-rw-rw-rw-   0        0        0      447 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/listindexrandom.py
+-rw-rw-rw-   0        0        0     1466 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/loadvariable.py
+-rw-rw-rw-   0        0        0     1175 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/loadvariabledict.py
+-rw-rw-rw-   0        0        0      831 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/maprange.py
+-rw-rw-rw-   0        0        0      853 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetattribute.py
+-rw-rw-rw-   0        0        0      556 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetnode.py
+-rw-rw-rw-   0        0        0      693 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/materialgetsocket.py
+-rw-rw-rw-   0        0        0     1673 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/math.py
+-rw-rw-rw-   0        0        0      568 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/matrixtoxyz.py
+-rw-rw-rw-   0        0        0     1045 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/mousedata.py
+-rw-rw-rw-   0        0        0      657 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectattr.py
+-rw-rw-rw-   0        0        0      352 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectdataname.py
+-rw-rw-rw-   0        0        0      584 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/objectdatavertices.py
+-rw-rw-rw-   0        0        0      741 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomfloat.py
+-rw-rw-rw-   0        0        0      690 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomint.py
+-rw-rw-rw-   0        0        0     1722 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomvalue.py
+-rw-rw-rw-   0        0        0      639 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/randomvect.py
+-rw-rw-rw-   0        0        0      929 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rangedthreshold.py
+-rw-rw-rw-   0        0        0     1522 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rebuilddata.py
+-rw-rw-rw-   0        0        0      867 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/resizevector.py
+-rw-rw-rw-   0        0        0     1930 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/rotatebypoint.py
+-rw-rw-rw-   0        0        0      462 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/screenposition.py
+-rw-rw-rw-   0        0        0      734 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/serializedata.py
+-rw-rw-rw-   0        0        0      322 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/simplevalue.py
+-rw-rw-rw-   0        0        0      930 2024-04-04 13:47:56.000000 uplogic-2.2/uplogic/nodes/parameters/storevalue.py
+-rw-rw-rw-   0        0        0      758 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/threshold.py
+-rw-rw-rw-   0        0        0      885 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/timedata.py
+-rw-rw-rw-   0        0        0     3026 2024-02-19 17:25:02.000000 uplogic-2.2/uplogic/nodes/parameters/tweenvalue.py
+-rw-rw-rw-   0        0        0      685 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/typecastvalue.py
+-rw-rw-rw-   0        0        0     4193 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/valueswitch.py
+-rw-rw-rw-   0        0        0      502 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorabsolute.py
+-rw-rw-rw-   0        0        0      587 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorangle.py
+-rw-rw-rw-   0        0        0       60 2023-09-30 12:04:19.000000 uplogic-2.2/uplogic/nodes/parameters/vectoranglecheck.py
+-rw-rw-rw-   0        0        0      378 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorlength.py
+-rw-rw-rw-   0        0        0     4632 2024-04-23 15:15:14.000000 uplogic-2.2/uplogic/nodes/parameters/vectormath.py
+-rw-rw-rw-   0        0        0      578 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorsplitxy.py
+-rw-rw-rw-   0        0        0      686 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorsplitxyz.py
+-rw-rw-rw-   0        0        0      439 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxy.py
+-rw-rw-rw-   0        0        0      514 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxyz.py
+-rw-rw-rw-   0        0        0      585 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vectorxyzw.py
+-rw-rw-rw-   0        0        0     1273 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vrcontrollervalues.py
+-rw-rw-rw-   0        0        0      486 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/vrheadsetvalues.py
+-rw-rw-rw-   0        0        0      923 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/withinrange.py
+-rw-rw-rw-   0        0        0      731 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/nodes/parameters/worldposition.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.565008 uplogic-2.2/uplogic/physics/
+-rw-rw-rw-   0        0        0      540 2023-03-06 11:18:24.000000 uplogic-2.2/uplogic/physics/__init__.py
+-rw-rw-rw-   0        0        0     4164 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/physics/buoyancy.py
+-rw-rw-rw-   0        0        0     4060 2024-03-22 08:57:02.000000 uplogic-2.2/uplogic/physics/character.py
+-rw-rw-rw-   0        0        0     3595 2023-11-06 03:14:00.000000 uplogic-2.2/uplogic/physics/collision.py
+-rw-rw-rw-   0        0        0     8370 2024-02-06 12:40:32.000000 uplogic-2.2/uplogic/physics/constraints.py
+-rw-rw-rw-   0        0        0    10164 2024-01-25 16:38:46.000000 uplogic-2.2/uplogic/physics/vehicle.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.565008 uplogic-2.2/uplogic/serialize/
+-rw-rw-rw-   0        0        0     2965 2023-12-11 16:15:51.000000 uplogic-2.2/uplogic/serialize/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.584942 uplogic-2.2/uplogic/shaders/
+-rw-rw-rw-   0        0        0      795 2024-04-23 15:16:36.000000 uplogic-2.2/uplogic/shaders/__init__.py
+-rw-rw-rw-   0        0        0      872 2023-04-01 06:53:25.000000 uplogic-2.2/uplogic/shaders/adaptivetonemapping.py
+-rw-rw-rw-   0        0        0     1633 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/blur.py
+-rw-rw-rw-   0        0        0      685 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/brightness.py
+-rw-rw-rw-   0        0        0     1182 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/shaders/buffer.py
+-rw-rw-rw-   0        0        0     1070 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/chromaticaberration.py
+-rw-rw-rw-   0        0        0     7049 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/distort.py
+-rw-rw-rw-   0        0        0     9821 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/dof.py
+-rw-rw-rw-   0        0        0     9068 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/droplets.py
+-rw-rw-rw-   0        0        0       10 2024-02-21 19:10:36.000000 uplogic-2.2/uplogic/shaders/filtersystem.py
+-rw-rw-rw-   0        0        0    33422 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/fxaa.py
+-rw-rw-rw-   0        0        0      916 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/grayscale.py
+-rw-rw-rw-   0        0        0     9683 2023-07-05 14:45:48.000000 uplogic-2.2/uplogic/shaders/hbao.py
+-rw-rw-rw-   0        0        0     1035 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/lens.py
+-rw-rw-rw-   0        0        0     1137 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/letterbox.py
+-rw-rw-rw-   0        0        0     1027 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/levels.py
+-rw-rw-rw-   0        0        0     4172 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/mist.py
+-rw-rw-rw-   0        0        0     1779 2024-02-12 11:42:26.000000 uplogic-2.2/uplogic/shaders/rendertoscreen.py
+-rw-rw-rw-   0        0        0     5818 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/shader.py
+-rw-rw-rw-   0        0        0     2268 2023-04-01 06:54:25.000000 uplogic-2.2/uplogic/shaders/sharpen.py
+-rw-rw-rw-   0        0        0     2898 2024-02-12 11:42:41.000000 uplogic-2.2/uplogic/shaders/splitscreen.py
+-rw-rw-rw-   0        0        0     5754 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/ssao.py
+-rw-rw-rw-   0        0        0     2373 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/shaders/texture.py
+-rw-rw-rw-   0        0        0     1189 2024-02-12 15:10:32.000000 uplogic-2.2/uplogic/shaders/vignette.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.592914 uplogic-2.2/uplogic/ui/
+-rw-rw-rw-   0        0        0      653 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/__init__.py
+-rw-rw-rw-   0        0        0     1712 2024-02-16 10:02:44.000000 uplogic-2.2/uplogic/ui/behaviors.py
+-rw-rw-rw-   0        0        0    10061 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/button.py
+-rw-rw-rw-   0        0        0     1722 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/camera.py
+-rw-rw-rw-   0        0        0     3577 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/canvas.py
+-rw-rw-rw-   0        0        0     3765 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/cursor.py
+-rw-rw-rw-   0        0        0     7177 2024-04-04 12:19:18.000000 uplogic-2.2/uplogic/ui/image.py
+-rw-rw-rw-   0        0        0     8118 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/ui/label.py
+-rw-rw-rw-   0        0        0    13537 2024-04-04 03:21:32.000000 uplogic-2.2/uplogic/ui/layout.py
+-rw-rw-rw-   0        0        0     5166 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/path.py
+-rw-rw-rw-   0        0        0     2041 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/render.py
+-rw-rw-rw-   0        0        0     8061 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/ui/slider.py
+-rw-rw-rw-   0        0        0     8690 2024-04-23 18:12:22.000000 uplogic-2.2/uplogic/ui/textinput.py
+-rw-rw-rw-   0        0        0    16519 2024-04-16 09:39:46.000000 uplogic-2.2/uplogic/ui/widget.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.600888 uplogic-2.2/uplogic/utils/
+-rw-rw-rw-   0        0        0     7473 2024-04-04 03:20:50.000000 uplogic-2.2/uplogic/utils/__init__.py
+-rw-rw-rw-   0        0        0     1642 2023-11-09 02:27:44.000000 uplogic-2.2/uplogic/utils/constants.py
+-rw-rw-rw-   0        0        0     1089 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/utils/engine.py
+-rw-rw-rw-   0        0        0      854 2022-09-08 15:54:10.000000 uplogic-2.2/uplogic/utils/errors.py
+-rw-rw-rw-   0        0        0     4650 2023-11-22 09:34:56.000000 uplogic-2.2/uplogic/utils/lights.py
+-rw-rw-rw-   0        0        0    11028 2024-04-04 03:23:58.000000 uplogic-2.2/uplogic/utils/math.py
+-rw-rw-rw-   0        0        0     4801 2023-12-31 14:36:53.000000 uplogic-2.2/uplogic/utils/nodetrees.py
+-rw-rw-rw-   0        0        0    17010 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/utils/objects.py
+-rw-rw-rw-   0        0        0    10075 2023-11-09 14:18:13.000000 uplogic-2.2/uplogic/utils/pooling.py
+-rw-rw-rw-   0        0        0    13778 2023-10-13 21:24:56.000000 uplogic-2.2/uplogic/utils/raycasting.py
+-rw-rw-rw-   0        0        0     6451 2024-03-18 08:04:37.000000 uplogic-2.2/uplogic/utils/scene.py
+-rw-rw-rw-   0        0        0     3528 2024-03-18 12:51:09.000000 uplogic-2.2/uplogic/utils/visualize.py
+-rw-rw-rw-   0        0        0     2553 2024-03-22 08:50:05.000000 uplogic-2.2/uplogic/utils/visuals.py
+drwxrwxrwx   0        0        0        0 2024-04-23 18:17:52.454378 uplogic-2.2/uplogic.egg-info/
+-rw-rw-rw-   0        0        0     1045 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    14795 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-23 18:17:52.000000 uplogic-2.2/uplogic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2022-03-17 18:28:53.000000 uplogic-2.2/uplogic.egg-info/zip-safe
```

### Comparing `uplogic-2.1/PKG-INFO` & `uplogic-2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 2.1
+Version: 2.2
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.1.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-2.1/setup.py` & `uplogic-2.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = 'v2.1'
+version = 'v2.2'
 shortdesc = "Uplogic utility for UPBGE."
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.md',
     'LICENSE.md'
 ]])
 
 
@@ -27,25 +27,25 @@
         'Topic :: Multimedia :: Graphics',
         'Programming Language :: Python',
     ],
     keywords='Blender UPBGE logic',
     author='Leopold Auersperg-Castell',
     author_email='lauersperg@gmx.at',
     url='https://github.com/UPBGE/uplogic',
-    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v2.1.tar.gz',
+    download_url='https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz',
     license='GPLv2',
     packages=[
         'uplogic',
         'uplogic.animation',
         'uplogic.audio',
         'uplogic.data',
         'uplogic.decorators',
         'uplogic.events',
         'uplogic.input',
-        'uplogic.logging',
+        'uplogic.console',
         'uplogic.network',
         'uplogic.nodes',
         'uplogic.nodes.actions',
         'uplogic.nodes.conditions',
         'uplogic.nodes.parameters',
         'uplogic.physics',
         'uplogic.serialize',
```

### Comparing `uplogic-2.1/uplogic/__init__.py` & `uplogic-2.2/uplogic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,20 +59,20 @@
 """
 
 from collections import deque
 
 from .utils import load_user_module
 from .utils import make_valid_name
 from .input import key_tap
-from .logging import enable
+from .console import enable
 from . import animation
 from . import audio
 from . import events
 from . import input
-from . import logging
+from . import console
 from . import network
 from . import physics
 from . import shaders
 from . import ui
 from . import utils
 import bge
 import bpy
@@ -247,8 +247,8 @@
         pass
 
     def shutdown(self):
         get_mainloop().stop()
 
 
 class ULLoop(CustomLoop):
-    pass
+    pass
```

### Comparing `uplogic-2.1/uplogic/animation/action.py` & `uplogic-2.2/uplogic/animation/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,18 +37,16 @@
         self.action = action
         self.frame = frame
         self.callback = callback
         self.consumed = False
         self.args = args
 
 
-class ULAction():
+class Action():
     '''
-    [DEPRECATED] Use `uplogic.animation.Action` instead.
-
     Wrapper class for animated actions that provides additional parameters
     and quick access properties.
 
     :param `game_object`: The `KX_GameObject` on which to play the action.
     :param `action_name`: The name of the action  of `bpy.data.actions`.
     :param `start_frame`: The first frame of the action.
     :param `end_frame`: The last frame of the action.
@@ -63,15 +61,15 @@
     animations on different layers together.
     :param `blend_mode`: Mode of blending of [`'blend'`, `'add'`]
     :param `keep`: Whether to keep the animation cached after playback has
     finished. This is useful for setting animation frames regardless of the
     action state.
     '''
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         game_object: GameObject,
         action_name: str,
         start_frame: int = 0,
         end_frame: int = 250,
@@ -194,14 +192,16 @@
         '''Intensity of the animation. Higher layers can be blended over lower
         ones.'''
         return self._intensity
 
     @intensity.setter
     def intensity(self, value: float):
         value = float(value)
+        if not value:
+            self.game_object.stopAction(self.layer)
         if not self.is_playing:
             return
         if not self.is_playing or value == self._intensity:
             return
         self._intensity = clamp(value, 0, 1)
         self._restart_action()
 
@@ -330,14 +330,17 @@
         '''Resume this action from pause.
         '''
         if self._frozen_speed >= 0:
             self.speed = self._frozen_speed
             self._frozen_speed = -1
 
     def stop(self):
+        self._act_system.remove(self)
+
+    def _stop(self):
         '''Stop playback of this action.
         '''
         self.stopped = True
         self.on_finish()
         self.game_object.stopAction(self.layer)
 
     def restart(self):
@@ -381,16 +384,19 @@
         self.speed = min + (delta * random())
 
     def set_frame(self, frame: float):
         '''Set the frame of this action.
         '''
         self.frame = frame
 
-class Action(ULAction):
-    '''Wrapper class for animated actions that provides additional parameters
+class ULAction(Action):
+    '''
+    [DEPRECATED] Use `uplogic.animation.Action` instead.
+
+    Wrapper class for animated actions that provides additional parameters
     and quick access properties.
 
     :param `game_object`: The `KX_GameObject` on which to play the action.
     :param `action_name`: The name of the action  of `bpy.data.actions`.
     :param `start_frame`: The first frame of the action.
     :param `end_frame`: The last frame of the action.
     :param `layer`: The layer on which to play the action. Leave at -1 for
@@ -402,9 +408,8 @@
     :param `speed`: Playback speed.
     :param `intensity`: "Intensity" of the action; Use this to blend
     animations on different layers together.
     :param `blend_mode`: Mode of blending of [`'blend'`, `'add'`]
     :param `keep`: Whether to keep the animation cached after playback has
     finished. This is useful for setting animation frames regardless of the
     action state.'''
-    _deprecated = False
-    pass
+    _deprecated = True
```

### Comparing `uplogic-2.1/uplogic/animation/actionsystem.py` & `uplogic-2.2/uplogic/animation/actionsystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         ActionSystem.lock_layer(action)
 
     def remove(self, action):
         '''Remove a `Action` from this system.
 
         :param `action`: `Action` which to remove.
         '''
-        action.stop()
+        action._stop()
         if action in self.actions:
             self.actions.remove(action)
         ActionSystem.free_layer(action)
 
     def shutdown(self):
         '''Shutdown and remove this action system. This will stop all actions
         playing in this system.'''
```

### Comparing `uplogic-2.1/uplogic/animation/rig.py` & `uplogic-2.2/uplogic/animation/rig.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/animation/sequence.py` & `uplogic-2.2/uplogic/animation/sequence.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,14 @@
                 if frame + s > end_frame:
                     if play_mode == 1:
                         leftover = frame + s - end_frame
                         span = end_frame - start_frame
                         while leftover > span:
                             leftover -= span
                         self.frame = start_frame + leftover
-                        print('Restart')
                     else:
                         self.frame = end_frame
                 else:
                     self.frame += s
         elif play_mode == 1:
             self.frame = end_frame if inverted else start_frame
         elif play_mode == 2:
```

### Comparing `uplogic-2.1/uplogic/audio/__init__.py` & `uplogic-2.2/uplogic/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/audio/audiosystem.py` & `uplogic-2.2/uplogic/audio/audiosystem.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/audio/music.py` & `uplogic-2.2/uplogic/audio/music.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/audio/sound.py` & `uplogic-2.2/uplogic/audio/sound.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,16 @@
                 occluder, point, normal = cam.rayCast(
                     location,
                     cam.worldPosition,
                     xray=False
                 )
                 occluded = self.occluded = False
                 penetration = 1
-                while occluder:
+                occ_count = 0
+                while occluder and occ_count < 5:
                     if occluder is speaker:
                         break
                     sound_occluder = occluder.blenderObject.get(
                         'sound_occluder',
                         True
                     )
                     if sound_occluder:
@@ -491,14 +492,15 @@
                         else:
                             penetration = 0
                     occluder, point, normal = occluder.rayCast(
                         location,
                         point,
                         xray=False
                     )
+                    occ_count += 1
                 cs = self._clear_sound
                 if occluded and cs > 0:
                     self._clear_sound -= transition
                 elif not occluded and cs < 1:
                     self._clear_sound += transition
                 if self._clear_sound < 0:
                     self._clear_sound = 0
```

### Comparing `uplogic-2.1/uplogic/data/__init__.py` & `uplogic-2.2/uplogic/data/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/data/file.py` & `uplogic-2.2/uplogic/data/file.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/data/globaldb.py` & `uplogic-2.2/uplogic/data/globaldb.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from bge import logic
 import bpy
 import os
 from uplogic.utils import unload_nodes
 
 
 class GlobalDB(object):
-    '''TODO: Documentation
+    '''Global Databank. Offers methods for storing and retrieving values akin to `bge.logic.globalDict`.
+    Values stored in this databank are available as long as the python interpreter runs and can be made permanent.
     '''
     index: int
     initialized: bool = False
 
     class LineBuffer(object):
         def __init__(self, buffer=[]):
             self.buffer = buffer
@@ -209,18 +210,18 @@
 
     def log(self):
         '''TODO: Documentation
         '''
         print(self.content)
 
 
-def store(key, value, category='uplogic.default_globals'):
+def store(key, value, category='uplogic.default_globals', persist=False):
     initialize()
     values = GlobalDB.retrieve(category)
-    values.put(key, value)
+    values.put(key, value, persist)
 
 
 def retrieve(key, category='uplogic.default_globals', default=None):
     initialize()
     values = GlobalDB.retrieve(category)
     return values.get(key, default)
```

### Comparing `uplogic-2.1/uplogic/data/serializers.py` & `uplogic-2.2/uplogic/data/serializers.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/decorators/__init__.py` & `uplogic-2.2/uplogic/decorators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
             setattr(cls, game_prop, prop)
             if not hasattr(cls, f'on_{game_prop}'):
                 setattr(cls, f'on_{game_prop}', on_attr)
         return cls
     return deco
 
 
-def instance_props(*prop_names) -> KX_PythonComponent:
+def instance_property(*prop_names) -> KX_PythonComponent:
     """Decorator for `KX_PythonComponent` or `KX_GameObject` classes and subclasses.
 
     Automatically adds property handlers for this class to use the `game_object.GroupObject[prop]`
     syntax instead of saving values on the instance itself.
 
     :param `prop_names`: Names of game properties as a list.
     """
```

### Comparing `uplogic-2.1/uplogic/events/__init__.py` & `uplogic-2.2/uplogic/events/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,35 +3,35 @@
 
 from bge import logic
 import time
 from uplogic.physics import on_collision  # noqa
 
 
 def on_pre_draw(callback):
-    ULEventManager.update_on.append(callback)
+    EventManager.update_on.append(callback)
 
 
 def on_post_draw(callback):
-    ULEventManager.update_on.append(callback)
+    EventManager.update_on.append(callback)
 
 
 def get_event_manager():
-    update = ULEventManager.update_on
+    update = EventManager.update_on
     if update is None:
         update = logic.getCurrentScene().post_draw
-    if ULEventManager.update not in update:
-        update.append(ULEventManager.update)
-    return ULEventManager
+    if EventManager.update not in update:
+        update.append(EventManager.update)
+    return EventManager
 
 
 def set_update_loop(loop):
-    ULEventManager.set_update_on(loop)
+    EventManager.set_update_on(loop)
 
 
-class ULEventManager():
+class EventManager():
     '''Manager for `ULEvent` objects, not inteded for manual use.
     '''
     events = {}
     callbacks = []
     done = []
 
     update_on = None
@@ -124,78 +124,78 @@
     :param `messenger`: Can be used to store an object.
     '''
 
     def __init__(self, id: int, content=None, messenger=None):
         self.id = id
         self.content = content
         self.messenger = messenger
-        ULEventManager.schedule(self.register)
+        EventManager.schedule(self.register)
 
     def register(self):
-        ULEventManager.register(self)
-        ULEventManager.cancel(self.register)
+        EventManager.register(self)
+        EventManager.cancel(self.register)
 
     def remove(self):
-        ULEventManager.events.pop(self.id, None)
-        ULEventManager.cancel(self.remove)
+        EventManager.events.pop(self.id, None)
+        EventManager.cancel(self.remove)
 
 
 def send(id: int, content=None, messenger=None) -> None:
     '''Send an event that can be reacted to.
 
     :param `id`: Identifier of the event; can be anything, not just `int`.
     :param `content`: This can be used to store data in an event.
     :param `messenger`: Can be used to store an object.
     '''
-    ULEventManager.send(id, content, messenger)
+    EventManager.send(id, content, messenger)
 
 
 def receive(id) -> ULEvent:
     '''Check if an event has occured.
 
     :param `id`: Identifier of the event; can be anything, not just `str`.
 
     :returns: `ULEvent` with `id`, `content` and `messenger` as attributes.
     '''
-    return ULEventManager.receive(id)
+    return EventManager.receive(id)
 
 
 def consume(id: int):
     '''Check if an event has occured. This will remove the event.
 
     :param `id`: Identifier of the event; can be anything, not just `str`.
 
     :returns: `ULEvent` with `id`, `content` and `messenger` as attributes.
     '''
-    return ULEventManager.consume(id, None)
+    return EventManager.consume(id, None)
 
 
 def bind(id: int, callback) -> None:
     '''Bind a callback to an event.
 
     :param `id`: Name of the event; can be anything, not just `str`.
     :param `callback`: This callback will be called every time the event is
     triggered.
     '''
     class BoundCallback():
         def __init__(self, id, cb) -> None:
             self.id = id
             self.callback = cb
-            ULEventManager.bind(self._check_evt)
+            EventManager.bind(self._check_evt)
 
         def _check_evt(self):
             evt = receive(self.id)
             if evt:
                 self.callback(evt)
 
         def unbind(self):
-            ULEventManager.unbind(self._check_evt)
+            EventManager.unbind(self._check_evt)
 
         def release(self):
-            ULEventManager.unbind(self._check_evt)
+            EventManager.unbind(self._check_evt)
 
     return BoundCallback(id, callback)
 
 
 class ScheduledEvent():
     '''Event generated by `uplogic.events.schedule()`.
 
@@ -208,28 +208,28 @@
     def __init__(self, delay, id, content, messenger):
         self.time = time.time()
         self.delay = self.time + delay
         self.id = id
         self.content = content
         self.messenger = messenger
         self._consumed = False
-        ULEventManager.schedule(self._send_scheduled)
+        EventManager.schedule(self._send_scheduled)
 
     def _send_scheduled(self):
         if time.time() >= self.delay:
             self.consume()
 
     def cancel(self):
-        ULEventManager.cancel(self._send_scheduled)
+        EventManager.cancel(self._send_scheduled)
 
     def consume(self):
         if self._consumed:
             return
         self._consumed = True
-        ULEventManager.cancel(self._send_scheduled)
+        EventManager.cancel(self._send_scheduled)
         ULEvent(self.id, self.content, self.messenger)
 
 
 def schedule(id: str, delay=0.0, content=None, messenger=None) -> ScheduledEvent:
     '''Send an event that can be reacted to with a delay.
 
     :param `id`: Name of the event; can be anything, not just `str`. If `id` is callable, `content` can be used as argument.
@@ -255,32 +255,32 @@
 
     def __init__(self, cb, delay=0.0, arg=None):
         self.time = time.time()
         self.delay = self.time + delay
         self.callback = cb
         self.arg = arg
         self._consumed = False
-        ULEventManager.schedule(self._call_scheduled)
+        EventManager.schedule(self._call_scheduled)
 
     def _call_scheduled(self):
         if time.time() >= self.delay:
             self.consume()
 
     def consume(self):
         if self._consumed:
             return
         self._consumed = True
-        ULEventManager.cancel(self._call_scheduled)
+        EventManager.cancel(self._call_scheduled)
         if self.arg is not None:
             self.callback(self.arg)
         else:
             self.callback()
 
     def cancel(self):
-        ULEventManager.cancel(self._call_scheduled)
+        EventManager.cancel(self._call_scheduled)
 
 
 def schedule_callback(cb, delay=0.0, arg=None) -> ScheduledCallback:
     '''Call a function with a delay. The function can have an argument when
     defined as a keyword.
 
     Callback cannot return anything.
```

### Comparing `uplogic-2.1/uplogic/input/__init__.py` & `uplogic-2.2/uplogic/input/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/input/gamepad.py` & `uplogic-2.2/uplogic/input/gamepad.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,14 +165,18 @@
     :param stick: which stick to use.
     can bei either `LS` or `RS` from `uplogic.input`.
     :param idx: gamepad index (default = 0).
     :param threshold: minimum value for each axis to be valid.
 
     :returns: set `(x, y)`
     '''
+    if stick == 'LS':
+        stick = LS
+    elif stick == 'RS':
+        stick = RS
     xaxis = STICKS[stick][0]
     yaxis = STICKS[stick][1]
     return Vector((
         gamepad_axis(xaxis, idx, threshold=threshold) * (-1 if invert[0] else 1),
         gamepad_axis(yaxis, idx, threshold=threshold) * (-1 if invert[1] else 1)
     ))
 
@@ -251,64 +255,67 @@
     joystick.strengthLeft = strength[0]
     joystick.strengthRight = strength[1]
     joystick.duration = int(round(time * 1000))
 
     joystick.startVibration()
 
 
-class ULGamePad():
-    """Wrapper class for a controller. The index determines which connected
+class Gamepad():
+    """Wrapper class for a gamepad/controller. The index determines which connected
     gamepad to use, the layout determines whether to use XBox or Sony button
     naming.
     
     :param `idx`: Which gamepad to use.
     :param `layout`: Layout determining button names; `str` in [`'XBOX'`,
     `'SONY'`].
     """
 
-    _deprecated = True
+    _deprecated = False
 
     def __init__(
         self,
         idx: int = 0,
         layout: dict = XBOX
     ) -> None:
         if self._deprecated:
             print('Warning: ULGamePad class will be renamed to "Gamepad" in future releases!')
         self.idx = idx
         self.layout = layout
         if not logic.joysticks[idx]:
             print(f'No Joystick found at index: {idx}')
-        self.joystick = logic.joysticks[idx]
+        self.device = logic.joysticks[idx]
 
     def button_down(self, button: str):
         return gamepad_down(button, self.idx, self.layout)
         
     def button_tap(self, button: str):
         return gamepad_tap(button, self.idx, self.layout)
 
     def button_up(self, button: str):
         return gamepad_up(button, self.idx, self.layout)
 
     def sticks(self, stick: str = LS, threshold: float = 0.07):
         return gamepad_stick(stick, self.idx, threshold)
     
-    def vibrate(self, strength: tuple = (.5, .5), time: float = 1.0):
-        if not self.joystick.hasVibration:
+    def rumble(self, strength: tuple = (.5, .5), time: float = 1.0):
+        if not self.device.hasVibration:
             print('Joystick at index {} has no vibration!'.format(self.idx))
             return
-        self.joystick.strengthLeft = strength[0]
-        self.joystick.strengthRight = strength[1]
-        self.joystick.duration = int(round(time * 1000))
+        self.device.strengthLeft = strength[0]
+        self.device.strengthRight = strength[1]
+        self.device.duration = int(round(time * 1000))
 
-        self.joystick.startVibration()
+        self.device.startVibration()
 
+    def vibrate(self, strength: tuple = (.5, .5), time: float = 1.0):
+        self.rumble(strength, time)
 
-class Gamepad(ULGamePad):
-    _deprecated = False
+
+class ULGamePad(Gamepad):
+    _deprecated = True
 
 
 class ULGamepadLook():
     """Automatically track the mouse movement and translate it to a rotate a
     body and optionally a head.
 
     This component can be activated/deactivated at any time to keep performance
```

### Comparing `uplogic-2.1/uplogic/input/keyboard.py` & `uplogic-2.2/uplogic/input/keyboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from bge import logic
 from bge import events
+from bge.types import SCA_InputEvent
 
 
 KEYBOARD_EVENTS = logic.keyboard.inputs
 '''Reference to `bge.logic.keyboard.inputs`
 '''
 
 _keys_active = {}
 
 
-def key_event(key: str) -> bool:
+def key_event(key: str) -> SCA_InputEvent:
     '''Retrieve key event.\n
     Not intended for manual use.
     '''
     if isinstance(key, int):
         key = KEYBOARD_EVENTS[key]
     else:
         key = KEYBOARD_EVENTS[
@@ -153,41 +154,66 @@
     `'BACKSPACE'`, `'COMMA'`, `'DEL'`, `'END'`, `'EQUAL'`, `'ESC'`, `'HOME'`, `'INSERT'`, `'LEFTBRACKET'`, `'RIGHTBRACKET'`,
     `'LINEFEED'`, `'MINUS'`, `'PAGEDOWN'`, `'PAGEUP'`, `'PAUSE'`, `'PERIOD'`, `'QUOTE'`, `'RET'`, `'ENTER'`, `'SEMICOLON'`,
     `'SLASH'`, `'SPACE'`, `'TAB'`]
     :param time: timeout for key down
 
     :returns: boolean
     '''
-    if key_event(key).activated:
+    evt = key_event(key)
+    if evt.activated:
         _keys_active[key] = 0
         return True
     k = _keys_active.get(key, 0)
     _keys_active[key] = k + (1 / (logic.getAverageFrameRate() or 0.01))
     if _keys_active[key] > time:
-        return key_event(key).active
+        return evt.active
     return False
 
 
-def record_keyboard(all=False) -> tuple[bool, int, str]:
-    '''Listen to keyboard actions
-    :returns: Tuple of `(pressed, keycode, character)`'''
+class RecordedCharacter(tuple):
+
+    @property
+    def pressed(self):
+        return self[0]
+
+    @property
+    def keycode(self):
+        return self[1]
+
+    @property
+    def character(self):
+        return self[2]
+
+
+def record_keyboard(down=True, all=False) -> RecordedCharacter[bool, int, str]:
+    '''Listen to keyboard events.
+
+    :param `down`: Record if key is down.
+    :param `all`: Record non-character keys.
+
+    :returns: List of tuples of `(pressed, keycode, character)`'''
     left_shift = KEYBOARD_EVENTS[events.LEFTSHIFTKEY].active
     right_shift = KEYBOARD_EVENTS[events.RIGHTSHIFTKEY].active
     active_events = logic.keyboard.activeInputs.copy()
 
+    func = key_down if down else key_pulse
+
+    evts = []
+
     for keycode in active_events:
-        if key_pulse(keycode):
+        if func(keycode):
+            # print(keycode)
             event = active_events[keycode]
             char = events.EventToCharacter(
                 event.type,
                 left_shift or right_shift
             )
-            return (
+            evts.append(RecordedCharacter((
                 True if char or all else False,
                 keycode,
                 char
-            )
-    return (False, None, None)
+            )))
+    return evts
 
 
 def keyboard_active() -> bool:
     return len(KEYBOARD_EVENTS) > 0
```

### Comparing `uplogic-2.1/uplogic/input/mouse.py` & `uplogic-2.2/uplogic/input/mouse.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/input/vr.py` & `uplogic-2.2/uplogic/input/vr.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/network/client.py` & `uplogic-2.2/uplogic/network/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import socket
 import pickle
 import threading
 import bge
 from uplogic.utils.constants import DISCONNECT_MSG
-from uplogic.logging import error, success
+from uplogic.console import error, success
 from uplogic.serialize import *
 
 class Client:
 
     def __init__(self, server, port=8303, connect=False):
         self.scene = bge.logic.getCurrentScene()
         self.server = server
```

### Comparing `uplogic-2.1/uplogic/network/server.py` & `uplogic-2.2/uplogic/network/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import bge
 import bpy
 import pickle
 import socket
 import threading
 from uplogic.utils.constants import DISCONNECT_MSG
-from uplogic.logging import error, success, debug
+from uplogic.console import error, success, debug
 import time
 
 
 class Server:
 
     def __init__(self, ip=None, port=8303, start=False):
         if ip is None:
```

### Comparing `uplogic-2.1/uplogic/nodes/__init__.py` & `uplogic-2.2/uplogic/nodes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,14 +139,19 @@
             o._result = None
 
     def add_output(self, getter):
         o = Output(getter)
         self.outputs.append(o)
         return o
 
+    # def add_input(self, name):
+    #     def ipt_get(self):
+    #         return self.get_input(getattr(self, name))
+    #     setattr(self, name, )
+
     def get_input(self, param):
         if isinstance(param, ULLogicBase):
             return param.get_value()
         else:
             return param
 
     def evaluate(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/__init__.py` & `uplogic-2.2/uplogic/nodes/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/nodes/actions/addfilter.py` & `uplogic-2.2/uplogic/nodes/actions/addfilter.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.shaders import FXAA
 from uplogic.shaders import HBAO
 from uplogic.shaders import SSAO
 from uplogic.shaders import Vignette
 from uplogic.shaders import Brightness
 from uplogic.shaders import ChromaticAberration
 from uplogic.shaders import Grayscale
 from uplogic.shaders import Levels
 from uplogic.shaders import Mist
+from uplogic.shaders import Blur
 
 
 class ULAddFilter(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.pass_idx = None
@@ -32,68 +32,74 @@
 
     def evaluate(self):
         self.done = False
         condition = self.get_input(self.condition)
         ftype = self.filter_type
         if not condition or self.filter:
             if self.filter:
-                if ftype == 'VIGNETTE':
+                if ftype in [3, 'VIGNETTE']:
                     self.filter.settings['power'] = self.get_input(self.power)
                     self.filter.settings['color'] = self.get_input(self.color)
-                elif ftype == 'BRIGHTNESS':
+                elif ftype in [4, 'BRIGHTNESS']:
                     self.filter.settings['brightness'] = self.get_input(self.brightness)
-                elif ftype == 'CHROMAB':
+                elif ftype in [5, 'CHROMAB']:
                     self.filter.settings['power'] = self.get_input(self.power)
-                elif ftype == 'GRAYSCALE':
+                elif ftype in [6, 'GRAYSCALE']:
                     self.filter.settings['power'] = self.get_input(self.power)
-                elif ftype == 'LEVELS':
+                elif ftype in [7, 'LEVELS']:
                     self.filter.settings['color'] = self.get_input(self.color)
-                elif ftype == 'MIST':
+                elif ftype in [8, 'MIST']:
                     self.filter.settings['power'] = self.get_input(self.power)
                     self.filter.settings['color'] = self.get_input(self.color)
                     self.filter.settings['start'] = self.get_input(self.start)
                     self.filter.settings['density'] = self.get_input(self.density)
-                elif ftype in ['HBAO', 'SSAO']:
+                elif ftype in [1, 2, 'HBAO', 'SSAO']:
                     self.filter.settings['power'] = self.get_input(self.power)
             return
 
-        if ftype == 'FXAA':
+        if ftype in [0, 'FXAA']:
             self.filter = FXAA(self.get_input(self.pass_idx))
-        elif ftype == 'HBAO':
+        elif ftype in [1, 'HBAO']:
             self.filter = HBAO(self.get_input(self.power), self.get_input(self.pass_idx))
-        elif ftype == 'SSAO':
+        elif ftype in [2, 'SSAO']:
             self.filter = SSAO(self.get_input(self.power), self.get_input(self.pass_idx))
-        elif ftype == 'VIGNETTE':
+        elif ftype in [3, 'VIGNETTE']:
             self.filter = Vignette(
                 self.get_input(self.power),
                 self.get_input(self.color),
                 self.get_input(self.pass_idx)
             )
-        elif ftype == 'BRIGHTNESS':
+        elif ftype in [4, 'BRIGHTNESS']:
             self.filter = Brightness(
                 self.get_input(self.brightness),
                 self.get_input(self.pass_idx)
             )
-        elif ftype == 'CHROMAB':
+        elif ftype in [5, 'CHROMAB']:
             self.filter = ChromaticAberration(
                 self.get_input(self.power),
                 self.get_input(self.pass_idx)
             )
-        elif ftype == 'GRAYSCALE':
+        elif ftype in [6, 'GRAYSCALE']:
             self.filter = Grayscale(
                 self.get_input(self.power),
                 self.get_input(self.pass_idx)
             )
-        elif ftype == 'LEVELS':
+        elif ftype in [7, 'LEVELS']:
             self.filter = Levels(
                 self.get_input(self.color),
                 self.get_input(self.pass_idx)
             )
-        elif ftype == 'MIST':
+        elif ftype in [8, 'MIST']:
             self.filter = Mist(
                 self.get_input(self.start),
                 self.get_input(self.density),
                 self.get_input(self.color),
                 self.get_input(self.power),
                 self.get_input(self.pass_idx)
             )
+        elif ftype == 9:
+            self.filter = Blur(
+                16,
+                self.get_input(self.power),
+                self.get_input(self.pass_idx)
+            )
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/addobject.py` & `uplogic-2.2/uplogic/nodes/actions/sendmessage.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,34 @@
-from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from bge.types import KX_GameObject
+from bge.logic import sendMessage
 
 
-class ULAddObject(ULActionNode):
+class ULSendMessage(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.name = None
-        self.reference = None
-        self.life = None
-        self.full_copy = False
+        self.from_obj = None
+        self.to_obj = None
+        self.subject = None
+        self.body = None
         self.done = False
-        self.obj = False
-        self.OBJ = self.add_output(self._get_obj)
-        self.OUT = self.add_output(self._get_done)
+        self.OUT = self.add_output(self.get_out)
 
-    def _get_done(self):
+    def get_out(self):
         return self.done
 
-    def _get_obj(self):
-        return self.obj
-
     def evaluate(self):
         self.done = False
-        condition = self.get_input(self.condition)
-        if not condition:
+        if not self.get_input(self.condition):
             return
-        life = self.get_input(self.life)
-        name = self.get_input(self.name)
-        full_copy = self.get_input(self.full_copy)
-        reference = self.get_input(self.reference)
-        scene = logic.getCurrentScene()
-        self.obj = scene.addObject(name, reference, life, full_copy)
+        from_obj: KX_GameObject = self.get_input(self.from_obj)
+        to_obj: KX_GameObject = self.get_input(self.to_obj)
+        subject = self.get_input(self.subject)
+        body = self.get_input(self.body)
+        sendMessage(
+            subject,
+            body,
+            to_obj.name if to_obj else '',
+            from_obj.name if from_obj else ''
+        )
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/addphysicsconstraint.py` & `uplogic-2.2/uplogic/nodes/actions/addphysicsconstraint.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULAddPhysicsConstraint(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.target = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/adduiwidget.py` & `uplogic-2.2/uplogic/nodes/actions/adduiwidget.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULAddUIWidget(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.parent_widget = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/alignaxistovector.py` & `uplogic-2.2/uplogic/nodes/actions/alignaxistovector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULAlignAxisToVector(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/appendlistitem.py` & `uplogic-2.2/uplogic/nodes/actions/appendlistitem.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULAppendListItem(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.items: list = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applyforce.py` & `uplogic-2.2/uplogic/nodes/actions/setcharactergravity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,28 @@
+from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULApplyForce(ULActionNode):
+class ULSetCharacterGravity(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.force = None
+        self.gravity = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        force = self.get_input(self.force)
-        local = self.local
-        game_object.applyForce(force, local)
+        gravity = self.get_input(self.gravity)
+        physics = constraints.getCharacter(game_object)
+        if physics:
+            physics.gravity = gravity
+        else:
+            game_object.gravity = gravity
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applyimpulse.py` & `uplogic-2.2/uplogic/nodes/actions/applytorque.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULApplyImpulse(ULActionNode):
+class ULApplyTorque(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.point = None
-        self.impulse = None
+        self.torque = None
+        self.local = False
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        point = self.get_input(self.point)
-        impulse = self.get_input(self.impulse)
+        torque = self.get_input(self.torque)
         local = self.local
-        if impulse:
-            game_object.applyImpulse(point, impulse, local)
+        if torque:
+            game_object.applyTorque(torque, local)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applymovement.py` & `uplogic-2.2/uplogic/nodes/actions/removefilter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.shaders import remove_filter
 
 
-class ULApplyMovement(ULActionNode):
+class ULRemoveFilter(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_object = None
-        self.movement = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        self.pass_idx = None
+        self.done = False
+        self.OUT = self.add_output(self._get_done)
 
-    def get_done(self):
+    def _get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.game_object)
-        movement = self.get_input(self.movement)
-        local = self.local
-        if movement:
-            game_object.applyMovement(movement, local)
+        pass_idx = self.get_input(self.pass_idx)
+        remove_filter(pass_idx)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applyrotation.py` & `uplogic-2.2/uplogic/nodes/actions/applyrotation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULApplyRotation(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applytorque.py` & `uplogic-2.2/uplogic/nodes/actions/setcollisionmask.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULApplyTorque(ULActionNode):
+class ULSetCollisionMask(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.torque = None
-        self.local = False
+        self.slots = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        torque = self.get_input(self.torque)
-        local = self.local
-        if torque:
-            game_object.applyTorque(torque, local)
+        slots = self.get_input(self.slots)
+        game_object.collisionMask = slots
+
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/applytransform.py` & `uplogic-2.2/uplogic/nodes/actions/applytransform.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULApplyTransform(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/cameraraycast.py` & `uplogic-2.2/uplogic/nodes/actions/cameraraycast.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.raycasting import raycast_camera, RayCastCameraData
 from uplogic.utils import get_bitmask
 
 
 class ULCameraRayCast(ULActionNode):
 
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/characterjump.py` & `uplogic-2.2/uplogic/nodes/actions/removephysicsconstraint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULCharacterJump(ULActionNode):
+class ULRemovePhysicsConstraint(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_object = None
+        self.object = None
+        self.name = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.game_object)
-        physics = constraints.getCharacter(game_object)
-        physics.jump()
-
+        obj = self.get_input(self.object)
+        name = self.get_input(self.name)
+        constraints.removeConstraint(obj[name].getConstraintId())
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/clampedmodifyproperty.py` & `uplogic-2.2/uplogic/nodes/actions/clampedmodifyproperty.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import clamp
 
 
 class ULClampedModifyProperty(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/clearvariables.py` & `uplogic-2.2/uplogic/nodes/actions/clearvariables.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 import json
 import os
 
 
 class ULClearVariables(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/copyproperty.py` & `uplogic-2.2/uplogic/nodes/actions/copyproperty.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULCopyProperty(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.from_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuibutton.py` & `uplogic-2.2/uplogic/nodes/actions/createuibutton.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import LabelButton
 from math import degrees
 
 
 class ULCreateUIButton(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuicanvas.py` & `uplogic-2.2/uplogic/nodes/actions/createuicanvas.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import Canvas
 
 
 class ULCreateUICanvas(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuiimage.py` & `uplogic-2.2/uplogic/nodes/actions/createuiimage.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import Image
 from math import degrees
 
 
 class ULCreateUIImage(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
@@ -16,14 +15,15 @@
         self.angle = None
         self.texture = None
         self._widget = None
         self.layout_type = 'RelativeLayout'
         self.boxlayout_type = 'vertical'
         self.halign_type = 'left'
         self.valign_type = 'bottom'
+        self.aspect_ratio = True
         self._done = False
         self.OUT = self.add_output(self._get_done)
         self.WIDGET = self.add_output(self._get_widget)
 
     def _get_done(self):
         return self._done
 
@@ -46,13 +46,14 @@
         self._widget = Image(
             pos=pos,
             size=size,
             texture=texture.name,
             relative={'pos': rel_pos, 'size': rel_size},
             halign=self.halign_type,
             valign=self.valign_type,
+            use_aspect_ratio=self.aspect_ratio,
             angle=angle
         )
         if parent:
             parent.add_widget(self._widget)
         self._done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuilabel.py` & `uplogic-2.2/uplogic/nodes/actions/createuilabel.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import Label
 from math import degrees
 
 
 class ULCreateUILabel(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
@@ -56,16 +55,14 @@
         else:
             shadow_offset = [0, 0]
             shadow_color = [0, 0, 0, 0]
 
         
         font = font.filepath.replace('\\', '/') if font else 0
 
-        print(rel_pos)
-
         self._widget = Label(
             pos=pos,
             relative={'pos': rel_pos},
             halign=self.halign_type,
             valign=self.valign_type,
             text=text,
             font=font,
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuilayout.py` & `uplogic-2.2/uplogic/nodes/actions/createuilayout.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import RelativeLayout, FloatLayout, BoxLayout
 from math import degrees
 
 
 layouts = {
     'FloatLayout': FloatLayout,
     'RelativeLayout': RelativeLayout,
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createuislider.py` & `uplogic-2.2/uplogic/nodes/actions/createuislider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import Slider, FrameSlider, ProgressSlider
 from mathutils import Vector
 from math import degrees
 
 
 class ULCreateUISlider(ULActionNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/createvehicle.py` & `uplogic-2.2/uplogic/nodes/actions/createvehicle.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.physics.vehicle import ULVehicle
 from uplogic.utils.constants import VEHICLE
 
 
 class ULCreateVehicle(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/cursorbehavior.py` & `uplogic-2.2/uplogic/nodes/actions/cursorbehavior.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULCursorBehavior(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.cursor_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/cursorvisibility.py` & `uplogic-2.2/uplogic/nodes/actions/cursorvisibility.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCursorVisibility(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.visibility_status = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/dispatchevent.py` & `uplogic-2.2/uplogic/nodes/actions/popdictkey.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,38 @@
-from uplogic.events import send
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.utils import debug
 
 
-class ULDispatchEvent(ULActionNode):
+class ULPopDictKey(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.subject = None
-        self.body = None
-        self.target = None
-        self.old_subject = None
+        self.dict = None
+        self.key = None
+        self.new_dict = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
+        self.DICT = self.add_output(self.get_dict)
+        self.VALUE = self.add_output(self.get_value)
 
     def get_done(self):
         return self.done
 
+    def get_dict(self):
+        return self.new_dict
+
+    def get_value(self):
+        return self.value
+
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        subject = self.get_input(self.subject)
-        body = self.get_input(self.body)
-        target = self.get_input(self.target)
-        send(subject, body, target)
+        dictionary = self.get_input(self.dict)
+        key = self.get_input(self.key)
+        if key in dictionary:
+            self.value = dictionary.pop(key)
+        else:
+            debug("Dict Delete Key Node: Key '{}' not in Dict!".format(key))
+            return
+        self.new_dict = dictionary
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/draw.py` & `uplogic-2.2/uplogic/nodes/actions/draw.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.utils.visualize import draw_line, draw_path, draw_box, draw_cube, draw_mesh, draw_arrow
-from uplogic.nodes import ULOutSocket
+from uplogic.utils.visualize import draw_line, draw_path, draw_box, draw_cube, draw_mesh, draw_arrow, draw_axis
 
 
 class DrawNode(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = False
         self.color = (1, 1, 1, 1)
@@ -22,15 +21,16 @@
         self.mode = 0
         self.modes = [
             self.draw_line,
             self.draw_arrow,
             self.draw_path,
             self.draw_cube,
             self.draw_box,
-            self.draw_mesh
+            self.draw_mesh,
+            self.draw_axis
         ]
 
     def get_out(self):
         return self.done
 
     def draw_line(self):
         draw_line(
@@ -72,13 +72,19 @@
 
     def draw_mesh(self):
         draw_mesh(
             self.get_input(self.object),
             self.get_input(self.color)
         )
 
+    def draw_axis(self):
+        draw_axis(
+            self.get_input(self.object),
+            self.get_input(self.length)
+        )
+
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         self.modes[self.mode]()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/drawbox.py` & `uplogic-2.2/uplogic/nodes/actions/drawbox.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.utils.visualize import draw_box
-from uplogic.nodes import ULOutSocket
 
 
 class ULDrawBox(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.color = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/drawcube.py` & `uplogic-2.2/uplogic/nodes/actions/drawcube.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
 from uplogic.utils.visualize import draw_cube
-from uplogic.nodes import ULOutSocket
 
 
 class ULDrawCube(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.color = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/drawline.py` & `uplogic-2.2/uplogic/nodes/actions/drawline.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge.render import drawLine
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULDrawLine(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.color = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/editbone.py` & `uplogic-2.2/uplogic/nodes/actions/editbone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from bge import logic
 from mathutils import Euler
 from mathutils import Vector
 from mathutils import Quaternion
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULEditBone(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.armature = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/endobject.py` & `uplogic-2.2/uplogic/nodes/actions/endobject.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULEndObject(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.scene = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/executesubnetwork.py` & `uplogic-2.2/uplogic/nodes/actions/executesubnetwork.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import make_valid_name
 
 
 class ULExecuteSubNetwork(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/followpath.py` & `uplogic-2.2/uplogic/nodes/actions/followpath.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.objects import rotate_to
 from uplogic.utils.objects import move_to
 
 
 class ULFollowPath(ULActionNode):
     class MotionPath(object):
         def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/gamepadlook.py` & `uplogic-2.2/uplogic/nodes/actions/gamepadlook.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.input.gamepad import GamepadLook
 from math import degrees
 
 
 class ULGamepadLook(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/gamepadvibration.py` & `uplogic-2.2/uplogic/nodes/actions/gamepadvibration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULGamepadVibration(ULActionNode):
     def __init__(self, axis=0):
         ULActionNode.__init__(self)
         self.condition = None
         self.index = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/getperformanceprofile.py` & `uplogic-2.2/uplogic/nodes/actions/getperformanceprofile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bge.logic import getRealTime
 
 
 class ULGetPerformanceProfile(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/installsubnetwork.py` & `uplogic-2.2/uplogic/nodes/actions/stopsubnetwork.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,28 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.utils import make_valid_name
 
 
-class ULInstallSubNetwork(ULActionNode):
+class ULStopSubNetwork(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.target_object = None
-        self.tree_name = None
-        self.initial_status = None
-        self._network = None
+        self.game_object = None
+        self.logic_network_name = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
-    def setup(self, network):
-        self._network = network
-
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        target_object = self.get_input(self.target_object)
-        tree_name = self.get_input(self.tree_name)
-        initial_status = self.get_input(self.initial_status)
-        self._network.install_subnetwork(
-            target_object,
-            tree_name,
-            initial_status
-        )
+        game_object = self.get_input(self.game_object)
+        logic_network_name = self.get_input(self.logic_network_name)
+        tree_name = make_valid_name(logic_network_name)
+        network = game_object.get(f'IGNLTree_{tree_name}')
+        if network is None:
+            return
+        network.stop()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/instream.py` & `uplogic-2.2/uplogic/nodes/actions/instream.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bge import events
 from bge.logic import keyboard
 
 
 class ULKeyLogger(ULActionNode):
     '''DEPRECATED
     This node has been moved to `parameters`, this is for legacy support.
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/listglobalvalues.py` & `uplogic-2.2/uplogic/nodes/actions/listglobalvalues.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.data import GlobalDB
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULListGlobalValues(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.data_id = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/listvariables.py` & `uplogic-2.2/uplogic/nodes/actions/listvariables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 import json
 import os
 
 
 class ULListVariables(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/loadblendfile.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveevolumetrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+import bpy
 
 
-class ULLoadBlendFile(ULActionNode):
+class ULSetEeveeVolumetrics(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.file_name = None
+        self.value = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        file_name = self.get_input(self.file_name)
-        logic.startGame(file_name)
+        value = self.get_input(self.value)
+        scene = logic.getCurrentScene()
+        bpy.data.scenes[
+            scene.name
+        ].eevee.use_volumetric_lights = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/loadfilecontent.py` & `uplogic-2.2/uplogic/nodes/actions/loadscene.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils.scene import FileLoader
+from uplogic.utils.scene import SceneLoader
+from bpy.types import Scene
 
 
-class ULLoadFileContent(ULActionNode):
+class ULLoadScene(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
+        self.scene = None
         self.done = False
         self.updated = False
         self.status = 0.0
         self.datatype = ''
         self.item = ''
         self.loader = None
         self.OUT = self.add_output(self.get_done)
@@ -33,17 +34,18 @@
         return self.done
 
     def get_updated(self):
         return self.updated
 
     def evaluate(self):
         self.done = False
-        condition = self.get_input(self.condition)
+        condition: bool = self.get_input(self.condition)
+        scene: Scene = self.get_input(self.scene)
         if condition and self.loader is None:
-            self.loader = FileLoader()
+            self.loader = SceneLoader(scene)
         if self.loader:
             self.updated = True
             self.status = self.loader.status
             self.item = self.loader.item
             self.datatype = self.loader.data
             if self.loader.finished:
                 self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/loadgame.py` & `uplogic-2.2/uplogic/nodes/actions/loadgame.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bge import logic, constraints
 from mathutils import Euler
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 import json
 
 
 class ULLoadGame(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/loadscene.py` & `uplogic-2.2/uplogic/nodes/actions/loadfilecontent.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils.scene import SceneLoader
-from bpy.types import Scene
+from uplogic.utils.scene import FileLoader
 
 
-class ULLoadScene(ULActionNode):
+class ULLoadFileContent(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.scene = None
         self.done = False
         self.updated = False
         self.status = 0.0
         self.datatype = ''
         self.item = ''
         self.loader = None
         self.OUT = self.add_output(self.get_done)
@@ -35,18 +32,17 @@
         return self.done
 
     def get_updated(self):
         return self.updated
 
     def evaluate(self):
         self.done = False
-        condition: bool = self.get_input(self.condition)
-        scene: Scene = self.get_input(self.scene)
+        condition = self.get_input(self.condition)
         if condition and self.loader is None:
-            self.loader = SceneLoader(scene)
+            self.loader = FileLoader()
         if self.loader:
             self.updated = True
             self.status = self.loader.status
             self.item = self.loader.item
             self.datatype = self.loader.data
             if self.loader.finished:
                 self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/localclient.py` & `uplogic-2.2/uplogic/nodes/actions/localclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.network import Client
 from time import time
 from uplogic.events import send, receive
 
 
 class ULLocalClient(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/localserver.py` & `uplogic-2.2/uplogic/nodes/actions/localserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.network import Server
 from uplogic.events import send, receive
 
 
 class ULLocalServer(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/makeuniquelight.py` & `uplogic-2.2/uplogic/nodes/actions/loadblendfile.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,22 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import make_unique_light
 
 
-class ULMakeUniqueLight(ULActionNode):
-
+class ULLoadBlendFile(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.light = None
+        self.file_name = None
         self.done = None
-        self._light = None
         self.OUT = self.add_output(self.get_done)
-        self.LIGHT = self.add_output(self.get_light)
 
     def get_done(self):
         return self.done
 
-    def get_light(self):
-        return self._light
-
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        self._light = make_unique_light(self.get_input(self.light))
+        file_name = self.get_input(self.file_name)
+        logic.startGame(file_name)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/modifyproperty.py` & `uplogic-2.2/uplogic/nodes/actions/modifyproperty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.math import clamp
 
 
 class ULModifyProperty(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/mouselook.py` & `uplogic-2.2/uplogic/nodes/actions/mouselook.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import render
 from bge import logic
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.input import MouseLook
 from math import degrees
 
 
 class ULMouseLook(ULActionNode):
 
     def __init__(self):
@@ -65,12 +64,13 @@
                     cap_x=cap_x,
                     use_cap_y=use_cap_y,
                     cap_y=cap_y,
                     invert=self.get_input(self.inverted),
                     smoothing=self.get_input(self.smooth),
                     local=head is not obj,
                     center_mouse=self.center_mouse,
-                    front=self.get_input(self.axis)
+                    front=self.get_input(self.axis),
+                    active=False
                 )
-        if self.mouselook is not None:
-            self.mouselook.active = condition
+        if self.mouselook is not None and condition:
+            self.mouselook.update()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/mouseraycast.py` & `uplogic-2.2/uplogic/nodes/actions/mouseraycast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import get_bitmask
 from uplogic.utils.raycasting import raycast_mouse, RayCastData
 
 
 class ULMouseRayCast(ULActionNode):
 
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/mousesetposition.py` & `uplogic-2.2/uplogic/nodes/actions/mousesetposition.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetMousePosition(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.screen_x = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/moveto.py` & `uplogic-2.2/uplogic/nodes/actions/moveto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 from uplogic.utils.objects import move_to
 
 
 class ULMoveTo(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/movetowithnavmesh.py` & `uplogic-2.2/uplogic/nodes/actions/movetowithnavmesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from bge import render
 from bge.types import KX_GameObject as GameObject
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 from uplogic.utils.objects import rotate_to
 from uplogic.utils.objects import move_to
 
 
 class ULMoveToWithNavmesh(ULActionNode):
 
     class MotionPath(object):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/pausesound.py` & `uplogic-2.2/uplogic/nodes/actions/makeuniquelight.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
-from uplogic.audio.sound import ULSound
+from uplogic.nodes import ULActionNode
+from uplogic.utils import make_unique_light
 
 
-class ULPauseSound(ULActionNode):
+class ULMakeUniqueLight(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.sound = None
-        self.done = False
+        self.light = None
+        self.done = None
+        self._light = None
         self.OUT = self.add_output(self.get_done)
+        self.LIGHT = self.add_output(self.get_light)
 
     def get_done(self):
         return self.done
 
+    def get_light(self):
+        return self._light
+
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        sound: ULSound = self.get_input(self.sound)
-        sound.pause()
+        self._light = make_unique_light(self.get_input(self.light))
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/playaction.py` & `uplogic-2.2/uplogic/nodes/actions/playaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from uplogic.animation import ActionSystem
 from uplogic.data import GlobalDB
 from uplogic.animation import Action
 from uplogic.events import receive
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.math import clamp
 from bpy.types import Action as BPYAction
 
 
 class ULPlayAction(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/playsequence.py` & `uplogic-2.2/uplogic/nodes/actions/playsequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.animation.sequence import Sequence
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 
 
 class ULPaySequence(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/popdictkey.py` & `uplogic-2.2/uplogic/nodes/actions/setglobalvalue.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,29 @@
+from uplogic.data import GlobalDB
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import debug
 
 
-class ULPopDictKey(ULActionNode):
+class ULSetGlobalValue(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.dict = None
+        self.data_id = None
         self.key = None
-        self.new_dict = None
+        self.value = None
+        self.persistent = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
-        self.DICT = self.add_output(self.get_dict)
-        self.VALUE = self.add_output(self.get_value)
 
     def get_done(self):
         return self.done
 
-    def get_dict(self):
-        return self.new_dict
-
-    def get_value(self):
-        return self.value
-
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        dictionary = self.get_input(self.dict)
+        data_id = self.get_input(self.data_id)
+        persistent = self.get_input(self.persistent)
         key = self.get_input(self.key)
-        if key in dictionary:
-            self.value = dictionary.pop(key)
-        else:
-            debug("Dict Delete Key Node: Key '{}' not in Dict!".format(key))
-            return
-        self.new_dict = dictionary
+        value = self.get_input(self.value)
+        db = GlobalDB.retrieve(data_id)
+        db.put(key, value, persistent)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/printvalue.py` & `uplogic-2.2/uplogic/nodes/actions/setresolution.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.logging import log
 
 
-class ULPrintValue(ULActionNode):
-
+class ULSetResolution(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.value = None
+        self.x_res = None
+        self.y_res = None
         self.done = None
-        self.msg_type = 'INFO'
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        value = self.get_input(self.value)
-        log(value, self.msg_type)
+        x_res = self.get_input(self.x_res)
+        y_res = self.get_input(self.y_res)
+        render.setWindowSize(x_res, y_res)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/projectileraycast.py` & `uplogic-2.2/uplogic/nodes/actions/projectileraycast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import logic
 from bge import render
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import get_bitmask
 from uplogic.utils.raycasting import raycast_projectile, RayCastProjectileData
 
 
 class ULProjectileRayCast(ULActionNode):
 
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/raycast.py` & `uplogic-2.2/uplogic/nodes/actions/raycast.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.raycasting import raycast, RayCastData
 from uplogic.utils.math import get_bitmask
 from bge.logic import getCurrentScene
 from bpy.types import Material
 
 
 class ULRaycast(ULActionNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removefilter.py` & `uplogic-2.2/uplogic/nodes/actions/togglefilter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.shaders import remove_filter
+from uplogic.shaders import toggle_filter
 
 
-class ULRemoveFilter(ULActionNode):
+class ULToggleFilter(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.pass_idx = None
         self.done = False
         self.OUT = self.add_output(self._get_done)
 
@@ -15,9 +14,9 @@
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         pass_idx = self.get_input(self.pass_idx)
-        remove_filter(pass_idx)
+        toggle_filter(pass_idx)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removelistindex.py` & `uplogic-2.2/uplogic/nodes/actions/removelistindex.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 
 class ULRemoveListIndex(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.items = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removelistvalue.py` & `uplogic-2.2/uplogic/nodes/actions/removelistvalue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 
 
 class ULRemoveListValue(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removeoverlaycollection.py` & `uplogic-2.2/uplogic/nodes/actions/setlightenergy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
-from bge import logic
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
+from bge.types import KX_GameObject
 
 
-class ULRemoveOverlayCollection(ULActionNode):
+class ULSetLightEnergy(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.collection = None
-        self.done = False
+        self.lamp = None
+        self.energy = None
+        self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        logic.getCurrentScene().removeOverlayCollection(
-            self.get_input(self.collection)
-        )
+        light: KX_GameObject = self.get_input(self.lamp)
+        energy = self.get_input(self.energy)
+        light = light.blenderObject.data
+        light.energy = energy
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removeparent.py` & `uplogic-2.2/uplogic/nodes/actions/removeparent.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULRemoveParent(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.child_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removephysicsconstraint.py` & `uplogic-2.2/uplogic/nodes/actions/dispatchevent.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
-from bge import constraints
+from uplogic.events import send
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULRemovePhysicsConstraint(ULActionNode):
+class ULDispatchEvent(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.object = None
-        self.name = None
+        self.subject = None
+        self.body = None
+        self.target = None
+        self.old_subject = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        obj = self.get_input(self.object)
-        name = self.get_input(self.name)
-        constraints.removeConstraint(obj[name].getConstraintId())
+        subject = self.get_input(self.subject)
+        body = self.get_input(self.body)
+        target = self.get_input(self.target)
+        send(subject, body, target)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/removevariable.py` & `uplogic-2.2/uplogic/nodes/actions/savevariable.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,62 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 import bpy
 import json
 import os
 
 
-class ULRemoveVariable(ULActionNode):
+class ULSaveVariable(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.name = None
+        self.val = None
         self.file_name = None
         self.path = ''
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
-    def write_to_json(self, path, name):
+    def write_to_json(self, path, name, val):
         data = None
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
             f = open(path, 'r')
             data = json.load(f)
-            if name in data:
-                del data[name]
+            data[name] = val
             f.close()
             f = open(path, 'w')
             json.dump(data, f, indent=2)
-            f.close()
         else:
-            debug('File does not exist!')
+            debug('Variable file does not exist - creating...')
+            f = open(path, 'w')
+            data = {name: val}
+            json.dump(data, f, indent=2)
+        f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         name = self.get_input(self.name)
-        cust_path = self.get_custom_path(self.path)
+        val = self.get_input(self.val)
 
+        cust_path = self.get_custom_path(self.path)
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
+
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, name)
+        self.write_to_json(path, name, val)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/replacemesh.py` & `uplogic-2.2/uplogic/nodes/actions/replacemesh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bge.types import KX_GameObject
 from bpy.types import Mesh
 
 
 class ULReplaceMesh(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/restartgame.py` & `uplogic-2.2/uplogic/nodes/actions/setgamma.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+import bpy
 
 
-class ULRestartGame(ULActionNode):
+class ULSetGamma(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
+        self.value = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        logic.restartGame()
+        value = self.get_input(self.value)
+        scene = logic.getCurrentScene()
+        bpy.data.scenes[
+            scene.name
+        ].view_settings.gamma = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/resumesound.py` & `uplogic-2.2/uplogic/nodes/actions/resumesound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 
 
 class ULResumeSound(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.sound = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/rotateto.py` & `uplogic-2.2/uplogic/nodes/actions/addobject.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import rotate_to
 
 
-class ULActionRotateTo(ULActionNode):
+class ULAddObject(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.moving_object = None
-        self.target_point = None
-        self.speed = None
-        self._done = False
-        self.rot_axis = 2
-        self.front_axis = 0
+        self.name = None
+        self.reference = None
+        self.life = None
+        self.full_copy = False
+        self.done = False
+        self.obj = False
+        self.OBJ = self.add_output(self._get_obj)
         self.OUT = self.add_output(self._get_done)
 
     def _get_done(self):
-        return self._done
+        return self.done
+
+    def _get_obj(self):
+        return self.obj
 
     def evaluate(self):
-        self._done = False
-        if not self.get_input(self.condition):
+        self.done = False
+        condition = self.get_input(self.condition)
+        if not condition:
             return
-        moving_object = self.get_input(self.moving_object)
-        target_point = self.get_input(self.target_point)
-        speed = self.get_input(self.speed)
-        rot_axis = self.get_input(self.rot_axis)
-        front_axis = self.get_input(self.front_axis)
-        rotate_to(moving_object, target_point, rot_axis, front_axis, speed)
-        self._done = True
+        life = self.get_input(self.life)
+        name = self.get_input(self.name)
+        full_copy = self.get_input(self.full_copy)
+        reference = self.get_input(self.reference)
+        scene = logic.getCurrentScene()
+        self.obj = scene.addObject(name, reference, life, full_copy)
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/runactuator.py` & `uplogic-2.2/uplogic/nodes/actions/setdynamics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,28 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULActionNode
 
 
-class ULRunActuator(ULActionNode):
-
+class ULSetDynamics(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_obj = None
-        self.cont_name = None
-        self.act_name = None
+        self.game_object = None
+        self.activate = False
+        self.ghost = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
-        game_obj = self.get_input(self.game_obj)
-        cont_name = self.get_input(self.cont_name)
-        act_name = self.get_input(self.act_name)
-        controller = game_obj.controllers[cont_name]
-        if act_name not in controller.actuators:
-            return
-        actuator = controller.actuators[act_name]
         if not self.get_input(self.condition):
             return
-        controller.activate(actuator)
+        game_object = self.get_input(self.game_object)
+        ghost = self.get_input(self.ghost)
+        activate = self.get_input(self.activate)
+        if activate:
+            game_object.restoreDynamics()
+        else:
+            game_object.suspendDynamics(ghost)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/runpython.py` & `uplogic-2.2/uplogic/nodes/actions/runpython.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 
 
 class ULRunPython(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/savegame.py` & `uplogic-2.2/uplogic/nodes/actions/savegame.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import constraints
 from bge import logic
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes.logictree import ULLogicTree
 import json
 import os
 
 
 class ULSaveGame(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/savevariable.py` & `uplogic-2.2/uplogic/nodes/actions/savevariabledict.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,53 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 import bpy
 import json
 import os
 
 
-class ULSaveVariable(ULActionNode):
+class ULSaveVariableDict(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.name = None
         self.val = None
         self.file_name = None
         self.path = ''
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
-    def write_to_json(self, path, name, val):
-        data = None
+    def write_to_json(self, path, val):
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
-            f = open(path, 'r')
-            data = json.load(f)
-            data[name] = val
-            f.close()
             f = open(path, 'w')
-            json.dump(data, f, indent=2)
+            json.dump(val, f, indent=2)
         else:
-            debug('Variable file does not exist - creating...')
+            debug('file does not exist - creating...')
             f = open(path, 'w')
-            data = {name: val}
-            json.dump(data, f, indent=2)
+            json.dump(val, f, indent=2)
         f.close()
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        name = self.get_input(self.name)
         val = self.get_input(self.val)
 
         cust_path = self.get_custom_path(self.path)
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
-
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, name, val)
+        self.write_to_json(path, val)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/savevariabledict.py` & `uplogic-2.2/uplogic/nodes/actions/removevariable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 import bpy
 import json
 import os
 
 
-class ULSaveVariableDict(ULActionNode):
+class ULRemoveVariable(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.val = None
+        self.name = None
         self.file_name = None
         self.path = ''
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
-    def write_to_json(self, path, val):
+    def write_to_json(self, path, name):
+        data = None
         if not path.endswith('.json'):
             path = path + f'{self.get_input(self.file_name)}.json'
         if os.path.isfile(path):
+            f = open(path, 'r')
+            data = json.load(f)
+            if name in data:
+                del data[name]
+            f.close()
             f = open(path, 'w')
-            json.dump(val, f, indent=2)
+            json.dump(data, f, indent=2)
+            f.close()
         else:
-            debug('file does not exist - creating...')
-            f = open(path, 'w')
-            json.dump(val, f, indent=2)
-        f.close()
+            debug('File does not exist!')
 
     def get_custom_path(self, path):
         if not path.endswith('/') and not path.endswith('json'):
             path = path + '/'
         return path
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        val = self.get_input(self.val)
-
+        name = self.get_input(self.name)
         cust_path = self.get_custom_path(self.path)
+
         path = (
             bpy.path.abspath('//Data/')
             if self.path == ''
             else bpy.path.abspath(cust_path)
         )
         os.makedirs(path, exist_ok=True)
 
-        self.write_to_json(path, val)
+        self.write_to_json(path, name)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/sendmessage.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveessr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,25 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from bge.types import KX_GameObject
-from bge.logic import sendMessage
-from uplogic.nodes import ULOutSocket
+import bpy
 
 
-class ULSendMessage(ULActionNode):
+class ULSetEeveeSSR(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.from_obj = None
-        self.to_obj = None
-        self.subject = None
-        self.body = None
-        self.done = False
-        self.OUT = self.add_output(self.get_out)
+        self.value = None
+        self.done = None
+        self.OUT = self.add_output(self.get_done)
 
-    def get_out(self):
+    def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        from_obj: KX_GameObject = self.get_input(self.from_obj)
-        to_obj: KX_GameObject = self.get_input(self.to_obj)
-        subject = self.get_input(self.subject)
-        body = self.get_input(self.body)
-        sendMessage(
-            subject,
-            body,
-            to_obj.name if to_obj else '',
-            from_obj.name if from_obj else ''
-        )
+        value = self.get_input(self.value)
+        scene = logic.getCurrentScene()
+        bpy.data.scenes[scene.name].eevee.use_ssr = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/sendnetworkmessage.py` & `uplogic-2.2/uplogic/nodes/actions/sendnetworkmessage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 
 class ULSendNetworkMessage(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.entity = None
         self.data = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setactionframe.py` & `uplogic-2.2/uplogic/nodes/actions/setactionframe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from uplogic.animation import ActionSystem
 from uplogic.animation.action import Action
 from uplogic.data import GlobalDB
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Action as BPYAction
 from bge.types import KX_GameObject
 
 
 class ULSetActionFrame(ULActionNode):
 
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setactuatorvalue.py` & `uplogic-2.2/uplogic/nodes/actions/setactuatorvalue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULActionNode
 
 
 class ULSetActuatorValue(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setboneconstraintattr.py` & `uplogic-2.2/uplogic/nodes/actions/setboneconstraintattr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetBoneConstraintAttribute(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.armature = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setboneconstraintinfluence.py` & `uplogic-2.2/uplogic/nodes/actions/setboneconstraintinfluence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetBoneConstraintInfluence(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.armature = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setboneconstrainttarget.py` & `uplogic-2.2/uplogic/nodes/actions/setboneconstrainttarget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetBoneConstraintTarget(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.armature = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setboneposition.py` & `uplogic-2.2/uplogic/nodes/actions/setboneposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from mathutils import Euler
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 
 
 class ULSetBonePosition(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcamera.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveebloom.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+import bpy
 
 
-class ULSetCamera(ULActionNode):
+class ULSetEeveeBloom(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.camera = None
+        self.value = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        camera = self.get_input(self.camera)
+        value = self.get_input(self.value)
         scene = logic.getCurrentScene()
-        scene.active_camera = camera
+        bpy.data.scenes[scene.name].eevee.use_bloom = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcamerafov.py` & `uplogic-2.2/uplogic/nodes/actions/setcamera.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetCameraFOV(ULActionNode):
+class ULSetCamera(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.camera = None
-        self.fov = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         camera = self.get_input(self.camera)
-        fov = self.get_input(self.fov)
-        camera.fov = fov
+        scene = logic.getCurrentScene()
+        scene.active_camera = camera
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcameraorthoscale.py` & `uplogic-2.2/uplogic/nodes/actions/setcameraorthoscale.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCameraOrthoScale(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.camera = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcharactergravity.py` & `uplogic-2.2/uplogic/nodes/actions/setproperty.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetCharacterGravity(ULActionNode):
+class ULSetProperty(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.gravity = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        self.property_name = None
+        self.property_value = None
+        self.mode = 0
+        self.done = False
+        self.OUT = self.add_output(self._get_done)
 
-    def get_done(self):
+    def _get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        gravity = self.get_input(self.gravity)
-        physics = constraints.getCharacter(game_object)
-        if physics:
-            physics.gravity = gravity
-        else:
-            game_object.gravity = gravity
+        property_name = self.get_input(self.property_name)
+        property_value = self.get_input(self.property_value)
         self.done = True
+        obj = game_object.blenderObject if self.mode else game_object
+        obj[property_name] = property_value
+        if self.mode:
+            obj.color = obj.color  # force object data refresh
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcharacterjumpspeed.py` & `uplogic-2.2/uplogic/nodes/actions/setcharacterjumpspeed.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCharacterJumpSpeed(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcharactermaxjumps.py` & `uplogic-2.2/uplogic/nodes/actions/setcharactermaxjumps.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCharacterMaxJumps(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcharactervelocity.py` & `uplogic-2.2/uplogic/nodes/actions/setcharactervelocity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCharacterVelocity(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcharacterwalkdir.py` & `uplogic-2.2/uplogic/nodes/actions/setcharacterwalkdir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import constraints
 from bge import logic
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 
 
 class ULSetCharacterWalkDir(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcollisiongroup.py` & `uplogic-2.2/uplogic/nodes/actions/setrigidbody.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetCollisionGroup(ULActionNode):
+class ULSetRigidBody(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.slots = None
-        self.mode = 0
+        self.activate = False
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        slots = self.get_input(self.slots)
-        if self.mode:
-            game_object.collisionMask = slots
+        activate = self.get_input(self.activate)
+        if activate:
+            game_object.enableRigidBody()
         else:
-            game_object.collisionGroup = slots
+            game_object.disableRigidBody()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcollisionmask.py` & `uplogic-2.2/uplogic/nodes/actions/setmaterial.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.utils import debug
+from bpy.types import Material
+from bge.types import KX_GameObject
 
 
-class ULSetCollisionMask(ULActionNode):
+class ULSetMaterial(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.slots = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        self.slot = None
+        self.mat_name = None
+        self.done = False
+        self.OUT = self.add_output(self._get_done)
 
-    def get_done(self):
+    def _get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.game_object)
-        slots = self.get_input(self.slots)
-        game_object.collisionMask = slots
-
+        game_object: KX_GameObject = self.get_input(self.game_object)
+        slot: int = self.get_input(self.slot)
+        material: Material = self.get_input(self.mat_name)
+        bl_obj = game_object.blenderObject
+        if slot > len(bl_obj.material_slots) - 1:
+            debug('Set Material: Slot does not exist!')
+            return
+        bl_obj.material_slots[slot].material = material
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setconstraintattribute.py` & `uplogic-2.2/uplogic/nodes/actions/setconstraintattribute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class SetConstraintAttributeNode(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcurvepoints.py` & `uplogic-2.2/uplogic/nodes/actions/setcurvepoints.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetCurvePoints(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.curve_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setcustomcursor.py` & `uplogic-2.2/uplogic/nodes/actions/setcustomcursor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.ui import Cursor, remove_custom_cursor
 from bpy.types import Image
 
 
 class ULSetCustomCursor(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setdictkey.py` & `uplogic-2.2/uplogic/nodes/actions/setdictkey.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetDictKey(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.dict = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setdynamics.py` & `uplogic-2.2/uplogic/nodes/actions/setphysics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetDynamics(ULActionNode):
+class ULSetPhysics(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
         self.activate = False
-        self.ghost = None
+        self.free_const = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        ghost = self.get_input(self.ghost)
         activate = self.get_input(self.activate)
+        free_const = self.get_input(self.free_const)
         if activate:
-            game_object.restoreDynamics()
+            game_object.restorePhysics()
         else:
-            game_object.suspendDynamics(ghost)
+            game_object.suspendPhysics(free_const)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveeao.py` & `uplogic-2.2/uplogic/nodes/actions/setvsync.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-from bge import logic
+from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
 
 
-class ULSetEeveeAO(ULActionNode):
-
+class ULSetVSync(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.value = None
+        self.vsync_mode = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[scene.name].eevee.use_gtao = value
+        render.setVsync(self.vsync_mode)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveebloom.py` & `uplogic-2.2/uplogic/nodes/parameters/storevalue.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,32 @@
-from bge import logic
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
+from uplogic.nodes import ULParameterNode
 
 
-class ULSetEeveeBloom(ULActionNode):
-
+class ULStoreValue(ULParameterNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
+        ULParameterNode.__init__(self)
         self.value = None
-        self.done = None
+        self.initialize = True
+        self.condition = None
+        self.done = False
+        self._stored_value = None
+
+        # WEIRD NAMING: self.DONE = Condition, self.OUT = Stored value
+        self.DONE = self.add_output(self.get_stored)
         self.OUT = self.add_output(self.get_done)
 
-    def get_done(self):
+    def get_stored(self):
         return self.done
 
+    def get_done(self):
+        return self._stored_value
+
     def evaluate(self):
         self.done = False
-        if not self.get_input(self.condition):
+        condition = self.get_input(self.condition)
+        if self.initialize:
+            self.initialize = False
+            condition = True
+        if not condition:
             return
-        value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[scene.name].eevee.use_bloom = value
+        self._stored_value = self.get_input(self.value)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveesmaa.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveesmaa.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 
 
 class ULSetEeveeSMAA(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveesmaaquality.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveesmaaquality.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 
 
 class ULSetEeveeSMAAQuality(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveessr.py` & `uplogic-2.2/uplogic/nodes/conditions/timer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-from bge import logic
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
+from uplogic.nodes import ULConditionNode
+from bge.logic import getRealTime
 
 
-class ULSetEeveeSSR(ULActionNode):
+class ULTimer(ULConditionNode):
 
     def __init__(self):
-        ULActionNode.__init__(self)
+        ULConditionNode.__init__(self)
         self.condition = None
-        self.value = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        self.delta_time = None
+        self._trigger = -1
+        self.network = None
+        self.OUT = self.add_output(self.get_out)
 
-    def get_done(self):
-        return self.done
+    def get_out(self):
+        return self.result
+
+    def setup(self, network):
+        self.network = network
 
     def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[scene.name].eevee.use_ssr = value
-        self.done = True
+        self.result = False
+        condition = self.get_input(self.condition)
+        delta_time = self.get_input(self.delta_time)
+        now = getRealTime()
+
+        if condition:
+            self._trigger = now + delta_time
+        if self._trigger == -1 or now < self._trigger:
+            self.result = False
+        else:
+            self.result = True
+            self._trigger = -1
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/seteeveevolumetrics.py` & `uplogic-2.2/uplogic/nodes/actions/setlightshadow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
+from bge.types import KX_GameObject
 
 
-class ULSetEeveeVolumetrics(ULActionNode):
+class ULSetLightShadow(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.value = None
+        self.lamp = None
+        self.use_shadow = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[
-            scene.name
-        ].eevee.use_volumetric_lights = value
+        light: KX_GameObject = self.get_input(self.lamp)
+        use_shadow = self.get_input(self.use_shadow)
+        light = light.blenderObject.data
+        light.use_shadow = use_shadow
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setexposure.py` & `uplogic-2.2/uplogic/nodes/actions/printvalue.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
+from uplogic.console import log
 
 
-class ULSetExposure(ULActionNode):
+class ULPrintValue(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.value = None
         self.done = None
+        self.msg_type = 'INFO'
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[
-            scene.name
-        ].view_settings.exposure = value
+        log(value, self.msg_type)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setfilterstate.py` & `uplogic-2.2/uplogic/nodes/actions/setfilterstate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.shaders import set_filter_state
 
 
 class ULSetFilterState(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setfullscreen.py` & `uplogic-2.2/uplogic/nodes/actions/setfullscreen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetFullscreen(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.use_fullscreen = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setgameobjectattr.py` & `uplogic-2.2/uplogic/nodes/actions/setgameobjectattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 
 
 class ULSetGameObjectAttribue(ULActionNode):
     def __init__(self, value_type='worldPosition'):
         ULActionNode.__init__(self)
         self.value_type = str(value_type)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setgamma.py` & `uplogic-2.2/uplogic/nodes/actions/stopallsounds.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,21 @@
-from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-import bpy
+from uplogic.data import GlobalDB
 
 
-class ULSetGamma(ULActionNode):
-
+class ULStopAllSounds(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.value = None
-        self.done = None
+        self.done = False
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        value = self.get_input(self.value)
-        scene = logic.getCurrentScene()
-        bpy.data.scenes[
-            scene.name
-        ].view_settings.gamma = value
+        aud_sys = GlobalDB.retrieve('uplogic.audio').get('default')
+        aud_sys.device.stopAll()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setglobalvalue.py` & `uplogic-2.2/uplogic/nodes/actions/vehicleapplyforce.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from uplogic.data import GlobalDB
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.physics import RWD
+from uplogic.utils.constants import VEHICLE
 
 
-class ULSetGlobalValue(ULActionNode):
-    def __init__(self):
+class ULVehicleApplyForce(ULActionNode):
+    def __init__(self, value_type=RWD):
         ULActionNode.__init__(self)
+        self.value_type = str(value_type)
         self.condition = None
-        self.data_id = None
-        self.key = None
-        self.value = None
-        self.persistent = None
-        self.done = None
+        self.vehicle = None
+        self.wheelcount = None
+        self._reset = False
+        self.power = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        data_id = self.get_input(self.data_id)
-        persistent = self.get_input(self.persistent)
-        key = self.get_input(self.key)
-        value = self.get_input(self.value)
-        db = GlobalDB.retrieve(data_id)
-        db.put(key, value, persistent)
+        game_object = self.get_input(self.vehicle)
+        vehicle = game_object.get(VEHICLE, None)
+        if vehicle is None:
+            return
+        value = self.get_input(self.value_type)
+        wheelcount = self.get_input(self.wheelcount)
+        power = self.get_input(self.power)
+        vehicle.accelerate(power, value, wheelcount)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setgravity.py` & `uplogic-2.2/uplogic/nodes/actions/setgravity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetGravity(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.scene = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setlightcolor.py` & `uplogic-2.2/uplogic/nodes/actions/setlightcolor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bge.types import KX_GameObject
 
 
 class ULSetLightColor(ULActionNode):
 
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setlightenergy.py` & `uplogic-2.2/uplogic/nodes/parameters/withinrange.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,29 @@
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from bge.types import KX_GameObject
+from uplogic.nodes import ULParameterNode
+from mathutils import Vector
 
 
-class ULSetLightEnergy(ULActionNode):
+class ULWithinRange(ULParameterNode):
 
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
-        self.lamp = None
-        self.energy = None
-        self.done = None
+        ULParameterNode.__init__(self)
+        self.value = None
+        self.range = None
+        self.min_value = None
+        self.max_value = None
+        self.operator = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
-        return self.done
+        v = self.get_input(self.value)
+        if self.min_value is not None:
+            r = Vector((self.get_input(self.min_value), self.get_input(self.max_value)))
+        else:
+            r = self.get_input(self.range)
+        value = self.calc_range(self.operator, v, r)
+        return value
 
-    def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        light: KX_GameObject = self.get_input(self.lamp)
-        energy = self.get_input(self.energy)
-        light = light.blenderObject.data
-        light.energy = energy
-        self.done = True
+    def calc_range(self, op, v, r):
+        if op == 'OUTSIDE':
+            return True if (v < r.x or v > r.y) else False
+        if op == 'INSIDE':
+            return True if (r.x < v < r.y) else False
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setlightshadow.py` & `uplogic-2.2/uplogic/nodes/actions/showframerate.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
+from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from bge.types import KX_GameObject
 
 
-class ULSetLightShadow(ULActionNode):
-
+class ULShowFramerate(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.lamp = None
-        self.use_shadow = None
+        self.use_framerate = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        light: KX_GameObject = self.get_input(self.lamp)
-        use_shadow = self.get_input(self.use_shadow)
-        light = light.blenderObject.data
-        light.use_shadow = use_shadow
+        use_framerate = self.get_input(self.use_framerate)
+        render.showFramerate(use_framerate)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setlistindex.py` & `uplogic-2.2/uplogic/nodes/actions/setlistindex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetListIndex(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.items: list = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setlogictreeproperty.py` & `uplogic-2.2/uplogic/nodes/actions/setlogictreeproperty.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/nodes/actions/setmaterial.py` & `uplogic-2.2/uplogic/nodes/actions/vehicleapplysteering.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import debug
-from bpy.types import Material
-from bge.types import KX_GameObject
+from uplogic.physics import RWD
+from uplogic.utils.constants import VEHICLE
 
 
-class ULSetMaterial(ULActionNode):
-    def __init__(self):
+class ULVehicleApplySteering(ULActionNode):
+    def __init__(self, value_type=RWD):
         ULActionNode.__init__(self)
+        self.value_type = str(value_type)
         self.condition = None
-        self.game_object = None
-        self.slot = None
-        self.mat_name = None
-        self.done = False
-        self.OUT = self.add_output(self._get_done)
+        self.vehicle = None
+        self.wheelcount = None
+        self._reset = False
+        self.power = None
+        self.OUT = self.add_output(self.get_done)
 
-    def _get_done(self):
+    def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object: KX_GameObject = self.get_input(self.game_object)
-        slot: int = self.get_input(self.slot)
-        material: Material = self.get_input(self.mat_name)
-        bl_obj = game_object.blenderObject
-        if slot > len(bl_obj.material_slots) - 1:
-            debug('Set Material: Slot does not exist!')
+        game_object = self.get_input(self.vehicle)
+        vehicle = game_object.get(VEHICLE, None)
+        if vehicle is None:
             return
-        bl_obj.material_slots[slot].material = material
+        value_type = self.get_input(self.value_type)
+        wheelcount = self.get_input(self.wheelcount)
+        power = self.get_input(self.power)
+        vehicle.steer(power, value_type, wheelcount)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setmatnodesocket.py` & `uplogic-2.2/uplogic/nodes/actions/setmatnodesocket.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 
 
 class ULSetMatNodeSocket(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setmatnodevalue.py` & `uplogic-2.2/uplogic/nodes/actions/setmatnodevalue.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 import bpy
 
 
 class ULSetMatNodeValue(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setnodesocket.py` & `uplogic-2.2/uplogic/nodes/actions/setcollisiongroup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from bpy.types import NodeTree
 
 
-class ULSetNodeSocket(ULActionNode):
+class ULSetCollisionGroup(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.tree_name = None
-        self.node_name = None
-        self.input_slot = None
-        self.value = None
-        self.done = False
-        self.OUT = self.add_output(self._get_done)
+        self.game_object = None
+        self.slots = None
+        self.mode = 0
+        self.done = None
+        self.OUT = self.add_output(self.get_done)
 
-    def _get_done(self):
+    def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        tree: NodeTree = self.get_input(self.tree_name)
-        node_name = self.get_input(self.node_name)
-        input_slot = self.get_input(self.input_slot)
-        value = self.get_input(self.value)
-        (
-            tree
-            .nodes[node_name]
-            .inputs[input_slot]
-            .default_value
-        ) = value
+        game_object = self.get_input(self.game_object)
+        slots = self.get_input(self.slots)
+        if self.mode:
+            game_object.collisionMask = slots
+        else:
+            game_object.collisionGroup = slots
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setnodevalue.py` & `uplogic-2.2/uplogic/nodes/actions/setnodevalue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import NodeTree
 import bpy
 
 
 class ULSetNodeValue(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setoverlaycollection.py` & `uplogic-2.2/uplogic/nodes/actions/setoverlaycollection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Collection
 from bge.types import KX_Camera
 
 class ULSetOverlayCollection(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setparent.py` & `uplogic-2.2/uplogic/nodes/actions/vehicleapplybraking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.physics import RWD
+from uplogic.utils.constants import VEHICLE
 
 
-class ULSetParent(ULActionNode):
-    def __init__(self):
+class ULVehicleApplyBraking(ULActionNode):
+    def __init__(self, value_type=RWD):
         ULActionNode.__init__(self)
+        self.value_type = str(value_type)
         self.condition = None
-        self.child_object = None
-        self.parent_object = None
-        self.compound = True
-        self.ghost = True
-        self.done = None
+        self.vehicle = None
+        self.wheelcount = None
+        self._reset = False
+        self.power = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        child_object = self.get_input(self.child_object)
-        parent_object = self.get_input(self.parent_object)
-        compound = self.get_input(self.compound)
-        ghost = self.get_input(self.ghost)
-        child_object.setParent(parent_object, compound, ghost)
+        game_object = self.get_input(self.vehicle)
+        vehicle = game_object.get(VEHICLE, None)
+        if vehicle is None:
+            return
+        value_type = self.get_input(self.value_type)
+        wheelcount = self.get_input(self.wheelcount)
+        power = self.get_input(self.power)
+        vehicle.brake(power, value_type, wheelcount)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setphysics.py` & `uplogic-2.2/uplogic/nodes/conditions/logictreestatus.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.nodes import ULConditionNode
 
 
-class ULSetPhysics(ULActionNode):
+class ULLogicTreeStatus(ULConditionNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
+        ULConditionNode.__init__(self)
         self.game_object = None
-        self.activate = False
-        self.free_const = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        self.tree_name = None
+        self._running = False
+        self._stopped = False
+        self.tree = None
+        self.IFRUNNING = self.add_output(self.get_running)
+        self.IFSTOPPED = self.add_output(self.get_stopped)
 
-    def get_done(self):
-        return self.done
+    def get_running(self):
+        tree = self.tree
+        if not tree:
+            return False
+        return tree.is_running()
+
+    def get_stopped(self):
+        tree = self.tree
+        if not tree:
+            return False
+        return tree.is_stopped()
 
     def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
         game_object = self.get_input(self.game_object)
-        activate = self.get_input(self.activate)
-        free_const = self.get_input(self.free_const)
-        if activate:
-            game_object.restorePhysics()
-        else:
-            game_object.suspendPhysics(free_const)
-        self.done = True
+        tree_name = self.get_input(self.tree_name)
+        self._running = False
+        self._stopped = False
+        self.tree = game_object.get(f'IGNLTree_{tree_name}')
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setprofile.py` & `uplogic-2.2/uplogic/nodes/actions/setprofile.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetProfile(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.use_profile = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setproperty.py` & `uplogic-2.2/uplogic/nodes/actions/toggleproperty.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetProperty(ULActionNode):
+class ULToggleProperty(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
         self.property_name = None
-        self.property_value = None
         self.mode = 0
         self.done = False
         self.OUT = self.add_output(self._get_done)
 
     def _get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
         property_name = self.get_input(self.property_name)
-        property_value = self.get_input(self.property_value)
-        self.done = True
         obj = game_object.blenderObject if self.mode else game_object
-        obj[property_name] = property_value
-        if self.mode:
-            obj.color = obj.color  # force object data refresh
+        value = obj.get(property_name)
+        obj[property_name] = not value
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setpyinstanceattr.py` & `uplogic-2.2/uplogic/nodes/actions/setpyinstanceattr.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 
 
 class ULSetPyInstanceAttr(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.instance = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setresolution.py` & `uplogic-2.2/uplogic/nodes/actions/setcamerafov.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-from bge import render
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetResolution(ULActionNode):
+class ULSetCameraFOV(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.x_res = None
-        self.y_res = None
+        self.camera = None
+        self.fov = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        x_res = self.get_input(self.x_res)
-        y_res = self.get_input(self.y_res)
-        render.setWindowSize(x_res, y_res)
+        camera = self.get_input(self.camera)
+        fov = self.get_input(self.fov)
+        camera.fov = fov
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setrigidbody.py` & `uplogic-2.2/uplogic/nodes/actions/setparent.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULSetRigidBody(ULActionNode):
+class ULSetParent(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_object = None
-        self.activate = False
+        self.child_object = None
+        self.parent_object = None
+        self.compound = True
+        self.ghost = True
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.game_object)
-        activate = self.get_input(self.activate)
-        if activate:
-            game_object.enableRigidBody()
-        else:
-            game_object.disableRigidBody()
+        child_object = self.get_input(self.child_object)
+        parent_object = self.get_input(self.parent_object)
+        compound = self.get_input(self.compound)
+        ghost = self.get_input(self.ghost)
+        child_object.setParent(parent_object, compound, ghost)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setscene.py` & `uplogic-2.2/uplogic/nodes/actions/setscene.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULActionNode
 from bge import logic
 from bpy.types import Scene
 
 
 class ULSetScene(ULActionNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setsensorvalue.py` & `uplogic-2.2/uplogic/nodes/actions/installsubnetwork.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULActionNode
 
 
-class ULSetSensorValue(ULActionNode):
-
+class ULInstallSubNetwork(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_obj = None
-        self.sens_name = None
-        self.field = None
-        self.value = None
+        self.target_object = None
+        self.tree_name = None
+        self.initial_status = None
+        self._network = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
+    def setup(self, network):
+        self._network = network
+
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_obj = self.get_input(self.game_obj)
-        sens_name = self.get_input(self.sens_name)
-        # sensor = game_obj.blenderObject.game.sensors.get(sens_name)
-        sensor = game_obj.sensors.get(sens_name)
-        if not sensor:
-            return
-        field = self.get_input(self.field)
-        value = self.get_input(self.value)
-        setattr(sensor, field, value)
+        target_object = self.get_input(self.target_object)
+        tree_name = self.get_input(self.tree_name)
+        initial_status = self.get_input(self.initial_status)
+        self._network.install_subnetwork(
+            target_object,
+            tree_name,
+            initial_status
+        )
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/settimescale.py` & `uplogic-2.2/uplogic/nodes/actions/settimescale.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSetTimeScale(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.scene = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setuiwidgetattr.py` & `uplogic-2.2/uplogic/nodes/actions/setuiwidgetattr.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import bpy
 
 attrs = {
     "show": 'bool_value',
     "color": 'color_value',
     "opacity": 'alpha_value',
     "pos": 'vec2_value',
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setvisibility.py` & `uplogic-2.2/uplogic/nodes/actions/setvisibility.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import logic
 from bpy.types import Collection
 from bge.types import KX_GameObject
 from bge.types import KX_Scene
 import bpy
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/setvsync.py` & `uplogic-2.2/uplogic/nodes/parameters/getresolution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from bge import render
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from mathutils import Vector
+from uplogic.nodes import ULParameterNode
 
 
-class ULSetVSync(ULActionNode):
+class ULGetResolution(ULParameterNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
-        self.vsync_mode = None
-        self.done = None
-        self.OUT = self.add_output(self.get_done)
+        ULParameterNode.__init__(self)
+        self.width = None
+        self.height = None
+        self.res = None
+        self.WIDTH = self.add_output(self.get_width)
+        self.HEIGHT = self.add_output(self.get_height)
+        self.RES = self.add_output(self.get_res)
 
-    def get_done(self):
-        return self.done
+    def get_width(self):
+        return render.getWindowWidth()
 
-    def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        render.setVsync(self.vsync_mode)
-        self.done = True
+    def get_height(self):
+        return render.getWindowHeight()
+
+    def get_res(self):
+        return Vector((self.width, self.height))
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/showframerate.py` & `uplogic-2.2/uplogic/nodes/actions/characterjump.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-from bge import render
+from bge import constraints
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULShowFramerate(ULActionNode):
+class ULCharacterJump(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.use_framerate = None
+        self.game_object = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        use_framerate = self.get_input(self.use_framerate)
-        render.showFramerate(use_framerate)
+        game_object = self.get_input(self.game_object)
+        physics = constraints.getCharacter(game_object)
+        physics.jump()
+
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/slowfollow.py` & `uplogic-2.2/uplogic/nodes/actions/slowfollow.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULSlowFollow(ULActionNode):
     def __init__(self, value_type='worldPosition'):
         ULActionNode.__init__(self)
         self.value_type = str(value_type)
         self.condition = NotImplementedError
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/spawnpool.py` & `uplogic-2.2/uplogic/nodes/actions/spawnpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.pooling import SpawnPool, Spawn, SimpleBullet, PhysicsBullet, SpawnedInstance
 from uplogic.events import send, receive
 from uplogic.utils import get_bitmask
 from bge.types import KX_GameObject
 
 
 class ULSpawnPool(ULActionNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/startsound.py` & `uplogic-2.2/uplogic/nodes/actions/startsound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.audio import Sound3D, Sound2D, Sample3D, Sample2D
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 
 
 class StartSoundNode(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = False
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/startsound2d.py` & `uplogic-2.2/uplogic/nodes/actions/startsound2d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.audio import Sound2D
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Sound
 
 
 class ULStartSound(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/startsound3d.py` & `uplogic-2.2/uplogic/nodes/actions/startsound3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from uplogic.audio import Sound3D
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 from bpy.types import Sound
 
 
 class ULStartSound3D(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/startspeaker.py` & `uplogic-2.2/uplogic/nodes/actions/startspeaker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bge import logic
 from uplogic.audio import Sound3D
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULStartSpeaker(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.occlusion = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/startsubnetwork.py` & `uplogic-2.2/uplogic/nodes/actions/startsubnetwork.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import make_valid_name
 
 
 class ULStartSubNetwork(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/stopaction.py` & `uplogic-2.2/uplogic/nodes/parameters/actionstatus.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 from uplogic.animation import ActionSystem
 from uplogic.data import GlobalDB
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.nodes import ULParameterNode
 
 
-class ULStopAction(ULActionNode):
-
+class ULActionStatus(ULParameterNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
+        ULParameterNode.__init__(self)
         self.game_object = None
         self.action_layer = None
-        self.done = None
+        self._action_name = None
+        self._action_frame = None
+        self.action = None
+        self._playing = False
         self.act_system = self.get_act_system()
-        self.OUT = self.add_output(self.get_done)
-        
+        self.OUT = self.add_output(self.get_out)
+        self.ACTION_NAME = self.add_output(self.get_action_name)
+        self.ACTION_FRAME = self.add_output(self.get_action_frame)
+
+    def get_out(self):
+        return bool(self.action and self.action.is_playing)
+
     def get_act_system(self):
         act_systems = GlobalDB.retrieve('uplogic.animation')
         if act_systems.check('default'):
             return act_systems.get('default')
         else:
             return ActionSystem('default')
 
-    def get_done(self):
-        return self.done
+    def get_action_name(self):
+        return self.action.name if self.action else None
+
+    def get_action_frame(self):
+        return self.action.frame if self.action else None
 
     def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
         game_object = self.get_input(self.game_object)
         action_layer = self.get_input(self.action_layer)
-
-        action = self.act_system.get_layer(game_object, action_layer)
-        if action is not None:
-            self.act_system.remove(action)
-        self.done = True
+        self.action = self.act_system.get_layer(game_object, action_layer)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/stopallsounds.py` & `uplogic-2.2/uplogic/nodes/conditions/mousepressed.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,18 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
-from uplogic.data import GlobalDB
+from uplogic.nodes import ULConditionNode
+from uplogic.input import mouse_tap
+from uplogic.input import mouse_down
+from uplogic.input import mouse_up
 
 
-class ULStopAllSounds(ULActionNode):
+class ULMousePressed(ULConditionNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
-        self.done = False
-        self.OUT = self.add_output(self.get_done)
+        ULConditionNode.__init__(self)
+        self.pulse = False
+        self.input_type = 1 if self.pulse else 0
+        self.mouse_button_code = None
+        self.OUT = self.add_output(self.get_pressed)
 
-    def get_done(self):
-        return self.done
-
-    def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        aud_sys = GlobalDB.retrieve('uplogic.audio').get('default')
-        aud_sys.device.stopAll()
-        self.done = True
+    def get_pressed(self):
+        mouse_button = self.get_input(self.mouse_button_code)
+        funcs = [mouse_tap, mouse_down, mouse_up]
+        return funcs[self.input_type](mouse_button)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/stopsound.py` & `uplogic-2.2/uplogic/nodes/actions/pausesound.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
+from uplogic.audio.sound import ULSound
 
 
-class ULStopSound(ULActionNode):
+class ULPauseSound(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.sound = None
         self.done = False
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        sound = self.get_input(self.sound)
-        sound.stop()
+        sound: ULSound = self.get_input(self.sound)
+        sound.pause()
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/stopsubnetwork.py` & `uplogic-2.2/uplogic/nodes/actions/seteeveeao.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,25 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import make_valid_name
+import bpy
 
 
-class ULStopSubNetwork(ULActionNode):
+class ULSetEeveeAO(ULActionNode):
+
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.game_object = None
-        self.logic_network_name = None
+        self.value = None
         self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.game_object)
-        logic_network_name = self.get_input(self.logic_network_name)
-        tree_name = make_valid_name(logic_network_name)
-        network = game_object.get(f'IGNLTree_{tree_name}')
-        if network is None:
-            return
-        network.stop()
+        value = self.get_input(self.value)
+        scene = logic.getCurrentScene()
+        bpy.data.scenes[scene.name].eevee.use_gtao = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/togglefilter.py` & `uplogic-2.2/uplogic/nodes/conditions/keypressed.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.shaders import toggle_filter
+from uplogic.nodes import ULConditionNode
+from uplogic.input import key_tap
+from uplogic.input import key_down
+from uplogic.input import key_up
 
 
-class ULToggleFilter(ULActionNode):
+class ULKeyPressed(ULConditionNode):
     def __init__(self):
-        ULActionNode.__init__(self)
-        self.condition = None
-        self.pass_idx = None
-        self.done = False
-        self.OUT = self.add_output(self._get_done)
+        ULConditionNode.__init__(self)
+        self.pulse = False
+        self.input_type = 1 if self.pulse else 0
+        self.key_code = 0
+        self.network = None
+        self.OUT = self.add_output(self.get_pressed)
 
-    def _get_done(self):
-        return self.done
-
-    def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        pass_idx = self.get_input(self.pass_idx)
-        toggle_filter(pass_idx)
-        self.done = True
+    def get_pressed(self):
+        keycode = self.get_input(self.key_code)
+        funcs = [key_tap, key_down, key_up]
+        return funcs[self.input_type](keycode)
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/toggleproperty.py` & `uplogic-2.2/uplogic/nodes/actions/applymovement.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULToggleProperty(ULActionNode):
+class ULApplyMovement(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
         self.game_object = None
-        self.property_name = None
-        self.mode = 0
-        self.done = False
-        self.OUT = self.add_output(self._get_done)
+        self.movement = None
+        self.done = None
+        self.OUT = self.add_output(self.get_done)
 
-    def _get_done(self):
+    def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
         game_object = self.get_input(self.game_object)
-        property_name = self.get_input(self.property_name)
-        obj = game_object.blenderObject if self.mode else game_object
-        value = obj.get(property_name)
-        obj[property_name] = not value
+        movement = self.get_input(self.movement)
+        local = self.local
+        if movement:
+            game_object.applyMovement(movement, local)
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/translate.py` & `uplogic-2.2/uplogic/nodes/actions/applyforce.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
-from uplogic.nodes import ULActionNode, ULOutSocket
+from uplogic.nodes import ULActionNode
 
 
-class ULTranslate(ULActionNode):
+class ULApplyForce(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.condition = None
-        self.moving_object = None
-        self.local = None
-        self.vect = None
-        self.speed = None
-        self._t = None
-        self._old_values = None
+        self.game_object = None
+        self.force = None
+        self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
-        print('"Translate" node is deprecated!')
+        self.done = False
+        if not self.get_input(self.condition):
+            return
+        game_object = self.get_input(self.game_object)
+        force = self.get_input(self.force)
+        local = self.local
+        game_object.applyForce(force, local)
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/vectoranglecheck.py` & `uplogic-2.2/uplogic/nodes/actions/vectoranglecheck.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULActionNode
 from uplogic.utils.constants import LOGIC_OPERATORS
 import math
 
 
 class ULVectorAngleCheck(ULActionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/vehicleapplybraking.py` & `uplogic-2.2/uplogic/nodes/actions/rotateto.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.physics import RWD
-from uplogic.utils.constants import VEHICLE
+from uplogic.utils import rotate_to
 
 
-class ULVehicleApplyBraking(ULActionNode):
-    def __init__(self, value_type=RWD):
+class ULActionRotateTo(ULActionNode):
+    def __init__(self):
         ULActionNode.__init__(self)
-        self.value_type = str(value_type)
         self.condition = None
-        self.vehicle = None
-        self.wheelcount = None
-        self._reset = False
-        self.power = None
-        self.OUT = self.add_output(self.get_done)
+        self.moving_object = None
+        self.target_point = None
+        self.speed = None
+        self._done = False
+        self.rot_axis = 2
+        self.front_axis = 0
+        self.OUT = self.add_output(self._get_done)
 
-    def get_done(self):
-        return self.done
+    def _get_done(self):
+        return self._done
 
     def evaluate(self):
-        self.done = False
+        self._done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.vehicle)
-        vehicle = game_object.get(VEHICLE, None)
-        if vehicle is None:
-            return
-        value_type = self.get_input(self.value_type)
-        wheelcount = self.get_input(self.wheelcount)
-        power = self.get_input(self.power)
-        vehicle.brake(power, value_type, wheelcount)
-        self.done = True
+        moving_object = self.get_input(self.moving_object)
+        target_point = self.get_input(self.target_point)
+        speed = self.get_input(self.speed)
+        rot_axis = self.get_input(self.rot_axis)
+        front_axis = self.get_input(self.front_axis)
+        rotate_to(moving_object, target_point, rot_axis, front_axis, speed)
+        self._done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/vehicleapplyforce.py` & `uplogic-2.2/uplogic/nodes/parameters/objectattr.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.physics import RWD
-from uplogic.utils.constants import VEHICLE
+from mathutils import Vector
+from uplogic.nodes import ULParameterNode
 
 
-class ULVehicleApplyForce(ULActionNode):
-    def __init__(self, value_type=RWD):
-        ULActionNode.__init__(self)
-        self.value_type = str(value_type)
-        self.condition = None
-        self.vehicle = None
-        self.wheelcount = None
-        self._reset = False
-        self.power = None
+class ULObjectAttribute(ULParameterNode):
+    def __init__(self):
+        ULParameterNode.__init__(self)
+        self.game_object = None
+        self.attribute_name = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
-        return self.done
-
-    def evaluate(self):
-        self.done = False
-        if not self.get_input(self.condition):
-            return
-        game_object = self.get_input(self.vehicle)
-        vehicle = game_object.get(VEHICLE, None)
-        if vehicle is None:
-            return
-        value = self.get_input(self.value_type)
-        wheelcount = self.get_input(self.wheelcount)
-        power = self.get_input(self.power)
-        vehicle.accelerate(power, value, wheelcount)
-        self.done = True
+        game_object = self.get_input(self.game_object)
+        attribute_name = self.get_input(self.attribute_name)
+        if not hasattr(game_object, attribute_name):
+            return Vector((0, 0, 0))
+        val = getattr(game_object, attribute_name)
+        return val.copy() if isinstance(val, Vector) else val
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/vehicleapplysteering.py` & `uplogic-2.2/uplogic/nodes/actions/setexposure.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,27 @@
+from bge import logic
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.physics import RWD
-from uplogic.utils.constants import VEHICLE
+import bpy
 
 
-class ULVehicleApplySteering(ULActionNode):
-    def __init__(self, value_type=RWD):
+class ULSetExposure(ULActionNode):
+
+    def __init__(self):
         ULActionNode.__init__(self)
-        self.value_type = str(value_type)
         self.condition = None
-        self.vehicle = None
-        self.wheelcount = None
-        self._reset = False
-        self.power = None
+        self.value = None
+        self.done = None
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
         return self.done
 
     def evaluate(self):
         self.done = False
         if not self.get_input(self.condition):
             return
-        game_object = self.get_input(self.vehicle)
-        vehicle = game_object.get(VEHICLE, None)
-        if vehicle is None:
-            return
-        value_type = self.get_input(self.value_type)
-        wheelcount = self.get_input(self.wheelcount)
-        power = self.get_input(self.power)
-        vehicle.steer(power, value_type, wheelcount)
+        value = self.get_input(self.value)
+        scene = logic.getCurrentScene()
+        bpy.data.scenes[
+            scene.name
+        ].view_settings.exposure = value
         self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/actions/vehiclesetattributes.py` & `uplogic-2.2/uplogic/nodes/actions/vehiclesetattributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.constants import VEHICLE
 from uplogic.physics import FWD
 from uplogic.physics import RWD
 from uplogic.physics import FOURWD
 
 
 class ULVehicleSetAttributes(ULActionNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/__init__.py` & `uplogic-2.2/uplogic/nodes/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/nodes/conditions/barrier.py` & `uplogic-2.2/uplogic/nodes/conditions/barrier.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 from bge.logic import getRealTime
 
 
 class ULBarrier(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/checkdistance.py` & `uplogic-2.2/uplogic/nodes/conditions/checkdistance.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
 from uplogic.utils.constants import LOGIC_OPERATORS
 from mathutils import Vector
 
 
 class ULCheckDistance(ULConditionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/collision.py` & `uplogic-2.2/uplogic/nodes/conditions/collision.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from bge.types import KX_GameObject
 from uplogic.nodes import ULConditionNode
 from uplogic.nodes import ULLogicContainer
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 from mathutils import Vector
 
 
 class ULCollision(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/compare.py` & `uplogic-2.2/uplogic/nodes/conditions/compare.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.constants import LOGIC_OPERATORS
 
 
 class ULCompare(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.operator = 'GREATER'
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/comparevectors.py` & `uplogic-2.2/uplogic/nodes/conditions/comparevectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.constants import LOGIC_OPERATORS
 
 
 class ULCompareVectors(ULConditionNode):
     def __init__(self, operator='GREATER'):
         ULConditionNode.__init__(self)
         self.operator = operator
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/controllerstatus.py` & `uplogic-2.2/uplogic/nodes/conditions/controllerstatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 
 
 class ULControllerStatus(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/evaluateproperty.py` & `uplogic-2.2/uplogic/nodes/conditions/evaluateproperty.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
 
 
 class ULEvaluateProperty(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/gamepadactive.py` & `uplogic-2.2/uplogic/nodes/conditions/gamepadactive.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/nodes/conditions/gamepadbutton.py` & `uplogic-2.2/uplogic/nodes/conditions/gamepadbutton.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.input import gamepad_tap
 from uplogic.input import gamepad_down
 from uplogic.input import gamepad_up
 
 
 class ULGamepadButton(ULConditionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/gamepadbuttonup.py` & `uplogic-2.2/uplogic/nodes/conditions/gamepadbuttonup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULGamepadButtonUp(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.pulse = False
         self.button = 0
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/handleevent.py` & `uplogic-2.2/uplogic/nodes/conditions/handleevent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from uplogic.events import receive
 from uplogic.events import ULEvent
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULHandleEvent(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.subject = None
         self.event = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/hasproperty.py` & `uplogic-2.2/uplogic/nodes/parameters/getproperty.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
-from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.nodes import ULOutSocket, ULParameterNode
 
 
-class ULHasProperty(ULConditionNode):
+class ULGetProperty(ULParameterNode):
     def __init__(self):
-        ULConditionNode.__init__(self)
+        ULParameterNode.__init__(self)
         self.game_object = None
         self.property_name = None
         self.mode = 0
-        self.OUT = self.add_output(self.get_stat)
+        self.OUT = self.add_output(self.get_property)
 
-    def get_stat(self):
+    def get_property(self):
         game_object = self.get_input(self.game_object)
         property_name = self.get_input(self.property_name)
-        return (
-            property_name in [p[0] for p in game_object.blenderObject.items()]
+        props = (
+            [p[0] for p in game_object.blenderObject.items()]
             if self.mode else
-            property_name in game_object.getPropertyNames()
+            game_object.getPropertyNames()
         )
+        if property_name in props:
+            obj = game_object if self.mode in [0, 'GAME'] else game_object.blenderObject
+            return obj.get(property_name)
+        game_object[property_name] = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/keypressed.py` & `uplogic-2.2/uplogic/nodes/parameters/getlogictreeproperty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,17 @@
-from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.input import key_tap
-from uplogic.input import key_down
-from uplogic.input import key_up
+from uplogic.nodes import ULOutSocket, ULParameterNode
+from uplogic.utils import make_valid_name
+from bpy.types import Object
 
 
-class ULKeyPressed(ULConditionNode):
+class ULGetLogicTreeProperty(ULParameterNode):
     def __init__(self):
-        ULConditionNode.__init__(self)
-        self.pulse = False
-        self.input_type = 1 if self.pulse else 0
-        self.key_code = 0
-        self.network = None
-        self.OUT = self.add_output(self.get_pressed)
+        ULParameterNode.__init__(self)
+        self.property_name = None
+        self.OUT = self.add_output(self.get_property)
 
-    def get_pressed(self):
-        keycode = self.get_input(self.key_code)
-        funcs = [key_tap, key_down, key_up]
-        return funcs[self.input_type](keycode)
+    def get_property(self):
+        property_name = self.get_input(self.property_name)
+        result = getattr(self.network.component, make_valid_name(property_name).lower(), False)
+        if isinstance(result, Object):
+            result = self.network.scene.getGameObjectFromObject(result)
+        return result
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/keyreleased.py` & `uplogic-2.2/uplogic/nodes/conditions/keyreleased.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 from bge.logic import keyboard
 
 
 class ULKeyReleased(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.pulse = False
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/logicand.py` & `uplogic-2.2/uplogic/nodes/conditions/logicand.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 
 
 class ULAnd(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.ca = None
         self.cb = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/logicgate.py` & `uplogic-2.2/uplogic/nodes/conditions/logicgate.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULLogicGate(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.ca = None
         self.cb = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/logicgatelist.py` & `uplogic-2.2/uplogic/nodes/conditions/logicgatelist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
 
 
 class ULLogicGateList(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/logicor.py` & `uplogic-2.2/uplogic/nodes/conditions/logicor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 
 
 class ULOr(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.ca = False
         self.cb = False
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/logictreestatus.py` & `uplogic-2.2/uplogic/nodes/conditions/timedelay.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
+from bge.logic import getRealTime
 
 
-class ULLogicTreeStatus(ULConditionNode):
+class ULTimeDelay(ULConditionNode):
+
     def __init__(self):
         ULConditionNode.__init__(self)
-        self.game_object = None
-        self.tree_name = None
-        self._running = False
-        self._stopped = False
-        self.tree = None
-        self.IFRUNNING = self.add_output(self.get_running)
-        self.IFSTOPPED = self.add_output(self.get_stopped)
-
-    def get_running(self):
-        tree = self.tree
-        if not tree:
-            return False
-        return tree.is_running()
+        self.condition = None
+        self.delay = None
+        self.triggers = []
+        self.result = False
+        self.OUT = self.add_output(self.get_out)
 
-    def get_stopped(self):
-        tree = self.tree
-        if not tree:
-            return False
-        return tree.is_stopped()
+    def get_out(self):
+        return self.result
 
     def evaluate(self):
-        game_object = self.get_input(self.game_object)
-        tree_name = self.get_input(self.tree_name)
-        self._running = False
-        self._stopped = False
-        self.tree = game_object.get(f'IGNLTree_{tree_name}')
+        self.result = False
+        condition = self.get_input(self.condition)
+        delay = self.get_input(self.delay)
+        now = getRealTime()
+        if condition:
+            self.triggers.append(now + delay)
+        if not self.triggers:
+            return
+        t = self.triggers[0]
+        if now >= t:
+            self.result = True
+            self.triggers.pop(0)
+            return
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/mouseover.py` & `uplogic-2.2/uplogic/nodes/conditions/mouseover.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.raycasting import raycast_mouse
 
 
 class ULMouseOver(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/mousepressed.py` & `uplogic-2.2/uplogic/nodes/conditions/mousepressedon.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+from bge import logic
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
-from uplogic.input import mouse_tap
-from uplogic.input import mouse_down
-from uplogic.input import mouse_up
+from uplogic.utils.raycasting import raycast_mouse
 
 
-class ULMousePressed(ULConditionNode):
+class ULMousePressedOn(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
-        self.pulse = False
-        self.input_type = 1 if self.pulse else 0
-        self.mouse_button_code = None
-        self.OUT = self.add_output(self.get_pressed)
+        self.game_object = None
+        self.mouse_button = None
+        self.OUT = self.add_output(self.get_changed)
 
-    def get_pressed(self):
-        mouse_button = self.get_input(self.mouse_button_code)
-        funcs = [mouse_tap, mouse_down, mouse_up]
-        return funcs[self.input_type](mouse_button)
+    def get_changed(self):
+        mouse_button = self.get_input(self.mouse_button)
+        game_object = self.get_input(self.game_object)
+        mstat = logic.mouse.inputs[mouse_button]
+        if not mstat.activated:
+            return False
+        mpos = logic.mouse.position
+        camera = logic.getCurrentScene().active_camera
+        vec = 10 * camera.getScreenVect(*mpos)
+        ray_target = camera.worldPosition - vec
+        distance = camera.getDistanceTo(game_object) * 2.0
+        dat = raycast_mouse(distance=distance)
+        return dat.obj == game_object
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/mousereleased.py` & `uplogic-2.2/uplogic/nodes/conditions/mousereleased.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 from bge import logic
 
 
 class ULMouseReleased(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.pulse = False
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/mousescroll.py` & `uplogic-2.2/uplogic/nodes/conditions/mousescroll.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULMouseScrolled(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.wheel_direction = 0
         self.OUT = self.add_output(self.get_wheel)
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/once.py` & `uplogic-2.2/uplogic/nodes/conditions/once.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 
 
 class ULOnce(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
         self.input_condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/onnexttick.py` & `uplogic-2.2/uplogic/nodes/conditions/onnexttick.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
+from uplogic.nodes import ULConditionNode
 
 
 class ULOnNextTick(ULConditionNode):
 
     def __init__(self):
         ULConditionNode.__init__(self)
         self.input_condition = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/onvaluechanged.py` & `uplogic-2.2/uplogic/nodes/actions/stopaction.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
+from uplogic.animation import ActionSystem
+from uplogic.data import GlobalDB
+from uplogic.nodes import ULActionNode
 
 
-class ULOnValueChanged(ULConditionNode):
+class ULStopAction(ULActionNode):
+
     def __init__(self):
-        ULConditionNode.__init__(self)
-        self.old = None
-        self.new = None
-        self.current_value = None
-        self.initialize = False
-        self.OUT = self.add_output(self.get_changed)
-        self.OLD = self.add_output(
-            self.get_previous_value
-        )
-        self.NEW = self.add_output(self.get_current_value)
-
-    def get_changed(self):
-        curr = self.get_input(self.current_value)
-        if not self.initialize:
-            self.initialize = True
-            self.old = self.new = curr
-            return False
-        elif self.old != curr:
-            self.new = curr
-            return True
-
-    def get_previous_value(self):
-        return self.old
-
-    def get_current_value(self):
-        return self.new
-
-    def reset(self):
-        super().reset()
-        self.old = self.new
+        ULActionNode.__init__(self)
+        self.condition = None
+        self.game_object = None
+        self.action_layer = None
+        self.done = None
+        self.act_system = self.get_act_system()
+        self.OUT = self.add_output(self.get_done)
+        
+    def get_act_system(self):
+        act_systems = GlobalDB.retrieve('uplogic.animation')
+        if act_systems.check('default'):
+            return act_systems.get('default')
+        else:
+            return ActionSystem('default')
+
+    def get_done(self):
+        return self.done
+
+    def evaluate(self):
+        self.done = False
+        if not self.get_input(self.condition):
+            return
+        game_object = self.get_input(self.game_object)
+        action_layer = self.get_input(self.action_layer)
+
+        action = self.act_system.get_layer(game_object, action_layer)
+        if action is not None:
+            self.act_system.remove(action)
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/onvaluechangedto.py` & `uplogic-2.2/uplogic/nodes/conditions/onvaluechangedto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULConditionNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULValueChangedTo(ULConditionNode):
     def __init__(self):
         ULConditionNode.__init__(self)
         self.monitored_value = None
         self.trigger_value = None
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/pulsify.py` & `uplogic-2.2/uplogic/nodes/actions/setsensorvalue.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
-from bge.logic import getRealTime
+from uplogic.nodes import ULActionNode
 
 
-class ULPulsify(ULConditionNode):
+class ULSetSensorValue(ULActionNode):
+
     def __init__(self):
-        ULConditionNode.__init__(self)
+        ULActionNode.__init__(self)
         self.condition = None
-        self.delay = None
-        self.result = False
-        self._old_time = getRealTime()
-        self._time = 0.0
-        self.OUT = self.add_output(self.get_out)
+        self.game_obj = None
+        self.sens_name = None
+        self.field = None
+        self.value = None
+        self.done = None
+        self.OUT = self.add_output(self.get_done)
 
-    def get_out(self):
-        return self.result
+    def get_done(self):
+        return self.done
 
     def evaluate(self):
-        self.result = False
-        now = getRealTime()
+        self.done = False
         if not self.get_input(self.condition):
-            self._time = 0.0
-            self._old_time = now
             return
-        if self._time <= 0.0:
-            self.result = True
-            self._time = self.get_input(self.delay)
-        self._time -= now - self._old_time
-        self._old_time = now
-        
+        game_obj = self.get_input(self.game_obj)
+        sens_name = self.get_input(self.sens_name)
+        # sensor = game_obj.blenderObject.game.sensors.get(sens_name)
+        sensor = game_obj.sensors.get(sens_name)
+        if not sensor:
+            return
+        field = self.get_input(self.field)
+        value = self.get_input(self.value)
+        setattr(sensor, field, value)
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/timedelay.py` & `uplogic-2.2/uplogic/nodes/parameters/resizevector.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,31 +1,34 @@
-from uplogic.nodes import ULConditionNode, ULOutSocket
-from bge.logic import getRealTime
+from uplogic.nodes import ULParameterNode
+from mathutils import Vector, Matrix
+import bpy
+from bge import logic
 
 
-class ULTimeDelay(ULConditionNode):
-
+class ResizeVectorNode(ULParameterNode):
     def __init__(self):
-        ULConditionNode.__init__(self)
-        self.condition = None
-        self.delay = None
-        self.triggers = []
-        self.result = False
-        self.OUT = self.add_output(self.get_out)
-
-    def get_out(self):
-        return self.result
-
-    def evaluate(self):
-        self.result = False
-        condition = self.get_input(self.condition)
-        delay = self.get_input(self.delay)
-        now = getRealTime()
-        if condition:
-            self.triggers.append(now + delay)
-        if not self.triggers:
-            return
-        t = self.triggers[0]
-        if now >= t:
-            self.result = True
-            self.triggers.pop(0)
-            return
+        ULParameterNode.__init__(self)
+        self.vec_in = Vector((0, 0, 0))
+        self._to_size = 3
+        self.funcs = [
+            self.get_2D_vec,
+            self.get_3D_vec,
+            self.get_4D_vec
+        ]
+
+    @property
+    def to_size(self):
+        return self._to_size
+
+    @to_size.setter
+    def to_size(self, val):
+        self.OUT = self.add_output(self.funcs[val])
+        self._to_size = val
+
+    def get_2D_vec(self):
+        return self.get_input(self.vec_in).to_2d()
+
+    def get_3D_vec(self):
+        return self.get_input(self.vec_in).to_3d()
+
+    def get_4D_vec(self):
+        return self.get_input(self.vec_in).to_4d()
```

### Comparing `uplogic-2.1/uplogic/nodes/conditions/vectoranglecheck.py` & `uplogic-2.2/uplogic/nodes/conditions/vectoranglecheck.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULConditionNode
 from uplogic.utils.constants import LOGIC_OPERATORS
 import math
 
 
 class ULVectorAngleCheck(ULConditionNode):
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/logictree.py` & `uplogic-2.2/uplogic/nodes/logictree.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         self.aud_system_owner = False
         self.init_glob_cats()
         self.audio_system = self.get_aud_system()
         self.sub_networks = []  # a list of networks updated by this network
         self.capslock_pressed = False
         self.evaluated_cells = 0
         scene = self.scene = logic.getCurrentScene()
-        mainloop = scene.get('uplogic.mainloop')
+        mainloop = logic.globalDict.get('loop')
         if mainloop:
             mainloop.logic_tree = self
 
     def get_aud_system(self):
         aud_sys = GlobalDB.retrieve('uplogic.audio').get('default')
         if not aud_sys:
             self.aud_system_owner = True
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/__init__.py` & `uplogic-2.2/uplogic/nodes/parameters/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,9 +97,12 @@
 from .serializedata import ULSerializeData
 from .rebuilddata import ULRebuildData
 from .fpsfactor import ULFPSFactor
 from .instream import ULKeyLogger
 from .rotatebypoint import ULRotateByPoint
 from .getlogictreeproperty import ULGetLogicTreeProperty
 from .resizevector import ResizeVectorNode
+from .curveinterpolation import CurveInterpolationNode
+from .tweenvalue import TweenValueNode
+from .getcollisiongroup import GetCollisionGroupNode
 
 from .randomvalue import ULRandomValue
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/actionstatus.py` & `uplogic-2.2/uplogic/nodes/parameters/characterinfo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,48 @@
-from uplogic.animation import ActionSystem
-from uplogic.data import GlobalDB
-from uplogic.nodes import ULOutSocket
+from bge import constraints
+from bge import logic
 from uplogic.nodes import ULParameterNode
+import bpy
 
 
-class ULActionStatus(ULParameterNode):
+class ULCharacterInfo(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
-        self.action_layer = None
-        self._action_name = None
-        self._action_frame = None
-        self.action = None
-        self._playing = False
-        self.act_system = self.get_act_system()
-        self.OUT = self.add_output(self.get_out)
-        self.ACTION_NAME = self.add_output(self.get_action_name)
-        self.ACTION_FRAME = self.add_output(self.get_action_frame)
-
-    def get_out(self):
-        return bool(self.action and self.action.is_playing)
-
-    def get_act_system(self):
-        act_systems = GlobalDB.retrieve('uplogic.animation')
-        if act_systems.check('default'):
-            return act_systems.get('default')
-        else:
-            return ActionSystem('default')
+        self.max_jumps = None
+        self.cur_jump = None
+        self.gravity = None
+        self.walk_dir = None
+        self.on_ground = None
+        self.local = False
+        self.MAX_JUMPS = self.add_output(self.get_max_jumps)
+        self.CUR_JUMP = self.add_output(self.get_current_jump)
+        self.GRAVITY = self.add_output(self.get_gravity)
+        self.WALKDIR = self.add_output(self.get_walk_dir)
+        self.ON_GROUND = self.add_output(self.get_on_ground)
+
+    def get_max_jumps(self):
+        return self.physics.maxJumps
+
+    def get_current_jump(self):
+        return self.physics.jumpCount
+
+    def get_gravity(self):
+        return self.physics.gravity
+
+    def get_walk_dir(self):
+        physics = self.physics
+        wdir = (
+            physics.walkDirection @ self.owner.worldOrientation
+            if self.local else
+            physics.walkDirection
+        )
+        return wdir * bpy.data.scenes[
+            logic.getCurrentScene().name
+        ].game_settings.physics_step_sub
 
-    def get_action_name(self):
-        return self.action.name if self.action else None
-
-    def get_action_frame(self):
-        return self.action.frame if self.action else None
+    def get_on_ground(self):
+        return self.physics.onGround
 
     def evaluate(self):
-        game_object = self.get_input(self.game_object)
-        action_layer = self.get_input(self.action_layer)
-        self.action = self.act_system.get_layer(game_object, action_layer)
+        game_object = self.owner = self.get_input(self.game_object)
+        self.physics = constraints.getCharacter(game_object)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/bonestatus.py` & `uplogic-2.2/uplogic/nodes/parameters/bonestatus.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import logic
 from mathutils import Euler
 from mathutils import Quaternion
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULBoneStatus(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.armature = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/characterinfo.py` & `uplogic-2.2/uplogic/nodes/parameters/rotatebypoint.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,67 @@
-from bge import constraints
-from bge import logic
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
-import bpy
+from uplogic.utils.math import rotate2d
+from uplogic.utils.math import rotate3d
+from uplogic.utils.math import rotate_by_axis
+from uplogic.utils.math import rotate_by_euler
+from mathutils import Vector
+from math import degrees
 
 
-class ULCharacterInfo(ULParameterNode):
+class ULRotateByPoint(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.game_object = None
-        self.max_jumps = None
-        self.cur_jump = None
-        self.gravity = None
-        self.walk_dir = None
-        self.on_ground = None
-        self.local = False
-        self.MAX_JUMPS = self.add_output(self.get_max_jumps)
-        self.CUR_JUMP = self.add_output(self.get_current_jump)
-        self.GRAVITY = self.add_output(self.get_gravity)
-        self.WALKDIR = self.add_output(self.get_walk_dir)
-        self.ON_GROUND = self.add_output(self.get_on_ground)
-
-    def get_max_jumps(self):
-        return self.physics.maxJumps
-
-    def get_current_jump(self):
-        return self.physics.jumpCount
-
-    def get_gravity(self):
-        return self.physics.gravity
-
-    def get_walk_dir(self):
-        physics = self.physics
-        wdir = (
-            physics.walkDirection @ self.owner.worldOrientation
-            if self.local else
-            physics.walkDirection
+        # self.mode = 0
+        self.global_axis = 0
+        self.origin = None
+        self.pivot = None
+        self.angle = None
+        self.arbitrary_axis = None
+        self.euler_angles = None
+        self.OUT = self.add_output(self.get_point)
+        self._operations = [
+            self._rotate2d,
+            self._rotate3d,
+            self._rotate_by_axis,
+            self._rotate_by_euler
+        ]
+
+    @property
+    def mode(self):
+        return None
+
+    @mode.setter
+    def mode(self, val):
+        self.OUT._value_getter = self._operations[val]
+
+    def _rotate2d(self):
+        return rotate2d(
+            self.get_input(self.origin),
+            self.get_input(self.pivot),
+            degrees(self.get_input(self.angle))
         )
-        return wdir * bpy.data.scenes[
-            logic.getCurrentScene().name
-        ].game_settings.physics_step_sub
-
-    def get_on_ground(self):
-        return self.physics.onGround
-
-    def evaluate(self):
-        game_object = self.owner = self.get_input(self.game_object)
-        self.physics = constraints.getCharacter(game_object)
+
+    def _rotate3d(self):
+        return rotate3d(
+            self.get_input(self.origin),
+            self.get_input(self.pivot),
+            degrees(self.get_input(self.angle)),
+            self.global_axis
+        )
+
+    def _rotate_by_axis(self):
+        return rotate_by_axis(
+            self.get_input(self.origin),
+            self.get_input(self.pivot),
+            degrees(self.get_input(self.angle)),
+            self.get_input(self.arbitrary_axis)
+        )
+
+    def _rotate_by_euler(self):
+        return rotate_by_euler(
+            self.get_input(self.origin),
+            self.get_input(self.pivot),
+            self.get_input(self.euler_angles)
+        )
+
+    def get_point(self):
+        return Vector((0, 0, 0))
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/childbyindex.py` & `uplogic-2.2/uplogic/nodes/parameters/childbyname.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-from bge.types import KX_GameObject as GameObject
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
+from bge.types import KX_GameObject
 
 
-class ULChildByIndex(ULParameterNode):
+class ULChildByName(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.from_parent: GameObject = None
-        self.index: int = None
+        self.from_parent = None
+        self.child = None
         self.CHILD = self.add_output(self.get_child)
 
     def get_child(self):
-        parent: GameObject = self.get_input(self.from_parent)
-        index: int = self.get_input(self.index)
-        if len(parent.children) > index:
-            return parent.children[index]
+        parent: KX_GameObject = self.get_input(self.from_parent)
+        child: KX_GameObject = self.get_input(self.child)
+        return parent.childrenRecursive.get(child.name)
+
+    def evaluate(self):
+        pass
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/childbyname.py` & `uplogic-2.2/uplogic/nodes/parameters/vectorxyz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from uplogic.nodes import ULOutSocket
+from mathutils import Vector
 from uplogic.nodes import ULParameterNode
-from bge.types import KX_GameObject
 
 
-class ULChildByName(ULParameterNode):
+class ULVectorXYZ(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.from_parent = None
-        self.child = None
-        self.CHILD = self.add_output(self.get_child)
+        self.input_x = None
+        self.input_y = None
+        self.input_z = None
+        self.OUTV = self.add_output(self.get_out_v)
 
-    def get_child(self):
-        parent: KX_GameObject = self.get_input(self.from_parent)
-        child: KX_GameObject = self.get_input(self.child)
-        return parent.childrenRecursive.get(child.name)
+    def get_out_v(self):
+        return Vector((
+            self.get_input(self.input_x),
+            self.get_input(self.input_y),
+            self.get_input(self.input_z)
+        ))
 
-    def evaluate(self):
-        pass
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/clamp.py` & `uplogic-2.2/uplogic/nodes/parameters/clamp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 
 
 class ULClamp(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/dictvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/dictvalue.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULDictValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.dict = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/euler.py` & `uplogic-2.2/uplogic/nodes/parameters/euler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Euler
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULEuler(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.input_x = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/eulertomatrix.py` & `uplogic-2.2/uplogic/nodes/parameters/vectorxyzw.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from mathutils import Euler
-from mathutils import Matrix
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
-class ULEulerToMatrix(ULParameterNode):
+class ULVectorXYZW(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.input_e = None
-        self.matrix = Matrix()
-        self.OUT = self.add_output(self.get_matrix)
+        self.input_x = None
+        self.input_y = None
+        self.input_z = None
+        self.input_w = None
+        self.OUTV = self.add_output(self.get_out_v)
 
-    def get_matrix(self):
-        vec = self.get_input(self.input_e)
-        if isinstance(vec, Vector):
-            vec = Euler((vec.x, vec.y, vec.z), 'XYZ')
-        return vec.to_matrix()
+    def get_out_v(self):
+        return Vector((
+            self.get_input(self.input_x),
+            self.get_input(self.input_y),
+            self.get_input(self.input_z),
+            self.get_input(self.input_w)
+        ))
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/formattedstring.py` & `uplogic-2.2/uplogic/nodes/parameters/formattedstring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULFormattedString(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.format_string = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/formula.py` & `uplogic-2.2/uplogic/nodes/parameters/formula.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 import math
 
 
 class ULFormula(ULParameterNode):
 
     @classmethod
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/gamepadsticks.py` & `uplogic-2.2/uplogic/nodes/parameters/gamepadsticks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic, types
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 
 
 class ULGamepadSticks(ULParameterNode):
     def __init__(self, axis=0):
         ULParameterNode.__init__(self)
         self.axis = axis
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/gamepadtrigger.py` & `uplogic-2.2/uplogic/nodes/parameters/gamepadtrigger.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from bge import logic
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 
 
 class ULGamepadTrigger(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.index = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getactuatorvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/getactuatorvalue.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULGetActuatorValue(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getcollectionobjects.py` & `uplogic-2.2/uplogic/nodes/actions/removeoverlaycollection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,23 @@
-from uplogic.nodes import ULOutSocket
-from uplogic.nodes import ULParameterNode
-from bpy.types import Collection
-from bge.logic import getCurrentScene
+from bge import logic
+from uplogic.nodes import ULActionNode
 
 
-class ULGetCollectionObjects(ULParameterNode):
+class ULRemoveOverlayCollection(ULActionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
+        ULActionNode.__init__(self)
+        self.condition = None
         self.collection = None
-        self.OUT = self.add_output(self.get_objects)
+        self.done = False
+        self.OUT = self.add_output(self.get_done)
 
-    def get_objects(self):
-        collection: Collection = self.get_input(self.collection)
-        scene = getCurrentScene()
-        return [scene.getGameObjectFromObject(o) for o in collection.objects]
+    def get_done(self):
+        return self.done
+
+    def evaluate(self):
+        self.done = False
+        if not self.get_input(self.condition):
+            return
+        logic.getCurrentScene().removeOverlayCollection(
+            self.get_input(self.collection)
+        )
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getcurvepoints.py` & `uplogic-2.2/uplogic/nodes/parameters/getcurvepoints.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULGetCurvePoints(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.curve = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getglobalvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/getglobalvalue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.data import GlobalDB
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULGetGlobalValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.data_id = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getlogictreeproperty.py` & `uplogic-2.2/uplogic/nodes/parameters/timedata.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,31 @@
-from uplogic.nodes import ULOutSocket, ULParameterNode
-from uplogic.utils import make_valid_name
-from bpy.types import Object
+from uplogic.nodes import ULParameterNode
+from uplogic.nodes.logictree import ULLogicTree
+from bge import logic
 
 
-class ULGetLogicTreeProperty(ULParameterNode):
+class ULTimeData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.property_name = None
-        self.OUT = self.add_output(self.get_property)
+        self.network: ULLogicTree = None
+        self.TIME_PER_FRAME = self.add_output(
+            self.get_time_per_frame
+        )
+        self.FPS = self.add_output(self.get_fps)
+        self.TIMELINE = self.add_output(self.get_timeline)
 
-    def get_property(self):
-        property_name = self.get_input(self.property_name)
-        result = getattr(self.network.component, make_valid_name(property_name).lower(), False)
-        if isinstance(result, Object):
-            result = self.network.scene.getGameObjectFromObject(result)
-        return result
+    def get_time_per_frame(self):
+        return self.network.time_per_frame
+
+    def get_fps(self):
+        tpf = self.network.time_per_frame or 1
+        fps = logic.getAverageFrameRate()
+        return fps if fps < 500 else 1 / tpf
+
+    def get_timeline(self):
+        return logic.getRealTime()
+
+    def setup(self, network):
+        self.network = network
+
+    def evaluate(self):
+        pass
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getnodeattribute.py` & `uplogic-2.2/uplogic/nodes/parameters/getnodeattribute.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import NodeTree
 
 
 class ULGetNodeAttribute(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.mat_name = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getnodesocket.py` & `uplogic-2.2/uplogic/nodes/parameters/getnodesocket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import NodeTree
 
 
 class ULGetNodeSocket(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.tree_name = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getproperty.py` & `uplogic-2.2/uplogic/nodes/conditions/hasproperty.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,19 @@
-from uplogic.nodes import ULOutSocket, ULParameterNode
+from uplogic.nodes import ULConditionNode
 
 
-class ULGetProperty(ULParameterNode):
+class ULHasProperty(ULConditionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
+        ULConditionNode.__init__(self)
         self.game_object = None
         self.property_name = None
         self.mode = 0
-        self.OUT = self.add_output(self.get_property)
+        self.OUT = self.add_output(self.get_stat)
 
-    def get_property(self):
+    def get_stat(self):
         game_object = self.get_input(self.game_object)
         property_name = self.get_input(self.property_name)
-        props = (
-            [p[0] for p in game_object.blenderObject.items()]
+        return (
+            property_name in [p[0] for p in game_object.blenderObject.items()]
             if self.mode else
-            game_object.getPropertyNames()
+            property_name in game_object.getPropertyNames()
         )
-        if property_name in props:
-            obj = game_object if self.mode in [0, 'GAME'] else game_object.blenderObject
-            return obj.get(property_name)
-        game_object[property_name] = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getresolution.py` & `uplogic-2.2/uplogic/nodes/parameters/vectorsplitxyz.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from bge import render
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
-class ULGetResolution(ULParameterNode):
+class ULVectorSplitXYZ(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.width = None
-        self.height = None
-        self.res = None
-        self.WIDTH = self.add_output(self.get_width)
-        self.HEIGHT = self.add_output(self.get_height)
-        self.RES = self.add_output(self.get_res)
+        self.input_v = None
+        self.output_v = Vector()
+        self.OUTX = self.add_output(self.get_out_x)
+        self.OUTY = self.add_output(self.get_out_y)
+        self.OUTZ = self.add_output(self.get_out_z)
 
-    def get_width(self):
-        return render.getWindowWidth()
+    def get_out_x(self):
+        return self.output_v.x
 
-    def get_height(self):
-        return render.getWindowHeight()
+    def get_out_y(self):
+        return self.output_v.y
 
-    def get_res(self):
-        return Vector((self.width, self.height))
+    def get_out_z(self):
+        return self.output_v.z
+
+    def evaluate(self):
+        vec = self.get_input(self.input_v)
+        self.output_v = vec
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getsensorvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/getsensorvalue.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from bge.types import KX_GameObject as GameObject
 
 
 class ULGetSensorValue(ULParameterNode):
 
     def __init__(self):
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/getuiwidgetattr.py` & `uplogic-2.2/uplogic/nodes/parameters/getuiwidgetattr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULGetUIWidgetAttr(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.widget = None
         self.widget_attr = 'show'
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/instream.py` & `uplogic-2.2/uplogic/nodes/parameters/instream.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/nodes/parameters/interpolate.py` & `uplogic-2.2/uplogic/nodes/parameters/maprange.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,27 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils import lerp
+from uplogic.utils.math import map_range, map_range_vector
 
 
-class ULInterpolate(ULParameterNode):
+class ULMapRange(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.a = None
-        self.b = None
-        self.fac = None
+        self.value = None
+        self.from_min = None
+        self.from_max = None
+        self.to_min = None
+        self.to_max = None
+        self.clamp = False
+        self.mode = 0
+        self.operations = [map_range, map_range_vector]
         self.OUT = self.add_output(self.get_done)
 
     def get_done(self):
-        a = self.get_input(self.a)
-        b = self.get_input(self.b)
-        fac = self.get_input(self.fac)
-        return lerp(a, b, fac)
+        return self.operations[self.mode](
+            self.get_input(self.value),
+            self.get_input(self.from_min),
+            self.get_input(self.from_max),
+            self.get_input(self.to_min),
+            self.get_input(self.to_max),
+            self.clamp
+        )
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/limitrange.py` & `uplogic-2.2/uplogic/nodes/parameters/limitrange.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULLimitRange(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
         self.value = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/listextend.py` & `uplogic-2.2/uplogic/nodes/parameters/listextend.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULListExtend(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.list_1: list = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/loadvariable.py` & `uplogic-2.2/uplogic/nodes/parameters/loadvariable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 import bpy
 import json
 import os
 
 
 class ULLoadVariable(ULParameterNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/loadvariabledict.py` & `uplogic-2.2/uplogic/nodes/parameters/loadvariabledict.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils import debug
 import bpy
 import json
 import os
 
 
 class ULLoadVariableDict(ULParameterNode):
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/maprange.py` & `uplogic-2.2/uplogic/nodes/parameters/materialgetattribute.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
-from uplogic.utils.math import map_range, map_range_vector
+from bpy.types import Material
+import bpy
 
 
-class ULMapRange(ULParameterNode):
-
+class ULGetMaterialAttribute(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.value = None
-        self.from_min = None
-        self.from_max = None
-        self.to_min = None
-        self.to_max = None
-        self.clamp = False
-        self.mode = 0
-        self.operations = [map_range, map_range_vector]
-        self.OUT = self.add_output(self.get_done)
+        self.mat_name = None
+        self.node_name = None
+        self.internal = None
+        self.attribute = None
+        self.OUT = self.add_output(self._get_val)
 
-    def get_done(self):
-        return self.operations[self.mode](
-            self.get_input(self.value),
-            self.get_input(self.from_min),
-            self.get_input(self.from_max),
-            self.get_input(self.to_min),
-            self.get_input(self.to_max),
-            self.clamp
+    def _get_val(self):
+        material: Material = self.get_input(self.mat_name)
+        node_name = self.get_input(self.node_name)
+        internal = self.get_input(self.internal)
+        attribute = self.get_input(self.attribute)
+        target = (
+            material
+            .node_tree
+            .nodes[node_name]
         )
+        if internal:
+            target = getattr(target, internal, target)
+        return getattr(target, attribute, None)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/materialgetnode.py` & `uplogic-2.2/uplogic/nodes/parameters/materialgetnode.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 import bpy
 
 
 class ULGetMaterialNode(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/materialgetsocket.py` & `uplogic-2.2/uplogic/nodes/parameters/materialgetsocket.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from bpy.types import Material
 
 
 class ULGetMaterialSocket(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.mat_name = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/math.py` & `uplogic-2.2/uplogic/nodes/parameters/math.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULMath(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
         self.operand_a = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/matrixtoxyz.py` & `uplogic-2.2/uplogic/nodes/parameters/matrixtoxyz.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULMatrixToXYZ(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.input_m = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/mousedata.py` & `uplogic-2.2/uplogic/nodes/parameters/mousedata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULMouseData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.MX = self.add_output(self.getmx)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/objectattr.py` & `uplogic-2.2/uplogic/nodes/parameters/vectorsplitxy.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from mathutils import Vector
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
-class ULObjectAttribute(ULParameterNode):
+class ULVectorSplitXY(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.game_object = None
-        self.attribute_name = None
-        self.OUT = self.add_output(self.get_done)
+        self.input_v = None
+        self.output_v = Vector((0, 0))
+        self.OUTX = self.add_output(self.get_out_x)
+        self.OUTY = self.add_output(self.get_out_y)
 
-    def get_done(self):
-        game_object = self.get_input(self.game_object)
-        attribute_name = self.get_input(self.attribute_name)
-        if not hasattr(game_object, attribute_name):
-            return Vector((0, 0, 0))
-        val = getattr(game_object, attribute_name)
-        return val.copy() if isinstance(val, Vector) else val
+    def get_out_x(self):
+        return self.output_v.x
+
+    def get_out_y(self):
+        return self.output_v.y
+
+    def evaluate(self):
+        vec = self.get_input(self.input_v)
+        self.output_v = vec
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/objectdatavertices.py` & `uplogic-2.2/uplogic/nodes/parameters/objectdatavertices.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 
 
 class ULObjectDataVertices(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.game_object = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/randomfloat.py` & `uplogic-2.2/uplogic/nodes/parameters/randomint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
+
+
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
-import sys
 import random
+import sys
 
 
-class ULRandomFloat(ULParameterNode):
+class ULRandomInt(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.max_value = None
         self.min_value = None
         self.OUT_A = self.add_output(self._get_output)
 
     def _get_output(self):
         min_value = self.get_input(self.min_value)
         max_value = self.get_input(self.max_value)
         if min_value > max_value:
             min_value, max_value = max_value, min_value
         if min_value == max_value:
-            min_value = sys.float_info.min
-            max_value = sys.float_info.max
+            min_value = -sys.maxsize
+            max_value = sys.maxsize
 
-        delta = max_value - min_value
-        return min_value + (delta * random.random())
+        return random.randint(min_value, max_value)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/randomvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/randomvalue.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from random import randint
 from random import random
 from random import uniform
 from mathutils import Vector
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/randomvect.py` & `uplogic-2.2/uplogic/nodes/parameters/randomvect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from mathutils import Vector
 from uplogic.nodes import ULActionNode
-from uplogic.nodes import ULOutSocket
 import random
 
 
 class ULRandomVect(ULActionNode):
     def __init__(self):
         ULActionNode.__init__(self)
         self.xyz = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/rangedthreshold.py` & `uplogic-2.2/uplogic/nodes/conditions/pulsify.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
-from mathutils import Vector
+from uplogic.nodes import ULConditionNode
+from bge.logic import getRealTime
 
 
-class ULRangedThreshold(ULParameterNode):
-
+class ULPulsify(ULConditionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
-        self.value = None
-        self.threshold = None
-        self.min_value = None
-        self.max_value = None
-        self.operator = None
-        self.OUT = self.add_output(self.get_done)
+        ULConditionNode.__init__(self)
+        self.condition = None
+        self.delay = None
+        self.result = False
+        self._old_time = getRealTime()
+        self._time = 0.0
+        self.OUT = self.add_output(self.get_out)
 
-    def get_done(self):
-        v = self.get_input(self.value)
-        if self.min_value is not None:
-            t = Vector((self.get_input(self.min_value), self.get_input(self.max_value)))
-        else:
-            t = self.get_input(self.threshold)
-        value = self.calc_threshold(self.operator, v, t)
-        return value
+    def get_out(self):
+        return self.result
 
-    def calc_threshold(self, op, v, t):
-        if op == 'OUTSIDE':
-            return v if (v < t.x or v > t.y) else 0
-        if op == 'INSIDE':
-            return v if (t.x < v < t.y) else 0
+    def evaluate(self):
+        self.result = False
+        now = getRealTime()
+        if not self.get_input(self.condition):
+            self._time = 0.0
+            self._old_time = now
+            return
+        if self._time <= 0.0:
+            self.result = True
+            self._time = self.get_input(self.delay)
+        self._time -= now - self._old_time
+        self._old_time = now
+
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/rebuilddata.py` & `uplogic-2.2/uplogic/nodes/parameters/rebuilddata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector, Matrix
 import bpy
 from bge import logic
 
 
 class ULRebuildData(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
+        self.condition = True
         self.data = None
         self.read_as = 'builtin'
         self.ret = None
         self.dattypes = {
             'Vec2': Vector,
             'Vec3': Vector,
             'Vec4': Vector,
@@ -20,24 +20,24 @@
         }
         self.OUT = self.add_output(self.get_data)
 
     def get_data(self):
         return self.ret
 
     def evaluate(self):
+        if not self.get_input(self.condition):
+            return
         dat = self.get_input(self.data)
         if dat is None:
             return
         if self.read_as == 'builtin':
             self.ret = dat
             return
         if self.read_as == 'GameObj':
             bobj = bpy.data.objects.get(dat['name'])
-            # obj = logic.getCurrentScene().objects.get(dat['data_id'])
-            # print(dat['data_id'])
             if bobj is None:
                 self.ret = None
                 return
             obj = logic.getCurrentScene().getGameObjectFromObject(bobj)
             for attr in dat:
                 if attr == 'properties':
                     for prop in dat[attr]:
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/threshold.py` & `uplogic-2.2/uplogic/nodes/parameters/threshold.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULThreshold(ULParameterNode):
 
     def __init__(self):
         ULParameterNode.__init__(self)
         self.value = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/typecastvalue.py` & `uplogic-2.2/uplogic/nodes/parameters/typecastvalue.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULTypeCastValue(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.value = None
         self.to_type = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/valueswitch.py` & `uplogic-2.2/uplogic/nodes/parameters/valueswitch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from uplogic.utils.constants import LOGIC_OPERATORS
 
 
 class ULValueSwitch(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.conditon = None
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/vectormath.py` & `uplogic-2.2/uplogic/nodes/parameters/vectormath.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 from mathutils import Vector
 
 
 class ULVectorMath(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.op = None
@@ -12,35 +11,35 @@
         self.factor = None
         self.scale = None
         self.vector_3 = None
         self.ior = None
         self.OUT = self.add_output(self.get_done)
         self.VOUT = self.add_output(self.get_done)
         self.calculations = {
+            'add': self.get_add,
+            'subtract': self.get_subtract,
+            'multiply': self.get_multiply,
+            'divide': self.get_divide,
+            'multadd': self.get_multadd,
+            'matmul': self.get_matmul,
             'scale': self.get_scale,
             'length': self.get_length,
             'distance': self.get_distance,
-            'angle': self.get_angle,
-            'angle_signed': self.get_angle_signed,
             'dot': self.get_dot,
-            'faceforward': self.get_faceforward,
+            'angle': self.get_angle,
             'refract': self.get_refract,
             'reflect': self.get_reflect,
+            'angle_signed': self.get_angle_signed,
+            'faceforward': self.get_faceforward,
             'project': self.get_project,
             'cross': self.get_cross,
-            'multadd': self.get_multadd,
-            'divide': self.get_divide,
-            'multiply': self.get_multiply,
-            'subtract': self.get_subtract,
-            'add': self.get_add,
-            'matmul': self.get_matmul,
             'normalize': self.get_normalize,
             'lerp': self.get_lerp,
             'slerp': self.get_slerp,
-            'negate': self.get_negate,
+            'negate': self.get_negate
         }
 
     def get_done(self):
         op = self.get_input(self.op)
         vector = self.get_input(self.vector)
         vector_2 = self.get_input(self.vector_2)
         vector_3 = self.get_input(self.vector_3)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/vectorsplitxy.py` & `uplogic-2.2/uplogic/nodes/parameters/vectorangle.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from mathutils import Vector
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
+import math
 
 
-class ULVectorSplitXY(ULParameterNode):
+class ULVectorAngle(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
-        self.input_v = None
-        self.output_v = Vector((0, 0))
-        self.OUTX = self.add_output(self.get_out_x)
-        self.OUTY = self.add_output(self.get_out_y)
+        self.op = None
+        self.vector: Vector = None
+        self.vector_2: Vector = None
+        self.OUT = self.add_output(self.get_done)
 
-    def get_out_x(self):
-        return self.output_v.x
-
-    def get_out_y(self):
-        return self.output_v.y
-
-    def evaluate(self):
-        vec = self.get_input(self.input_v)
-        self.output_v = vec
+    def get_done(self):
+        vector: Vector = self.get_input(self.vector)
+        vector_2: Vector = self.get_input(self.vector_2)
+        rad: float = vector.angle(vector_2)
+        deg: float = rad * 180/math.pi
+        return deg
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/vectorxyzw.py` & `uplogic-2.2/uplogic/nodes/actions/setnodesocket.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-from mathutils import Vector
-from uplogic.nodes import ULOutSocket
-from uplogic.nodes import ULParameterNode
+from uplogic.nodes import ULActionNode
+from bpy.types import NodeTree
 
 
-class ULVectorXYZW(ULParameterNode):
+class ULSetNodeSocket(ULActionNode):
     def __init__(self):
-        ULParameterNode.__init__(self)
-        self.input_x = None
-        self.input_y = None
-        self.input_z = None
-        self.input_w = None
-        self.OUTV = self.add_output(self.get_out_v)
+        ULActionNode.__init__(self)
+        self.condition = None
+        self.tree_name = None
+        self.node_name = None
+        self.input_slot = None
+        self.value = None
+        self.done = False
+        self.OUT = self.add_output(self._get_done)
 
-    def get_out_v(self):
-        return Vector((
-            self.get_input(self.input_x),
-            self.get_input(self.input_y),
-            self.get_input(self.input_z),
-            self.get_input(self.input_w)
-        ))
+    def _get_done(self):
+        return self.done
+
+    def evaluate(self):
+        self.done = False
+        if not self.get_input(self.condition):
+            return
+        tree: NodeTree = self.get_input(self.tree_name)
+        node_name = self.get_input(self.node_name)
+        input_slot = self.get_input(self.input_slot)
+        value = self.get_input(self.value)
+        (
+            tree
+            .nodes[node_name]
+            .inputs[input_slot]
+            .default_value
+        ) = value
+        self.done = True
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/vrcontrollervalues.py` & `uplogic-2.2/uplogic/nodes/parameters/vrcontrollervalues.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from uplogic.nodes import ULOutSocket
 from uplogic.nodes import ULParameterNode
 from uplogic.input import VRController
 
 
 class ULGetVRControllerValues(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
```

### Comparing `uplogic-2.1/uplogic/nodes/parameters/worldposition.py` & `uplogic-2.2/uplogic/nodes/parameters/worldposition.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from uplogic.nodes import ULParameterNode
-from uplogic.nodes import ULOutSocket
 
 
 class ULWorldPosition(ULParameterNode):
     def __init__(self):
         ULParameterNode.__init__(self)
         self.camera = None
         self.screen_x = None
```

### Comparing `uplogic-2.1/uplogic/physics/__init__.py` & `uplogic-2.2/uplogic/physics/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/physics/buoyancy.py` & `uplogic-2.2/uplogic/physics/buoyancy.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,34 +39,34 @@
     def update(self):
         if not self._active:
             return
         up = Vector((0, 0, 1))
         flotsam = self.game_object
         lindamp = .1
         wpos = flotsam.worldPosition
-        obj, point, normal, direction = raycast(
+        ray = raycast(
             flotsam,
             wpos,
             up,
             self.height,
             WATER,
             xray=True,
             local=True,
             visualize=True
         )
-        if obj:
+        if ray.obj:
             lindamp = .8
-            lift = (up * (wpos - point).length * self.buoyancy)
+            lift = (up * (wpos - ray.point).length * self.buoyancy)
             flotsam.applyImpulse(
                 wpos,
                 vec_clamp(lift, max=self.buoyancy),
                 False
             )
             if self.align:
-                self.game_object.alignAxisToVect(normal, 2, .2)
+                self.game_object.alignAxisToVect(ray.normal, 2, .2)
         flotsam.linearDamping = lindamp
         flotsam.angularDamping = lindamp * .8
 
     def destroy(self):
         logic.getCurrentScene().pre_draw.remove(self.update)
 
 
@@ -101,28 +101,28 @@
         ship = self.game_object
         max_lin_damp = .9 - self.linear_damping
         max_ang_damp = .8 - self.linear_damping
         lin_dampen_factor = 0
         ang_dampen_factor = 0
         for buoy in self.buoys:
             wpos = buoy.worldPosition
-            obj, point, normal, direction = raycast(
+            ray = raycast(
                 buoy,
                 wpos,
                 up,
                 self.height,
                 WATER,
                 xray=True,
                 local=True
             )
-            if obj:
+            if ray.obj:
                 div = 1 / lifts
                 lin_dampen_factor += (max_lin_damp * div)
                 ang_dampen_factor += (max_ang_damp * div)
-                lift = (up * (wpos - point).length * self.buoyancy) * div
+                lift = (up * (wpos - ray.point).length * self.buoyancy) * div
                 ship.applyImpulse(
                     wpos,
                     vec_clamp(lift, max=self.buoyancy * 2 * div),
                     False
                 )
         ship.linearDamping = self.linear_damping + lin_dampen_factor
         ship.angularDamping = self.angular_damping + ang_dampen_factor
```

### Comparing `uplogic-2.1/uplogic/physics/character.py` & `uplogic-2.2/uplogic/physics/character.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from bge import logic
 from bge.constraints import getCharacter
 from bge.types import KX_GameObject as GameObject
 from uplogic.utils.constants import FRAMETIME_COMPARE
-# from uplogic.logging import warning
 from mathutils import Vector
 import bpy
 
 
 class ULCharacter():
     _deprecated = True
```

### Comparing `uplogic-2.1/uplogic/physics/collision.py` & `uplogic-2.2/uplogic/physics/collision.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/physics/constraints.py` & `uplogic-2.2/uplogic/physics/constraints.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/physics/vehicle.py` & `uplogic-2.2/uplogic/physics/vehicle.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/serialize/__init__.py` & `uplogic-2.2/uplogic/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/__init__.py` & `uplogic-2.2/uplogic/shaders/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,13 +10,16 @@
 from .mist import Mist
 from .levels import Levels
 from .letterbox import Letterbox
 from .distort import Distort
 from .droplets import Droplets
 from .blur import Blur
 from .dof import DoF
+from .lens import Lens
+from .texture import Texture
 from .chromaticaberration import ChromaticAberration
 from .sharpen import Sharpen
+from .splitscreen import SplitScreen
 from .shader import load_glsl
 from .shader import remove_filter
 from .shader import toggle_filter
 from .shader import set_filter_state
```

### Comparing `uplogic-2.1/uplogic/shaders/adaptivetonemapping.py` & `uplogic-2.2/uplogic/shaders/adaptivetonemapping.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/blur.py` & `uplogic-2.2/uplogic/shaders/blur.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,17 +39,18 @@
 			color += texture(bgl_RenderedTexture, uv+vec2(cos(d),sin(d)) * radius * i);
         }
     }
     color /= quality * samples - 15.0;
     fragColor = color;
 }"""
 
+
 class Blur(Filter2D):
 
-    def __init__(self, samples=16, power=1.0, idx: int = None) -> None:
+    def __init__(self, power=1.0, samples=16, idx: int = None) -> None:
        self.settings = {'samples': float(samples), 'power': float(power)}
        super().__init__(glsl, idx, {'samples': self.settings, 'power': self.settings})
 
     @property
     def samples(self):
         return self.settings['samples']
```

### Comparing `uplogic-2.1/uplogic/shaders/brightness.py` & `uplogic-2.2/uplogic/shaders/brightness.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/buffer.py` & `uplogic-2.2/uplogic/shaders/buffer.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,31 +6,49 @@
 
 in vec4 bgl_TexCoord;
 uniform float gamma;
 out vec4 fragColor;
 
 void main()
 {
-    fragColor = pow(texture(bgl_RenderedTexture, bgl_TexCoord.xy), vec4(gamma)) * pow(1, 2);
+    fragColor = pow(texture(bgl_RenderedTexture, bgl_TexCoord.xy), vec4(gamma));
 }
 """
 
 
 class Buffer(Filter2D):
 
-    def __init__(self, gamma=1, exposure=0, idx: int = None) -> None:
+    def __init__(self, gamma=1, idx: int = None) -> None:
         self.settings = {'gamma': float(gamma)}
         super().__init__(glsl, idx, {'gamma': self.settings})
         self._filter.addOffScreen(0)
 
     @property
     def bindcode(self):
         return self._filter.offScreen.colorBindCodes[0]
 
     @property
     def texture(self):
         return self._filter.offScreen.getColorTexture()
 
-    @property
-    def depth_texture(self):
-        return self._filter.offScreen.getDepthTexture()
+
+depth_glsl = """
+uniform sampler2D bgl_DepthTexture;
+
+in vec4 bgl_TexCoord;
+uniform float gamma;
+out vec4 fragColor;
+
+void main()
+{
+    fragColor = pow(texture(bgl_DepthTexture, bgl_TexCoord.xy), vec4(gamma));
+}
+"""
+
+
+class DepthBuffer(Buffer):
+
+    def __init__(self, gamma=1, idx: int = None) -> None:
+        self.settings = {'gamma': float(gamma)}
+        super().__init__(depth_glsl, idx, {'gamma': self.settings})
+        self._filter.addOffScreen(0)
```

### Comparing `uplogic-2.1/uplogic/shaders/chromaticaberration.py` & `uplogic-2.2/uplogic/shaders/chromaticaberration.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,25 +2,27 @@
 
 glsl = """
 uniform sampler2D bgl_RenderedTexture;
 in vec4 bgl_TexCoord;
 
 uniform float power;
 
+out vec4 fragColor;
+
 void main()
 {
    vec2 texcoord = bgl_TexCoord.xy;
    vec3 sum = vec3(0.0);
    vec3 distance = vec3(1.0-(power*0.01), 1.0-(power*0.02), 1.0-(power*0.03));
 
    sum.r = vec3(texture(bgl_RenderedTexture, (texcoord -vec2(0.5,0.5)) * distance[0] + vec2(0.5,0.5))).r;
    sum.g = vec3(texture(bgl_RenderedTexture, (texcoord -vec2(0.5,0.5)) * distance[1] + vec2(0.5,0.5))).g;
    sum.b = vec3(texture(bgl_RenderedTexture, (texcoord -vec2(0.5,0.5)) * distance[2] + vec2(0.5,0.5))).b;
 
-   gl_FragColor = vec4(sum, 1.0);
+   fragColor = vec4(sum, 1.0);
 }
 """
 
 
 class ChromaticAberration(Filter2D):
 
     def __init__(self, power: float = 2.0, idx: int = None) -> None:
```

### Comparing `uplogic-2.1/uplogic/shaders/distort.py` & `uplogic-2.2/uplogic/shaders/droplets.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from .shader import Filter2D
 from bge import logic
+from mathutils import Vector
 
 
 glsl = """
 /* Original Code by martins upitis @youtube: https://www.youtube.com/watch?v=UkskiSza4p0
 Modified by Iza Zed for uplogic
 */
 
 in vec4 bgl_TexCoord;
 #define gl_TexCoord glTexCoord
 vec4 glTexCoord[4] = vec4[](bgl_TexCoord,bgl_TexCoord,bgl_TexCoord,bgl_TexCoord);
 
 out vec4 fragColor;
-#define gl_FragColor fragColor
-
 
 uniform sampler2D bgl_RenderedTexture;
 uniform float bgl_RenderedTextureWidth;
 uniform float bgl_RenderedTextureHeight;
 
-uniform float timer, resettimer, randomtime, power;
+uniform float timer, time, randomtime, blur;
+uniform vec3 color;
 
 vec2 texcoord = vec2(gl_TexCoord[0]).st;
 
 const float permTexUnit = 1.0/256.0;		// Perm texture texel-size
 const float permTexUnitHalf = 0.5/256.0;	// Half perm texture texel-size
 
 float width = bgl_RenderedTextureWidth;
@@ -38,14 +38,36 @@
     float noiseG =  fract(noise*1.2154)*2.0-1.0; 
     float noiseB =  fract(noise*1.3453)*2.0-1.0;
     float noiseA =  fract(noise*1.3647)*2.0-1.0;
     
     return vec4(noiseR,noiseG,noiseB,noiseA);
 }
 
+vec3 fblur(vec2 uv){
+    float samples = 16;
+    vec2 resolution = vec2(bgl_RenderedTextureWidth, bgl_RenderedTextureHeight);
+    float Pi = 6.28318530718;
+
+    float quality = 3.0;
+   
+    vec2 radius = blur/resolution.xy;
+
+    vec3 frag = texture(bgl_RenderedTexture, uv).rgb;
+
+    for( float d=0.0; d<Pi; d+=Pi/samples)
+    {
+		for(float i = 1.0/quality; i<=1.0; i+=1.0/quality)
+        {
+			frag += texture(bgl_RenderedTexture, uv+vec2(cos(d),sin(d)) * radius * i).rgb;
+        }
+    }
+    frag /= quality * samples - 15.0;
+    return frag;
+}
+
 float fade(in float t) {
     return t*t*t*(t*(t*6.0-15.0)+10.0);
 }
 
 float pnoise3D(in vec3 p)
 {
     vec3 pi = permTexUnit*floor(p)+permTexUnitHalf; // Integer part, scaled so +1 moves permTexUnit texel
@@ -98,131 +120,145 @@
     float rotX = ((tc.x*2.0-1.0)*(width/height)*cos(angle)) - ((tc.y*2.0-1.0)*sin(angle));
     float rotY = ((tc.y*2.0-1.0)*cos(angle)) + ((tc.x*2.0-1.0)*(width/height)*sin(angle));
     rotX = ((rotX/(width/height))*0.5+0.5);
     rotY = rotY*0.5+0.5;
     return vec2(rotX,rotY);
 }
 
-
-
 void main(void)
 {
-    vec4 original = gl_FragColor = texture2D(bgl_RenderedTexture, texcoord);
+    if (time > 10){
+        fragColor = texture(bgl_RenderedTexture, texcoord);
+        return;
+    }
     float grainsize = 100.0;
-    //texture edge bleed removal
     float fade = 12;
     vec2 distortFade = vec2(0.0);
     distortFade.s = clamp(texcoord.s*fade,0.0,1.0);
     distortFade.s -= clamp(1.0-(1.0-texcoord.s)*fade,0.0,1.0);
     distortFade.t = clamp(texcoord.t*fade,0.0,1.0);
     distortFade.t -= clamp(1.0-(1.0-texcoord.t)*fade,0.0,1.0); 
 
     vec2 rotCoordsR = texcoord;
     
     float dfade = 1.0-pow((1.0-distortFade.s*distortFade.t),2.0);
     float noiz = 0.0;
     float drop = 0.0;
 
-    float resettimerslow = resettimer*0.02;
-    float resettimerfaster = resettimer*0.5;
+    float timeslow = time*0.02;
+    float timefaster = time*0.5;
     
-    if (resettimer > 0.0 && resettimer < 4.0)
+    if (time > 0.0 && time < 4.0)
     {
-    //noiz += pnoise3D(vec3(texcoord*vec2(width/50.0,height/80.0)+vec2(0.0,timer*0.8),timer*0.2))*0.1;
-    noiz += pnoise3D(vec3(texcoord*vec2(width/90.0,height/200.0)+vec2(0.0,timer*0.6),1.0+timer*0.2))*0.25;
-    //noiz += pnoise3D(vec3(texcoord*vec2(width/200.0,height/400.0)+vec2(0.0,timer*0.4),2.0+timer*0.4))*0.25;
-    noiz += pnoise3D(vec3(texcoord*vec2(width/1200.0,height/1800.0)+vec2(0.0,timer*0.5),3.0+timer*0.3))*0.75;
+        noiz += pnoise3D(vec3(texcoord*vec2(width/90.0,height/200.0)+vec2(0.0,timer*0.6),1.0+timer*0.2))*0.25;
+        noiz += pnoise3D(vec3(texcoord*vec2(width/1200.0,height/1800.0)+vec2(0.0,timer*0.5),3.0+timer*0.3))*0.75;
     }
     
-    if (resettimer > 0.0 && resettimer < 100.0)
+    if (time > 0.0 && time < 100.0)
     {
-    drop += pnoise3D(vec3(texcoord*vec2(width/40.0,height/60.0),randomtime/8.0+timer*0.02))*0.2;
-    drop += pnoise3D(vec3(texcoord*vec2(width/80.0,height/200.0),randomtime*2.1+timer*0.03))*0.25;
-    //drop += pnoise3D(vec3(texcoord*vec2(width/200.0,height/400.0),randomtime*0.23+timer*0.04))*0.2;
-    //drop += pnoise3D(vec3(texcoord*vec2(width/800.0,height/1800.0),randomtime*1.64+timer*0.05))*0.1;
+        drop += pnoise3D(vec3(texcoord*vec2(width/40.0,height/60.0),randomtime/8.0+timer*0.02))*0.2;
+        drop += pnoise3D(vec3(texcoord*vec2(width/80.0,height/200.0),randomtime*2.1+timer*0.03))*0.25;
     }
         
-    float dropfade = clamp(resettimer*10.0,0.0,1.0);
+    float dropfade = clamp(time*10.0,0.0,1.0);
     
-    float drops = clamp(smoothstep(0.0+resettimerfaster,0.5+resettimerfaster,noiz*0.5+0.5),0.0,1.0);
-    float droplet = clamp(smoothstep(0.75+resettimerslow,1.0+resettimerslow,drop*0.5+0.5),0.0,1.0);
+    float drops = clamp(smoothstep(0.0+timefaster,0.5+timefaster,noiz*0.5+0.5),0.0,1.0);
+    float droplet = clamp(smoothstep(0.75+timeslow,1.0+timeslow,drop*0.5+0.5),0.0,1.0);
     
     droplet = pow(clamp(droplet+drops,0.0,1.0),0.1)*3.0;
-    float dropletmask = smoothstep(0.77+resettimerslow,0.79+resettimerslow,drop*0.5+0.5);
+    float dropletmask = smoothstep(0.77+timeslow,0.79+timeslow,drop*0.5+0.5);
 
-    //drops = pow(drops,0.1)*2.0;
-    float mask = smoothstep(0.02+resettimerfaster,0.03+resettimerfaster,noiz*0.5+0.5);	
-
-    vec2 wave;
+    float mask = smoothstep(0.02+timefaster,0.03+timefaster,noiz*0.5+0.5);
     
-    vec2 wavecoordR;
-    vec2 wavecoordG;
-    vec2 wavecoordB;
-    vec2 dropcoordR;
-    vec2 dropcoordG;	
-    vec2 dropcoordB;
 
-    if (resettimer < 1.0)
-    {
-    wave.x = sin((texcoord.x-texcoord.y*2.0)-timer*1.5)*0.25;
-    wave.x += cos((texcoord.y*4.0-texcoord.x*6.0)+timer*4.2)*0.5;
-    wave.x += sin((texcoord.x*9.0+texcoord.y*8.0)+timer*3.5)*0.25;
-    
-    wave.y = sin((texcoord.x*2.0+texcoord.x*2.5)+timer*2.5)*0.25;
-    wave.y += cos((texcoord.y*3.0+texcoord.x*6.0)-timer*2.5)*0.5;
-    wave.y += sin((texcoord.x*11.0-texcoord.y*12.0)+timer*4.5)*0.25;
-    }
-    
-    wave = wave*dfade;
+    vec2 droplets = vec2(dFdx(texcoord+droplet).r,dFdy(texcoord+droplet).g);		
 
-    wavecoordR = texcoord-wave*0.004;
-    wavecoordG = texcoord-wave*0.006;	
-    wavecoordB = texcoord-wave*0.008;
+    vec2 dropcoordR;
+    vec2 dropcoordG;
+    vec2 dropcoordB;
 
-    vec3 color = texture2D(bgl_RenderedTexture, texcoord).rgb;
+    droplets = droplets*dfade;
     
-    vec3 wavecolor = vec3(0.0);
-    wavecolor.r = texture2D(bgl_RenderedTexture, wavecoordR).r;
-    wavecolor.g = texture2D(bgl_RenderedTexture, wavecoordG).g;
-    wavecolor.b = texture2D(bgl_RenderedTexture, wavecoordB).b;
-    
-    vec3 final = mix(wavecolor,color,dropfade);
-//    final = wavecolor;
-
-
-    gl_FragColor = mix(original, vec4(final,1.0), power);
+    dropcoordR = (texcoord-droplets*1.1);
+    dropcoordG = (texcoord-droplets*1.2);	
+    dropcoordB = (texcoord-droplets*1.3);	
+
+    vec3 frag = texture(bgl_RenderedTexture, texcoord).rgb;
+
+    vec3 dropletcolor = vec3(0.0);
+    if (blur != 0.0){
+        dropletcolor.r = fblur(dropcoordR).r * color.x;
+        dropletcolor.g = fblur(dropcoordG).g * color.y;
+        dropletcolor.b = fblur(dropcoordB).b * color.z;
+    } else {
+        dropletcolor.r = texture(bgl_RenderedTexture, dropcoordR).r * color.x;
+        dropletcolor.g = texture(bgl_RenderedTexture, dropcoordG).g * color.y;
+        dropletcolor.b = texture(bgl_RenderedTexture, dropcoordB).b * color.z;
+    }
     
+    vec3 final = mix(frag, dropletcolor, clamp(dropletmask+mask,0.0,1.0)*dropfade);
+    fragColor = vec4(final,1.0);
 }"""
 
 
-class Distort(Filter2D):
+class Droplets(Filter2D):
 
-    def __init__(self, power=1.0, speed=1.0, idx: int = None) -> None:
+    def __init__(self, color=(1, 1, 1), speed=1.0, blur=0.0, idx: int = None) -> None:
         now = logic.getRealTime()
         self.speed = speed
-        self.settings = {'power': float(power), 'timer': now, 'resettimer': 0.0, 'randomtime': logic.getRandomFloat()}
+        self.settings = {
+            'blur': float(blur),
+            'color': Vector(color),
+            'timer': float(now),
+            'time': float(100.0),
+            'randomtime': float(logic.getRandomFloat())
+        }
         self._last_time = now
         self.randomize()
-        super().__init__(glsl, idx, {'power': self.settings, 'timer': self.settings, 'resettimer': self.settings, 'randomtime': self.settings})
+        super().__init__(glsl, idx, {
+            'blur': self.settings,
+            'color': self.settings,
+            'timer': self.settings,
+            'time': self.settings,
+            'randomtime': self.settings
+        })
 
     def update(self):
         now = logic.getRealTime()
-        self.timer += (now - self._last_time) * self.speed
+        diff = (now - self._last_time) * self.speed
+        self.timer += diff
         self._last_time = now
-        self.resettimer += (now - self._last_time) * self.speed
+        self.time += diff
         super().update()
 
     def randomize(self):
         self.randomtime = (logic.getRandomFloat()*5)*2.0-1.0
 
     def restart(self):
-        self.resettimer = 0.0
+        self.randomize()
+        self.time = 0.0
         self.timer = 0.0
 
     @property
+    def blur(self):
+        return self.settings['blur']
+
+    @blur.setter
+    def blur(self, val):
+        self.settings['blur'] = float(val)
+
+    @property
+    def color(self):
+        return self.settings['color']
+
+    @color.setter
+    def color(self, val):
+        self.settings['color'] = Vector(val).to_3d()
+
+    @property
     def timer(self):
         return self.settings['timer']
 
     @timer.setter
     def timer(self, val):
         self.settings['timer'] = float(val)
 
@@ -231,21 +267,13 @@
         return self.settings['randomtime']
 
     @randomtime.setter
     def randomtime(self, val):
         self.settings['randomtime'] = float(val)
 
     @property
-    def resettimer(self):
-        return self.settings['resettimer']
-
-    @resettimer.setter
-    def resettimer(self, val):
-        self.settings['resettimer'] = float(val)
-
-    @property
-    def power(self):
-        return self.settings['power']
+    def time(self):
+        return self.settings['time']
 
-    @power.setter
-    def power(self, val):
-        self.settings['power'] = float(val)
+    @time.setter
+    def time(self, val):
+        self.settings['time'] = float(val)
```

### Comparing `uplogic-2.1/uplogic/shaders/dof.py` & `uplogic-2.2/uplogic/shaders/dof.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 float width = bgl_RenderedTextureWidth; //texture width
 float height = bgl_RenderedTextureHeight; //texture height
 
 in vec4 bgl_TexCoord;
 vec2 texcoord = bgl_TexCoord.xy;
 
-out vec4 fragColor
+out vec4 fragColor;
 
 vec2 texel = vec2(1.0/width,1.0/height);
 
 uniform float distance;  //external focal point value, but you may use autofocus option below
 //float distance = 1;
 
 //------------------------------------------
@@ -192,29 +192,29 @@
 	kernel[0] = 1.0/16.0;   kernel[1] = 2.0/16.0;   kernel[2] = 1.0/16.0;
 	kernel[3] = 2.0/16.0;   kernel[4] = 4.0/16.0;   kernel[5] = 2.0/16.0;
 	kernel[6] = 1.0/16.0;   kernel[7] = 2.0/16.0;   kernel[8] = 1.0/16.0;
 
 
 	for( int i=0; i<9; i++ )
 	{
-		float tmp = texture2D(bgl_DepthTexture, coords + offset[i]).r;
+		float tmp = texture(bgl_DepthTexture, coords + offset[i]).r;
 		d += tmp * kernel[i];
 	}
 
 	return d;
 }
 
 
 vec3 color(vec2 coords,float blur) //processing the sample
 {
 	vec3 col = vec3(0.0);
 
-	col.r = texture2D(bgl_RenderedTexture,coords + vec2(0.0,1.0)*texel*fringe*blur).r;
-	col.g = texture2D(bgl_RenderedTexture,coords + vec2(-0.866,-0.5)*texel*fringe*blur).g;
-	col.b = texture2D(bgl_RenderedTexture,coords + vec2(0.866,-0.5)*texel*fringe*blur).b;
+	col.r = texture(bgl_RenderedTexture,coords + vec2(0.0,1.0)*texel*fringe*blur).r;
+	col.g = texture(bgl_RenderedTexture,coords + vec2(-0.866,-0.5)*texel*fringe*blur).g;
+	col.b = texture(bgl_RenderedTexture,coords + vec2(0.866,-0.5)*texel*fringe*blur).b;
 
 	vec3 lumcoeff = vec3(0.299,0.587,0.114);
 	float lum = dot(col.rgb, lumcoeff);
 	float thresh = max((lum-threshold)*gain, 0.0);
 	return col+mix(vec3(0.0),col,thresh*blur);
 }
 
@@ -230,36 +230,36 @@
 	}
 	return vec2(noiseX,noiseY);
 }
 
 void main() 
 {
 
-	float depth = texture2D(bgl_DepthTexture, texcoord).x;
+	float depth = texture(bgl_DepthTexture, texcoord).x;
 	float blur = 0.0;
 
 	if (depthblur)
 	{
 		depth = bdepth(texcoord);
 	}
 
 	blur = clamp((abs(depth - distance)/fstop)*100.0,-power,power);
 
 	if (autofocus)
 	{
-		float fDepth = texture2D(bgl_DepthTexture, focus).x;
+		float fDepth = texture(bgl_DepthTexture, focus).x;
 		blur = clamp((abs(depth - fDepth)/fstop)*100.0,-power,power);
 	}
 
 	vec2 noise = rand(texcoord)*namount*blur;
 
 	float w = (1.0/width)*blur+noise.x;
 	float h = (1.0/height)*blur+noise.y;
 
-	vec3 col = texture2D(bgl_RenderedTexture, texcoord).rgb;
+	vec3 col = texture(bgl_RenderedTexture, texcoord).rgb;
 	float s = 1.0;
 
 	int ringsamples;
 
 	for (int i = 1; i <= rings; i += 1)
 	{   
 		ringsamples = i * samples;
```

### Comparing `uplogic-2.1/uplogic/shaders/droplets.py` & `uplogic-2.2/uplogic/shaders/distort.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 from .shader import Filter2D
 from bge import logic
-from mathutils import Vector
 
 
 glsl = """
 /* Original Code by martins upitis @youtube: https://www.youtube.com/watch?v=UkskiSza4p0
 Modified by Iza Zed for uplogic
 */
 
 in vec4 bgl_TexCoord;
 #define gl_TexCoord glTexCoord
 vec4 glTexCoord[4] = vec4[](bgl_TexCoord,bgl_TexCoord,bgl_TexCoord,bgl_TexCoord);
 
 out vec4 fragColor;
-#define gl_FragColor fragColor
+
 
 uniform sampler2D bgl_RenderedTexture;
 uniform float bgl_RenderedTextureWidth;
 uniform float bgl_RenderedTextureHeight;
 
-uniform float timer, time, randomtime, blur;
-uniform vec3 color;
+uniform float timer, resettimer, randomtime, power;
 
 vec2 texcoord = vec2(gl_TexCoord[0]).st;
 
 const float permTexUnit = 1.0/256.0;		// Perm texture texel-size
 const float permTexUnitHalf = 0.5/256.0;	// Half perm texture texel-size
 
 float width = bgl_RenderedTextureWidth;
@@ -39,36 +37,14 @@
     float noiseG =  fract(noise*1.2154)*2.0-1.0; 
     float noiseB =  fract(noise*1.3453)*2.0-1.0;
     float noiseA =  fract(noise*1.3647)*2.0-1.0;
     
     return vec4(noiseR,noiseG,noiseB,noiseA);
 }
 
-vec3 fblur(vec2 uv){
-    float samples = 16;
-    vec2 resolution = vec2(bgl_RenderedTextureWidth, bgl_RenderedTextureHeight);
-    float Pi = 6.28318530718;
-
-    float quality = 3.0;
-   
-    vec2 radius = blur/resolution.xy;
-
-    vec3 frag = texture(bgl_RenderedTexture, uv).rgb;
-
-    for( float d=0.0; d<Pi; d+=Pi/samples)
-    {
-		for(float i = 1.0/quality; i<=1.0; i+=1.0/quality)
-        {
-			frag += texture(bgl_RenderedTexture, uv+vec2(cos(d),sin(d)) * radius * i).rgb;
-        }
-    }
-    frag /= quality * samples - 15.0;
-    return frag;
-}
-
 float fade(in float t) {
     return t*t*t*(t*(t*6.0-15.0)+10.0);
 }
 
 float pnoise3D(in vec3 p)
 {
     vec3 pi = permTexUnit*floor(p)+permTexUnitHalf; // Integer part, scaled so +1 moves permTexUnit texel
@@ -121,160 +97,110 @@
     float rotX = ((tc.x*2.0-1.0)*(width/height)*cos(angle)) - ((tc.y*2.0-1.0)*sin(angle));
     float rotY = ((tc.y*2.0-1.0)*cos(angle)) + ((tc.x*2.0-1.0)*(width/height)*sin(angle));
     rotX = ((rotX/(width/height))*0.5+0.5);
     rotY = rotY*0.5+0.5;
     return vec2(rotX,rotY);
 }
 
+
 void main(void)
 {
-    if (time > 10){
-        gl_FragColor = texture(bgl_RenderedTexture, texcoord);
-        return;
-    }
+    vec4 original = texture(bgl_RenderedTexture, texcoord);
     float grainsize = 100.0;
+    //texture edge bleed removal
     float fade = 12;
     vec2 distortFade = vec2(0.0);
     distortFade.s = clamp(texcoord.s*fade,0.0,1.0);
     distortFade.s -= clamp(1.0-(1.0-texcoord.s)*fade,0.0,1.0);
     distortFade.t = clamp(texcoord.t*fade,0.0,1.0);
     distortFade.t -= clamp(1.0-(1.0-texcoord.t)*fade,0.0,1.0); 
 
     vec2 rotCoordsR = texcoord;
-    
+
     float dfade = 1.0-pow((1.0-distortFade.s*distortFade.t),2.0);
     float noiz = 0.0;
-    float drop = 0.0;
 
-    float timeslow = time*0.02;
-    float timefaster = time*0.5;
+    float resettimerslow = resettimer*0.02;
+    float resettimerfaster = resettimer*0.5;
     
-    if (time > 0.0 && time < 4.0)
+    if (resettimer > 0.0 && resettimer < 4.0)
     {
         noiz += pnoise3D(vec3(texcoord*vec2(width/90.0,height/200.0)+vec2(0.0,timer*0.6),1.0+timer*0.2))*0.25;
         noiz += pnoise3D(vec3(texcoord*vec2(width/1200.0,height/1800.0)+vec2(0.0,timer*0.5),3.0+timer*0.3))*0.75;
     }
+
+    float mask = smoothstep(0.02+resettimerfaster,0.03+resettimerfaster,noiz*0.5+0.5);	
+
+    vec2 wave;
     
-    if (time > 0.0 && time < 100.0)
+    vec2 wavecoordR;
+    vec2 wavecoordG;
+    vec2 wavecoordB;
+
+    if (resettimer < 1.0)
     {
-        drop += pnoise3D(vec3(texcoord*vec2(width/40.0,height/60.0),randomtime/8.0+timer*0.02))*0.2;
-        drop += pnoise3D(vec3(texcoord*vec2(width/80.0,height/200.0),randomtime*2.1+timer*0.03))*0.25;
+        wave.x = sin((texcoord.x-texcoord.y*2.0)-timer*1.5)*0.25;
+        wave.x += cos((texcoord.y*4.0-texcoord.x*6.0)+timer*4.2)*0.5;
+        wave.x += sin((texcoord.x*9.0+texcoord.y*8.0)+timer*3.5)*0.25;
+
+        wave.y = sin((texcoord.x*2.0+texcoord.x*2.5)+timer*2.5)*0.25;
+        wave.y += cos((texcoord.y*3.0+texcoord.x*6.0)-timer*2.5)*0.5;
+        wave.y += sin((texcoord.x*11.0-texcoord.y*12.0)+timer*4.5)*0.25;
     }
-        
-    float dropfade = clamp(time*10.0,0.0,1.0);
     
-    float drops = clamp(smoothstep(0.0+timefaster,0.5+timefaster,noiz*0.5+0.5),0.0,1.0);
-    float droplet = clamp(smoothstep(0.75+timeslow,1.0+timeslow,drop*0.5+0.5),0.0,1.0);
-    
-    droplet = pow(clamp(droplet+drops,0.0,1.0),0.1)*3.0;
-    float dropletmask = smoothstep(0.77+timeslow,0.79+timeslow,drop*0.5+0.5);
-
-    float mask = smoothstep(0.02+timefaster,0.03+timefaster,noiz*0.5+0.5);
-    
-
-    vec2 droplets = vec2(dFdx(texcoord+droplet).r,dFdy(texcoord+droplet).g);		
+    wave = wave*dfade;
 
-    vec2 dropcoordR;
-    vec2 dropcoordG;
-    vec2 dropcoordB;
+    wavecoordR = texcoord-wave*0.004;
+    wavecoordG = texcoord-wave*0.006;	
+    wavecoordB = texcoord-wave*0.008;
 
-    droplets = droplets*dfade;
+    vec3 color = texture(bgl_RenderedTexture, texcoord).rgb;
     
-    dropcoordR = (texcoord-droplets*1.1);
-    dropcoordG = (texcoord-droplets*1.2);	
-    dropcoordB = (texcoord-droplets*1.3);	
-
-    vec3 frag = texture(bgl_RenderedTexture, texcoord).rgb;
-
-    vec3 dropletcolor = vec3(0.0);
-    if (blur != 0.0){
-        dropletcolor.r = fblur(dropcoordR).r * color.x;
-        dropletcolor.g = fblur(dropcoordG).g * color.y;
-        dropletcolor.b = fblur(dropcoordB).b * color.z;
-    } else {
-        dropletcolor.r = texture(bgl_RenderedTexture, dropcoordR).r * color.x;
-        dropletcolor.g = texture(bgl_RenderedTexture, dropcoordG).g * color.y;
-        dropletcolor.b = texture(bgl_RenderedTexture, dropcoordB).b * color.z;
-    }
+    vec3 wavecolor = vec3(0.0);
+    wavecolor.r = texture(bgl_RenderedTexture, wavecoordR).r;
+    wavecolor.g = texture(bgl_RenderedTexture, wavecoordG).g;
+    wavecolor.b = texture(bgl_RenderedTexture, wavecoordB).b;
+
+    fragColor = mix(original, vec4(wavecolor, 1.0), power);
     
-    vec3 final = mix(frag, dropletcolor, clamp(dropletmask+mask,0.0,1.0)*dropfade);
-    gl_FragColor = vec4(final,1.0);
 }"""
 
 
-class Droplets(Filter2D):
+class Distort(Filter2D):
 
-    def __init__(self, color=(1, 1, 1), speed=1.0, blur=0.0, idx: int = None) -> None:
+    def __init__(self, power=1.0, speed=1.0, idx: int = None) -> None:
         now = logic.getRealTime()
         self.speed = speed
-        self.settings = {
-            'blur': float(blur),
-            'color': Vector(color),
-            'timer': float(now),
-            'time': float(100.0),
-            'randomtime': float(logic.getRandomFloat())
-        }
+        self.settings = {'power': float(power), 'timer': now, 'resettimer': 0.0}
         self._last_time = now
-        self.randomize()
-        super().__init__(glsl, idx, {
-            'blur': self.settings,
-            'color': self.settings,
-            'timer': self.settings,
-            'time': self.settings,
-            'randomtime': self.settings
-        })
+        super().__init__(glsl, idx, {'power': self.settings, 'timer': self.settings, 'resettimer': self.settings})
 
     def update(self):
         now = logic.getRealTime()
-        diff = (now - self._last_time) * self.speed
-        self.timer += diff
+        self.timer += (now - self._last_time) * self.speed
         self._last_time = now
-        self.time += diff
+        self.resettimer += (now - self._last_time) * self.speed
         super().update()
 
-    def randomize(self):
-        self.randomtime = (logic.getRandomFloat()*5)*2.0-1.0
-
-    def restart(self):
-        self.randomize()
-        self.time = 0.0
-        self.timer = 0.0
-
-    @property
-    def blur(self):
-        return self.settings['blur']
-
-    @blur.setter
-    def blur(self, val):
-        self.settings['blur'] = float(val)
-
-    @property
-    def color(self):
-        return self.settings['color']
-
-    @color.setter
-    def color(self, val):
-        self.settings['color'] = Vector(val).to_3d()
-
     @property
     def timer(self):
         return self.settings['timer']
 
     @timer.setter
     def timer(self, val):
         self.settings['timer'] = float(val)
 
     @property
-    def randomtime(self):
-        return self.settings['randomtime']
+    def resettimer(self):
+        return self.settings['resettimer']
 
-    @randomtime.setter
-    def randomtime(self, val):
-        self.settings['randomtime'] = float(val)
+    @resettimer.setter
+    def resettimer(self, val):
+        self.settings['resettimer'] = float(val)
 
     @property
-    def time(self):
-        return self.settings['time']
+    def power(self):
+        return self.settings['power']
 
-    @time.setter
-    def time(self, val):
-        self.settings['time'] = float(val)
+    @power.setter
+    def power(self, val):
+        self.settings['power'] = float(val)
```

### Comparing `uplogic-2.1/uplogic/shaders/fxaa.py` & `uplogic-2.2/uplogic/shaders/fxaa.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,15 +322,15 @@
 #endif
 
 #else
 
 #define FxaaTexTop(t, p) vec4(texture(t, p, 0.0).rgb, 1.0)
 #define LumaTop(t, p) CalcLuma(texture(t, p, 0.0).rgb)
 #if (FXAA_FAST_PIXEL_OFFSET == 1)
-    #define LumaOff(t, p, o, r) CalcLuma(texture2DLodOffset(t, p, 0.0, o).rgb)
+    #define LumaOff(t, p, o, r) CalcLuma(textureLodOffset(t, p, 0.0, o).rgb)
 #else
     #define LumaOff(t, p, o, r) CalcLuma(texture(t, p + (o * r), 0.0).rgb)
 #endif
 
 #endif
 
 /*============================================================================
```

### Comparing `uplogic-2.1/uplogic/shaders/grayscale.py` & `uplogic-2.2/uplogic/shaders/grayscale.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/hbao.py` & `uplogic-2.2/uplogic/shaders/hbao.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/letterbox.py` & `uplogic-2.2/uplogic/shaders/vignette.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 from .shader import Filter2D
+from mathutils import Vector
 
 
 glsl = """
 uniform sampler2D bgl_RenderedTexture;
 
 in vec4 bgl_TexCoord;
 uniform float power;
-uniform float factor;
+uniform vec3 color;
 
 out vec4 fragColor;
 
-void main()
+void main( )
 {
-    float pow = clamp(1.0 - power, 0.0, 1.0);
-	vec4 px =  texture(bgl_RenderedTexture, bgl_TexCoord.xy);
-    if (bgl_TexCoord.y > 1.0-factor || bgl_TexCoord.y < factor){
-        fragColor = vec4(0.0, 0.0, 0.0, 1.0);
-        return;
-    }
-	fragColor = vec4(
-        px.r,
-        px.g,
-        px.b,
-        1.0
-    );
+	vec2 uv = bgl_TexCoord.xy;
+    uv *=  1.0 - uv.yx;
+    float vig = uv.x * uv.y * 15;
+    vig = pow(vig, power);
+    vec4 vcol = vec4(color.x, color.y, color.z, 1);
+    vec4 px = texture(bgl_RenderedTexture, bgl_TexCoord.xy);
+
+    fragColor = mix(vcol, px, vig);
 }
 """
 
 
-class Letterbox(Filter2D):
+class Vignette(Filter2D):
 
-    def __init__(self, power: float = 1.0, factor: float = 0.1, idx: int = None) -> None:
-        self.settings = {'power': float(power), 'factor': float(factor)}
-        super().__init__(glsl, idx, {'power': self.settings, 'factor': self.settings})
+    def __init__(self, power: float = 0.25, color=(0., 0., 0.), idx: int = None) -> None:
+        self.settings = {'power': float(power), 'color': Vector(color)}
+        super().__init__(glsl, idx, {'power': self.settings, 'color': self.settings})
 
     @property
     def power(self):
         return self.settings['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = float(val)
-    
+        self.settings['power'] = val
+
     @property
-    def factor(self):
-        return self.settings['factor']
+    def color(self):
+        return self.settings['color']
 
-    @factor.setter
-    def factor(self, val):
-        self.settings['factor'] = float(val)
+    @color.setter
+    def color(self, val):
+        if not isinstance(val, Vector):
+            val = Vector(val)
+        self.settings['color'] = val
```

### Comparing `uplogic-2.1/uplogic/shaders/levels.py` & `uplogic-2.2/uplogic/shaders/levels.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/mist.py` & `uplogic-2.2/uplogic/shaders/mist.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 
 glsl = """
 in vec4 bgl_TexCoord;
 #define gl_TexCoord glTexCoord
 vec4 glTexCoord[4] = vec4[](bgl_TexCoord,bgl_TexCoord,bgl_TexCoord,bgl_TexCoord);
 out vec4 fragColor;
-#define gl_FragColor fragColor
 
 uniform sampler2D bgl_RenderedTexture;
 uniform sampler2D bgl_DepthTexture;
 vec2 texcoord = vec2(gl_TexCoord[0]).st;
 vec2 cancoord = vec2(gl_TexCoord[3]).st;
 
 int model = 3; //mist model
@@ -30,15 +29,15 @@
 float linearize(float depth)
 {
     return -zfar * znear / (depth * (zfar - znear) - zfar);
 }
 
 void main(void)
 {    
-    float depth = linearize(texture2D(bgl_DepthTexture,texcoord.xy).x);
+    float depth = linearize(texture(bgl_DepthTexture,texcoord.xy).x);
 
     if (depth > zfar){
     //Clip the mist to allow for skyboxes
     depth = 0.0;
     }
 
     if (radial > 0){
@@ -68,15 +67,15 @@
         //Exponential Squared Mist
         factor = max(depth - start, 0.0);
         factor = 1.0 - exp(-(factor * factor)*density*density*0.0003);
     }
 
     vec4 dif = texture(bgl_RenderedTexture, texcoord);
 
-    gl_FragColor = mix(dif, mix(dif, mist, clamp(factor, 0.0, 1.0)), power);
+    fragColor = mix(dif, mix(dif, mist, clamp(factor, 0.0, 1.0)), power);
 
 }
 """
 
 
 class Mist(Filter2D):
```

### Comparing `uplogic-2.1/uplogic/shaders/rendertoscreen.py` & `uplogic-2.2/uplogic/shaders/rendertoscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/shader.py` & `uplogic-2.2/uplogic/shaders/shader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from bge import logic
 from mathutils import Vector, Matrix
 from uplogic.utils.errors import PassIndexOccupiedError
 from uplogic.utils import debug
 from pathlib import Path
+import bpy, bge
 
 
 def load_glsl(filepath: str):
     return Path(filepath).read_text()
 
 
 def remove_filter(pass_idx):
@@ -128,14 +129,16 @@
                     (
                         [value[0][0], value[0][1], value[0][2], value[0][3]],
                         [value[1][0], value[1][1], value[1][2], value[1][3]],
                         [value[2][0], value[2][1], value[2][2], value[2][3]],
                         [value[3][0], value[2][1], value[3][2], value[3][3]]
                     ),
                 )
+        elif cls is bpy.types.Image:
+            self._filter.setTexture(0, value.bindcode, name)
 
 
 class Filter2D(ULFilter):
     _deprecated = False
 
 
 class Attachment2D(ULFilter):
```

### Comparing `uplogic-2.1/uplogic/shaders/sharpen.py` & `uplogic-2.2/uplogic/shaders/sharpen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/splitscreen.py` & `uplogic-2.2/uplogic/shaders/splitscreen.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/shaders/ssao.py` & `uplogic-2.2/uplogic/shaders/ssao.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 bool mist = true; //use mist?
 float miststart = 0.0; //mist start
 float mistend = 100.0; //mist end
 
 bool onlyAO = false; //use only ambient occlusion pass?
 float lumInfluence = 0.7; //how much luminance affects occlusion
 
+out vec4 fragColor;
+
 //--------------------------------------------------------
 
 vec2 rand(vec2 coord) //generating noise/pattern texture for dithering
 {
 	float noiseX = ((fract(1.0-coord.s*(width/2.0))*0.25)+(fract(coord.t*(height/2.0))*0.75))*2.0-1.0;
 	float noiseY = ((fract(1.0-coord.s*(width/2.0))*0.75)+(fract(coord.t*(height/2.0))*0.25))*2.0-1.0;
 	
@@ -68,24 +70,24 @@
 		noiseY = clamp(fract(sin(dot(coord ,vec2(12.9898,78.233)*2.0)) * 43758.5453),0.0,1.0)*2.0-1.0;
 	}
 	return vec2(noiseX,noiseY)*noiseamount;
 }
 
 float doMist()
 {
-	float zdepth = texture2D(bgl_DepthTexture,texCoord.xy).x;
+	float zdepth = texture(bgl_DepthTexture,texCoord.xy).x;
 	float depth = -zfar * znear / (zdepth * (zfar - znear) - zfar);
 	return clamp((depth-miststart)/mistend,0.0,1.0);
 }
 
 float readDepth(in vec2 coord) 
 {
 	coord.x = clamp(coord.x,0.001,0.999);
     coord.y = clamp(coord.y,0.001,0.999);
-	return (2.0 * znear) / (zfar + znear - texture2D(bgl_DepthTexture, coord ).x * (zfar-znear));
+	return (2.0 * znear) / (zfar + znear - texture(bgl_DepthTexture, coord ).x * (zfar-znear));
 }
 
 float compareDepths(in float depth1, in float depth2,inout int far)
 {   
 	float garea = aowidth; //gauss bell width    
 	float diff = (depth1 - depth2)*100.0; //depth difference (0-100)
 	//reduce left bell width to avoid self-shadowing 
@@ -172,15 +174,15 @@
 	
 	if (onlyAO)
 	{
 	final = vec3(mix(vec3(ao),vec3(1.0),luminance*lumInfluence)); //ambient occlusion only
 	}
 	
 	
-	gl_FragColor = mix(vec4(color, 1.0), vec4(final, 1.0), power);
+	fragColor = mix(vec4(color, 1.0), vec4(final, 1.0), power);
 	
 }
 """
 
 
 class SSAO(Filter2D):
```

### Comparing `uplogic-2.1/uplogic/shaders/vignette.py` & `uplogic-2.2/uplogic/shaders/letterbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,48 @@
 from .shader import Filter2D
-from mathutils import Vector
 
 
 glsl = """
 uniform sampler2D bgl_RenderedTexture;
 
 in vec4 bgl_TexCoord;
 uniform float power;
-uniform vec3 color;
+uniform float factor;
 
 out vec4 fragColor;
 
-void main( )
+void main()
 {
-	vec2 uv = bgl_TexCoord.xy;
-    uv *=  1.0 - uv.yx;
-    float vig = uv.x * uv.y * 15;
-    vig = pow(vig, power);
-    vec4 vcol = vec4(color.x, color.y, color.z, 1);
-    vec4 px = texture(bgl_RenderedTexture, bgl_TexCoord.xy);
-
-    fragColor = mix(vcol, px, vig);
+    float pow = clamp(power, 0.0, 1.0);
+	vec4 px =  texture(bgl_RenderedTexture, bgl_TexCoord.xy);
+    bool cutoff = (bgl_TexCoord.y > 1.0-factor || bgl_TexCoord.y < factor);
+
+    fragColor = mix(
+        px,
+        vec4(0.0, 0.0, 0.0, 1.0),
+        (cutoff ? 1.0 : 0.0) * pow
+    );
 }
 """
 
 
-class Vignette(Filter2D):
+class Letterbox(Filter2D):
 
-    def __init__(self, power: float = 0.25, color=(0., 0., 0.), idx: int = None) -> None:
-        self.settings = {'power': float(power), 'color': Vector(color)}
-        super().__init__(glsl, idx, {'power': self.settings, 'color': self.settings})
+    def __init__(self, power: float = 1.0, factor: float = 0.1, idx: int = None) -> None:
+        self.settings = {'power': float(power), 'factor': float(factor)}
+        super().__init__(glsl, idx, {'power': self.settings, 'factor': self.settings})
 
     @property
     def power(self):
         return self.settings['power']
 
     @power.setter
     def power(self, val):
-        self.settings['power'] = val
-
+        self.settings['power'] = float(val)
+    
     @property
-    def color(self):
-        return self.settings['color']
+    def factor(self):
+        return self.settings['factor']
 
-    @color.setter
-    def color(self, val):
-        if not isinstance(val, Vector):
-            val = Vector(val)
-        self.settings['color'] = val
+    @factor.setter
+    def factor(self, val):
+        self.settings['factor'] = float(val)
```

### Comparing `uplogic-2.1/uplogic/ui/__init__.py` & `uplogic-2.2/uplogic/ui/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,8 +11,9 @@
 from .canvas import Canvas
 from .slider import Slider
 from .slider import FrameSlider
 from .slider import ProgressSlider
 from .path import Path
 from .path import WorldPath
 from .behaviors import MouseListener
+from .textinput import TextInput
 # from .render import RenderedTexture
```

### Comparing `uplogic-2.1/uplogic/ui/behaviors.py` & `uplogic-2.2/uplogic/ui/behaviors.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/button.py` & `uplogic-2.2/uplogic/ui/button.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/camera.py` & `uplogic-2.2/uplogic/ui/camera.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/canvas.py` & `uplogic-2.2/uplogic/ui/canvas.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/cursor.py` & `uplogic-2.2/uplogic/ui/cursor.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/image.py` & `uplogic-2.2/uplogic/ui/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,40 @@
 from uplogic.utils.math import rotate2d
 from gpu_extras.batch import batch_for_shader
 from mathutils import Vector
 
 
 class Image(Widget):
 
+    vertex_shader = """
+    in vec2 texCoord;
+    in vec2 pos;
+    out vec2 uv;
+
+    uniform mat4 ModelViewProjectionMatrix;
+
+    void main() {
+        uv = texCoord;
+        gl_Position = ModelViewProjectionMatrix * vec4(pos.xy, 0.0, 1.0);
+    }
+    """
+
+    fragment_shader = """
+    in vec2 uv;
+    out vec4 fragColor;
+
+    uniform sampler2D image;
+    uniform float alpha = 1.0;
+
+    void main() {
+        vec4 color = mix(vec4(0.0), texture(image, uv), alpha);
+        fragColor = pow(color, vec4(.5));
+    }
+    """
+
     def __init__(self, pos=[0, 0], size=(100, 100), relative={}, texture=None, halign='left', valign='bottom', use_aspect_ratio: bool = True, angle=0):
         self._texture = None
         self._image = None
         self.use_aspect_ratio = use_aspect_ratio
         self._opacity = 1
         super().__init__(pos, size, relative=relative, halign=halign, valign=valign, angle=angle)
         self.texture = texture
@@ -68,41 +94,15 @@
             x1 = rotate2d(x1, pivot, self._draw_angle)
             y0 = rotate2d(y0, pivot, self._draw_angle)
             y1 = rotate2d(y1, pivot, self._draw_angle)
         vertices = self._vertices = (
             x1, x0, y1, y0
         )
 
-        tex_vert_shader = """
-        in vec2 texCoord;
-        in vec2 pos;
-        out vec2 uv;
-
-        uniform mat4 ModelViewProjectionMatrix;
-
-        void main() {
-            uv = texCoord;
-            gl_Position = ModelViewProjectionMatrix * vec4(pos.xy, 0.0, 1.0);
-        }
-        """
-
-        tex_frag_shader = """
-        in vec2 uv;
-        out vec4 fragColor;
-
-        uniform sampler2D image;
-        uniform float alpha = 1.0;
-
-        void main() {
-            vec4 color = mix(vec4(0.0), texture(image, uv), alpha);
-            fragColor = pow(color, vec4(.5));
-        }
-        """
-        self._shader = gpu.types.GPUShader(tex_vert_shader, tex_frag_shader)
-        self._shader.uniform_float("alpha", self.opacity)
+        self._shader = gpu.types.GPUShader(self.vertex_shader, self.fragment_shader)
         self._batch = batch_for_shader(
             self._shader, 'TRI_STRIP',
             {
                 "pos": vertices,
                 "texCoord": (
                     (.9999, .0001),
                     (0.0001, 0.0001),
@@ -115,14 +115,15 @@
     def draw(self):
         gpu.state.blend_set("ALPHA")
         super()._setup_draw()
         if self.texture is None:
             super().draw()
             return
         self._shader.bind()
+        self._shader.uniform_float("alpha", self.opacity)
         self._shader.uniform_sampler("image", self.texture)
         self._batch.draw(self._shader)
         super().draw()
 
 
 class Sprite(Image):
```

### Comparing `uplogic-2.1/uplogic/ui/label.py` & `uplogic-2.2/uplogic/ui/label.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,34 +4,42 @@
 from uplogic.utils.math import rotate2d
 import math
 
 
 class Label(Widget):
     '''Widget for displaying text
 
-    :param `orientation`: Whether to arrange widgets horizontally or vertically; Can be (`'horizontal'`, `'vertical'`).
     :param `pos`: Initial position of this widget in either pixels or factor.
     :param `relative`: Whether to use pixels or factor for size or pos; example: `{'pos': True, 'size': True}`.
+    :param `text`: Initial text for this label.
+    :param `font`: Font name.
+    :param `font_color`: Color in RGBA.
+    :param `font_size`: Font size in pt or factor.
+    :param `line_height`: Total line height relative to character size (1 is same as character height).
+    :param `shadow`: Draw a shadow behind the text.
+    :param `shadow_offset`: Relative position of the shadow in px.
+    :param `shadow_color`: Shadow color in RGBA.
     :param `halign`: Horizontal alignment of the widget, can be (`left`, `center`, `right`).
     :param `valign`: Vertical alignment of the widget, can be (`bottom`, `center`, `top`).
+    :param `wrap`: Split lines that are too long for the containing widget.
     :param `angle`: Rotation in degrees of this widget around the pivot defined by the alignment.
     '''
 
     def __init__(
         self,
         pos=[0, 0],
         relative={},
         text='',
         font='',
-        font_color=[1, 1, 1, 1],
+        font_color=[1., 1., 1., 1.],
         font_size=12,
         line_height=1.5,
         shadow=False,
-        shadow_offset=[2, -2],
-        shadow_color=[0, 0, 0, .6],
+        shadow_offset=[1, -1],
+        shadow_color=[.0, .0, .0, 1.],
         halign='left',
         valign='bottom',
         wrap=False,
         angle=0
     ):
         self._parent = None
         self._children = None
@@ -41,14 +49,15 @@
         self.shadow = shadow
         self.shadow_offset = shadow_offset
         self.shadow_color = shadow_color
         self.font_size = font_size
         self.font_color = font_color
         self.font = font
         self.wrap = wrap
+        self.lines = []
         Widget.__init__(self, pos, (0, 0), (0, 0, 0, 0), relative, angle=angle)
         self.text_halign = halign
         self.text_valign = valign
 
     @property
     def text(self):
         return self._text
@@ -112,41 +121,44 @@
     # @font_opacity.setter
     # def font_opacity(self, val):
     #     self._font_color[3] = val * self.opacity
 
     @property
     def dimensions(self):
         dim = blf.dimensions(self.font, self.text)
-        return (dim[0], blf.dimensions(self.font, 'Aj')[1])
+        lines = len(self.lines) or 1
+        return (dim[0], blf.dimensions(self.font, 'Aj')[1] * lines)
 
     @property
     def _draw_size(self):
-        parsize = self.parent._draw_size
         relative = self.relative.get('font_size', False)
-        blf.size(self.font, parsize[1] * self.font_size if relative else self.font_size)
+        fontsize = self.parent._draw_size[1] * self.font_size if relative else self.font_size
+        blf.size(self.font, fontsize)
         return self.dimensions
 
     def make_floating(self, pos=True, size=True, halign='center', valign='center'):
         self.relative['pos'] = pos
         self.relative['size'] = size
         self.text_halign = halign
         self.text_valign = valign
+        return self
 
     def draw(self):
         super()._setup_draw()
         parsize = self.parent._draw_size
         relative = self.relative.get('font_size', False)
         font = self.font
         blf.size(font, parsize[1] * self.font_size if relative else self.font_size)
         col = self.font_color
         blf.color(font, col[0], col[1], col[2], col[3] * self.opacity)
         charsize = blf.dimensions(font, 'A')
         smallsize = blf.dimensions(font, 'a')[1]
         lowsize = blf.dimensions(font, 'g')[1]
         diff = lowsize - smallsize
+
         if self.angle or self.parent._draw_angle:
             blf.enable(font, blf.ROTATION)
             blf.rotation(font, math.radians(self._draw_angle))
         if self.parent.use_clipping:
             verts = self.parent._vertices
             blf.enable(font, blf.CLIPPING)
             blf.clipping(font, verts[0][0], verts[0][1] + charsize[1], verts[2][0], verts[2][1])
@@ -168,46 +180,47 @@
                 underground = dimensions[1] > charsize[1]
                 lheight = (charsize[1] * self.line_height)
                 if self.text_halign == 'center':
                     pos[0] -= (dimensions[0] * .5)
                 elif self.text_halign == 'right':
                     pos[0] -= dimensions[0]
                 if self.text_valign == 'top':
-                    if underground:
-                        pos[1] += (diff)
+                    # if underground:
+                    # pos[1] += (diff)
                     pos[1] -= lheight
                 elif self.text_valign == 'center':
-                    if underground:
-                        pos[1] += (diff * .5)
+                    # if underground:
+                        # pos[1] += (diff * .5)
                     pos[1] += (.5 * lheight * (len(lines) - 1)) - (.5 * lheight)
                 elif self.text_valign == 'bottom':
                     pos[1] += (lheight * (len(lines) -2))
                 if self.parent and self.parent._draw_angle:
                     pos = rotate2d(pos, self.pivot, self.parent.angle)
                 blf.position(font, pos[0], pos[1] - (charsize[1] * i * self.line_height), 0)
                 blf.draw(font, txt)
         else:
             dimensions = blf.dimensions(font, self.text)
             pos = self._draw_pos.copy()
-            underground = dimensions[1] > charsize[1]
+            # underground = dimensions[1] > charsize[1]
 
             if self.text_halign == 'center':
                 pos[0] -= (dimensions[0] * .5)
             elif self.text_halign == 'right':
                 pos[0] -= dimensions[0]
             if self.text_valign == 'top':
-                if underground:
-                    pos[1] += (diff)
-                pos[1] -= dimensions[1]
+                # if underground:
+                    # pos[1] += diff
+                pos[1] -= charsize[1] * self.line_height
             elif self.text_valign == 'center':
-                if underground:
-                    pos[1] += (diff * .5)
-                pos[1] -= (.5 * dimensions[1])
+                # if underground:
+                    # pos[1] += (diff * .5)
+                pos[1] -= (.5 * charsize[1])
             if self.parent and self.parent._draw_angle:
                 pos = rotate2d(pos, self.pivot, self.parent.angle)
             blf.position(font, pos[0], pos[1], 0)
             blf.draw(font, self.text)
 
         super().draw()
+        self.lines = lines
         blf.disable(font, blf.WORD_WRAP)
         blf.disable(font, blf.SHADOW)
         blf.disable(font, blf.ROTATION)
```

### Comparing `uplogic-2.1/uplogic/ui/layout.py` & `uplogic-2.2/uplogic/ui/layout.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/path.py` & `uplogic-2.2/uplogic/ui/path.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/render.py` & `uplogic-2.2/uplogic/ui/render.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/slider.py` & `uplogic-2.2/uplogic/ui/slider.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/ui/widget.py` & `uplogic-2.2/uplogic/ui/widget.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,27 +15,48 @@
     :param `size`: Initial size of this widget in either pixels or factor.
     :param `bg_color`: Color to draw in the area of the widget.
     :param `relative`: Whether to use pixels or factor for size or pos; example: `{'pos': True, 'size': True}`.
     :param `halign`: Horizontal alignment of the widget, can be (`left`, `center`, `right`).
     :param `valign`: Vertical alignment of the widget, can be (`bottom`, `center`, `top`).
     :param `angle`: Rotation in degrees of this widget around the pivot defined by the alignment.
     '''
+
+    vertex_shader = '''
+    uniform mat4 ModelViewProjectionMatrix;
+    in vec3 pos;
+
+    void main()
+    {
+        gl_Position = ModelViewProjectionMatrix * vec4(pos.xy, 0.0, 1.0f);
+    }
+    '''
+
+    fragment_shader = '''
+    uniform vec4 color;
+    out vec4 fragColor;
+
+    void main()
+    {
+        fragColor = color;
+    }
+    '''
+
     def __init__(self, pos=(0, 0), size=(0, 0), bg_color=(0, 0, 0, 0), relative={}, halign='left', valign='bottom', angle=0):
         self.halign = halign
         self.valign = valign
         self._parent = None
         self._show = True
         self._pos = [0, 0]
         self._children: list[Widget] = []
         self.relative = relative
         self._rebuild = True
         self.size = size
         self.pos = pos
         self.bg_color = bg_color
-        self._vertices = None # (Vector((0, 0)), Vector((0, 0)), Vector((0, 0)), Vector((0, 0)))
+        self._vertices = None  # (Vector((0, 0)), Vector((0, 0)), Vector((0, 0)), Vector((0, 0)))
         self.angle = angle
         self._build_shader()
         self._clipped = [0, 0]
         self.use_clipping = False
         self.copy_height = False
         self.copy_width = False
         self.opacity = 1
@@ -50,18 +71,26 @@
     def set_visible(self, flag=True):
         self.show = flag
 
     def set_invisible(self):
         self.show = False
 
     def make_floating(self, pos=True, size=True, halign='center', valign='center'):
+        """Quickly set the attributes of this widget to use relative data.
+
+        :param `pos`: Use relative position.
+        :param `size`: Use relative size.
+        :param `halign`: The horizontal alignment.
+        :param `valign`: The vertical alignment.
+        """
         self.relative['pos'] = pos
         self.relative['size'] = size
         self.halign = halign
         self.valign = valign
+        return self
 
     @property
     def active(self):
         parent = self
         while parent is not None:
             if not parent._active:
                 return False
@@ -424,15 +453,16 @@
             Vector(y1),
             Vector(y0),
             Vector(x0)
         )
         indices = (
             (0, 1, 2), (2, 3, 0)
         )
-        self._shader = gpu.shader.from_builtin('UNIFORM_COLOR')
+        # self._shader = gpu.shader.from_builtin('UNIFORM_COLOR')
+        self._shader = gpu.types.GPUShader(self.vertex_shader, self.fragment_shader)
         self._batch = batch_for_shader(self._shader, 'TRIS', {"pos": vertices}, indices=indices)
         self._batch_line = batch_for_shader(self._shader, 'LINE_STRIP', {"pos": vertices})
         self._batch_points = batch_for_shader(self._shader, 'POINTS', {"pos": vertices})
 
     def _setup_draw(self):
         if self._rebuild is True:
             self._build_shader()
@@ -467,14 +497,15 @@
         :param `widget`: `Widget` to add.
         '''
         if widget not in self.children:
             widget.parent = self
             self.children.append(widget)
             self.canvas._set_z(-1)
         self.children = sorted(self.children, key=lambda widget: widget.z, reverse=False)
+        return widget
 
     def _set_z(self, z):
         z += 1
         self.z = z
         for c in self.children:
             z = c._set_z(z)
         return z
```

### Comparing `uplogic-2.1/uplogic/utils/__init__.py` & `uplogic-2.2/uplogic/utils/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from .visualize import draw_box  # noqa
 from .visualize import draw_cube  # noqa
 from .visualize import draw_line  # noqa
 from .visualize import draw_path  # noqa
 from .visualize import draw_mesh  # noqa
 from .visualize import draw_arrow  # noqa
 from .visualize import draw_arrow_path  # noqa
+from .visualize import draw_axis  # noqa
 from .scene import FileLoader  # noqa
 from .scene import SceneLoader  # noqa
 from .math import clamp
 from .math import cycle
 from .math import vec_abs
 from .math import vec_clamp
 from .math import interpolate
@@ -55,14 +56,15 @@
 from .math import map_range
 from .math import mouse_over
 from .math import screen_to_world
 from .math import world_to_screen
 from .math import rotate2d
 from .math import rotate3d
 from .math import rotate_by_axis
+from .math import rotate_by_euler
 from .objects import xrot_to
 from .objects import yrot_to
 from .objects import zrot_to
 from .objects import rotate_to
 from .constants import WATER
 from .constants import OPERATORS
 from .constants import LOGIC_OPERATORS
```

### Comparing `uplogic-2.1/uplogic/utils/constants.py` & `uplogic-2.2/uplogic/utils/constants.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/engine.py` & `uplogic-2.2/uplogic/utils/engine.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/errors.py` & `uplogic-2.2/uplogic/utils/errors.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/lights.py` & `uplogic-2.2/uplogic/utils/lights.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/math.py` & `uplogic-2.2/uplogic/utils/math.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 from mathutils import Vector
+from mathutils import Euler
+from mathutils import Matrix
 from bge import logic
 from bge.types import KX_GameObject as GameObject
 import math
 
 
-def clamp(value: float or Vector, min: float = 0, max: float = 1) -> float:
+def clamp(value: float or Vector, lower: float = 0, upper: float = 1) -> float:
     """Clamp a value in between two other values.
 
-    :param value: input value
-    :param min: minimum value
-    :param max: maximum value
+    :param `value`: input value
+    :param `min`: minimum value
+    :param `max`: maximum value
 
     :returns: clamped value as float
     """
     if isinstance(value, Vector):
         return vec_clamp(value, min, max)
-    if value < min:
-        return min
-    if value > max:
-        return max
-    return value
+    # if value < min:
+    #     return min
+    # if value > max:
+    #     return max
+    return max(lower, min(value, upper))
 
 
-def cycle(value: float or Vector, min: float = 0, max: float = 1) -> float:
+def cycle(value: float, min: float = 0, max: float = 1) -> float:
     """Clamp a value in between two other values.
 
-    :param value: input value
-    :param min: minimum value
-    :param max: maximum value
+    :param `value`: input value
+    :param `min`: minimum value
+    :param `max`: maximum value
 
     :returns: clamped value as float
     """
     if isinstance(value, Vector):
         return vec_clamp(value, min, max)
     if value < min:
         return max
@@ -39,17 +41,17 @@
         return min
     return value
 
 
 def vec_clamp(vec: Vector, min: float = 0, max: float = 1) -> Vector:
     """Clamp length of a vector.
 
-    :param value: `Vector`
-    :param min: minimum length
-    :param max: maximum length
+    :param `value`: `Vector`
+    :param `min`: minimum length
+    :param `max`: maximum length
 
     :returns: clamped vector as float
     """
     vec = vec.copy()
     if vec.length < min:
         vec.normalize()
         return vec * min
@@ -58,31 +60,31 @@
         return vec * max
     return vec
 
 
 def interpolate(a: float, b: float, fac: float, threshold: float = 0.001) -> float:
     """Interpolate between 2 values using a factor.
 
-    :param a: starting value
-    :param b: target value
-    :param fac: interpolation factor
+    :param `a`: starting value
+    :param `b`: target value
+    :param `fac`: interpolation factor
 
     :returns: calculated value as float
     """
     if -threshold < a-b < threshold:
         return b
     return (fac * b) + ((1-fac) * a)
 
 
 def lerp(a: float, b: float, fac: float, threshold: float = 0.001) -> float:
     """Interpolate between 2 values using a factor.
 
-    :param a: starting value
-    :param b: target value
-    :param fac: interpolation factor
+    :param `a`: starting value
+    :param `b`: target value
+    :param `fac`: interpolation factor
 
     :returns: calculated value as float
     """
     if -threshold < a-b < threshold:
         return b
     return (fac * b) + ((1-fac) * a)
 
@@ -337,7 +339,17 @@
     target_point = Vector((
             (target_point[0] * math.cos(thz)) - (target_point[1] * math.sin(thz)),
             (target_point[0] * math.sin(thz)) + (target_point[1] * math.cos(thz)),
             target_point[2]
     ))
 
     return pivot + target_point
+
+
+def rotate_by_euler(origin: Vector, pivot: Vector, angles: Euler):
+
+    origin = origin.copy() - pivot
+    angles = Euler(angles)
+
+    transmat = angles.to_matrix()
+
+    return pivot + origin @ transmat
```

### Comparing `uplogic-2.1/uplogic/utils/nodetrees.py` & `uplogic-2.2/uplogic/utils/nodetrees.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/objects.py` & `uplogic-2.2/uplogic/utils/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def xrot_to(
     rotating_object,
     target_pos,
     front_axis_code=1,
     factor=1
 ):
     local = get_local(rotating_object, target_pos)
-    front = Vector((1, 0)) if front_axis_code == 1 else Vector((0, 1))
+    front = Vector((1, 0)) if front_axis_code in [1, 4] else Vector((0, 1))
     if front_axis_code > 2:
         front.negate()
     angle = Vector((local.y, local.z))
     if angle.length < .001:
         return
     angle = angle.angle_signed(front)
     rotating_object.applyRotation((angle*factor, 0, 0), True)
@@ -35,15 +35,15 @@
 def yrot_to(
     rotating_object,
     target_pos,
     front_axis_code=1,
     factor=1
 ):
     local = get_local(rotating_object, target_pos)
-    front = Vector((1, 0)) if front_axis_code == 0 else Vector((0, 1))
+    front = Vector((1, 0)) if front_axis_code in [0, 3] else Vector((0, 1))
     if front_axis_code > 2:
         front.negate()
     angle = Vector((local.x, local.z))
     if angle.length < .001:
         return
     angle = angle.angle_signed(front)
     rotating_object.applyRotation((0, angle*factor, 0), True)
@@ -52,16 +52,17 @@
 def zrot_to(
     rotating_object,
     target_pos,
     front_axis_code=1,
     factor=1
 ):
     local = get_local(rotating_object, target_pos)
-    front = Vector((1, 0)) if front_axis_code == 0 else Vector((0, 1))
+    front = Vector((1, 0)) if front_axis_code in [0, 3] else Vector((0, 1))
     if front_axis_code > 2:
+        print(front)
         front.negate()
     angle = Vector((local.x, local.y))
     if angle.length < .001:
         return
     angle = angle.angle_signed(front)
     rotating_object.applyRotation((0, 0, angle*factor), True)
 
@@ -75,14 +76,15 @@
 ):
     """Rotate an object around a local axis towards a point"""
     front = front_axis
     if front > 2:
         front -= 3
     if rotation_axis == front:
         return
+    print(front_axis)
     if rotation_axis == 0:
         xrot_to(
             object,
             target,
             front_axis,
             factor
         )
```

### Comparing `uplogic-2.1/uplogic/utils/pooling.py` & `uplogic-2.2/uplogic/utils/pooling.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/raycasting.py` & `uplogic-2.2/uplogic/utils/raycasting.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic/utils/scene.py` & `uplogic-2.2/uplogic/utils/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def set_scene(scene: str or bpy.types.Scene) -> None:
     logic.getCurrentScene().replace(scene)
 
 
 def get_custom_loop():
-    return logic.getCurrentScene()['uplogic.mainloop']
+    return logic.globalDict.get('loop', None)
 
 
 class FileLoader():
     '''Load the content of the currently'''
 
     def __init__(self, start=False):
         self.status = 0.0
@@ -140,31 +140,37 @@
     def load_next(self):
         cam = logic.getCurrentScene().active_camera
         self.object.worldPosition = cam.worldPosition - cam.getAxisVect((0, 0, 1)) * 100
         if self.images:
             self.tex_image.image = self.images.pop()
             self.status += 1 / self.datasize
             self.item = self.tex_image.image.name
+            self.on_progress(self.status)
             return
         if self.materials:
             mat = self.materials.pop()
             self.object.blenderObject.material_slots[0].material = mat
             self.status += 1 / self.datasize
             self.data = 'shaders'
             self.item = mat.name
+            self.on_progress(self.status)
             return
         if self.meshes:
             self.bobj.data = self.meshes.pop()
             self.status += 1 / self.datasize
             self.data = 'objects'
             self.item = self.bobj.data.name
+            self.on_progress(self.status)
             return
         logic.getCurrentScene().pre_draw.remove(self.load_next)
         self.object.endObject()
         bpy.data.materials.remove(self.temp_map)
         bpy.data.objects.remove(self.bobj)
         bpy.data.meshes.remove(self.bmesh)
         self.finished = True
         self.on_finish()
 
+    def on_progress(self, progress):
+        pass
+
     def on_finish(self):
         pass
```

### Comparing `uplogic-2.1/uplogic/utils/visuals.py` & `uplogic-2.2/uplogic/utils/visuals.py`

 * *Files identical despite different names*

### Comparing `uplogic-2.1/uplogic.egg-info/PKG-INFO` & `uplogic-2.2/uplogic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: uplogic
-Version: 2.1
+Version: 2.2
 Summary: Uplogic utility for UPBGE.
 Home-page: https://github.com/UPBGE/uplogic
 Author: Leopold Auersperg-Castell
 Author-email: lauersperg@gmx.at
 License: GPLv2
-Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.1.tar.gz
+Download-URL: https://github.com/UPBGE/uplogic/archive/refs/tags/v2.2.tar.gz
 Keywords: Blender UPBGE logic
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Graphics
 Classifier: Programming Language :: Python
 License-File: LICENSE.md
```

### Comparing `uplogic-2.1/uplogic.egg-info/SOURCES.txt` & `uplogic-2.2/uplogic.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 uplogic/animation/actionsystem.py
 uplogic/animation/rig.py
 uplogic/animation/sequence.py
 uplogic/audio/__init__.py
 uplogic/audio/audiosystem.py
 uplogic/audio/music.py
 uplogic/audio/sound.py
+uplogic/console/__init__.py
 uplogic/data/__init__.py
 uplogic/data/file.py
 uplogic/data/globaldb.py
 uplogic/data/serializers.py
 uplogic/decorators/__init__.py
 uplogic/events/__init__.py
 uplogic/input/__init__.py
 uplogic/input/gamepad.py
 uplogic/input/keyboard.py
 uplogic/input/mouse.py
 uplogic/input/vr.py
-uplogic/logging/__init__.py
 uplogic/network/__init__.py
 uplogic/network/client.py
 uplogic/network/server.py
 uplogic/nodes/__init__.py
 uplogic/nodes/logictree.py
 uplogic/nodes/actions/__init__.py
 uplogic/nodes/actions/addfilter.py
@@ -246,27 +246,29 @@
 uplogic/nodes/parameters/bonestatus.py
 uplogic/nodes/parameters/characterinfo.py
 uplogic/nodes/parameters/childbyindex.py
 uplogic/nodes/parameters/childbyname.py
 uplogic/nodes/parameters/clamp.py
 uplogic/nodes/parameters/colorrgb.py
 uplogic/nodes/parameters/colorrgba.py
+uplogic/nodes/parameters/curveinterpolation.py
 uplogic/nodes/parameters/dictvalue.py
 uplogic/nodes/parameters/distance.py
 uplogic/nodes/parameters/euler.py
 uplogic/nodes/parameters/eulertomatrix.py
 uplogic/nodes/parameters/formattedstring.py
 uplogic/nodes/parameters/formula.py
 uplogic/nodes/parameters/fpsfactor.py
 uplogic/nodes/parameters/gamepadsticks.py
 uplogic/nodes/parameters/gamepadtrigger.py
 uplogic/nodes/parameters/getactuatorvalue.py
 uplogic/nodes/parameters/getcollection.py
 uplogic/nodes/parameters/getcollectionobjectnames.py
 uplogic/nodes/parameters/getcollectionobjects.py
+uplogic/nodes/parameters/getcollisiongroup.py
 uplogic/nodes/parameters/getcurvepoints.py
 uplogic/nodes/parameters/getfont.py
 uplogic/nodes/parameters/getfullscreen.py
 uplogic/nodes/parameters/getglobalvalue.py
 uplogic/nodes/parameters/getgravity.py
 uplogic/nodes/parameters/getimage.py
 uplogic/nodes/parameters/getlightcolor.py
@@ -321,14 +323,15 @@
 uplogic/nodes/parameters/rotatebypoint.py
 uplogic/nodes/parameters/screenposition.py
 uplogic/nodes/parameters/serializedata.py
 uplogic/nodes/parameters/simplevalue.py
 uplogic/nodes/parameters/storevalue.py
 uplogic/nodes/parameters/threshold.py
 uplogic/nodes/parameters/timedata.py
+uplogic/nodes/parameters/tweenvalue.py
 uplogic/nodes/parameters/typecastvalue.py
 uplogic/nodes/parameters/valueswitch.py
 uplogic/nodes/parameters/vectorabsolute.py
 uplogic/nodes/parameters/vectorangle.py
 uplogic/nodes/parameters/vectoranglecheck.py
 uplogic/nodes/parameters/vectorlength.py
 uplogic/nodes/parameters/vectormath.py
@@ -353,38 +356,42 @@
 uplogic/shaders/blur.py
 uplogic/shaders/brightness.py
 uplogic/shaders/buffer.py
 uplogic/shaders/chromaticaberration.py
 uplogic/shaders/distort.py
 uplogic/shaders/dof.py
 uplogic/shaders/droplets.py
+uplogic/shaders/filtersystem.py
 uplogic/shaders/fxaa.py
 uplogic/shaders/grayscale.py
 uplogic/shaders/hbao.py
+uplogic/shaders/lens.py
 uplogic/shaders/letterbox.py
 uplogic/shaders/levels.py
 uplogic/shaders/mist.py
 uplogic/shaders/rendertoscreen.py
 uplogic/shaders/shader.py
 uplogic/shaders/sharpen.py
 uplogic/shaders/splitscreen.py
 uplogic/shaders/ssao.py
+uplogic/shaders/texture.py
 uplogic/shaders/vignette.py
 uplogic/ui/__init__.py
 uplogic/ui/behaviors.py
 uplogic/ui/button.py
 uplogic/ui/camera.py
 uplogic/ui/canvas.py
 uplogic/ui/cursor.py
 uplogic/ui/image.py
 uplogic/ui/label.py
 uplogic/ui/layout.py
 uplogic/ui/path.py
 uplogic/ui/render.py
 uplogic/ui/slider.py
+uplogic/ui/textinput.py
 uplogic/ui/widget.py
 uplogic/utils/__init__.py
 uplogic/utils/constants.py
 uplogic/utils/engine.py
 uplogic/utils/errors.py
 uplogic/utils/lights.py
 uplogic/utils/math.py
```

