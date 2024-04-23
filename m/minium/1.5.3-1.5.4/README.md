# Comparing `tmp/minium-1.5.3.tar.gz` & `tmp/minium-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/minium-1.5.3.tar", last modified: Mon Jan 15 11:47:51 2024, max compression
+gzip compressed data, was "dist/minium-1.5.4.tar", last modified: Mon Apr 22 13:01:37 2024, max compression
```

## Comparing `minium-1.5.3.tar` & `minium-1.5.4.tar`

### file list

```diff
@@ -1,365 +1,372 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.651251 minium-1.5.3/
--rw-r--r--   0 root         (0) root         (0)      699 2024-01-15 11:47:51.651251 minium-1.5.3/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium/
--rw-r--r--   0 root         (0) root         (0)     1213 2024-01-08 08:32:33.000000 minium-1.5.3/minium/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium/externlib/
--rw-r--r--   0 root         (0) root         (0)       58 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium/externlib/android_base/
--rw-r--r--   0 root         (0) root         (0)     1012 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/android_base/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium/externlib/at/
--rw-r--r--   0 root         (0) root         (0)     4087 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1755 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/apkapi.py
--rw-r--r--   0 root         (0) root         (0)     5609 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/atproxy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.619251 minium-1.5.3/minium/externlib/at/bin/
--rw-r--r--   0 root         (0) root         (0)  3566862 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/bin/AtServer.apk
--rw-r--r--   0 root         (0) root         (0)    95449 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/bin/AtStub.jar
--rw-r--r--   0 root         (0) root         (0)     3222 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/command_line.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/core/
--rw-r--r--   0 root         (0) root         (0)       37 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      951 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/accesshelper.py
--rw-r--r--   0 root         (0) root         (0)    47044 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/adbwrap.py
--rw-r--r--   0 root         (0) root         (0)    10763 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/basedriver.py
--rw-r--r--   0 root         (0) root         (0)    15919 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/case_repair_adapter.py
--rw-r--r--   0 root         (0) root         (0)      624 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/config.py
--rw-r--r--   0 root         (0) root         (0)    31731 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/element.py
--rw-r--r--   0 root         (0) root         (0)      669 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    18740 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/javadriver.py
--rw-r--r--   0 root         (0) root         (0)     3620 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/resguard.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/core/stf/
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/stf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1662 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/stf/mincap.py
--rw-r--r--   0 root         (0) root         (0)     5507 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/stf/minitouch.py
--rw-r--r--   0 root         (0) root         (0)    11596 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/uidevice.py
--rw-r--r--   0 root         (0) root         (0)    17965 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/uixml.py
--rw-r--r--   0 root         (0) root         (0)     2711 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/core/websocketcli.py
--rw-r--r--   0 root         (0) root         (0)     2186 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/eventmonitor.py
--rw-r--r--   0 root         (0) root         (0)     1087 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/hook.py
--rw-r--r--   0 root         (0) root         (0)     8495 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/jlogcat.py
--rw-r--r--   0 root         (0) root         (0)    36015 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/keycode.py
--rw-r--r--   0 root         (0) root         (0)     9492 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/perfcollector.py
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/tests/
--rw-r--r--   0 root         (0) root         (0)      690 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/AtEvent.py
--rw-r--r--   0 root         (0) root         (0)      326 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/AtSocket.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/adbtest.py
--rw-r--r--   0 root         (0) root         (0)      490 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/airtesttest.py
--rw-r--r--   0 root         (0) root         (0)    10434 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/atdevicetest.py
--rw-r--r--   0 root         (0) root         (0)      474 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/attestbase.py
--rw-r--r--   0 root         (0) root         (0)     1022 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/drivertest.py
--rw-r--r--   0 root         (0) root         (0)     1768 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/elementtest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/tests/images/
--rw-r--r--   0 root         (0) root         (0)     7525 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/images/1.jpg
--rw-r--r--   0 root         (0) root         (0)     4388 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/images/2.jpg
--rw-r--r--   0 root         (0) root         (0)    80712 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/images/image.jpg
--rw-r--r--   0 root         (0) root         (0)      493 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/javadrivertest.py
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/minicap_test.py
--rw-r--r--   0 root         (0) root         (0)      375 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/minitest.py
--rw-r--r--   0 root         (0) root         (0)      843 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/minitouch_test.py
--rw-r--r--   0 root         (0) root         (0)      792 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/u2test.py
--rw-r--r--   0 root         (0) root         (0)     1797 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/uixmltest.py
--rw-r--r--   0 root         (0) root         (0)      493 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/vs_test.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/tests/webdrivertest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/utils/
--rw-r--r--   0 root         (0) root         (0)       37 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4896 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/apkinfo.py
--rw-r--r--   0 root         (0) root         (0)   105609 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/axmlparser.py
--rw-r--r--   0 root         (0) root         (0)    27360 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/axmlparser3.py
--rw-r--r--   0 root         (0) root         (0)      526 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/commonhelper.py
--rw-r--r--   0 root         (0) root         (0)     8332 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/decorator.py
--rw-r--r--   0 root         (0) root         (0)      257 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/magic.py
--rw-r--r--   0 root         (0) root         (0)     2457 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/nbsp.py
--rw-r--r--   0 root         (0) root         (0)     1435 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/utils/threadhelper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.623251 minium-1.5.3/minium/externlib/at/vision/
--rw-r--r--   0 root         (0) root         (0)       56 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/vision/__init__.py
--rw-r--r--   0 root         (0) root         (0)      394 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/vision/template_match.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/at/webdriver/
--rw-r--r--   0 root         (0) root         (0)       72 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15310 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/driver.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/error.py
--rw-r--r--   0 root         (0) root         (0)     1376 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/jsapi.py
--rw-r--r--   0 root         (0) root         (0)     1519 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/miniapp.py
--rw-r--r--   0 root         (0) root         (0)    18973 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/stub.js
--rw-r--r--   0 root         (0) root         (0)      682 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/tabdescription.py
--rw-r--r--   0 root         (0) root         (0)    13042 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/tabwebsocket.py
--rw-r--r--   0 root         (0) root         (0)     8904 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/webelement.py
--rw-r--r--   0 root         (0) root         (0)     1638 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/webhelper.py
--rw-r--r--   0 root         (0) root         (0)     1399 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/webdriver/wspools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/at/wechat/
--rw-r--r--   0 root         (0) root         (0)       79 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/wechat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/wechat/activtiy.py
--rw-r--r--   0 root         (0) root         (0)      144 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/wechat/appvars.py
--rw-r--r--   0 root         (0) root         (0)       80 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/at/wsimp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/bin/
--rwxr-xr-x   0 root         (0) root         (0)      993 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/bin/wat
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/case_repair_sdk/
--rw-r--r--   0 root         (0) root         (0)     7663 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/case_repair_sdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2816 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/case_repair_sdk/default_trace.py
--rw-r--r--   0 root         (0) root         (0)       53 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/wda/
--rw-r--r--   0 root         (0) root         (0)    44144 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1297 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wda/screenhelper.py
--rw-r--r--   0 root         (0) root         (0)     1421 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wda/xcui_element_types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/wechat_mp_inspector/
--rw-r--r--   0 root         (0) root         (0)      672 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6474 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/basemp.py
--rw-r--r--   0 root         (0) root         (0)    33040 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/basewebsocket.py
--rw-r--r--   0 root         (0) root         (0)      134 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/build_info.json
--rw-r--r--   0 root         (0) root         (0)     6348 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/cdpdriver.py
--rw-r--r--   0 root         (0) root         (0)     3780 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.627251 minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/
--rw-r--r--   0 root         (0) root         (0)      252 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13797 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/baseconn.py
--rw-r--r--   0 root         (0) root         (0)     5771 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/lockdownconn.py
--rw-r--r--   0 root         (0) root         (0)    25513 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/websocketconn.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.631251 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/
--rw-r--r--   0 root         (0) root         (0)      248 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8489 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/androiddriver.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/basedriver.py
--rw-r--r--   0 root         (0) root         (0)     1906 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/config.py
--rw-r--r--   0 root         (0) root         (0)     6173 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/iosdriver.py
--rw-r--r--   0 root         (0) root         (0)    49409 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/mpdriver.py
--rw-r--r--   0 root         (0) root         (0)     1481 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/emitter.py
--rw-r--r--   0 root         (0) root         (0)     1181 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/event.py
--rw-r--r--   0 root         (0) root         (0)      153 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.631251 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/
--rw-r--r--   0 root         (0) root         (0)      371 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1537 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/androidinspector.py
--rw-r--r--   0 root         (0) root         (0)    10254 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/androidwxainspector.py
--rw-r--r--   0 root         (0) root         (0)     1461 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/baseinspector.py
--rw-r--r--   0 root         (0) root         (0)     4241 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/iosinspector.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/ioswxainspector.py
--rw-r--r--   0 root         (0) root         (0)     1778 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/lazyloader.py
--rw-r--r--   0 root         (0) root         (0)      759 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/logger.py
--rw-r--r--   0 root         (0) root         (0)    32713 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/miniprogram.py
--rw-r--r--   0 root         (0) root         (0)     9521 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/mpdriver.py
--rw-r--r--   0 root         (0) root         (0)     5848 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/officialaccount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.631251 minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/basepage.py
--rw-r--r--   0 root         (0) root         (0)     4745 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/chromepage.py
--rw-r--r--   0 root         (0) root         (0)     3300 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/safaripage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.631251 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/
--rw-r--r--   0 root         (0) root         (0)      253 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/__init__.py
--rw-r--r--   0 root         (0) root         (0)      838 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/baseprotocol.py
--rw-r--r--   0 root         (0) root         (0)     3538 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/basesession.py
--rw-r--r--   0 root         (0) root         (0)     1851 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/basewebkit.py
--rw-r--r--   0 root         (0) root         (0)     6105 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/cdp.py
--rw-r--r--   0 root         (0) root         (0)     2118 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/protocolcommand.py
--rw-r--r--   0 root         (0) root         (0)   294746 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/protocoltypes.py
--rw-r--r--   0 root         (0) root         (0)     3231 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/wip.py
--rw-r--r--   0 root         (0) root         (0)     2448 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/title.py
--rw-r--r--   0 root         (0) root         (0)    15316 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wechat_mp_inspector/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.631251 minium-1.5.3/minium/externlib/wx_wda/
--rw-r--r--   0 root         (0) root         (0)      448 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wx_wda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13280 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wx_wda/wdaUI.py
--rw-r--r--   0 root         (0) root         (0)    16692 2024-01-08 08:32:33.000000 minium-1.5.3/minium/externlib/wx_wda/webDriverTool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/
--rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19022 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/assertbase.py
--rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.5.3/minium/framework/casedump.py
--rw-r--r--   0 root         (0) root         (0)     7785 2023-08-28 08:37:33.000000 minium-1.5.3/minium/framework/caseinspect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/dist/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/dist/css/
--rw-r--r--   0 root         (0) root         (0)      763 2024-01-12 03:15:59.000000 minium-1.5.3/minium/framework/dist/css/app.a0b163c8.css
--rw-r--r--   0 root         (0) root         (0)   241389 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/dist/css/chunk-vendors.1d2c6903.css
--rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/dist/favicon.ico
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/dist/fonts/
--rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/dist/fonts/element-icons.535877f5.woff
--rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/dist/fonts/element-icons.732389de.ttf
--rw-r--r--   0 root         (0) root         (0)      847 2024-01-12 03:15:59.000000 minium-1.5.3/minium/framework/dist/index.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/dist/js/
--rw-r--r--   0 root         (0) root         (0)    20660 2024-01-12 03:15:59.000000 minium-1.5.3/minium/framework/dist/js/app.f6da66fe.js
--rw-r--r--   0 root         (0) root         (0)  1465900 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/dist/js/chunk-vendors.76d61689.js
--rw-r--r--   0 root         (0) root         (0)     3447 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/errorReport.py
--rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.635251 minium-1.5.3/minium/framework/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/framework/libs/tgit/
--rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/libs/tgit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/libs/tgit/auth.py
--rw-r--r--   0 root         (0) root         (0)    97167 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/libs/tgit/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/framework/libs/unittest/
--rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.5.3/minium/framework/libs/unittest/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22297 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/libs/unittest/case.py
--rw-r--r--   0 root         (0) root         (0)     5629 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/libs/unittest/suite.py
--rw-r--r--   0 root         (0) root         (0)    22119 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/loader.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-08-28 08:37:33.000000 minium-1.5.3/minium/framework/logcolor.py
--rw-r--r--   0 root         (0) root         (0)     7414 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/miniconfig.py
--rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/miniddt.py
--rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.5.3/minium/framework/minidoctor.py
--rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/minilimit.py
--rw-r--r--   0 root         (0) root         (0)     1268 2023-08-28 08:37:33.000000 minium-1.5.3/minium/framework/miniprogram.py
--rw-r--r--   0 root         (0) root         (0)     6974 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/miniresult.py
--rw-r--r--   0 root         (0) root         (0)     3573 2023-06-21 12:00:44.000000 minium-1.5.3/minium/framework/minisuite.py
--rw-r--r--   0 root         (0) root         (0)    35267 2024-01-08 08:32:33.000000 minium-1.5.3/minium/framework/minitest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2023-08-28 08:37:33.000000 minium-1.5.3/minium/framework/modifier.py
--rw-r--r--   0 root         (0) root         (0)    17061 2023-04-27 02:49:43.000000 minium-1.5.3/minium/framework/report.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.5.3/minium/framework/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/framework/tools/
--rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.5.3/minium/framework/tools/report_issue.py
--rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.5.3/minium/framework/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/miniprogram/
--rw-r--r--   0 root         (0) root         (0)      688 2023-04-27 02:49:43.000000 minium-1.5.3/minium/miniprogram/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/miniprogram/base_driver/
--rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.5.3/minium/miniprogram/base_driver/__init__.py
--rw-r--r--   0 root         (0) root         (0)    59899 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/app.py
--rw-r--r--   0 root         (0) root         (0)     4634 2023-08-28 08:37:33.000000 minium-1.5.3/minium/miniprogram/base_driver/callback.py
--rw-r--r--   0 root         (0) root         (0)    29122 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/connection.py
--rw-r--r--   0 root         (0) root         (0)    46903 2023-08-28 08:37:33.000000 minium-1.5.3/minium/miniprogram/base_driver/element.py
--rw-r--r--   0 root         (0) root         (0)    18066 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/h5_element.py
--rw-r--r--   0 root         (0) root         (0)     1987 2023-08-28 08:37:33.000000 minium-1.5.3/minium/miniprogram/base_driver/minium.py
--rw-r--r--   0 root         (0) root         (0)     5959 2023-06-21 12:00:44.000000 minium-1.5.3/minium/miniprogram/base_driver/minium_log.py
--rw-r--r--   0 root         (0) root         (0)    10290 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/minium_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/miniprogram/base_driver/page/
--rw-r--r--   0 root         (0) root         (0)     5146 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/page/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27073 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/page/h5page.py
--rw-r--r--   0 root         (0) root         (0)    25093 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/page/page.py
--rw-r--r--   0 root         (0) root         (0)     1790 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/page/skylinepage.py
--rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.5.3/minium/miniprogram/base_driver/prefixer.py
--rw-r--r--   0 root         (0) root         (0)      132 2024-01-15 11:47:47.000000 minium-1.5.3/minium/miniprogram/base_driver/version.json
--rw-r--r--   0 root         (0) root         (0)      816 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/base_driver/version.py
--rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.5.3/minium/miniprogram/base_driver/waiter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/miniprogram/h5tools/
--rw-r--r--   0 root         (0) root         (0)        0 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2534 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/client.py
--rw-r--r--   0 root         (0) root         (0)     2754 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/commandProcessor.py
--rw-r--r--   0 root         (0) root         (0)     3745 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5816 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/h5CommandManager.py
--rw-r--r--   0 root         (0) root         (0)    11330 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/h5PageOperator.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/h5UserAPI.py
--rw-r--r--   0 root         (0) root         (0)     1827 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/jsonConcat.py
--rw-r--r--   0 root         (0) root         (0)     1118 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/logger.py
--rw-r--r--   0 root         (0) root         (0)     1778 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/h5tools/utils.py
--rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.5.3/minium/miniprogram/qq_minium.py
--rw-r--r--   0 root         (0) root         (0)    40301 2024-01-08 08:32:33.000000 minium-1.5.3/minium/miniprogram/wx_minium.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/native/
--rw-r--r--   0 root         (0) root         (0)     3522 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/__init__.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.5.3/minium/native/exception.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.639251 minium-1.5.3/minium/native/qq_native/
--rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.5.3/minium/native/qq_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.5.3/minium/native/qq_native/qandroidnative.py
--rw-r--r--   0 root         (0) root         (0)     1148 2023-06-21 12:00:44.000000 minium-1.5.3/minium/native/qq_native/qbasenative.py
--rwxr-xr-x   0 root         (0) root         (0)    16848 2023-06-21 12:00:44.000000 minium-1.5.3/minium/native/qq_native/qiosnative.py
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.5.3/minium/native/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.643251 minium-1.5.3/minium/native/wx_native/
--rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.5.3/minium/native/wx_native/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65332 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/wx_native/androidnative.py
--rw-r--r--   0 root         (0) root         (0)    28967 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/wx_native/basenative.py
--rw-r--r--   0 root         (0) root         (0)    10749 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/wx_native/idenative.py
--rw-r--r--   0 root         (0) root         (0)    62519 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/wx_native/iosnative.py
--rw-r--r--   0 root         (0) root         (0)     3616 2024-01-08 08:32:33.000000 minium-1.5.3/minium/native/wx_native/wording.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.643251 minium-1.5.3/minium/utils/
--rw-r--r--   0 root         (0) root         (0)      444 2023-08-28 08:37:33.000000 minium-1.5.3/minium/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.5.3/minium/utils/emitter.py
--rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.5.3/minium/utils/eventloop.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-08-28 08:37:33.000000 minium-1.5.3/minium/utils/injectjs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium/utils/js/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.647251 minium-1.5.3/minium/utils/js/es5/
--rw-r--r--   0 root         (0) root         (0)      146 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      164 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      281 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)      144 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/checkEnv.js
--rw-r--r--   0 root         (0) root         (0)       76 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      157 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      545 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/createContext.js
--rw-r--r--   0 root         (0) root         (0)      346 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      235 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      284 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/getCurrentPages.js
--rw-r--r--   0 root         (0) root         (0)      617 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2024-01-15 11:47:31.000000 minium-1.5.3/minium/utils/js/es5/helpers.js
--rw-r--r--   0 root         (0) root         (0)     3971 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/hijackWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      425 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      235 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      244 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/hookWxMethodWithId.js
--rw-r--r--   0 root         (0) root         (0)      124 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      215 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      124 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      493 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      218 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1188 2024-01-15 11:47:29.000000 minium-1.5.3/minium/utils/js/es5/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1206 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      461 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      699 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1524 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      443 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      436 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      503 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)      259 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/initMockWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     4829 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      814 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     1869 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      194 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/mockWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1274 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      322 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1031 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/requestStack.js
--rw-r--r--   0 root         (0) root         (0)       84 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/restoreWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      295 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      208 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)     7135 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/testAsync.js
--rw-r--r--   0 root         (0) root         (0)     2896 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/utils.js
--rw-r--r--   0 root         (0) root         (0)      311 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/uuid.js
--rw-r--r--   0 root         (0) root         (0)      183 2024-01-15 11:47:30.000000 minium-1.5.3/minium/utils/js/es5/waitUtil.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.647251 minium-1.5.3/minium/utils/js/min/
--rw-r--r--   0 root         (0) root         (0)      138 2024-01-15 11:47:45.000000 minium-1.5.3/minium/utils/js/min/addCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      165 2024-01-15 11:47:42.000000 minium-1.5.3/minium/utils/js/min/addNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      202 2024-01-15 11:47:43.000000 minium-1.5.3/minium/utils/js/min/callContextMethod.js
--rw-r--r--   0 root         (0) root         (0)      136 2024-01-15 11:47:34.000000 minium-1.5.3/minium/utils/js/min/checkEnv.js
--rw-r--r--   0 root         (0) root         (0)       77 2024-01-15 11:47:37.000000 minium-1.5.3/minium/utils/js/min/checkInject.js
--rw-r--r--   0 root         (0) root         (0)      130 2024-01-15 11:47:38.000000 minium-1.5.3/minium/utils/js/min/cleanCloudCallMockRule.js
--rw-r--r--   0 root         (0) root         (0)      158 2024-01-15 11:47:37.000000 minium-1.5.3/minium/utils/js/min/cleanNetworkMockRule.js
--rw-r--r--   0 root         (0) root         (0)      422 2024-01-15 11:47:36.000000 minium-1.5.3/minium/utils/js/min/createContext.js
--rw-r--r--   0 root         (0) root         (0)      312 2024-01-15 11:47:39.000000 minium-1.5.3/minium/utils/js/min/editEditorText.js
--rw-r--r--   0 root         (0) root         (0)      187 2024-01-15 11:47:42.000000 minium-1.5.3/minium/utils/js/min/evalMockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      146 2024-01-15 11:47:40.000000 minium-1.5.3/minium/utils/js/min/getAppConfig.js
--rw-r--r--   0 root         (0) root         (0)      295 2024-01-15 11:47:33.000000 minium-1.5.3/minium/utils/js/min/getCurrentPages.js
--rw-r--r--   0 root         (0) root         (0)      555 2024-01-15 11:47:45.000000 minium-1.5.3/minium/utils/js/min/getUni.js
--rw-r--r--   0 root         (0) root         (0)    38266 2024-01-15 11:47:44.000000 minium-1.5.3/minium/utils/js/min/helpers.js
--rw-r--r--   0 root         (0) root         (0)     3250 2024-01-15 11:47:44.000000 minium-1.5.3/minium/utils/js/min/hijackWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      329 2024-01-15 11:47:40.000000 minium-1.5.3/minium/utils/js/min/hookCurrentPageMethod.js
--rw-r--r--   0 root         (0) root         (0)      221 2024-01-15 11:47:42.000000 minium-1.5.3/minium/utils/js/min/hookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      230 2024-01-15 11:47:37.000000 minium-1.5.3/minium/utils/js/min/hookWxMethodWithId.js
--rw-r--r--   0 root         (0) root         (0)      125 2024-01-15 11:47:34.000000 minium-1.5.3/minium/utils/js/min/ideHandleAuthModal.js
--rw-r--r--   0 root         (0) root         (0)      210 2024-01-15 11:47:33.000000 minium-1.5.3/minium/utils/js/min/ideHandleMap.js
--rw-r--r--   0 root         (0) root         (0)      125 2024-01-15 11:47:42.000000 minium-1.5.3/minium/utils/js/min/ideHandleModal.js
--rw-r--r--   0 root         (0) root         (0)      476 2024-01-15 11:47:33.000000 minium-1.5.3/minium/utils/js/min/ideMockAuth.js
--rw-r--r--   0 root         (0) root         (0)      156 2024-01-15 11:47:36.000000 minium-1.5.3/minium/utils/js/min/ideMockAuthSetting.js
--rw-r--r--   0 root         (0) root         (0)     1130 2024-01-15 11:47:36.000000 minium-1.5.3/minium/utils/js/min/ideMockChooseLocation.js
--rw-r--r--   0 root         (0) root         (0)     1212 2024-01-15 11:47:40.000000 minium-1.5.3/minium/utils/js/min/ideMockGetLocation.js
--rw-r--r--   0 root         (0) root         (0)      430 2024-01-15 11:47:43.000000 minium-1.5.3/minium/utils/js/min/ideMockGetUserProfile.js
--rw-r--r--   0 root         (0) root         (0)      705 2024-01-15 11:47:33.000000 minium-1.5.3/minium/utils/js/min/ideMockGetWeRunData.js
--rw-r--r--   0 root         (0) root         (0)     1457 2024-01-15 11:47:35.000000 minium-1.5.3/minium/utils/js/min/ideMockModal.js
--rw-r--r--   0 root         (0) root         (0)      419 2024-01-15 11:47:38.000000 minium-1.5.3/minium/utils/js/min/ideMockShowActionSheet.js
--rw-r--r--   0 root         (0) root         (0)      419 2024-01-15 11:47:32.000000 minium-1.5.3/minium/utils/js/min/ideMockShowModal.js
--rw-r--r--   0 root         (0) root         (0)      496 2024-01-15 11:47:36.000000 minium-1.5.3/minium/utils/js/min/ideMockSubscribeMessage.js
--rw-r--r--   0 root         (0) root         (0)      262 2024-01-15 11:47:44.000000 minium-1.5.3/minium/utils/js/min/initMockWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     4032 2024-01-15 11:47:34.000000 minium-1.5.3/minium/utils/js/min/mockChooseImage.js
--rw-r--r--   0 root         (0) root         (0)      778 2024-01-15 11:47:41.000000 minium-1.5.3/minium/utils/js/min/mockCloudCall.js
--rw-r--r--   0 root         (0) root         (0)     1476 2024-01-15 11:47:35.000000 minium-1.5.3/minium/utils/js/min/mockNetwork.js
--rw-r--r--   0 root         (0) root         (0)      182 2024-01-15 11:47:35.000000 minium-1.5.3/minium/utils/js/min/mockWxMethod.js
--rw-r--r--   0 root         (0) root         (0)     1280 2024-01-15 11:47:32.000000 minium-1.5.3/minium/utils/js/min/networkPannel.js
--rw-r--r--   0 root         (0) root         (0)      304 2024-01-15 11:47:38.000000 minium-1.5.3/minium/utils/js/min/releaseHookWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      895 2024-01-15 11:47:39.000000 minium-1.5.3/minium/utils/js/min/requestStack.js
--rw-r--r--   0 root         (0) root         (0)       85 2024-01-15 11:47:40.000000 minium-1.5.3/minium/utils/js/min/restoreWxMethod.js
--rw-r--r--   0 root         (0) root         (0)      294 2024-01-15 11:47:41.000000 minium-1.5.3/minium/utils/js/min/startGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)      209 2024-01-15 11:47:38.000000 minium-1.5.3/minium/utils/js/min/stopGetPerformance.js
--rw-r--r--   0 root         (0) root         (0)       94 2024-01-15 11:47:46.000000 minium-1.5.3/minium/utils/js/min/testAsync.js
--rw-r--r--   0 root         (0) root         (0)     2351 2024-01-15 11:47:39.000000 minium-1.5.3/minium/utils/js/min/utils.js
--rw-r--r--   0 root         (0) root         (0)      304 2024-01-15 11:47:45.000000 minium-1.5.3/minium/utils/js/min/uuid.js
--rw-r--r--   0 root         (0) root         (0)       69 2024-01-15 11:47:41.000000 minium-1.5.3/minium/utils/js/min/waitUtil.js
--rw-r--r--   0 root         (0) root         (0)     1984 2024-01-12 03:15:59.000000 minium-1.5.3/minium/utils/lazyloader.py
--rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.5.3/minium/utils/meta.py
--rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.5.3/minium/utils/platforms.py
--rw-r--r--   0 root         (0) root         (0)    17871 2024-01-08 08:32:33.000000 minium-1.5.3/minium/utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-15 11:47:51.615251 minium-1.5.3/minium.egg-info/
--rw-r--r--   0 root         (0) root         (0)      699 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12769 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      147 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-01-15 11:47:50.000000 minium-1.5.3/minium.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-15 11:47:51.651251 minium-1.5.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2953 2024-01-15 09:16:38.000000 minium-1.5.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.765286 minium-1.5.4/
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-15 09:01:56.000000 minium-1.5.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      699 2024-04-22 13:01:37.765286 minium-1.5.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.729286 minium-1.5.4/minium/
+-rw-r--r--   0 root         (0) root         (0)     1213 2024-01-08 08:32:33.000000 minium-1.5.4/minium/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.733286 minium-1.5.4/minium/externlib/
+-rw-r--r--   0 root         (0) root         (0)       58 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.733286 minium-1.5.4/minium/externlib/android_base/
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/android_base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.733286 minium-1.5.4/minium/externlib/at/
+-rw-r--r--   0 root         (0) root         (0)     4087 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1755 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/apkapi.py
+-rw-r--r--   0 root         (0) root         (0)     5609 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/atproxy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.737286 minium-1.5.4/minium/externlib/at/bin/
+-rw-r--r--   0 root         (0) root         (0)  3566862 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/bin/AtServer.apk
+-rw-r--r--   0 root         (0) root         (0)    95449 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/bin/AtStub.jar
+-rw-r--r--   0 root         (0) root         (0)     3222 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/command_line.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.737286 minium-1.5.4/minium/externlib/at/core/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      951 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/accesshelper.py
+-rw-r--r--   0 root         (0) root         (0)    47044 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/adbwrap.py
+-rw-r--r--   0 root         (0) root         (0)    10763 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)    15919 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/case_repair_adapter.py
+-rw-r--r--   0 root         (0) root         (0)      624 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    31731 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/element.py
+-rw-r--r--   0 root         (0) root         (0)      669 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)    18740 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/javadriver.py
+-rw-r--r--   0 root         (0) root         (0)     3620 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/resguard.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.737286 minium-1.5.4/minium/externlib/at/core/stf/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/stf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/stf/mincap.py
+-rw-r--r--   0 root         (0) root         (0)     5507 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/stf/minitouch.py
+-rw-r--r--   0 root         (0) root         (0)    11596 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/uidevice.py
+-rw-r--r--   0 root         (0) root         (0)    17965 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/uixml.py
+-rw-r--r--   0 root         (0) root         (0)     2711 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/core/websocketcli.py
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/eventmonitor.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/hook.py
+-rw-r--r--   0 root         (0) root         (0)     8495 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/jlogcat.py
+-rw-r--r--   0 root         (0) root         (0)    36015 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/keycode.py
+-rw-r--r--   0 root         (0) root         (0)     9492 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/perfcollector.py
+-rw-r--r--   0 root         (0) root         (0)        7 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.737286 minium-1.5.4/minium/externlib/at/tests/
+-rw-r--r--   0 root         (0) root         (0)      690 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/AtEvent.py
+-rw-r--r--   0 root         (0) root         (0)      326 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/AtSocket.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/adbtest.py
+-rw-r--r--   0 root         (0) root         (0)      490 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/airtesttest.py
+-rw-r--r--   0 root         (0) root         (0)    10434 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/atdevicetest.py
+-rw-r--r--   0 root         (0) root         (0)      474 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/attestbase.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/drivertest.py
+-rw-r--r--   0 root         (0) root         (0)     1768 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/elementtest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.737286 minium-1.5.4/minium/externlib/at/tests/images/
+-rw-r--r--   0 root         (0) root         (0)     7525 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/images/1.jpg
+-rw-r--r--   0 root         (0) root         (0)     4388 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/images/2.jpg
+-rw-r--r--   0 root         (0) root         (0)    80712 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/images/image.jpg
+-rw-r--r--   0 root         (0) root         (0)      493 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/javadrivertest.py
+-rw-r--r--   0 root         (0) root         (0)      480 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/minicap_test.py
+-rw-r--r--   0 root         (0) root         (0)      375 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/minitest.py
+-rw-r--r--   0 root         (0) root         (0)      843 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/minitouch_test.py
+-rw-r--r--   0 root         (0) root         (0)      792 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/u2test.py
+-rw-r--r--   0 root         (0) root         (0)     1797 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/uixmltest.py
+-rw-r--r--   0 root         (0) root         (0)      493 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/vs_test.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/tests/webdrivertest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/at/utils/
+-rw-r--r--   0 root         (0) root         (0)       37 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4896 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/apkinfo.py
+-rw-r--r--   0 root         (0) root         (0)   105609 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/axmlparser.py
+-rw-r--r--   0 root         (0) root         (0)    27360 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/axmlparser3.py
+-rw-r--r--   0 root         (0) root         (0)      526 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/commonhelper.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/decorator.py
+-rw-r--r--   0 root         (0) root         (0)      257 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/magic.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/nbsp.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/utils/threadhelper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/at/vision/
+-rw-r--r--   0 root         (0) root         (0)       56 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/vision/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      394 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/vision/template_match.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/at/webdriver/
+-rw-r--r--   0 root         (0) root         (0)       72 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15310 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/driver.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/error.py
+-rw-r--r--   0 root         (0) root         (0)     1376 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/jsapi.py
+-rw-r--r--   0 root         (0) root         (0)     1519 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/miniapp.py
+-rw-r--r--   0 root         (0) root         (0)    18973 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/stub.js
+-rw-r--r--   0 root         (0) root         (0)      682 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/tabdescription.py
+-rw-r--r--   0 root         (0) root         (0)    13042 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/tabwebsocket.py
+-rw-r--r--   0 root         (0) root         (0)     8904 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/webelement.py
+-rw-r--r--   0 root         (0) root         (0)     1638 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/webhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/webdriver/wspools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/at/wechat/
+-rw-r--r--   0 root         (0) root         (0)       79 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/wechat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/wechat/activtiy.py
+-rw-r--r--   0 root         (0) root         (0)      144 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/wechat/appvars.py
+-rw-r--r--   0 root         (0) root         (0)       80 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/at/wsimp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/bin/
+-rwxr-xr-x   0 root         (0) root         (0)      993 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/bin/wat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/case_repair_sdk/
+-rw-r--r--   0 root         (0) root         (0)     7663 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/case_repair_sdk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2816 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/case_repair_sdk/default_trace.py
+-rw-r--r--   0 root         (0) root         (0)       53 2024-04-15 09:01:56.000000 minium-1.5.4/minium/externlib/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/wda/
+-rw-r--r--   0 root         (0) root         (0)    44548 2024-04-22 13:00:37.000000 minium-1.5.4/minium/externlib/wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/wda/screenhelper.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/wda/xcui_element_types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/wechat_mp_inspector/
+-rw-r--r--   0 root         (0) root         (0)      672 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6921 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/basemp.py
+-rw-r--r--   0 root         (0) root         (0)    33040 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/basewebsocket.py
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/build_info.json
+-rw-r--r--   0 root         (0) root         (0)     6348 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/cdpdriver.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.741286 minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19519 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/baseconn.py
+-rw-r--r--   0 root         (0) root         (0)     9018 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/lockdownconn.py
+-rw-r--r--   0 root         (0) root         (0)    25525 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/websocketconn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.745286 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/
+-rw-r--r--   0 root         (0) root         (0)      248 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10054 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/androiddriver.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/basedriver.py
+-rw-r--r--   0 root         (0) root         (0)     2313 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/config.py
+-rw-r--r--   0 root         (0) root         (0)     6626 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/iosdriver.py
+-rw-r--r--   0 root         (0) root         (0)    63908 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/mpdriver.py
+-rw-r--r--   0 root         (0) root         (0)     6493 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/officialaccount.py
+-rw-r--r--   0 root         (0) root         (0)     1481 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/emitter.py
+-rw-r--r--   0 root         (0) root         (0)     1181 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/event.py
+-rw-r--r--   0 root         (0) root         (0)      153 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.745286 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/
+-rw-r--r--   0 root         (0) root         (0)      371 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1608 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/androidinspector.py
+-rw-r--r--   0 root         (0) root         (0)     8038 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/androidwxainspector.py
+-rw-r--r--   0 root         (0) root         (0)     1742 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/baseinspector.py
+-rw-r--r--   0 root         (0) root         (0)     6673 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/iosinspector.py
+-rw-r--r--   0 root         (0) root         (0)     8346 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/ioswxainspector.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/wxainspector.py
+-rw-r--r--   0 root         (0) root         (0)     5671 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/lazyloader.py
+-rw-r--r--   0 root         (0) root         (0)      759 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/logger.py
+-rw-r--r--   0 root         (0) root         (0)    34395 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     9521 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/mpdriver.py
+-rw-r--r--   0 root         (0) root         (0)     5961 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/officialaccount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.745286 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1620 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/basepage.py
+-rw-r--r--   0 root         (0) root         (0)     5361 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/chromepage.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/mppage.py
+-rw-r--r--   0 root         (0) root         (0)     3762 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/safaripage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.745286 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/
+-rw-r--r--   0 root         (0) root         (0)      253 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      868 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/baseprotocol.py
+-rw-r--r--   0 root         (0) root         (0)     4005 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/basesession.py
+-rw-r--r--   0 root         (0) root         (0)     1851 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/basewebkit.py
+-rw-r--r--   0 root         (0) root         (0)     6127 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/cdp.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/protocolcommand.py
+-rw-r--r--   0 root         (0) root         (0)   323628 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/protocoltypes.py
+-rw-r--r--   0 root         (0) root         (0)    12103 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/wip.py
+-rw-r--r--   0 root         (0) root         (0)     2448 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/title.py
+-rw-r--r--   0 root         (0) root         (0)    25166 2024-04-22 13:01:28.000000 minium-1.5.4/minium/externlib/wechat_mp_inspector/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.745286 minium-1.5.4/minium/externlib/wx_wda/
+-rw-r--r--   0 root         (0) root         (0)      448 2024-01-08 08:32:33.000000 minium-1.5.4/minium/externlib/wx_wda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13600 2024-04-15 09:01:56.000000 minium-1.5.4/minium/externlib/wx_wda/wdaUI.py
+-rw-r--r--   0 root         (0) root         (0)    26780 2024-04-15 09:01:56.000000 minium-1.5.4/minium/externlib/wx_wda/webDriverTool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/
+-rw-r--r--   0 root         (0) root         (0)       58 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19022 2024-01-08 08:32:33.000000 minium-1.5.4/minium/framework/assertbase.py
+-rw-r--r--   0 root         (0) root         (0)     1587 2022-11-07 03:36:55.000000 minium-1.5.4/minium/framework/casedump.py
+-rw-r--r--   0 root         (0) root         (0)     7785 2023-08-28 08:37:33.000000 minium-1.5.4/minium/framework/caseinspect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/dist/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/dist/css/
+-rw-r--r--   0 root         (0) root         (0)      763 2024-01-12 03:15:59.000000 minium-1.5.4/minium/framework/dist/css/app.a0b163c8.css
+-rw-r--r--   0 root         (0) root         (0)   241389 2024-01-08 08:32:33.000000 minium-1.5.4/minium/framework/dist/css/chunk-vendors.1d2c6903.css
+-rw-r--r--   0 root         (0) root         (0)     2108 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/dist/favicon.ico
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/dist/fonts/
+-rw-r--r--   0 root         (0) root         (0)    28200 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/dist/fonts/element-icons.535877f5.woff
+-rw-r--r--   0 root         (0) root         (0)    55956 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/dist/fonts/element-icons.732389de.ttf
+-rw-r--r--   0 root         (0) root         (0)      847 2024-01-12 03:15:59.000000 minium-1.5.4/minium/framework/dist/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/dist/js/
+-rw-r--r--   0 root         (0) root         (0)    20660 2024-01-12 03:15:59.000000 minium-1.5.4/minium/framework/dist/js/app.f6da66fe.js
+-rw-r--r--   0 root         (0) root         (0)  1465900 2024-01-08 08:32:33.000000 minium-1.5.4/minium/framework/dist/js/chunk-vendors.76d61689.js
+-rw-r--r--   0 root         (0) root         (0)     2398 2023-06-21 12:00:44.000000 minium-1.5.4/minium/framework/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/libs/tgit/
+-rw-r--r--   0 root         (0) root         (0)      152 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/libs/tgit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1007 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/libs/tgit/auth.py
+-rw-r--r--   0 root         (0) root         (0)    97167 2023-06-21 12:00:44.000000 minium-1.5.4/minium/framework/libs/tgit/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/libs/unittest/
+-rw-r--r--   0 root         (0) root         (0)      243 2022-12-28 03:15:03.000000 minium-1.5.4/minium/framework/libs/unittest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22332 2024-04-15 09:01:56.000000 minium-1.5.4/minium/framework/libs/unittest/case.py
+-rw-r--r--   0 root         (0) root         (0)     5629 2023-06-21 12:00:44.000000 minium-1.5.4/minium/framework/libs/unittest/suite.py
+-rw-r--r--   0 root         (0) root         (0)    22143 2024-04-22 13:00:37.000000 minium-1.5.4/minium/framework/loader.py
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-08-28 08:37:33.000000 minium-1.5.4/minium/framework/logcolor.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2024-04-22 13:00:37.000000 minium-1.5.4/minium/framework/miniconfig.py
+-rw-r--r--   0 root         (0) root         (0)     3427 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/miniddt.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-07 07:19:07.000000 minium-1.5.4/minium/framework/minidoctor.py
+-rw-r--r--   0 root         (0) root         (0)     1207 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/minilimit.py
+-rw-r--r--   0 root         (0) root         (0)     1268 2023-08-28 08:37:33.000000 minium-1.5.4/minium/framework/miniprogram.py
+-rw-r--r--   0 root         (0) root         (0)     6974 2024-01-08 08:32:33.000000 minium-1.5.4/minium/framework/miniresult.py
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-06-21 12:00:44.000000 minium-1.5.4/minium/framework/minisuite.py
+-rw-r--r--   0 root         (0) root         (0)    36729 2024-04-22 13:00:37.000000 minium-1.5.4/minium/framework/minitest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-08-28 08:37:33.000000 minium-1.5.4/minium/framework/modifier.py
+-rw-r--r--   0 root         (0) root         (0)    17113 2024-01-29 03:14:44.000000 minium-1.5.4/minium/framework/report.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-05-09 06:36:06.000000 minium-1.5.4/minium/framework/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/framework/tools/
+-rw-r--r--   0 root         (0) root         (0)       54 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2716 2022-06-30 06:29:28.000000 minium-1.5.4/minium/framework/tools/report_issue.py
+-rw-r--r--   0 root         (0) root         (0)     3974 2022-12-19 02:27:07.000000 minium-1.5.4/minium/framework/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.749286 minium-1.5.4/minium/miniprogram/
+-rw-r--r--   0 root         (0) root         (0)      726 2024-04-15 09:01:56.000000 minium-1.5.4/minium/miniprogram/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/miniprogram/base_driver/
+-rw-r--r--   0 root         (0) root         (0)      191 2022-06-30 06:29:28.000000 minium-1.5.4/minium/miniprogram/base_driver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66034 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/app.py
+-rw-r--r--   0 root         (0) root         (0)     4802 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/callback.py
+-rw-r--r--   0 root         (0) root         (0)    29330 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/connection.py
+-rw-r--r--   0 root         (0) root         (0)    49414 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/element.py
+-rw-r--r--   0 root         (0) root         (0)    20263 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/h5_element.py
+-rw-r--r--   0 root         (0) root         (0)     1987 2023-08-28 08:37:33.000000 minium-1.5.4/minium/miniprogram/base_driver/minium.py
+-rw-r--r--   0 root         (0) root         (0)     7246 2024-04-15 09:01:56.000000 minium-1.5.4/minium/miniprogram/base_driver/minium_log.py
+-rw-r--r--   0 root         (0) root         (0)    10290 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/base_driver/minium_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/miniprogram/base_driver/page/
+-rw-r--r--   0 root         (0) root         (0)     5240 2024-04-15 09:01:56.000000 minium-1.5.4/minium/miniprogram/base_driver/page/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26481 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/page/h5page.py
+-rw-r--r--   0 root         (0) root         (0)    27835 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/base_driver/page/page.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/base_driver/page/skylinepage.py
+-rw-r--r--   0 root         (0) root         (0)      771 2022-06-30 06:29:28.000000 minium-1.5.4/minium/miniprogram/base_driver/prefixer.py
+-rw-r--r--   0 root         (0) root         (0)     4601 2024-04-15 09:01:56.000000 minium-1.5.4/minium/miniprogram/base_driver/selector.py
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-22 13:01:28.000000 minium-1.5.4/minium/miniprogram/base_driver/version.json
+-rw-r--r--   0 root         (0) root         (0)      816 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/base_driver/version.py
+-rw-r--r--   0 root         (0) root         (0)      263 2022-06-30 06:29:28.000000 minium-1.5.4/minium/miniprogram/base_driver/waiter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/miniprogram/h5tools/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2024-04-15 09:01:56.000000 minium-1.5.4/minium/miniprogram/h5tools/client.py
+-rw-r--r--   0 root         (0) root         (0)     2754 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/commandProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     3745 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5816 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/h5CommandManager.py
+-rw-r--r--   0 root         (0) root         (0)    11330 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/h5PageOperator.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/h5UserAPI.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/h5tools/jsonConcat.py
+-rw-r--r--   0 root         (0) root         (0)     1118 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1778 2024-01-08 08:32:33.000000 minium-1.5.4/minium/miniprogram/h5tools/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6692 2022-06-30 06:29:28.000000 minium-1.5.4/minium/miniprogram/qq_minium.py
+-rw-r--r--   0 root         (0) root         (0)    44781 2024-04-22 13:00:37.000000 minium-1.5.4/minium/miniprogram/wx_minium.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/native/
+-rw-r--r--   0 root         (0) root         (0)     4047 2024-04-22 13:00:37.000000 minium-1.5.4/minium/native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-06-30 06:29:28.000000 minium-1.5.4/minium/native/exception.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/native/qq_native/
+-rw-r--r--   0 root         (0) root         (0)      118 2022-06-30 06:29:28.000000 minium-1.5.4/minium/native/qq_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2022-06-30 06:29:28.000000 minium-1.5.4/minium/native/qq_native/qandroidnative.py
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-06-21 12:00:44.000000 minium-1.5.4/minium/native/qq_native/qbasenative.py
+-rwxr-xr-x   0 root         (0) root         (0)    16848 2023-06-21 12:00:44.000000 minium-1.5.4/minium/native/qq_native/qiosnative.py
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.5.4/minium/native/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.753286 minium-1.5.4/minium/native/wx_native/
+-rw-r--r--   0 root         (0) root         (0)       23 2022-06-30 06:29:28.000000 minium-1.5.4/minium/native/wx_native/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    77133 2024-04-22 13:00:37.000000 minium-1.5.4/minium/native/wx_native/androidnative.py
+-rw-r--r--   0 root         (0) root         (0)    32476 2024-04-22 13:00:37.000000 minium-1.5.4/minium/native/wx_native/basenative.py
+-rw-r--r--   0 root         (0) root         (0)    10749 2024-01-08 08:32:33.000000 minium-1.5.4/minium/native/wx_native/idenative.py
+-rw-r--r--   0 root         (0) root         (0)    71178 2024-04-22 13:00:37.000000 minium-1.5.4/minium/native/wx_native/iosnative.py
+-rw-r--r--   0 root         (0) root         (0)     3616 2024-01-08 08:32:33.000000 minium-1.5.4/minium/native/wx_native/wording.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.757286 minium-1.5.4/minium/utils/
+-rw-r--r--   0 root         (0) root         (0)      459 2024-01-29 03:14:44.000000 minium-1.5.4/minium/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2023-04-27 02:49:44.000000 minium-1.5.4/minium/utils/emitter.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-10-14 03:16:26.000000 minium-1.5.4/minium/utils/eventloop.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-08-28 08:37:33.000000 minium-1.5.4/minium/utils/injectjs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.729286 minium-1.5.4/minium/utils/js/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.761286 minium-1.5.4/minium/utils/js/es5/
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      164 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      281 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      144 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-22 13:01:09.000000 minium-1.5.4/minium/utils/js/es5/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      157 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      545 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      346 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      147 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      284 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/getCurrentPages.js
+-rw-r--r--   0 root         (0) root         (0)      617 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2024-04-22 13:01:12.000000 minium-1.5.4/minium/utils/js/es5/helpers.js
+-rw-r--r--   0 root         (0) root         (0)     3971 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/hijackWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)     2499 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/hookNavigation.js
+-rw-r--r--   0 root         (0) root         (0)      235 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      244 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/hookWxMethodWithId.js
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      215 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      493 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      218 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1188 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1206 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      461 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      699 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1524 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      443 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      436 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      503 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)      259 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/initMockWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     4829 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      814 2024-04-22 13:01:10.000000 minium-1.5.4/minium/utils/js/es5/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     1867 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      194 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/mockWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1414 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      322 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1031 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)       84 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/restoreWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      208 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)     7123 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)     2894 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/utils.js
+-rw-r--r--   0 root         (0) root         (0)      311 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/uuid.js
+-rw-r--r--   0 root         (0) root         (0)      183 2024-04-22 13:01:11.000000 minium-1.5.4/minium/utils/js/es5/waitUtil.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.765286 minium-1.5.4/minium/utils/js/min/
+-rw-r--r--   0 root         (0) root         (0)      138 2024-04-22 13:01:26.000000 minium-1.5.4/minium/utils/js/min/addCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      165 2024-04-22 13:01:23.000000 minium-1.5.4/minium/utils/js/min/addNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      202 2024-04-22 13:01:24.000000 minium-1.5.4/minium/utils/js/min/callContextMethod.js
+-rw-r--r--   0 root         (0) root         (0)      136 2024-04-22 13:01:14.000000 minium-1.5.4/minium/utils/js/min/checkEnv.js
+-rw-r--r--   0 root         (0) root         (0)       77 2024-04-22 13:01:17.000000 minium-1.5.4/minium/utils/js/min/checkInject.js
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-22 13:01:19.000000 minium-1.5.4/minium/utils/js/min/cleanCloudCallMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-22 13:01:18.000000 minium-1.5.4/minium/utils/js/min/cleanNetworkMockRule.js
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-22 13:01:17.000000 minium-1.5.4/minium/utils/js/min/createContext.js
+-rw-r--r--   0 root         (0) root         (0)      312 2024-04-22 13:01:20.000000 minium-1.5.4/minium/utils/js/min/editEditorText.js
+-rw-r--r--   0 root         (0) root         (0)      187 2024-04-22 13:01:23.000000 minium-1.5.4/minium/utils/js/min/evalMockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-22 13:01:21.000000 minium-1.5.4/minium/utils/js/min/getAppConfig.js
+-rw-r--r--   0 root         (0) root         (0)      295 2024-04-22 13:01:14.000000 minium-1.5.4/minium/utils/js/min/getCurrentPages.js
+-rw-r--r--   0 root         (0) root         (0)      555 2024-04-22 13:01:26.000000 minium-1.5.4/minium/utils/js/min/getUni.js
+-rw-r--r--   0 root         (0) root         (0)    38266 2024-04-22 13:01:25.000000 minium-1.5.4/minium/utils/js/min/helpers.js
+-rw-r--r--   0 root         (0) root         (0)     3250 2024-04-22 13:01:26.000000 minium-1.5.4/minium/utils/js/min/hijackWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      329 2024-04-22 13:01:21.000000 minium-1.5.4/minium/utils/js/min/hookCurrentPageMethod.js
+-rw-r--r--   0 root         (0) root         (0)     2112 2024-04-22 13:01:23.000000 minium-1.5.4/minium/utils/js/min/hookNavigation.js
+-rw-r--r--   0 root         (0) root         (0)      221 2024-04-22 13:01:22.000000 minium-1.5.4/minium/utils/js/min/hookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      230 2024-04-22 13:01:18.000000 minium-1.5.4/minium/utils/js/min/hookWxMethodWithId.js
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-22 13:01:15.000000 minium-1.5.4/minium/utils/js/min/ideHandleAuthModal.js
+-rw-r--r--   0 root         (0) root         (0)      210 2024-04-22 13:01:14.000000 minium-1.5.4/minium/utils/js/min/ideHandleMap.js
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-22 13:01:23.000000 minium-1.5.4/minium/utils/js/min/ideHandleModal.js
+-rw-r--r--   0 root         (0) root         (0)      476 2024-04-22 13:01:13.000000 minium-1.5.4/minium/utils/js/min/ideMockAuth.js
+-rw-r--r--   0 root         (0) root         (0)      156 2024-04-22 13:01:17.000000 minium-1.5.4/minium/utils/js/min/ideMockAuthSetting.js
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-22 13:01:16.000000 minium-1.5.4/minium/utils/js/min/ideMockChooseLocation.js
+-rw-r--r--   0 root         (0) root         (0)     1212 2024-04-22 13:01:20.000000 minium-1.5.4/minium/utils/js/min/ideMockGetLocation.js
+-rw-r--r--   0 root         (0) root         (0)      430 2024-04-22 13:01:24.000000 minium-1.5.4/minium/utils/js/min/ideMockGetUserProfile.js
+-rw-r--r--   0 root         (0) root         (0)      705 2024-04-22 13:01:14.000000 minium-1.5.4/minium/utils/js/min/ideMockGetWeRunData.js
+-rw-r--r--   0 root         (0) root         (0)     1457 2024-04-22 13:01:16.000000 minium-1.5.4/minium/utils/js/min/ideMockModal.js
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-22 13:01:19.000000 minium-1.5.4/minium/utils/js/min/ideMockShowActionSheet.js
+-rw-r--r--   0 root         (0) root         (0)      419 2024-04-22 13:01:13.000000 minium-1.5.4/minium/utils/js/min/ideMockShowModal.js
+-rw-r--r--   0 root         (0) root         (0)      496 2024-04-22 13:01:17.000000 minium-1.5.4/minium/utils/js/min/ideMockSubscribeMessage.js
+-rw-r--r--   0 root         (0) root         (0)      262 2024-04-22 13:01:25.000000 minium-1.5.4/minium/utils/js/min/initMockWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     4032 2024-04-22 13:01:15.000000 minium-1.5.4/minium/utils/js/min/mockChooseImage.js
+-rw-r--r--   0 root         (0) root         (0)      778 2024-04-22 13:01:22.000000 minium-1.5.4/minium/utils/js/min/mockCloudCall.js
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-04-22 13:01:15.000000 minium-1.5.4/minium/utils/js/min/mockNetwork.js
+-rw-r--r--   0 root         (0) root         (0)      182 2024-04-22 13:01:16.000000 minium-1.5.4/minium/utils/js/min/mockWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)     1350 2024-04-22 13:01:13.000000 minium-1.5.4/minium/utils/js/min/networkPannel.js
+-rw-r--r--   0 root         (0) root         (0)      304 2024-04-22 13:01:18.000000 minium-1.5.4/minium/utils/js/min/releaseHookWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      895 2024-04-22 13:01:19.000000 minium-1.5.4/minium/utils/js/min/requestStack.js
+-rw-r--r--   0 root         (0) root         (0)       85 2024-04-22 13:01:21.000000 minium-1.5.4/minium/utils/js/min/restoreWxMethod.js
+-rw-r--r--   0 root         (0) root         (0)      294 2024-04-22 13:01:21.000000 minium-1.5.4/minium/utils/js/min/startGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)      209 2024-04-22 13:01:19.000000 minium-1.5.4/minium/utils/js/min/stopGetPerformance.js
+-rw-r--r--   0 root         (0) root         (0)       94 2024-04-22 13:01:27.000000 minium-1.5.4/minium/utils/js/min/testAsync.js
+-rw-r--r--   0 root         (0) root         (0)     2351 2024-04-22 13:01:20.000000 minium-1.5.4/minium/utils/js/min/utils.js
+-rw-r--r--   0 root         (0) root         (0)      304 2024-04-22 13:01:26.000000 minium-1.5.4/minium/utils/js/min/uuid.js
+-rw-r--r--   0 root         (0) root         (0)       69 2024-04-22 13:01:22.000000 minium-1.5.4/minium/utils/js/min/waitUtil.js
+-rw-r--r--   0 root         (0) root         (0)     5671 2024-04-15 09:01:56.000000 minium-1.5.4/minium/utils/lazyloader.py
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-04-27 02:49:44.000000 minium-1.5.4/minium/utils/meta.py
+-rw-r--r--   0 root         (0) root         (0)      162 2022-06-30 06:29:28.000000 minium-1.5.4/minium/utils/platforms.py
+-rw-r--r--   0 root         (0) root         (0)    18433 2024-04-22 13:00:37.000000 minium-1.5.4/minium/utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 13:01:37.733286 minium-1.5.4/minium.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      699 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    13064 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      168 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-22 13:01:35.000000 minium-1.5.4/minium.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-04-22 13:00:37.000000 minium-1.5.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-22 13:01:37.765286 minium-1.5.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3151 2024-04-15 09:01:56.000000 minium-1.5.4/setup.py
```

### Comparing `minium-1.5.3/minium/__init__.py` & `minium-1.5.4/minium/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/android_base/__init__.py` & `minium-1.5.4/minium/externlib/android_base/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/__init__.py` & `minium-1.5.4/minium/externlib/at/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/apkapi.py` & `minium-1.5.4/minium/externlib/at/apkapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/atproxy.py` & `minium-1.5.4/minium/externlib/at/atproxy.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/bin/AtServer.apk` & `minium-1.5.4/minium/externlib/at/bin/AtServer.apk`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/bin/AtStub.jar` & `minium-1.5.4/minium/externlib/at/bin/AtStub.jar`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/command_line.py` & `minium-1.5.4/minium/externlib/at/command_line.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/accesshelper.py` & `minium-1.5.4/minium/externlib/at/core/accesshelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/adbwrap.py` & `minium-1.5.4/minium/externlib/at/core/adbwrap.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/basedriver.py` & `minium-1.5.4/minium/externlib/at/core/basedriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/case_repair_adapter.py` & `minium-1.5.4/minium/externlib/at/core/case_repair_adapter.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/config.py` & `minium-1.5.4/minium/externlib/at/core/config.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/element.py` & `minium-1.5.4/minium/externlib/at/core/element.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/exceptions.py` & `minium-1.5.4/minium/externlib/at/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/javadriver.py` & `minium-1.5.4/minium/externlib/at/core/javadriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/resguard.py` & `minium-1.5.4/minium/externlib/at/core/resguard.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/stf/mincap.py` & `minium-1.5.4/minium/externlib/at/core/stf/mincap.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/stf/minitouch.py` & `minium-1.5.4/minium/externlib/at/core/stf/minitouch.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/uidevice.py` & `minium-1.5.4/minium/externlib/at/core/uidevice.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/uixml.py` & `minium-1.5.4/minium/externlib/at/core/uixml.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/core/websocketcli.py` & `minium-1.5.4/minium/externlib/at/core/websocketcli.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/eventmonitor.py` & `minium-1.5.4/minium/externlib/at/eventmonitor.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/hook.py` & `minium-1.5.4/minium/externlib/at/hook.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/jlogcat.py` & `minium-1.5.4/minium/externlib/at/jlogcat.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/keycode.py` & `minium-1.5.4/minium/externlib/at/keycode.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/perfcollector.py` & `minium-1.5.4/minium/externlib/at/perfcollector.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/AtEvent.py` & `minium-1.5.4/minium/externlib/at/tests/AtEvent.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/atdevicetest.py` & `minium-1.5.4/minium/externlib/at/tests/atdevicetest.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/drivertest.py` & `minium-1.5.4/minium/externlib/at/tests/drivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/elementtest.py` & `minium-1.5.4/minium/externlib/at/tests/elementtest.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/images/1.jpg` & `minium-1.5.4/minium/externlib/at/tests/images/1.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/images/2.jpg` & `minium-1.5.4/minium/externlib/at/tests/images/2.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/images/image.jpg` & `minium-1.5.4/minium/externlib/at/tests/images/image.jpg`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/minitouch_test.py` & `minium-1.5.4/minium/externlib/at/tests/minitouch_test.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/u2test.py` & `minium-1.5.4/minium/externlib/at/tests/u2test.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/uixmltest.py` & `minium-1.5.4/minium/externlib/at/tests/uixmltest.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/tests/webdrivertest.py` & `minium-1.5.4/minium/externlib/at/tests/webdrivertest.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/apkinfo.py` & `minium-1.5.4/minium/externlib/at/utils/apkinfo.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/axmlparser.py` & `minium-1.5.4/minium/externlib/at/utils/axmlparser.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/axmlparser3.py` & `minium-1.5.4/minium/externlib/at/utils/axmlparser3.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/commonhelper.py` & `minium-1.5.4/minium/externlib/at/utils/commonhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/decorator.py` & `minium-1.5.4/minium/externlib/at/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/nbsp.py` & `minium-1.5.4/minium/externlib/at/utils/nbsp.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/utils/threadhelper.py` & `minium-1.5.4/minium/externlib/at/utils/threadhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/driver.py` & `minium-1.5.4/minium/externlib/at/webdriver/driver.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/jsapi.py` & `minium-1.5.4/minium/externlib/at/webdriver/jsapi.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/miniapp.py` & `minium-1.5.4/minium/externlib/at/webdriver/miniapp.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/stub.js` & `minium-1.5.4/minium/externlib/at/webdriver/stub.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/tabdescription.py` & `minium-1.5.4/minium/externlib/at/webdriver/tabdescription.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/tabwebsocket.py` & `minium-1.5.4/minium/externlib/at/webdriver/tabwebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/webelement.py` & `minium-1.5.4/minium/externlib/at/webdriver/webelement.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/webhelper.py` & `minium-1.5.4/minium/externlib/at/webdriver/webhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/webdriver/wspools.py` & `minium-1.5.4/minium/externlib/at/webdriver/wspools.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/at/wechat/activtiy.py` & `minium-1.5.4/minium/externlib/at/wechat/activtiy.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/bin/wat` & `minium-1.5.4/minium/externlib/bin/wat`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/case_repair_sdk/__init__.py` & `minium-1.5.4/minium/externlib/case_repair_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/case_repair_sdk/default_trace.py` & `minium-1.5.4/minium/externlib/case_repair_sdk/default_trace.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wda/__init__.py` & `minium-1.5.4/minium/externlib/wda/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -927,16 +927,21 @@
                 redata = self.http.post("/element", data)
 
         elems = []
         if not redata:
             return elems
         response = redata.value
         for elem in response:
-            if self._class_name and elem.get("type") != self._class_name:
-                continue
+            if self._class_name:
+                if "type" not in elem:
+                    class_name = self._property("name", eid=elem["ELEMENT"])
+                else:
+                    class_name = elem.get("type")
+                if class_name != self._class_name:
+                    continue
             if self.session.http.isWda and self._label and elem.get("label") != self._label:
                 continue
             elems.append(elem)
         return elems
 
     def subelems(self, timeout=None, **kwargs):
         # element = self.wait(timeout)
@@ -1351,11 +1356,16 @@
             redata = self.http.post("element/%s/elements" % eid, data)
 
         elems = []
         if not redata:
             return elems
         response = redata.value
         for elem in response:
-            if self._class_name and elem.get("type") != self._class_name:
-                continue
+            if self._class_name:
+                if "type" not in elem:
+                    class_name = self._property("name", eid=elem["ELEMENT"])
+                else:
+                    class_name = elem.get("type")
+                if class_name != self._class_name:
+                    continue
             elems.append(elem)
         return elems
```

### Comparing `minium-1.5.3/minium/externlib/wda/screenhelper.py` & `minium-1.5.4/minium/externlib/wda/screenhelper.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wda/xcui_element_types.py` & `minium-1.5.4/minium/externlib/wda/xcui_element_types.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/__init__.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/basemp.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/basemp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-07-11 15:35:44
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-07-20 21:36:44
+LastEditTime: 2023-12-11 17:30:11
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/miniprogram.py
 Description: 开放平台基础实例
 '''
 import re
 import requests
 import time
 import json
 from .logger import logger
 from .title import *
 from .utils import pick_unuse_port, Object
 from .mpdriver import *
 from .exception import *
+from typing import List, Tuple
 
 class Tab(Object):
     @property
     def description(self):
         return self["description"]
 
     @description.setter
@@ -68,20 +69,22 @@
         :param at.At at_instance: at实例
         """
         self.at = at_instance
         self.config = config
         self.logger = logger
         self.logger.setLevel(self.config.logger_level)
 
-    def _get_current_active_process(self, reg_exp):
+    def _get_current_active_process(self, reg_exp, top_m=15):
         """
         grep top 5 process, and return process match {reg_exp}
         :return: process_name, pid
+
+        top m[10], n[2] times, per d[2] seconds
         """
-        output = self.at.adb.run_shell(f'COLUMNS=512 top -m 10 -n 2 -d 2|grep -e "{reg_exp}"')
+        output = self.at.adb.run_shell(f'COLUMNS=512 top -m {top_m} -n 2 -d 2|grep -e "{reg_exp}"')
         self.logger.debug(output)
         lines = [re.sub(r"\x1B[^m]*m", "", line.strip()) for line in output.strip().split("\n")]  # Filter control character
         result = []
         for output2 in lines:
             r = re.compile("(%s)" % reg_exp)
             m = r.search(output2)
             if m:
@@ -92,40 +95,45 @@
             return result
         # 没有match的, 退化成非grep的形式看看
         return [self.at.adb.get_current_active_process(reg_exp)]
 
     def _get_current_appbrand(self):
         """获取当前小程序进程名和进程id
 
-        :return str, int: processname, pid
+        :return str, int: List[(processname, pid)]
         """
-        result = [[r[0], str(r[1]).strip()] for r in self._get_current_active_process(
-            re.escape("com.tencent.mm:appbrand") + "\d*"
-        )]
-        if len(result) != 1:
+        for top_m in (15, 20):  # 如果top15找不到尝试使用top20
+            result: List[Tuple[str, str]] = [(r[0], str(r[1]).strip()) for r in self._get_current_active_process(
+                re.escape("com.tencent.mm:appbrand") + "\d*", top_m=top_m
+            )]
             tmp = {}
             for r in result:
                 processname, processpid = r
+                if not processpid or processpid == "None":
+                    continue
                 if processpid not in tmp:
                     tmp[processpid] = r
                     self.logger.debug(
                         f"current appbrand processname[{processname}], id[{processpid}]"
                     )
-            return list(tmp.values())
-        return result
+            result = list(tmp.values())
+            if result:
+                return result
+        return [(None, None),]
 
     def _get_current_mm(self):
         """获取当前小程序进程名和进程id
 
         :return str, int: processname, pid
         """
-        result = self._get_current_active_process(r"com\.tencent\.mm.*")
-        for pname, pid in result:
-            if pname == "com.tencent.mm":
-                return pname, pid
+        for top_m in (15, 20):  # 如果top15找不到尝试使用top20
+            result = self._get_current_active_process(r"com\.tencent\.mm.*", top_m=top_m)
+            for pname, pid in result:
+                if pname == "com.tencent.mm":
+                    return pname, pid
         return None, None
 
     def _get_debug_sock_name(self, pid=None):
         """获取socket映射名
 
         :return dict[str, str]: {sock_name: pid}
         """
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/basewebsocket.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/basewebsocket.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/cdpdriver.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/cdpdriver.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/command.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/command.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/baseconn.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/baseconn.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-11 17:08:57
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 10:53:21
+LastEditTime: 2024-02-28 17:39:11
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/session/basesession.py
 Description: 类websocket的会话实现, 支持发送消息以及监听回调
 '''
 import abc
-from typing import Tuple, Dict, Any, List, Callable
+from typing import Tuple, Dict, Any, List, Callable, Union
 import time
 from enum import Enum
 import threading
 from ..logger import logger
 from ..emitter import MyEventEmitter
-from ..utils import json2obj, Object, ProcessSafeEventLoop, AsyncCondition, AsyncCallback
+from ..utils import json2obj, Object, ProcessSafeEventLoop, ThreadSafeEventLoop, AsyncCondition, AsyncCallback, catch
 from ..command import CommandType, Command, AsyncCommand
 from ..event import BaseEvent
 from asyncio.coroutines import iscoroutine
 import asyncio
 import json
 
 class AbstractConnection(metaclass=abc.ABCMeta):
     @abc.abstractmethod
-    def send_command(self, data: dict or CommandType): pass
+    def send_command(self, data: Union[dict, CommandType]): pass
 
     @abc.abstractmethod
-    def on(self, event: str or BaseEvent, callback: Callable): pass
+    def on(self, event: Union[str, BaseEvent], callback: Callable): pass
 
 
 class BaseConnection(AbstractConnection):
     """
     子类通过
     1. 调用`_on_message`实现回包消息处理
     2. 调用`send`和`send_async`实现同步和异步命令发送
@@ -39,24 +39,29 @@
     def __init__(self, loop: asyncio.AbstractEventLoop=None) -> None:
         self._id = str(id(self))
         self.logger = logger.getChild(f"Conn{self._id[-4:]}")
 
         self._ee = MyEventEmitter()
         self._msg_lock = threading.Condition()  # 信息锁
         self._sync_wait_map = {}  # 同步消息kv表, id -> result
-        self._async_msg_map: Dict[str or int, AsyncCommand] = {}  # 异步命令kv表, id -> AsyncCommand
+        self._async_msg_map: Dict[Union[str, int], AsyncCommand] = {}  # 异步命令kv表, id -> AsyncCommand
         self._method_wait_map = {}  # 等待命令kv表, method -> result
         self._observers: Dict[str, List[Callable]] = {}  # 监听表, method -> handler(callback function)
         # event loop 用来处理on message回调中的异步函数
-        if loop:
-            self._event_loop = ProcessSafeEventLoop(loop)
-        else:
-            self._event_loop = ProcessSafeEventLoop()
+        self._event_loop = ThreadSafeEventLoop()
+        # self.logger.info("self._event_loop %d" % id(self._event_loop))
+        # if loop:
+        #     self._event_loop = ThreadSafeEventLoop(loop)
+        # else:
+        #     self._event_loop = ThreadSafeEventLoop()
             # events._set_running_loop(self._event_loop.loop)
 
+    @property
+    def id(self):
+        return self._id
         
     def _on_message(self, message):
         """接收json like会包信息, 尽量不要有阻塞操作"""
         self.logger.debug("RECV < %.510s" % message)
         ret_json = json2obj(message)
         if not ret_json:
             return
@@ -94,14 +99,15 @@
                 self._async_msg_map.pop(cmd.id)
             del cmd
             raise
         return cmd.id
 
     def create_async_callback_task(self, callback, *args):
         # self.logger.warn("create_async_callback_task: %s" % callback.__name__)
+        # self.logger.warning("loop running %s" % self._event_loop.is_running())
         async def _callback(*_args):
             # self.logger.warn("@async call %s" % callback.__name__)
             ret = callback(*_args)
             if iscoroutine(ret):
                 return await ret
             return ret
         if isinstance(callback, AsyncCallback):
@@ -133,15 +139,15 @@
         etime = time.time()
         if etime - stime >= cmd.max_timeout:
             cmd.max_timeout = 0
         else:
             cmd.max_timeout = cmd.max_timeout - (etime - stime)  # 剩余要等待的时间
         return ret
 
-    
+    @abc.abstractmethod
     def _check_conn_exception(self, cmd: Command):
         """检查链接异常状态, 决定命令是否继续[等待]
 
         :param Command cmd: 指令
         """
         pass
     
@@ -220,15 +226,15 @@
 
     def handle_message(self, ret_json) -> Tuple[str, Any]:
         req_id, result = self._handle_response(ret_json)
         if not req_id:
             result = self._handle_event(ret_json)
         return req_id, result
 
-    def on(self, event: str or BaseEvent, callback: Callable or AsyncCallback):
+    def on(self, event: Union[str, BaseEvent], callback: Union[Callable, AsyncCallback]):
         """监听事件
 
         :param str event: 事件名
         :param function callback: 回调函数
         """
         if not callable(callback) and not isinstance(callback, AsyncCallback):
             raise TypeError(
@@ -264,61 +270,176 @@
             raise KeyError(e)
 
     def send_command(self, cmd: CommandType, **extend):
         if isinstance(cmd, Command):
             return self.send(cmd, **extend)
         return self.send_async(cmd, **extend)
 
-    @abc.abstractclassmethod
+    @abc.abstractmethod
     def _safely_send(self, cmd: CommandType, **extend):
         """真实发送消息的方法"""
         pass
 
     @abc.abstractmethod
     def _handle_response(self, ret_json) -> Tuple[str, Any]: ...
 
     @abc.abstractmethod
     def _handle_event(self, ret_json) -> BaseEvent: ...
 
 class BaseAsyncConnection(BaseConnection):
+    """
+    子类通过
+    1. 调用`_on_message`实现回包消息处理
+    2. 调用`send`和`send_async`实现同步和异步命令发送
+    3. 可调用`_send`和`_send_async`实现同步和异步命令发送(send和send_async的async版本)
+    
+    4. `on`可监听事件
+
+    PS: `_async`开头的函数为`_`开头函数的async版本, `_`开头函数为一般函数的async版本
+    """
     def __init__(self, loop: asyncio.AbstractEventLoop = None) -> None:
         super().__init__(loop)
-        self._async_msg_lock = AsyncCondition()
+        self._async_msg_lock = AsyncCondition(loop=loop or self._event_loop)
 
     # connection中有在主线程使用了async接口的情况下, send_command不能有非async阻塞操作
     # _receive_response中等待和通知接口需要进行异步重构
 
     @abc.abstractmethod
+    async def _async_check_conn_exception(self, cmd):
+        raise NotImplementedError("AsyncConnection need implement async function _async_check_conn_exception")
+
+    async def _async_receive_response(self, cmd: Command):
+        # 等待接收到message的通知
+        while cmd.max_timeout > 0:
+            if (
+                cmd.id in self._sync_wait_map
+                and self._sync_wait_map[cmd.id] is not None
+            ):  # 不等待就获取到数据了, 这个recv太快了吧
+                self.logger.info("🚀🚀🚀🚀🚀🚀🚀火速获取到返回导致处理不过来🚀🚀🚀🚀🚀🚀🚀")
+                response = self._sync_wait_map.pop(cmd.id)
+                if isinstance(response, Exception):
+                    raise response
+                return response
+            await self._async_wait(cmd)
+
+            if (
+                cmd.id in self._sync_wait_map
+                and self._sync_wait_map[cmd.id] is not None
+            ):  # 获取到了数据
+                response = self._sync_wait_map.pop(cmd.id)
+                if isinstance(response, Exception):
+                    raise response
+                return response
+            try:
+                await self._async_check_conn_exception(cmd)
+            except:
+                if cmd.id in self._sync_wait_map:
+                    del self._sync_wait_map[cmd.id]
+                raise
+            if cmd.max_timeout > 0:  # 线程是被其他消息唤醒，重新等待
+                self.logger.debug("rewait for %s" % cmd.id)
+                continue
+            else:
+                if cmd.id in self._sync_wait_map:
+                    del self._sync_wait_map[cmd.id]
+                # test_link(self._url)  # 出现超时的情况, 尝试另外建立链接看看是不是inspector问题
+                if cmd.reason and isinstance(cmd.reason, ConnectionAbortedError):
+                    raise TimeoutError(
+                        f"[{cmd.id}][{cmd.desc}] command timeout cause by {cmd.reason}"
+                    )
+                raise TimeoutError(
+                    f"[{cmd.id}][{cmd.desc}] receive from remote timeout"
+                )
+
+    @abc.abstractclassmethod
+    async def _async_safely_send(self, cmd: CommandType, **extend):
+        """_safely_send 的 async 版本"""
+        pass
+
+    @abc.abstractmethod
     def await_(self, awaitable): ...
 
     def _wait(self, cmd: Command):
         """重构试用异步等待"""
         return self.await_(self._async_wait(cmd))
 
     def _notify(self):
         """重构使用异步通知"""
+        # try:
+        #     self.logger.info("start _notify")
+        #     return self.await_(self._async_notify())
+        # finally:
+        #     self.logger.info("end _notify")
+        return self.await_(self._async_notify())
         return self._event_loop.run_coroutine(self._async_notify())
     
     async def _async_wait(self, cmd: Command):
         stime = time.time()
         await self._async_msg_lock.acquire()
+        await self._async_msg_lock.wait(0)
+        # self.logger.debug(self._async_msg_lock._loop)
+        # self.logger.debug(catch(asyncio.get_running_loop)())
+        # self.logger.debug("start wait%d, %d" % (id(self._async_msg_lock._loop), id(catch(asyncio.get_running_loop)())))
+        # await self._async_msg_lock.wait(0)
+        # self.logger.info(f"wait loop {id(self._async_msg_lock._loop)}")
         ret = await self._async_msg_lock.wait(timeout=cmd.max_timeout)
+        # self.logger.info(f"after wait loop {id(self._async_msg_lock._loop)}, ret: {ret}")
         self._async_msg_lock.release()
         etime = time.time()
         if etime - stime >= cmd.max_timeout:
             cmd.max_timeout = 0
         else:
             cmd.max_timeout = cmd.max_timeout - (etime - stime)  # 剩余要等待的时间
         return ret
     
     async def _async_notify(self):
+        # self.logger.info("🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀 _async_notify loop %d", id(catch(asyncio.get_running_loop)()))
         await self._async_msg_lock.acquire()
+        # self.logger.debug(self._async_msg_lock._loop)
+        # self.logger.debug(catch(asyncio.get_running_loop)())
+        # self.logger.debug("%d, %d" % (id(self._async_msg_lock._loop), id(catch(asyncio.get_running_loop)())))
+        # self.logger.info(f" start notify loop {id(self._async_msg_lock._loop)}, {len(self._async_msg_lock._waiters)}")
         self._async_msg_lock.notify_all()
+        # await asyncio.sleep(0)
+        # self.logger.info(f"notify loop {id(self._async_msg_lock._loop)}, {len(self._async_msg_lock._waiters)}")
         self._async_msg_lock.release()
+        # self.logger.info("🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀 end _async_notify loop")
+
+    def get_aysnc_msg_return(self, msg_id=None, timeout=Command.max_timeout):
+        return self._event_loop.run_coroutine(self._get_aysnc_msg_return(msg_id, timeout)).result()
 
+    # ⬇️⬇️⬇️ 对外/继承重写需要使用到的 async 接口
+    async def _send_command(self, cmd: CommandType, **extend):
+        if isinstance(cmd, Command):
+            return await self._send(cmd, **extend)
+        return await self._send_async(cmd, **extend)
+
+    async def _send(self, cmd: Command, **extend):
+        # send 的 async 版本
+        # 同步发送消息，函数会阻塞
+        with cmd:
+            self._sync_wait_map[cmd.id] = None  # 该ID未有返回message
+            await self._async_safely_send(cmd, **extend)
+            return await self._async_receive_response(cmd)
+
+    async def _send_async(
+        self, cmd: AsyncCommand, ignore_response=False, **extend
+    ) -> str:
+        # send_async 的 async 版本
+        if not ignore_response:
+            self._async_msg_map[cmd.id] = cmd
+        try:
+            await self._async_safely_send(cmd, **extend)
+        except ConnectionAbortedError:
+            if not ignore_response:
+                self._async_msg_map.pop(cmd.id)
+            del cmd
+            raise
+        return cmd.id
+    
     async def _get_aysnc_msg_return(self, msg_id=None, timeout=Command.max_timeout):
         """等待异步消息返回
 
         :param str msg_id: 消息id, defaults to None
         :param int timeout: 最长等待时间, defaults to Command.max_timeout
         :raises response: 消息错误
         :return any: 消息结果
@@ -343,16 +464,15 @@
                             self._async_msg_map.pop(msg_id)
                         break
             if isinstance(response, Exception):
                 raise response
             return response
         return None
 
-    def get_aysnc_msg_return(self, msg_id=None, timeout=Command.max_timeout):
-        return self._event_loop.run_coroutine(self._get_aysnc_msg_return(msg_id, timeout)).result()
+    # ⬆️⬆️⬆️ async 接口
 
 class STATE(Enum):
     CLOSE = 1  # 链接关闭
     OPEN = 2  # 链接连通
     PEDING = 3  # 链接连接中
     RECONNECTING = 4  # 重新链接中
     INIT = 5
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/lockdownconn.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/lockdownconn.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-22 16:06:05
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-16 16:48:08
+LastEditTime: 2024-02-28 17:46:49
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/connection/lockdownconn.py
 Description: 定义通过lockdown连接的webinspector链接
 '''
-from typing import Mapping, Tuple, Any, Dict
+from typing import Mapping, Tuple, Any, Dict, Union
 import json
 import time
+import asyncio
 from dataclasses import dataclass
 from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 from pymobiledevice3.services.webinspector import WebinspectorService
 
 from wechat_mp_inspector.command import Command, CommandType, AsyncCommand
 from ..command import CommandType, Command, BaseCommand
 from .baseconn import BaseAsyncConnection, BaseEvent, STATE
 from ..pages.safaripage import BasePage, Page
-from ..utils import json2obj, Object, cost_debug, AsyncCondition
+from ..utils import json2obj, Object, cost_debug, AsyncCondition, ThreadSafeEventLoop, catch
 from ..event import BaseEvent
 from ..logger import logger
 
 
 OPEN_TIMEOUT = 30  # 链接超时时间
 
 
@@ -29,16 +30,18 @@
 class SocketCommandExtend:
     session_id: str
     app_id: str
     page_id: str
 
 
 class LockdownConnection(WebinspectorService, BaseAsyncConnection):
+    application_pages: Dict[str, Dict[str, Page]]
     INSTANCES: Dict[str, 'LockdownConnection'] = {}  # 控制生成单实例
     _state = STATE.CLOSE  # 默认链接状态close
+    loop = None
     
     _unique_id = None
 
     def __new__(
         cls, lockdown: LockdownServiceProvider, loop=None, timeout=None
     ):
         unique_id = lockdown.udid
@@ -48,24 +51,32 @@
             if inst._state != STATE.CLOSE:
                 return inst  # 使用旧的实例
             # 缓存的实例没有链接
             inst.destroy()
             INSTANCES[unique_id] = inst  # 不改变实例, 直接重新init
             return inst
         inst = object.__new__(cls)
+        # 创建唯一实例唯一一个循环
+        # if loop is None:
+        #     loop = ThreadSafeEventLoop(loop)
+        inst.loop = loop
         inst._unique_id = unique_id
         INSTANCES[unique_id] = inst
         return inst
 
     def __init__(self, lockdown: LockdownServiceProvider, loop=None, timeout=None):
         if self._state != STATE.CLOSE:  # 有已经链接的实例
             return
-        BaseAsyncConnection.__init__(self, loop=loop)
-        # ❕❕❕WebinspectorService中的异步调用基本为call_soon, 不能跨线程调用
-        WebinspectorService.__init__(self, lockdown, loop)
+        super().__init__(lockdown, self.loop)
+        super(WebinspectorService, self).__init__(loop=loop or self.loop)
+        # BaseAsyncConnection.__init__(self, loop=loop)
+        # # ❕❕❕WebinspectorService中的异步调用基本为call_soon, 不能跨线程调用
+        # WebinspectorService.__init__(self, lockdown, loop)
+        # self.logger.info(f"current connection_id: {self.connection_id}")
+        # self.logger.info(f"connection loop: {id(self.loop)} type: {self.loop.__class__.__name__}")
         self.connect(timeout or OPEN_TIMEOUT)
         self._state = STATE.OPEN
         while not self.connected_application:
             # 等待连接到webinspectord服务等app, 证明服务已经注册好
             self.flush_input()
         self._is_close_on_my_own = False  # 链接是自己主动断开的, 主要标记是否进行链接重连
 
@@ -75,32 +86,65 @@
             self.__class__.INSTANCES.pop(self._unique_id)
         if self._is_close_on_my_own:
             self.logger.debug("already destroy")
             return
         self._is_close_on_my_own = True
         self.close()
 
+    def _ensure_future(self, coro):
+        return asyncio.ensure_future(coro, loop=self.loop)
+
     # ⬇️⬇️⬇️ 以下是重构方法
+    async def _send_message(self, selector: str, args=None):
+        if args is None:
+            args = {}
+        if not args.get('WIRConnectionIdentifierKey', None):
+            args['WIRConnectionIdentifierKey'] = self.connection_id
+        await self.service.aio_send_plist({'__selector': selector, '__argument': args})
+
     async def _forward_indicate_web_view(self, app_id: str, page_id: int, enable: bool):
         # 纯fix
+        self.logger.debug(f'_forward_indicate_web_view')
         await self._send_message('_rpc_forwardIndicateWebView:', {
             'WIRApplicationIdentifierKey': app_id,
             'WIRPageIdentifierKey': page_id,
             'WIRIndicateEnabledKey': enable,
         })
 
-    async def _forward_socket_data(self, session_id: str, app_id: str, page_id: int, data: Mapping or str):
+    async def _forward_socket_data(self, session_id: str, app_id: str, page_id: int, data: Union[Mapping, str]):
         _data = data.encode() if isinstance(data, str) else json.dumps(data).encode()
         await self._send_message('_rpc_forwardSocketData:', {
             'WIRApplicationIdentifierKey': app_id,
             'WIRPageIdentifierKey': page_id,
             'WIRSessionIdentifierKey': session_id,
             'WIRSocketDataKey': _data,
         })
 
+    async def _forward_web_page_close(self, app_id: str, page_id: int, connection_id: str=None):
+        self.logger.debug(f'_forward_web_page_close: {connection_id}')
+        message = {
+            'WIRApplicationIdentifierKey': app_id,
+            'WIRPageIdentifierKey': page_id,
+            'WIRConnectionIdentifierKey': connection_id or self.connection_id  # close other or self connection
+        }
+        await self._send_message('_rpc_forwardWebPageClose:', message)
+
+    async def _forward_connection_died(self, connection_id: str, app_id: str, page_id: int):
+        self.logger.debug(f'_forward_connection_died: {connection_id}')
+        message = {
+            'WIRApplicationIdentifierKey': app_id,
+            'WIRPageIdentifierKey': page_id,
+            'WIRConnectionIdentifierKey': connection_id
+        }
+        await self._send_message('_rpc_forwardConnectionDied:', message)
+
+    async def _forward_socket_setup(self, session_id: str, app_id: str, page_id: int, pause: bool = False):
+        self.logger.debug(f'_forward_socket_setup [a]{app_id}.[p]{page_id}.[s]{session_id}')
+        return await super()._forward_socket_setup(session_id, app_id, page_id, pause)
+
     def _handle_application_sent_listing(self, arg):
         """重构该方法生产新的page实例"""
         appid_ = arg['WIRApplicationIdentifierKey']
         if appid_ in self.application_pages:
             for id_, page in arg['WIRListingKey'].items():
                 page["appid_"] = appid_
                 if id_ in self.application_pages[appid_]:
@@ -123,25 +167,47 @@
             raise ConnectionAbortedError("close by myself")
         elif self._state == STATE.CLOSE:
             if cmd.id in self._sync_wait_map:
                 del self._sync_wait_map[cmd.id]
             if cmd.reason:
                 raise cmd.reason
             raise ConnectionAbortedError("connection closed")
+        
+    async def _async_check_conn_exception(self, cmd: Command):
+        return self._check_conn_exception(cmd)
+
+    def _forward_get_listing(self, app_id):
+        return self._ensure_future(super()._forward_get_listing(app_id))
+
+    # def await_(self, awaitable):
+    #     return super().await_(awaitable)
 
     # ⬆️⬆️⬆️ 以上是重构方法
     
     # lockdown connection使用了异步接口, send_command不能有非async阻塞操作
     # _receive_response中等待和通知接口需要进行异步重构
 
     def _safely_send(self, cmd: CommandType, **extend):
         kwargs = {}
         for i in ("session_id", "app_id", "page_id"):
             if i not in extend:
                 raise RuntimeError(f"socket command miss {i}")
             else:
                 kwargs[i] = extend[i]
         kwargs["data"] = cmd.dumps()
-        self.logger.debug("SEND > %.510s" % json.dumps(kwargs))
+        self.logger.debug("%s > %.510s" % ("ASEND" if isinstance(cmd, AsyncCommand) else "SEND", json.dumps(kwargs)))
         return self.await_(self.send_socket_data(**kwargs))
     
+    async def _async_safely_send(self, cmd: CommandType, **extend):
+        # self.logger.debug("🚀🚀🚀🚀🚀🚀🚀🚀🚀🚀 _async_safely_send loop %d", id(catch(asyncio.get_running_loop)()))
+        kwargs = {}
+        for i in ("session_id", "app_id", "page_id"):
+            if i not in extend:
+                raise RuntimeError(f"socket command miss {i}")
+            else:
+                kwargs[i] = extend[i]
+        kwargs["data"] = cmd.dumps()
+        self.logger.debug("%s > %.510s" % ( "SEND" if isinstance(cmd, Command) else "ASEND" ,json.dumps(kwargs)))
+        return await self.send_socket_data(**kwargs)
+
+
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/connection/websocketconn.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/connection/websocketconn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-11 17:41:41
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 11:29:42
+LastEditTime: 2024-02-28 17:29:26
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/session/wssession.py
 Description: 基于websocket链接的session
 '''
 from .baseconn import AbstractConnection, STATE, BaseConnection
 import websocket
 from websocket import WebSocketBadStatusException
 from ..utils import *
 from ..emitter import ee
 from ..command import *
 from ..event import *
 from asyncio.coroutines import iscoroutine
 from enum import Enum
-from typing import Dict
+from typing import Dict, Union
 
 logger = logging.getLogger("WMI")
 
 MAX_WAIT_TIMEOUT = 30  # 指令默认等待回复时间
 MAX_RETRY = 2  #  重连的情况, 最大重试的次数
 OPEN_TIMEOUT = 10  # 等待ws on_open
 CLOSE_TIMEOUT = 5  # 等待ws on_close
@@ -640,15 +640,15 @@
             and not self.is_connected
             and not self.is_close_by_myself
         ):
             raise ConnectionAbortedError(
                 "send message[%s] fail because connection is not established" % cmd.id
             ) from self._last_reconnect_fail_reason
         
-    def send_command(self, data: dict or CommandType):
+    def send_command(self, data: Union[dict, CommandType]):
         if isinstance(data, Command):
             return self.send(data)
         if isinstance(data, AsyncCommand):
             return self.send_async(data)
         if "method" in data:
             return self._safely_send(self._gen_command(data["method"], data.get("params", None)))
         return self._send(json.dumps(data))
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/androiddriver.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/androiddriver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-21 17:27:49
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 11:07:39
+LastEditTime: 2024-03-04 14:17:20
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/androiddriver.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 
 import time
 import at
 import re
 import json
 import uuid
 import requests
-from typing import List, Dict
+from typing import List, Dict, Union, Optional, Generic, TypeVar, Type
 from .basedriver import BaseDriver
 from .config import AndroidConfig
 from ..utils import pick_unuse_port, Object, get_url_path
 from ..pages.chromepage import *
 from ..protocol.basesession import BaseSession
 from ..protocol.cdp import CDPSession, CDPConnection
 from ..inspector.androidinspector import AndroidInspector
 
+T = TypeVar("T")
 
-class AndroidDriver(BaseDriver):
+class AndroidDriver(BaseDriver, Generic[T]):
+    _cls: Type[T] = AndroidInspector
     WEB_DEBUG_PORT_REGEX_MAPPING = {
         "x5": [r"webview_devtools_remote_(?P<pid>\d+)"],
         "xweb": [
             r"com\.tencent\.mm_devtools_remote(?P<pid>\d+)",
             r"xweb_devtools_remote_(?P<pid>\d+)",
         ],
         # xweb成功伪装成系统内核
@@ -73,14 +75,49 @@
                 self.logger.debug(line)
             for reg_str in AndroidDriver.WEB_DEBUG_PORT_REGEX_LIST:
                 m = re.search(reg_str, line)
                 if m is not None and m.group() not in target_ports:
                     target_ports[m.group()] = m.group("pid")
         self.logger.debug(target_ports)
         return target_ports
+    
+    def _get_current_active_process(self, reg_exp, top_m=15):
+        """
+        grep top 5 process, and return process match {reg_exp}
+        :return: process_name, pid
+
+        top m[10], n[2] times, per d[2] seconds
+        """
+        output = self.at.adb.run_shell(f'COLUMNS=512 top -m {top_m} -n 2 -d 2|grep -e "{reg_exp}"')
+        self.logger.debug(output)
+        lines = [re.sub(r"\x1B[^m]*m", "", line.strip()) for line in output.strip().split("\n")]  # Filter control character
+        result = []
+        for output2 in lines:
+            r = re.compile("(%s)" % reg_exp)
+            m = r.search(output2)
+            if m:
+                pid = output2.split()[0]
+                m_name = m.group(1)
+                result.append((m_name, pid))
+        if result:
+            return result
+        # 没有match的, 退化成非grep的形式看看
+        return [self.at.adb.get_current_active_process(reg_exp)]
+    
+    def _get_current_mm(self):
+        """获取当前小程序进程名和进程id
+
+        :return str, int: processname, pid
+        """
+        for top_m in (15, 20):  # 如果top15找不到尝试使用top20
+            result = self._get_current_active_process(r"com\.tencent\.mm.*", top_m=top_m)
+            for pname, pid in result:
+                if pname == "com.tencent.mm":
+                    return pname, pid
+        return None, None
         
     def p_forward(self, sock_name):
         if sock_name in AndroidDriver.CACHE_PORT:
             return AndroidDriver.CACHE_PORT[sock_name]["port"]
         port = pick_unuse_port()
         cmd = "forward tcp:%d localabstract:%s" % (port, sock_name)
         AndroidDriver.CACHE_PORT[sock_name] = {
@@ -145,33 +182,34 @@
         if webSocketDebuggerUrl in self.IGNORE_ID:
             self.logger.debug("ignore %s", webSocketDebuggerUrl)
             return None
         return ChromeNormalPage(
             tab["title"], 
             tab.get("url", ""), 
             webSocketDebuggerUrl,
-            tab.get("id", None) or get_url_path(webSocketDebuggerUrl),
-            tcp_port,
+            tab.get("description"),
+            unique_id=tab.get("id", None) or get_url_path(webSocketDebuggerUrl),
+            tcp_port=tcp_port,
             sock_name=sock_name,
         )
 
-    def refresh_page(self, page: ChromeNormalPage) -> ChromeNormalPage or None:
+    def refresh_page(self, page: ChromeNormalPage) -> Optional[ChromeNormalPage]:
         """刷新page实例, 兼容逻辑, 在原port不可用时使用
 
         :param ChromeNormalPage page: page实例
         """
         sock_name = page.ext_info.sock_name
         tabs, tcp_port = self.get_tabs_by_sock(sock_name)
         self.logger.info(f"refresh debugger url, new port: {tcp_port}")
         for tab in tabs:
             _page = self._create_page_from_tab(tab, tcp_port, sock_name)
             if _page == page:
                 return _page
 
-    def get_pages(self) -> List[ChromeTab]:
+    def get_pages(self) -> List[ChromeNormalPage]:
         pages = []
         sock_dict = self._get_debug_sock_name()  # sock_name -> pid
         for sock_name, pid in sock_dict.items():
             self.logger.debug(f"find debugger port for {sock_name}")
             try:
                 tabs, tcp_port = self.get_tabs_by_sock(sock_name)
             except RuntimeError:
@@ -183,18 +221,18 @@
             for tab in tabs:
                 page = self._create_page_from_tab(tab, tcp_port, sock_name)
                 if not page:
                     continue
                 pages.append(page)
         return pages
     
-    def inspector_session(self, page: ChromeNormalPage) -> AndroidInspector:
+    def inspector_session(self, page: ChromeNormalPage) -> T:
         session_id = str(uuid.uuid4()).upper()
         connection = CDPConnection(page.webSocketDebuggerUrl, unique_id=page.unique_id)
-        return AndroidInspector(CDPSession(connection, session_id, page, self.refresh_page))
+        return self.__class__._cls(CDPSession(connection, session_id, page, self.refresh_page), page=page)
 
 
 if __name__ == "__main__":
     import requests
     import logging
     import threading
     from ..protocol.protocoltypes import *
@@ -206,15 +244,15 @@
         "connect_timeout": 5,
     })
     driver = AndroidDriver(config)
     # requests.get("http://mmtest.oa.com/weappopentest/launchtest/SendMsgTools?user_name=yopotest1-3&app_id=wx3eb9cfc5787d5458&app_type=0")
     pages = driver.get_pages()
     target_page = None
     for page in pages:
-        if isinstance(page, WebViewPage) and page.visible:
+        if isinstance(page, ChromeWebViewPage) and page.visible:
             target_page = page
             break
     if target_page is None:
         raise RuntimeError("没有符合条件的页面")
     threading.Thread(target=driver.inspector_session, args=(target_page,)).start()
     inspector = driver.inspector_session(target_page)    
     print(inspector.send_command(Runtime.evaluate(expression="""__wxConfig""", returnByValue=True)))
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/basedriver.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/basedriver.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-21 13:36:33
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-07 16:29:23
+LastEditTime: 2024-03-01 20:45:03
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/basedriver.py
 Description: 驱动基类, 定义驱动基本运转方式
 '''
 import abc
 import logging
 from typing import List
 from .config import *
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/iosdriver.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/iosdriver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-21 14:12:23
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-16 16:32:35
+LastEditTime: 2024-03-01 20:32:30
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/iosdriver.py
 Description: 这是默认设置,请设置`customMade`, 打开koroFileHeader查看配置 进行设置: https://github.com/OBKoro1/koro1FileHeader/wiki/%E9%85%8D%E7%BD%AE
 '''
 import time
 import uuid
 import asyncio
 from typing import List, Mapping
 from dataclasses import fields
 from pymobiledevice3.lockdown import create_using_usbmux
 from .config import IOSConfig
 from ..utils import get_result
 from .basedriver import BaseDriver, BaseConfig
 from ..inspector.iosinspector import IOSInspectorSession
 from ..protocol.wip import WIPSession, WIPConnection
-from ..connection.lockdownconn import Page
+from ..pages.safaripage import Page, WirTypes
 
 
-class IOSDriver(BaseDriver):
+class IOSDriver(BaseDriver[IOSInspectorSession]):
     EXTEND_BUNDLE = ['process-com.apple.WebKit.WebContent', ]
 
     def __init__(self, config: IOSConfig) -> None:
         self.config = config
         # Connecting via usbmuxd
         lockdown = create_using_usbmux(serial=self.config.udid)
         connection = WIPConnection(lockdown, timeout=self.config.connect_timeout)
@@ -62,17 +62,21 @@
             self.connection.get_open_pages()  # 刷一下页面列表
         return self.app
     
     def async_(self, coro):
         """运行异步函数"""
         return asyncio.run_coroutine_threadsafe(coro, loop=self.loop)
 
-    def await_(self, awaitable):
+    def ensure_future(self, coro):
+        return asyncio.ensure_future(coro, loop=self.loop)
+
+    def await_(self, awaitable, loop=None):
         """运行并等待异步函数"""
-        return self.loop.run_until_complete(asyncio.ensure_future(awaitable, loop=self.loop))
+        loop = loop or self.loop
+        return loop.run_until_complete(asyncio.ensure_future(awaitable, loop=loop))
 
     def setup_inspector_socket(self, session_id, app_id, page_id):
         """注册一个页面的inspector会话"""
         return self.connection.setup_inspector_socket(session_id, app_id, page_id)
 
     def wait_for_app(self, timeout):
         return self.connection.await_(self._wait_for_app(timeout))
@@ -107,14 +111,15 @@
         return await IOSInspectorSession.create(WIPSession(self.connection, session_id, page))
 
     def sleep(self, seconds):
         self.await_(asyncio.sleep(seconds))
 
 
 if __name__ == "__main__":
+    import re
     import requests
     import logging
     import threading
     from ..protocol.protocoltypes import *
     from ..utils import ProcessSafeEventLoop
     logging.basicConfig(level=logging.DEBUG)
     
@@ -128,26 +133,30 @@
     if not driver.wait_for_app(20):
         raise RuntimeError("没加载好")
     print(driver.app)
     pages = driver.get_pages()
     # 选择一个页面
     target_page = None
     for page in pages:
+        # if (page.web_title or "").find("wx3eb9cfc5787d5458") > 0 and re.search(r"ContextId\[0\]", (page.web_title or "")):
+        #     target_page = page
+        #     break
         if (page.web_title or "").find("wx3eb9cfc5787d5458") > 0 and (page.web_title or "").find("ContextId[1]") > 0 or (page.web_url or "").find("wx3eb9cfc5787d5458") > 0:
             if target_page is None:
                 target_page = page
             elif target_page.id_ < page.id_:
                 target_page = page
     if target_page is None:
         raise RuntimeError("没有符合条件的页面")
     print(f"inspect {target_page}, thread id: {threading.get_ident()}")
     inspector = driver.inspector_session(target_page)
     driver.sleep(2)
     try:
         print("cmd.id: %s" % inspector.send_command(Runtime.enable(), sync=False))
+        print("cmd.id: %s, aync" % inspector.await_(inspector._send_command(Runtime.enable(), sync=True)) )
         driver.await_(asyncio.sleep(2))
     except TimeoutError:
         driver.await_(asyncio.sleep(0))
     # threading.Thread(target=inspector.send_command, args=(Runtime.evaluate(expression="""__wxConfig""", returnByValue=True),)).start()
     # driver.await_(asyncio.sleep(10))
     print(inspector.send_command(Runtime.evaluate(expression="""__wxConfig""", returnByValue=True)))
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/driver/mpdriver.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/driver/mpdriver.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 Date: 2023-10-09 16:41:56
 LastEditors: yopofeng yopofeng@tencent.com
 LastEditTime: 2023-10-18 16:02:27
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/mpdriver.py
 Description: 小程序驱动
 """
 import uuid
+import asyncio
 from dataclasses import asdict
-from typing import Dict, List, Tuple, Iterable, TYPE_CHECKING
+from typing import Dict, List, Tuple, Iterable, TYPE_CHECKING, Callable, Union, Optional
 
 from ..lazyloader import lazy_import
 from ..pages.basepage import BasePage
 from wechat_mp_inspector.inspector.baseinspector import BaseInspector
 from .basedriver import BaseConfig, BaseDriver
 from .androiddriver import (
     AndroidDriver,
     AndroidConfig,
     AndroidInspector,
     CDPConnection,
     CDPSession,
 )
 
+from ..inspector.wxainspector import WebviewInspector, H5Inspector
+
 if TYPE_CHECKING:
     import wechat_mp_inspector.driver.iosdriver as iosdriver
     import wechat_mp_inspector.pages.safaripage as safaripage
     import wechat_mp_inspector.inspector.androidwxainspector as AWI
     import wechat_mp_inspector.inspector.ioswxainspector as IWI
 else:
     iosdriver = lazy_import("wechat_mp_inspector.driver.iosdriver")
@@ -34,91 +37,18 @@
     IWI = lazy_import("wechat_mp_inspector.inspector.ioswxainspector")
 from ..pages.basepage import *
 from ..pages.chromepage import *
 from .config import AndroidMP, IOSMP, MPConfig
 from ..logger import logger
 import threading
 import time
-from ..utils import WaitThread, thread_wait, get_url_path
+from ..utils import WaitThread, thread_wait, get_url_path, async_race
 from ..exception import *
 from ..emitter import MyEventEmitter
-
-class WebviewPage(object):
-    """小程序普通页面实例"""
-
-    PAGE_INFO_MAP = {}  # webviewId -> page_info
-    inspector: AWI.WebviewInspector
-    page_info: dict
-
-    def __new__(cls, inspector: AWI.WebviewInspector, **page_info):
-        if "webviewId" in page_info:
-            webview_id = page_info["webviewId"]
-        else:
-            webview_id = None
-        inst = object.__new__(cls)
-        if webview_id in cls.PAGE_INFO_MAP:
-            page_info.update(cls.PAGE_INFO_MAP[webview_id])
-        elif webview_id:
-            cls.PAGE_INFO_MAP[webview_id] = page_info
-        inst.inspector = inspector
-        inst.page_info = page_info
-        return inst
-
-    def __init__(self, inspector: AWI.WebviewInspector, **page_info) -> None:
-        page_str = str(self)
-
-        def on_ws_state_change(value):
-            if not value:
-                logger.info("%s link destory" % page_str)
-
-        self.on_ws_state_change = on_ws_state_change
-        self.inspector.on("ConnectionStateChange", self.on_ws_state_change)
-
-    def __del__(self):
-        logger and logger.debug("%s del" % str(self))
-        self.inspector.remove_listener("ConnectionStateChange", self.on_ws_state_change)
-
-    def __str__(self) -> str:
-        return "[%s]%s" % (
-            self.page_info.get("webviewId"),
-            f"{self.inspector.page.path}[{'visible' if self.inspector.page.visible else 'invisible'}]"
-            if self.inspector.page.title
-            else "unknow",
-        )
-
-    def evaluate(self, expression, **kwargs):
-        return self.inspector.runtime.evaluate(expression, **kwargs)
-
-
-class H5Page(WebviewPage):
-    PAGE_INFO_MAP = {}  # webviewId -> page_info
-    inspector: AWI.H5Inspector
-
-    def __str__(self) -> str:
-        return "[%s]%s[%s]" % (
-            self.page_info.get("webviewId"),
-            self.inspector.page.title,
-            self.inspector.page.url,
-        )
-
-
-class SkylinePage(object):
-    def __init__(self, inspector: AWI.SkylineInspector, **page_info) -> None:
-        self.inspector = inspector
-        self.page_info = page_info
-
-    def __str__(self) -> str:
-        return "[%s]%s[skyline]" % (
-            self.page_info.get("webviewId"),
-            f"{self.page_info['route']}",
-        )
-
-    def evaluate(self, expression, **kwargs):
-        return self.inspector.evaluate(expression, **kwargs)
-
+from ..pages.mppage import WebviewPage, H5Page, SkylinePage
 
 class MiniProgram(BaseDriver):
     driver: BaseDriver = None
     config: MPConfig = None
 
     IGNORE_ID = {}  # appid -> [*unique_ids], 记录一些确定不属于该小程序的 unique id, 减少重复的检查
 
@@ -148,14 +78,15 @@
                 inst.driver = iosdriver.IOSDriver(inst.config)
         return inst
 
     def __init__(self, appid, config: MPConfig = None):
         self.appid = appid
         self.config = config
         self.logger = logger.getChild(f"Mini{self.appid}")
+        self.logger.setLevel(config.logger_level)
         if self.appid not in MiniProgram.IGNORE_ID:
             MiniProgram.IGNORE_ID[self.appid] = []
         self.IGNORE_ID: List[str] = MiniProgram.IGNORE_ID[self.appid]
 
     def get_pages(self):
         return self.driver.get_pages()
 
@@ -172,17 +103,17 @@
         super().__init__(appid, config)
         self.processpid: str = None
         self.at = self.driver.at
         self.sock_cache: Dict[str, str] = {}  # 符合条件的sock缓存一下, [(sock_name, pid)]
         self.appservice: AWI.AppserviceInspector = None
         self.main = None  # maincontext, 一般只有基础库在使用
         self.skyline: AWI.SkylineInspector = None
-        self.pages: Dict[str, AWI.WebviewInspector] = {}  # webviewId -> driver
+        self.pages: Dict[str, AWI.WebviewInspector] = {}  # webviewId -> inspector
         self.ws2page: Dict[str, str] = {}  # debugger url -> webviewId
-        self.h5_pages: Dict[str, AWI.H5Inspector] = {}  # webviewId -> driver
+        self.h5_pages: Dict[str, AWI.H5Inspector] = {}  # webviewId -> inspector
         self._current_page = None
         self._enable_skyline = self.config.skyline
         self._enable_webview = self.config.webview
         self._enable_h5 = self.config.h5
         if self._enable_h5:
             self._enable_webview = True  # 需要检测当前页面是不是确定有web-view组件，必须开启webview检测
         self._enable_sock_cache = self.config.sock_cache
@@ -195,83 +126,67 @@
         self._stop_refresh = False
         if self._enable_skyline:  # 默认先检测appservice链接, 进行一次初始化
             self.init()
 
     def __mark(self, name, start_time):
         self.logger.debug("🚀 %s cost: %.3f" % (name, time.time() - start_time))
 
-    def _get_current_active_process(self, reg_exp):
-        """
-        grep top 5 process, and return process match {reg_exp}
-        :return: process_name, pid
-        """
-        output = self.at.adb.run_shell(
-            f'COLUMNS=512 top -m 10 -n 2 -d 2|grep -e "{reg_exp}"'
-        )
-        self.logger.debug(output)
-        lines = [
-            re.sub(r"\x1B[^m]*m", "", line.strip())
-            for line in output.strip().split("\n")
-        ]  # Filter control character
-        result = []
-        for output2 in lines:
-            r = re.compile("(%s)" % reg_exp)
-            m = r.search(output2)
-            if m:
-                pid = output2.split()[0]
-                m_name = m.group(1)
-                result.append((m_name, pid))
-        if result:
-            return result
-        # 没有match的, 退化成非grep的形式看看
-        return [self.at.adb.get_current_active_process(reg_exp)]
-
     def _get_current_appbrand(self):
         """获取当前小程序进程名和进程id
 
-        :return str, int: processname, pid
+        :return str, int: List[(processname, pid)]
         """
-        result = [
-            [r[0], str(r[1]).strip()]
-            for r in self._get_current_active_process(
-                re.escape("com.tencent.mm:appbrand") + "\d*"
-            )
-        ]
-        if len(result) != 1:
+        for top_m in (15, 20):  # 如果top15找不到尝试使用top20
+            result: List[Tuple[str, str]] = [(r[0], str(r[1]).strip()) for r in self.driver._get_current_active_process(
+                re.escape("com.tencent.mm:appbrand") + "\d*", top_m=top_m
+            )]
             tmp = {}
             for r in result:
                 processname, processpid = r
+                if not processpid or processpid == "None":
+                    continue
                 if processpid not in tmp:
                     tmp[processpid] = r
                     self.logger.debug(
                         f"current appbrand processname[{processname}], id[{processpid}]"
                     )
-            return list(tmp.values())
-        return result
+            result = list(tmp.values())
+            if result:
+                return result
+        return [(None, None),]
 
-    def _init_pid(self):
+    def _init_pid(self) -> str or List[str] or None: # type: ignore
         st = time.time()
+        processpid = None
         if not self.processpid:
             result = self._get_current_appbrand()
             self.__mark("get appbrand pid", st)
             if len(result) == 1:
                 processname, processpid = result[0]
                 self.logger.debug(
                     f"current appbrand processname[{processname}], id[{processpid}]"
                 )
                 self.processpid = processpid
-            else:
-                ret = [r[1] for r in result]
-                ret.sort(key=lambda x: int(x))  # 按进称号排
-                return ret
+            elif result:
+                result.sort(key=lambda x:int(x[1]))  # 按进称号排
+                self.logger.debug(
+                    f"current appbrand name-id: [{','.join([str(r) for r in result])}]"
+                )
+                return [r[1] for r in result]
         else:
             processpid = self.processpid
         return processpid
 
-    def _get_pages(self, processpids: str or List[str]) -> Tuple[List["ChromeAppServicePage"], List["ChromeWebViewPage"], List["ChromeNormalPage"]]:
+    def _get_pages(
+        self, processpids: Union[str, List[str]]
+    ) -> Tuple[
+        List["ChromeAppServicePage"],
+        List["ChromeWebViewPage"],
+        List["ChromeNormalPage"],
+    ]:
         """获取pid下的page实例
 
         :param str pid: process id, defaults to None
         :return List[NormalPage]: 页面实例
         """
 
         def _init_tabs(processpid: str):
@@ -315,16 +230,17 @@
                             webSocketDebuggerUrl = tab.get("webSocketDebuggerUrl")
                             if not webSocketDebuggerUrl:
                                 continue
                             page = ChromeNormalPage(
                                 tab["title"],
                                 tab.get("url", ""),
                                 webSocketDebuggerUrl,
-                                tab.get("id", None) or get_url_path(webSocketDebuggerUrl),
-                                tcp_port,
+                                tab.get("description"),
+                                unique_id=tab.get("id", None) or get_url_path(webSocketDebuggerUrl),
+                                tcp_port=tcp_port,
                                 sock_name=sock_name,
                             )
                             if not page:
                                 continue
                             if page.unique_id in self.IGNORE_ID:
                                 self.logger.debug("ignore %s", page.unique_id)
                                 continue
@@ -409,32 +325,32 @@
         inspector = self.inspector_session(page)
         inspector.set_default_command_timeout(self.config.cmd_timeout)
         # 重启小程序有可能不会改表sock, 但context的unique id可能变化, 需要重新监听
         if inspector.id in AWI.WxaInspector.CONTEXT:  # 已经建立了监听等操作
             AWI.WxaInspector.CONTEXT.pop(inspector.id)
         # service的ws都可以链接上, 但是命令不一定会响应, 需要兼容
         try:
-            main_context = AWI.MainServiceInspector(inspector)
+            main_context = AWI.MainServiceInspector(inspector, page)
         except TimeoutError as te:
             self.logger.exception(te)
             return False
         appid = None
         stime = time.time()
         while time.time() < stime + 5:  # __wxConfig?.accountInfo?.appId注入可能需要些时间
             appid = main_context.evaluate("""__wxConfig?.accountInfo?.appId || ''""")
             if appid:
                 break
             if self.appservice:  # 别的线程已经初始化了
                 break
             time.sleep(0.5)
         if appid == self.appid:
-            self.appservice = AWI.AppserviceInspector(inspector)
+            self.appservice = AWI.AppserviceInspector(inspector, page)
             self._enable_page_info = False  # 如果存在appservice相关信息由appservice更新
             if self._enable_skyline:
-                self.skyline = AWI.SkylineInspector(inspector)
+                self.skyline = AWI.SkylineInspector(inspector, page)
             else:
                 self.logger.info("不进行skyline页面检测")
             self.main = main_context
             return main_context.wait_init(5)  # 等一下初始化
         elif appid:  # 确认当前service不属于目标appid：
             self.IGNORE_ID.append(unique_id)
             return False
@@ -463,16 +379,18 @@
                 except Exception as e:
                     self.logger.error("appservice/skyline链接建立失败")
                     self.logger.exception(e)
             else:
                 self.logger.warning("appservice/skyline链接建立失败, 未检测到相关线程")
         self.__mark("check appservice thread", st)
         return self.appservice
-    
-    def _get_real_webview_id(self, inspector: AWI.WebviewInspector, page: ChromeWebViewPage) -> Tuple[str, str]:
+
+    def _get_real_webview_id(
+        self, inspector: AWI.WebviewInspector, page: ChromeWebViewPage
+    ) -> Tuple[str, str]:
         try:
             ret = inspector.runtime.evaluate(
                 """var i={"webview_id": window.__webviewId__, "appid": __wxConfig__.accountInfo.appId, "route": window.__route__};i"""
             )
             return ret.webview_id, ret.route
         except Exception as e:
             self.logger.exception(f"page[{page.path}] get appid fail")
@@ -589,30 +507,28 @@
         return current_wv_page
 
     def _check_h5(
         self,
         page: ChromeNormalPage,
         webview_id,
         h5_pages: List[AWI.H5Inspector],
-    ) -> AWI.H5Inspector or None:
+    ) -> Optional[AWI.H5Inspector]:
         self.logger.info(f"check {page}")
         try:
             inspector = self.inspector_session(page)
         except Exception as e:
             self.logger.error(f"connect to h5 fail: {page.url}")
             return
         if not self.ws2page.get(page.unique_id):  # 这个websocket没有检查过
             is_mp_h5 = inspector.evaluate("window.__wxjs_environment ? true : false")
             if not is_mp_h5:
                 self.IGNORE_ID.append(page.unique_id)  # 不是mp的h5
                 inspector._session.connection.destroy()
                 return
-            self.ws2page[
-                page.unique_id
-            ] = True  # 标记一下检测过的情况, 第一次检测过肯定不会有对应的webview_id
+            self.ws2page[page.unique_id] = True  # 标记一下检测过的情况, 第一次检测过肯定不会有对应的webview_id
         else:  # 检测过又不在IGNORE_ID中的肯定是mp h5
             pass
         self.logger.info(f"find a mp h5 page: {page.title}, url: {page.url}")
         if not inspector.hidden:
             self.h5_pages[webview_id] = inspector
             self.ws2page[page.unique_id] = webview_id
             return inspector
@@ -659,27 +575,30 @@
                             current_wv_page.page_info.get("route", "").rstrip(".html")
                             != current_page.route
                         ):
                             self.logger.warning(
                                 f"检测current page异常: {current_page.route} != {current_wv_page.page_info.get('route', '')}, 可能是{current_wv_page.inspector.page.title}不准确引起"
                             )
                         else:
-                            real_id, _ = self._get_real_webview_id(current_wv_page.inspector, current_wv_page.inspector.page)
+                            real_id, _ = self._get_real_webview_id(
+                                current_wv_page.inspector,
+                                current_wv_page.inspector.page,
+                            )
                             if real_id != webview_id:
                                 self.logger.warning(
                                     f"检测current page异常, webviewId不一样: {current_page.webviewId} != {real_id}"
                                 )
                             else:
                                 fake_id = current_wv_page.page_info.get("webviewId")
                                 # 用真实webview id, 需要更新 self.pages & self.ws2page
                                 if fake_id in self.pages:
                                     inspector = self.pages[fake_id]
                                     self.ws2page[inspector.page.unique_id] = webview_id
                                     self.pages[webview_id] = self.pages.pop(fake_id)
-                            
+
             elif not current_wv_page.inspector.is_webview:
                 skip = True
             else:
                 webview_id = current_wv_page.page_info.get("webviewId")
                 current_page = current_wv_page.page_info
             semaphore = threading.Semaphore(0)  # 并行检测使用
             if not skip:
@@ -844,17 +763,15 @@
                     # 更新一下信息
                     normal_pages = self._get_pages(self._init_pid())[2]
                     inspector = self.h5_pages[page.webviewId]
                     for np in normal_pages:
                         if np == inspector.page:  # up info
                             inspector.page = np
                             break
-                    return H5Page(
-                        inspector, **page
-                    )  # 这种情况下, 没法刷新实时的url
+                    return H5Page(inspector, **page)  # 这种情况下, 没法刷新实时的url
                 return WebviewPage(self.pages[page.webviewId], **page)
             refresh_thread.join()  # 之前没有出现过的page, 等待重新扫一遍.
             self._print_summary()
             # self._current_page 跟 page 关联一下, update self.pages/self.h5_pages/self.ws2page
             webview_id = self._current_page.page_info.get("webviewId", "")
             if str(webview_id).startswith("fake"):  # 更新真实的webview id
                 url = self._current_page.inspector.page.webSocketDebuggerUrl
@@ -869,23 +786,25 @@
             return None
         # 没有appservice只能靠webview渲染的visible判断
         self.init()
         return self._current_page
 
     # driver 方法
     def get_pages(self):
-        appservice_pages, webview_pages, normal_pages = self._get_pages(self._init_pid())
+        appservice_pages, webview_pages, normal_pages = self._get_pages(
+            self._init_pid()
+        )
         return appservice_pages + webview_pages + normal_pages
 
     def inspector_session(self, page: ChromeNormalPage):
         session_id = str(uuid.uuid4()).upper()
         connection = CDPConnection(page.webSocketDebuggerUrl, unique_id=page.unique_id)
         session = CDPSession(connection, session_id, page, self.driver.refresh_page)
         if isinstance(page, ChromeAppServicePage):
-            return AWI.WxaInspector(session)
+            return AWI.WxaInspector(session, page)
         elif isinstance(page, ChromeWebViewPage):
             return AWI.WebviewInspector(session, page)
         elif isinstance(page, ChromeNormalPage):
             return AWI.H5Inspector(session, page)
         return AndroidInspector(session)
 
 
@@ -898,159 +817,476 @@
         self.ee = MyEventEmitter()
         self.inited = None
         self.closed = False
         # driver中其他实例
         self.appservice: IWI.AppserviceInspector = None
         self.skyline: IWI.SkylineInspector = None
         self.main: IWI.MainServiceInspector = None
+        self.pages: Dict[str, IWI.WebviewInspector] = {}  # webviewId -> inspector
+        self.uid2wid: Dict[str, str] = {}  # unique_id -> webviewId
+        self.h5_pages: Dict[str, IWI.H5Inspector] = {}  # webviewId -> inspector
+        self._current_page = None
 
         # 配置
         self._enable_skyline = self.config.skyline
         self._enable_webview = self.config.webview
         self._enable_h5 = self.config.h5
         if self._enable_h5:
             self._enable_webview = True  # 需要检测当前页面是不是确定有web-view组件，必须开启webview检测
         self._enable_page_info = self.config.init_page_info
-        
+        self._fake_webview_id_map = {}  # 生成假的webview id. sock url -> webviewId
+        self._fake_webview_id = 1  # 从1开始
+        self._fake_webview_id_lock = asyncio.Lock()
 
     @classmethod
-    def listen_app(cls, mini: 'IOSMiniProgram', timeout=20):
+    def listen_app(cls, mini: "IOSMiniProgram", timeout=20):
         while not mini.closed and not mini.inited:  # app没有初始化 & driver未释放
             try:
                 mini.inited = mini.driver.wait_for_app(timeout)
             except TimeoutError:
                 mini.inited = False
             if not mini.inited:
                 mini.logger.warning("app没加载好")
             else:
                 mini.logger.info("监听到app")
                 mini.ee.emit("app_ready")
 
     def close(self):
         self.closed = True
-    
+
     def __mark(self, name, start_time):
         self.logger.debug("🚀 %s cost: %.3f" % (name, time.time() - start_time))
 
-    def _check_appservice(self, page: 'safaripage.SafariAppServicePage') -> bool:
+    def _check_appservice(self, page: "safaripage.SafariAppServicePage") -> bool:
         self.logger.info("try to connect appservice")
         unique_id = page.unique_id
         if unique_id in self.IGNORE_ID:
             self.logger.info("ignore %s", unique_id)
             return False
-        type_ = IWI.WxaInspector.check_type(page.title)
+        type_ = page.type_ or IWI.WxaInspector.check_type(page.title)
         if type_ is not IWI.AppserviceInspector:
             return False
         inspector = self.inspector_session(page)
+        if inspector is None:
+            return False
         inspector.set_default_command_timeout(self.config.cmd_timeout)
         appid = None
         stime = time.time()
         while time.time() < stime + 5:  # __wxConfig?.accountInfo?.appId注入可能需要些时间
             appid = inspector.evaluate("""__wxConfig?.accountInfo?.appId || ''""")
             if appid:
                 break
             if self.appservice:  # 别的线程已经初始化了
                 break
         if appid == self.appid:
-            self.appservice =  inspector
+            self.appservice = inspector
             self._enable_page_info = False
             return True
         elif appid:
             self.IGNORE_ID.append(unique_id)
         return False
-    
-    def _check_skyline(self, page: 'safaripage.SafariAppServicePage') -> bool:
+
+    def _check_skyline(self, page: "safaripage.SafariAppServicePage") -> bool:
         if not self._enable_skyline:
             self.logger.info("不进行skyline页面检测")
             return False
         self.logger.info("try to connect skyline")
         unique_id = page.unique_id
         if unique_id in self.IGNORE_ID:
             self.logger.info("ignore %s", unique_id)
             return False
-        type_ = IWI.WxaInspector.check_type(page.title)
+        type_ = page.type_ or IWI.WxaInspector.check_type(page.title)
         if type_ is not IWI.SkylineInspector:
             return False
         inspector = self.inspector_session(page)
+        if inspector is None:
+            return False
         inspector.set_default_command_timeout(self.config.cmd_timeout)
         appid = None
         stime = time.time()
         while time.time() < stime + 5:  # __wxConfig?.accountInfo?.appId注入可能需要些时间
             appid = inspector.evaluate("""__wxConfig?.accountInfo?.appId || ''""")
             if appid:
                 break
-            if self.appservice:  # 别的线程已经初始化了
+            if self.skyline:  # 别的线程已经初始化了
                 break
         if appid == self.appid:
-            self.appservice =  inspector
+            self.skyline = inspector
             self._enable_page_info = False
             return True
         elif appid:
             self.IGNORE_ID.append(unique_id)
         return False
-        
 
+    def _init_appservice(
+        self, appservice_pages: Dict[str, "safaripage.SafariAppServicePage"]
+    ) -> 'IWI.AppserviceInspector':
+        """初始化appservice线程
 
+        :param Dict[str, 'SafariAppServicePage'] appservice_titles: 符合appservice线程的page
+        """
+        st = time.time()
+        # inspector = self.inspector_session(appservice_pages["main"])
+        if not self.appservice and "appservice" in appservice_pages:
+            # check appservice
+            self._check_appservice(appservice_pages["appservice"])
+        if not self.skyline and self._enable_skyline and "skyline" in appservice_pages:
+            # check skyline
+            self._check_skyline(appservice_pages["skyline"])
+        self.__mark("check appservice thread", st)
+        return self.appservice
 
-    def _init_appservice(self, appservice_pages: Iterable['safaripage.SafariAppServicePage']
-    ) -> IWI.AppserviceInspector:
-        """初始化appservice线程
+    async def _get_real_webview_id(
+        self, inspector: "IWI.WebviewInspector", page: "safaripage.SafariWebViewPage"
+    ) -> Tuple[str, str]:
+        try:
+            ret = await inspector._evaluate(
+                """var i={"webview_id": window.__webviewId__, "appid": (window.__wxConfig__||window.__wxConfig).accountInfo.appId, "route": window.__route__};i"""
+            )
+            page.appid = ret.appid
+            return ret.webview_id, ret.route
+        except Exception as e:
+            self.logger.exception(f"page[{page}] get appid fail")
+        return None, None
+
+    async def _get_webview_id(
+        self, inspector: "IWI.WebviewInspector", page: "safaripage.SafariWebViewPage"
+    ) -> Tuple[str, str]:
+        if self._enable_page_info or page.appid == "preload":
+            return await self._get_real_webview_id(inspector, page)
+        else:
+            return await self._get_fake_webview_id(inspector, page)
+
+    async def _get_fake_webview_id(
+        self, inspector: "IWI.PageInspector", page: "safaripage.SafariNormalPage"
+    ):
+        async with self._fake_webview_id_lock:
+            if inspector.id in self._fake_webview_id_map:
+                return self._fake_webview_id_map[inspector.id], getattr(
+                    page, "path", ""
+                )
+            webview_id = f"fake{page.id_}"
+            self._fake_webview_id += 1
+            self._fake_webview_id_map[inspector.id] = webview_id
+            return webview_id, getattr(page, "path", "")
+
+    async def _check_webview(
+        self,
+        page: "safaripage.SafariWebViewPage",
+        inspector: WebviewInspector,
+        new_pages: set,
+    ) -> Tuple[str, str, "IWI.WebviewInspector", bool]:
+        """检查webview页面状态
+
+        :param safaripage.SafariWebViewPage page: 页面实例
+        :param WebviewInspector inspector: inspector实例
+        :param set new_pages: 新页面集合
+        :return Tuple[str, str, "IWI.WebviewInspector", bool]: webview_id, route, inspector, visible
+        """
+        self.logger.info(f"checking {page}")
+        webview_id, route = await self._get_webview_id(inspector, page)
+        if not webview_id:
+            return None, None, None, False
+        self.pages[
+            webview_id
+        ] = inspector  # 后续可以通过 getCurrentPages().pop().__wxWebviewId__ 查找当前页面是否已经链接过
+        new_pages.add(webview_id)
+        self.uid2wid[page.unique_id] = webview_id
+        hidden = await inspector._hidden()
+        return webview_id, route, inspector, not hidden
+
+    async def _page_hidden(self, inspector: "IWI.PageInspector"):
+        try:
+            return await inspector._hidden()
+        except TimeoutError:
+            inspector.close()
+            return True
+
+    async def _check_visible_page(
+        self, pages: List["safaripage.SafariNormalPage"], check_func: Callable=_check_webview, page_type=WebviewPage, inspector_map: Dict[str, "IWI.PageInspector"]={}
+    ):
+        """检查当前没有hidden的页面
+
+        :param List[safaripage.SafariNormalPage] pages: 页面列表
+        :param Callable check_func: 检查函数, 参考self._check_webview, defaults to _check_webview
+        :param WebviewPage page_type: current_page的实例化类, defaults to WebviewPage
+        :param dict inspector_map: 记录 webviewid -> inspector的dict
+        :return WebviewPage, set: current_page, current_pages
+        """
+        current_page = None
+        current_pages = set()  # 用于更新self.pages
+        check_threads: List[asyncio.Future] = []
+        for page in pages:
+            if not self.uid2wid.get(page.unique_id):  # 未检查过, 丢到线程中并行检查
+                try:
+                    inspector = self.inspector_session(page)
+                except Exception as e:
+                    self.logger.exception(f"inspect {page} fail")
+                    continue
+                if inspector is None:
+                    self.logger.warning(f"inspect {page} fail")
+                    continue
+                future = self.driver.ensure_future(
+                    check_func(page, inspector, current_pages)
+                )
+                check_threads.append(future)
+            else:
+                webview_id = self.uid2wid[page.unique_id]
+                current_pages.add(webview_id)
+                inspector = inspector_map[webview_id]
+                inspector.page = page  # 刷新title
+                route = None
+        if check_threads:  # 有新页面
+            results = self.driver.await_(asyncio.gather(*check_threads))  # 等待并行链接的情况
+            for webview_id, route, inspector, visible in results:
+                if not webview_id:
+                    continue
+                if visible:
+                    current_page = page_type(
+                        inspector, route=route, webviewId=webview_id
+                    )
+                    self.logger.info("current page: %s" % current_page)
+        if (
+            not current_page and current_pages
+        ):
+            inspectors = [inspector_map[webview_id] for webview_id in current_pages]
+            hidden, idx = self.driver.await_(
+                async_race(
+                    *[self._page_hidden(inspector) for inspector in inspectors],
+                    expected_result=False,
+                    loop=self.driver.loop,
+                )
+            )
+            if hidden is False:
+                inspector = inspectors[idx]
+                current_page = page_type(
+                    inspector, route=route, webviewId=webview_id
+                )
+                self.logger.info("current page: %s" % current_page)
+        if not current_page:  # 没有任何webview页面是visible, 可能是h5页面, 也可能当前页面是skyline
+            self.logger.warning("no visible webview page")
+        return current_page, current_pages
+
+    def _init_webview(
+        self, webview_pages: List["safaripage.SafariWebViewPage"]
+    ) -> "IWI.WebviewInspector":
+        """初始化webview页面
 
-        :param Iterable['SafariAppServicePage'] appservice_titles: 符合appservice线程的page
+        :param List[safaripage.SafariWebViewPage] webview_pages: webview页面列表
+        :return IWI.WebviewInspector: 当前webview页面的inspector
         """
         st = time.time()
-        if not self.appservice:
-            for page in appservice_pages:
-                if not self.appservice and self._check_appservice(page):
+        current_wv_page = None  # 当前webview渲染的页面
+        if self._enable_webview:
+            _webview_pages = []
+            for page in webview_pages:
+                if page.appid != self.appid and page.appid != "preload":  # preload竟然也能用
                     continue
-                if not self.skyline and self._check_skyline(page):
+                _webview_pages.append(page)
+            current_wv_page, current_pages = self.driver.await_(self._check_visible_page(_webview_pages, self._check_webview, WebviewPage, self.pages))
+            """
+            current_pages = set()  # 用于更新self.pages
+            check_webview_threads: List[asyncio.Future] = []
+            for page in webview_pages:
+                # getCurrentPages().pop().__wxWebviewId__ 对应 window.__webviewId__
+                # __wxConfig__.accountInfo.appId 为appid, 插件页面中该信息也为宿主appid
+                if page.appid != self.appid and page.appid != "preload":  # preload竟然也能用
                     continue
-        self.__mark("check appservice thread", st)
-        return self.appservice
+                t = None
+                if not self.uid2wid.get(page.unique_id):  # 未检查过, 丢到线程中并行检查
+                    try:
+                        inspector = self.inspector_session(page)
+                    except Exception as e:
+                        self.logger.exception(f"inspect {page} fail")
+                        continue
+                    if inspector is None:
+                        self.logger.warning(f"inspect {page} fail")
+                        continue
+                    future = self.driver.ensure_future(
+                        self._check_webview(page, inspector, current_pages)
+                    )
+                    check_webview_threads.append(future)
+                else:
+                    webview_id = self.uid2wid[page.unique_id]
+                    current_pages.add(webview_id)
+                    inspector = self.pages[webview_id]
+                    inspector.page = page  # 刷新title
+                    route = None
+            if check_webview_threads:  # 有新页面
+                results = self.driver.await_(
+                    asyncio.gather(*check_webview_threads)
+                )  # 等待并行链接的情况
+                for webview_id, route, inspector, visible in results:
+                    if not webview_id:
+                        continue
+                    if visible:
+                        self._current_page = WebviewPage(
+                            inspector, route=route, webviewId=webview_id
+                        )
+                        current_wv_page = self._current_page
+                        self.logger.info("current page: %s" % self._current_page)
+            if (
+                not current_wv_page and current_pages
+            ):  # 没有任何webview页面是visible, 可能是h5页面, 也可能当前页面是skyline
+                inspectors = [self.pages[webview_id] for webview_id in current_pages]
+                hidden, idx = self.driver.await_(
+                    async_race(
+                        *[inspector._hidden() for inspector in inspectors],
+                        expected_result=False,
+                        loop=self.driver.loop,
+                    )
+                )
+                if hidden is False:
+                    inspector = inspectors[idx]
+                    self._current_page = WebviewPage(
+                        inspector, route=route, webviewId=webview_id
+                    )
+                    current_wv_page = self._current_page
+                    self.logger.info("current page: %s" % self._current_page)
+            if not current_wv_page:  # 没有任何webview页面是visible, 可能是h5页面, 也可能当前页面是skyline
+                self.logger.warning("no visible webview page")
+            """
+            if current_wv_page:
+                self._current_page = current_wv_page
+            # 清理旧页面
+            for old_wv_id in list(self.pages.keys()):
+                if old_wv_id not in current_pages:  # 页面可能销毁了
+                    inspector = self.pages.pop(old_wv_id)
+                    self.logger.debug(f"{str(inspector.page)} maybe has destroyed")
+                    if inspector.page.unique_id in self.uid2wid:
+                        self.uid2wid.pop(inspector.page.unique_id)
+                    inspector.close()
+                    if old_wv_id in self.h5_pages:
+                        inspector = self.h5_pages.pop(old_wv_id)
+                        self.logger.debug(f"{str(inspector.page)} maybe has destroyed")
+                        if inspector.page.unique_id in self.uid2wid:
+                            self.uid2wid.pop(inspector.page.unique_id)
+                        inspector.close()
+            self.__mark(f"check {len(webview_pages)} webview page", st)
+        else:
+            self.logger.info("不进行webview页面检测")
+        return current_wv_page
+
+    async def _check_h5(
+        self, page: "safaripage.SafariNormalPage", inspector: H5Inspector
+    ):
+        self.logger.info(f"checking {page}")
+        webview_id, route = await self._get_fake_webview_id(inspector, page)
+        if not webview_id:
+            return None, None, None, False
+        self.h5_pages[webview_id] = inspector
+        self.uid2wid[page.unique_id] = webview_id
+        hidden = await inspector._hidden()
+        return webview_id, route, inspector, not hidden
+
+    def _init_h5(
+        self,
+        normal_pages: List["safaripage.SafariNormalPage"],
+        current_wv_page: "safaripage.SafariWebViewPage",
+    ):
+        """初始化h5页面
 
+        :param List[safaripage.SafariNormalPage] normal_pages: 页面实例
+        :param safaripage.SafariWebViewPage current_wv_page: 当前webview页面, 但ios上如果没有appservice应该检测不出来当前是哪个
+        """
+        if self._enable_h5 and normal_pages:
+            st = time.time()
+            if self.appservice:
+                # TODO
+                pass
+            else:
+                if current_wv_page:
+                    # 没有appservice情况下, webview page的visible状态不明
+                    return None
+                check_webview_threads: List[asyncio.Future] = []
+                for page in normal_pages:
+                    pass
 
     def _init(self):
         """
         初始化:
         1. 扫描所有的可以debug的页面
         2. 过滤出符合当前appid的页面
         """
-        appservice_pages, webview_pages, normal_pages = self._get_pages()
+        stime = time.time()
+        _appservice_pages, _webview_pages, _normal_pages = self._get_pages()
         # 初始化 appservice
+        self.logger.info("🚀🚀🚀🚀 service 🚀🚀🚀🚀")
+        self.logger.info("\n".join([str(_) for _ in _webview_pages]))
+        appservice_pages = IWI.WxaInspector.check_service_page(_appservice_pages, self.appid)
         self._init_appservice(appservice_pages)
+        self.logger.debug(self.appservice)
 
+        # 检测小程序webview渲染的页面
+        self.logger.info("🚀🚀🚀🚀 webview 🚀🚀🚀🚀")
+        self.logger.info("\n".join([str(_) for _ in _webview_pages]))
+        self.logger.info("🚀🚀🚀🚀 normal 🚀🚀🚀🚀")
+        self.logger.info("\n".join([str(_) for _ in _normal_pages]))
+        current_wv_page = self._init_webview(_webview_pages)
+        # 检测h5页面
+        self._init_h5(
+            _normal_pages,
+            current_wv_page,
+        )
 
-        
-    def init(self):
+        self.__mark("init total", stime)
+
+    def _refresh(self):
+        stime = time.time()
+        _appservice_pages, _webview_pages, _normal_pages = self._get_pages()
+        # 检测小程序webview渲染的页面
+        self.logger.info("🚀🚀🚀🚀 webview 🚀🚀🚀🚀")
+        self.logger.info("\n".join([str(_) for _ in _webview_pages]))
+        self.logger.info("🚀🚀🚀🚀 normal 🚀🚀🚀🚀")
+        self.logger.info("\n".join([str(_) for _ in _normal_pages]))
+        current_wv_page = self._init_webview(_webview_pages)
+        # 检测h5页面
+        self._init_h5(
+            _normal_pages,
+            current_wv_page,
+        )
+        self.__mark("refresh total", stime)
+
+    def init(self, timeout=10):
         if self.inited is None:
             self.inited = False
             threading.Thread(target=IOSMiniProgram.listen_app, args=(self, ), daemon=True).start()
+            # IOSMiniProgram.listen_app(self)
         if not self.inited:
             self.ee.remove_listener("app_ready", self._init)
-            # self.ee.on("app_ready", self._init)
+            self.ee.on("app_ready", self._init)
+            if self.wait_init(timeout=timeout):
+                self._init()
         else:
             self._init()
         return self.inited
         # if not self.driver.wait_for_app(20):
         #     self.logger.warning("app没加载好")
 
     def wait_init(self, timeout=10):
         if self.inited:
             return True
         s = threading.Semaphore(0)
         self.ee.once("app_ready", s.release)
-        return s.acquire(timeout=timeout)       
+        return s.acquire(timeout=timeout)
 
     # mp driver 方法
     @property
     def current_page(self):
-        pass
+        if self.appservice:
+            current_page = self.appservice.current_page
 
     # driver 方法
-    def _get_pages(self) -> Tuple[List["safaripage.SafariAppServicePage"], List["safaripage.SafariWebViewPage"], List["safaripage.SafariNormalPage"]]:
+    def _get_pages(
+        self,
+    ) -> Tuple[
+        List["safaripage.SafariAppServicePage"],
+        List["safaripage.SafariWebViewPage"],
+        List["safaripage.SafariNormalPage"],
+    ]:
         pages = self.driver.get_pages()
         appservice_pages = []
         webview_pages = []
         other_pages = []
         for p in pages:
             inst = safaripage.SafariNormalPage(p)
             if inst:
@@ -1058,33 +1294,58 @@
                     appservice_pages.append(inst)
                 elif isinstance(inst, safaripage.SafariWebViewPage):
                     webview_pages.append(inst)
                 else:
                     other_pages.append(inst)
         return appservice_pages, webview_pages, other_pages
 
-    def get_pages(self) -> List['safaripage.SafariNormalPage' or 'safaripage.SafariAppServicePage' or 'safaripage.SafariWebViewPage']:
+    def get_pages(
+        self,
+    ) -> List[
+        "safaripage.SafariNormalPage"
+        or "safaripage.SafariAppServicePage"
+        or "safaripage.SafariWebViewPage"
+    ]:
         appservice_pages, webview_pages, normal_pages = self._get_pages()
         return appservice_pages + webview_pages + normal_pages
 
-    def inspector_session(self, page: 'safaripage.SafariNormalPage') -> Union['IWI.WxaInspector', 'IWI.WebviewInspector', 'IWI.H5Inspector', 'IWI.IOSInspectorSession']:
+    async def _inspector_session(
+        self, page: "safaripage.SafariNormalPage"
+    ) -> Union[
+        "IWI.WxaInspector",
+        "IWI.WebviewInspector",
+        "IWI.H5Inspector",
+        "IWI.IOSInspectorSession",
+    ]:
         session_id = str(uuid.uuid4()).upper()
         session = iosdriver.WIPSession(self.driver.connection, session_id, page.page)
         if isinstance(page, safaripage.SafariAppServicePage):
-            return self.driver.await_(IWI.WxaInspector.create(session, page))
+            return await IWI.WxaInspector.create(session, page, timeout=10)
         elif isinstance(page, safaripage.SafariWebViewPage):
-            return self.driver.await_(IWI.WebviewInspector.create(session))
+            return await IWI.WebviewInspector.create(session, page, timeout=10)
         elif isinstance(page, safaripage.SafariNormalPage):
-            return self.driver.await_(IWI.H5Inspector.create(session))
-        return self.driver.await_(IWI.IOSInspectorSession.create(session))
+            return await IWI.H5Inspector.create(session, page)
+        return await IWI.IOSInspectorSession.create(session)
+
+    def inspector_session(
+        self, page: "safaripage.SafariNormalPage"
+    ) -> Union[
+        "IWI.WxaInspector",
+        "IWI.WebviewInspector",
+        "IWI.H5Inspector",
+        "IWI.IOSInspectorSession",
+    ]:
+        return self.driver.await_(self._inspector_session(page), loop=self.driver.connection.loop)
 
 
 if __name__ == "__main__":
     from ..protocol.protocoltypes import *
     import sys
+    import asyncio
+
     print(sys.version_info)
 
     appid = "wx3eb9cfc5787d5458"
     # readme
     # mini: AndroidMiniProgram = MiniProgram(
     #     appid, AndroidMP(logger_level=10, skyline=True)
     # )
@@ -1115,23 +1376,66 @@
     #     logger.warning("h5: %s" % inspector.send_command(Runtime.evaluate(expression="""document.title""", returnByValue=True)))
     #     inspector.close()
 
     # print(mini.current_page)
     # logger.info(mini.current_page.evaluate("""__wxConfig__?.accountInfo?.appId"""))
 
     # ios
-    mini: IOSMiniProgram = MiniProgram(appid, IOSMP({
-        "bundle": 'com.tencent.qy.xin',
-        "connect_timeout": 5,
-        "logger_level": 10
-    }))
-    if not mini.init():
-        mini.wait_init(22)
-    pages= mini.get_pages()
-    for p in pages:
-        print(p)
-    if not mini.init():
-        mini.wait_init(22)
-    pages= mini.get_pages()
-    for p in pages:
-        print(p)
+    mini: IOSMiniProgram = MiniProgram(
+        appid,
+        IOSMP(
+            {"bundle": "com.tencent.qy.xin", "connect_timeout": 5, "logger_level": 10, "init_page_info": True, "cmd_timeout": 3}
+        ),
+    )
+    # IOSMiniProgram.listen_app(mini)
+    # mini.wait_init(10)
+    if not mini.init(1):
+        if not mini.wait_init(10):
+            exit(-1)
+    # exit(0)
+    time.sleep(3)
+    a, w, n = mini._get_pages()
+
+    print("🚀🚀🚀🚀 appservice 🚀🚀🚀🚀")
+    print("\n".join([str(_) for _ in a]))
+    print("🚀🚀🚀🚀 webview 🚀🚀🚀🚀")
+    print("\n".join([str(_) for _ in w]))
+    inspector1: IWI.WxaInspector = None
+    for i in range(len(a)-1, -1, -1):
+        inspector1 = mini.inspector_session(a[i])
+        if inspector1 is not None:
+            break
+    try:
+        print(inspector1)
+        inspector1.await_(inspector1._send_command(
+            "Runtime.evaluate", {
+                "expression": """(window.__wxConfig||window.__wxConfig__).accountInfo""", 
+                "returnByValue": True
+            }, max_timeout=3
+        ))
+        logger.info("🚀🚀🚀🚀 %s", inspector1.evaluate(
+            """__wxConfig.accountInfo""", returnByValue=True
+        ))
+    except:
+        logger.exception("")
+    
+    inspector2: IWI.WebviewInspector = None
+    for i in range(len(w)):
+        inspector2 = mini.inspector_session(w[i])
+        if inspector2 is not None:
+            break
+    logger.info("🚀🚀🚀🚀 %s", inspector2.evaluate(
+        """(window.__wxConfig||window.__wxConfig__).accountInfo""", returnByValue=True, timeout=3
+    ))
+
+
+    # mini.init()
+    # print(f"current page {mini._current_page}")
+
+    # mini._refresh()
+    # print(f"current page {mini._current_page}")
+    # pages= mini.get_pages()
+    # for p in pages:
+    #     print(p)
+    # inspector2.await_(asyncio.sleep(3))
+    mini.driver.connection.destroy()
     mini.close()
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/emitter.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/emitter.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/event.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/event.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/androidinspector.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/androidinspector.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-14 14:21:52
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 10:57:33
+LastEditTime: 2024-02-28 17:42:16
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/inspector/androidinspector.py
 Description: 定义inspector基本逻辑, 与protocol互相引用
 '''
+from typing import Union
 from .baseinspector import *
 from ..protocol.cdp import CDPSession
 
 class AndroidInspector(BaseInspector):
     DEFAULT_COMMAND_TIMEOUT = 10
     _session: CDPSession
-    def __init__(self, session: CDPSession) -> None:
-        super(AndroidInspector, self).__init__(session)
+    def __init__(self, session: CDPSession, **kwargs) -> None:
+        super(AndroidInspector, self).__init__(session=session, **kwargs)
 
     @property
     def id(self):
         return self._session.connection.id
         
-    def send_command(self, command: str or ProtocolCommand or CommandType, params: dict = None, *, sync=True, max_timeout=None, **kwargs):
+    def send_command(self, command: Union[str, ProtocolCommand, CommandType], params: dict = None, *, sync=True, max_timeout=None, **kwargs):
         if max_timeout is None:
             max_timeout = self.default_command_timeout
         return self._session.send_command(command, params, sync=sync, max_timeout=max_timeout, **kwargs)
 
-    def on(self, event: str or BaseEvent, callback: typing.Callable):
+    def on(self, event: Union[str, BaseEvent], callback: typing.Callable):
         return self._session.on(event, callback)
 
-    def remove_listener(self, event: str or BaseEvent, callback: typing.Callable):
+    def remove_listener(self, event: Union[str, BaseEvent], callback: typing.Callable):
         return self._session.remove_listener(event, callback)
 
-    def remove_all_listeners(self, event: str or BaseEvent=None):
+    def remove_all_listeners(self, event: Union[str, BaseEvent]=None):
         if event:
             return self._session.remove_listener(event, callback=None)
         return self._session.remove_all_listeners()
 
     def close(self):
         return self._session.close()
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/androidwxainspector.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/mpdriver.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,144 +1,94 @@
-'''
+"""
 Author: yopofeng yopofeng@tencent.com
-Date: 2023-10-11 11:52:33
+Date: 2023-06-06 17:11:49
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-31 20:52:07
-FilePath: /wechat-mp-inspector/wechat_mp_inspector/inspector/wxainspector.py
-Description: 安卓小程序wxa service线程inspector和各种页面类型的inspector
-'''
+LastEditTime: 2023-06-09 17:23:59
+FilePath: /at/at/webdriver/weapp/skylinedriver.py
+Description: 封装mp的驱动
+"""
 import time
-import typing
-from dataclasses import dataclass
-from ..protocol.cdp import CDPSession, ChromeInspectorProtocol
-from .baseinspector import BaseInspector
-from .androidinspector import AndroidInspector
-from ..connection.baseconn import BaseConnection
-from ..logger import logger
-from ..utils import Callback, Object
-from ..exception import *
-from ..pages.basepage import *
-if typing.TYPE_CHECKING:
-    from ..pages.chromepage import *
-    from ..pages.safaripage import *
-
-__all__ = [
-    'WxaInspector',
-    'MainServiceInspector',
-    'AppserviceInspector',
-    'SkylineInspector',
-    'WebviewInspector',
-    'H5Inspector'
-]
-
-class Runtime(object):
-    TMP = set()
-    domain = ChromeInspectorProtocol.protocol.Runtime
-    def __init__(self, session: CDPSession, ) -> None:
-        self.session = session
-        if session.connection.id not in Runtime.TMP:
-            self._test_pong()
-            Runtime.TMP.add(session.connection.id)
-            
-    def _test_pong(self):
-        """5s一次来自inpector的pong信息"""
-        _id = self.session.send_command(
-            self.domain.addBinding(name="test_pong"), sync=False
-        )
-        self.session.connection._ee.once(
-            _id,
-            lambda *args: self.session.send_command(self.domain.evaluate(expression="""setInterval(function(){typeof test_pong !== "undefined" && test_pong(new Date().toString().slice(0, 24))}, 5000)"""), sync=False)
-        )
+import logging
 
-    def add_binding(self, name):
-        return self.session.send_command(
-            self.domain.addBinding(name=name)
+from .utils import Callback
+from .cdpdriver import CDPWebSocket, Runtime
+from .exception import *
+
+logger = logging.getLogger("WMI")
+
+
+class AppserviceWebSocket(CDPWebSocket):
+    def __new__(
+        cls,
+        debugger_url,
+        sock_name,
+        title,
+        tcp_port=None,
+        *args,
+        auto_reconnect=False,
+        **kwargs,
+    ):
+        if not debugger_url and not tcp_port:
+            raise Runtime("miss debugger_url or tcp_port")
+        return super().__new__(
+            cls,
+            debugger_url,
+            sock_name,
+            title,
+            tcp_port,
+            *args,
+            unique_id=AppserviceWebSocket.get_unique_id(sock_name, title),
+            auto_reconnect=auto_reconnect,
+            **kwargs,
         )
 
-    def discard_console(self):
-        """
-        Runtime.discardConsoleEntries
-        异步即可
-        """
-        self.session.connection.ignore_method.add("Runtime.consoleAPICalled")
-        return self.session.send_command(
-            self.domain.discardConsoleEntries(),
-            sync=False,
-            ignore_response=True
-        )
+    @classmethod
+    def get_unique_id(cls, sock_name, title):
+        """生成唯一id"""
+        return f"{sock_name}:{title}"
 
-    def disable(self):
-        """Runtime.disable"""
-        return self.session.send_command(self.domain.disable())
-
-    def enable(self):
-        """Runtime.enable"""
-        return self.session.send_command(self.domain.enable())
-    
-    def evaluate(
-        self,
-        expression: str,
-        contextId=None,
-        uniqueContextId=None,
-        timeout=None,
-        returnByValue=True,
-        **kwargs
-    ):
-        cmd = self.domain.evaluate(expression=expression, includeCommandLineAPI=True, returnByValue=returnByValue, **kwargs)
-        if uniqueContextId:
-            cmd.uniqueContextId = uniqueContextId
-        elif contextId:
-            cmd.contextId = contextId
-        return self.session.send_command(cmd, max_timeout=timeout).result.result.value
+    @classmethod
+    def get_debugger_url(cls, sock_name, title, tcp_port, *args, **kwargs):
+        return "ws://127.0.0.1:%s/page/%s" % (tcp_port, title)
 
-    
-    def on(self, event, callback: Callback = None) -> Callback:
-        if callback is None:
-            _callback = Callback()
-        elif isinstance(callback, Callback):
-            _callback = callback
-        else:
-            _callback = Callback(callback)
-        self.session.on("Runtime." + event, _callback.callback)
-        return _callback
 
-class WxaInspector(AndroidInspector):
-    CONTEXT = {}  # session.connection.id -> context_map[name -> (context_id, context_unique_id)]
+class WxaServiceDriver(object):
+    CONTEXT = {}  # ws.id -> context_map[name -> (context_id, context_unique_id)]
     CONTEXT_NAME = ()
     context_created_callback = None
     logger = logger.getChild("WxaService")
 
     @classmethod
-    def listenContextCreated(cls, session: CDPSession):
+    def listenContextCreated(cls, ws: CDPWebSocket):
         cls.logger.info("start listen context created")
-        runtime = Runtime(session)
+        runtime = Runtime(ws)
 
-        def executionContextCreated(context_info: ChromeInspectorProtocol.protocol.Runtime.executionContextCreated):
+        def executionContextCreated(context_info):
             cls.logger.info(f"context info: {context_info}")
-            cls.CONTEXT[session.connection.id][context_info.context.name] = (
+            cls.CONTEXT[ws.id][context_info.context.name] = (
                 context_info.context.id,
                 context_info.context.uniqueId,
             )
 
         runtime.discard_console()
         # enable只有第一次执行会回调现有的context内容, 先disable
         runtime.disable()
-        cls.CONTEXT[session.connection.id] = {}
+        cls.CONTEXT[ws.id] = {}
         cls.context_created_callback = runtime.on(
             "executionContextCreated", executionContextCreated
         )
         runtime.enable()
 
-    def __init__(self, session: CDPSession) -> None:
-        super().__init__(session)
-        self.runtime = Runtime(session)
+    def __init__(self, ws: AppserviceWebSocket) -> None:
+        self.ws = ws
+        self.runtime = Runtime(ws)
         self.context_id = None
         self.context_unique_id = None
-        if session.connection.id in WxaInspector.CONTEXT:  # 已经建立了监听等操作
-            context_map = WxaInspector.CONTEXT[session.connection.id]
+        if ws.id in WxaServiceDriver.CONTEXT:  # 已经建立了监听等操作
+            context_map = WxaServiceDriver.CONTEXT[ws.id]
             for context_name in self.__class__.CONTEXT_NAME:
                 if context_name in context_map:
                     self.context_id, self.context_unique_id = context_map[context_name]
             if not self.inited:  # context还没有创建, 注册监听
                 self.logger.warning(
                     "%s context not init, listen them"
                     % (" or ".join(self.__class__.CONTEXT_NAME))
@@ -146,151 +96,207 @@
                 self.context_created_callback = self.runtime.on(
                     "executionContextCreated", self.onContextCreated
                 )
         else:
             self.context_created_callback = self.runtime.on(
                 "executionContextCreated", self.onContextCreated
             )
-            WxaInspector.listenContextCreated(session)
+            WxaServiceDriver.listenContextCreated(ws)
 
     @property
     def inited(self):
         return bool(self.context_id or self.context_unique_id)
 
+    def onContextCreated(self, context_info):
+        if context_info.context.name in self.__class__.CONTEXT_NAME:
+            self.context_id = context_info.context.id
+            self.context_unique_id = context_info.context.uniqueId
+
     def ensure_init(self):
         if not self.inited:
             self.logger.warning(
                 "%s context not init" % (" or ".join(self.__class__.CONTEXT_NAME))
             )
             return False
         return True
-    
+
+    def evaluate(self, expression: str, timeout=None, **kwargs):
+        if not self.ensure_init():
+            return
+        return self.runtime.evaluate(
+            expression, self.context_id, self.context_unique_id, timeout, **kwargs
+        )
+
     def wait_init(self, timeout=0):
         if self.inited:
             return True
         if not self.context_created_callback:
             self.logger.warning("not listened")
             return False
         stime = time.time()
         while self.context_created_callback.acquire(
             max(timeout - (time.time() - stime), 0)
         ):
             if self.inited:
                 return True
-        return False
-    
+
     @property
     def is_connecting(self):
         try:
             return self.evaluate(
                 "typeof __wxConfig__ !== 'undefined' ? true: false", timeout=5
             )
         except TimeoutError:
-            self.logger.warning(f"WxaServiceDriver thread maybe disconnected: [{self._session.connection._url}]")
+            self.logger.warning(f"WxaServiceDriver thread maybe disconnected: [{self.ws._url}]")
             return False
-
-    def onContextCreated(self, context_info: ChromeInspectorProtocol.protocol.Runtime.executionContextCreated):
-        if context_info.context.name in self.__class__.CONTEXT_NAME:
-            self.context_id = context_info.context.id
-            self.context_unique_id = context_info.context.uniqueId
-
-    def evaluate(self, expression: str, timeout=None, **kwargs):
-        if not self.ensure_init():
-            return
-        return self.runtime.evaluate(
-            expression, self.context_id, self.context_unique_id, timeout, **kwargs
-        )
+        
+    def close(self):
+        pass
 
 
-class MainServiceInspector(WxaInspector):
+class MainServiceDriver(WxaServiceDriver):
     CONTEXT_NAME = ("MainContext",)
 
-    def __init__(self, session: CDPSession or WxaInspector) -> None:
-        if isinstance(session, WxaInspector):
-            super().__init__(session._session)
-        else:
-            super().__init__(session)
+    def __init__(self, ws: AppserviceWebSocket) -> None:
+        super().__init__(ws)
         if not self.context_id:
             self.context_id = 1  # 主context默认id == 1
 
 
-class CurrentPage(Object):
-    route: str = ''
-    webviewId: str = ''
-    renderer: str = ''
-    exparserNodeId: str = ''
-    url: str = ''
-
-class AppserviceInspector(WxaInspector):
+class AppserviceDriver(WxaServiceDriver):
     CONTEXT_NAME = ("SubContext-2",)
 
-    def __init__(self, session: CDPSession or WxaInspector) -> None:
-        if isinstance(session, WxaInspector):
-            super().__init__(session._session)
-        else:
-            super().__init__(session)
-
-    def _get_current_page(self) -> CurrentPage:
+    def _get_current_page(self):
         js = """(function(){
         var i = getCurrentPages().pop()
         return {
             "route": i.route,
             "webviewId": i.__wxWebviewId__,
             "renderer": i.renderer,
             "exparserNodeId": i.__wxExparserNodeId__
         }})()"""
         try:
-            return CurrentPage(**self.evaluate(js))
+            return self.evaluate(js)
         except Exception as e:
             if str(e) == "uniqueContextId not found":
                 raise UniqueContextIdNotFound(str(e))
             raise
 
     @property
     def current_page(self):
         return self._get_current_page()
 
 
-class SkylineInspector(WxaInspector):
+class SkylineDriver(WxaServiceDriver):
     CONTEXT_NAME = ("SubContext-3", "app_sub_render")
 
-    def __init__(self, session: CDPSession or WxaInspector) -> None:
-        if isinstance(session, WxaInspector):
-            super().__init__(session._session)
-        else:
-            super().__init__(session)
-
-
-class PageInspector(AndroidInspector):
-    def __init__(self, session: CDPSession) -> None:
-        super().__init__(session)
-        self.runtime = Runtime(session)
-
-    def evaluate(self, expression, **kwargs):
-        return self.runtime.evaluate(expression, **kwargs)
 
-class WebviewInspector(PageInspector):
+class WebviewDriver(object):
     """小程序的webview页面"""
-    def __init__(self, session: CDPSession, page: 'ChromeWebViewPage' or 'SafariWebViewPage'=None) -> None:
-        super().__init__(session)
-        self.page = page
+
+    def __init__(self, ws: CDPWebSocket, title=None) -> None:
+        self.ws = ws
+        self.title = title
+        self.runtime = Runtime(ws)
         self._is_webview = None
 
     @property
     def is_webview(self):
         """是否是web-view页面"""
         if self._is_webview is None:
             self._is_webview = self.runtime.evaluate(
                 """document.querySelector("wx-web-view") ? true : false"""
             )
         return self._is_webview
     
-class H5Inspector(PageInspector):
+    def evaluate(self, expression, **kwargs):
+        return self.runtime.evaluate(expression, **kwargs)
+    
+    def close(self):
+        self.ws.close()
+
+
+class H5Driver(object):
     """普通h5"""
-    def __init__(self, session: CDPSession, page: 'ChromeNormalPage' or 'SafariNormalPage'=None) -> None:
-        super().__init__(session)
-        self.page = page
-        self.runtime = Runtime(session)
+
+    def __init__(self, ws: CDPWebSocket, title=None, url=None) -> None:
+        self.ws = ws
+        self.title = title
+        self.url = url
+        self.runtime = Runtime(ws)
 
     @property
     def hidden(self):
-        return self.runtime.evaluate("document.hidden")
+        return self.runtime.evaluate("document.hidden")
+
+    def evaluate(self, expression, **kwargs):
+        return self.runtime.evaluate(expression, **kwargs)
+    
+    def close(self):
+        self.ws.close()
+
+
+class WebviewPage(object):
+    PAGE_INFO_MAP = {}  # webviewId -> page_info
+    driver: WebviewDriver
+    page_info: dict
+    def __new__(cls, driver: WebviewDriver, **page_info):
+        if "webviewId" in page_info:
+            webview_id = page_info["webviewId"]
+        else:
+            webview_id = None
+        inst = object.__new__(cls)
+        if webview_id in cls.PAGE_INFO_MAP:
+            page_info.update(cls.PAGE_INFO_MAP[webview_id])
+        elif webview_id:
+            cls.PAGE_INFO_MAP[webview_id] = page_info
+        inst.driver = driver
+        inst.page_info = page_info
+        return inst
+    
+    def __init__(self, driver: WebviewDriver, **page_info) -> None:
+        page_str = str(self)
+        def on_ws_state_change(value):
+            if not value:
+                logger.info("%s link destory" % page_str)
+        self.on_ws_state_change = on_ws_state_change
+        self.driver.ws.on("ConnectionStateChange", self.on_ws_state_change)
+
+    def __del__(self):
+        logger.debug("%s del" % str(self))
+        self.driver.ws.remove_listener("ConnectionStateChange", self.on_ws_state_change)
+
+    def __str__(self) -> str:
+        return "[%s]%s" % (
+                    self.page_info.get("webviewId"),
+                    f"{self.driver.title.path}[{'visible' if self.driver.title.visible else 'invisible'}]"
+                    if self.driver.title
+                    else "unknow",
+                )
+    
+    def evaluate(self, expression, **kwargs):
+        return self.driver.evaluate(expression, **kwargs)
+    
+class H5Page(WebviewPage):
+    PAGE_INFO_MAP = {}  # webviewId -> page_info
+    driver: H5Driver
+
+    def __str__(self) -> str:
+        return "[%s]%s[%s]" % (
+                    self.page_info.get("webviewId"),
+                    self.driver.title,
+                    self.driver.url
+                )
+
+class SkylinePage(object):
+    def __init__(self, driver: SkylineDriver, **page_info) -> None:
+        self.driver = driver
+        self.page_info = page_info
+    
+    def __str__(self) -> str:
+        return "[%s]%s[skyline]" % (
+                    self.page_info.get("webviewId"),
+                    f"{self.page_info['route']}"
+                )
+
+    def evaluate(self, expression, **kwargs):
+        return self.driver.evaluate(expression, **kwargs)
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/inspector/baseinspector.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/inspector/baseinspector.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-14 14:21:52
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 10:54:39
+LastEditTime: 2024-02-28 17:44:02
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/inspector/baseinspector.py
 Description: 定义inspector基本逻辑, 与protocol互相引用
 '''
 import typing
+from typing import Union
 import abc
 from ..protocol.basesession import BaseSession
 from ..event import BaseEvent
 from ..command import CommandType
 from ..protocol.protocolcommand import ProtocolCommand
 
-class BaseInspector:
+class BaseInspector(metaclass=abc.ABCMeta):
     DEFAULT_COMMAND_TIMEOUT = 10
-    def __init__(self, session: BaseSession) -> None:
+    def __init__(self, session: BaseSession, **kwargs) -> None:
         self._session = session
         self.default_command_timeout = self.__class__.DEFAULT_COMMAND_TIMEOUT
 
     def set_default_command_timeout(self, timeout: int):
         self.default_command_timeout = timeout
 
     @property
     def id(self):
         return self._session.id_
         
     @abc.abstractmethod
-    def send_command(self, command: str or ProtocolCommand or CommandType, params: dict = None, *, sync=True, max_timeout=DEFAULT_COMMAND_TIMEOUT, **kwargs):
+    def send_command(self, command: Union[str, ProtocolCommand, CommandType], params: dict = None, *, sync=True, max_timeout=DEFAULT_COMMAND_TIMEOUT, **kwargs):
         pass
 
+    async def _send_command(self, command: Union[str, ProtocolCommand, CommandType], params: dict = None, *, sync=True, max_timeout=DEFAULT_COMMAND_TIMEOUT, **kwargs):
+        raise NotImplementedError()
+
     @abc.abstractmethod
-    def on(self, event: str or BaseEvent, callback: typing.Callable):
+    def on(self, event: Union[str, BaseEvent], callback: typing.Callable):
         pass
 
     @abc.abstractmethod
-    def remove_listener(self, event: str or BaseEvent, callback: typing.Callable): ...
+    def remove_listener(self, event: Union[str, BaseEvent], callback: typing.Callable): ...
 
     @abc.abstractmethod
-    def remove_all_listeners(self, event: str or BaseEvent=None): ...
+    def remove_all_listeners(self, event: Union[str, BaseEvent]=None): ...
 
     @abc.abstractmethod
     def close(self): ...
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/logger.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/logger.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/miniprogram.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/miniprogram.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 import re
 import requests
 import time
 import json
 import logging
 import typing
+from typing import Union
 import threading
 from .logger import logger, setLevel
 from .title import *
 from .utils import pick_unuse_port, WaitThread, Object, thread_wait
 from .basemp import BaseMP, BMPConfig
 from .mpdriver import *
 from .exception import *
@@ -66,44 +67,48 @@
         self._enable_page_info = self.config.init_page_info
         self._fake_webview_id_map = {}  # 生成假的webview id. sock url -> webviewId
         self._fake_webview_id = 1  # 从1开始
         self._fake_webview_id_lock = threading.Lock()
         self._refresh_lock = threading.RLock()
         self._refresh_thread = None
         self._stop_refresh = False
+        self._last_init_time = None
         self.init()
 
     def __del__(self):
         # self.close()
         pass
 
     def __mark(self, name, start_time):
         self.logger.debug("🚀 %s cost: %.3f" % (name, time.time() - start_time))
         # return time.time()
 
-    def _init_pid(self):
+    def _init_pid(self) -> str or typing.List[str] or None:
         st = time.time()
+        processpid = None
         if not self.processpid:
             result = self._get_current_appbrand()
             self.__mark("get appbrand pid", st)
             if len(result) == 1:
                 processname, processpid = result[0]
                 self.logger.debug(
                     f"current appbrand processname[{processname}], id[{processpid}]"
                 )
                 self.processpid = processpid
-            else:
-                ret = [r[1] for r in result]
-                ret.sort(key=lambda x:int(x))  # 按进称号排
-                return ret 
+            elif result:
+                result.sort(key=lambda x:int(x[1]))  # 按进称号排
+                self.logger.debug(
+                    f"current appbrand name-id: [{','.join([str(r) for r in result])}]"
+                )
+                return [r[1] for r in result]
         else:
             processpid = self.processpid
         return processpid
 
-    def _init_tabs(self, processpids: str or typing.List[str]):
+    def _init_tabs(self, processpids: Union[str, typing.List[str]]):
         """初始化所有符合条件的tab
 
         :param str or typing.List[str] processpid: 小程序进程id
         :return: appservice_titles, webview_titles, other_titles
         """
         def _init_tabs(processpid: str):
             st = time.time()
@@ -118,16 +123,16 @@
             sock_dict = (self._enable_sock_cache and cache_cnt >= 0 and self.sock_cache) or self._get_debug_sock_name()
             if processpid not in sock_dict.values():  # 再确认一下是不是真的没有
                 sock_dict = self._get_debug_sock_name(processpid)
             for sock_name, pid in sock_dict.items():  # 可能有多个remote debug port, 找出属于小程序的那个. sock_cache至少有两个才不
                 # 优化点:
                 # 1. appservice在一个sock中, 微信不重启不会改变.
                 # 2. webview在一个sock中, 不重启也不会改变
-                self.logger.debug(f"find debugger port for {sock_name}")
-                if pid == processpid:
+                self.logger.debug(f"find debugger port for {sock_name}, pid: {pid}, target pid: {processpid}")
+                if pid == processpid or processpid is None or processpid == "None": # 没有检测到目标pid, 全部都当符合条件
                     retry_cnt = 1  # webview title有可能会处于initial状态, 需要至少等一个visible/invisible才可以继续
                     stime = time.time()
                     while retry_cnt:
                         retry_cnt -= 1
                         is_webview_sock = False
                         tabs, tcp_port = self.get_tabs_by_sock(sock_name)
                         self.logger.info(
@@ -388,14 +393,15 @@
         self._init_appservice(appservice_titles)
         # 检测小程序webview渲染的页面
         current_wv_page, current_wv_sock = self._init_webview(webview_titles)
         # 检测小程序h5页面
         self._init_h5(other_titles, current_wv_page, current_wv_sock)
         self.__mark("init total", stime)
         self.print_summary()
+        self._last_init_time = time.time()
 
     def restart(self):
         """
         重启小程序后使用, 重启微信需要重新实例化
         """
         self.sock_cache: typing.Dict[str, str] = {}  # 符合条件的sock缓存一下, [(sock_name, pid)]
         self.appservice = None
@@ -514,24 +520,28 @@
                 self.logger.info("不进行skyline页面检测")
             self.main = main_context
             return main_context.wait_init(5)  # 等一下初始化
         elif appid:  # 确认当前service不属于目标appid：
             self.IGNORE_ID.append(unique_id)
             return False
         
+    def _get_real_webview_id(self, driver: WebviewDriver, title: WebViewTitle=None) -> typing.Tuple[str, str]:
+        try:
+            ret = driver.runtime.evaluate(
+                """var i={"webview_id": window.__webviewId__, "appid": __wxConfig__.accountInfo.appId, "route": window.__route__};i"""
+            )
+            return ret.webview_id, ret.route
+        except Exception as e:
+            self.logger.exception(f"page[{title and title.path}] get appid fail")
+        return None, None
+
     def _get_webview_id(self, driver: WebviewDriver, title: WebViewTitle) -> typing.Tuple[str, str]:
         url = driver.ws._url
         if self._enable_page_info:
-            try:
-                ret = driver.runtime.evaluate(
-                    """var i={"webview_id": window.__webviewId__, "appid": __wxConfig__.accountInfo.appId, "route": window.__route__};i"""
-                )
-                return ret.webview_id, ret.route
-            except Exception as e:
-                self.logger.exception(f"page[{title.path}] get appid fail") 
+            return self._get_real_webview_id(driver, title)
         else:
             with self._fake_webview_id_lock:
                 if url in self._fake_webview_id_map:
                     return self._fake_webview_id_map[url], title.path
                 webview_id = f"fake{self._fake_webview_id}"
                 self._fake_webview_id += 1
                 self._fake_webview_id_map[url] = webview_id
@@ -608,16 +618,18 @@
             d.ws.destroy()
         self.pages = {}
         self.ws2page = {}
         for d in self.h5_pages.values():
             d.ws.destroy()
         self.h5_pages = {}
 
-    @property
-    def current_page(self):
+    def get_current_page(self, cnt):
+        # 可递归重试获取当前页面
+        if cnt > 2:
+            return None
         if self.appservice:
             st = time.time()
             refresh_thread = WaitThread(target=self.refresh, daemon=True)
             refresh_thread.start()  # 先刷
             try:
                 page = self.appservice.current_page
             except (TimeoutError, UniqueContextIdNotFound, ConnectionAbortedError):
@@ -633,38 +645,55 @@
             if page.renderer == "skyline":
                 self._stop_refresh = True
                 refresh_thread.join()
                 self.print_summary()
                 return SkylinePage(self.skyline, **page)
             # webview渲染的页面
             if page.webviewId in self.pages:
+                self._stop_refresh = True
                 if page.webviewId in self.h5_pages:
                     return H5Page(
                         self.h5_pages[page.webviewId], **page
                     )  # 这种情况下, 没法刷新实时的url
                 return WebviewPage(self.pages[page.webviewId], **page)
             refresh_thread.join()  # 之前没有出现过的page, 等待重新扫一遍
             self.print_summary()
             # self._current_page 跟 page 关联一下, update self.pages/self.h5_pages/self.ws2page
+            # BUG: appservice中拿到的page信息, 有可能在chrome tabs中还没有更新过来!
             webview_id = self._current_page.page_info.get("webviewId", "")
             if str(webview_id).startswith("fake"):  # 更新真实的webview id
-                url = self._current_page.driver.ws._url
-                self.ws2page[url] = page.webviewId
-                self.pages[page.webviewId] = self.pages.pop(webview_id)
-                if webview_id in self.h5_pages:
-                    self.h5_pages[page.webviewId] = self.h5_pages.pop(webview_id)
+                real_webview_id, real_route = self._get_real_webview_id(self._current_page.driver, None)
+                if real_webview_id is None:  # 链接不通？大致校验一下path吧
+                    if page.route != self._current_page.page_info.get("route"):
+                        # 拿不到真实webview id, 同时path不是同一个, 认为触发了以上bug
+                        time.sleep(cnt+2)
+                        return self.get_current_page(cnt+1)
+                else:
+                    # 先更新信息
+                    url = self._current_page.driver.ws._url
+                    self.ws2page[url] = real_webview_id
+                    self.pages[real_webview_id] = self.pages.pop(webview_id)
+                    if webview_id in self.h5_pages:
+                        self.h5_pages[real_webview_id] = self.h5_pages.pop(webview_id)
+                    if real_webview_id != page.webviewId: # 应该也触发了上面的bug了
+                        time.sleep(cnt+2)
+                        return self.get_current_page(cnt+1)
             if page.webviewId in self.pages:
                 if page.webviewId in self.h5_pages:
                     return H5Page(self.h5_pages[page.webviewId], **page)
                 return WebviewPage(self.pages[page.webviewId], **page)
             return None
         # 没有appservice只能靠webview渲染的visible判断
         self.init()
         return self._current_page
 
+    @property
+    def current_page(self):
+        return self.get_current_page(0)
+
 
 if __name__ == "__main__":
     import at
 
     level = logging.DEBUG
     logging.basicConfig(level=level)
     logging.lastResort.level = level
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/mpdriver.py` & `minium-1.5.4/minium/native/wx_native/idenative.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,302 +1,355 @@
-"""
-Author: yopofeng yopofeng@tencent.com
-Date: 2023-06-06 17:11:49
-LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-06-09 17:23:59
-FilePath: /at/at/webdriver/weapp/skylinedriver.py
-Description: 封装mp的驱动
-"""
-import time
-import logging
-
-from .utils import Callback
-from .cdpdriver import CDPWebSocket, Runtime
-from .exception import *
-
-logger = logging.getLogger("WMI")
-
-
-class AppserviceWebSocket(CDPWebSocket):
-    def __new__(
-        cls,
-        debugger_url,
-        sock_name,
-        title,
-        tcp_port=None,
-        *args,
-        auto_reconnect=False,
-        **kwargs,
-    ):
-        if not debugger_url and not tcp_port:
-            raise Runtime("miss debugger_url or tcp_port")
-        return super().__new__(
-            cls,
-            debugger_url,
-            sock_name,
-            title,
-            tcp_port,
-            *args,
-            unique_id=AppserviceWebSocket.get_unique_id(sock_name, title),
-            auto_reconnect=auto_reconnect,
-            **kwargs,
-        )
-
-    @classmethod
-    def get_unique_id(cls, sock_name, title):
-        """生成唯一id"""
-        return f"{sock_name}:{title}"
-
-    @classmethod
-    def get_debugger_url(cls, sock_name, title, tcp_port, *args, **kwargs):
-        return "ws://127.0.0.1:%s/page/%s" % (tcp_port, title)
-
-
-class WxaServiceDriver(object):
-    CONTEXT = {}  # ws.id -> context_map[name -> (context_id, context_unique_id)]
-    CONTEXT_NAME = ()
-    context_created_callback = None
-    logger = logger.getChild("WxaService")
-
-    @classmethod
-    def listenContextCreated(cls, ws: CDPWebSocket):
-        cls.logger.info("start listen context created")
-        runtime = Runtime(ws)
-
-        def executionContextCreated(context_info):
-            cls.logger.info(f"context info: {context_info}")
-            cls.CONTEXT[ws.id][context_info.context.name] = (
-                context_info.context.id,
-                context_info.context.uniqueId,
-            )
+#!/usr/bin/env python3
+# Created by xiazeng on 2019-06-11
+import typing
+from .basenative import BaseNative, logger
+from ...utils.utils import Version
+from ...framework.exception import MiniLaunchError
+if typing.TYPE_CHECKING:
+    import minium
+
+class IdeNative(BaseNative):
+    _mini: 'minium.WXMinium' = None  # ide的native操作也依赖minium的实例，可能引起循环引用，需要谨慎处理
+
+    def __init__(self, json_conf, mini=None):
+        self.use_native = False
+        self.mini = mini
+        super().__init__(json_conf)
+        self._support_privacy = True
 
-        runtime.discard_console()
-        # enable只有第一次执行会回调现有的context内容, 先disable
-        runtime.disable()
-        cls.CONTEXT[ws.id] = {}
-        cls.context_created_callback = runtime.on(
-            "executionContextCreated", executionContextCreated
-        )
-        runtime.enable()
-
-    def __init__(self, ws: AppserviceWebSocket) -> None:
-        self.ws = ws
-        self.runtime = Runtime(ws)
-        self.context_id = None
-        self.context_unique_id = None
-        if ws.id in WxaServiceDriver.CONTEXT:  # 已经建立了监听等操作
-            context_map = WxaServiceDriver.CONTEXT[ws.id]
-            for context_name in self.__class__.CONTEXT_NAME:
-                if context_name in context_map:
-                    self.context_id, self.context_unique_id = context_map[context_name]
-            if not self.inited:  # context还没有创建, 注册监听
-                self.logger.warning(
-                    "%s context not init, listen them"
-                    % (" or ".join(self.__class__.CONTEXT_NAME))
-                )
-                self.context_created_callback = self.runtime.on(
-                    "executionContextCreated", self.onContextCreated
-                )
-        else:
-            self.context_created_callback = self.runtime.on(
-                "executionContextCreated", self.onContextCreated
-            )
-            WxaServiceDriver.listenContextCreated(ws)
+    def __del__(self):
+        self.mini = None
 
-    @property
-    def inited(self):
-        return bool(self.context_id or self.context_unique_id)
+    def release(self):
+        super().release()
+        self.mini = None
 
-    def onContextCreated(self, context_info):
-        if context_info.context.name in self.__class__.CONTEXT_NAME:
-            self.context_id = context_info.context.id
-            self.context_unique_id = context_info.context.uniqueId
-
-    def ensure_init(self):
-        if not self.inited:
-            self.logger.warning(
-                "%s context not init" % (" or ".join(self.__class__.CONTEXT_NAME))
-            )
-            return False
-        return True
+    @property
+    def mini(self):
+        return self._mini
 
-    def evaluate(self, expression: str, timeout=None, **kwargs):
-        if not self.ensure_init():
+    @mini.setter
+    def mini(self, value):
+        if self._mini == value:
             return
-        return self.runtime.evaluate(
-            expression, self.context_id, self.context_unique_id, timeout, **kwargs
-        )
-
-    def wait_init(self, timeout=0):
-        if self.inited:
-            return True
-        if not self.context_created_callback:
-            self.logger.warning("not listened")
-            return False
-        stime = time.time()
-        while self.context_created_callback.acquire(
-            max(timeout - (time.time() - stime), 0)
-        ):
-            if self.inited:
-                return True
+        self._mini = value
+        if value is not None and getattr(self._mini, "connection"):
+            self._get_dev_tool_info()
+            try:
+                # 探测一下是不是支持官方隐私弹窗操作
+                self._allow_privacy()
+            except NotImplementedError:
+                self._support_privacy = False
 
-    @property
-    def is_connecting(self):
-        try:
-            return self.evaluate(
-                "typeof __wxConfig__ !== 'undefined' ? true: false", timeout=5
-            )
-        except TimeoutError:
-            self.logger.warning(f"WxaServiceDriver thread maybe disconnected: [{self.ws._url}]")
-            return False
-        
-    def close(self):
+    def start_wechat(self):
         pass
 
+    def stop_wechat(self):
+        ...
 
-class MainServiceDriver(WxaServiceDriver):
-    CONTEXT_NAME = ("MainContext",)
+    def connect_weapp(self, path):
+        ...
 
-    def __init__(self, ws: AppserviceWebSocket) -> None:
-        super().__init__(ws)
-        if not self.context_id:
-            self.context_id = 1  # 主context默认id == 1
-
-
-class AppserviceDriver(WxaServiceDriver):
-    CONTEXT_NAME = ("SubContext-2",)
-
-    def _get_current_page(self):
-        js = """(function(){
-        var i = getCurrentPages().pop()
-        return {
-            "route": i.route,
-            "webviewId": i.__wxWebviewId__,
-            "renderer": i.renderer,
-            "exparserNodeId": i.__wxExparserNodeId__
-        }})()"""
+    def _get_dev_tool_info(self):
         try:
-            return self.evaluate(js)
-        except Exception as e:
-            if str(e) == "uniqueContextId not found":
-                raise UniqueContextIdNotFound(str(e))
-            raise
+            result = self._mini.connection.send("Tool.getInfo", max_timeout=3).result
+        except Exception:
+            # not support Tool.getInfo
+            return
+        if Version(result.SDKVersion) < Version("2.7.3"):
+            raise MiniLaunchError("基础库版本[%s]过低，请确认基础库版本>=2.7.3" % self.sdk_version)
+        if str(result.version).endswith("2") and Version(result.version) >= "1.06.2211072":  # nightly
+            self.use_native = True
+        elif str(result.version).endswith("1") and Version(result.version) >= "1.06.2212011":  # RC
+            self.use_native = True
+        elif Version(result.version) >= "1.06.2301160":  # Stable
+            self.use_native = True
+
+    def _send(self, method, data=None):
+        if self.use_native and self.mini:
+            ret = self.mini.connection.send("Tool.native", {
+                "method": method,
+                "data": data
+            })
+            if "error" in ret.result:
+                message = ret.result.error.get('message', '')
+                if message.startswith("can not find in protocol:"):
+                    raise NotImplementedError(message)
+                logger.warning(f"handle {method} error: {message}")
+                return Exception(message)
+            return ret.result
 
-    @property
-    def current_page(self):
-        return self._get_current_page()
+    def send(self, method, data=None):
+        if isinstance(self._send(method, data), Exception):
+            return False
+        return True
 
+    def go_home(self):
+        """
+        跳转到小程序首页
+        """
+        if self.use_native:
+            return self.send("goHome")
+
+    def navigate_back(self):
+        """
+        左上角返回上一页
+        """
+        if self.use_native:
+            return self.send("navigateLeft")
+
+    def switch_tab(self, url):
+        """
+        点击tabBar
+        """
+        if self.use_native:
+            return self.send("switchTab", {
+                "url": url,  # tabbar 路径, 不带参数
+            })
+
+    def close_payment_dialog(self):
+        """
+        关闭支付弹窗
+        """
+        if self.use_native:
+            return self.send("closePaymentDialog")
+
+    def screen_shot(self, filename, return_format="raw"):
+        if self.mini:
+            self.mini.app.platform = "ide"  # 防止无限回调
+            self.mini.app.screen_shot(filename, return_format)
+            return filename
+        return ""
+
+    def pick_media_file(
+        self,
+        cap_type="camera",
+        media_type="photo",
+        original=False,
+        duration=5.0,
+        names=None,
+    ):
+        raise NotImplementedError("ide not implemented")
 
-class SkylineDriver(WxaServiceDriver):
-    CONTEXT_NAME = ("SubContext-3", "app_sub_render")
+    def allow_authorize(self, answer=True, title=None):
+        return self._allow_authorize(answer)
 
+    def _allow_authorize(self, answer):
+        """
+        mock实现, 所有接口引发的原生弹窗授权理论上都可以使用
+        """
+        if self.use_native:
+            return self.send("authorizeAllow" if answer else "authorizeCancel")
+
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleAuthModal",
+                [
+                    "允许" if answer else "拒绝",
+                ],
+            )
+        return False
+    
+    def _allow_privacy(self, answer=True):
+        return self.send("clickCoverView", {"nodetype": "text", "text": "同意" if answer else "拒绝"})
 
-class WebviewDriver(object):
-    """小程序的webview页面"""
+    def allow_privacy(self, answer=True) -> bool:
+        """处理隐私弹窗
 
-    def __init__(self, ws: CDPWebSocket, title=None) -> None:
-        self.ws = ws
-        self.title = title
-        self.runtime = Runtime(ws)
-        self._is_webview = None
+        :param bool answer: true for 同意, false for 拒绝, defaults to True
+        :raises NotImplementedError:
+        :return bool: true for 处理成功, false for 处理失败
+        """
+        if self.mini:
+            try:
+                ret = self.mini.app.call_wx_method("getPrivacySetting").result.result.needAuthorization
+                if ret:  # 需要处理隐私弹窗, 不支持
+                    return self._allow_privacy(answer)
+            except NotImplementedError as e:
+                if str(e).find("wx.getPrivacySetting") >= 0:
+                    return True  # 不支持getPrivacySetting接口证明没有隐私弹窗
+                raise
+            except:
+                return False
+        return False
+
+    def allow_login(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_get_user_info(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_get_location(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_get_we_run_data(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_record(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_write_photos_album(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_camera(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_get_user_phone(self, answer=True):
+        self._allow_authorize(answer)
+
+    def allow_send_subscribe_message(self, answer=True):
+        """
+        允许发送订阅消息
+        """
+        if self.use_native:
+            return self.handle_modal("允许" if answer else "取消")
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleAuthModal",
+                [
+                    "允许" if answer else "取消",
+                ],
+            )
+        return False
 
-    @property
-    def is_webview(self):
-        """是否是web-view页面"""
-        if self._is_webview is None:
-            self._is_webview = self.runtime.evaluate(
-                """document.querySelector("wx-web-view") ? true : false"""
+    def handle_modal(self, btn_text="确定", title: str = None, force_title=False):
+        """
+        mock实现, 所有接口引发的原生弹窗理论上都可以使用
+        ps: 需要兼容一下授权弹窗
+
+        新工具版本支持native操作, 区分confirm/cancel, btn_text参数支持bool类型指定confirm/cancel
+        """
+        if self.use_native:
+            cancel = not btn_text if isinstance(btn_text, bool) else btn_text in ("取消", "拒绝")
+            if cancel:
+                return self.send("cancelModal")
+            else:
+                return self.send("confirmModal")
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleModal",
+                [
+                    btn_text,
+                ],
             )
-        return self._is_webview
-    
-    def evaluate(self, expression, **kwargs):
-        return self.runtime.evaluate(expression, **kwargs)
-    
-    def close(self):
-        self.ws.close()
 
+    def handle_action_sheet(self, item):
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleModal",
+                [
+                    item,
+                ],
+            )
+        # self.handle_modal(item)
 
-class H5Driver(object):
-    """普通h5"""
+    def forward_miniprogram(
+        self, name: str, text: str = None, create_new_chat: bool = True
+    ):
+        raise NotImplementedError("ide not implemented")
 
-    def __init__(self, ws: CDPWebSocket, title=None, url=None) -> None:
-        self.ws = ws
-        self.title = title
-        self.url = url
-        self.runtime = Runtime(ws)
+    def forward_miniprogram_inside(
+        self, name: str, text: str = None, create_new_chat: bool = True
+    ):
+        if self.use_native:
+            ret = self.send("shareConfirm")
+            if ret:
+                self.forward_miniprogram_cancel()
+            return ret
+        raise NotImplementedError("ide not implemented")
+
+    def forward_miniprogram_cancel(self):
+        if self.use_native:
+            return self.send("shareCancel")
+        return False
+        
+    def handle_alter_before_unload(self, answer=True):
+        """wx.enableAlertBeforeUnload弹框
 
-    @property
-    def hidden(self):
-        return self.runtime.evaluate("document.hidden")
+        :param bool answer: true for确定, false for 取消, defaults to True
+        """
+        if self.use_native:
+            return self.send("confirmConfirm" if answer else "confirmCancel")
+        return False
+
+    def input_text(self, text):
+        if self.mini:
+            self.mini.app.get_current_page().get_element("input").input(text)
+
+    def input_clear(self):
+        if self.mini:
+            self.mini.app.get_current_page().get_element("input").input("")
+
+    def textarea_text(self, text, index=0):
+        if self.mini:
+            els = self.mini.app.get_current_page().get_elements("textarea")
+            els[index].input(text)
+
+    def textarea_clear(self, index=0):
+        if self.mini:
+            els = self.mini.app.get_current_page().get_elements("textarea")
+            els[index].input("")
+
+    def send_custom_message(self, message=None):
+        ...
+
+    def phone_call(self):
+        ...
+
+    def map_select_location(self, name=None):
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleMap",
+                [
+                    name,
+                ],
+            )
 
-    def evaluate(self, expression, **kwargs):
-        return self.runtime.evaluate(expression, **kwargs)
-    
-    def close(self):
-        self.ws.close()
+    def map_back_to_mp(self):
+        if self.mini:
+            return self.mini.app._evaluate_js(
+                "ideHandleMap",
+                [
+                    "取消",
+                ],
+            )
 
+    def deactivate(self, duration):
+        ...
 
-class WebviewPage(object):
-    PAGE_INFO_MAP = {}  # webviewId -> page_info
-    driver: WebviewDriver
-    page_info: dict
-    def __new__(cls, driver: WebviewDriver, **page_info):
-        if "webviewId" in page_info:
-            webview_id = page_info["webviewId"]
-        else:
-            webview_id = None
-        inst = object.__new__(cls)
-        if webview_id in cls.PAGE_INFO_MAP:
-            page_info.update(cls.PAGE_INFO_MAP[webview_id])
-        elif webview_id:
-            cls.PAGE_INFO_MAP[webview_id] = page_info
-        inst.driver = driver
-        inst.page_info = page_info
-        return inst
-    
-    def __init__(self, driver: WebviewDriver, **page_info) -> None:
-        page_str = str(self)
-        def on_ws_state_change(value):
-            if not value:
-                logger.info("%s link destory" % page_str)
-        self.on_ws_state_change = on_ws_state_change
-        self.driver.ws.on("ConnectionStateChange", self.on_ws_state_change)
+    def get_authorize_settings(self):
+        ...
 
-    def __del__(self):
-        logger.debug("%s del" % str(self))
-        self.driver.ws.remove_listener("ConnectionStateChange", self.on_ws_state_change)
+    def back_from_authorize_setting(self):
+        ...
 
-    def __str__(self) -> str:
-        return "[%s]%s" % (
-                    self.page_info.get("webviewId"),
-                    f"{self.driver.title.path}[{'visible' if self.driver.title.visible else 'invisible'}]"
-                    if self.driver.title
-                    else "unknow",
-                )
-    
-    def evaluate(self, expression, **kwargs):
-        return self.driver.evaluate(expression, **kwargs)
-    
-class H5Page(WebviewPage):
-    PAGE_INFO_MAP = {}  # webviewId -> page_info
-    driver: H5Driver
-
-    def __str__(self) -> str:
-        return "[%s]%s[%s]" % (
-                    self.page_info.get("webviewId"),
-                    self.driver.title,
-                    self.driver.url
-                )
-
-class SkylinePage(object):
-    def __init__(self, driver: SkylineDriver, **page_info) -> None:
-        self.driver = driver
-        self.page_info = page_info
-    
-    def __str__(self) -> str:
-        return "[%s]%s[skyline]" % (
-                    self.page_info.get("webviewId"),
-                    f"{self.page_info['route']}"
-                )
+    def authorize_page_checkbox_enable(self, name, enable):
+        ...
 
-    def evaluate(self, expression, **kwargs):
-        return self.driver.evaluate(expression, **kwargs)
+    # back to miniprogram use
+    def _get_current_activity(self):
+        return ""
+
+    def _is_in_wechat(self, activity: str):
+        return True
+
+    def _is_in_wechat_main(self, activity: str):
+        return False
+
+    def _is_in_miniprogram(self, activity: str):
+        """
+        需要甄别: 插件页面、webview页面、普通页面
+        """
+        return True
+
+    def _is_in_target_miniprogram(self, appid: str):
+        return True
+
+    def _close_miniprogram(self):
+        return True
+
+    def _get_any_modal(self, confirm=False):
+        return None
+
+    def _is_in_payment(self):
+        return False
+
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/officialaccount.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/officialaccount.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-07-11 15:35:44
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-07-21 18:37:14
+LastEditTime: 2023-11-30 21:22:34
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/officialaccount.py
 Description: 公众号实例
 '''
 import time
 import json
 import typing
 import threading
@@ -51,16 +51,16 @@
 
     def _init_tabs(self, processpid) -> typing.List[Tab]:
         result = []
         for sock_name, pid in self._get_debug_sock_name().items():  # 可能有多个remote debug port, 找出属于小程序的那个. sock_cache至少有两个才不
             # 优化点:
             # 1. appservice在一个sock中, 微信不重启不会改变.
             # 2. webview在一个sock中, 不重启也不会改变
-            self.logger.debug(f"find debugger port for {sock_name}")
-            if pid == str(processpid).strip():
+            self.logger.debug(f"find debugger port for {sock_name}, pid: {pid}, target pid: {processpid}")
+            if pid == str(processpid).strip() or processpid is None: # 没有检测到目标pid, 全部都当符合条件
                 retry_cnt = 1  # webview title有可能会处于initial状态, 需要至少等一个visible/invisible才可以继续
                 while retry_cnt:
                     retry_cnt -= 1
                     tabs, tcp_port = self.get_tabs_by_sock(sock_name)
                     self.logger.info(
                         "tabs: %s" % (",".join([tab["title"] for tab in tabs]))
                     )
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/basepage.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/basepage.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,60 @@
 '''
 Author: yopofeng
 Date: 2023-09-27 23:41:11
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-31 17:47:53
+LastEditTime: 2024-02-29 11:05:40
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/pages.py
 Description: 定义各种page实例
 
 Copyright (c) 2023 by ${git_name_email}, All Rights Reserved. 
 '''
 
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 import re
 from typing import Union, List, Mapping
-
+from ..utils import Object
+from json import JSONEncoder
 
 @dataclass  
 class BasePage:
     title: str = ''
     url: str = ''
 
 class NormalPage(BasePage):
     unique_id = None
     empty = False
 
+    def __init__(self, title='', url='', **kwargs):
+        super().__init__(title, url)
+        self.ext_info = Object()
+        self.update_ext_info(kwargs)
+
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, NormalPage):
             return False
         return self.unique_id == __value.unique_id
     
     def __str__(self) -> str:
         return f"id: {self.unique_id}, type: {self.__class__.__name__}, url: {self.url}, title: {self.title}"
 
+    def update_ext_info(self, info: dict):
+        for k, v in info.items():
+            if v is not None:
+                self.ext_info[k] = v
+
 class WebViewPage(NormalPage):
     appid: str = ''
     path: str = ''
-    visible: bool = None
-    initial: bool = False
+    # visible: bool = None
+    # initial: bool = False
 
 class AppServicePage(NormalPage):
     appid = ''
 
+class DataClassJSONEncoder(JSONEncoder):
+    def default(self, o):
+        if isinstance(o, BasePage):
+            return asdict(o)
+        # Let the base class default method raise the TypeError
+        return JSONEncoder.default(self, o)
+
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/chromepage.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/chromepage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 '''
 Author: yopofeng
 Date: 2023-09-27 23:41:11
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-19 11:35:23
+LastEditTime: 2024-02-28 17:09:05
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/pages.py
 Description: 定义各种page实例
 
 Copyright (c) 2023 by ${git_name_email}, All Rights Reserved. 
 '''
 
 from dataclasses import dataclass
+import json
 import re
 from .basepage import BasePage, NormalPage, WebViewPage, AppServicePage
 from typing import Union, List, Mapping
 from ..utils import Object
 
 def reg_match(reg_list, string):
     for reg in reg_list:
@@ -26,14 +27,33 @@
         if string.startswith(state):
             return state
     return None
 
 @dataclass
 class ChromeTab(BasePage):
     webSocketDebuggerUrl: str = ''
+    description: Object = None
+
+    @property
+    def description(self) -> Object:
+        return self._description
+
+    @description.setter
+    def description(self, v):
+        if isinstance(v, Object):
+            self._description = v
+        elif isinstance(v, str):
+            try:
+                self._description = json.loads(v, object_hook=Object)
+            except ValueError:
+                self._description = v
+        elif isinstance(v, dict):
+            self._description = Object(v)
+        else:
+            self._description = v
 
 
 class ChromeNormalPage(ChromeTab, NormalPage):
     def __new__(cls, title, url='', *args, **kwargs):
         if isinstance(title, BasePage):
             return title
         
@@ -48,18 +68,18 @@
                     inst.appid = ts[0]
             elif reg_match(IgnorePage.REG_LIST, title):
                 return None  # 直接不创建实例
         if not inst:
             inst = object.__new__(ChromeNormalPage)
         return inst
 
-    def __init__(self, title: str, url='', webSocketDebuggerUrl='', unique_id=None, *args, **kwargs) -> None:
+    def __init__(self, title: str, url='', webSocketDebuggerUrl='', description=None, *args, unique_id=None, **kwargs) -> None:
         if isinstance(title, ChromeNormalPage):
             return
-        super(ChromeNormalPage, self).__init__(title, url, webSocketDebuggerUrl)
+        super(ChromeNormalPage, self).__init__(title, url, webSocketDebuggerUrl, description)
         self.unique_id = unique_id 
         self.empty = (title == "about:blank" or url == "about:blank")
         self.ext_info = Object(kwargs)
 
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, ChromeNormalPage):
             return False
@@ -87,16 +107,16 @@
         self.initial = True if state == "INITIAL" else False
 
 
 class ChromeAppServicePage(ChromeNormalPage):
     REG_LIST  = [r"\d+:\d+:WxaService", r"wx[a-z0-9]+:\d+:service"]
     appid = None
     tcp_port = ''
-    def __init__(self, title: str, url='', webSocketDebuggerUrl='', unique_id=None, tcp_port='', *args, **kwargs) -> None:
-        super().__init__(title, url, webSocketDebuggerUrl, *args, **kwargs)
+    def __init__(self, title: str, url='', webSocketDebuggerUrl='', *args, unique_id=None, tcp_port='', **kwargs) -> None:
+        super().__init__(title, url, webSocketDebuggerUrl, *args, unique_id=unique_id, **kwargs)
         self.tcp_port = tcp_port
         self.webSocketDebuggerUrl = "ws://127.0.0.1:%s/page/%s" % (tcp_port, title)
 
     @property
     def unique_id(self):
         return f"{self.ext_info.sock_name}:{self.title}"
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/pages/safaripage.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/pages/safaripage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,104 +1,107 @@
 '''
 Author: yopofeng
 Date: 2023-09-27 23:41:11
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-10-31 21:11:55
+LastEditTime: 2024-02-28 17:44:54
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/driver/pages.py
 Description: 定义各种page实例
 
 Copyright (c) 2023 by ${git_name_email}, All Rights Reserved. 
 '''
 
 from dataclasses import dataclass
 from .basepage import BasePage, NormalPage, WebViewPage, AppServicePage
 import re
 from typing import Union, List, Mapping, TYPE_CHECKING
-from ..utils import Object
+from ..utils import Object, reg_search
 from pymobiledevice3.services.webinspector import Page as _Page, WirTypes
-
-def reg_match(reg_list, string):
-    m = None
-    for reg in reg_list:
-        m = re.match(reg, string)
-        if m:
-            break
-    return m
+import json
+from ..logger import logger
 
 def state_match(states, string: str) -> str:
     for state in states:
         if string.startswith(state):
             return state
     return None
 
 # 重构一下page实例
 @dataclass
 class Page(BasePage, _Page):
+    connection_id_: str = ""
     appid_ = None
     @classmethod
     def from_page_dictionary(cls, page_dict: Mapping) -> 'Page':
         p: Page = super(Page, cls).from_page_dictionary(page_dict)
         if p.type_ == WirTypes.JAVASCRIPT:
             p.web_title = page_dict['WIRTitleKey']
+            if "WIRConnectionIdentifierKey" in page_dict:
+                p.connection_id_ = page_dict["WIRConnectionIdentifierKey"]
         if 'WIRTitleKey' in page_dict:
             p.title = page_dict['WIRTitleKey']
         if 'WIRURLKey' in page_dict:
             p.url = page_dict['WIRURLKey']
+        # for test
+        # if "WIRConnectionIdentifierKey" in page_dict:
+        #     logger.info(json.dumps(page_dict, indent=2))
         return p
 
     def __str__(self):
         return f'id: {self.id_}[{self.type_}], title: {self.title}, url: {self.url}'
 
 
 class SafariNormalPage(NormalPage):
     page: Page
-    def __new__(cls, page: Page or BasePage, *args, **kwargs):
+    def __new__(cls, page: Union[Page, BasePage], *args, **kwargs):
         if not isinstance(page, Page):
             return page
         
         inst = None
         if page.type_ == WirTypes.JAVASCRIPT:
-            m = reg_match(SafariAppServicePage.REG_LIST, page.title)
+            m = reg_search(SafariAppServicePage.REG_LIST, page.title)
             if m:
                 inst = object.__new__(SafariAppServicePage)
                 inst.appid = m.group("appid")
-            elif reg_match(IgnorePage.REG_LIST, page.title):
+            elif reg_search(IgnorePage.REG_LIST, page.title):
                 return None
         elif page.type_ == WirTypes.WEB_PAGE:
-            m = reg_match(SafariWebViewPage.REG_LIST, page.url)
+            m = reg_search(SafariWebViewPage.REG_LIST, page.url)
             if m:
                 inst = object.__new__(SafariWebViewPage)
                 inst.appid = m.group("appid")
-            elif reg_match(IgnorePage.REG_LIST, page.url):
+            elif reg_search(IgnorePage.REG_LIST, page.url):
                 return None
         if inst is None:
             inst = object.__new__(SafariNormalPage)
         inst.page = page
         return inst
 
     def __init__(self, page: Page, *args, **kwargs):
         super().__init__(page.title, page.url)
         self.appid_ = page.appid_
         self.id_ = page.id_
         self.unique_id = page.id_
-        self.ext_info = Object(kwargs)
+        self.ext_info = Object()
+        self.update_ext_info(kwargs)
 
     def __eq__(self, __value: object) -> bool:
         if not isinstance(__value, SafariNormalPage):
             return False
         return self.unique_id == __value.unique_id
 
 
+
 class SafariWebViewPage(SafariNormalPage, WebViewPage):
-    REG_LIST = [ r"^https://servicewechat\.com/(?P<appid>wx[a-z0-9]+)", ]
+    REG_LIST = [ re.compile(r"^https://servicewechat\.com/(?P<appid>wx[a-z0-9]+)"), re.compile(r"^https://servicewechat\.com/(?P<appid>preload)/page-frame.html")]
     appid = None
 
 class SafariAppServicePage(SafariNormalPage):
-    REG_LIST = [ r".*Appid\[(?P<appid>wx[a-z0-9]+)\]", ]
+    REG_LIST = [ re.compile(r"Appid\[(?P<appid>wx[a-z0-9]+)\]"), ]
     appid = None
+    type_ = None  # wechat_mp_inspector.inspector.ioswxainspector.INSPECTORS
 
 class IgnorePage(SafariNormalPage):
-    REG_LIST = [r".*Appid\[Preload\]", r"https://servicewechat\.com/preload"]
+    REG_LIST = [re.compile(r"Appid\[Preload\]"), re.compile(r"https://servicewechat\.com/preload"), re.compile(f"^file:///")]
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/baseprotocol.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/baseprotocol.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-11 17:25:44
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-09-21 11:46:48
+LastEditTime: 2024-02-28 17:45:06
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/protocol/baseprotocol.py
 Description: 协议类, 定义生成指令和解析事件的方法
 '''
 import abc
+from typing import Union
 from ..command import CommandType, Commands, Command, AsyncCommand
 from ..event import BaseEvent
 
 class BaseProtocol(metaclass=abc.ABCMeta):
     def __init__(self, inspector=None) -> None:
         self._inspector = inspector
 
     async def init(self):
         """需要进行异步初始化的操作"""
         pass
 
     @abc.abstractmethod
-    def get_command(self, command: str or Commands, params: dict, *, sync=True, **kwargs) -> CommandType: pass
+    def get_command(self, command: Union[str, Commands], params: dict, *, sync=True, **kwargs) -> CommandType: pass
     @abc.abstractmethod
     def parse_event(self, message: dict) -> BaseEvent: pass
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/basesession.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/basesession.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-22 18:52:16
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-13 10:54:59
+LastEditTime: 2024-02-28 19:04:26
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/protocol/basesession.py
 Description: 定义协议session
 '''
 import abc
 import typing
+from typing import Union
 import threading
 from .baseprotocol import BaseProtocol, CommandType, BaseEvent, Command, AsyncCommand
 from .protocolcommand import ProtocolCommand
 from ..connection.baseconn import BaseConnection
 from ..command import CommandType
 from ..event import BaseEvent
 from ..logger import logger
 
 class BaseSession(metaclass=abc.ABCMeta):
     id_: str
     @abc.abstractmethod
-    def send_command(self, data: dict or CommandType): pass
+    def send_command(self, data: Union[dict, CommandType]): pass
 
     @abc.abstractmethod
-    def on(self, event: str or BaseEvent, callback: typing.Callable): pass
+    def on(self, event: Union[str, BaseEvent], callback: typing.Callable): pass
 
     @abc.abstractmethod
     def close(self): ...
 
     @abc.abstractmethod
-    def remove_listener(self, event: str or BaseEvent, callback: typing.Callable): ...
+    def remove_listener(self, event: Union[str, BaseEvent], callback: typing.Callable): ...
 
     @abc.abstractmethod
     def remove_all_listeners(self): ...
 
 
 class BaseWebkitSession(BaseSession):
     protocol: BaseProtocol
     def __init__(self, session_id: str, connection: BaseConnection) -> None:
         self.id_ = session_id
         self._id = str(id(self))
         self._msg_id_lock = threading.Lock()
-        self._msg_id = 1
+        # start with 1
+        # self._msg_id = 1
+        # start with id
+        self._msg_id = int(self._id[-3:])
         self.connection = connection
         self.logger = getattr(connection, "logger", logger)
+        self._max_timeout = None
         # connection采用单实例模式, 使用链接的id可以避免id重复问题
         self._use_conn_id = hasattr(self.connection, "get_command_id")
 
+    def set_max_timeout(self, max_timeout: int):
+        self._max_timeout = max_timeout
+
     def get_command_id(self):
         """生成命令id
 
         :return int: 唯一的命令id
         """
         if self._use_conn_id:
             return self.connection.get_command_id()
         with self._msg_id_lock:
             self._msg_id += 1
             return self._msg_id
         
-    def _gen_command(self, command: str or ProtocolCommand or CommandType, params: dict=None, max_timeout=None, sync=True, ignore_response=False) -> CommandType:
+    def _gen_command(self, command: Union[str, ProtocolCommand, CommandType], params: dict=None, max_timeout=None, sync=True, ignore_response=False) -> CommandType:
         cmd = None
+        if max_timeout is None:
+            max_timeout = self._max_timeout
         if sync:
             if isinstance(command, Command):
                 cmd = command
             elif isinstance(command, AsyncCommand):
                 cmd = Command(command.method, command.params, desc=command.desc, max_timeout=max_timeout)
             elif isinstance(command, ProtocolCommand):
                 cmd = Command(command._method, command._arguments, max_timeout=max_timeout)
@@ -84,7 +94,10 @@
                     cmd = Command(command, params, max_timeout=max_timeout)
                 else:
                     cmd = AsyncCommand(command, params, ignore_response=ignore_response)
         if not cmd.id:
             cmd.id = self.get_command_id()
         cmd.conn_id = self._id
         return cmd
+
+    async def _send_command(self, data: Union[dict, CommandType]):
+        raise NotImplementedError("unsupport async send command")
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/basewebkit.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/basewebkit.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/cdp.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/cdp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-09-11 19:39:54
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-11-14 16:31:45
+LastEditTime: 2024-02-28 17:46:08
 FilePath: /wechat-mp-inspector/wechat_mp_inspector/protocol/cdp.py
 Description: 定义Chrome DevTools协议: https://chromedevtools.github.io/devtools-protocol/
 '''
 import threading
 import json
-from typing import Tuple, Any, Callable, Dict
+from typing import Tuple, Any, Callable, Dict, Union
 from .basesession import BaseWebkitSession, ProtocolCommand
 from ..connection.websocketconn import WebSocketConnection, STATE, lock_init
 from ..pages.chromepage import *
 from .basewebkit import ChromeInspectorProtocol, Command, CDP
 from .baseprotocol import BaseProtocol, CommandType, BaseEvent, Command, AsyncCommand
 from ..utils import get_url_path
 from ..exception import InspectorDetachedError
@@ -55,15 +55,15 @@
         super().__init__(
             debugger_url,
             *args,
             unique_id=unique_id,
             auto_reconnect=auto_reconnect,
             **kwargs
         )
-        self.ignore_method = set()
+        # self.ignore_method = set()
         self.protocol = ChromeInspectorProtocol()
         self.detached = False
         self.on("Inspector.detached", self.inspector_detached)
 
     def _reconnect(self, optime=None, *args):
         if self.detached:
             raise InspectorDetachedError(self.detached)
@@ -106,15 +106,15 @@
     connection: CDPConnection
     def __init__(self, connection: CDPConnection, id_, page: ChromeNormalPage, refresh_page_handler=None) -> None:
         super().__init__(id_, connection)
         self.protocol = connection.protocol
         self.page = page
         self.refresh_page_handler = refresh_page_handler
 
-    def send_command(self, command: str or ProtocolCommand or CommandType, params: dict = None, *, sync=True, **kwargs):
+    def send_command(self, command: Union[str, ProtocolCommand, CommandType], params: dict = None, *, sync=True, **kwargs):
         """发送命令, 并等待回复"""
         cmd = self._gen_command(command, params, sync=sync, **kwargs)
         try:
             return self.connection.send_command(cmd)
         except ConnectionAbortedError as e:
             if not self.refresh_page_handler:
                 raise
@@ -130,19 +130,19 @@
                     raise
                 # 刷新成功了
                 self.page = new_page
                 self.connection = CDPConnection(new_page.webSocketDebuggerUrl, unique_id=new_page.unique_id)
                 return self.connection.send_command(cmd)
             raise
 
-    def on(self, event: str or BaseEvent, callback: Callable):
+    def on(self, event: Union[str, BaseEvent], callback: Callable):
         """监听事件"""
         return self.connection.on(event, callback)
     
-    def remove_listener(self, event: str or BaseEvent, callback: Callable):
+    def remove_listener(self, event: Union[str, BaseEvent], callback: Callable):
         return self.connection.remove_listener(event, callback)
 
     def remove_all_listeners(self):
         return self.connection.remove_all_listeners()
 
     def close(self):
         self.connection.close()
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/protocolcommand.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/protocolcommand.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/protocol/protocoltypes.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/protocol/protocoltypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,56 +251,72 @@
     @dataclass
     class enable(ProtocolCommand):
         """Enables animation domain notifications."""
         pass
     
     @dataclass
     class getCurrentTime(ProtocolCommand):
-        """Returns the current time of the an animation."""
+        """[Just CDP] Returns the current time of the an animation."""
         id: str
     
     @dataclass
     class getPlaybackRate(ProtocolCommand):
-        """Gets the playback rate of the document timeline."""
+        """[Just CDP] Gets the playback rate of the document timeline."""
         pass
     
     @dataclass
     class releaseAnimations(ProtocolCommand):
-        """Releases a set of animations to no longer be manipulated."""
+        """[Just CDP] Releases a set of animations to no longer be manipulated."""
         animations: list
     
     @dataclass
     class resolveAnimation(ProtocolCommand):
         """Gets the remote object of the Animation."""
         animationId: str
+        objectGroup: str = OPTIONAL
     
     @dataclass
     class seekAnimations(ProtocolCommand):
-        """Seek a set of animations to a particular time within each animation."""
+        """[Just CDP] Seek a set of animations to a particular time within each animation."""
         animations: list
         currentTime: int
     
     @dataclass
     class setPaused(ProtocolCommand):
-        """Sets the paused state of a set of animations."""
+        """[Just CDP] Sets the paused state of a set of animations."""
         animations: list
         paused: bool
     
     @dataclass
     class setPlaybackRate(ProtocolCommand):
-        """Sets the playback rate of the document timeline."""
+        """[Just CDP] Sets the playback rate of the document timeline."""
         playbackRate: int
     
     @dataclass
     class setTiming(ProtocolCommand):
-        """Sets the timing of an animation node."""
+        """[Just CDP] Sets the timing of an animation node."""
         animationId: str
         duration: int
         delay: int
     
+    @dataclass
+    class requestEffectTarget(ProtocolCommand):
+        """[Just WIP] Gets the `DOM.NodeId` for the target of the effect of the animation with the given `AnimationId`."""
+        animationId: Animation.AnimationId
+    
+    @dataclass
+    class startTracking(ProtocolCommand):
+        """[Just WIP] Start tracking animations. This will produce a `trackingStart` event."""
+        pass
+    
+    @dataclass
+    class stopTracking(ProtocolCommand):
+        """[Just WIP] Stop tracking animations. This will produce a `trackingComplete` event."""
+        pass
+    
 
 @domainclass
 class Audits:
     """[Just CDP][Experimental] Audits domain allows investigation of page violations and possible improvements."""
     class AffectedCookie:
         """Information about a cookie that is affected by an inspector issue."""
         name: str
@@ -726,117 +742,127 @@
         extensions: list
     
     class extensionsDisabled(BaseEvent):
         extensionIds: list
     
     @dataclass
     class setPermission(ProtocolCommand):
-        """Set permission settings for given origin."""
+        """[Just CDP] Set permission settings for given origin."""
         permission: Browser.PermissionDescriptor
         setting: Browser.PermissionSetting
         origin: str = OPTIONAL
         browserContextId: Browser.BrowserContextID = OPTIONAL
     
     @dataclass
     class grantPermissions(ProtocolCommand):
-        """Grant specific permissions to the given origin and reject all others."""
+        """[Just CDP] Grant specific permissions to the given origin and reject all others."""
         permissions: list
         origin: str = OPTIONAL
         browserContextId: Browser.BrowserContextID = OPTIONAL
     
     @dataclass
     class resetPermissions(ProtocolCommand):
-        """Reset all permission management for all origins."""
+        """[Just CDP] Reset all permission management for all origins."""
         browserContextId: Browser.BrowserContextID = OPTIONAL
     
     @dataclass
     class setDownloadBehavior(ProtocolCommand):
-        """Set the behavior when downloading a file."""
+        """[Just CDP] Set the behavior when downloading a file."""
         behavior: str
         browserContextId: Browser.BrowserContextID = OPTIONAL
         downloadPath: str = OPTIONAL
         eventsEnabled: bool = OPTIONAL
     
     @dataclass
     class cancelDownload(ProtocolCommand):
-        """Cancel a download if in progress"""
+        """[Just CDP] Cancel a download if in progress"""
         guid: str
         browserContextId: Browser.BrowserContextID = OPTIONAL
     
     @dataclass
     class close(ProtocolCommand):
-        """Close browser gracefully."""
+        """[Just CDP] Close browser gracefully."""
         pass
     
     @dataclass
     class crash(ProtocolCommand):
-        """Crashes browser on the main thread."""
+        """[Just CDP] Crashes browser on the main thread."""
         pass
     
     @dataclass
     class crashGpuProcess(ProtocolCommand):
-        """Crashes GPU process."""
+        """[Just CDP] Crashes GPU process."""
         pass
     
     @dataclass
     class getVersion(ProtocolCommand):
-        """Returns version information."""
+        """[Just CDP] Returns version information."""
         pass
     
     @dataclass
     class getBrowserCommandLine(ProtocolCommand):
-        """Returns the command line switches for the browser process if, and only if
+        """[Just CDP] Returns the command line switches for the browser process if, and only if
 --enable-automation is on the commandline."""
         pass
     
     @dataclass
     class getHistograms(ProtocolCommand):
-        """Get Chrome histograms."""
+        """[Just CDP] Get Chrome histograms."""
         query: str = OPTIONAL
         delta: bool = OPTIONAL
     
     @dataclass
     class getHistogram(ProtocolCommand):
-        """Get a Chrome histogram by name."""
+        """[Just CDP] Get a Chrome histogram by name."""
         name: str
         delta: bool = OPTIONAL
     
     @dataclass
     class getWindowBounds(ProtocolCommand):
-        """Get position and size of the browser window."""
+        """[Just CDP] Get position and size of the browser window."""
         windowId: Browser.WindowID
     
     @dataclass
     class getWindowForTarget(ProtocolCommand):
-        """Get the browser window that contains the devtools target."""
+        """[Just CDP] Get the browser window that contains the devtools target."""
         targetId: Target.TargetID = OPTIONAL
     
     @dataclass
     class setWindowBounds(ProtocolCommand):
-        """Set position and/or size of the browser window."""
+        """[Just CDP] Set position and/or size of the browser window."""
         windowId: Browser.WindowID
         bounds: Browser.Bounds
     
     @dataclass
     class setDockTile(ProtocolCommand):
-        """Set dock tile details, platform-specific."""
+        """[Just CDP] Set dock tile details, platform-specific."""
         badgeLabel: str = OPTIONAL
         image: str = OPTIONAL
     
     @dataclass
     class executeBrowserCommand(ProtocolCommand):
-        """Invoke custom browser commands used by telemetry."""
+        """[Just CDP] Invoke custom browser commands used by telemetry."""
         commandId: Browser.BrowserCommandId
     
     @dataclass
     class addPrivacySandboxEnrollmentOverride(ProtocolCommand):
-        """Allows a site to use privacy sandbox features that require enrollment
+        """[Just CDP] Allows a site to use privacy sandbox features that require enrollment
 without the site actually being enrolled. Only supported on page targets."""
         url: str
     
+    @dataclass
+    class enable(ProtocolCommand):
+        """[Just WIP] Enables Browser domain events."""
+        pass
+    
+    @dataclass
+    class disable(ProtocolCommand):
+        """[Just WIP] Disables Browser domain events."""
+        pass
+    
 
 @domainclass
 class CSS:
     """This domain exposes CSS read/write operations. All CSS objects (stylesheets, rules, and styles)
 have an associated `id` used in subsequent operations on the related object. Each object type has
 a specific `id` structure, and those are not interchangeable between objects of different kinds.
 CSS objects can be loaded using the `get*ForNode()` calls (which accept a DOM node id). A client
@@ -1190,18 +1216,19 @@
     @dataclass
     class addRule(ProtocolCommand):
         """Inserts a new rule with the given `ruleText` in a stylesheet with given `styleSheetId`, at the
 position specified by `location`."""
         styleSheetId: CSS.StyleSheetId
         ruleText: str
         location: CSS.SourceRange
+        selector: str
     
     @dataclass
     class collectClassNames(ProtocolCommand):
-        """Returns all class names from specified stylesheet."""
+        """[Just CDP] Returns all class names from specified stylesheet."""
         styleSheetId: CSS.StyleSheetId
     
     @dataclass
     class createStyleSheet(ProtocolCommand):
         """Creates a new special "via-inspector" stylesheet in the frame with given `frameId`."""
         frameId: Page.FrameId
     
@@ -1221,14 +1248,15 @@
         """Ensures that the given node will have specified pseudo-classes whenever its style is computed by
 the browser."""
         nodeId: DOM.NodeId
         forcedPseudoClasses: list
     
     @dataclass
     class getBackgroundColors(ProtocolCommand):
+        """[Just CDP]"""
         nodeId: DOM.NodeId
     
     @dataclass
     class getComputedStyleForNode(ProtocolCommand):
         """Returns the computed style for a DOM node identified by `nodeId`."""
         nodeId: DOM.NodeId
     
@@ -1238,137 +1266,182 @@
 attributes) for a DOM node identified by `nodeId`."""
         nodeId: DOM.NodeId
     
     @dataclass
     class getMatchedStylesForNode(ProtocolCommand):
         """Returns requested styles for a DOM node identified by `nodeId`."""
         nodeId: DOM.NodeId
+        includePseudo: bool = OPTIONAL
+        includeInherited: bool = OPTIONAL
     
     @dataclass
     class getMediaQueries(ProtocolCommand):
-        """Returns all media queries parsed by the rendering engine."""
+        """[Just CDP] Returns all media queries parsed by the rendering engine."""
         pass
     
     @dataclass
     class getPlatformFontsForNode(ProtocolCommand):
-        """Requests information about platform fonts which we used to render child TextNodes in the given
+        """[Just CDP] Requests information about platform fonts which we used to render child TextNodes in the given
 node."""
         nodeId: DOM.NodeId
     
     @dataclass
     class getStyleSheetText(ProtocolCommand):
         """Returns the current textual content for a stylesheet."""
         styleSheetId: CSS.StyleSheetId
     
     @dataclass
     class getLayersForNode(ProtocolCommand):
-        """Returns all layers parsed by the rendering engine for the tree scope of a node.
+        """[Just CDP] Returns all layers parsed by the rendering engine for the tree scope of a node.
 Given a DOM element identified by nodeId, getLayersForNode returns the root
 layer for the nearest ancestor document or shadow root. The layer root contains
 the full layer tree for the tree scope and their ordering."""
         nodeId: DOM.NodeId
     
     @dataclass
     class trackComputedStyleUpdates(ProtocolCommand):
-        """Starts tracking the given computed styles for updates. The specified array of properties
+        """[Just CDP] Starts tracking the given computed styles for updates. The specified array of properties
 replaces the one previously specified. Pass empty array to disable tracking.
 Use takeComputedStyleUpdates to retrieve the list of nodes that had properties modified.
 The changes to computed style properties are only tracked for nodes pushed to the front-end
 by the DOM agent. If no changes to the tracked properties occur after the node has been pushed
 to the front-end, no updates will be issued for the node."""
         propertiesToTrack: list
     
     @dataclass
     class takeComputedStyleUpdates(ProtocolCommand):
-        """Polls the next batch of computed style updates."""
+        """[Just CDP] Polls the next batch of computed style updates."""
         pass
     
     @dataclass
     class setEffectivePropertyValueForNode(ProtocolCommand):
-        """Find a rule with the given active property for the given node and set the new value for this
+        """[Just CDP] Find a rule with the given active property for the given node and set the new value for this
 property"""
         nodeId: DOM.NodeId
         propertyName: str
         value: str
     
     @dataclass
     class setKeyframeKey(ProtocolCommand):
-        """Modifies the keyframe rule key text."""
+        """[Just CDP] Modifies the keyframe rule key text."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         keyText: str
     
     @dataclass
     class setMediaText(ProtocolCommand):
-        """Modifies the rule selector."""
+        """[Just CDP] Modifies the rule selector."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         text: str
     
     @dataclass
     class setContainerQueryText(ProtocolCommand):
-        """Modifies the expression of a container query."""
+        """[Just CDP] Modifies the expression of a container query."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         text: str
     
     @dataclass
     class setSupportsText(ProtocolCommand):
-        """Modifies the expression of a supports at-rule."""
+        """[Just CDP] Modifies the expression of a supports at-rule."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         text: str
     
     @dataclass
     class setScopeText(ProtocolCommand):
-        """Modifies the expression of a scope at-rule."""
+        """[Just CDP] Modifies the expression of a scope at-rule."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         text: str
     
     @dataclass
     class setRuleSelector(ProtocolCommand):
         """Modifies the rule selector."""
         styleSheetId: CSS.StyleSheetId
         range: CSS.SourceRange
         selector: str
+        ruleId: CSS.CSSRuleId
     
     @dataclass
     class setStyleSheetText(ProtocolCommand):
         """Sets the new stylesheet text."""
         styleSheetId: CSS.StyleSheetId
         text: str
     
     @dataclass
     class setStyleTexts(ProtocolCommand):
-        """Applies specified style edits one after another in the given order."""
+        """[Just CDP] Applies specified style edits one after another in the given order."""
         edits: list
     
     @dataclass
     class startRuleUsageTracking(ProtocolCommand):
-        """Enables the selector recording."""
+        """[Just CDP] Enables the selector recording."""
         pass
     
     @dataclass
     class stopRuleUsageTracking(ProtocolCommand):
-        """Stop tracking rule usage and return the list of rules that were used since last call to
+        """[Just CDP] Stop tracking rule usage and return the list of rules that were used since last call to
 `takeCoverageDelta` (or since start of coverage instrumentation)."""
         pass
     
     @dataclass
     class takeCoverageDelta(ProtocolCommand):
-        """Obtain list of rules that became used since last call to this method (or since start of coverage
+        """[Just CDP] Obtain list of rules that became used since last call to this method (or since start of coverage
 instrumentation)."""
         pass
     
     @dataclass
     class setLocalFontsEnabled(ProtocolCommand):
-        """Enables/disables rendering of local CSS fonts (enabled by default)."""
+        """[Just CDP] Enables/disables rendering of local CSS fonts (enabled by default)."""
         enabled: bool
     
+    @dataclass
+    class getFontDataForNode(ProtocolCommand):
+        """[Just WIP] Returns the primary font of the computed font cascade for a DOM node identified by <code>nodeId</code>."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class getAllStyleSheets(ProtocolCommand):
+        """[Just WIP] Returns metainfo entries for all known stylesheets."""
+        pass
+    
+    @dataclass
+    class getStyleSheet(ProtocolCommand):
+        """[Just WIP] Returns stylesheet data for the specified <code>styleSheetId</code>."""
+        styleSheetId: CSS.StyleSheetId
+    
+    @dataclass
+    class setStyleText(ProtocolCommand):
+        """[Just WIP] Sets the new <code>text</code> for the respective style."""
+        styleId: CSS.CSSStyleId
+        text: str
+    
+    @dataclass
+    class setGroupingHeaderText(ProtocolCommand):
+        """[Just WIP] Modifies an @rule grouping's header text."""
+        ruleId: CSS.CSSRuleId
+        headerText: str
+    
+    @dataclass
+    class getSupportedCSSProperties(ProtocolCommand):
+        """[Just WIP] Returns all supported CSS property names."""
+        pass
+    
+    @dataclass
+    class getSupportedSystemFontFamilyNames(ProtocolCommand):
+        """[Just WIP] Returns all supported system font family names."""
+        pass
+    
+    @dataclass
+    class setLayoutContextTypeChangedMode(ProtocolCommand):
+        """[Just WIP] Change how layout context type changes are handled for nodes. When the new mode would observe nodes the frontend has not yet recieved, those nodes will be sent to the frontend immediately."""
+        mode: CSS.LayoutContextTypeChangedMode
+    
 
 @domainclass
 class CacheStorage:
     """[Just CDP][Experimental]"""
     CacheId: str
     CachedResponseType: str
     class DataEntry:
@@ -1783,59 +1856,59 @@
         """Called when an element enters/exits a power efficient playback state."""
         nodeId: DOM.NodeId
         timestamp: Network.Timestamp
         isPowerEfficient: bool
     
     @dataclass
     class collectClassNamesFromSubtree(ProtocolCommand):
-        """Collects class names for the node with given id and all of it's child nodes."""
+        """[Just CDP] Collects class names for the node with given id and all of it's child nodes."""
         nodeId: DOM.NodeId
     
     @dataclass
     class copyTo(ProtocolCommand):
-        """Creates a deep copy of the specified node and places it into the target container before the
+        """[Just CDP] Creates a deep copy of the specified node and places it into the target container before the
 given anchor."""
         nodeId: DOM.NodeId
         targetNodeId: DOM.NodeId
         insertBeforeNodeId: DOM.NodeId = OPTIONAL
     
     @dataclass
     class describeNode(ProtocolCommand):
-        """Describes node given its id, does not require domain to be enabled. Does not start tracking any
+        """[Just CDP] Describes node given its id, does not require domain to be enabled. Does not start tracking any
 objects, can be used for automation."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
         depth: int = OPTIONAL
         pierce: bool = OPTIONAL
     
     @dataclass
     class scrollIntoViewIfNeeded(ProtocolCommand):
-        """Scrolls the specified rect of the given node into view if not already visible.
+        """[Just CDP] Scrolls the specified rect of the given node into view if not already visible.
 Note: exactly one between nodeId, backendNodeId and objectId should be passed
 to identify the node."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
         rect: DOM.Rect = OPTIONAL
     
     @dataclass
     class disable(ProtocolCommand):
-        """Disables DOM agent for the given page."""
+        """[Just CDP] Disables DOM agent for the given page."""
         pass
     
     @dataclass
     class discardSearchResults(ProtocolCommand):
         """Discards search results from the session with the given id. `getSearchResults` should no longer
 be called for that search."""
         searchId: str
     
     @dataclass
     class enable(ProtocolCommand):
-        """Enables DOM agent for the given page."""
+        """[Just CDP] Enables DOM agent for the given page."""
         includeWhitespace: str = OPTIONAL
     
     @dataclass
     class focus(ProtocolCommand):
         """Focuses the given element."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
@@ -1844,52 +1917,52 @@
     @dataclass
     class getAttributes(ProtocolCommand):
         """Returns attributes for the specified node."""
         nodeId: DOM.NodeId
     
     @dataclass
     class getBoxModel(ProtocolCommand):
-        """Returns boxes for the given node."""
+        """[Just CDP] Returns boxes for the given node."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
     
     @dataclass
     class getContentQuads(ProtocolCommand):
-        """Returns quads that describe node position on the page. This method
+        """[Just CDP] Returns quads that describe node position on the page. This method
 might return multiple quads for inline nodes."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
     
     @dataclass
     class getDocument(ProtocolCommand):
         """Returns the root DOM node (and optionally the subtree) to the caller.
 Implicitly enables the DOM domain events for the current target."""
         depth: int = OPTIONAL
         pierce: bool = OPTIONAL
     
     @dataclass
     class getFlattenedDocument(ProtocolCommand):
-        """Returns the root DOM node (and optionally the subtree) to the caller.
+        """[Just CDP] Returns the root DOM node (and optionally the subtree) to the caller.
 Deprecated, as it is not designed to work well with the rest of the DOM agent.
 Use DOMSnapshot.captureSnapshot instead."""
         depth: int = OPTIONAL
         pierce: bool = OPTIONAL
     
     @dataclass
     class getNodesForSubtreeByStyle(ProtocolCommand):
-        """Finds nodes with a given computed style in a subtree."""
+        """[Just CDP] Finds nodes with a given computed style in a subtree."""
         nodeId: DOM.NodeId
         computedStyles: list
         pierce: bool = OPTIONAL
     
     @dataclass
     class getNodeForLocation(ProtocolCommand):
-        """Returns node id at given location. Depending on whether DOM domain is enabled, nodeId is
+        """[Just CDP] Returns node id at given location. Depending on whether DOM domain is enabled, nodeId is
 either returned or not."""
         x: int
         y: int
         includeUserAgentShadowDOM: bool = OPTIONAL
         ignorePointerEventsNone: bool = OPTIONAL
     
     @dataclass
@@ -1897,15 +1970,15 @@
         """Returns node's HTML markup."""
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
     
     @dataclass
     class getRelayoutBoundary(ProtocolCommand):
-        """Returns the id of the nearest ancestor that is a relayout boundary."""
+        """[Just CDP] Returns the id of the nearest ancestor that is a relayout boundary."""
         nodeId: DOM.NodeId
     
     @dataclass
     class getSearchResults(ProtocolCommand):
         """Returns search results from given `fromIndex` to given `toIndex` from the search with the given
 identifier."""
         searchId: str
@@ -1916,20 +1989,31 @@
     class hideHighlight(ProtocolCommand):
         """Hides any highlight."""
         pass
     
     @dataclass
     class highlightNode(ProtocolCommand):
         """Highlights DOM node."""
-        pass
+        highlightConfig: DOM.HighlightConfig
+        nodeId: DOM.NodeId = OPTIONAL
+        objectId: Runtime.RemoteObjectId = OPTIONAL
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+        showRulers: bool = OPTIONAL
     
     @dataclass
     class highlightRect(ProtocolCommand):
         """Highlights given rectangle."""
-        pass
+        x: int
+        y: int
+        width: int
+        height: int
+        color: DOM.RGBAColor = OPTIONAL
+        outlineColor: DOM.RGBAColor = OPTIONAL
+        usePageCoordinates: bool = OPTIONAL
     
     @dataclass
     class markUndoableState(ProtocolCommand):
         """Marks last undoable state."""
         pass
     
     @dataclass
@@ -1941,23 +2025,25 @@
     
     @dataclass
     class performSearch(ProtocolCommand):
         """Searches for a given string in the DOM tree. Use `getSearchResults` to access search results or
 `cancelSearch` to end this search session."""
         query: str
         includeUserAgentShadowDOM: bool = OPTIONAL
+        nodeIds: list = OPTIONAL
+        caseSensitive: bool = OPTIONAL
     
     @dataclass
     class pushNodeByPathToFrontend(ProtocolCommand):
         """Requests that the node is sent to the caller given its path. // FIXME, use XPath"""
         path: str
     
     @dataclass
     class pushNodesByBackendIdsToFrontend(ProtocolCommand):
-        """Requests that a batch of nodes is sent to the caller given their backend node ids."""
+        """[Just CDP] Requests that a batch of nodes is sent to the caller given their backend node ids."""
         backendNodeIds: list
     
     @dataclass
     class querySelector(ProtocolCommand):
         """Executes `querySelector` on a given node."""
         nodeId: DOM.NodeId
         selector: str
@@ -1966,15 +2052,15 @@
     class querySelectorAll(ProtocolCommand):
         """Executes `querySelectorAll` on a given node."""
         nodeId: DOM.NodeId
         selector: str
     
     @dataclass
     class getTopLayerElements(ProtocolCommand):
-        """Returns NodeIds of current top layer elements.
+        """[Just CDP] Returns NodeIds of current top layer elements.
 Top layer is rendered closest to the user within a viewport, therefore its elements always
 appear on top of all other content."""
         pass
     
     @dataclass
     class redo(ProtocolCommand):
         """Re-does the last undone action."""
@@ -2028,33 +2114,33 @@
 attribute value and types in several attribute name/value pairs."""
         nodeId: DOM.NodeId
         text: str
         name: str = OPTIONAL
     
     @dataclass
     class setFileInputFiles(ProtocolCommand):
-        """Sets files for the given file input element."""
+        """[Just CDP] Sets files for the given file input element."""
         files: list
         nodeId: DOM.NodeId = OPTIONAL
         backendNodeId: DOM.BackendNodeId = OPTIONAL
         objectId: Runtime.RemoteObjectId = OPTIONAL
     
     @dataclass
     class setNodeStackTracesEnabled(ProtocolCommand):
-        """Sets if stack traces should be captured for Nodes. See `Node.getNodeStackTraces`. Default is disabled."""
+        """[Just CDP] Sets if stack traces should be captured for Nodes. See `Node.getNodeStackTraces`. Default is disabled."""
         enable: bool
     
     @dataclass
     class getNodeStackTraces(ProtocolCommand):
-        """Gets stack traces associated with a Node. As of now, only provides stack trace for Node creation."""
+        """[Just CDP] Gets stack traces associated with a Node. As of now, only provides stack trace for Node creation."""
         nodeId: DOM.NodeId
     
     @dataclass
     class getFileInfo(ProtocolCommand):
-        """Returns file information for the given
+        """[Just CDP] Returns file information for the given
 File wrapper."""
         objectId: Runtime.RemoteObjectId
     
     @dataclass
     class setInspectedNode(ProtocolCommand):
         """Enables console to refer to the node with given id via $x (see Command Line API for more details
 $x functions)."""
@@ -2081,34 +2167,179 @@
     @dataclass
     class undo(ProtocolCommand):
         """Undoes the last performed action."""
         pass
     
     @dataclass
     class getFrameOwner(ProtocolCommand):
-        """Returns iframe node that owns iframe with the given domain."""
+        """[Just CDP] Returns iframe node that owns iframe with the given domain."""
         frameId: Page.FrameId
     
     @dataclass
     class getContainerForNode(ProtocolCommand):
-        """Returns the query container of the given node based on container query
+        """[Just CDP] Returns the query container of the given node based on container query
 conditions: containerName, physical, and logical axes. If no axes are
 provided, the style container is returned, which is the direct parent or the
 closest element with a matching container-name."""
         nodeId: DOM.NodeId
         containerName: str = OPTIONAL
         physicalAxes: DOM.PhysicalAxes = OPTIONAL
         logicalAxes: DOM.LogicalAxes = OPTIONAL
     
     @dataclass
     class getQueryingDescendantsForContainer(ProtocolCommand):
-        """Returns the descendants of a container query container that have
+        """[Just CDP] Returns the descendants of a container query container that have
 container queries against this container."""
         nodeId: DOM.NodeId
     
+    @dataclass
+    class getSupportedEventNames(ProtocolCommand):
+        """[Just WIP] Gets the list of builtin DOM event names."""
+        pass
+    
+    @dataclass
+    class getDataBindingsForNode(ProtocolCommand):
+        """[Just WIP] Returns all data binding relationships between data that is associated with the node and the node itself."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class getAssociatedDataForNode(ProtocolCommand):
+        """[Just WIP] Returns all data that has been associated with the node and is available for data binding."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class getEventListenersForNode(ProtocolCommand):
+        """[Just WIP] Returns event listeners relevant to the node."""
+        nodeId: DOM.NodeId
+        includeAncestors: bool = OPTIONAL
+    
+    @dataclass
+    class setEventListenerDisabled(ProtocolCommand):
+        """[Just WIP] Enable/disable the given event listener. A disabled event listener will not fire."""
+        eventListenerId: DOM.EventListenerId
+        disabled: bool
+    
+    @dataclass
+    class setBreakpointForEventListener(ProtocolCommand):
+        """[Just WIP] Set a breakpoint on the given event listener."""
+        eventListenerId: DOM.EventListenerId
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class removeBreakpointForEventListener(ProtocolCommand):
+        """[Just WIP] Remove any breakpoints on the given event listener."""
+        eventListenerId: DOM.EventListenerId
+    
+    @dataclass
+    class getAccessibilityPropertiesForNode(ProtocolCommand):
+        """[Just WIP] Returns a dictionary of accessibility properties for the node."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class insertAdjacentHTML(ProtocolCommand):
+        """[Just WIP]"""
+        nodeId: DOM.NodeId
+        position: str
+        html: str
+    
+    @dataclass
+    class setInspectModeEnabled(ProtocolCommand):
+        """[Just WIP] Enters the 'inspect' mode. In this mode, elements that user is hovering over are highlighted. Backend then generates 'inspect' command upon element selection."""
+        enabled: bool
+        highlightConfig: DOM.HighlightConfig = OPTIONAL
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+    
+    @dataclass
+    class setInspectModeEnabled(ProtocolCommand):
+        """[Just WIP] Enters the 'inspect' mode. In this mode, elements that user is hovering over are highlighted. Backend then generates 'inspect' command upon element selection."""
+        enabled: bool
+        highlightConfig: DOM.HighlightConfig = OPTIONAL
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+        showRulers: bool = OPTIONAL
+    
+    @dataclass
+    class highlightQuad(ProtocolCommand):
+        """[Just WIP] Highlights given quad. Coordinates are absolute with respect to the main frame viewport."""
+        quad: DOM.Quad
+        color: DOM.RGBAColor = OPTIONAL
+        outlineColor: DOM.RGBAColor = OPTIONAL
+        usePageCoordinates: bool = OPTIONAL
+    
+    @dataclass
+    class highlightSelector(ProtocolCommand):
+        """[Just WIP] Highlights all DOM nodes that match a given selector. A string containing a CSS selector must be specified."""
+        selectorString: str
+        highlightConfig: DOM.HighlightConfig
+        frameId: str = OPTIONAL
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+    
+    @dataclass
+    class highlightSelector(ProtocolCommand):
+        """[Just WIP] Highlights all DOM nodes that match a given selector. A string containing a CSS selector must be specified."""
+        selectorString: str
+        highlightConfig: DOM.HighlightConfig
+        frameId: str = OPTIONAL
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+        showRulers: bool = OPTIONAL
+    
+    @dataclass
+    class highlightNodeList(ProtocolCommand):
+        """[Just WIP] Highlights each DOM node in the given list."""
+        nodeIds: list
+        highlightConfig: DOM.HighlightConfig
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+    
+    @dataclass
+    class highlightNodeList(ProtocolCommand):
+        """[Just WIP] Highlights each DOM node in the given list."""
+        nodeIds: list
+        highlightConfig: DOM.HighlightConfig
+        gridOverlayConfig: DOM.GridOverlayConfig = OPTIONAL
+        flexOverlayConfig: DOM.FlexOverlayConfig = OPTIONAL
+        showRulers: bool = OPTIONAL
+    
+    @dataclass
+    class highlightFrame(ProtocolCommand):
+        """[Just WIP] Highlights owner element of the frame with given id."""
+        frameId: Network.FrameId
+        contentColor: DOM.RGBAColor = OPTIONAL
+        contentOutlineColor: DOM.RGBAColor = OPTIONAL
+    
+    @dataclass
+    class showGridOverlay(ProtocolCommand):
+        """[Just WIP] Shows a grid overlay for a node that begins a 'grid' layout context. The command has no effect if <code>nodeId</code> is invalid or the associated node does not begin a 'grid' layout context. A node can only have one grid overlay at a time; subsequent calls with the same <code>nodeId</code> will override earlier calls."""
+        nodeId: DOM.NodeId
+        gridOverlayConfig: DOM.GridOverlayConfig
+    
+    @dataclass
+    class hideGridOverlay(ProtocolCommand):
+        """[Just WIP] Hides a grid overlay for a node that begins a 'grid' layout context. The command has no effect if <code>nodeId</code> is specified and invalid, or if there is not currently an overlay set for the <code>nodeId</code>."""
+        nodeId: DOM.NodeId = OPTIONAL
+    
+    @dataclass
+    class showFlexOverlay(ProtocolCommand):
+        """[Just WIP] Shows a flex overlay for a node that begins a 'flex' layout context. The command has no effect if <code>nodeId</code> is invalid or the associated node does not begin a 'flex' layout context. A node can only have one flex overlay at a time; subsequent calls with the same <code>nodeId</code> will override earlier calls."""
+        nodeId: DOM.NodeId
+        flexOverlayConfig: DOM.FlexOverlayConfig
+    
+    @dataclass
+    class hideFlexOverlay(ProtocolCommand):
+        """[Just WIP] Hides a flex overlay for a node that begins a 'flex' layout context. The command has no effect if <code>nodeId</code> is specified and invalid, or if there is not currently an overlay set for the <code>nodeId</code>."""
+        nodeId: DOM.NodeId = OPTIONAL
+    
+    @dataclass
+    class setAllowEditingUserAgentShadowTrees(ProtocolCommand):
+        """[Just WIP] Controls whether any DOM commands work for nodes inside a UserAgent shadow tree."""
+        allow: bool
+    
 
 @domainclass
 class DOMDebugger:
     """DOM debugging allows setting breakpoints on particular DOM operations and events. JavaScript
 execution will stop on these operations as if there was a regular breakpoint set."""
     DOMBreakpointType: str
     CSPViolationType: str
@@ -2125,68 +2356,99 @@
         originalHandler: Runtime.RemoteObject
         backendNodeId: DOM.BackendNodeId
     
     EventBreakpointType: str
 
     @dataclass
     class getEventListeners(ProtocolCommand):
-        """Returns event listeners of the given object."""
+        """[Just CDP] Returns event listeners of the given object."""
         objectId: Runtime.RemoteObjectId
         depth: int = OPTIONAL
         pierce: bool = OPTIONAL
     
     @dataclass
     class removeDOMBreakpoint(ProtocolCommand):
         """Removes DOM breakpoint that was set using `setDOMBreakpoint`."""
         nodeId: DOM.NodeId
         type: DOMDebugger.DOMBreakpointType
     
     @dataclass
     class removeEventListenerBreakpoint(ProtocolCommand):
-        """Removes breakpoint on particular DOM event."""
+        """[Just CDP] Removes breakpoint on particular DOM event."""
         eventName: str
         targetName: str = OPTIONAL
     
     @dataclass
     class removeInstrumentationBreakpoint(ProtocolCommand):
-        """Removes breakpoint on particular native event."""
+        """[Just CDP] Removes breakpoint on particular native event."""
         eventName: str
     
     @dataclass
     class removeXHRBreakpoint(ProtocolCommand):
-        """Removes breakpoint from XMLHttpRequest."""
+        """[Just CDP] Removes breakpoint from XMLHttpRequest."""
         url: str
     
     @dataclass
     class setBreakOnCSPViolation(ProtocolCommand):
-        """Sets breakpoint on particular CSP violations."""
+        """[Just CDP] Sets breakpoint on particular CSP violations."""
         violationTypes: list
     
     @dataclass
     class setDOMBreakpoint(ProtocolCommand):
         """Sets breakpoint on particular operation with DOM."""
         nodeId: DOM.NodeId
         type: DOMDebugger.DOMBreakpointType
+        options: Debugger.BreakpointOptions = OPTIONAL
     
     @dataclass
     class setEventListenerBreakpoint(ProtocolCommand):
-        """Sets breakpoint on particular DOM event."""
+        """[Just CDP] Sets breakpoint on particular DOM event."""
         eventName: str
         targetName: str = OPTIONAL
     
     @dataclass
     class setInstrumentationBreakpoint(ProtocolCommand):
-        """Sets breakpoint on particular native event."""
+        """[Just CDP] Sets breakpoint on particular native event."""
         eventName: str
     
     @dataclass
     class setXHRBreakpoint(ProtocolCommand):
-        """Sets breakpoint on XMLHttpRequest."""
+        """[Just CDP] Sets breakpoint on XMLHttpRequest."""
         url: str
     
+    @dataclass
+    class setEventBreakpoint(ProtocolCommand):
+        """[Just WIP] Sets breakpoint on particular event of given type."""
+        breakpointType: DOMDebugger.EventBreakpointType
+        eventName: str = OPTIONAL
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class removeEventBreakpoint(ProtocolCommand):
+        """[Just WIP] Removes breakpoint on particular event of given type."""
+        breakpointType: DOMDebugger.EventBreakpointType
+        eventName: str = OPTIONAL
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class setURLBreakpoint(ProtocolCommand):
+        """[Just WIP] Sets breakpoint on network activity for the given URL."""
+        url: str
+        isRegex: bool = OPTIONAL
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class removeURLBreakpoint(ProtocolCommand):
+        """[Just WIP] Removes breakpoint from network activity for the given URL."""
+        url: str
+        isRegex: bool = OPTIONAL
+    
 
 @domainclass
 class DOMSnapshot:
     """[Just CDP][Experimental] This domain facilitates obtaining document snapshots with DOM, layout, and style information."""
     class DOMNode:
         """A Node in the DOM tree."""
         nodeType: int
@@ -2381,14 +2643,15 @@
         newValue: str
     
     class domStorageItemsCleared(BaseEvent):
         storageId: DOMStorage.StorageId
     
     @dataclass
     class clear(ProtocolCommand):
+        """[Just CDP]"""
         storageId: DOMStorage.StorageId
     
     @dataclass
     class disable(ProtocolCommand):
         """Disables storage tracking, prevents storage events from being sent to the client."""
         pass
     
@@ -2408,14 +2671,19 @@
     
     @dataclass
     class setDOMStorageItem(ProtocolCommand):
         storageId: DOMStorage.StorageId
         key: str
         value: str
     
+    @dataclass
+    class clearDOMStorageItems(ProtocolCommand):
+        """[Just WIP]"""
+        storageId: DOMStorage.StorageId
+    
 
 @domainclass
 class Database:
     DatabaseId: str
     class Database:
         """Database object."""
         id: Database.DatabaseId
@@ -2778,23 +3046,23 @@
         objectStoreName: str
         securityOrigin: str = OPTIONAL
         storageKey: str = OPTIONAL
         storageBucket: Storage.StorageBucket = OPTIONAL
     
     @dataclass
     class deleteDatabase(ProtocolCommand):
-        """Deletes a database."""
+        """[Just CDP] Deletes a database."""
         databaseName: str
         securityOrigin: str = OPTIONAL
         storageKey: str = OPTIONAL
         storageBucket: Storage.StorageBucket = OPTIONAL
     
     @dataclass
     class deleteObjectStoreEntries(ProtocolCommand):
-        """Delete a range of entries from an object store"""
+        """[Just CDP] Delete a range of entries from an object store"""
         databaseName: str
         objectStoreName: str
         keyRange: IndexedDB.KeyRange
         securityOrigin: str = OPTIONAL
         storageKey: str = OPTIONAL
         storageBucket: Storage.StorageBucket = OPTIONAL
     
@@ -2819,15 +3087,15 @@
         securityOrigin: str = OPTIONAL
         storageKey: str = OPTIONAL
         storageBucket: Storage.StorageBucket = OPTIONAL
         keyRange: IndexedDB.KeyRange = OPTIONAL
     
     @dataclass
     class getMetadata(ProtocolCommand):
-        """Gets metadata of an object store."""
+        """[Just CDP] Gets metadata of an object store."""
         databaseName: str
         objectStoreName: str
         securityOrigin: str = OPTIONAL
         storageKey: str = OPTIONAL
         storageBucket: Storage.StorageBucket = OPTIONAL
     
     @dataclass
@@ -3046,14 +3314,19 @@
         pass
     
     @dataclass
     class enable(ProtocolCommand):
         """Enables inspector domain notifications."""
         pass
     
+    @dataclass
+    class initialized(ProtocolCommand):
+        """[Just WIP] Sent by the frontend after all initialization messages have been sent."""
+        pass
+    
 
 @domainclass
 class LayerTree:
     LayerId: str
     SnapshotId: str
     class ScrollRect:
         """Rectangle where scrolling happens on the main thread."""
@@ -3147,62 +3420,73 @@
         clip: DOM.Rect
     
     class layerTreeDidChange(BaseEvent):
         layers: list
     
     @dataclass
     class compositingReasons(ProtocolCommand):
-        """Provides the reasons why the given layer was composited."""
+        """[Just CDP] Provides the reasons why the given layer was composited."""
         layerId: LayerTree.LayerId
     
     @dataclass
     class disable(ProtocolCommand):
         """Disables compositing tree inspection."""
         pass
     
     @dataclass
     class enable(ProtocolCommand):
         """Enables compositing tree inspection."""
         pass
     
     @dataclass
     class loadSnapshot(ProtocolCommand):
-        """Returns the snapshot identifier."""
+        """[Just CDP] Returns the snapshot identifier."""
         tiles: list
     
     @dataclass
     class makeSnapshot(ProtocolCommand):
-        """Returns the layer snapshot identifier."""
+        """[Just CDP] Returns the layer snapshot identifier."""
         layerId: LayerTree.LayerId
     
     @dataclass
     class profileSnapshot(ProtocolCommand):
+        """[Just CDP]"""
         snapshotId: LayerTree.SnapshotId
         minRepeatCount: int = OPTIONAL
         minDuration: int = OPTIONAL
         clipRect: DOM.Rect = OPTIONAL
     
     @dataclass
     class releaseSnapshot(ProtocolCommand):
-        """Releases layer snapshot captured by the back-end."""
+        """[Just CDP] Releases layer snapshot captured by the back-end."""
         snapshotId: LayerTree.SnapshotId
     
     @dataclass
     class replaySnapshot(ProtocolCommand):
-        """Replays the layer snapshot and returns the resulting bitmap."""
+        """[Just CDP] Replays the layer snapshot and returns the resulting bitmap."""
         snapshotId: LayerTree.SnapshotId
         fromStep: int = OPTIONAL
         toStep: int = OPTIONAL
         scale: int = OPTIONAL
     
     @dataclass
     class snapshotCommandLog(ProtocolCommand):
-        """Replays the layer snapshot and returns canvas log."""
+        """[Just CDP] Replays the layer snapshot and returns canvas log."""
         snapshotId: LayerTree.SnapshotId
     
+    @dataclass
+    class layersForNode(ProtocolCommand):
+        """[Just WIP] Returns the layer tree structure of the current page."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class reasonsForCompositingLayer(ProtocolCommand):
+        """[Just WIP] Provides the reasons why the given layer was composited."""
+        layerId: LayerTree.LayerId
+    
 
 @domainclass
 class Log:
     """[Just CDP] Provides access to log entries."""
     class LogEntry:
         """Log entry."""
         source: str
@@ -3297,64 +3581,86 @@
     
     class trackingComplete(BaseEvent):
         """Tracking stopped."""
         timestamp: int
     
     @dataclass
     class getDOMCounters(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class prepareForLeakDetection(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class forciblyPurgeJavaScriptMemory(ProtocolCommand):
-        """Simulate OomIntervention by purging V8 memory."""
+        """[Just CDP] Simulate OomIntervention by purging V8 memory."""
         pass
     
     @dataclass
     class setPressureNotificationsSuppressed(ProtocolCommand):
-        """Enable/disable suppressing memory pressure notifications in all processes."""
+        """[Just CDP] Enable/disable suppressing memory pressure notifications in all processes."""
         suppressed: bool
     
     @dataclass
     class simulatePressureNotification(ProtocolCommand):
-        """Simulate a memory pressure notification in all processes."""
+        """[Just CDP] Simulate a memory pressure notification in all processes."""
         level: Memory.PressureLevel
     
     @dataclass
     class startSampling(ProtocolCommand):
-        """Start collecting native memory profile."""
+        """[Just CDP] Start collecting native memory profile."""
         samplingInterval: int = OPTIONAL
         suppressRandomness: bool = OPTIONAL
     
     @dataclass
     class stopSampling(ProtocolCommand):
-        """Stop collecting native memory profile."""
+        """[Just CDP] Stop collecting native memory profile."""
         pass
     
     @dataclass
     class getAllTimeSamplingProfile(ProtocolCommand):
-        """Retrieve native memory allocations profile
+        """[Just CDP] Retrieve native memory allocations profile
 collected since renderer process startup."""
         pass
     
     @dataclass
     class getBrowserSamplingProfile(ProtocolCommand):
-        """Retrieve native memory allocations profile
+        """[Just CDP] Retrieve native memory allocations profile
 collected since browser process startup."""
         pass
     
     @dataclass
     class getSamplingProfile(ProtocolCommand):
-        """Retrieve native memory allocations profile collected since last
+        """[Just CDP] Retrieve native memory allocations profile collected since last
 `startSampling` call."""
         pass
     
+    @dataclass
+    class enable(ProtocolCommand):
+        """[Just WIP] Enables Memory domain events."""
+        pass
+    
+    @dataclass
+    class disable(ProtocolCommand):
+        """[Just WIP] Disables Memory domain events."""
+        pass
+    
+    @dataclass
+    class startTracking(ProtocolCommand):
+        """[Just WIP] Start tracking memory. This will produce a `trackingStart` event."""
+        pass
+    
+    @dataclass
+    class stopTracking(ProtocolCommand):
+        """[Just WIP] Stop tracking memory. This will produce a `trackingComplete` event."""
+        pass
+    
 
 @domainclass
 class Network:
     """Network domain allows tracking network activities of the page. It exposes information about http,
 file, data and other requests and responses, their headers, bodies, timing, etc."""
     ResourceType: str
     LoaderId: str
@@ -3971,50 +4277,50 @@
     class responseIntercepted(BaseEvent):
         """Fired when HTTP response has been intercepted. The frontend must response with <code>Network.interceptContinue</code> or <code>Network.interceptWithResponse</code>` to continue this response."""
         requestId: Network.RequestId
         response: Network.Response
     
     @dataclass
     class setAcceptedEncodings(ProtocolCommand):
-        """Sets a list of content encodings that will be accepted. Empty list means no encoding is accepted."""
+        """[Just CDP] Sets a list of content encodings that will be accepted. Empty list means no encoding is accepted."""
         encodings: list
     
     @dataclass
     class clearAcceptedEncodingsOverride(ProtocolCommand):
-        """Clears accepted encodings set by setAcceptedEncodings"""
+        """[Just CDP] Clears accepted encodings set by setAcceptedEncodings"""
         pass
     
     @dataclass
     class canClearBrowserCache(ProtocolCommand):
-        """Tells whether clearing browser cache is supported."""
+        """[Just CDP] Tells whether clearing browser cache is supported."""
         pass
     
     @dataclass
     class canClearBrowserCookies(ProtocolCommand):
-        """Tells whether clearing browser cookies is supported."""
+        """[Just CDP] Tells whether clearing browser cookies is supported."""
         pass
     
     @dataclass
     class canEmulateNetworkConditions(ProtocolCommand):
-        """Tells whether emulation of network conditions is supported."""
+        """[Just CDP] Tells whether emulation of network conditions is supported."""
         pass
     
     @dataclass
     class clearBrowserCache(ProtocolCommand):
-        """Clears browser cache."""
+        """[Just CDP] Clears browser cache."""
         pass
     
     @dataclass
     class clearBrowserCookies(ProtocolCommand):
-        """Clears browser cookies."""
+        """[Just CDP] Clears browser cookies."""
         pass
     
     @dataclass
     class continueInterceptedRequest(ProtocolCommand):
-        """Response to Network.requestIntercepted which either modifies the request to continue with any
+        """[Just CDP] Response to Network.requestIntercepted which either modifies the request to continue with any
 modifications, or blocks it, or completes it with the provided response bytes. If a network
 fetch occurs as a result which encounters a redirect an additional Network.requestIntercepted
 event will be sent with the same InterceptionId.
 Deprecated, use Fetch.continueRequest, Fetch.fulfillRequest and Fetch.failRequest instead."""
         interceptionId: Network.InterceptionId
         errorReason: Network.ErrorReason = OPTIONAL
         rawResponse: str = OPTIONAL
@@ -4022,28 +4328,28 @@
         method: str = OPTIONAL
         postData: str = OPTIONAL
         headers: Network.Headers = OPTIONAL
         authChallengeResponse: Network.AuthChallengeResponse = OPTIONAL
     
     @dataclass
     class deleteCookies(ProtocolCommand):
-        """Deletes browser cookies with matching name and url or domain/path pair."""
+        """[Just CDP] Deletes browser cookies with matching name and url or domain/path pair."""
         name: str
         url: str = OPTIONAL
         domain: str = OPTIONAL
         path: str = OPTIONAL
     
     @dataclass
     class disable(ProtocolCommand):
         """Disables network tracking, prevents network events from being sent to the client."""
         pass
     
     @dataclass
     class emulateNetworkConditions(ProtocolCommand):
-        """Activates emulation of network conditions."""
+        """[Just CDP] Activates emulation of network conditions."""
         offline: bool
         latency: int
         downloadThroughput: int
         uploadThroughput: int
         connectionType: Network.ConnectionType = OPTIONAL
     
     @dataclass
@@ -4051,86 +4357,86 @@
         """Enables network tracking, network events will now be delivered to the client."""
         maxTotalBufferSize: int = OPTIONAL
         maxResourceBufferSize: int = OPTIONAL
         maxPostDataSize: int = OPTIONAL
     
     @dataclass
     class getAllCookies(ProtocolCommand):
-        """Returns all browser cookies. Depending on the backend support, will return detailed cookie
+        """[Just CDP] Returns all browser cookies. Depending on the backend support, will return detailed cookie
 information in the `cookies` field.
 Deprecated. Use Storage.getCookies instead."""
         pass
     
     @dataclass
     class getCertificate(ProtocolCommand):
-        """Returns the DER-encoded certificate."""
+        """[Just CDP] Returns the DER-encoded certificate."""
         origin: str
     
     @dataclass
     class getCookies(ProtocolCommand):
-        """Returns all browser cookies for the current URL. Depending on the backend support, will return
+        """[Just CDP] Returns all browser cookies for the current URL. Depending on the backend support, will return
 detailed cookie information in the `cookies` field."""
         urls: list = OPTIONAL
     
     @dataclass
     class getResponseBody(ProtocolCommand):
         """Returns content served for the given request."""
         requestId: Network.RequestId
     
     @dataclass
     class getRequestPostData(ProtocolCommand):
-        """Returns post data sent with the request. Returns an error when no data was sent with the request."""
+        """[Just CDP] Returns post data sent with the request. Returns an error when no data was sent with the request."""
         requestId: Network.RequestId
     
     @dataclass
     class getResponseBodyForInterception(ProtocolCommand):
-        """Returns content served for the given currently intercepted request."""
+        """[Just CDP] Returns content served for the given currently intercepted request."""
         interceptionId: Network.InterceptionId
     
     @dataclass
     class takeResponseBodyForInterceptionAsStream(ProtocolCommand):
-        """Returns a handle to the stream representing the response body. Note that after this command,
+        """[Just CDP] Returns a handle to the stream representing the response body. Note that after this command,
 the intercepted request can't be continued as is -- you either need to cancel it or to provide
 the response body. The stream only supports sequential read, IO.read will fail if the position
 is specified."""
         interceptionId: Network.InterceptionId
     
     @dataclass
     class replayXHR(ProtocolCommand):
-        """This method sends a new XMLHttpRequest which is identical to the original one. The following
+        """[Just CDP] This method sends a new XMLHttpRequest which is identical to the original one. The following
 parameters should be identical: method, url, async, request body, extra headers, withCredentials
 attribute, user, password."""
         requestId: Network.RequestId
     
     @dataclass
     class searchInResponseBody(ProtocolCommand):
-        """Searches for given string in response content."""
+        """[Just CDP] Searches for given string in response content."""
         requestId: Network.RequestId
         query: str
         caseSensitive: bool = OPTIONAL
         isRegex: bool = OPTIONAL
     
     @dataclass
     class setBlockedURLs(ProtocolCommand):
-        """Blocks URLs from loading."""
+        """[Just CDP] Blocks URLs from loading."""
         urls: list
     
     @dataclass
     class setBypassServiceWorker(ProtocolCommand):
-        """Toggles ignoring of service worker for each request."""
+        """[Just CDP] Toggles ignoring of service worker for each request."""
         bypass: bool
     
     @dataclass
     class setCacheDisabled(ProtocolCommand):
-        """Toggles ignoring cache for each request. If `true`, cache will not be used."""
+        """[Just CDP] Toggles ignoring cache for each request. If `true`, cache will not be used."""
         cacheDisabled: bool
     
     @dataclass
     class setCookie(ProtocolCommand):
-        """Sets a cookie with the given cookie data; may overwrite equivalent cookies if they exist."""
+        """[Just CDP] Sets a cookie with the given cookie data; may overwrite equivalent cookies if they exist."""
         name: str
         value: str
         url: str = OPTIONAL
         domain: str = OPTIONAL
         path: str = OPTIONAL
         secure: bool = OPTIONAL
         httpOnly: bool = OPTIONAL
@@ -4140,59 +4446,150 @@
         sameParty: bool = OPTIONAL
         sourceScheme: Network.CookieSourceScheme = OPTIONAL
         sourcePort: int = OPTIONAL
         partitionKey: str = OPTIONAL
     
     @dataclass
     class setCookies(ProtocolCommand):
-        """Sets given cookies."""
+        """[Just CDP] Sets given cookies."""
         cookies: list
     
     @dataclass
     class setExtraHTTPHeaders(ProtocolCommand):
         """Specifies whether to always send extra HTTP headers with the requests from this page."""
         headers: Network.Headers
     
     @dataclass
     class setAttachDebugStack(ProtocolCommand):
-        """Specifies whether to attach a page script stack id in requests"""
+        """[Just CDP] Specifies whether to attach a page script stack id in requests"""
         enabled: bool
     
     @dataclass
     class setRequestInterception(ProtocolCommand):
-        """Sets the requests to intercept that match the provided patterns and optionally resource types.
+        """[Just CDP] Sets the requests to intercept that match the provided patterns and optionally resource types.
 Deprecated, please use Fetch.enable instead."""
         patterns: list
     
     @dataclass
     class setUserAgentOverride(ProtocolCommand):
-        """Allows overriding user agent with the given string."""
+        """[Just CDP] Allows overriding user agent with the given string."""
         userAgent: str
         acceptLanguage: str = OPTIONAL
         platform: str = OPTIONAL
         userAgentMetadata: Emulation.UserAgentMetadata = OPTIONAL
     
     @dataclass
     class getSecurityIsolationStatus(ProtocolCommand):
-        """Returns information about the COEP/COOP isolation status."""
+        """[Just CDP] Returns information about the COEP/COOP isolation status."""
         frameId: Page.FrameId = OPTIONAL
     
     @dataclass
     class enableReportingApi(ProtocolCommand):
-        """Enables tracking for the Reporting API, events generated by the Reporting API will now be delivered to the client.
+        """[Just CDP] Enables tracking for the Reporting API, events generated by the Reporting API will now be delivered to the client.
 Enabling triggers 'reportingApiReportAdded' for all existing reports."""
         enable: bool
     
     @dataclass
     class loadNetworkResource(ProtocolCommand):
-        """Fetches the resource and returns the content."""
+        """[Just CDP] Fetches the resource and returns the content."""
         url: str
         options: Network.LoadNetworkResourceOptions
         frameId: Page.FrameId = OPTIONAL
     
+    @dataclass
+    class setResourceCachingDisabled(ProtocolCommand):
+        """[Just WIP] Toggles whether the resource cache may be used when loading resources in the inspected page. If <code>true</code>, the resource cache will not be used when loading resources."""
+        disabled: bool
+    
+    @dataclass
+    class loadResource(ProtocolCommand):
+        """[Just WIP] Loads a resource in the context of a frame on the inspected page without cross origin checks."""
+        frameId: Network.FrameId
+        url: str
+    
+    @dataclass
+    class getSerializedCertificate(ProtocolCommand):
+        """[Just WIP] Fetches a serialized secure certificate for the given requestId to be displayed via InspectorFrontendHost.showCertificate."""
+        requestId: Network.RequestId
+    
+    @dataclass
+    class resolveWebSocket(ProtocolCommand):
+        """[Just WIP] Resolves JavaScript WebSocket object for given request id."""
+        requestId: Network.RequestId
+        objectGroup: str = OPTIONAL
+    
+    @dataclass
+    class setInterceptionEnabled(ProtocolCommand):
+        """[Just WIP] Enable interception of network requests."""
+        enabled: bool
+    
+    @dataclass
+    class addInterception(ProtocolCommand):
+        """[Just WIP] Add an interception."""
+        url: str
+        stage: Network.NetworkStage
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class removeInterception(ProtocolCommand):
+        """[Just WIP] Remove an interception."""
+        url: str
+        stage: Network.NetworkStage
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class interceptContinue(ProtocolCommand):
+        """[Just WIP] Continue request or response without modifications."""
+        requestId: Network.RequestId
+        stage: Network.NetworkStage
+    
+    @dataclass
+    class interceptWithRequest(ProtocolCommand):
+        """[Just WIP] Replace intercepted request with the provided one."""
+        requestId: Network.RequestId
+        url: str = OPTIONAL
+        method: str = OPTIONAL
+        headers: Network.Headers = OPTIONAL
+        postData: str = OPTIONAL
+    
+    @dataclass
+    class interceptWithResponse(ProtocolCommand):
+        """[Just WIP] Provide response content for an intercepted response."""
+        requestId: Network.RequestId
+        content: str
+        base64Encoded: bool
+        mimeType: str = OPTIONAL
+        status: int = OPTIONAL
+        statusText: str = OPTIONAL
+        headers: Network.Headers = OPTIONAL
+    
+    @dataclass
+    class interceptRequestWithResponse(ProtocolCommand):
+        """[Just WIP] Provide response for an intercepted request. Request completely bypasses the network in this case and is immediately fulfilled with the provided data."""
+        requestId: Network.RequestId
+        content: str
+        base64Encoded: bool
+        mimeType: str
+        status: int
+        statusText: str
+        headers: Network.Headers
+    
+    @dataclass
+    class interceptRequestWithError(ProtocolCommand):
+        """[Just WIP] Fail request with given error type."""
+        requestId: Network.RequestId
+        errorType: Network.ResourceErrorType
+    
+    @dataclass
+    class setEmulatedConditions(ProtocolCommand):
+        """[Just WIP] Emulate various network conditions (e.g. bytes per second, latency, etc.)."""
+        bytesPerSecondLimit: int = OPTIONAL
+    
 
 @domainclass
 class Overlay:
     """[Just CDP][Experimental] This domain provides various functionality related to drawing atop the inspected page."""
     class SourceOrderConfig:
         """Configuration data for drawing the source order of an elements children."""
         parentOutlineColor: DOM.RGBA
@@ -4876,64 +5273,64 @@
     
     class defaultUserPreferencesDidChange(BaseEvent):
         """Fired when the default value of a user preference changes at the system level."""
         preferences: list
     
     @dataclass
     class addScriptToEvaluateOnLoad(ProtocolCommand):
-        """Deprecated, please use addScriptToEvaluateOnNewDocument instead."""
+        """[Just CDP] Deprecated, please use addScriptToEvaluateOnNewDocument instead."""
         scriptSource: str
     
     @dataclass
     class addScriptToEvaluateOnNewDocument(ProtocolCommand):
-        """Evaluates given script in every frame upon creation (before loading frame's scripts)."""
+        """[Just CDP] Evaluates given script in every frame upon creation (before loading frame's scripts)."""
         source: str
         worldName: str = OPTIONAL
         includeCommandLineAPI: bool = OPTIONAL
         runImmediately: bool = OPTIONAL
     
     @dataclass
     class bringToFront(ProtocolCommand):
-        """Brings page to front (activates tab)."""
+        """[Just CDP] Brings page to front (activates tab)."""
         pass
     
     @dataclass
     class captureScreenshot(ProtocolCommand):
-        """Capture page screenshot."""
+        """[Just CDP] Capture page screenshot."""
         format: str = OPTIONAL
         quality: int = OPTIONAL
         clip: Page.Viewport = OPTIONAL
         fromSurface: bool = OPTIONAL
         captureBeyondViewport: bool = OPTIONAL
         optimizeForSpeed: bool = OPTIONAL
     
     @dataclass
     class captureSnapshot(ProtocolCommand):
-        """Returns a snapshot of the page as a string. For MHTML format, the serialization includes
+        """[Just CDP] Returns a snapshot of the page as a string. For MHTML format, the serialization includes
 iframes, shadow DOM, external resources, and element-inline styles."""
         format: str = OPTIONAL
     
     @dataclass
     class clearDeviceMetricsOverride(ProtocolCommand):
-        """Clears the overridden device metrics."""
+        """[Just CDP] Clears the overridden device metrics."""
         pass
     
     @dataclass
     class clearDeviceOrientationOverride(ProtocolCommand):
-        """Clears the overridden Device Orientation."""
+        """[Just CDP] Clears the overridden Device Orientation."""
         pass
     
     @dataclass
     class clearGeolocationOverride(ProtocolCommand):
-        """Clears the overridden Geolocation Position and Error."""
+        """[Just CDP] Clears the overridden Geolocation Position and Error."""
         pass
     
     @dataclass
     class createIsolatedWorld(ProtocolCommand):
-        """Creates an isolated world for the given frame."""
+        """[Just CDP] Creates an isolated world for the given frame."""
         frameId: Page.FrameId
         worldName: str = OPTIONAL
         grantUniveralAccess: bool = OPTIONAL
     
     @dataclass
     class deleteCookie(ProtocolCommand):
         """Deletes browser cookie with given name, domain and path."""
@@ -4948,60 +5345,63 @@
     @dataclass
     class enable(ProtocolCommand):
         """Enables page domain notifications."""
         pass
     
     @dataclass
     class getAppManifest(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class getInstallabilityErrors(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class getManifestIcons(ProtocolCommand):
-        """Deprecated because it's not guaranteed that the returned icon is in fact the one used for PWA installation."""
+        """[Just CDP] Deprecated because it's not guaranteed that the returned icon is in fact the one used for PWA installation."""
         pass
     
     @dataclass
     class getAppId(ProtocolCommand):
-        """Returns the unique (PWA) app id.
+        """[Just CDP] Returns the unique (PWA) app id.
 Only returns values if the feature flag 'WebAppEnableManifestId' is enabled"""
         pass
     
     @dataclass
     class getAdScriptId(ProtocolCommand):
+        """[Just CDP]"""
         frameId: Page.FrameId
     
     @dataclass
     class getCookies(ProtocolCommand):
         """Returns all browser cookies for the page and all of its subframes. Depending
 on the backend support, will return detailed cookie information in the
 `cookies` field."""
         pass
     
     @dataclass
     class getFrameTree(ProtocolCommand):
-        """Returns present frame tree structure."""
+        """[Just CDP] Returns present frame tree structure."""
         pass
     
     @dataclass
     class getLayoutMetrics(ProtocolCommand):
-        """Returns metrics relating to the layouting of the page, such as viewport bounds/scale."""
+        """[Just CDP] Returns metrics relating to the layouting of the page, such as viewport bounds/scale."""
         pass
     
     @dataclass
     class getNavigationHistory(ProtocolCommand):
-        """Returns navigation history for the current page."""
+        """[Just CDP] Returns navigation history for the current page."""
         pass
     
     @dataclass
     class resetNavigationHistory(ProtocolCommand):
-        """Resets navigation history for the current page."""
+        """[Just CDP] Resets navigation history for the current page."""
         pass
     
     @dataclass
     class getResourceContent(ProtocolCommand):
         """Returns content of the given resource."""
         frameId: Page.FrameId
         url: str
@@ -5009,35 +5409,35 @@
     @dataclass
     class getResourceTree(ProtocolCommand):
         """Returns present frame / resource tree structure."""
         pass
     
     @dataclass
     class handleJavaScriptDialog(ProtocolCommand):
-        """Accepts or dismisses a JavaScript initiated dialog (alert, confirm, prompt, or onbeforeunload)."""
+        """[Just CDP] Accepts or dismisses a JavaScript initiated dialog (alert, confirm, prompt, or onbeforeunload)."""
         accept: bool
         promptText: str = OPTIONAL
     
     @dataclass
     class navigate(ProtocolCommand):
         """Navigates current page to the given URL."""
         url: str
         referrer: str = OPTIONAL
         transitionType: Page.TransitionType = OPTIONAL
         frameId: Page.FrameId = OPTIONAL
         referrerPolicy: Page.ReferrerPolicy = OPTIONAL
     
     @dataclass
     class navigateToHistoryEntry(ProtocolCommand):
-        """Navigates current page to the given history entry."""
+        """[Just CDP] Navigates current page to the given history entry."""
         entryId: int
     
     @dataclass
     class printToPDF(ProtocolCommand):
-        """Print page as PDF."""
+        """[Just CDP] Print page as PDF."""
         landscape: bool = OPTIONAL
         displayHeaderFooter: bool = OPTIONAL
         printBackground: bool = OPTIONAL
         scale: int = OPTIONAL
         paperWidth: int = OPTIONAL
         paperHeight: int = OPTIONAL
         marginTop: int = OPTIONAL
@@ -5052,62 +5452,64 @@
         generateTaggedPDF: bool = OPTIONAL
     
     @dataclass
     class reload(ProtocolCommand):
         """Reloads given page optionally ignoring the cache."""
         ignoreCache: bool = OPTIONAL
         scriptToEvaluateOnLoad: str = OPTIONAL
+        revalidateAllResources: bool = OPTIONAL
     
     @dataclass
     class removeScriptToEvaluateOnLoad(ProtocolCommand):
-        """Deprecated, please use removeScriptToEvaluateOnNewDocument instead."""
+        """[Just CDP] Deprecated, please use removeScriptToEvaluateOnNewDocument instead."""
         identifier: Page.ScriptIdentifier
     
     @dataclass
     class removeScriptToEvaluateOnNewDocument(ProtocolCommand):
-        """Removes given script from the list."""
+        """[Just CDP] Removes given script from the list."""
         identifier: Page.ScriptIdentifier
     
     @dataclass
     class screencastFrameAck(ProtocolCommand):
-        """Acknowledges that a screencast frame has been received by the frontend."""
+        """[Just CDP] Acknowledges that a screencast frame has been received by the frontend."""
         sessionId: int
     
     @dataclass
     class searchInResource(ProtocolCommand):
         """Searches for given string in resource content."""
         frameId: Page.FrameId
         url: str
         query: str
         caseSensitive: bool = OPTIONAL
         isRegex: bool = OPTIONAL
+        requestId: Network.RequestId = OPTIONAL
     
     @dataclass
     class setAdBlockingEnabled(ProtocolCommand):
-        """Enable Chrome's experimental ad filter on all sites."""
+        """[Just CDP] Enable Chrome's experimental ad filter on all sites."""
         enabled: bool
     
     @dataclass
     class setBypassCSP(ProtocolCommand):
-        """Enable page Content Security Policy by-passing."""
+        """[Just CDP] Enable page Content Security Policy by-passing."""
         enabled: bool
     
     @dataclass
     class getPermissionsPolicyState(ProtocolCommand):
-        """Get Permissions Policy state on given frame."""
+        """[Just CDP] Get Permissions Policy state on given frame."""
         frameId: Page.FrameId
     
     @dataclass
     class getOriginTrials(ProtocolCommand):
-        """Get Origin Trials on given frame."""
+        """[Just CDP] Get Origin Trials on given frame."""
         frameId: Page.FrameId
     
     @dataclass
     class setDeviceMetricsOverride(ProtocolCommand):
-        """Overrides the values of device screen dimensions (window.screen.width, window.screen.height,
+        """[Just CDP] Overrides the values of device screen dimensions (window.screen.width, window.screen.height,
 window.innerWidth, window.innerHeight, and "device-width"/"device-height"-related CSS media
 query results)."""
         width: int
         height: int
         deviceScaleFactor: int
         mobile: bool
         scale: int = OPTIONAL
@@ -5117,160 +5519,234 @@
         positionY: int = OPTIONAL
         dontSetVisibleSize: bool = OPTIONAL
         screenOrientation: Emulation.ScreenOrientation = OPTIONAL
         viewport: Page.Viewport = OPTIONAL
     
     @dataclass
     class setDeviceOrientationOverride(ProtocolCommand):
-        """Overrides the Device Orientation."""
+        """[Just CDP] Overrides the Device Orientation."""
         alpha: int
         beta: int
         gamma: int
     
     @dataclass
     class setFontFamilies(ProtocolCommand):
-        """Set generic font families."""
+        """[Just CDP] Set generic font families."""
         fontFamilies: Page.FontFamilies
         forScripts: list = OPTIONAL
     
     @dataclass
     class setFontSizes(ProtocolCommand):
-        """Set default font sizes."""
+        """[Just CDP] Set default font sizes."""
         fontSizes: Page.FontSizes
     
     @dataclass
     class setDocumentContent(ProtocolCommand):
-        """Sets given markup as the document's HTML."""
+        """[Just CDP] Sets given markup as the document's HTML."""
         frameId: Page.FrameId
         html: str
     
     @dataclass
     class setDownloadBehavior(ProtocolCommand):
-        """Set the behavior when downloading a file."""
+        """[Just CDP] Set the behavior when downloading a file."""
         behavior: str
         downloadPath: str = OPTIONAL
     
     @dataclass
     class setGeolocationOverride(ProtocolCommand):
-        """Overrides the Geolocation Position or Error. Omitting any of the parameters emulates position
+        """[Just CDP] Overrides the Geolocation Position or Error. Omitting any of the parameters emulates position
 unavailable."""
         latitude: int = OPTIONAL
         longitude: int = OPTIONAL
         accuracy: int = OPTIONAL
     
     @dataclass
     class setLifecycleEventsEnabled(ProtocolCommand):
-        """Controls whether page will emit lifecycle events."""
+        """[Just CDP] Controls whether page will emit lifecycle events."""
         enabled: bool
     
     @dataclass
     class setTouchEmulationEnabled(ProtocolCommand):
-        """Toggles mouse event-based touch event emulation."""
+        """[Just CDP] Toggles mouse event-based touch event emulation."""
         enabled: bool
         configuration: str = OPTIONAL
     
     @dataclass
     class startScreencast(ProtocolCommand):
-        """Starts sending each frame using the `screencastFrame` event."""
+        """[Just CDP] Starts sending each frame using the `screencastFrame` event."""
         format: str = OPTIONAL
         quality: int = OPTIONAL
         maxWidth: int = OPTIONAL
         maxHeight: int = OPTIONAL
         everyNthFrame: int = OPTIONAL
     
     @dataclass
     class stopLoading(ProtocolCommand):
-        """Force the page stop all navigations and pending resource fetches."""
+        """[Just CDP] Force the page stop all navigations and pending resource fetches."""
         pass
     
     @dataclass
     class crash(ProtocolCommand):
-        """Crashes renderer on the IO thread, generates minidumps."""
+        """[Just CDP] Crashes renderer on the IO thread, generates minidumps."""
         pass
     
     @dataclass
     class close(ProtocolCommand):
-        """Tries to close page, running its beforeunload hooks, if any."""
+        """[Just CDP] Tries to close page, running its beforeunload hooks, if any."""
         pass
     
     @dataclass
     class setWebLifecycleState(ProtocolCommand):
-        """Tries to update the web lifecycle state of the page.
+        """[Just CDP] Tries to update the web lifecycle state of the page.
 It will transition the page to the given state according to:
 https://github.com/WICG/web-lifecycle/"""
         state: str
     
     @dataclass
     class stopScreencast(ProtocolCommand):
-        """Stops sending each frame in the `screencastFrame`."""
+        """[Just CDP] Stops sending each frame in the `screencastFrame`."""
         pass
     
     @dataclass
     class produceCompilationCache(ProtocolCommand):
-        """Requests backend to produce compilation cache for the specified scripts.
+        """[Just CDP] Requests backend to produce compilation cache for the specified scripts.
 `scripts` are appeneded to the list of scripts for which the cache
 would be produced. The list may be reset during page navigation.
 When script with a matching URL is encountered, the cache is optionally
 produced upon backend discretion, based on internal heuristics.
 See also: `Page.compilationCacheProduced`."""
         scripts: list
     
     @dataclass
     class addCompilationCache(ProtocolCommand):
-        """Seeds compilation cache for given url. Compilation cache does not survive
+        """[Just CDP] Seeds compilation cache for given url. Compilation cache does not survive
 cross-process navigation."""
         url: str
         data: str
     
     @dataclass
     class clearCompilationCache(ProtocolCommand):
-        """Clears seeded compilation cache."""
+        """[Just CDP] Clears seeded compilation cache."""
         pass
     
     @dataclass
     class setSPCTransactionMode(ProtocolCommand):
-        """Sets the Secure Payment Confirmation transaction mode.
+        """[Just CDP] Sets the Secure Payment Confirmation transaction mode.
 https://w3c.github.io/secure-payment-confirmation/#sctn-automation-set-spc-transaction-mode"""
         mode: Page.AutoResponseMode
     
     @dataclass
     class setRPHRegistrationMode(ProtocolCommand):
-        """Extensions for Custom Handlers API:
+        """[Just CDP] Extensions for Custom Handlers API:
 https://html.spec.whatwg.org/multipage/system-state.html#rph-automation"""
         mode: Page.AutoResponseMode
     
     @dataclass
     class generateTestReport(ProtocolCommand):
-        """Generates a report for testing."""
+        """[Just CDP] Generates a report for testing."""
         message: str
         group: str = OPTIONAL
     
     @dataclass
     class waitForDebugger(ProtocolCommand):
-        """Pauses page execution. Can be resumed using generic Runtime.runIfWaitingForDebugger."""
+        """[Just CDP] Pauses page execution. Can be resumed using generic Runtime.runIfWaitingForDebugger."""
         pass
     
     @dataclass
     class setInterceptFileChooserDialog(ProtocolCommand):
-        """Intercept file chooser requests and transfer control to protocol clients.
+        """[Just CDP] Intercept file chooser requests and transfer control to protocol clients.
 When file chooser interception is enabled, native file chooser dialog is not shown.
 Instead, a protocol event `Page.fileChooserOpened` is emitted."""
         enabled: bool
     
     @dataclass
     class setPrerenderingAllowed(ProtocolCommand):
-        """Enable/disable prerendering manually.
+        """[Just CDP] Enable/disable prerendering manually.
 
 This command is a short-term solution for https://crbug.com/1440085.
 See https://docs.google.com/document/d/12HVmFxYj5Jc-eJr5OmWsa2bqTJsbgGLKI6ZIyx0_wpA
 for more details.
 
 TODO(https://crbug.com/1440085): Remove this once Puppeteer supports tab targets."""
         isAllowed: bool
     
+    @dataclass
+    class overrideUserAgent(ProtocolCommand):
+        """[Just WIP] Override's the user agent of the inspected page"""
+        value: str = OPTIONAL
+    
+    @dataclass
+    class overrideSetting(ProtocolCommand):
+        """[Just WIP] Allows the frontend to override the inspected page's settings."""
+        setting: Page.Setting
+        value: bool = OPTIONAL
+    
+    @dataclass
+    class overrideUserPreference(ProtocolCommand):
+        """[Just WIP] Allows the frontend to override the user's preferences on the inspected page."""
+        name: Page.UserPreferenceName
+        value: Page.UserPreferenceValue = OPTIONAL
+    
+    @dataclass
+    class setCookie(ProtocolCommand):
+        """[Just WIP] Sets a new browser cookie with the given name, domain, and path."""
+        cookie: Page.Cookie
+    
+    @dataclass
+    class setBootstrapScript(ProtocolCommand):
+        """[Just WIP]"""
+        source: str = OPTIONAL
+    
+    @dataclass
+    class searchInResources(ProtocolCommand):
+        """[Just WIP] Searches for given string in frame / resource tree structure."""
+        text: str
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class setShowRulers(ProtocolCommand):
+        """[Just WIP] Requests that backend draw rulers in the inspector overlay"""
+        result: bool
+    
+    @dataclass
+    class setShowPaintRects(ProtocolCommand):
+        """[Just WIP] Requests that backend shows paint rectangles"""
+        result: bool
+    
+    @dataclass
+    class setEmulatedMedia(ProtocolCommand):
+        """[Just WIP] Emulates the given media for CSS media queries."""
+        media: str
+    
+    @dataclass
+    class snapshotNode(ProtocolCommand):
+        """[Just WIP] Capture a snapshot of the specified node that does not include unrelated layers."""
+        nodeId: DOM.NodeId
+    
+    @dataclass
+    class snapshotRect(ProtocolCommand):
+        """[Just WIP] Capture a snapshot of the page within the specified rectangle and coordinate system."""
+        x: int
+        y: int
+        width: int
+        height: int
+        coordinateSystem: Page.CoordinateSystem
+    
+    @dataclass
+    class archive(ProtocolCommand):
+        """[Just WIP] Grab an archive of the page."""
+        pass
+    
+    @dataclass
+    class setScreenSizeOverride(ProtocolCommand):
+        """[Just WIP] Overrides screen size exposed to DOM and used in media queries for testing with provided values."""
+        width: int = OPTIONAL
+        height: int = OPTIONAL
+    
 
 @domainclass
 class Performance:
     """[Just CDP]"""
     class Metric:
         """Run-time execution metric."""
         name: str
@@ -5446,36 +5922,36 @@
         schemeIsCryptographic: bool
         explanations: list
         insecureContentStatus: Security.InsecureContentStatus
         summary: str
     
     @dataclass
     class disable(ProtocolCommand):
-        """Disables tracking security state changes."""
+        """[Just CDP] Disables tracking security state changes."""
         pass
     
     @dataclass
     class enable(ProtocolCommand):
-        """Enables tracking security state changes."""
+        """[Just CDP] Enables tracking security state changes."""
         pass
     
     @dataclass
     class setIgnoreCertificateErrors(ProtocolCommand):
-        """Enable/disable whether all certificate errors should be ignored."""
+        """[Just CDP][Experimental] Enable/disable whether all certificate errors should be ignored."""
         ignore: bool
     
     @dataclass
     class handleCertificateError(ProtocolCommand):
-        """Handles a certificate error that fired a certificateError event."""
+        """[Just CDP] Handles a certificate error that fired a certificateError event."""
         eventId: int
         action: Security.CertificateErrorAction
     
     @dataclass
     class setOverrideCertificateErrors(ProtocolCommand):
-        """Enable/disable overriding certificate errors. If enabled, all certificate error events need to
+        """[Just CDP] Enable/disable overriding certificate errors. If enabled, all certificate error events need to
 be handled by the DevTools client and should be answered with `handleCertificateError` commands."""
         override: bool
     
 
 @domainclass
 class ServiceWorker:
     RegistrationID: str
@@ -5522,71 +5998,89 @@
         registrations: list
     
     class workerVersionUpdated(BaseEvent):
         versions: list
     
     @dataclass
     class deliverPushMessage(ProtocolCommand):
+        """[Just CDP]"""
         origin: str
         registrationId: ServiceWorker.RegistrationID
         data: str
     
     @dataclass
     class disable(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class dispatchSyncEvent(ProtocolCommand):
+        """[Just CDP]"""
         origin: str
         registrationId: ServiceWorker.RegistrationID
         tag: str
         lastChance: bool
     
     @dataclass
     class dispatchPeriodicSyncEvent(ProtocolCommand):
+        """[Just CDP]"""
         origin: str
         registrationId: ServiceWorker.RegistrationID
         tag: str
     
     @dataclass
     class enable(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class inspectWorker(ProtocolCommand):
+        """[Just CDP]"""
         versionId: str
     
     @dataclass
     class setForceUpdateOnPageLoad(ProtocolCommand):
+        """[Just CDP]"""
         forceUpdateOnPageLoad: bool
     
     @dataclass
     class skipWaiting(ProtocolCommand):
+        """[Just CDP]"""
         scopeURL: str
     
     @dataclass
     class startWorker(ProtocolCommand):
+        """[Just CDP]"""
         scopeURL: str
     
     @dataclass
     class stopAllWorkers(ProtocolCommand):
+        """[Just CDP]"""
         pass
     
     @dataclass
     class stopWorker(ProtocolCommand):
+        """[Just CDP]"""
         versionId: str
     
     @dataclass
     class unregister(ProtocolCommand):
+        """[Just CDP]"""
         scopeURL: str
     
     @dataclass
     class updateRegistration(ProtocolCommand):
+        """[Just CDP]"""
         scopeURL: str
     
+    @dataclass
+    class getInitializationInfo(ProtocolCommand):
+        """[Just WIP] Returns the initialization information for this target."""
+        pass
+    
 
 @domainclass
 class Storage:
     """[Just CDP][Experimental]"""
     SerializedStorageKey: str
     StorageType: str
     class UsageForType:
@@ -6079,139 +6573,149 @@
     
     class dispatchMessageFromTarget(BaseEvent):
         targetId: str
         message: str
     
     @dataclass
     class activateTarget(ProtocolCommand):
-        """Activates (focuses) the target."""
+        """[Just CDP] Activates (focuses) the target."""
         targetId: Target.TargetID
     
     @dataclass
     class attachToTarget(ProtocolCommand):
-        """Attaches to the target with given id."""
+        """[Just CDP] Attaches to the target with given id."""
         targetId: Target.TargetID
         flatten: bool = OPTIONAL
     
     @dataclass
     class attachToBrowserTarget(ProtocolCommand):
-        """Attaches to the browser target, only uses flat sessionId mode."""
+        """[Just CDP] Attaches to the browser target, only uses flat sessionId mode."""
         pass
     
     @dataclass
     class closeTarget(ProtocolCommand):
-        """Closes the target. If the target is a page that gets closed too."""
+        """[Just CDP] Closes the target. If the target is a page that gets closed too."""
         targetId: Target.TargetID
     
     @dataclass
     class exposeDevToolsProtocol(ProtocolCommand):
-        """Inject object to the target's main frame that provides a communication
+        """[Just CDP] Inject object to the target's main frame that provides a communication
 channel with browser target.
 
 Injected object will be available as `window[bindingName]`.
 
 The object has the follwing API:
 - `binding.send(json)` - a method to send messages over the remote debugging protocol
 - `binding.onmessage = json => handleMessage(json)` - a callback that will be called for the protocol notifications and command responses."""
         targetId: Target.TargetID
         bindingName: str = OPTIONAL
     
     @dataclass
     class createBrowserContext(ProtocolCommand):
-        """Creates a new empty BrowserContext. Similar to an incognito profile but you can have more than
+        """[Just CDP] Creates a new empty BrowserContext. Similar to an incognito profile but you can have more than
 one."""
         disposeOnDetach: bool = OPTIONAL
         proxyServer: str = OPTIONAL
         proxyBypassList: str = OPTIONAL
         originsWithUniversalNetworkAccess: list = OPTIONAL
     
     @dataclass
     class getBrowserContexts(ProtocolCommand):
-        """Returns all browser contexts created with `Target.createBrowserContext` method."""
+        """[Just CDP] Returns all browser contexts created with `Target.createBrowserContext` method."""
         pass
     
     @dataclass
     class createTarget(ProtocolCommand):
-        """Creates a new page."""
+        """[Just CDP] Creates a new page."""
         url: str
         width: int = OPTIONAL
         height: int = OPTIONAL
         browserContextId: Browser.BrowserContextID = OPTIONAL
         enableBeginFrameControl: bool = OPTIONAL
         newWindow: bool = OPTIONAL
         background: bool = OPTIONAL
         forTab: bool = OPTIONAL
     
     @dataclass
     class detachFromTarget(ProtocolCommand):
-        """Detaches session with given id."""
+        """[Just CDP] Detaches session with given id."""
         sessionId: Target.SessionID = OPTIONAL
         targetId: Target.TargetID = OPTIONAL
     
     @dataclass
     class disposeBrowserContext(ProtocolCommand):
-        """Deletes a BrowserContext. All the belonging pages will be closed without calling their
+        """[Just CDP] Deletes a BrowserContext. All the belonging pages will be closed without calling their
 beforeunload hooks."""
         browserContextId: Browser.BrowserContextID
     
     @dataclass
     class getTargetInfo(ProtocolCommand):
-        """Returns information about a target."""
+        """[Just CDP] Returns information about a target."""
         targetId: Target.TargetID = OPTIONAL
     
     @dataclass
     class getTargets(ProtocolCommand):
-        """Retrieves a list of available targets."""
+        """[Just CDP] Retrieves a list of available targets."""
         filter: Target.TargetFilter = OPTIONAL
     
     @dataclass
     class sendMessageToTarget(ProtocolCommand):
         """Sends protocol message over session with given id.
 Consider using flat mode instead; see commands attachToTarget, setAutoAttach,
 and crbug.com/991325."""
         message: str
         sessionId: Target.SessionID = OPTIONAL
         targetId: Target.TargetID = OPTIONAL
     
     @dataclass
     class setAutoAttach(ProtocolCommand):
-        """Controls whether to automatically attach to new targets which are considered to be related to
+        """[Just CDP] Controls whether to automatically attach to new targets which are considered to be related to
 this one. When turned on, attaches to all existing related targets as well. When turned off,
 automatically detaches from all currently attached targets.
 This also clears all targets added by `autoAttachRelated` from the list of targets to watch
 for creation of related targets."""
         autoAttach: bool
         waitForDebuggerOnStart: bool
         flatten: bool = OPTIONAL
         filter: Target.TargetFilter = OPTIONAL
     
     @dataclass
     class autoAttachRelated(ProtocolCommand):
-        """Adds the specified target to the list of targets that will be monitored for any related target
+        """[Just CDP] Adds the specified target to the list of targets that will be monitored for any related target
 creation (such as child frames, child workers and new versions of service worker) and reported
 through `attachedToTarget`. The specified target is also auto-attached.
 This cancels the effect of any previous `setAutoAttach` and is also cancelled by subsequent
 `setAutoAttach`. Only available at the Browser target."""
         targetId: Target.TargetID
         waitForDebuggerOnStart: bool
         filter: Target.TargetFilter = OPTIONAL
     
     @dataclass
     class setDiscoverTargets(ProtocolCommand):
-        """Controls whether to discover available targets and notify via
+        """[Just CDP] Controls whether to discover available targets and notify via
 `targetCreated/targetInfoChanged/targetDestroyed` events."""
         discover: bool
         filter: Target.TargetFilter = OPTIONAL
     
     @dataclass
     class setRemoteLocations(ProtocolCommand):
-        """Enables target discovery for the specified locations, when `setDiscoverTargets` was set to
+        """[Just CDP] Enables target discovery for the specified locations, when `setDiscoverTargets` was set to
 `true`."""
         locations: list
     
+    @dataclass
+    class setPauseOnStart(ProtocolCommand):
+        """[Just WIP] If set to true, new targets will be paused on start waiting for resume command. Other commands can be dispatched on the target before it is resumed."""
+        pauseOnStart: bool
+    
+    @dataclass
+    class resume(ProtocolCommand):
+        """[Just WIP] Will resume target if it was paused on start."""
+        targetId: str
+    
 
 @domainclass
 class Tethering:
     """[Just CDP][Experimental] The Tethering domain defines methods and events for browser port binding."""
 
     class accepted(BaseEvent):
         """Informs that port was successfully bound and got a specified connection id."""
@@ -7036,14 +7540,25 @@
     
     @dataclass
     class enable(ProtocolCommand):
         """Enables console domain, sends the messages collected so far to the client by means of the
 `messageAdded` notification."""
         pass
     
+    @dataclass
+    class getLoggingChannels(ProtocolCommand):
+        """[Just WIP] List of the different message sources that are non-default logging channels."""
+        pass
+    
+    @dataclass
+    class setLoggingChannelLevel(ProtocolCommand):
+        """[Just WIP] Modify the level of a channel."""
+        source: Console.ChannelSource
+        level: Console.ChannelLevel
+    
 
 @domainclass
 class Debugger:
     """Debugger domain exposes JavaScript debugging capabilities. It allows setting and removing
 breakpoints, stepping through execution, exploring stack traces, etc."""
     BreakpointId: str
     CallFrameId: str
@@ -7256,67 +7771,72 @@
         objectGroup: str = OPTIONAL
         includeCommandLineAPI: bool = OPTIONAL
         silent: bool = OPTIONAL
         returnByValue: bool = OPTIONAL
         generatePreview: bool = OPTIONAL
         throwOnSideEffect: bool = OPTIONAL
         timeout: Runtime.TimeDelta = OPTIONAL
+        doNotPauseOnExceptionsAndMuteConsole: bool = OPTIONAL
+        saveResult: bool = OPTIONAL
+        emulateUserGesture: bool = OPTIONAL
     
     @dataclass
     class getPossibleBreakpoints(ProtocolCommand):
-        """Returns possible locations for breakpoint. scriptId in start and end range locations should be
+        """[Just CDP] Returns possible locations for breakpoint. scriptId in start and end range locations should be
 the same."""
         start: Debugger.Location
         end: Debugger.Location = OPTIONAL
         restrictToFunction: bool = OPTIONAL
     
     @dataclass
     class getScriptSource(ProtocolCommand):
         """Returns source for the script with given id."""
         scriptId: Runtime.ScriptId
     
     @dataclass
     class disassembleWasmModule(ProtocolCommand):
+        """[Just CDP]"""
         scriptId: Runtime.ScriptId
     
     @dataclass
     class nextWasmDisassemblyChunk(ProtocolCommand):
-        """Disassemble the next chunk of lines for the module corresponding to the
+        """[Just CDP] Disassemble the next chunk of lines for the module corresponding to the
 stream. If disassembly is complete, this API will invalidate the streamId
 and return an empty chunk. Any subsequent calls for the now invalid stream
 will return errors."""
         streamId: str
     
     @dataclass
     class getWasmBytecode(ProtocolCommand):
-        """This command is deprecated. Use getScriptSource instead."""
+        """[Just CDP] This command is deprecated. Use getScriptSource instead."""
         scriptId: Runtime.ScriptId
     
     @dataclass
     class getStackTrace(ProtocolCommand):
-        """Returns stack trace with given `stackTraceId`."""
+        """[Just CDP] Returns stack trace with given `stackTraceId`."""
         stackTraceId: Runtime.StackTraceId
     
     @dataclass
     class pause(ProtocolCommand):
         """Stops on the next JavaScript statement."""
         pass
     
     @dataclass
     class pauseOnAsyncCall(ProtocolCommand):
+        """[Just CDP]"""
         parentStackTraceId: Runtime.StackTraceId
     
     @dataclass
     class removeBreakpoint(ProtocolCommand):
         """Removes JavaScript breakpoint."""
         breakpointId: Debugger.BreakpointId
     
     @dataclass
     class restartFrame(ProtocolCommand):
-        """Restarts particular call frame from the beginning. The old, deprecated
+        """[Just CDP] Restarts particular call frame from the beginning. The old, deprecated
 behavior of `restartFrame` is to stay paused and allow further CDP commands
 after a restart was scheduled. This can cause problems with restarting, so
 we now continue execution immediatly after it has been scheduled until we
 reach the beginning of the restarted frame.
 
 To stay back-wards compatible, `restartFrame` now expects a `mode`
 parameter to be present. If the `mode` parameter is missing, `restartFrame`
@@ -7339,60 +7859,62 @@
         scriptId: Runtime.ScriptId
         query: str
         caseSensitive: bool = OPTIONAL
         isRegex: bool = OPTIONAL
     
     @dataclass
     class setAsyncCallStackDepth(ProtocolCommand):
-        """Enables or disables async call stacks tracking."""
+        """[Just CDP] Enables or disables async call stacks tracking."""
         maxDepth: int
     
     @dataclass
     class setBlackboxPatterns(ProtocolCommand):
-        """Replace previous blackbox patterns with passed ones. Forces backend to skip stepping/pausing in
+        """[Just CDP] Replace previous blackbox patterns with passed ones. Forces backend to skip stepping/pausing in
 scripts with url matching one of the patterns. VM will try to leave blackboxed script by
 performing 'step in' several times, finally resorting to 'step out' if unsuccessful."""
         patterns: list
     
     @dataclass
     class setBlackboxedRanges(ProtocolCommand):
-        """Makes backend skip steps in the script in blackboxed ranges. VM will try leave blacklisted
+        """[Just CDP] Makes backend skip steps in the script in blackboxed ranges. VM will try leave blacklisted
 scripts by performing 'step in' several times, finally resorting to 'step out' if unsuccessful.
 Positions array contains positions where blackbox state is changed. First interval isn't
 blackboxed. Array should be sorted."""
         scriptId: Runtime.ScriptId
         positions: list
     
     @dataclass
     class setBreakpoint(ProtocolCommand):
         """Sets JavaScript breakpoint at a given location."""
         location: Debugger.Location
         condition: str = OPTIONAL
+        options: Debugger.BreakpointOptions = OPTIONAL
     
     @dataclass
     class setInstrumentationBreakpoint(ProtocolCommand):
-        """Sets instrumentation breakpoint."""
+        """[Just CDP] Sets instrumentation breakpoint."""
         instrumentation: str
     
     @dataclass
     class setBreakpointByUrl(ProtocolCommand):
         """Sets JavaScript breakpoint at given location specified either by URL or URL regex. Once this
 command is issued, all existing parsed scripts will have breakpoints resolved and returned in
 `locations` property. Further matching script parsing will result in subsequent
 `breakpointResolved` events issued. This logical breakpoint will survive page reloads."""
         lineNumber: int
         url: str = OPTIONAL
         urlRegex: str = OPTIONAL
         scriptHash: str = OPTIONAL
         columnNumber: int = OPTIONAL
         condition: str = OPTIONAL
+        options: Debugger.BreakpointOptions = OPTIONAL
     
     @dataclass
     class setBreakpointOnFunctionCall(ProtocolCommand):
-        """Sets JavaScript breakpoint before each call to the given function.
+        """[Just CDP] Sets JavaScript breakpoint before each call to the given function.
 If another function was created from the same source as a given one,
 calling it will also trigger the breakpoint."""
         objectId: Runtime.RemoteObjectId
         condition: str = OPTIONAL
     
     @dataclass
     class setBreakpointsActive(ProtocolCommand):
@@ -7400,42 +7922,43 @@
         active: bool
     
     @dataclass
     class setPauseOnExceptions(ProtocolCommand):
         """Defines pause on exceptions state. Can be set to stop on all exceptions, uncaught exceptions,
 or caught exceptions, no exceptions. Initial pause on exceptions state is `none`."""
         state: str
+        options: Debugger.BreakpointOptions = OPTIONAL
     
     @dataclass
     class setReturnValue(ProtocolCommand):
-        """Changes return value in top frame. Available only at return break position."""
+        """[Just CDP] Changes return value in top frame. Available only at return break position."""
         newValue: Runtime.CallArgument
     
     @dataclass
     class setScriptSource(ProtocolCommand):
-        """Edits JavaScript source live.
+        """[Just CDP] Edits JavaScript source live.
 
 In general, functions that are currently on the stack can not be edited with
 a single exception: If the edited function is the top-most stack frame and
 that is the only activation of that function on the stack. In this case
 the live edit will be successful and a `Debugger.restartFrame` for the
 top-most function is automatically triggered."""
         scriptId: Runtime.ScriptId
         scriptSource: str
         dryRun: bool = OPTIONAL
         allowTopFrameEditing: bool = OPTIONAL
     
     @dataclass
     class setSkipAllPauses(ProtocolCommand):
-        """Makes page not interrupt on any pauses (breakpoint, exception, dom exception etc)."""
+        """[Just CDP] Makes page not interrupt on any pauses (breakpoint, exception, dom exception etc)."""
         skip: bool
     
     @dataclass
     class setVariableValue(ProtocolCommand):
-        """Changes value of variable in a callframe. Object-based scopes are not supported and must be
+        """[Just CDP] Changes value of variable in a callframe. Object-based scopes are not supported and must be
 mutated manually."""
         scopeNumber: int
         variableName: str
         newValue: Runtime.CallArgument
         callFrameId: Debugger.CallFrameId
     
     @dataclass
@@ -7450,14 +7973,91 @@
         pass
     
     @dataclass
     class stepOver(ProtocolCommand):
         """Steps over the statement."""
         skipList: list = OPTIONAL
     
+    @dataclass
+    class setAsyncStackTraceDepth(ProtocolCommand):
+        """[Just WIP] Set the async stack trace depth for the page. A value of zero disables recording of async stack traces."""
+        depth: int
+    
+    @dataclass
+    class addSymbolicBreakpoint(ProtocolCommand):
+        """[Just WIP] Adds a JavaScript breakpoint that pauses execution whenever a function with the given name is about to be called."""
+        symbol: str
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class removeSymbolicBreakpoint(ProtocolCommand):
+        """[Just WIP] Removes a previously added symbolic breakpoint."""
+        symbol: str
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class continueUntilNextRunLoop(ProtocolCommand):
+        """[Just WIP] Continues execution until the current evaluation completes. This will trigger either a Debugger.paused or Debugger.resumed event."""
+        pass
+    
+    @dataclass
+    class stepNext(ProtocolCommand):
+        """[Just WIP] Steps over the expression. This will trigger either a Debugger.paused or Debugger.resumed event."""
+        pass
+    
+    @dataclass
+    class getFunctionDetails(ProtocolCommand):
+        """[Just WIP] Returns detailed information on given function."""
+        functionId: Runtime.RemoteObjectId
+    
+    @dataclass
+    class getBreakpointLocations(ProtocolCommand):
+        """[Just WIP] Returns a list of valid breakpoint locations within the given location range."""
+        start: Debugger.Location
+        end: Debugger.Location
+    
+    @dataclass
+    class setPauseOnDebuggerStatements(ProtocolCommand):
+        """[Just WIP] Control whether the debugger pauses execution before `debugger` statements."""
+        enabled: bool
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class setPauseOnAssertions(ProtocolCommand):
+        """[Just WIP] Set pause on assertions state. Assertions are console.assert assertions."""
+        enabled: bool
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class setPauseOnMicrotasks(ProtocolCommand):
+        """[Just WIP] Pause when running the next JavaScript microtask."""
+        enabled: bool
+        options: Debugger.BreakpointOptions = OPTIONAL
+    
+    @dataclass
+    class setPauseForInternalScripts(ProtocolCommand):
+        """[Just WIP] Change whether to pause in the debugger for internal scripts. The default value is false."""
+        shouldPause: bool
+    
+    @dataclass
+    class setShouldBlackboxURL(ProtocolCommand):
+        """[Just WIP] Sets whether the given URL should be in the list of blackboxed scripts, which are ignored when pausing/stepping/debugging."""
+        url: str
+        shouldBlackbox: bool
+        caseSensitive: bool = OPTIONAL
+        isRegex: bool = OPTIONAL
+    
+    @dataclass
+    class setBlackboxBreakpointEvaluations(ProtocolCommand):
+        """[Just WIP] Sets whether evaluation of breakpoint conditions, ignore counts, and actions happen at the location of the breakpoint or are deferred due to blackboxing."""
+        blackboxBreakpointEvaluations: bool
+    
 
 @domainclass
 class HeapProfiler:
     """[Just CDP][Experimental]"""
     HeapSnapshotObjectId: str
     class SamplingHeapProfileNode:
         """Sampling Heap Profile node. Holds callsite information, allocation statistics and child nodes."""
@@ -7921,14 +8521,15 @@
     
     @dataclass
     class awaitPromise(ProtocolCommand):
         """Add handler to promise with given promise object id."""
         promiseObjectId: Runtime.RemoteObjectId
         returnByValue: bool = OPTIONAL
         generatePreview: bool = OPTIONAL
+        saveResult: bool = OPTIONAL
     
     @dataclass
     class callFunctionOn(ProtocolCommand):
         """Calls function with given declaration on the given object. Object group of the result is
 inherited from the target object."""
         functionDeclaration: str
         objectId: Runtime.RemoteObjectId = OPTIONAL
@@ -7940,31 +8541,33 @@
         awaitPromise: bool = OPTIONAL
         executionContextId: Runtime.ExecutionContextId = OPTIONAL
         objectGroup: str = OPTIONAL
         throwOnSideEffect: bool = OPTIONAL
         uniqueContextId: str = OPTIONAL
         generateWebDriverValue: bool = OPTIONAL
         serializationOptions: Runtime.SerializationOptions = OPTIONAL
+        doNotPauseOnExceptionsAndMuteConsole: bool = OPTIONAL
+        emulateUserGesture: bool = OPTIONAL
     
     @dataclass
     class compileScript(ProtocolCommand):
-        """Compiles expression."""
+        """[Just CDP] Compiles expression."""
         expression: str
         sourceURL: str
         persistScript: bool
         executionContextId: Runtime.ExecutionContextId = OPTIONAL
     
     @dataclass
     class disable(ProtocolCommand):
         """Disables reporting of execution contexts creation."""
         pass
     
     @dataclass
     class discardConsoleEntries(ProtocolCommand):
-        """Discards collected exceptions and console API calls."""
+        """[Just CDP] Discards collected exceptions and console API calls."""
         pass
     
     @dataclass
     class enable(ProtocolCommand):
         """Enables reporting of execution contexts creation by means of `executionContextCreated` event.
 When the reporting gets enabled the event will be sent immediately for each existing execution
 context."""
@@ -7986,43 +8589,49 @@
         timeout: Runtime.TimeDelta = OPTIONAL
         disableBreaks: bool = OPTIONAL
         replMode: bool = OPTIONAL
         allowUnsafeEvalBlockedByCSP: bool = OPTIONAL
         uniqueContextId: str = OPTIONAL
         generateWebDriverValue: bool = OPTIONAL
         serializationOptions: Runtime.SerializationOptions = OPTIONAL
+        doNotPauseOnExceptionsAndMuteConsole: bool = OPTIONAL
+        saveResult: bool = OPTIONAL
+        emulateUserGesture: bool = OPTIONAL
     
     @dataclass
     class getIsolateId(ProtocolCommand):
-        """Returns the isolate id."""
+        """[Just CDP] Returns the isolate id."""
         pass
     
     @dataclass
     class getHeapUsage(ProtocolCommand):
-        """Returns the JavaScript heap usage.
+        """[Just CDP] Returns the JavaScript heap usage.
 It is the total usage of the corresponding isolate not scoped to a particular Runtime."""
         pass
     
     @dataclass
     class getProperties(ProtocolCommand):
         """Returns properties of a given object. Object group of the result is inherited from the target
 object."""
         objectId: Runtime.RemoteObjectId
         ownProperties: bool = OPTIONAL
         accessorPropertiesOnly: bool = OPTIONAL
         generatePreview: bool = OPTIONAL
         nonIndexedPropertiesOnly: bool = OPTIONAL
+        fetchStart: int = OPTIONAL
+        fetchCount: int = OPTIONAL
     
     @dataclass
     class globalLexicalScopeNames(ProtocolCommand):
-        """Returns all let, const and class variables from global scope."""
+        """[Just CDP] Returns all let, const and class variables from global scope."""
         executionContextId: Runtime.ExecutionContextId = OPTIONAL
     
     @dataclass
     class queryObjects(ProtocolCommand):
+        """[Just CDP]"""
         prototypeObjectId: Runtime.RemoteObjectId
         objectGroup: str = OPTIONAL
     
     @dataclass
     class releaseObject(ProtocolCommand):
         """Releases remote object with given id."""
         objectId: Runtime.RemoteObjectId
@@ -8030,75 +8639,144 @@
     @dataclass
     class releaseObjectGroup(ProtocolCommand):
         """Releases all remote objects that belong to a given group."""
         objectGroup: str
     
     @dataclass
     class runIfWaitingForDebugger(ProtocolCommand):
-        """Tells inspected instance to run if it was waiting for debugger to attach."""
+        """[Just CDP] Tells inspected instance to run if it was waiting for debugger to attach."""
         pass
     
     @dataclass
     class runScript(ProtocolCommand):
-        """Runs script with given id in a given context."""
+        """[Just CDP] Runs script with given id in a given context."""
         scriptId: Runtime.ScriptId
         executionContextId: Runtime.ExecutionContextId = OPTIONAL
         objectGroup: str = OPTIONAL
         silent: bool = OPTIONAL
         includeCommandLineAPI: bool = OPTIONAL
         returnByValue: bool = OPTIONAL
         generatePreview: bool = OPTIONAL
         awaitPromise: bool = OPTIONAL
     
     @dataclass
     class setAsyncCallStackDepth(ProtocolCommand):
-        """Enables or disables async call stacks tracking."""
+        """[Just CDP] Enables or disables async call stacks tracking."""
         maxDepth: int
     
     @dataclass
     class setCustomObjectFormatterEnabled(ProtocolCommand):
+        """[Just CDP]"""
         enabled: bool
     
     @dataclass
     class setMaxCallStackSizeToCapture(ProtocolCommand):
+        """[Just CDP]"""
         size: int
     
     @dataclass
     class terminateExecution(ProtocolCommand):
-        """Terminate current or next JavaScript execution.
+        """[Just CDP] Terminate current or next JavaScript execution.
 Will cancel the termination when the outer-most script execution ends."""
         pass
     
     @dataclass
     class addBinding(ProtocolCommand):
-        """If executionContextId is empty, adds binding with the given name on the
+        """[Just CDP] If executionContextId is empty, adds binding with the given name on the
 global objects of all inspected contexts, including those created later,
 bindings survive reloads.
 Binding function takes exactly one argument, this argument should be string,
 in case of any other input, function throws an exception.
 Each binding function call produces Runtime.bindingCalled notification."""
         name: str
         executionContextId: Runtime.ExecutionContextId = OPTIONAL
         executionContextName: str = OPTIONAL
     
     @dataclass
     class removeBinding(ProtocolCommand):
-        """This method does not remove binding function from global object but
+        """[Just CDP] This method does not remove binding function from global object but
 unsubscribes current runtime agent from Runtime.bindingCalled notifications."""
         name: str
     
     @dataclass
     class getExceptionDetails(ProtocolCommand):
-        """This method tries to lookup and populate exception details for a
+        """[Just CDP] This method tries to lookup and populate exception details for a
 JavaScript Error object.
 Note that the stackTrace portion of the resulting exceptionDetails will
 only be populated if the Runtime domain was enabled at the time when the
 Error was thrown."""
         errorObjectId: Runtime.RemoteObjectId
     
+    @dataclass
+    class parse(ProtocolCommand):
+        """[Just WIP] Parses JavaScript source code for errors."""
+        source: str
+    
+    @dataclass
+    class getPreview(ProtocolCommand):
+        """[Just WIP] Returns a preview for the given object."""
+        objectId: Runtime.RemoteObjectId
+    
+    @dataclass
+    class getDisplayableProperties(ProtocolCommand):
+        """[Just WIP] Returns displayable properties of a given object. Object group of the result is inherited from the target object. Displayable properties are own properties, internal properties, and native getters in the prototype chain (assumed to be bindings and treated like own properties for the frontend)."""
+        objectId: Runtime.RemoteObjectId
+        fetchStart: int = OPTIONAL
+        fetchCount: int = OPTIONAL
+        generatePreview: bool = OPTIONAL
+    
+    @dataclass
+    class getCollectionEntries(ProtocolCommand):
+        """[Just WIP] Returns entries of given Map / Set collection."""
+        objectId: Runtime.RemoteObjectId
+        objectGroup: str = OPTIONAL
+        fetchStart: int = OPTIONAL
+        fetchCount: int = OPTIONAL
+    
+    @dataclass
+    class saveResult(ProtocolCommand):
+        """[Just WIP] Assign a saved result index to this value."""
+        value: Runtime.CallArgument
+        contextId: Runtime.ExecutionContextId = OPTIONAL
+    
+    @dataclass
+    class setSavedResultAlias(ProtocolCommand):
+        """[Just WIP] Creates an additional reference to all saved values in the Console using the the given string as a prefix instead of $."""
+        alias: str = OPTIONAL
+    
+    @dataclass
+    class getRuntimeTypesForVariablesAtOffsets(ProtocolCommand):
+        """[Just WIP] Returns detailed information on the given function."""
+        locations: list
+    
+    @dataclass
+    class enableTypeProfiler(ProtocolCommand):
+        """[Just WIP] Enables type profiling on the VM."""
+        pass
+    
+    @dataclass
+    class disableTypeProfiler(ProtocolCommand):
+        """[Just WIP] Disables type profiling on the VM."""
+        pass
+    
+    @dataclass
+    class enableControlFlowProfiler(ProtocolCommand):
+        """[Just WIP] Enables control flow profiling on the VM."""
+        pass
+    
+    @dataclass
+    class disableControlFlowProfiler(ProtocolCommand):
+        """[Just WIP] Disables control flow profiling on the VM."""
+        pass
+    
+    @dataclass
+    class getBasicBlocks(ProtocolCommand):
+        """[Just WIP] Returns a list of basic blocks for the given sourceID with information about their text ranges and whether or not they have executed."""
+        sourceID: str
+    
 
 @domainclass
 class Schema:
     """[Just CDP] This domain is deprecated."""
     class Domain:
         """Description of the protocol domain."""
         name: str
@@ -8618,10 +9296,7 @@
 EventList: List[EventTypes] = [Accessibility.loadComplete, Accessibility.nodesUpdated, Animation.animationCanceled, Animation.animationCreated, Animation.animationStarted, Animation.nameChanged, Animation.effectChanged, Animation.targetChanged, Animation.animationDestroyed, Animation.trackingStart, Animation.trackingUpdate, Animation.trackingComplete, Audits.issueAdded, Autofill.addressFormFilled, BackgroundService.recordingStateChanged, BackgroundService.backgroundServiceEventReceived, Browser.downloadWillBegin, Browser.downloadProgress, Browser.extensionsEnabled, Browser.extensionsDisabled, CSS.fontsUpdated, CSS.mediaQueryResultChanged, CSS.styleSheetAdded, CSS.styleSheetChanged, CSS.styleSheetRemoved, CSS.nodeLayoutFlagsChanged, Cast.sinksUpdated, Cast.issueUpdated, DOM.attributeModified, DOM.attributeRemoved, DOM.characterDataModified, DOM.childNodeCountUpdated, DOM.childNodeInserted, DOM.childNodeRemoved, DOM.distributedNodesUpdated, DOM.documentUpdated, DOM.inlineStyleInvalidated, DOM.pseudoElementAdded, DOM.topLayerElementsUpdated, DOM.pseudoElementRemoved, DOM.setChildNodes, DOM.shadowRootPopped, DOM.shadowRootPushed, DOM.inspect, DOM.willDestroyDOMNode, DOM.customElementStateChanged, DOM.didAddEventListener, DOM.willRemoveEventListener, DOM.didFireEvent, DOM.powerEfficientPlaybackStateChanged, DOMStorage.domStorageItemAdded, DOMStorage.domStorageItemRemoved, DOMStorage.domStorageItemUpdated, DOMStorage.domStorageItemsCleared, Database.addDatabase, Emulation.virtualTimeBudgetExpired, Input.dragIntercepted, Inspector.detached, Inspector.targetCrashed, Inspector.targetReloadedAfterCrash, Inspector.evaluateForTestInFrontend, Inspector.inspect, LayerTree.layerPainted, LayerTree.layerTreeDidChange, Log.entryAdded, Memory.memoryPressure, Memory.trackingStart, Memory.trackingUpdate, Memory.trackingComplete, Network.dataReceived, Network.eventSourceMessageReceived, Network.loadingFailed, Network.loadingFinished, Network.requestIntercepted, Network.requestServedFromCache, Network.requestWillBeSent, Network.resourceChangedPriority, Network.signedExchangeReceived, Network.responseReceived, Network.webSocketClosed, Network.webSocketCreated, Network.webSocketFrameError, Network.webSocketFrameReceived, Network.webSocketFrameSent, Network.webSocketHandshakeResponseReceived, Network.webSocketWillSendHandshakeRequest, Network.webTransportCreated, Network.webTransportConnectionEstablished, Network.webTransportClosed, Network.requestWillBeSentExtraInfo, Network.responseReceivedExtraInfo, Network.trustTokenOperationDone, Network.subresourceWebBundleMetadataReceived, Network.subresourceWebBundleMetadataError, Network.subresourceWebBundleInnerResponseParsed, Network.subresourceWebBundleInnerResponseError, Network.reportingApiReportAdded, Network.reportingApiReportUpdated, Network.reportingApiEndpointsChangedForOrigin, Network.requestServedFromMemoryCache, Network.responseIntercepted, Overlay.inspectNodeRequested, Overlay.nodeHighlightRequested, Overlay.screenshotRequested, Overlay.inspectModeCanceled, Page.domContentEventFired, Page.fileChooserOpened, Page.frameAttached, Page.frameClearedScheduledNavigation, Page.frameDetached, Page.frameNavigated, Page.documentOpened, Page.frameResized, Page.frameRequestedNavigation, Page.frameScheduledNavigation, Page.frameStartedLoading, Page.frameStoppedLoading, Page.downloadWillBegin, Page.downloadProgress, Page.interstitialHidden, Page.interstitialShown, Page.javascriptDialogClosed, Page.javascriptDialogOpening, Page.lifecycleEvent, Page.backForwardCacheNotUsed, Page.loadEventFired, Page.navigatedWithinDocument, Page.screencastFrame, Page.screencastVisibilityChanged, Page.windowOpen, Page.compilationCacheProduced, Page.defaultUserPreferencesDidChange, Performance.metrics, PerformanceTimeline.timelineEventAdded, Security.certificateError, Security.visibleSecurityStateChanged, Security.securityStateChanged, ServiceWorker.workerErrorReported, ServiceWorker.workerRegistrationUpdated, ServiceWorker.workerVersionUpdated, Storage.cacheStorageContentUpdated, Storage.cacheStorageListUpdated, Storage.indexedDBContentUpdated, Storage.indexedDBListUpdated, Storage.interestGroupAccessed, Storage.sharedStorageAccessed, Storage.storageBucketCreatedOrUpdated, Storage.storageBucketDeleted, Storage.attributionReportingSourceRegistered, Target.attachedToTarget, Target.detachedFromTarget, Target.receivedMessageFromTarget, Target.targetCreated, Target.targetDestroyed, Target.targetCrashed, Target.targetInfoChanged, Target.didCommitProvisionalTarget, Target.dispatchMessageFromTarget, Tethering.accepted, Tracing.bufferUsage, Tracing.dataCollected, Tracing.tracingComplete, Fetch.requestPaused, Fetch.authRequired, WebAudio.contextCreated, WebAudio.contextWillBeDestroyed, WebAudio.contextChanged, WebAudio.audioListenerCreated, WebAudio.audioListenerWillBeDestroyed, WebAudio.audioNodeCreated, WebAudio.audioNodeWillBeDestroyed, WebAudio.audioParamCreated, WebAudio.audioParamWillBeDestroyed, WebAudio.nodesConnected, WebAudio.nodesDisconnected, WebAudio.nodeParamConnected, WebAudio.nodeParamDisconnected, WebAuthn.credentialAdded, WebAuthn.credentialAsserted, Media.playerPropertiesChanged, Media.playerEventsAdded, Media.playerMessagesLogged, Media.playerErrorsRaised, Media.playersCreated, DeviceAccess.deviceRequestPrompted, Preload.ruleSetUpdated, Preload.ruleSetRemoved, Preload.prerenderAttemptCompleted, Preload.preloadEnabledStateUpdated, Preload.prefetchStatusUpdated, Preload.prerenderStatusUpdated, Preload.preloadingAttemptSourcesUpdated, FedCm.dialogShown, Console.messageAdded, Console.messageRepeatCountUpdated, Console.messagesCleared, Console.heapSnapshot, Debugger.breakpointResolved, Debugger.paused, Debugger.resumed, Debugger.scriptFailedToParse, Debugger.scriptParsed, Debugger.globalObjectCleared, Debugger.didSampleProbe, Debugger.playBreakpointActionSound, HeapProfiler.addHeapSnapshotChunk, HeapProfiler.heapStatsUpdate, HeapProfiler.lastSeenObjectId, HeapProfiler.reportHeapSnapshotProgress, HeapProfiler.resetProfiles, Profiler.consoleProfileFinished, Profiler.consoleProfileStarted, Profiler.preciseCoverageDeltaUpdate, Runtime.bindingCalled, Runtime.consoleAPICalled, Runtime.exceptionRevoked, Runtime.exceptionThrown, Runtime.executionContextCreated, Runtime.executionContextDestroyed, Runtime.executionContextsCleared, Runtime.inspectRequested, Canvas.canvasAdded, Canvas.canvasRemoved, Canvas.canvasSizeChanged, Canvas.canvasMemoryChanged, Canvas.extensionEnabled, Canvas.clientNodesChanged, Canvas.recordingStarted, Canvas.recordingProgress, Canvas.recordingFinished, Canvas.programCreated, Canvas.programDeleted, Heap.garbageCollected, Heap.trackingStart, Heap.trackingComplete, Worker.workerCreated, Worker.workerTerminated, Worker.dispatchMessageFromWorker, CPUProfiler.trackingStart, CPUProfiler.trackingUpdate, CPUProfiler.trackingComplete, Timeline.eventRecorded, Timeline.recordingStarted, Timeline.recordingStopped, Timeline.autoCaptureStarted, ScriptProfiler.trackingStart, ScriptProfiler.trackingUpdate, ScriptProfiler.trackingComplete, ApplicationCache.applicationCacheStatusUpdated, ApplicationCache.networkStateUpdated]
 EventMap = {event.__name__: event for event in EventList }
 
 def create_event(event_name, params):
     if event_name in EventMap:
         return EventMap[event_name](event_name, params)
     return BaseEvent(event_name, params)
-
-ApplicationCache.disable()
-ApplicationCache.getManifestForFrame(frameId=1)
```

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/title.py` & `minium-1.5.4/minium/externlib/wechat_mp_inspector/title.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/externlib/wechat_mp_inspector/utils.py` & `minium-1.5.4/minium/utils/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,187 @@
-import json
+#!/usr/local/bin/python3
+# -*- coding: utf-8 -*-
+"""
+Author:         yopofeng
+Filename:       utils.py
+Create time:    2021/9/24 21:21
+Description:
+
+"""
 import time
-import traceback
-import logging
+import typing
+from typing import overload, Union
+import types
+import platform
+import re
+import sys
+import inspect
 import threading
+import logging
 import os
-import sys
 import asyncio
-import socket
-import typing
-from functools import wraps
 import functools
 import concurrent.futures
+import json
+import socket
+import subprocess
+from .lazyloader import lazy_import
+def unquote(string):
+    return string.replace('+', ' ').replace("%2F", "/").replace("%7E", "~")
+
 try:
     import urllib
-    urlparse = urllib.urlparse
+    urlencode = urllib.urlencode
+    unquote = urllib.unquote
 except AttributeError:
-    from urllib.parse import urlparse
+    from urllib.parse import urlencode
+    from urllib.parse import unquote
 except ImportError:
-    urlparse = None
+    try:
+        from urllib3.request import urlencode
+    except ModuleNotFoundError:  # 2.0.2 后改了
+        raise RuntimeError("maybe you should install urllib3<2.0")
+
+logger = logging.getLogger("minium")
+
+
+def timeout(duration, interval=1):
+    """
+    重试超时装饰器,在超时之前会每隔{interval}秒重试一次
+    注意：被修饰的函数必须要有非空返回,这是重试终止的条件！！！
+    :param duration: seconds
+    :return:
+    """
+
+    def spin_until_true(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            timeout = time.time() + duration
+            execed = False
+            r = None
+            while not (r or timeout < time.time() and execed):
+                r = func(*args, **kwargs)
+                execed = True
+                if r or timeout < time.time():
+                    return r
+                time.sleep(interval)
+            return r
+
+        return wrapper
+
+    return spin_until_true
+
+
+def retry(cnt, expected_exception=None, report: types.FunctionType=None):
+    """
+    重试固定次数装饰器, 被修饰函数没有raise error则直接返回, 有则最多执行${cnt}次
+    :cnt: 重试次数，函数最多被执行 ${cnt} 次
+    :expected_exception: 命中预期的错误(isinstance(e, expected_exception))才重试, None为所有错误
+    :report: 重试成功后上报
+    """
+    def try_until_no_error(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            _cnt = 0
+            while _cnt < cnt:
+                try:
+                    _cnt += 1
+                    ret = func(*args, **kwargs)
+                except:
+                    if _cnt >= cnt:
+                        raise
+                    e = sys.exc_info()[1]
+                    if expected_exception is None or isinstance(e, expected_exception):
+                        logger.warning(
+                            f'{f"第 {_cnt} 次" if _cnt < cnt else "最后一次"}重新运行{func.__name__}'
+                        )
+                        logger.info(f'原因: {e.__class__.__name__}{str(e.args)}')
+                        continue
+                    raise
+                else:
+                    if report and _cnt > 1:
+                        report(_cnt, func.__name__)
+                    return ret
+        return wrapper
+    return try_until_no_error
+
+
+CatchableType = typing.Union[types.FunctionType, types.MethodType]
+
+
+@overload
+def catch(wrapped: CatchableType, *args: typing.Tuple[Exception, ...]) -> CatchableType:
+    ...
+
+
+@overload
+def catch(*args: typing.Tuple[Exception, ...]) -> CatchableType:
+    ...
+
+
+def catch(*args):
+    """
+    抓获指定/所有exception
+    :wrapped: 被修饰的函数, 如果为空则作为修饰器使用
+    :expected_exception: 指定/所有exception
+    :return: Exception/None
+
+    etc.
+    @catch
+    def catchAllException():
+        raise Exception("test")
+
+    @catch(ValueError, RuntimeError)
+    def catchValueAndRuntimeError():
+        raise ValueError("test")
+
+    def raiseValueError():
+        raise ValueError("test")
+    catch(raiseValueError)() -> ValueError("test")
+    catch(raiseValueError, ValueError)() -> ValueError("test")
+    catch(raiseValueError, ValueError, RuntimeError)() -> ValueError("test")
+    catch(ValueError, RuntimeError)(raiseValueError)() -> ValueError("test")
+    catch(raiseValueError, RuntimeError)() -> raise ValueError("test")
+    """
+    wrapped = None
+    expected_exception = None
+    if len(args) == 0:
+        expected_exception = None
+    elif len(args) >= 1:
+        if inspect.isfunction(args[0]) or inspect.ismethod(args[0]):
+            wrapped = args[0]
+            expected_exception = args[1:] or None
+        else:
+            expected_exception = args
+
+    def try_catch(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                func(*args, **kwargs)
+            except:
+                e = sys.exc_info()[1]
+                if expected_exception is None or isinstance(e, expected_exception):
+                    logger.error("catch error: %s", e)
+                    return e
+                raise
+
+        return wrapper
+
+    if wrapped:
+        return try_catch(wrapped)
+    # 修饰器用法
+    return try_catch
+
+
+class WaitTimeoutError(TimeoutError):
+    pass
 
-logger = logging.getLogger("WMI")
+
+TimeoutErrors = (TimeoutError, WaitTimeoutError, asyncio.exceptions.TimeoutError)
 
 
 class WaitThread(threading.Thread):
     def __init__(
         self,
         group=None,
         target=None,
@@ -31,15 +189,15 @@
         args=(),
         kwargs=None,
         daemon=None,
         semaphore=None,
     ):
         super().__init__(group, target, name, args, kwargs, daemon=daemon)
         self._result = None
-        self._exception = None
+        self._exception: BaseException = None
         self._semaphore: threading.Semaphore = semaphore
 
     def run(self):
         try:
             if self._target:
                 self._result = self._target(*self._args, **self._kwargs)
         except:
@@ -53,163 +211,132 @@
 
     def get_result(self, timeout=None, block=True):
         if block:
             self.join(timeout=timeout)
         if self._exception:
             raise self._exception
         if block and self.is_alive():
-            raise TimeoutError("wait [%s] seconds timeout" % timeout)
+            raise WaitTimeoutError("wait [%s] seconds timeout" % timeout)
         return self._result
 
 
-def thread_all(ts: typing.List[WaitThread]):
-    """并行执行多个线程, 返回所有的结果
-
-    :param typing.List[WaitThread] ts: 线程组
+def wait(timeout, default=None):
+    """
+    等待修饰器
+    等待timeout时间, 如果函数没有返回则返回default
     """
-    for t in ts:
-        t.start()
-    for t in ts:
-        t.join()
-    return [t._exception or t._result  for t in ts]
-
-def thread_race(ts: typing.List[WaitThread], timeout: int=None) -> typing.Any:
-    """并行执行多个线程, 返回最快的一个结果
-
-    :param typing.List[WaitThread] ts: 线程组
-    :param int timeout: 等待超时时间, None == 一直等
-    :raises TimeoutError: 等待结果超时
-    :return typing.Any: 结果
-    """
-    semaphore = threading.Semaphore(0)
-    for t in ts:
-        t._semaphore = semaphore
-        t.start()
-    if not semaphore.acquire(timeout=timeout):
-        raise TimeoutError(f"{len(ts)} threads race timeout")
-    for t in ts:
-        if not t.is_alive():
-            return t.get_result()
-
-def thread_wait(ts: typing.List[WaitThread], expected: typing.Any, timeout: int=None):
-    """并行执行多个线程, 等待预期结果
-
-    :param typing.List[WaitThread] ts: 线程组
-    :param typing.Any expected: 期待值, not None
-    :param int timeout: 等待超时时间, None == 一直等
-    :raises ValueError: 等不到结果
-    """
-    semaphore = threading.Semaphore(0)
-    for t in ts:
-        t._semaphore = semaphore
-        t.start()
-    cnt = len(ts)
-    exp = None
-    while cnt and semaphore.acquire(timeout=timeout):
-        cnt -= 1
-        for t in ts:
-            if not t.is_alive() and t._result == expected:
-                return t.get_result()
-            elif not t.is_alive() and t._exception:
-                exp = t._exception
-    raise ValueError("wait expected value error") from exp
-
-class Callback(object):
-    def __init__(self, callback=None) -> None:
-        self.__callback = callback
-        self.__called = threading.Semaphore(0)
-        self.__is_called = False
-        self.__callback_result = None
-        self.__callback_results = []  # 累积的结果
-
-    def callback(self, params):
-        self.__is_called = True
-        self.__callback_result = params
-        self.__callback_results.append(self.__callback_result)
-        self.__called.release()
-        if self.__callback:
-            self.__callback(params)
-
-    @property
-    def is_called(self):
-        """callback曾被调用过
 
-        :return bool: True: called, False: never called
-        """
-        return self.__is_called
+    def spin_until_true(func):
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs):
+            t = WaitThread(target=func, args=args, kwargs=kwargs)
+            t.setDaemon(True)
+            t.start()
+            try:
+                return t.get_result(timeout)
+            except WaitTimeoutError:
+                logger.error("wait %s %ss timeout" % (func.__name__, timeout))
+                return default
 
-    @property
-    def result(self):
-        """最后一个结果
+        return wrapper
 
-        :return any: 回调结果
-        """
-        return self.__callback_result
+    return spin_until_true
 
-    @property
-    def results(self):
-        """返回所有结果
 
-        :return list[any]: 所有回调结果
-        """
-        return list(self.__callback_results)
+_platform = platform.platform()
+isWindows = "Windows" in _platform
+isMacOS = "Darwin" in _platform or "macOS" in _platform
+
+
+class Version(object):
+    def __init__(self, version: str) -> None:
+        m = re.match(r"^([0-9\.]+|latest|dev|trial)", version or "")
+        if not m:
+            raise ValueError(f"{version} format not collect")
+        self.version = "latest" if m.group(1) in ("latest", "dev", "trial") else m.group(1)
+
+    def __str__(self) -> str:
+        return self.version
+
+    def __comp_version(self, a: str, b: str) -> int:
+        """
+        description: 对比基础库版本
+        param {*} self
+        param {str} a
+        param {str} b
+        return {int} 1 if a > b, 0 if a == b ,-1 if a < b
+        """
+        latest = ("latest", "dev")  # latest, dev版本看作是最大的版本号
+        if a in latest:
+            return 0 if b in latest else 1
+        if b in latest:
+            return 0 if a in latest else 1
+        i = 0
+        a = a.split(".")
+        b = b.split(".")
+        while i < len(a) and i < len(b):
+            if int(a[i]) > int(b[i]):
+                return 1
+            elif int(a[i]) < int(b[i]):
+                return -1
+            i += 1
+        return 0
+
+    def __lt__(self, version):
+        if isinstance(version, str):
+            version = Version(version)
+        if self.__comp_version(self.version, version.version) == -1:
+            return True
+        return False
 
-    def acquire(self, timeout=10):
-        """acquire next callback
+    def __gt__(self, version):
+        if isinstance(version, str):
+            version = Version(version)
+        if self.__comp_version(self.version, version.version) == -1:
+            return False
+        return True
 
-        :param int timeout: wait seconds, defaults to 10
-        """
-        return self.__called.acquire(timeout=timeout)
+    def __le__(self, version):
+        if isinstance(version, str):
+            version = Version(version)
+        if self.__comp_version(self.version, version.version) != 1:
+            return True
+        return False
 
-    def wait_called(self, timeout=10) -> bool:
-        """
-        等待回调调用, 默认等待最多10s
-        """
-        if self.__is_called:
+    def __ge__(self, version):
+        if isinstance(version, str):
+            version = Version(version)
+        if self.__comp_version(self.version, version.version) != -1:
             return True
-        return self.acquire(timeout=timeout)
+        return False
 
-    def get_callback_result(self, timeout=0) -> any:
-        """
-        获取回调结果, 超时未获取到结果报AssertionError
-        1. 回调参数只有一个的情况会解构
-        2. 回调参数中有多个的情况会直接返回参数list
-        """
-        if self.wait_called(timeout):
-            return self.__callback_result
-        assert self.__is_called, f"No callback received within {timeout} seconds"
+    def __eq__(self, version):
+        if isinstance(version, str):
+            version = Version(version)
+        return self.version == version.version
 
-    def get_all_result(self):
-        """获取所有结果, 并清空回调状态
 
-        :return list[any]: 所有结果
-        """
-        results = self.__callback_results
-        self.__callback_results = []
-        self.__is_called = False
-        while self.__called.acquire(False):
-            pass
-        return results
+def add_path_to_env(path: str):
+    """
+    把路径添加到PATH环境变量中
+    """
+    SPLIT = ":" if isMacOS else ";"
+    _path = path if os.path.isdir(path) else os.path.dirname(path)
+    env_paths = (os.environ["PATH"] or "").split(SPLIT)
+    if _path not in env_paths:
+        env_paths.append(_path)
+    os.environ["PATH"] = SPLIT.join(env_paths)
+
 
 class ProcessSafeEventLoop(object):
-    def __init__(self, loop: asyncio.AbstractEventLoop=None) -> None:
+    def __init__(self) -> None:
         self.pid = os.getpid()
-        if loop is not None:
-            self.loop = loop
-            asyncio.set_event_loop(self.loop)
-            if not self.loop.is_running():
-                self.run_loop()
-                return
-        try:
-            self.loop = asyncio.get_running_loop()
-            logger.warning("use current loop")
-        except RuntimeError:
-            self.loop = asyncio.new_event_loop()
-            asyncio.set_event_loop(self.loop)
-            self.run_loop()
+        self.loop = asyncio.new_event_loop()
+        asyncio.set_event_loop(self.loop)
+        self.run_loop()
 
     def run_loop(self):
         threading.Thread(target=self.loop.run_forever, daemon=True).start()
 
     def stop_loop(self):
         self.loop.stop()
 
@@ -226,19 +353,14 @@
 
     def is_running(self):
         return self.loop.is_running()
 
     def __getattr__(self, name):
         return getattr(self.loop, name)
 
-Future = typing.Union[asyncio.futures.Future, concurrent.futures.Future]
-EventLoop = typing.Union[ProcessSafeEventLoop, asyncio.BaseEventLoop]
-class WaitTimeoutError(TimeoutError):
-    pass
-
 
 async def _cancel_and_wait(fut, loop):
     """Cancel the *fut* future or task and wait until it completes."""
 
     waiter = loop.create_future()
     cb = functools.partial(_release_waiter, waiter)
     fut.add_done_callback(cb)
@@ -254,15 +376,15 @@
 
 def _release_waiter(waiter, *args):
     if not waiter.done():
         waiter.set_result(None)
 
 
 async def async_wait(
-    fut, timeout, loop: ProcessSafeEventLoop or asyncio.AbstractEventLoop = None
+    fut, timeout, loop: Union[ProcessSafeEventLoop, asyncio.AbstractEventLoop] = None
 ):
     """
     reference asyncio.wait_for
     wait fut done, when timeout, raise
     """
     if loop is None:
         loop = asyncio.get_running_loop()
@@ -306,43 +428,20 @@
                 raise WaitTimeoutError() from exc
             else:
                 raise WaitTimeoutError()
     finally:
         timeout_handle.cancel()
 
 
-def get_result(
-    fut: Future,
-    timeout=None,
-    default=None,
-):
-    # asyncio.futures.Future.result 去掉了timeout参数
-    if isinstance(fut, concurrent.futures.Future):
-        try:
-            return fut.result(timeout)
-        except concurrent.futures.TimeoutError as ext:
-            if default is not None:
-                return default
-            raise WaitTimeoutError() from ext
-    loop = fut.get_loop()
-    try:
-        return asyncio.run_coroutine_threadsafe(
-            async_wait(fut, timeout=timeout, loop=loop), loop=loop
-        ).result()
-    except WaitTimeoutError as ext:
-        if default is not None:
-            return default
-        raise WaitTimeoutError() from ext
-
 class AsyncCondition(asyncio.Condition):
     def __init__(
         self,
         lock: asyncio.Lock = None,
         *,
-        loop: asyncio.AbstractEventLoop or ProcessSafeEventLoop = None,
+        loop: Union[asyncio.AbstractEventLoop, ProcessSafeEventLoop] = None,
     ) -> None:
         if isinstance(loop, ProcessSafeEventLoop):
             loop = loop.loop
         if sys.version_info < (3, 10):
             super().__init__(lock, loop=loop)
         else:  # loop参数将在3.10废除
             asyncio.set_event_loop(loop)
@@ -354,75 +453,41 @@
         if timeout is None:
             return await coro
         try:
             return await async_wait(coro, timeout=timeout, loop=loop)
         except WaitTimeoutError:
             return False
 
-class AsyncCallback(object):
-    def __init__(self, loop: EventLoop = None) -> None:
-        if loop is None:
-            self._loop = asyncio.get_running_loop()
-        else:
-            self._loop = loop
-        self._is_called = False
-        self._waiter: Future = self._loop.create_future()
-
-    async def set_result(self, args):
-        if not self._waiter.done():
-            self._is_called = True
-            result = args[0] if args and len(args) == 1 else args
-            if isinstance(result, BaseException):
-                self._waiter.set_exception(result)
-            else:
-                self._waiter.set_result(result)
 
-    def cancel(self):
-        self._waiter.cancel()
-
-    def callback(self, *args):
-        if not self._waiter.done():
-            self._loop.run_coroutine(self.set_result(args))
+Future = typing.Union[asyncio.futures.Future, concurrent.futures.Future]
+EventLoop = typing.Union[ProcessSafeEventLoop, asyncio.BaseEventLoop]
 
-    @property
-    def is_called(self):
-        return self._waiter.done()
 
-    def wait_called(self, timeout=10) -> bool:
-        """
-        等待回调调用, 默认等待最多10s
-        """
-        if timeout == 0:
-            return self._waiter.done()
-        if self._waiter.done():
-            return True
+def get_result(
+    fut: Future,
+    timeout=None,
+    default=None,
+):
+    # asyncio.futures.Future.result 去掉了timeout参数
+    if isinstance(fut, concurrent.futures.Future):
         try:
-            return self._loop.run_coroutine(
-                async_wait(self._waiter, timeout, self._loop)
-            ).result()
-        except WaitTimeoutError:
-            return False
-        except Exception:
-            return self._waiter.done()
-
-    def get_callback_result(self, timeout=0) -> any:
-        if self.wait_called(timeout):
-            try:
-                return self._waiter.result()
-            except Exception:
-                return sys.exc_info()[1]
-        assert self._is_called, f"No callback received within {timeout} seconds"
-
-    def get_result(self, timeout=0):
-        """
-        获取回调结果, 结果如果为exception直接抛出, 超时未获取到则抛MiniTimeoutError
-        """
-        if self.wait_called(timeout):
-            return self._waiter.result()
-        raise WaitTimeoutError(f"No callback received within {timeout} seconds")
+            return fut.result(timeout)
+        except concurrent.futures.TimeoutError as ext:
+            if default is not None:
+                return default
+            raise WaitTimeoutError() from ext
+    loop = fut.get_loop()
+    try:
+        return asyncio.run_coroutine_threadsafe(
+            async_wait(fut, timeout=timeout, loop=loop), loop=loop
+        ).result()
+    except WaitTimeoutError as ext:
+        if default is not None:
+            return default
+        raise WaitTimeoutError() from ext
 
 
 class Object(dict):
     def __init__(self, __map=None, **kwargs):
         if __map:
             kwargs.update(__map)
         extend = {}
@@ -437,67 +502,104 @@
         try:
             return self[__k]
         except KeyError:
             return None
 
     def __setattr__(self, __k, __v):
         if isinstance(__v, dict):
-            __v = Object(__v)
+            __v = self.__class__(__v)
         if isinstance(__v, list):
             for index, v in enumerate(__v):
                 if isinstance(v, dict):
-                    __v[index] = Object(v)
+                    __v[index] = self.__class__(v)
         if hasattr(self.__class__, __k):
             super(Object, self).__setattr__(__k, __v)
         else:
             self[__k] = __v
 
     @classmethod
     def parse_from_file(cls, file_path):
         if not os.path.isfile(file_path):
             raise RuntimeError(f"{file_path} not exists")
         with open(file_path, "r", encoding="utf8") as fp:
             return cls(json.load(fp))
-
-
-def json2obj(data):
-    try:
-        return json.loads(data, object_hook=Object)
-    except (TypeError, json.JSONDecodeError):
-        return None
-
-
+        
 def pick_unuse_port():
     s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     s.bind(("localhost", 0))
     addr, port = s.getsockname()
     s.close()
     return port
 
 def cost_debug(target: int=5):
     """耗时监测修饰器, 需要调用self.logger打印提示信息
 
     :param int target: 检测耗时目标时间, defaults to 5
     """
     def _cost_debug(func):
-        @wraps(func)
+        @functools.wraps(func)
         def wrapper(self, *args, **kwargs):
             st = time.time()
             try:
                 return func(self, *args, **kwargs)
             finally:
                 cost = time.time() - st
                 if cost > target:
                     getattr(self, "logger", logger).debug("call %s cost %.3fs" % (func.__name__, cost))
         return wrapper
     return _cost_debug
 
-def get_url_path(url):
-    if not url:
-        return ""
-    if urlparse:
-        path = urlparse(url).path
+if typing.TYPE_CHECKING:
+    import cv2
+else:
+    cv2 = lazy_import("cv2")
+
+
+def mark_tap_point(img_path: str, point: typing.Tuple, offset_y=0):
+    if not cv2:
+        return False
+    # print("@mark_tap_point paint %d, %d, %d" % (int(point[0]), int(point[1]), offset_y))
+    img = cv2.imread(img_path)
+    cv2.circle(img, (int(point[0]), int(point[1] + offset_y)), 20, (255, 0, 0), -1)
+    cv2.imwrite(img_path, img)
+    return True
+
+# 根据给定矩形信息裁剪图片
+def crop_img(img_path: str, rect: typing.Tuple):
+    """根据给定矩形信息裁剪图片
+
+    :param str img_path: 图片路径
+    :param typing.Tuple rect: x,y,w,h. w 默认img.shape[1] - x, h 默认img.shape[0] - y
+    :return _type_: _description_
+    """
+    if not cv2:
+        return False
+    img = cv2.imread(img_path)
+    x, y, w, h = rect
+    if w is None:
+        w = img.shape[1] - x
+    if h is None:
+        h = img.shape[0] - y
+    img = img[y:y + h, x:x + w]
+    cv2.imwrite(img_path, img)
+    # cv2.imwrite(os.path.join(os.path.dirname(img_path), "tmp.png"), img)
+    return True
+
+
+def do_shell(cmd):
+    process = subprocess.Popen(
+        cmd,
+        stdin=subprocess.PIPE,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        shell=True,
+    )
+    output = process.communicate()[0].strip()
+    if isinstance(output, bytes):
+        return str(output, encoding="utf-8")
     else:
-        path = "/".join(url.split("/")[3:])
-    if not path:  #没有path, 直接返回原url
-        return url
-    return path
+        return str(output)
+
+if __name__ == "__main__":
+    offset = 298
+    crop_img("/Users/yopofeng/workspace/minium/minitest-demo/testcase/outputs/20231218174636/test_allow_get_location/20231218174935948727/images/1702892976.png", [0, 154, None, None])
+    crop_img("/Users/yopofeng/workspace/minium/minitest-demo/testcase/outputs/20231218174636/test_allow_get_user_info/20231218174944858842/images/1702892985.png", [0, 0, None, 154])
```

### Comparing `minium-1.5.3/minium/externlib/wx_wda/wdaUI.py` & `minium-1.5.4/minium/externlib/wx_wda/wdaUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,24 @@
 
 class WdaUI(object):
     def __init__(self, server_url=None, bundle_id=None):
         if server_url is None:
             server_url = "http://localhost:8100"
         logger.info("启动 %s" % bundle_id)
         self.client = wda.Client(server_url)
-        self.session = self.client.session(bundle_id)
+        self.session = None
+        try:
+            # check app state
+            res = self.client.session().app_state(bundle_id)
+            if res.value == 4:  # 不需要重新拉起了
+                self.session = self.client.session()
+        except Exception:
+            pass
+        if not self.session:
+            self.session = self.client.session(bundle_id)
         self._height = 0
         self._width = 0
 
     def reconnect(self):  # reconnect session
         self.session = self.client.session()
 
     def set_alert_callback(self, callback):
```

### Comparing `minium-1.5.3/minium/framework/assertbase.py` & `minium-1.5.4/minium/framework/assertbase.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/casedump.py` & `minium-1.5.4/minium/framework/casedump.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/caseinspect.py` & `minium-1.5.4/minium/framework/caseinspect.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/css/app.a0b163c8.css` & `minium-1.5.4/minium/framework/dist/css/app.a0b163c8.css`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/css/chunk-vendors.1d2c6903.css` & `minium-1.5.4/minium/framework/dist/css/chunk-vendors.1d2c6903.css`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/favicon.ico` & `minium-1.5.4/minium/framework/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/fonts/element-icons.535877f5.woff` & `minium-1.5.4/minium/framework/dist/fonts/element-icons.535877f5.woff`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/fonts/element-icons.732389de.ttf` & `minium-1.5.4/minium/framework/dist/fonts/element-icons.732389de.ttf`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/index.html` & `minium-1.5.4/minium/framework/dist/index.html`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/js/app.f6da66fe.js` & `minium-1.5.4/minium/framework/dist/js/app.f6da66fe.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/dist/js/chunk-vendors.76d61689.js` & `minium-1.5.4/minium/framework/dist/js/chunk-vendors.76d61689.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/exception.py` & `minium-1.5.4/minium/framework/exception.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/libs/tgit/auth.py` & `minium-1.5.4/minium/framework/libs/tgit/auth.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/libs/tgit/client.py` & `minium-1.5.4/minium/framework/libs/tgit/client.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/libs/unittest/case.py` & `minium-1.5.4/minium/framework/libs/unittest/case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import types
 import contextlib
+from typing import Union
 from functools import wraps
 from unittest.case import (
     addModuleCleanup,
     FunctionTestCase,
     SkipTest,
     skip,
     skipIf as skipIfSrc,
@@ -474,15 +475,15 @@
         need_skip = func()
     elif func.__code__.co_argcount == 1:
         need_skip = func(args[0])  # just use TestCase
     else:
         need_skip = func(*args, **kwargs)  # mybe ddt case
     return need_skip
 
-def skipIf(func_or_condition: types.FunctionType or bool, reason=''):
+def skipIf(func_or_condition: Union[types.FunctionType, bool], reason=''):
     """
     Skip a test if the condition is true.
     """
     if isinstance(func_or_condition, bool):
         return skipIfSrc(func_or_condition, reason)
     def wrapper(wrapped):
         @wraps(wrapped)
@@ -497,15 +498,15 @@
             # normal wrapped func
             if _whether_need_skip(func_or_condition, *args, **kwargs):
                 raise SkipTest(reason)
             return wrapped(*args, **kwargs)
         return inner
     return wrapper
 
-def expectedException(exception_or_type: Exception or type):
+def expectedException(exception_or_type: Union[Exception, type]):
     def wrapper(wrapped):
         @wraps(wrapped)
         def inner(self: TestCase, *args, **kwargs):
             if isinstance(exception_or_type, type):
                 _type = exception_or_type
                 _value = None
             else:
```

### Comparing `minium-1.5.3/minium/framework/libs/unittest/suite.py` & `minium-1.5.4/minium/framework/libs/unittest/suite.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/loader.py` & `minium-1.5.4/minium/framework/loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
             for tests in copy.deepcopy(g_case_list):
                 new_q.put(tests)
             q = new_q
         if only_native:
             c.only_native = True
         logger.info(f"start session with {run_mode} mode \n{c}\n")
         s = Session(conf=c, queue=q, generate_report=generate_report)
+        s.daemon = True
         s.start()
         session_list.append(s)
 
     rest_time = task_limit_time  # 任务剩余时间
     for se in session_list:
         stime = time.time()
         se.join(rest_time)
```

### Comparing `minium-1.5.3/minium/framework/logcolor.py` & `minium-1.5.4/minium/framework/logcolor.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/miniconfig.py` & `minium-1.5.4/minium/framework/miniconfig.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-22
 import os
 import json
 import logging
 import yaml
 import copy
+from typing import TypedDict, Union, Optional
 
 logger = logging.getLogger("minium")
 
 
 class Path(str):
     pass
 
 
+class IOSDevice(TypedDict):
+    udid: str
+    model: Optional[str]
+    version: Optional[str]
+    name: Optional[str]
+
+class IOSDesire(TypedDict):
+    device_info: IOSDevice
+    wda_bundle: Optional[str]
+    wda_project_path: Optional[str]
+
+
+class AndroidDesire(TypedDict):
+    serial: Optional[str]
+    uiautomator_version: Optional[int]
+
+
+
 default_config = {
     "debug": False,                             # debug模式
     "base_dir": os.path.abspath(os.getcwd()),   # 如果没有配置, 默认工作目录, 如果通过文件生成则为文件所在目录
     "platform": "ide",                          # 平台: ide, android, ios
     "app": "wx",                                # 承载的app: wx
     "debug_mode": "debug",                      # 日志级别
     "close_ide": False,                         # 是否关闭IDE
```

### Comparing `minium-1.5.3/minium/framework/miniddt.py` & `minium-1.5.4/minium/framework/miniddt.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/minilimit.py` & `minium-1.5.4/minium/framework/minilimit.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/miniprogram.py` & `minium-1.5.4/minium/framework/miniprogram.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/miniresult.py` & `minium-1.5.4/minium/framework/miniresult.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/minisuite.py` & `minium-1.5.4/minium/framework/minisuite.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/minitest.py` & `minium-1.5.4/minium/framework/minitest.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,38 +7,57 @@
 import time
 import inspect
 import copy
 
 import minium
 import minium.miniprogram.base_driver.minium_log
 import minium.native
+import xml.dom.minidom
 from minium.native.exception import *
 from .miniconfig import MiniConfig
 from .assertbase import AssertBase, HookAssert
 from .libs.unittest import SkipTest
 from .logcolor import *
 from .exception import *
 from ..utils.utils import retry, catch, crop_img
 from .miniprogram import MiniProgram
 from ..miniprogram import Minium
 from ..miniprogram.base_driver.app import App
 from ..miniprogram.base_driver.page import Page
 from ..miniprogram.base_driver.element import BaseElement
 from ..native import NativeType
-from typing import Tuple
+from typing import Tuple, List, TypedDict, Dict, Literal, Optional, Union
 from minium.miniprogram.base_driver.minium_log import report_exception, ExceptionData
 
 # import matplotlib.pyplot as plt
 
 logger = logging.getLogger("minium")
 
+# {timestamp: float, start_timestamp: int, request: Union[dict, None], end_timestamp: int, response: Union[dict, None}]
+class NetworkMessage(TypedDict):
+    timestamp: float
+    start_timestamp: int
+    request: Optional[dict]
+    response: Optional[dict]
+    end_timestamp: int
+
+# {"type": "log|warn|error", "message": str, "dt": str}
+class LogMessage(TypedDict):
+    __required_keys__ = ["type", "dt"]
+    __optional_keys__ = ["args", "message"]
+    type: Literal["log", "warn", "error"]
+    message: str
+    args: List[str]
+    dt: str
+
+
 g_minium: Minium = None
 g_native: NativeType = None
-g_log_message_list = []
-g_network_message_dict = {}  # 记录请求消息
+g_log_message_list: List[LogMessage] = []
+g_network_message_dict: Dict[str, NetworkMessage] = {}  # 记录请求消息
 g_network_req_cache = {}  # 记录请求体消息(降低重复请求消息量)
 g_network_resp_cache = {}  # 记录请求返回消息(降低重复请求消息量)
 FRAMEWORK_RETRY = 1  # case失败, 框架针对错误进行重试的次数
 NATIVE_CACHE = {}  # platform -> native
 
 
 def full_reset():
@@ -224,38 +243,43 @@
         "type": "error",
         "args": [message["message"] + "\n\n" + message["stack"],]
     }
     g_log_message_list.append(msg)
 
 
 def send_request(message):
-    [msg_id, obj, ms, hash_id] = message["args"]
+    [msg_id, obj, ms, hash_id, page] = message["args"]
     if hash_id and obj:  # 传了原始request obj, 记录起来
         g_network_req_cache[hash_id] = {"obj": obj, "timestamp": time.time()}
     elif hash_id and hash_id in g_network_req_cache:
         obj = g_network_req_cache[hash_id]["obj"]
         g_network_req_cache[hash_id]["timestamp"] = time.time()
     if msg_id not in g_network_message_dict:
-        g_network_message_dict[msg_id] = {"timestamp": time.time() * 1000}
-    g_network_message_dict[msg_id]["start_timestamp"] = ms
-    g_network_message_dict[msg_id]["request"] = json.loads(obj)
+        g_network_message_dict[msg_id] = info = {"timestamp": time.time() * 1000}
+    else:
+        info = g_network_message_dict[msg_id]
+    info["start_timestamp"] = ms
+    info["page"] = page
+    info["request"] = json.loads(obj)
 
 
 def request_callback(message):
     [msg_id, res, ms, hash_id, mocked] = message["args"]
     if hash_id and res:  # 传了原始response res, 记录起来
         g_network_resp_cache[hash_id] = {"res": res, "timestamp": time.time()}
     elif hash_id and hash_id in g_network_resp_cache:
         res = g_network_resp_cache[hash_id]["res"]
         g_network_resp_cache[hash_id]["timestamp"] = time.time()
     if msg_id not in g_network_message_dict:
-        g_network_message_dict[msg_id] = {"timestamp": time.time() * 1000}
-    g_network_message_dict[msg_id]["end_timestamp"] = ms
-    g_network_message_dict[msg_id]["response"] = json.loads(res)
-    g_network_message_dict[msg_id]["mocked"] = bool(mocked)
+        g_network_message_dict[msg_id] = info = {"timestamp": time.time() * 1000}
+    else:
+        info = g_network_message_dict[msg_id]
+    info["end_timestamp"] = ms
+    info["response"] = json.loads(res)
+    info["mocked"] = bool(mocked)
 
 
 class MetaMiniTest(HookAssert):
     def __new__(cls, name, bases, attrs):
         return super(MetaMiniTest, cls).__new__(cls, name, bases, attrs)
 
     @property
@@ -275,14 +299,15 @@
     mini: Minium = None
     native: NativeType = None
     appId = ""
     appName = ""
     logger = logger
 
     _app: App = None
+    _app_launch_time = None
 
     def __init__(self, methodName: str = "runTest") -> None:
         super().__init__(methodName)
         # 这个case是否需要重试, 目前重试原则为
         # 1. case运行过程中遇到断连的情况
         self.__will_retry = None
 
@@ -413,15 +438,15 @@
                     reset_minium()
                     self._update_miniprogram(self.native, None)
                 self.init_miniprogram()
 
             if check_result == ResetError.OK and self.test_config.check_mp_foreground:
                 ret = self.native and self.native.back_to_miniprogram()
                 if ret and ret != ResetError.OK:
-                    if ret == ResetError.RELAUNCH_APP:
+                    if ret == ResetError.RELAUNCH_APP or ret == ResetError.ERROR:
                         self.logger.warning(
                             "back_to_miniprogram error, reset app, post native: %s, minium: %s"
                             % (id(self.mini), id(self.native))
                         )
                         full_reset()
                         self._update_miniprogram(None, None)
                         self.init_miniprogram()
@@ -430,18 +455,19 @@
                             "back_to_miniprogram error, reset miniprogram, post minium: %s"
                             % id(self.native)
                         )
                         reset_minium()
                         self._update_miniprogram(self.native, None)
                         self.init_miniprogram()
             if self.test_config.auto_relaunch:
-                self.app.go_home()
+                self.mini.app.go_home()
         # 体验评分是个整体的评价，每个case太短了，没意义
         # if self.test_config.audits:
         #     self._is_audits_setup = self._setup_audits()
+        self._app_launch_time = self.mini.last_launch_time
         self._framework_capture("setup")
         self._is_perf_setup = self._setup_perf()
         # update start_timestamp
         self.results["start_timestamp"] = time.time()
         logger.info("=========case: %s start=========" % self._testMethodName)
 
     def _setup_perf(self):
@@ -568,29 +594,29 @@
         if not self._is_audits_setup:
             return
         if self.start_audit:
             self.stop_audits()
         self.results["audit_html"] = self.audit_html
         self.results["audit_json"] = self.audit_json
 
-    def get_weapp_logs(self) -> []:
+    def get_weapp_logs(self) -> List[LogMessage]:
         """返回当前case运行期间捕获的小程序日志, 包括jserror
 
         :return [{"type": "log|warn|error", "message": str, "dt": str}]: 消息列表
         """
         log_messages = g_log_message_list
         return [
             {"type": log["type"], "message": (log["args"][0] if len(log["args"]) else ""), "dt": log["dt"]}
             for log in log_messages
         ]
     
-    def get_current_requests(self) -> []:
+    def get_current_requests(self):
         """返回当前case运行期间捕获的小程序请求日志
 
-        :return [{timestamp: float, start_timestamp: int, request: dict or None, end_timestamp: int, response: dict or None}]: 消息列表
+        :return [{timestamp: float, start_timestamp: int, request: Union[dict, None], end_timestamp: int, response: Union[dict, None]}]: 消息列表
         """
         network_message = g_network_message_dict
         network_message_list = [network_message[msg_id] for msg_id in network_message]
         network_message_list.sort(
             key=lambda x: x.get("start_timestamp", None) or x["timestamp"]
         )
         return network_message_list
@@ -618,15 +644,15 @@
         network_message = g_network_message_dict
         g_network_message_dict = {}
         network_message_list = [network_message[msg_id] for msg_id in network_message]
         network_message_list.sort(
             key=lambda x: x.get("start_timestamp", None) or x["timestamp"]
         )
         with open(request_filename, "w", encoding="UTF-8") as f:
-            # msg => {timestamp, start_timestamp, request: dict or None, end_timestamp, response: dict or None}
+            # msg => {timestamp, start_timestamp, request: Union[dict, None], end_timestamp, response: Union[dict, None]}
             for msg in network_message_list:
                 # logger.debug("\nrequest: {}\nresponse: {}".format(msg.get("request", "Error: Request None"),
                 # msg.get("response", "Error: Response Empty")))
                 if not msg.get("start_timestamp"):
                     msg["start_timestamp"] = msg["timestamp"]
                     msg["request"] = None
                 if not msg.get("end_timestamp"):
@@ -661,14 +687,20 @@
         if (
             isinstance(error, MiniElementNotFoundError)
             and not self.test_config.teardown_snapshot
         ):
             # 找不到元素, 把wxml拿回来帮助用户排查. 如果配置了`teardown_snapshot`, 则已经获取过不需要再获取
             self.results["page_wxml"] = self.page_wxml
             return
+        last_launch_time = self.mini and self.mini.last_launch_time
+        if last_launch_time and last_launch_time != self._app_launch_time:
+            # 过程中可能存在 app 重启的情况, 框架原因，重试一次
+            if self.__will_retry is None:
+                self.__will_retry = FRAMEWORK_RETRY
+            return
         
     def _callTestMethod(self, method):
         try:
             self.logger.info("call test method")
             method()
         except SkipTest:
             raise
@@ -690,14 +722,15 @@
         self._teardown_snapshot()
         super(MiniTest, self)._miniTearDown()
 
     def _cleanup_before_retry(self):
         # 清理一下输出路径(等于删除上一个结果)
         if self.test_config.case_output and os.path.isdir(self.test_config.case_output):
             shutil.rmtree(self.test_config.case_output)
+        # self._app_launch_time = self.mini.last_launch_time
 
     def run(self, result=None):
         ret = super().run(result)
         if self.__will_retry is None:
             return ret
         while self.__will_retry > 0 and not self.results["success"]:
             self.__will_retry -= 1
@@ -728,16 +761,22 @@
         if self.mini.sdk_version > "2.19.5":
             wxml = self.page.get_element("/*").outer_wxml
         else:
             wxml = self.page.get_element("page").inner_wxml
         if wxml:
             filename = datetime.datetime.now().strftime("%d%H%M%S.wxml")
             filepath = self.wrap_filename(filename)
-            with open(filepath, "w", encoding="utf8") as fd:
-                fd.write(wxml)
+            try:
+                # pretty
+                dom = xml.dom.minidom.parseString(wxml)
+                wxml = dom.toprettyxml(indent="  ")
+            except:
+                pass
+            with open(filepath, "wb") as fd:
+                fd.write(wxml.encode("utf8", "replace"))
             return filename
         return wxml
 
     @catch
     @retry(2)
     def _framework_capture(self, name=""):
         """框架截图, 尝试两次, 不报错
@@ -755,15 +794,15 @@
 
         :param Exception error: 具体报错, 截图文件名由报错类名定义
         """
         if not self.test_config.error_capture:
             return ""
         return self.capture(error.__class__.__name__)
 
-    def capture(self, name="", region: App.CurrentPage or Page or BaseElement=None):
+    def capture(self, name="", region: Union[App.CurrentPage, Page, BaseElement]=None):
         """
         :param name: 图片名称
         ::param region: 截图区域, 默认为当前页面
         :return: str: image_path or ""
         """
         if name:
             filename = "%s.png" % name
@@ -784,29 +823,29 @@
                 self.mini.app._current_page.path
                 if self.mini and self.mini.app._current_page
                 else ""
             )
             if region:
                 if isinstance(region, (Page, App.CurrentPage)):  # 把状态栏干掉
                     self.add_screen(name, path, page_path, "page")
-                    # self.app.pixel_ratio  # 访问一下获取状态栏的高度
+                    # self.mini.app.pixel_ratio  # 访问一下获取状态栏的高度
                     crop_img(path, [0, getattr(self.native, "status_bar_height", 0), None, None])
                     return path
                 elif isinstance(region, BaseElement):
                     self.add_screen(name, path, page_path, "element")
                     offset_y = 0
-                    if self.app.current_page.page_id == region.page_id:  # 还在当前页面
-                        navigation_style = self.app.current_page.navigation_style
+                    if self.mini.app.current_page.page_id == region.page_id:  # 还在当前页面
+                        navigation_style = self.mini.app.current_page.navigation_style
                         if navigation_style != "custom" and hasattr(
                             self.native, "webview_offset_y"
                         ):
                             # 非自定义页面是, 拿一下webview_offset_y
                             offset_y = self.native.webview_offset_y
                     rect = region.rect
-                    real_rect = list(int(p * self.app.pixel_ratio) for p in [rect["left"], rect["top"], rect["width"], rect["height"]])
+                    real_rect = list(int(p * self.mini.app.pixel_ratio) for p in [rect["left"], rect["top"], rect["width"], rect["height"]])
                     real_rect[1] += offset_y  # 增加导航栏偏移
                     crop_img(path, real_rect)
                     return path
             self.add_screen(name, path, page_path)
             return path
         else:
             logger.warning("%s not exists", path)
@@ -829,15 +868,15 @@
 
     def stop_audits(self, format=None):
         """
         获取体验评分
         :return: 体验评分报告
         """
         format = ["html", "json"] if format is None else format
-        ret = self.app._stop_audits()
+        ret = self.mini.app._stop_audits()
         if len(format) == 0:
             raise Exception("未定义format")
         if not "result" in ret:
             raise Exception("stop_audits获取数据为空")
         if not "report" in ret["result"]:
             raise Exception("stop_audits获取html数据为空")
         if not "data" in ret["result"]:
```

### Comparing `minium-1.5.3/minium/framework/modifier.py` & `minium-1.5.4/minium/framework/modifier.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/report.py` & `minium-1.5.4/minium/framework/report.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,14 +201,15 @@
                         screen_info.append(
                             {
                                 "name": os.path.splitext(image_name)[0],
                                 "url": "",
                                 "path": "images/%s" % image_name,
                                 "ts": ts,
                                 "datetime": datetime,
+                                "use_region": False
                             }
                         )
                         screen_info.sort(key=lambda x: x["ts"])
                         case_info["screen_info"] = screen_info
     return unfinished_case_datas
```

### Comparing `minium-1.5.3/minium/framework/session.py` & `minium-1.5.4/minium/framework/session.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/tools/report_issue.py` & `minium-1.5.4/minium/framework/tools/report_issue.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/framework/wording.py` & `minium-1.5.4/minium/framework/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/__init__.py` & `minium-1.5.4/minium/miniprogram/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,11 +18,11 @@
 
 APP = {"wx": WXMinium, "qq": QQMinium}
 
 Minium = typing.Union[WXMinium, QQMinium]
 def get_minium_driver(conf, *args, **kwargs) -> Minium:
     if conf is None:
         conf = {}
-    application = conf.get("app", APP_WX)
+    application = conf.get("app", APP_WX) if isinstance(conf, dict) else APP_WX
     if application not in APP.keys():
         raise RuntimeError("the 'app' in your config file is not in predefine, not support yet")
     return APP[application](conf, *args, **kwargs)
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/app.py` & `minium-1.5.4/minium/miniprogram/base_driver/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,37 +7,38 @@
 @Date: 2019-03-11 14:41:43
 @LastEditTime: 2019-06-05 16:30:44
 """
 from __future__ import annotations
 import typing
 import types
 from enum import Enum
-from typing import Any
+from typing import Any, Union, Literal, Optional
 import functools
 import re
 
 from .page import AsyncPage, Page, PageType, create, create_async, load_page, create_base_page
 from .minium_object import MiniumObject, RetryableApi
 from ...framework.exception import *
 from ...utils.injectjs import JsMode
 from ...utils.platforms import *
 from ...utils.emitter import ee
 from ...utils.eventloop import event_loop
-from ...utils.utils import get_result, WaitTimeoutError, retry, catch, urlencode, AsyncCondition
+from ...utils.utils import get_result, WaitTimeoutError, retry, catch, urlencode, AsyncCondition, unquote
 from .callback import AsyncCallback, Callback
 from .connection import Command
 import os
 import json
 import threading
 import base64
 import io
 import time
 import datetime
 import copy
 from collections import OrderedDict
+from dataclasses import dataclass
 
 if typing.TYPE_CHECKING:
     from ...native import NativeType
 
 cur_path = os.path.dirname(os.path.realpath(__file__))  # source_path是存放资源文件的路径
 conf_path = os.path.join(os.path.dirname(cur_path), "conf/iOS_conf")
 
@@ -162,14 +163,46 @@
             raise wt
         except MiniClientOfflineError as co:
             raise MiniTimeoutCauseByClientOffline(str(co)) from co
         except MiniConnectionClosedError as cc:
             raise MiniTimeoutCauseByConnectionBreakError(str(cc)) from cc
 
 
+def parse_query(query_str: str) -> dict:
+    """解析query字符串, 需要解析urlencoded格式"""
+    ret = {}
+    for item in query_str.split("&"):
+        k, v = item.split("=")
+        ret[k] = unquote(v)
+    return ret
+
+def split_route_url(url: str) -> typing.Tuple[str, dict]:
+    """拆分 url, 返回 (path, query)"""
+    try:
+        m = re.match("([^\?]+)(.*)$", url)
+        assert m and len(m.groups()) == 2
+        return m.group(1).strip(), parse_query(m.group(2)[1:] or "")
+    except:
+        return url.split("?")[0].strip(), {}
+@dataclass
+class Route:
+    open_type: str
+    op_time: float
+    op_from: Literal["minium", "weapp"]  # minium: 来自指令, weapp: 来自小程序上报
+    path: str = ""
+    query: dict = None
+    delta: int = 1
+
+@dataclass
+class RouteDone:
+    webview_id: str
+    timestamp: float
+    path: str
+    query: dict = None
+
 class App(MiniumObject, metaclass=RetryableApi):
     __RETRY_API__ = [
         "enable_log",
         "screen_shot",
         "expose_function",
         "get_all_pages_path",
         "get_current_page",
@@ -196,45 +229,97 @@
         "_mock_wx_method",  # 各类mock方法都使用到
         "_page_stack",
         # private
         "__get_pages_config",
     ]
 
     class CurrentPage(object):
-        """代理current_page
         """
+        代理current_page
+        """
+        app: App = None
         def __init__(self, app: App) -> None:
             self.app = app
 
         def __del__(self):
             self.app = None
 
         @property
         def _current_page(self):
             return self.app._current_page or self.app.get_current_page()
 
-        def _catch_page_destroyed_error(self, func):
+        def _catch_page_destroyed_error(self, func: Union[typing.Callable, property]):
             @functools.wraps(func)
             def wrapper(*args, **kwargs):
                 try:
+                    is_property = isinstance(func, property)
+                    if is_property:
+                        # property, 先bind, 再通过是否有 set value 来决定 bind fget/fset
+                        if len(args) > 0: # fset
+                            return types.MethodType(func.fset, self.app._current_page)(*args)
+                        return types.MethodType(func.fget, self.app._current_page)()
                     return func(*args, **kwargs)
                 except PageDestroyed:
-                    destroyed_page: PageType = getattr(func, "__self__")
-                    if destroyed_page and destroyed_page == self.app._current_page:  # 如果这里的page没有发生变化, 先刷新一次
-                        self.app.get_current_page()
-                    attr = getattr(self.app._current_page, func.__name__)
+                    self.app.get_current_page()  # 先刷新一次
+                    # 重新获取 attr
+                    if is_property:
+                        if len(args) > 0: # fset
+                            attr = types.MethodType(func.fset, self.app._current_page)
+                        else:
+                            attr = types.MethodType(func.fget, self.app._current_page)
+                    else:
+                        attr = getattr(self.app._current_page, func.__name__)
                     return attr(*args, **kwargs)
             return wrapper
+        
+        def __page_update(self):
+            """判断当前页面是否发生变化
+
+            :return bool or PageType: False: 无变化, 其他: 有变化
+            """
+            if self.app.route_return_page:  # 可能存在加载中页面
+                if self.app.route_return_page.page:  # 已经加载好的
+                    return False
+                if self.app.route_return_page._page == self.app._current_page:  # 当前页面就是等待加载的页面
+                    return self.app.route_return_page.wait_page_done()
+            return False
+        
+        def __get_page_attr(self, __name: str):
+            # 获取属性
+            _current_page = super().__getattribute__("_current_page")
+            prop = _current_page.__class__.__dict__.get(__name)
+            if isinstance(prop, property):
+                return True, prop
+            return False, getattr(_current_page, __name)
 
         def __getattr__(self, __name: str) -> Any:
-            attr = getattr(self._current_page, __name)
-            if callable(attr):  # 可能是api接口
-                return self._catch_page_destroyed_error(attr)
+            is_property, attr = self.__get_page_attr(__name)
+            if callable(attr) or is_property:  # 可能是api接口
+                if self.__page_update():
+                    is_property, attr = self.__get_page_attr(__name)
+                    if not callable(attr) and is_property:
+                        return attr
+                wrapped = self._catch_page_destroyed_error(attr)
+                return wrapped() if is_property else wrapped
             return attr
         
+        def __setattr__(self, __name: str, __value: Any) -> types.NoneType:
+            if __name in self.__dict__ or __name in self.__class__.__dict__:  # 自有属性
+                return super().__setattr__(__name, __value)
+            _current_page = super().__getattribute__("_current_page")
+            prop = _current_page.__class__.__dict__.get(__name)
+            if isinstance(prop, property):
+                # property属性
+                fset = prop.fset
+                if not fset:
+                    raise AttributeError(f"'{self._current_page.__class__.__name__}' object can't set attribute '{__name}'")
+                self.__page_update()
+                return self._catch_page_destroyed_error(prop)(__value)
+            return setattr(_current_page, __name, __value)
+            
         def __eq__(self, page):
             return self._current_page == page
         
         def __ne__(self, page) -> bool:
             return not (self._current_page == page)
         
         def __repr__(self):
@@ -245,18 +330,22 @@
 
     def __init__(self, connection, relaunch=False, native: NativeType=None, platform="ide", enable_h5=True, **kwargs):
         """
         创建一个 APP 实例
         :param connection:
         """
         super().__init__()
+        self.logger = self.logger.getChild(f"App{str(id(self))[-4:]}")
+        self._released = False
+        self._do_when_released = []
         self.connection = connection
         self.native = native
         self.platform = platform
         self.enable_h5 = enable_h5
+        self.extra_info = kwargs
         self.js_mode: JsMode = (
             JsMode.JUST_ES5 if platform in [OS_ANDROID, OS_IOS] else JsMode.ALL
         )  # 真机调试2.0环境下只支持es5语法
         self._msg_lock = threading.Condition()
         self._async_msg_lock = AsyncCondition(loop=event_loop)
         self._is_log_enable = False
         self._pixel_ratio = None
@@ -269,45 +358,52 @@
         self.current_page = App.CurrentPage(self)
         self._mocked_images = None
         self._mocked_images_dir = None
         self._mocked_images_data = {}
         self._screen_shot_timeout = None
         # init methods
         # 以下注入需要严格按照顺序: checkEnv -> helpers -> utils
-        env = self._evaluate_js("checkEnv")
+        env = self.env
         self._is_injected = env.get("injected")  # 是否已经注入过了, 注入过的环境不需要重复注入, 防止出现多次回调等预期之外的情况
         self._is_third_app = env.get("isThirdApp")  # 是否是第三方开发框架构建的小程序, 影响mock & hook功能
         self._route_change_listener()
         if not self._is_injected and self.js_mode is JsMode.JUST_ES5:  # 注入一些垫片
             self._evaluate_js("helpers")
         self._evaluate_js("utils")
         self._evaluate_js("hijackWxMethod")  # 初始化劫持wx方法的各种方法
         self._request_stack_listener()
         # super(App, self)._evaluate_js("hijackWxMethod", code_format_info={"function": "miniumHijackFn"}, mode=JsMode.JUST_ES5)  # 初始化劫持wx方法的各种方法
         # if self._is_third_app:
         #     self._evaluate_js("initMockWxMethod")
         self.pages = []
         self.tabbar_pages = {}
         self.__get_pages_config()
-
+        # hook页面跳转
+        self._navigation_stack = []
+        self._hook_navigation()
         # hook一些原生弹窗:
         # showModal
         # showToast
         self._modals_lock = threading.RLock()
         self._modals = {
             "showModal": OrderedDict(),
             "showToast": OrderedDict()
         }
         self._clean_thread = None
         self._hook_native()
         self._clean_modal_cache()
+        self._do_when_released.append(self._clean_modal_cache)
         
         if relaunch:
             self.relaunch(self.main_page_path.path, self.main_page_path.query)
 
+    @property
+    def env(self):
+        return self._evaluate_js("checkEnv")
+
     def _clean_modal_cache(self):
         """定期清理modal弹窗缓存信息"""
         DELTA = 120  # 2min
         ctime = time.time()
         for api in self._modals:
             modals = self._modals[api]
             ids = []
@@ -315,14 +411,16 @@
                 if info["timeStamp"] + DELTA < ctime:
                     ids.append(callId)
                 else:
                     break
             with self._modals_lock:
                 for callId in ids:
                     modals.pop(callId)
+        if self._released:
+            return
         self._clean_thread = threading.Timer(240, self._clean_modal_cache)  # 4min一次
         self._clean_thread.daemon = True
         self._clean_thread.start()
 
     def _hook_native(self):
         """hook原生弹窗"""
         def callback(api, stage):
@@ -341,15 +439,36 @@
                         self._modals[api][callId].update({
                             stage: ret
                         })
             return nw
         for api in ("showModal", "showToast"):
             before = Callback(callback(api, "before"))
             cb = Callback(callback(api, "callback"))
-            self.hook_wx_method(api, before=before, callback=cb, with_id=True)
+            hook_id = self.hook_wx_method(api, before=before, callback=cb, with_id=True)
+            # self._do_when_released.append(
+            #     functools.partial(self.release_hook_wx_method, api, hook_id)
+            # )
+
+    def _hook_navigation(self):
+        """hook小程序页面跳转"""
+        hook_id = "global"
+        methods = ["navigateTo", "redirectTo", "switchTab", "navigateBack", "reLaunch"]
+        for method in methods:
+            def callback(method_, obj, *args):
+                url = obj.get("url") or ""
+                if obj.get("oriPath") and not url.startswith("/"):  # navigate from
+                    # 兼容系统
+                    ori_path = obj.get("oriPath", "").replace("/", os.sep)
+                    url = url.replace("/", os.sep)
+                    url = os.path.normpath(os.path.join(ori_path, url))
+                self._navigation_stack.append(Route(method_, time.time(), "weapp", *split_route_url(url), obj.get("delta")))
+            callback_obj = Callback(functools.partial(callback, method)).callback
+            self._expose_function(f"{method}_before_{hook_id}", callback_obj)
+            self._do_when_released.append(functools.partial(self._unregister, f"{method}_before_{hook_id}", callback_obj))
+        self._evaluate_js("hookNavigation")
 
     def _get_modal_info(self, since=None, api=None):
         """获取小程序弹窗信息
 
         :param int since: 从此时开始之后出现的弹窗, defaults to None - all
         :return List[dict]: 所有弹窗信息
         """
@@ -384,24 +503,34 @@
         infos = self._get_modal_info(api="showModal")
         return self._format_modal_info(filter(lambda x: "callback" not in x, infos))
 
     def release(self):
         """释放循环引用
         _current_page -> app -> _current_page
         """
+        self.logger.info(f"release app {self}")
         current_page = self._current_page
         if current_page:
             self._current_page = None
             current_page.app = None
         if self.current_page:
             self.current_page.app = None
             self.current_page = None
         if self._clean_thread:
             self._clean_thread.cancel()
             self._clean_thread = None
+        self._unregister("onAppRouteDone", self._on_route_changed)
+        self._released = True
+        _do_when_released = self._do_when_released
+        self._do_when_released = []
+        for f in _do_when_released:
+            try:
+                f()
+            except Exception as e:
+                self.logger.warning(f"call {f.func.__name__ if isinstance(f, functools.partial) else f.__name__} when app released error: {e}")
 
     @property
     def app_id(self):
         if not self._appid:
             self._appid = self._get_account_info_sync().result.result.miniProgram.appId
         return self._appid
 
@@ -888,15 +1017,15 @@
                 is_wait_url_change=is_wait_url_change,
                 wait_route_done_time=5,
             )
         else:
             page = self.relaunch(main_page_path.path, main_page_path.query)
         return page
 
-    def get_async_response(self, msg_id: str, timeout=None) -> None or dict:
+    def get_async_response(self, msg_id: str, timeout=None) -> Optional[dict]:
         """
         description: 获取异步调用的结果
         param {*} self
         param {str} msg_id 消息ID
         param {int} timeout 超时时间
         return {*}
         """
@@ -972,14 +1101,15 @@
             open_type,
             path,
             route_done_lock=self._async_msg_lock if is_wait_url_change else None,
         ) as cmd:
             cmd.listen_route_change(wait_timeout)
 
             cmd.open_id = self.call_wx_method_async(open_type, [{"url": path}])
+            self._navigation_stack.append(Route(open_type, time.time(), "minium", *split_route_url(path), 0))
             # 理论上RouteCommand中通过ee监听了不会再在这里获取到结果, 以防线程切换过程导致时序问题，这里做一个兜底
             response = self.connection.get_aysnc_msg_return(cmd.open_id)
             if response is None:
                 try:
                     cmd.get_open_result(wait_timeout)
                 except MiniTimeoutError:
                     self.logger.warning(f"等待wx.{open_type}回调失败")
@@ -1000,22 +1130,27 @@
         update_time = args[1] if len(args) > 1 else int(time.time() * 1000)
         if (
             self._route_return_page_update_time
             and self._route_return_page_update_time > update_time
         ):
             # 旧信息, 丢弃
             return
+        self._navigation_stack.append(RouteDone(options.webviewId, time.time(), options.path, options.query))
         self.route_return_page = create_async(
             options.webviewId, options.path, options.query, options.get("renderer", None), app=self
         )
         self._notify_msg_lock()
         # 记录当前页面
-        self.route_return_page._callback = lambda page: setattr(self, "_current_page", page)
+        def route_callback(page):
+            self._current_page = page
+
+        self.route_return_page._callback = route_callback
         if self.route_return_page.page is not None:
             self._current_page = self.route_return_page.page
+            self.route_return_page._callback = None
         else:  # 先把_current_page更新成基础页面
             self._current_page = self.route_return_page._page
         self.logger.info("Route changed, %s" % message)
 
     def _route_changed(self, timeout=None):
         if not timeout:
             timeout = 5
@@ -1046,15 +1181,15 @@
         if not timeout:
             timeout = 5
 
         ret = await self._wait_msg_lock(timeout)
         return ret
 
     def _route_change_listener(self):
-        self._unregister("onAppRouteDone")
+        self._unregister("onAppRouteDone", self._on_route_changed)
         self._expose_function("onAppRouteDone", self._on_route_changed)
         self._evaluate(
             """function () {
     if (!global.__minium__.onAppRouteDone) {
         wx.onAppRouteDone(function (options) {
             var c = getCurrentPages().pop()
             if (c && c.__wxWebviewId__ == options.webviewId) options.renderer = c.renderer
@@ -1086,17 +1221,17 @@
     def _stop_audits(self):
         ret = self.connection.send("Tool.stopAudits")
         return ret
 
     def hook_wx_method(
         self,
         method: str,
-        before: Callback or types.FunctionType = None,
-        after: Callback or types.FunctionType = None,
-        callback: Callback or types.FunctionType = None,
+        before: Union[Callback, types.FunctionType] = None,
+        after: Union[Callback, types.FunctionType] = None,
+        callback: Union[Callback, types.FunctionType] = None,
         with_id = False,
     ) -> int:
         """
         hook wx 方法
         :param method: 需要 hook 的方法
         :param before: 在需要 hook 的方法之前调用
         :param after: 在需要 hook 的方法之后调用
@@ -1325,15 +1460,15 @@
         self._evaluate_js("mockWxMethod", [method,], code_format_info={
             "function": "undefined"
         })
 
     def _mock_network(
         self,
         interface: str,
-        rule: str or dict,
+        rule: Union[str, dict],
         success=None,
         fail=None,
         mock_type=MockNetworkType.ALWAYS,
     ):
         if success and fail:
             raise RuntimeError("Can't call back both SUCCESS and FAIL")
         if not (success or fail):
@@ -1407,21 +1542,21 @@
         return self._evaluate_js(
             "cleanCloudCallMockRule",
             [
                 interface,
             ],
         )
 
-    def mock_request(self, rule: str or dict, success=None, fail=None):
+    def mock_request(self, rule: Union[str, dict], success=None, fail=None):
         """
         mock wx.request, 根据正则mock规则返回mock结果
         """
         return self._mock_network("request", rule, success, fail)
 
-    def mock_request_once(self, rule: str or dict, success=None, fail=None):
+    def mock_request_once(self, rule: Union[str, dict], success=None, fail=None):
         """
         mock wx.request, 根据正则mock规则返回mock结果, 一旦匹配上了, 即废除该rule
         """
         return self._mock_network("request", rule, success, fail, MockNetworkType.ONCE)
 
     def restore_request(self):
         return self._restore_network("request")
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/callback.py` & `minium-1.5.4/minium/miniprogram/base_driver/callback.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     def __init__(self, callback: types.FunctionType = None) -> None:
         self.__callback = callback
         self.__called = threading.Semaphore(0)
         self.__is_called = False
         self.__callback_result = None
         self.__callback_results = []  # 累积的结果
 
+    def __call__(self, *args, **kwds):
+        return self.callback(*args, **kwds)
+
     def callback(self, args):
         self.__is_called = True
         self.__callback_result = (
             args[0] if isinstance(args, (tuple, list)) and len(args) == 1 else args
         )
         self.__callback_results.append(self.__callback_result)
         self.__called.release()
@@ -111,14 +114,17 @@
     def cancel(self):
         self._waiter.cancel()
 
     def callback(self, *args):
         if not self._waiter.done():
             self._loop.run_coroutine(self.set_result(args))
 
+    def __call__(self, *args, **kwds):
+        return self.callback(*args, **kwds)
+
     @property
     def is_called(self):
         return self._waiter.done()
 
     def wait_called(self, timeout=10) -> bool:
         """
         等待回调调用, 默认等待最多10s
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/connection.py` & `minium-1.5.4/minium/miniprogram/base_driver/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 Filename:       connection_new.py
 Create time:    2019/6/14 16:29
 Description:
 
 """
 import types
 import typing
-from typing_extensions import Self
+from typing_extensions import Self, Optional, Callable
 import time
 import websocket
 from websocket import WebSocketConnectionClosedException
 import json
-from typing import TypeVar
+from typing import TypeVar, Union
 from .minium_log import MonitorMetaClass
 from ...framework.exception import *
 from uuid import uuid4
 import threading
 import logging
 from asyncio.coroutines import iscoroutine
 from ...utils.utils import ProcessSafeEventLoop, WaitThread, cost_debug
@@ -142,15 +142,15 @@
         cls.max_timeout = timeout
 
 
 class AsyncCommand(BaseCommand):
     """异步命令"""
     def __init__(self, method: str, params: dict = None, desc: str = None) -> None:
         super().__init__(method, params, desc)
-        self.result: DevToolMessage or Exception = None  # 命令返回结果
+        self.result: Union[DevToolMessage, Exception] = None  # 命令返回结果
 
 C = TypeVar('C', Command, AsyncCommand)
 
 def json2obj(data):
     try:
         return json.loads(data, object_hook=DevToolMessage)
     except (TypeError, json.JSONDecodeError):
@@ -264,15 +264,15 @@
         # 清理异步命令存储
         for k in list(self._async_msg_map.keys()):
             self._async_msg_map.pop(k)
         self._is_close_on_my_own = True
         self._is_close_by_cmd = True
         self._is_close_app_by_cmd = True
 
-    def register(self, method: str, callback):
+    def register(self, method: str, callback: Union[Callable, Callback]):
         if method not in self.observers:
             self.observers[method] = []
         self.observers[method].append(callback)
 
     def remove(self, method: str, callback=None):
         if method in self.observers.keys():
             if callback is None:  # remove all callback
@@ -313,14 +313,15 @@
             for callback in self.observers[method]:
                 if callable(callback):
                     # callback(message)
                     self.create_async_callback_task(callback, message)
                 else:
                     raise MiniNoncallableError(f"{str(callback)}(message={message})")
         else:
+            self.logger.warning(f'no observer listening event {message["name"] if method == "App.bindingCalled" else method}')
             return
 
     def _connect(self, timeout=MAX_WAIT_TIMEOUT):
         error_callback = Callback()
         close_callback = Callback()
         ee.once("ws_close", close_callback.callback)
         ee.once("ws_error", error_callback.callback)
@@ -413,15 +414,15 @@
         :raise MiniConnectionClosedError:
         """
         message = cmd.dumps()
         self.logger.debug(f'{"SEND" if sync else "ASYNC_SEND"} > [{self._id}]{message}')
         if not self._send(message) and not self._is_connected:
             raise MiniConnectionClosedError("send message[%s] fail because connection is not established" % cmd.id)
 
-    def _gen_command(self, method: str or C, params=None, max_timeout=None, sync=True) -> C:
+    def _gen_command(self, method: Union[str, C], params=None, max_timeout=None, sync=True) -> C:
         if sync:
             if isinstance(method, Command):
                 cmd = method
             elif isinstance(method, AsyncCommand):
                 cmd = Command(method.method, method.params, desc=method.desc)
             else:
                 cmd = Command(method, params, max_timeout)
@@ -433,23 +434,23 @@
                 del method  # 删除监听函数
             else:
                 cmd = AsyncCommand(method, params)
         if not cmd.id:
             cmd.id = str(uuid4())
         return cmd
 
-    def send(self, method: str or Command, params=None, max_timeout=None):
+    def send(self, method: Union[str, Command], params=None, max_timeout=None):
         # 同步发送消息，函数会阻塞
         cmd: Command = self._gen_command(method, params, max_timeout)
         with cmd:
             self._sync_wait_map[cmd.id] = None  # 该ID未有返回message
             self._safely_send(cmd)
             return self._receive_response(cmd)
 
-    def send_async(self, method: str or AsyncCommand, params=None, ignore_response=False) -> str:
+    def send_async(self, method: Union[str, AsyncCommand], params=None, ignore_response=False) -> str:
         cmd: AsyncCommand = self._gen_command(method, params, sync=False)
         if not ignore_response:
             self._async_msg_map[cmd.id] = cmd
         try:
             self._safely_send(cmd, sync=False)
         except MiniConnectError:
             if not ignore_response:
@@ -597,15 +598,15 @@
         finally:
             self._is_reconnecting.release()
             self.after_reconnect()
         self.logger.warning("connection reconnect fail")
         self._last_reconnect_fail_time = time.time()
         return False
 
-    def wait_reconnect(self, timeout=None) -> None or Exception:
+    def wait_reconnect(self, timeout=None) -> Optional[Exception]:
         wait_time = MAX_RETRY * MAX_WAIT_TIMEOUT + 10 if timeout is None else timeout
         if not self._is_reconnecting.acquire(timeout=wait_time):
             return TimeoutError(f"connection did not reconnect within {wait_time} seconds")
         self._is_reconnecting.release()
         if not self._is_connected:
             return self._last_reconnect_fail_reason or MiniReConnectSvrError("reconnect fail")
 
@@ -720,22 +721,22 @@
         self._set_all_async_command_fail(MiniConnectionClosedError("connection destroy"))
         if self._thread:
             self._thread.join(CLOSE_TIMEOUT)
         if self._event_loop.is_running():
             self._event_loop.stop_loop()
         self.__class__.delete(self.id)
 
-    def wait_for(self, method: str or Command, max_timeout=None):
+    def wait_for(self, method: Union[str, Command], max_timeout=None):
         if isinstance(method, Command):
             cmd = method
         else:
             cmd = Command(method, max_timeout=max_timeout)
         if cmd.method in self._method_wait_map and self._method_wait_map.get(
             cmd.method, None
-        ):  # 已经有间听到并没被删除（一般只有别的线程同样在等这个方法，但又还没响应才会命中，兜底逻辑）
+        ):  # 已经有监听到并没被删除（一般只有别的线程同样在等这个方法，但又还没响应才会命中，兜底逻辑）
             return True
         self._method_wait_map[cmd.method] = None
         while cmd.max_timeout > 0:
             self._wait(cmd)
             if cmd.method in self._method_wait_map and self._method_wait_map.get(
                 cmd.method, None
             ):
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/element.py` & `minium-1.5.4/minium/miniprogram/base_driver/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,21 +5,26 @@
 @LastEditors: lockerzhang
 @Description: 元素相关的操作和信息获取
 @Date: 2019-03-11 14:42:10
 @LastEditTime: 2019-06-06 15:13:32
 """
 from __future__ import annotations
 import typing
-from minium.framework.exception import MiniElementNotFoundError, MiniTimeoutCauseByConnectionBreakError
+from typing import Union
+from ...framework.exception import MiniElementNotFoundError, MiniTimeoutCauseByConnectionBreakError
 from .minium_object import MiniumObject, RetryableApi
 from ...utils.utils import timeout
 from ...utils.emitter import ee
 import time
 from .prefixer import *
 from .connection import Command
+from .selector import Selector
+from ...framework.exception import MiniCommandError
+if typing.TYPE_CHECKING:
+    from .page import Page
 
 
 class Element:
     tagName: str
     elementId: str
     nodeId: typing.Optional[str]
 
@@ -37,14 +42,16 @@
         return self[name]
 
     def __getitem__(self, name):
         name = Rect.key_map.get(name, name)
         return super(Rect, self).__getitem__(name)
 
 
+DEFAULT_ENV = {}
+
 class BaseElement(MiniumObject, metaclass=RetryableApi):
     """
     元素基类
     """
     __RETRY_EXCEPTION__ = (MiniTimeoutCauseByConnectionBreakError,)  # 小程序掉线Element实例可能就没用了
     __RETRY_API__ = [
         "data",
@@ -64,19 +71,21 @@
         # private
         "_property",  # 属性相关
         "_dom_property",  # dom属性相关
         "_get_window_properties",  # window属性相关
         "__get_elements",  # get element相关都经过该接口
     ]
 
-    def __init__(self, element: Element, page_id: str, connection):
+    def __init__(self, element: Element, page_id: str, connection, selector: Selector=None, env: dict=DEFAULT_ENV):
         """
         初始化
         """
         super().__init__()
+        self.selector = selector
+        self.env = env
         self.parent_node_id = None  # 自定义组件中的自元素需要记录一下其父元素的node id
         self.element_id = element.elementId
         self.page_id = page_id
         self._tag_name = element.tagName
         self.connection = connection
 
     def __str__(self) -> str:
@@ -382,46 +391,54 @@
         ::after	             view::after	            在 view 组件后边插入内容
         ::before	         view::before	            在 view 组件前边插入内容
 
         :param selector: 选择器
         :param max_timeout: 超时时间
         :return:element 对象 list
         """
-        if inner_text is None and value is None and text_contains is None:
-            need_filter = False
+        if isinstance(selector, Selector):
+            _selector = selector
         else:
-            need_filter = True
-        if not need_filter:
-            return self._get_elements_by_css(selector, max_timeout, index=index)
+            _selector = Selector(css=selector, text=inner_text, contains_text=text_contains, val=value, index=index)
+        if not _selector.need_filter:
+            return self._get_elements_by_css(_selector, max_timeout)
 
         @timeout(max_timeout)
         def filter_elements():
             # 需要过滤内容，有返回元素不是终结条件, 需要获取所有元素后再作过滤
-            elements = self._get_elements_by_css(selector, max_timeout, index=-1)
+            new_selector = Selector(_selector)
+            new_selector.index = -1
+            elements = self._get_elements_by_css(new_selector, max_timeout)
             els = []
             for element in elements:
-                if inner_text and element.inner_text != inner_text:
+                if _selector.text and element.inner_text != _selector.text:
                     continue
-                if value and element.value() != value:
+                if _selector.val and element.value() != _selector.val:
                     continue
-                if text_contains and text_contains not in element.inner_text:
+                if _selector.contains_text and _selector.contains_text not in element.inner_text:
                     continue
+                # element.selector.text = inner_text
+                # element.selector.contains_text = text_contains
+                # element.selector.val = value
                 els.append(element)
-                if len(els) == (index + 1):
+                if len(els) == (_selector.index + 1):
                     return els
             return els
 
         return filter_elements()
 
-    def __get_elements(self, selector: str, index=-1):
+    def __get_elements(self, selector: typing.Union[str, Selector], index=-1):
+        if not isinstance(selector, Selector):
+            selector = Selector(css=selector, index=index)
         elements = []
-        ret = self._send("Element.getElements", {"selector": selector})
+        ret = self._send("Element.getElements", {"selector": selector.css})
+        selector.parent = self.selector
         for el in ret.result.elements:
-            elements.append(create(el, self.page_id, self.connection))
-            if len(elements) == (index + 1):  # index==-1时，不会match，就会全部返回
+            elements.append(create(el, self.page_id, self.connection, selector))
+            if len(elements) == (selector.index + 1):  # index==-1时，不会match，就会全部返回
                 return elements
         return elements
 
     def __search_child(
         self, selector_list: list, parent: ElementType = None, index=-1  # type: ignore # noqa: F811
     ) -> typing.List[ElementType]:
         # index == -1: get所有, index >=0: get index+1个
@@ -460,33 +477,36 @@
                 selector_list[0:], _el
             )  # selector_list[0:]相当于copy
             child_els += child_el
             if len(child_els) == (index + 1):
                 return child_els
         return child_els
 
-    def _get_elements_by_css(self, selector: str, max_timeout=0, index=-1) -> typing.List[ElementType]:
+    def _get_elements_by_css(self, selector: typing.Union[str, Selector], max_timeout=0, index=-1) -> typing.List[ElementType]:
         """
         1. 现存自定义组件中的class会自动加前缀，但不包括slot占位的元素
         2. slot元素的class命名规则
         2.1 <page><test><view class="这个class不会加前缀"></view></test></page>
         2.2 <custom><test><view class="这个class会加上custom组件对应的前缀"></view></test></custom>
         3. 自定义组件中通过id获取元素失败
         """
-
+        if isinstance(selector, Selector):
+            _selector = selector
+        else:
+            _selector = Selector(css=selector, index=index)
         @timeout(max_timeout)
-        def search_elements(_selector: list or tuple):
-            return self.__search_child(_selector[0:], index=index)
+        def search_elements(_selectors: Union[list, tuple]):
+            return self.__search_child(_selectors[0:], index=_selector.index)
 
         self.logger.info("try to get elements: %s" % selector)
-        _selector_list = selector.split(">>>")
+        _selector_list = _selector.css.split(">>>")
         _selector_list.reverse()  # 新增处理【>>>】穿透自定义组件逻辑
         els = search_elements(_selector_list)
         if len(els) == 0:
-            self.logger.warning(f"Could not found any element '{selector}' you need")
+            self.logger.warning(f"Could not found any element '{_selector.css}' you need")
         else:
             self.logger.info("find elements success: %s" % str(els))
         return els
 
     def attribute(self, name):
         """
         获取元素属性
@@ -783,19 +803,40 @@
         :return:
         """
         if self._tag_name != "input" and self._tag_name != "textarea":
             self.logger.warning(
                 "Element's type is not fit for the method which you call"
             )
             return
+        # 3.3.4重构了 input, 导致 textarea.input 失败
+        if self._tag_name == "textarea" and self.env.get("sdk_version") and self.env.get("sdk_version") > "3.3.3":
+            self.logger.warning(
+                f'sdk version {self.env.get("sdk_version")} may not support textarea.input, please use lower sdk version'
+            )
+            return
         func = "{x}.input".format(x=self._tag_name)
         value = text.strip()
-        self.call_func(func, args=[value])
-        if text.endswith("\n") or with_confirm:  # 换行符结尾认为是confirm
+        if text.endswith("\n"):  # 换行符结尾认为是confirm
+            with_confirm = True
+        less_then_3_3_0 = self.env.get("sdk_version") and self.env.get("sdk_version") < "3.3.0"
+        try:
+            # v3.3.0 后直接支持with_confirm
+            self.call_func(func, args=[value, with_confirm])
+        except MiniCommandError as ce:
+            if str(ce) == "e.stopPropagation is not a function":  # 基础库(v3.3.4)引入的报错, ide 环境下兼容一下
+                if with_confirm:
+                    self.trigger("confirm", {"value": value})
+                self.trigger("blur", {"value": value, "cursor": len(value)})
+                return
+            raise
+        if with_confirm and less_then_3_3_0:
+            # 需要显式触发一个
             self.trigger("confirm", {"value": value})
+        if less_then_3_3_0:
+            self.trigger("blur", {"value": value, "cursor": len(value)})
         # self.trigger("input", {"value": text})
 
     #####################
     #       picker      #
     #####################
     def pick(self, value):
         """
@@ -1521,15 +1562,15 @@
         "stopBGM",
         "stopPreview",
         "switchCamera",
         "toggleTorch",
     )
 
 
-ELEMENT_TYPE = {
+ELEMENT_TYPE: typing.Dict[str, 'ElementType'] = {
     "video": VideoElement,
     "audio": AudioElement,
     "live-player": LivePlayerElement,
     "live-pusher": LivePusherElement,
     "scroll-view": ViewElement,
     "swiper": ViewElement,
     "movable-view": ViewElement,
@@ -1549,14 +1590,26 @@
     ViewElement,
     FormElement,
     LivePlayerElement,
     LivePusherElement,
 ]
 
 
-def create(element: Element, page_id: str, connection) -> ElementType:
+def create(element: Element, page_id: str, connection, selector, page: Page=None) -> ElementType:
+    if page and page.app:
+        env = {
+            "sdk_version": page.app.extra_info.get("sdk_version")
+        }
+    else:
+        env = {}
     if "nodeId" in element.keys():
-        return CustomElement(element, page_id, connection)
+        el = CustomElement(element, page_id, connection)
+        el.selector = Selector(selector)
+        el.env = env
+        el.selector.node_id = el.node_id
     else:
-        return ELEMENT_TYPE.get(element.tagName, BaseElement)(
+        el = ELEMENT_TYPE.get(element.tagName, BaseElement)(
             element, page_id, connection
         )
+        el.selector = selector
+        el.env = env
+    return el
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/h5_element.py` & `minium-1.5.4/minium/miniprogram/base_driver/h5_element.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*-coding: utf-8 -*-
 '''
 Author: gavinggu gavinggu@tencent.com
 Date: 2023-09-04 14:23:50
-LastEditors: gavinggu gavinggu@tencent.com
-LastEditTime: 2023-09-04 15:42:02
+LastEditors: yopofeng yopofeng@tencent.com
+LastEditTime: 2024-04-17 20:04:49
 FilePath: /py-minium/minium/miniprogram/base_driver/h5_element.py
 Description: h5页面元素测试动作
 '''
 
 import time
 import logging
 import json
-from minium.miniprogram.h5tools.exceptions import *
+from ..h5tools.exceptions import *
 
 
 logger = logging.getLogger("minium")
 
 
 class H5Element:
     def __init__(self, client, node_id):
@@ -509,8 +509,64 @@
         更改元素的attribute取值
         :param attribute_name: attribute名称
         :param attribute_value: attribute内容
         """
         self.client.send_command("DOM.setAttributesAsText", {
             "nodeId": self.node_id,
             "text": f'{attribute_name}="{attribute_value}"'
-        })
+        })
+
+    @property
+    def top(self):
+        """
+        获取元素顶部相对于视图窗口顶部的top值
+        """
+        object_id = self.client.send_command('DOM.resolveNode', {'nodeId': self.node_id})['result']['object'][
+            'objectId']
+        top = self.client.send_command('Runtime.callFunctionOn', {
+            'objectId': object_id,
+            'functionDeclaration': 'function() { return this.getBoundingClientRect().top; }',
+            'returnByValue': True,
+        })['result']['result']['value']
+        return top
+
+    @property
+    def left(self):
+        """
+        获取元素左侧相对于视图窗口左侧的left值
+        """
+        object_id = self.client.send_command('DOM.resolveNode', {'nodeId': self.node_id})['result']['object'][
+            'objectId']
+        left = self.client.send_command('Runtime.callFunctionOn', {
+            'objectId': object_id,
+            'functionDeclaration': 'function() { return this.getBoundingClientRect().left; }',
+            'returnByValue': True,
+        })['result']['result']['value']
+        return left
+
+    @property
+    def bottom(self):
+        """
+        获取元素底部相对于视图窗口顶部的bottom值
+        """
+        object_id = self.client.send_command('DOM.resolveNode', {'nodeId': self.node_id})['result']['object'][
+            'objectId']
+        bottom = self.client.send_command('Runtime.callFunctionOn', {
+            'objectId': object_id,
+            'functionDeclaration': 'function() { return this.getBoundingClientRect().bottom; }',
+            'returnByValue': True,
+        })['result']['result']['value']
+        return bottom
+
+    @property
+    def right(self):
+        """
+        获取元素右侧相对于视图窗口左侧的right值
+        """
+        object_id = self.client.send_command('DOM.resolveNode', {'nodeId': self.node_id})['result']['object'][
+            'objectId']
+        right = self.client.send_command('Runtime.callFunctionOn', {
+            'objectId': object_id,
+            'functionDeclaration': 'function() { return this.getBoundingClientRect().right; }',
+            'returnByValue': True,
+        })['result']['result']['value']
+        return right
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/minium.py` & `minium-1.5.4/minium/miniprogram/base_driver/minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/minium_log.py` & `minium-1.5.4/minium/miniprogram/base_driver/minium_log.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 Filename:       minium_log.py
 Create time:    2019-08-29 11:12
 Description:
 
 """
 
 from functools import wraps
+import sys
 import datetime
 import types
+from typing import Union
 import json
 import requests
 import queue
 import threading
 import logging
 import os
 import time
@@ -27,52 +29,88 @@
 
 REPORT_DOMAIN = "minitest.weixin.qq.com"
 REPORT_PATH = "xbeacon/user_report"
 app_id = None
 version = build_version().get("version")
 revision = build_version().get("revision")
 __DEV = os.environ.get("MINIUM_DEV", None)
+
+
+class ILogsCmd:
+    minium_new = "api_log"
+    minium_exception = "cloud_exception_log"
+
+
 class ReportData(dict):
+    # required fields
     cmd = ""
+    app_id = app_id
+    version = ""
+    revision = ""
+
+    def __init__(self):
+        self.version = version
+        self.revision = revision
+        self.app_id = app_id
+        super().__init__(self.__dict__)
 
     def __eq__(self, __value: object) -> bool:
         if isinstance(__value, ReportData):
             return self.dumps() == __value.dumps()
         return super().__eq__(__value)
 
     def dumps(self):
         return json.dumps(self)
 
+
 class ExceptionData(ReportData):
+    # 错误上报
     def __init__(self, err: Exception, **kwargs):
         kwargs["from"] = "minium"
-        self.TimeStamp = getattr(err, "timestamp", None) or time.strftime("%Y-%m-%d %H:%M:%S", time.localtime())
+        self.TimeStamp = getattr(err, "timestamp", None) or time.strftime(
+            "%Y-%m-%d %H:%M:%S", time.localtime()
+        )
         self.error = err.__class__.__name__
         self.err_msg = getattr(err, "msg", None) or str(err)
         self.Uin = 0
-        self.version = version
-        self.revision = revision
         self.ext = ""
-        self.app_id = app_id
         self.msg_id = getattr(err, "msg_id", "")
         self.__dict__.update(kwargs)
-        super().__init__(self.__dict__)
-        self.cmd = "cloud_exception_log"
+        super().__init__()
+        self.cmd = ILogsCmd.minium_exception
 
 
 class ConsumeData(ReportData):
-    def __init__(self, __map: dict, **kwargs):
-        self.version = version
-        self.revision = revision
-        self.app_id = app_id
+    # 耗时上报
+    def __init__(self, func_name, consuming, args=[], kwargs={}, **_kwargs):
         self.time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        __map.update(kwargs)
-        self.__dict__.update(__map)
-        super().__init__(self.__dict__)
-        self.cmd = "api_log"
+        self.func = func_name
+        self.consuming = consuming
+        self.args = args
+        self.kwargs = kwargs
+        self.__dict__.update(_kwargs)
+        super().__init__()
+        self.cmd = ILogsCmd.minium_new
+
+
+class UsageData(ReportData):
+    REPORTED = set()
+
+    def __new__(cls, feature):
+        if feature in UsageData.REPORTED:
+            return None
+        UsageData.REPORTED.add(feature)
+        return super().__new__(cls)
+
+    # 功能使用上报
+    def __init__(self, feature, **kwargs):
+        self.usage = feature
+        super().__init__()
+        self.cmd = ILogsCmd.minium_new
+
 
 def process_report():
     global existFlag
     while not existFlag:
         lock.acquire()
         lock.wait(10)
         lock.release()
@@ -88,15 +126,29 @@
         fail += 1
         if fail >= 10:
             existFlag = 1
     else:
         fail = 0
 
 
-def report_exception(data: ExceptionData):
+def report_exception(data: Union[ExceptionData, types.FunctionType, types.MethodType]):
+    def _report_exception(func):
+        @wraps(func)
+        def wrapper(*args, **kwargs):
+            try:
+                return func(*args, **kwargs)
+            except:
+                e = sys.exc_info()[1]
+                report_exception(ExceptionData(err=e, func=func.__name__))
+                raise
+
+        return wrapper
+
+    if isinstance(data, (types.FunctionType, types.MethodType)):
+        return _report_exception(data)
     if not data.app_id:
         return
     report_queue.put(data)
     lock.acquire()
     lock.notify()
     lock.release()
 
@@ -150,14 +202,15 @@
 thread.setDaemon(True)
 thread.start()
 
 usage = []
 
 REPORT_THRESHOLD = 10000  # 上报阈值
 
+
 def minium_log(func):
     """
     函数统计装饰器
     :param func:
     :return:
     """
 
@@ -176,21 +229,18 @@
         end = datetime.datetime.now()
         consuming = int((end - start).total_seconds() * 1000)
         if app_id is None and hasattr(self, "app_id"):
             app_id = self.app_id
         if consuming < REPORT_THRESHOLD:
             return result
         new_args = list(args[1:])
-        
-        consum_data = ConsumeData({
-            "func": func_name,
-            "args": str(new_args),
-            "kwargs": kwargs,
-            "consuming": consuming
-        })
+
+        consum_data = ConsumeData(
+            func_name=func_name, args=str(new_args), kwargs=kwargs, consuming=consuming
+        )
 
         if app_id is None:
             usage.append(consum_data)
         else:
             report_queue.put(consum_data)
             for f in usage:
                 f["app_id"] = app_id
@@ -218,7 +268,12 @@
                 and not k.startswith("register")
                 and not k.startswith("notify")
                 and not k.startswith("remove")
             ):
                 attr_dict[k] = minium_log(v)
         return type.__new__(mcs, cls_name, bases, attr_dict)
 
+
+def report_usage(feature):
+    usage = UsageData(feature)
+    if usage is not None:
+        report_queue.put(usage)
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/minium_object.py` & `minium-1.5.4/minium/miniprogram/base_driver/minium_object.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/page/__init__.py` & `minium-1.5.4/minium/miniprogram/base_driver/page/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,46 +1,49 @@
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-06-13 20:11:47
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-12-05 17:17:42
+LastEditTime: 2024-03-08 16:53:03
 FilePath: /py-minium/minium/miniprogram/base_driver/page/__init__.py
 Description: 页面实例
 '''
 from __future__ import annotations
 import typing
 if typing.TYPE_CHECKING:
     from ..app import App
+from ..minium_log import report_exception, report_usage, ExceptionData
 from ..callback import Callback
 from ....utils.platforms import *
 from ....utils.utils import ProcessSafeEventLoop, AsyncCondition, get_result, catch, WaitTimeoutError
 from ....utils import lazy_import
 from ....framework.exception import *
 from .page import Page
 from .skylinepage import SkylinePage
 # 插件模块使用懒加载
 if typing.TYPE_CHECKING:
     from . import h5page
 else:
-    h5page = lazy_import("minium.miniprogram.base_driver.page.h5page")
+    h5page = lazy_import(".h5page", __package__)
 
 
 def _get_h5_config(page: Page):
     return h5page.H5Config(
         platform=page.app.platform,
         appid=page.app.app_id,
         device={
             "uiautomator_version": page.app.native.uiautomator_version,
             "serial": page.app.native.serial
         } if page.app.platform in (OS_ANDROID,) else {}
     )
 
+@report_exception
 def _check_webview(page: Page):
     if page.is_webview:  # 当前页面是h5页面
         page.logger.debug(f"loading h5 page {page.path}")
+        report_usage("H5")
         config = _get_h5_config(page)
         try:
             debugger_url = h5page.H5Page.get_websocket_debugger_url(config)
         except (NotImplementedError, ValueError):
             debugger_url = page.app.native.get_websocket_debugger_url()
         if debugger_url:
             page.logger.info(f"get page[{page.page_id}:{page.path}] websocket debugger url succ: {debugger_url}")
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/page/h5page.py` & `minium-1.5.4/minium/miniprogram/base_driver/page/h5page.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*-coding: utf-8 -*-
 '''
 Author: yopofeng yopofeng@tencent.com
 Date: 2023-04-03 11:32:50
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2023-12-05 16:35:32
+LastEditTime: 2024-04-17 20:05:46
 FilePath: /py-minium/minium/miniprogram/base_driver/page/h5page.py
 Description: h5页面实例
 '''
 
 import logging
 import re
 import time
@@ -15,71 +15,29 @@
 import subprocess
 import requests
 import json
 import socket
 import threading
 from .page import Page
 from websockets.sync.client import connect
-from minium.miniprogram.h5tools.h5PageOperator import H5PageOperator
-from minium.miniprogram.h5tools.utils import timer, print_caller_info_decorator
-from minium.miniprogram.h5tools.client import CDPClient, AndroidClient
-from minium.miniprogram.h5tools.exceptions import NoSuchElementException
-from minium.miniprogram.base_driver.h5_element import H5Element
+from ...h5tools.h5PageOperator import H5PageOperator
+from ...h5tools.utils import timer, print_caller_info_decorator
+from ...h5tools.client import Sock, AndroidClient
+from ...h5tools.exceptions import NoSuchElementException
+from ..h5_element import H5Element
 
 
 logger = logging.getLogger("minium")
-# 使用at的sock
-# from minium.native.lib.at.webdriver import driver
 
 _ADB_GET_TOP_ACTIVITY_CMD = {
     "Darwin": "adb shell dumpsys activity top | grep ACTIVITY | grep appbrand",  # Mac os 下查找字符串是grep
     "Linux": "adb shell dumpsys activity top | grep ACTIVITY | grep appbrand",  # Mac os 下查找字符串是grep
-    "Windows": "adb shell dumpsys activity top | findstr ACTIVITY | grep appbrand"  # windows 下查找字符串是findstr
+    "Windows": "adb shell dumpsys activity top | findstr ACTIVITY | findstr appbrand"  # windows 下查找字符串是findstr
 }
 
-
-class Sock:
-    def __init__(self, url):
-        self._url = url
-        self._req_id = 0
-        self.logger = logger
-
-    def async_request_cdp(self, sendStr):
-        "不阻塞异步执行, 不需要返回数据"
-        with connect(self._url) as websocket:
-            websocket.send(self._set_req_id(sendStr))
-
-    def sync_request_cdp(self, sendStr):
-        "阻塞直到获取返回数据, 或者超时报错"
-        with connect(self._url) as websocket:
-            send_message = self._set_req_id(sendStr)
-            websocket.send(send_message)
-            rec_message = websocket.recv(timeout=20)
-            return json.loads(rec_message)
-
-    def _set_req_id(self, params):
-        "添加请求websocket请求id"
-        self._req_id += 1
-        if isinstance(params, dict):
-            params["id"] = self._req_id
-            params = json.dumps(params, ensure_ascii=False)
-        elif isinstance(params, str):
-            try:
-                self.logger.info(f"未带id的协议参数{params}")
-                params_dict = json.loads(params)
-                params_dict["id"] = self._req_id
-                params = json.dumps(params_dict, ensure_ascii=False)
-            except json.JSONDecodeError:
-                self.logger.error(f"Invalid JSON string: {params}")
-        else:
-            self.logger.info(f"Unsupported params type: {type(params)}")
-            return None
-        return params
-
-
 class H5Config(dict):
     platform: str = ""
     appid: str = ""
     device: dict = {}  # https://minitest.weixin.qq.com/#/minium/Python/framework/config?id=device_desire%e9%85%8d%e7%bd%ae%e9%a1%b9
 
     def __init__(self, **kwargs):
         for k in kwargs:
@@ -509,14 +467,43 @@
                 break
 
         if not node_id:
             raise NoSuchElementException(picker)
 
         return H5Element(self.client, node_id)
 
+    @timer(10, 2)
+    def get_elements(
+            self,
+            picker: str,
+            *args
+    ):
+        """
+        :param  picker: 支持xpath, selector, 文案定位
+        :return: List
+        """
+        self.client.send_command("DOM.getDocument")
+
+        if isinstance(picker, str) or (len(args) < 2 and isinstance(args, str)):
+            picker = picker if picker else args
+            result = self.client.send_command("DOM.performSearch", {"query": picker})
+            search_id, count = result['result']["searchId"], result['result']["resultCount"]
+        else:
+            raise ValueError("Invalid arguments")
+
+        if count == 0:
+            raise Exception(f"No element found for xpath: {picker}")
+
+        node_ids = self.client.send_command("DOM.getSearchResults", {
+            "searchId": search_id,
+            "fromIndex": 0,
+            "toIndex": count,
+        })['result']['nodeIds']
+        return [H5Element(self.client, node_id) for node_id in node_ids]
+
     def scroll_to(self, scroll_top, duration=1):
         """
         滚动到指定位置
         :param scroll_top:  位置 px
         :param duration:  滚动时长为秒
         :return:
         """
@@ -699,15 +686,15 @@
         获取微信小程序H5进程号
         """
         os_name = platform.system()
         cmd = _ADB_GET_TOP_ACTIVITY_CMD[os_name]
         try:
             stdout, std_error = self._run_command(self._specify_device_on_cmd(cmd, device))
             str_list = stdout.split('pid=')
-            pid = str_list[1].split("\r\n")[0]
+            pid = re.split("\s", str_list[1])[0]
             return pid
         except RuntimeError as e:
             self.logger.error(f"获取内嵌H5进程号失败，请检查设备是否在线: {e}")
             return None
 
     def _run_command(self, cmd, printDetails=False, cwd=None):
         """
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/page/page.py` & `minium-1.5.4/minium/miniprogram/base_driver/page/page.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,19 +6,21 @@
 @Description: 小程序页面
 @Date: 2019-03-11 14:42:29
 @LastEditTime: 2019-06-05 17:04:02
 """
 from __future__ import annotations
 import re
 from functools import wraps
+from typing import Union
 from typing_extensions import Self
-from minium.framework.exception import MiniElementNotFoundError, MiniAppError, MiniTimeoutCauseByConnectionBreakError, MiniLowVersionSdkError
+from ....framework.exception import MiniElementNotFoundError, MiniAppError, MiniTimeoutCauseByConnectionBreakError, MiniLowVersionSdkError, PageDestroyed
 import typing
 import types
 from ..element import *
+from ..selector import Selector
 from ..minium_object import MiniumObject, RetryableApi
 # from .h5page import H5Page, H5Config
 from ....utils.utils import timeout
 from ..connection import Command
 import json
 if typing.TYPE_CHECKING:
     from ..app import App
@@ -90,15 +92,15 @@
         self.app = None
 
     def __repr__(self):
         return "Page(id={0}, path={1}, query={2})".format(
             self.page_id, self.path, self.query
         )
 
-    def __eq__(self, page: Self or str):
+    def __eq__(self, page: Union[Self, str]):
         """
         重载 ==
         直接对比page path和query
         """
         if isinstance(page, Page):
             # 都有page id的情况, 直接判断id即可
             if page.page_id and self.page_id:
@@ -117,15 +119,15 @@
                 page_path = re.sub(Page.PLUGIN_PATH_REG, "", page.path)
                 return self_path == page_path
             return self.path == page.path
         else:
             _page = Page(None, page, None, None)
             return self == _page
 
-    def __ne__(self, page: Self or str) -> bool:
+    def __ne__(self, page: Union[Self, str]) -> bool:
         return not (self == page)
 
     @property
     def data(self):
         """
         获取页面 Data
         :return: json
@@ -215,15 +217,15 @@
                 return False
         return self._is_webview
     
     @is_webview.setter
     def is_webview(self, v: bool):
         self._is_webview = v
 
-    def wait_data_contains(self, *keys_list: list or str, max_timeout: int = 10):
+    def wait_data_contains(self, *keys_list: Union[list, str], max_timeout: int = 10):
         """
         description: 等待Page.data中包含指定keys
         param {*} self
         param {array} keys_list: items is list or str split by "."
         param {int} max_timeout
         return {bool}
         """
@@ -278,15 +280,15 @@
                 text_contains=text_contains,
             ),
             max_timeout,
         )
 
     def get_element(
         self,
-        selector: str,
+        selector: Union[str, Selector],
         inner_text=None,
         text_contains=None,
         value=None,
         max_timeout=0,
         xpath=None,
     ) -> ElementType:
         """
@@ -308,30 +310,29 @@
         :param selector: CSS选择器/XPATH
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
         :param max_timeout: 超时时间
         :return:element 对象
         """
-        if (selector and selector.startswith("/")) or xpath:
+        if isinstance(selector, Selector):
+            _selector = selector
+        else:
+            _selector = Selector(css=selector, text=inner_text, contains_text=text_contains, val=value)
+        selector, is_xpath = _selector.check_selector()
+        if is_xpath:
             # use xpath
             return self.get_element_by_xpath(
-                xpath or selector,
+                _selector,
                 max_timeout=max_timeout,
-                inner_text=inner_text,
-                value=value,
-                text_contains=text_contains,
             )
+        _selector.index = 0
         r = self.get_elements(
-            selector,
+            _selector,
             max_timeout,
-            inner_text=inner_text,
-            value=value,
-            text_contains=text_contains,
-            index=0,
         )
         if not r:
             raise MiniElementNotFoundError("element[%s] not found" % selector)
         return r[0]
 
     def call_method(self, method, args=None):
         if not args:
@@ -371,15 +372,15 @@
                     return True
                 else:
                     time.sleep(0.25)
             return False
 
     def get_elements(
         self,
-        selector,
+        selector: Union[Selector, str],
         max_timeout=0,
         inner_text=None,
         text_contains=None,
         value=None,
         index=-1,
         xpath=None,
     ) -> typing.List[ElementType]:
@@ -390,49 +391,48 @@
         :param value: value
         :param text_contains: 包含的文字
         :param max_timeout: 超时时间
         :param index: index == -1: get所有, index >=0: get index+1个
         :param xpath: 使用xpath
         :return:element 对象 list
         """
-        if selector and selector.startswith("/"):
-            # 以/或//开头的认为是xpath
-            xpath = selector
-            selector = None
-        if inner_text is None and value is None and text_contains is None:
-            need_filter = False
+        if isinstance(selector, Selector):
+            _selector = selector
         else:
-            need_filter = True
-        if not need_filter and selector:
+            _selector = Selector(css=selector, text=inner_text, contains_text=text_contains, val=value, index=index)
+        selector, is_xpath = _selector.check_selector()
+        if not _selector.need_filter and _selector.css:
             # 不需要过滤内容，直接返回
-            return self._get_elements_by_css(selector, max_timeout, index=index)
-        elif xpath:
+            return self._get_elements_by_css(_selector, max_timeout, index=_selector.index)
+        elif is_xpath:
             # xpath支持text() contains()等条件，不需要额外做过滤
             return self.get_elements_by_xpath(
-                xpath,
-                max_timeout=max_timeout,
-                inner_text=inner_text,
-                text_contains=text_contains,
-                value=value,
+                _selector,
+                max_timeout=max_timeout
             )
 
         @timeout(max_timeout)
         def filter_elements():
             # 需要过滤内容，有返回元素不是终结条件, 需要获取所有元素后再作过滤
-            elements = self._get_elements_by_css(selector, max_timeout, index=-1)
+            new_selector = Selector(_selector)
+            new_selector.index = -1
+            elements = self._get_elements_by_css(new_selector, max_timeout)
             els = []
             for element in elements:
-                if inner_text and element.inner_text != inner_text:
+                if _selector.text and element.inner_text != _selector.text:
                     continue
-                if value and element.value() != value:
+                if _selector.val and element.value() != _selector.val:
                     continue
-                if text_contains and text_contains not in element.inner_text:
+                if _selector.contains_text and _selector.contains_text not in element.inner_text:
                     continue
+                # element.selector.text = inner_text
+                # element.selector.contains_text = text_contains
+                # element.selector.val = value
                 els.append(element)
-                if len(els) == (index + 1):
+                if len(els) == (_selector.index + 1):
                     return els
             return els
 
         return filter_elements()
 
     def scroll_to(self, scroll_top, duration=300):
         """
@@ -460,52 +460,60 @@
         根据xpath查找元素
         :param xpath: xpath
         :param max_timeout: 超时时间
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
         """
+        if isinstance(xpath, Selector):
+            _selector = xpath
+        else:
+            _selector = Selector(xpath=xpath, text=inner_text, contains_text=text_contains, val=value, index=index)
         if inner_text is not None:
-            xpath += '[text()="%s"]' % inner_text
+            _selector.text = inner_text
         elif text_contains is not None:
-            xpath += '[contains(text(), "%s")]' % text_contains
+            _selector.contains_text = text_contains
         elif value is not None:
-            xpath += '[@value="%s"]' % value
+            _selector.val = value
 
         @timeout(max_timeout)
         def search_elements():
-            return self._get_elements_by_xpath(xpath, index=index)
+            return self._get_elements_by_xpath(_selector)
 
         return search_elements()
 
     def get_element_by_xpath(
         self, xpath, max_timeout=10, inner_text=None, value=None, text_contains=None
     ) -> ElementType:
         """
         根据xpath查找元素
         :param xpath: xpath
         :param max_timeout: 超时时间
         :param inner_text: inner_text
         :param value: value
         :param text_contains: 包含的文字
         """
+        if isinstance(xpath, Selector):
+            _selector = xpath
+        else:
+            _selector = Selector(xpath=xpath, text=inner_text, contains_text=text_contains, val=value)
         if inner_text is not None:
-            xpath += '[normalize-space(text())="%s"]' % inner_text
+            _selector.text = inner_text
         elif text_contains is not None:
-            xpath += '[contains(text(), "%s")]' % text_contains
+            _selector.contains_text = text_contains
         elif value is not None:
-            xpath += '[@value="%s"]' % value
+            _selector.val = value
 
         @timeout(max_timeout)
         def search_element():
-            return self._get_element_by_xpath(xpath)
+            return self._get_element_by_xpath(_selector)
 
         el = search_element()
         if not el:
-            raise MiniElementNotFoundError("element[%s] not found" % xpath)
+            raise MiniElementNotFoundError("element[%s] not found" % _selector.to_selector())
         return el
 
     def _get_window_properties(self, names=None):
         """
         获取 window 对象的属性值。
         :param names:
         :return:
@@ -523,20 +531,22 @@
         # self.logger.debug(f"method {method}, params: {params}")
         return (
             self.connection.send(method, params)
             if sync
             else self.connection.send_async(method, params)
         )
 
-    def __get_elements(self, selector: str, index=-1):
+    def __get_elements(self, selector: Union[str, Selector], index=-1):
+        if not isinstance(selector, Selector):
+            selector = Selector(css=selector, index=index)
         elements = []
-        ret = self._send("Page.getElements", {"selector": selector})
+        ret = self._send("Page.getElements", {"selector": selector.css})
         for el in ret.result.elements:
-            elements.append(create(el, self.page_id, self.connection))
-            if len(elements) == (index + 1):  # index==-1时，不会match，就会全部返回
+            elements.append(create(el, self.page_id, self.connection, selector, page=self))
+            if len(elements) == (selector.index + 1):  # index==-1时，不会match，就会全部返回
                 return elements
         return elements
 
     def __search_child(
         self, selector_list: list, parent: ElementType = None, index=-1
     ) -> typing.List[ElementType]:
         # index == -1: get所有, index >=0: get index+1个
@@ -571,46 +581,51 @@
             )  # selector_list[0:]相当于copy
             child_els += child_el
             if len(child_els) == (index + 1):
                 return child_els
         return child_els
 
     def _get_elements_by_css(
-        self, selector: str, max_timeout=0, index=-1
+        self, selector: Union[str, Selector], max_timeout=0, index=-1
     ) -> typing.List[ElementType]:
         """
         1. 现存自定义组件中的class会自动加前缀，但不包括slot占位的元素
         2. slot元素的class命名规则
         2.1 <page><test><view class="这个class不会加前缀"></view></test></page>
         2.2 <custom><test><view class="这个class会加上custom组件对应的前缀"></view></test></custom>
         3. 自定义组件中通过id获取元素失败
         """
-
+        if isinstance(selector, Selector):
+            _selector = selector
+        else:
+            _selector = Selector(css=selector, index=index)
         @timeout(max_timeout)
-        def search_elements(_selector: list or tuple):
+        def search_elements(_selectors: Union[list, tuple]):
             return self.__search_child(
-                _selector[0:], index=index
+                _selectors[0:], index=index
             )  # __search_child回pop元素，第一次search失败后重试会有问题，copy一份
 
-        self.logger.info("try to get elements: %s" % selector)
-        _selector_list = selector.split(">>>")
+        self.logger.info("try to get elements: %s" % _selector.css)
+        _selector_list = _selector.css.split(">>>")
         _selector_list.reverse()  # 新增处理【>>>】穿透自定义组件逻辑
         els = search_elements(_selector_list)
         if len(els) == 0:
-            self.logger.warning(f"Could not found any element '{selector}' you need")
+            self.logger.warning(f"Could not found any element '{_selector.css}' you need")
         else:
             self.logger.info("find elements success: %s" % str(els))
         return els
 
     def _get_element(self, selector, max_timeout=0) -> ElementType:
+        if not isinstance(selector, Selector):
+            selector = Selector(css=selector)
         def search_element():
-            ret = self._send("Page.getElement", {"selector": selector})
-            return create(ret.result, self.page_id, self.connection)
+            ret = self._send("Page.getElement", {"selector": selector.css})
+            return create(ret.result, self.page_id, self.connection, selector, page=self)
 
-        self.logger.info("try to get element: %s" % selector)
+        self.logger.info("try to get element: %s" % selector.css)
         el = search_element()
         self.logger.info("find element success: %s" % str(el))
         return el
 
     def _element_is_exists(
         self, selector: str = None, xpath: str = None, **kwargs
     ) -> bool:
@@ -633,14 +648,16 @@
                 )
             else:
                 return (
                     True
                     if self.get_elements_by_xpath(xpath, 0, index=0, **kwargs)
                     else False
                 )
+        except PageDestroyed:
+            raise
         except Exception:
             return False
 
     # 正式支持xpath后，考虑复用get_element接口，通过检测selector类型来决定使用什么选择器
     # def _is_xpath(self, selector):
     #     """
     #     检测一个selector是否是xpath
@@ -655,62 +672,91 @@
     #         return True
     #     try:
     #         translator.css_to_xpath(selector)
     #         return False
     #     except SelectorError:
     #         return True
     #     return False
+        
+    def _is_origin_xpath(self, xpath: str):
+        return xpath.startswith("/html") or xpath.startswith("/body") or re.search("/wx-\w+", xpath)
+        
+    def _resolve_xpath(self, xpath: str):
+        """
+        解析xpath
+        """
+        xpath = (
+            xpath[5:] if xpath.find("/page/") == 0 else xpath
+        )  # xpath不能以/page/开头（不存在的根节点）
+        # /html/body/wx-view[9]/wx-mytest//wx-test2/wx-view[1]/wx-view[2]/wx-text/span[2]
+        # /html/wx-tab-bar-wrapper/tab-bar/wx-view/wx-view[3]/wx-view -> /tab-bar-wrapper/view/view[3]/view
+        # /html/wx-root-portal-content/wx-view/wx-view -> /root-portal-content/view/view
+        # /html/body/wx-scroll-view/div/div[1]/div/wx-view[1]/wx-popup/wx-root-portal/wx-root-portal-content/wx-view/wx-view
+        # `root-portal`:
+        # for 录制回放: /root-portal-content/xxx -> //root-portal-content/xxx
+        # for chrome inpector: 未弹出: /html/body//wx-root-portal/wx-root-portal-content/xxx, 弹出: /html/wx-root-portal-content/xxx
+        # is original xpath
+        # 如果xpath中包含`wx-`标签
+        if self._is_origin_xpath(xpath):
+            xpath = re.sub(r"/wx-", "/", "/".join(filter(lambda xp: not xp or xp.find("wx-") == 0, xpath.split("/"))))
+            self.logger.info(f"maybe you are finding xpath: {xpath}")
+            return xpath
+        return xpath
 
     def _get_element_by_xpath(self, xpath: str) -> ElementType:
         """
         description: 通过xpath获取元素
         param {*} self
         param {str} xpath
         return {*} ElementType or None
         """
-        xpath = (
-            xpath[5:] if xpath.find("/page/") == 0 else xpath
-        )  # xpath不能以/page/开头（不存在的根节点）
+        if isinstance(xpath, Selector):
+            _selector = xpath
+        else:
+            _selector = Selector(xpath=xpath)
+        _selector.xpath = self._resolve_xpath(_selector.xpath)
         try:
-            ret = self._send("Page.getElementByXpath", {"selector": xpath})
+            ret = self._send("Page.getElementByXpath", {"selector": _selector.to_selector()})
         except MiniAppError as e:
             if str(e) == "no such element":
                 return None
             raise
-        return create(ret.result, self.page_id, self.connection)
+        return create(ret.result, self.page_id, self.connection, _selector, page=self)
 
-    def _get_elements_by_xpath(self, xpath: str, index=-1) -> typing.List[ElementType]:
+    def _get_elements_by_xpath(self, xpath: Union[str, Selector], index=-1) -> typing.List[ElementType]:
         """
         description: 通过xpath获取元素
         param {*} self
         param {str} xpath
         return {*} List[ElementType]
         """
-        xpath = (
-            xpath[5:] if xpath.find("/page/") == 0 else xpath
-        )  # xpath不能以/page/开头（不存在的根节点）
+        if isinstance(xpath, Selector):
+            _selector = xpath
+        else:
+            _selector = Selector(xpath=xpath, index=index)
+        _selector.xpath = self._resolve_xpath(_selector.xpath)
         if not self._can_i_use("Page.getElementsByXpath"):
-            el = self._get_element_by_xpath(xpath)  # 降级使用Page.getElementByXpath
+            el = self._get_element_by_xpath(_selector)  # 降级使用Page.getElementByXpath
             return [el] if el else []
         try:
-            ret = self._send("Page.getElementsByXpath", {"selector": xpath})
+            ret = self._send("Page.getElementsByXpath", {"selector": _selector.to_selector()})
         except MiniAppError as e:
             if str(e) == "no such element":
                 return []
             if (
                 str(e).find("Page.getElementsByXpath unimplemented") > 0
             ):  # or str(e) in ["r is not iterable",]:
                 self._unset_interface("Page.getElementsByXpath")
-                el = self._get_element_by_xpath(xpath)  # 降级使用Page.getElementByXpath
+                el = self._get_element_by_xpath(_selector)  # 降级使用Page.getElementByXpath
                 return [el] if el else []
             raise
         elements = []
         for el in ret.result.elements:
-            elements.append(create(el, self.page_id, self.connection))
-            if len(elements) == (index + 1):
+            elements.append(create(el, self.page_id, self.connection, _selector, page=self))
+            if len(elements) == (_selector.index + 1):
                 return elements
         return elements
 
     def _page_evaluate(self, app_function: str, args=None, sync=True):
         """
         在当前页面执行命令
         """
```

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/page/skylinepage.py` & `minium-1.5.4/minium/miniprogram/base_driver/page/skylinepage.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/prefixer.py` & `minium-1.5.4/minium/miniprogram/base_driver/prefixer.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/base_driver/version.py` & `minium-1.5.4/minium/miniprogram/base_driver/version.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/client.py` & `minium-1.5.4/minium/miniprogram/h5tools/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 LastEditTime: 2023-10-18 10:41:34
 FilePath: /py-minium/minium/miniprogram/h5tools/client.py
 Description: h5 通信模块
 '''
 import logging
 import json
 from websockets.sync.client import connect
+from wechat_mp_inspector import AndroidConfig, AndroidDriver
+
 
 logger = logging.getLogger("minium")
 
 
 class CDPClient:
 
     _request_id = 0
@@ -45,19 +47,20 @@
             if 'id' in response_data and response_data['id'] == type(self)._request_id:
                 return response_data
 
     def disconnect(self):
         if self.websocket:
             self.websocket.close()
 
+
 # new client
-from wechat_mp_inspector import AndroidConfig, AndroidDriver
 class AndroidClient:
     CACHE = {}
     driver: AndroidDriver = None
+
     def __init__(self, config: dict) -> None:
         self.inspector = None
         self.page = None
         key = f"{config.device['serial']}-{config.appid}" if config.appid else f"{config.device['serial']}"
         if key in AndroidClient.CACHE:
             self.driver = AndroidClient.CACHE[key]
         else:
@@ -73,10 +76,47 @@
         if not self.page:
             logger.warning(f"driver无法获取 {debugger_url} 的page实例")
             raise RuntimeError(f"driver无法获取 {debugger_url} 的page实例")
         inspector = self.driver.inspector_session(self.page)
         for e in enable_list:
             inspector.send_command(e)
         return inspector
-        
 
 
+class Sock:
+
+    def __init__(self, url):
+        self._url = url
+        self._req_id = 0
+        self.logger = logger
+
+    def async_request_cdp(self, sendStr):
+        "不阻塞异步执行, 不需要返回数据"
+        with connect(self._url) as websocket:
+            websocket.send(self._set_req_id(sendStr))
+
+    def sync_request_cdp(self, sendStr):
+        "阻塞直到获取返回数据, 或者超时报错"
+        with connect(self._url) as websocket:
+            send_message = self._set_req_id(sendStr)
+            websocket.send(send_message)
+            rec_message = websocket.recv(timeout=20)
+            return json.loads(rec_message)
+
+    def _set_req_id(self, params):
+        "添加请求websocket请求id"
+        self._req_id += 1
+        if isinstance(params, dict):
+            params["id"] = self._req_id
+            params = json.dumps(params, ensure_ascii=False)
+        elif isinstance(params, str):
+            try:
+                self.logger.info(f"未带id的协议参数{params}")
+                params_dict = json.loads(params)
+                params_dict["id"] = self._req_id
+                params = json.dumps(params_dict, ensure_ascii=False)
+            except json.JSONDecodeError:
+                self.logger.error(f"Invalid JSON string: {params}")
+        else:
+            self.logger.info(f"Unsupported params type: {type(params)}")
+            return None
+        return params
```

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/commandProcessor.py` & `minium-1.5.4/minium/miniprogram/h5tools/commandProcessor.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/exceptions.py` & `minium-1.5.4/minium/miniprogram/h5tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/h5CommandManager.py` & `minium-1.5.4/minium/miniprogram/h5tools/h5CommandManager.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/h5PageOperator.py` & `minium-1.5.4/minium/miniprogram/h5tools/h5PageOperator.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/h5UserAPI.py` & `minium-1.5.4/minium/miniprogram/h5tools/h5UserAPI.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/jsonConcat.py` & `minium-1.5.4/minium/miniprogram/h5tools/jsonConcat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import json
 import string
 
-from minium.miniprogram.h5tools import h5CommandManager
+from . import h5CommandManager
 
 
 class JsonConcat(object):
     def __init__(self, managerType):
         if managerType == "h5":
             self.manager = h5CommandManager.H5CommandManager()
```

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/logger.py` & `minium-1.5.4/minium/miniprogram/h5tools/logger.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/h5tools/utils.py` & `minium-1.5.4/minium/miniprogram/h5tools/utils.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/qq_minium.py` & `minium-1.5.4/minium/miniprogram/qq_minium.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/miniprogram/wx_minium.py` & `minium-1.5.4/minium/miniprogram/wx_minium.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,23 @@
 import os
 import base64
 import json
 import re
 import threading
 import time
 from websocket import WebSocketConnectionClosedException
+from typing import Union, Optional
 
-from minium.utils.injectjs import getInjectJsCode, setInjectJsMode
+from ..utils.injectjs import getInjectJsCode, setInjectJsMode
 from .base_driver.version import build_version
 from .base_driver.minium import BaseMinium
 from .base_driver.app import App
-from .base_driver.connection import Connection
+from .base_driver.connection import Connection, Command
 from .base_driver.minium_object import MiniumObject
+from .base_driver.callback import Callback
 from ..framework.miniconfig import MiniConfig, get_log_level
 from ..framework.exception import *
 from ..native import get_native_driver, NativeType
 from ..utils.platforms import *
 from ..utils.utils import (
     isWindows,
     isMacOS,
@@ -47,22 +49,40 @@
 class LogLevel(object):
     INFO = 20
     DEBUG_SEND = 12
     METHOD_TRACE = 11
     DEBUG = 9
 
 
+class ConfigPath(str): ...
+class ProjectPath(str): ...
+
+def is_project_path(path: str):
+    project_private_config_path = os.path.join(path, "project.private.config.json")
+    project_config_path = os.path.join(path, "project.config.json")
+    if os.path.isfile(project_config_path) or os.path.isfile(project_private_config_path):
+        return True
+    return False
+
+def is_config_path(path: str) -> Union[bool, MiniConfig]:
+    if os.path.isfile(path):
+        try:
+            return MiniConfig.from_file(path)
+        except:
+            return False
+    return False
+
 class WXMinium(BaseMinium):
     """
     自动化入口
     """
 
     def __init__(
         self,
-        conf: MiniConfig = None,
+        conf: Union[MiniConfig, ConfigPath, ProjectPath] = None,
         uri="ws://localhost",
         native: NativeType = None,
         **kwargs,
     ):
         """
         初始化
         :param uri: WebSocket 地址
@@ -73,25 +93,34 @@
         # 私有变量
         self.__wait_for_initialized_time = None  # 等待app.initialized信号的最后时间
         # 公有变量
         if not conf:
             conf = MiniConfig()
         elif isinstance(conf, dict):
             conf = MiniConfig(conf)
+        elif isinstance(conf, str):
+            # 识别是否是 config.json / project_path
+            ret = is_config_path(conf)
+            if ret is not False:
+                conf = ret
+            elif is_project_path(conf):
+                conf = MiniConfig({"project_path": conf})
+            else:
+                raise ValueError(f"{conf} 不是合法的 project path 或 config path")
         self.conf = conf
         self.logger.setLevel(get_log_level(conf.debug_mode))
         self.logger.debug(self.conf)
         self._native = native
         if native is None and conf.platform:
             try:
                 self._native = get_native_driver(conf.platform, conf)
             except KeyError as ke:  # 配置不全
                 self.logger.error(ke)
-            except:
-                self.logger.warning(f"instantiate {conf.platform} native driver fail")
+            except Exception as e:
+                self.logger.warning(f"instantiate {conf.platform} native driver fail: {str(e)}")
             else:
                 if not self.native.is_in_wechat():
                     self.native.start_wechat()
         self.version = build_version().get("version", "1.2.0")
         self.sdk_version: Version = Version("0.0.0")
         self.dev_tool_version: Version = Version("0.0.0")
         self.platform = "ide"  # ide, android, ios
@@ -110,14 +139,15 @@
         self.ticket = conf.get("account_info", {}).get("ticket", None)
         self.project_path = conf.get("project_path", None)
         self.is_remote = False
         self.is_connected = False
         self.is_audits_running = False  # 体验评分在跑
         self.launch_app_lock = threading.RLock()  # 全局只需有一个launch app的线程
         self.__is_app_relaunching = False
+        self.last_launch_time = time.time()
         self.last_launch_cost_time = 1  # 最后一次拉起小程序需要的时间
         self.last_launch_error = None  # 成功为none
 
         try:
             self.launch_weapp()
 
             if self.native:
@@ -137,34 +167,38 @@
             raise
 
     @property
     def app(self) -> App:
         return self._app
 
     @app.setter
-    def app(self, v: App or None):
+    def app(self, v: Optional[App]):
         if v:
             setInjectJsMode(v.js_mode)  # 每次更新app实例时更新一下
         self._app = v
 
     @property
     def native(self) -> NativeType:
         return self._native
     
     @native.setter
-    def native(self, v: NativeType or None):
+    def native(self, v: Optional[NativeType]):
         platform_change = False
         if v:
             if self._native is None or self._native.platform != v.platform:
                 platform_change = True
         self._native = v
         if platform_change:
             self._native_platform_change(self._native.platform)
 
-    def __get_dev_tool_info(self):
+    @property
+    def page(self) -> App.CurrentPage:
+        return self.app.current_page
+
+    def _get_dev_tool_info(self):
         try:
             result = self.connection.send("Tool.getInfo", max_timeout=3).result
         except:
             # not support Tool.getInfo
             return
         self.sdk_version = Version(result.SDKVersion)
         if self.sdk_version < Version("2.7.3"):
@@ -231,42 +265,43 @@
             self.native.release_auto_authorize()
         self.native = None
 
     def __getattr__(self, name):
         """
         当minium中方法不存在且native中存在，返回native的方法
         """
-        if name != "native" and self.native:
+        if name != "native" and name != "_native" and self.native:
             item = getattr(self.native, name, None)
             if callable(item):
                 return item
         raise AttributeError(
             "'%s' object has no attribute '%s'" % (self.__class__.__name__, name)
         )
 
-    def __wait_app_initialized(self, timeout, signal):
+    def __wait_app_initialized(self, signal: Command):
         """
-        等待 {signal} 信号, 代表小程序ready了, 可以响应命令了
+        等待 {signal.method} 信号, 代表小程序ready了, 可以响应命令了
         """
         self.__wait_for_initialized_time = time.time()
+        timeout = signal.max_timeout
         self.logger.info(
-            "wait for [%s], start at %d" % (signal, self.__wait_for_initialized_time)
+            "wait for [%s], start at %d" % (signal.method, self.__wait_for_initialized_time)
         )
-        ret = self.connection.wait_for(method=signal, max_timeout=timeout)
+        ret = self.connection.wait_for(signal)
         ctime = time.time()
         if not ret and (ctime - self.__wait_for_initialized_time) < timeout:
             # 没有监听到信号，同时等待期间时间有更新
+            if signal.is_cancel:
+                return ret
+            signal.max_timeout = timeout - (ctime - self.__wait_for_initialized_time)
             self.logger.warning(
                 "rewait [%s] for %f"
-                % (signal, timeout - (ctime - self.__wait_for_initialized_time))
-            )
-            ret = self.connection.wait_for(
-                method=signal,
-                max_timeout=timeout - (ctime - self.__wait_for_initialized_time),
+                % (signal.method, signal.max_timeout)
             )
+            ret = self.connection.wait_for(signal)
         return ret
 
     def _evaluate_js(
         self,
         filename,
         args=None,
         sync=True,
@@ -489,25 +524,69 @@
                 raise
             except MiniLaunchError as ml:  # 怎么都拉不起, 尝试重启小程序
                 if self.native:
                     self.native.start_wechat()
                 raise ml
             self.qr_code = path
 
+    def _app_initialized_callback(self, args):
+        params = args[0] if isinstance(args, (tuple, list)) and len(args) == 1 else args
+        self.logger.info("receive App.initialized")
+        if params and params.get("from") == "devtools":
+            def _relaunch():
+                if not self.launch_app_lock.acquire(False):
+                    self.logger.info("other thread relaunching app")
+                    # 已经有线程在 launch weapp
+                    return
+                self.logger.info("start instantiate app %d" % threading.get_ident())
+                self.__is_app_relaunching = True
+                stime = time.time()
+                # 真机调试下也有可能刷
+                try:
+                    self._get_system_info()
+                    if self.platform != "ide":
+                        return
+                    if self.app:
+                        injected = self.app.evaluate("""function(){return (global.__minium__) ? true : false}""", sync=True).get("result", {}).get("result", False)
+                        if injected:
+                            self.logger.warning("receive App.initialized, but not relaunch miniprogram")
+                            return
+                    self._instantiate_app()
+                    if not self.app.is_injected:
+                        self._inject()
+                except Exception as e:
+                    self.logger.exception(e)
+                finally:
+                    self.logger.info(f"end instantiate app, cost: {time.time() - stime}")
+                    self.__is_app_relaunching = False
+                    self.launch_app_lock.release()
+            t = threading.Thread(target=_relaunch)
+            t.setDaemon(True)
+            t.start()
+            return t
+
+    def _listen_app_initialized(self):
+        # listen {"method":"App.initialized","params":{"from":"devtools"}}
+        # 单例
+        self.connection.remove("App.initialized", self._app_initialized_callback)
+        self.connection.register("App.initialized", self._app_initialized_callback)
+
     def launch_weapp(self):
         """
         拉起小程序
         """
         self.__setup_dev_tool()
         stime = time.time()
         self.launch_dev_tool()
         if self.platform  == "ide":
             # launch/connect后仍然是ide, 需要启动远程调试
             self._native_platform_change(self.conf.get("platform", None))
         self.last_launch_cost_time = time.time() - stime
+        self._listen_app_initialized()
+        
 
     @property
     def is_app_relaunching(self):
         return self.__is_app_relaunching
 
     def _relaunch_ide(self, *args):
         """重新拉起ide
@@ -520,55 +599,60 @@
                 self.logger.info("other thread relaunching app")
                 # 已经有线程在 launch weapp
                 return
             self.logger.info("start relaunch app %d" % threading.get_ident())
             self.__is_app_relaunching = True
             stime = time.time()
             try:
+                if self.start_cmd and "--auto-account" in self.start_cmd and self.connection:
+                    try:
+                        self.logger.info("try to close tool")
+                        setattr(self.connection, "_is_close_by_cmd", True)
+                        self.connection.send_async("Tool.close", ignore_response=True)
+                        if self.native and self.platform != "ide":
+                            self.native.close_local_debug_modal()
+                    except:
+                        pass
                 if self.connection:
                     self.connection.destroy()
                 self.close_project()
                 self.launch_dev_tool()
-                if self.conf.get("platform", None) != "ide" and self.platform  == "ide":
-                    # launch/connect后仍然是ide, 需要启动远程调试
-                    try:
-                        path = self.enable_remote_debug(
-                            use_push=self.conf.get("use_push", True),
-                            connect_timeout=self.conf.get("remote_connect_timeout", 180),
-                        )
-                    except RemoteDebugConnectionLost:
-                        self.release()
-                        raise
-                    except MiniLaunchError as ml:  # 怎么都拉不起, 尝试重启小程序
-                        if self.native:
-                            self.native.start_wechat()
-                        raise ml
-                    self.qr_code = path
+                if self.platform  == "ide":
+                    self._native_platform_change(self.conf.get("platform", None))
                 self.last_launch_cost_time = time.time() - stime
                 self.last_launch_error = None
+                # 根据配置注入一些必要的代码
+                if not self.app.is_injected:
+                    self._inject()
+                self._listen_app_initialized()
             except Exception as e:
                 self.last_launch_error = e
                 self.logger.exception(e)
                 if self.connection:
                     self.connection.destroy()
             finally:
                 self.logger.info("end relaunch app")
                 self.__is_app_relaunching = False
                 self.launch_app_lock.release()
         t = threading.Thread(target=_relaunch)
         t.setDaemon(True)
         t.start()
+        return t
 
-    def __update_project_config(self):
+    def _update_project_config(self):
+        project_private_config_path = os.path.join(self.project_path, "project.private.config.json")
         project_config_path = os.path.join(self.project_path, "project.config.json")
         if os.path.isfile(project_config_path):
             conf = {}
             setting = {}
             with open(project_config_path, "r", encoding="UTF-8") as fd:
                 j = json.loads(fd.read().strip())
+            if os.path.isfile(project_private_config_path):
+                with open(project_private_config_path, "r", encoding="UTF-8") as fd:
+                    j.update(json.loads(fd.read().strip()))
             self.sdk_version = Version(
                 j.get("libVersion", "").strip() or self.sdk_version.version
             )
             if self.sdk_version < Version("2.7.3"):  # 尝试fix基础库版本信息
                 conf["libVersion"] = "3.0.0"  # latest应该是不合法的
             # update setting
             if j.get("setting", None) is None:
@@ -585,14 +669,17 @@
     def close_project(self):
         if not self.start_cmd:
             return
         if self.project_path and "--auto-account" not in self.start_cmd:
             self._dev_cli(f'close --project "{self.project_path}"')
 
     def launch_dev_tool(self):
+        """加载开发者工具
+        拉起开发者工具 -> 连接开发者工具 -> 实例化 App
+        """
         # start dev tool with minium model
         self.logger.info("Starting dev tool and launch MiniProgram project ...")
         is_port_in_use = False
         if self.project_path:
             if not os.path.exists(self.project_path):
                 raise MiniConfigError("project_path: %s not exists" % self.project_path)
             if not os.path.isdir(self.project_path):
@@ -602,15 +689,15 @@
             if not os.path.isfile(
                 os.path.join(self.project_path, "project.config.json")
             ):
                 raise MiniConfigError(
                     "can't find project.config.json in %s, please confirm the directory contains"
                     " miniproject project" % self.project_path
                 )
-            self.__update_project_config()
+            self._update_project_config()
             # config start cmd
             self.start_cmd = 'auto --project "%s" --auto-port %s' % (
                 self.project_path,
                 self.test_port,
             )
             if self.open_id:
                 self.start_cmd += f" --auto-account {self.open_id}"
@@ -679,32 +766,24 @@
                 return
             raise e
         except MiniLaunchError:
             # 初始化app error
             raise
 
     def connect_dev_tool(self):
+        """链接开发者工具并实例化 App"""
         i = 3
         while i:
             try:
                 self.logger.info("Trying to connect Dev tool ...")
                 self.connection = Connection.create(
                     self.uri, timeout=self.conf.get("request_timeout")
                 )
-                self.__get_dev_tool_info()
-                self._get_system_info()
-                if self.app:
-                    self.app.release()  # 释放上一个
-                self.app = App(
-                    self.connection,
-                    self.conf.get("auto_relaunch"),
-                    native=self.native,
-                    platform=self.platform,
-                    enable_h5=self.conf.get("enable_h5", True),
-                )
+                self._get_dev_tool_info()
+                self._instantiate_app()
                 ee.on("ide_closed", self._relaunch_ide)
             except RemoteDebugConnectionLost:  # 链接上了, 但小程序没有响应
                 raise
             except MiniLaunchError:
                 raise
             except Exception as e:
                 self.logger.exception(e)
@@ -729,14 +808,34 @@
         else:
             cmd_template = "%s login"
         # 需要输出二维码，所以直接用os.system就好了
         ret = os.system(cmd_template % self.dev_tool_path)
         if ret == 0:
             return self.launch_dev_tool()
 
+    def _instantiate_app(self):
+        """实例化 app"""
+        # 获取当前真正的 platform 
+        self._get_system_info()
+        if self.app:
+            app = self.app
+            app.release()  # 释放上一个
+            del app
+        self.app = App(
+            self.connection,
+            self.conf.get("auto_relaunch"),
+            native=self.native,
+            platform=self.platform,
+            enable_h5=self.conf.get("enable_h5", True),
+            # extra info
+            sdk_version=self.sdk_version
+        )
+        self.logger.info(f"new app instanst {self.app}")
+        self.last_launch_time = time.time()
+
     def get_app_config(self, *names):
         """
         获取 app 的配置
         :return: object
         """
         return self._evaluate_js("getAppConfig", args=names)
 
@@ -764,30 +863,26 @@
         if use_push:
             retry_times = RETRY_TIMES
             while retry_times > 0:
                 thread1 = None
                 thread2 = None
                 semaphore = threading.Semaphore(0)  # 用Semaphore标记其中一个信号已到达
                 try:
+                    cmd1 = Command("App.initialized", max_timeout=connect_timeout + 30 * (RETRY_TIMES - retry_times))
                     thread1 = WaitThread(
                         target=self.__wait_app_initialized,
-                        args=(
-                            connect_timeout + 30 * (RETRY_TIMES - retry_times),
-                            "App.initialized",
-                        ),
+                        args=(cmd1,),
                         semaphore=semaphore,
                     )
                     thread1.setDaemon(True)
                     thread1.start()
+                    cmd2 = Command("Tool.onRemoteDebugConnected", max_timeout=connect_timeout + 30 * (RETRY_TIMES - retry_times))
                     thread2 = WaitThread(
                         target=self.__wait_app_initialized,
-                        args=(
-                            connect_timeout + 30 * (RETRY_TIMES - retry_times),
-                            "Tool.onRemoteDebugConnected",
-                        ),
+                        args=(cmd2,),
                         semaphore=semaphore,
                     )
                     thread2.setDaemon(True)
                     thread2.start()
                     self.logger.info(
                         f"Enable remote debug, for the {4 - retry_times}th times"
                     )
@@ -809,50 +904,52 @@
                             " network or proxy effective or not "
                         )
                         raise
                     continue
                 else:
                     retry_times -= 1
                     ret1 = ret2 = False
-                    semaphore.acquire()  # 等待初始化信号
+                    if self.native:
+                        while not semaphore.acquire(timeout=10):
+                            # 等待初始化信号, 每 10s 检测一下是不是【断开连接】
+                            if not self.native.check_connected():
+                                self.logger.warning("出现连接断开的情况，重试...")
+                                break
+                    else:
+                        semaphore.acquire()  # 等待初始化信号
                     if thread1:
                         ret1 = thread1.get_result(block=False) or False
                     if thread2:
                         ret2 = thread2.get_result(block=False) or False
                     if retry_times == 0 and ret1 is False and ret2 is False:
                         self.logger.error(
                             "Wait for APP initialized has been fail three times. Please check your"
                             " phone's current foreground APP is WeChat or not, and check"
                             " miniProgram has been open or not "
                         )
                         raise MiniLaunchError("Launch APP Error")
+                    cmd1.cancel()
+                    cmd2.cancel()
                     if ret1 is True or ret2 is True:
                         break
                     else:
                         # 等不到App.initialized一般就是白屏，通道不通，exit会报错，跳出重试，需要catch
+                        # if self.native and not self.native.check_connected():
+                        #     self.logger.warning("出现连接断开的情况，重试...")
                         try:
                             self.app.exit()
                         except (MiniTimeoutError, MiniConnectionClosedError):
                             # 白屏的时候切换一下扫码编译，有时会有意想不到效果
                             self.connection.send(
                                 "Tool.enableRemoteDebug",
                                 params={"auto": False},
                                 max_timeout=connect_timeout,
                             )
             # 远程调试开启成功后，小程序运行态已经转到手机，需要重新实例化app
-            self._get_system_info()
-            if self.app:
-                self.app.release()  # 释放上一个
-            self.app = App(
-                self.connection,
-                self.conf.get("auto_relaunch"),
-                native=self.native,
-                platform=self.platform,
-                enable_h5=self.conf.get("enable_h5", True),
-            )
+            self._instantiate_app()
             setattr(self.connection, "_is_close_app_by_cmd", False)  # 重新拉起重置一下
             if not self.app.is_injected:
                 self._inject()
             return None
         if path is None:
             path = os.path.join(self.conf.outputs, "debug_qrcode.jpg")
         qr_data = self.connection.send(
@@ -966,15 +1063,15 @@
         self.stop_audits()
         self.shutdown()
         # 清理一下手机弹窗
         if self.conf.platform != "ide" and native:
             native.close_local_debug_modal()
         native = None
 
-    def wait_app_relaunch(self, timeout=None) -> None or Exception:
+    def wait_app_relaunch(self, timeout=None) -> Optional[Exception]:
         wait_launch_time = self.last_launch_cost_time + 20 if timeout is None else timeout
         self.logger.warning(f"app is relaunching, wait {wait_launch_time} seconds for it")
         if not self.launch_app_lock.acquire(timeout=wait_launch_time):
             return TimeoutError(f"app did not relaunch within {wait_launch_time} seconds")
         self.logger.warning("app is relaunch complete")
         self.launch_app_lock.release()
         if self.last_launch_error:
```

### Comparing `minium-1.5.3/minium/native/__init__.py` & `minium-1.5.4/minium/native/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-22
 import typing
+from typing import overload, Literal, Union
 
-from minium.framework.miniconfig import MiniConfig, logger
+from ..framework.miniconfig import MiniConfig, logger, IOSDesire, AndroidDesire
 from .exception import *
 
 # # weChat
 from minium.native.wx_native.basenative import BaseNative
 
 # from minium.native.wx_native.androidnative import WXAndroidNative
 # from minium.native.wx_native.iosnative import WXIOSNative
@@ -23,15 +24,15 @@
     from .qq_native.qandroidnative import QAndroidNative
     from .qq_native.qiosnative import QiOSNative
     NativeType = typing.Union[IdeNative, WXAndroidNative, WXIOSNative, QAndroidNative, QiOSNative]
 else:
     NativeType = BaseNative
 
 # platform
-from minium.utils.platforms import *
+from ..utils.platforms import *
 # OS_ANDROID = "android"
 # OS_IOS = "ios"
 # OS_IDE = "ide"
 # OS_MAC = "mac"
 # OS_WIN = "win"
 
 # application
@@ -96,11 +97,22 @@
     else:
         json_conf = {"outputs": conf.outputs, "debug": conf.debug or False}
         json_conf.update(conf.device_desire or {})
         app = APP[conf.app.lower() + "_" + os_name.lower()](json_conf)
     app.platform = os_name
     return app
 
-
-def Native(json_conf, platform=None, app="wx"):
-    cfg = MiniConfig({"platform": platform, "app": app, "device_desire": json_conf})
+@overload
+def Native(platform: str, app="wx") -> NativeType: ...
+@overload
+def Native(json_conf: Union[AndroidDesire, IOSDesire], platform: str=None, app="wx") -> NativeType: ...
+
+def Native(json_conf: Union[AndroidDesire, IOSDesire], platform: str=None, app="wx") -> NativeType:
+    if json_conf in PLATFORMS:
+        if platform:
+            app = platform
+        platform = json_conf
+        json_conf = {}
+        cfg = MiniConfig({"platform": platform, "app": app, "device_desire": json_conf})
+    else:
+        cfg = MiniConfig({"platform": platform, "app": app, "device_desire": json_conf})
     return get_native_driver(platform, cfg)
```

### Comparing `minium-1.5.3/minium/native/qq_native/qandroidnative.py` & `minium-1.5.4/minium/native/qq_native/qandroidnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/native/qq_native/qbasenative.py` & `minium-1.5.4/minium/native/qq_native/qbasenative.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/native/qq_native/qiosnative.py` & `minium-1.5.4/minium/native/qq_native/qiosnative.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/native/wx_native/androidnative.py` & `minium-1.5.4/minium/native/wx_native/androidnative.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,167 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-22
 from __future__ import annotations
 import os.path
 import time
 import typing
 
-from minium.utils.utils import timeout, wait
-from .basenative import BaseNative, NativeError, ModalStatus, NativeModal
+from ...utils.utils import timeout, wait
+from .basenative import BaseNative, NativeError, ModalStatus, NativeModal, NodeType, _SourceTree, etree, pyclasslookup
 import at
+import at.core.config
 from at.core.adbwrap import AdbWrap
 from at.core.element import Element as ATElement, AtSelector
 from at.webdriver import driver
+import at.core.uixml
 from at.core.uixml import UiView, Rect
+from at.utils import decorator
 import at.keycode
 import json
 import logging
 import threading
 import shutil
 import ssl
 import requests
 import functools
 import re
-from typing import Tuple, List, Dict
+from typing import Tuple, List, Dict, Union
+from typing_extensions import Self, Optional
 from ...externlib.android_base import UiDefine, ScreenType
 from .wording import Language, WORDING
 import xml.etree.ElementTree as ET
 
+at.core.uixml.parse_int = lambda i: 0 if i is None else int(i)
+def parse_bounds(bounds):
+    m = re.match(r"\[(\d+),(\d+)\]\[(\d+),(\d+)\]", bounds or "")
+    if m is None:
+        return 0, 0, 0, 0
+    return m.groups()
+at.core.uixml.parse_bounds = parse_bounds
+
 ssl._create_default_https_context = ssl._create_unverified_context
 
 WECHAT_PACKAGE = "com.tencent.mm"
 WECHAT_ACTIVITY = "ui.LauncherUI"
 MINIPROGRAM_ACTIVITY = "plugin.appbrand.ui.AppBrandUI"
 MINIPROGRAM_PLUGIN_ACTIVITY = "plugin.appbrand.ui.AppBrandPluginUI"
 
 
 logger = logging.getLogger("minium")
 _MIN_NORMALIZED_FRAME_LENGTH = 0.5
 
+if etree:
+    class MyElementClass(etree.ElementBase):
+        ui_view = None
+
+    class MyLookup(pyclasslookup.PythonElementClassLookup):
+        def lookup(self, doc, root):
+            if root.tag in ["node", "hierarchy"]:
+                return MyElementClass
+            # delegate to default
+            return None
+
+else:
+    class MyElementClass(object): ...
+    class MyLookup(object): ...
+
+
+class UiViewNode(UiView, NodeType):
+    _node: "etree._Element"
+    def __new__(cls, source: Union[str, UiViewNode, "etree._Element"], *args, **kwargs) -> Self:
+        if isinstance(source, UiViewNode):
+            return source
+        return object.__new__(cls)
+
+    def __init__(self, source: Union[str, UiViewNode, "etree._Element", SourceTree], resgurad=None):
+        if isinstance(source, UiViewNode):
+            # copy
+            return
+        if isinstance(source, str):
+            node = SourceTree(source).tree
+        elif isinstance(source, SourceTree):
+            node = source.tree
+        elif isinstance(source, etree._Element):
+            node = source
+        else:
+            raise ValueError("Invalid type %s passed into UiViewNode." % (type(source)))
+        super().__init__(node, resgurad)
+        if isinstance(source, str):
+            self._xml = source
+        else:
+            self._xml = None
+
+    @classmethod
+    def parse(cls, el: etree._Element):
+        return UiViewNode(el)
+
+    @property
+    def simple_text(self) -> str:
+        return str(self)
+    
+    @property
+    def xml(self) -> str:
+        if self._xml is not None:
+            return self._xml
+        e = etree.Element(self._node.tag, self._node.attrib)
+        return etree.tounicode(e, pretty_print=True)
+        
+    def get_children(self) -> List[UiViewNode]:
+        childrens: List[etree._Element] =  self._node.getchildren()
+        return [UiViewNode(child, self.rg) for child in childrens]
+
+    @property
+    def parent(self):
+        parent_node: "etree._Element" = self._node.getparent()
+        try:
+            if hasattr(parent_node, "ui_view"):
+                return parent_node.ui_view
+            return UiViewNode(parent_node, self.rg)
+        except:
+            return None
+        
+    def is_leaf(self):
+        return not self.get_children()
+    
+    def unique_key(self):
+        return self.xml
+    
+    def g(self, attr, default_value=None):
+        try:
+            value = self._node.attrib[attr]
+        except:
+            return default_value
+        if isinstance(value, str):
+            value = value.strip()
+        return value
+
+def remove_kinda_window(source_tree: SourceTree) -> SourceTree:
+    """
+    支付界面XML有很多kinda_main_container，只保留最后一个，其他的删除
+    """
+    els: List["etree._Element"] = source_tree.tree.xpath("//*[@resource-id='com.tencent.mm:id/kinda_main_container']")
+    for el in els[0:-1]:  # 保留最后一个
+        parent: "etree._Element" = el.getparent()
+        parent.remove(el)
+    return source_tree
+
+class SourceTree(_SourceTree[UiViewNode]):
+    node_type = UiViewNode
+
+    @property
+    def tree(self):
+        if self._tree is None:
+            parser = etree.XMLParser()
+            setElementClassLookup = parser.setElementClassLookup if hasattr(parser, "setElementClassLookup") else parser.set_element_class_lookup
+            setElementClassLookup(MyLookup())
+            if isinstance(self._source, self.node_type):
+                self._tree = etree.XML(self._source.xml.encode("utf8"), parser)
+            else:
+                self._tree = etree.XML(self._source.encode("utf8"), parser)
+        return self._tree
 
 def auto_reconnect(func):
     @functools.wraps(func)
     def wrapper(self: WXAndroidNative, *args, **kwargs):
         try:
             ret = func(self, *args, **kwargs)
         except (requests.ConnectionError, requests.ReadTimeout) as e:
@@ -81,40 +202,53 @@
 
     GET_CURRENT_ACTIVITY_CMD = [
         'dumpsys activity activities | grep -E "mFocusedActivity|mResumedActivity"',
         'dumpsys activity activities | grep -E "mCurrentFocus|mFocusedApp"',
         'dumpsys window | grep -E "mCurrentFocus|mFocusedApp"',
     ]
     GET_CURRENT_ACTIVITY_CMD_IDX = 0
+
+    GET_CURRENT_DISPLAY_CMD = [
+        ('dumpsys display | grep mDisplayId', 'mDisplayId'),
+    ]
+
+    # 解绑了银行卡 + 零钱不足
+    PAYMENT_RETURN_XPATH = '//node[@content-desc="添加新银行卡" and @class="android.widget.Button"]//preceding::node[contains(@content-desc, "零钱不足")]//preceding::node[@text="选择付款方式"]//preceding-sibling::node[@content-desc="返回" and @clickable="true"]'
     
+    # 用户隐私
+    PRIVACY_ALLOW_XPATH = '//node[contains(@text, "用户隐私")]//preceding::node[@text="拒绝"]//following::node[@text="同意"]'
+    PRIVACY_DENY_XPATH = '//node[contains(@text, "用户隐私")]//preceding::node[@text="同意"]//preceding::node[@text="拒绝"]'
     def __init__(self, json_conf):
         super(WXAndroidNative, self).__init__(json_conf)
         if json_conf is None:
             json_conf = {}
         self.serial = json_conf.get("serial") or AdbWrap.get_default_serial()
         self.uiautomator_version = int(json_conf.get("uiautomator_version", "2"))
         at.uiautomator_version = self.uiautomator_version
         self.at = at.At(self.serial)
         self.at.java_driver.set_capture_op(False)
         self.ui = UiDefine(self.at)
         self.screen_size = self.at.device.device_size()
         self.lang = json_conf.get("lang")
+        self._full_tree = None
+        self._source_tree = None
         self.perf_thread = None
         self.perf_flag = False
         self.ef_able_flag = False
         self.fps_data_dict = {}  # fps dict
         self.jank_count_dict = {}  # 卡顿次数
         self.fps_thread = None
         self.startup_time = 0
         self.outputs = json_conf.get("outputs") or os.path.dirname(
             os.path.realpath(__file__)
         )
         self.debug = json_conf.get("debug", False)
         self.outputs_screen = os.path.join(self.outputs, "image")
         self.screen_type = ScreenType.AT  # 截图方式，默认使用at
+        self._screen_fail_cnt = 0  # 连续截图失败次数, 超过3次则切换
         self._empty_base_screen_dir(self.outputs_screen)
         self._current_views = None
         self._app_brand_action_bar_bottom = None
         # 1. 原始版本, 使用计算数字坐标的方式进行点击.
         # 2. 数字按钮具有固定的rid, 格式为: `com.tencent.mm:id/tenpay_keyboard_{number}`
         self.pay_modal_version = 0
         # 弹窗的层级有不同
@@ -179,18 +313,36 @@
         self._last_modal_type = None
 
     @property
     def current_views(self):
         if self._current_views is None:
             return self._get_current_views()
         return self._current_views
+    
+    def source(self):
+        res = self.at.java_driver.request_at_device("dumpUi", [])
+        for _ in range(3):
+            res = self.at.java_driver.request_at_device("dumpUi", [])
+            if res and len(res.strip()) != 0:
+                full_tree = SourceTree(res)
+                if not full_tree.xpath("/hierarchy/node"):
+                    self.at.java_driver.reconnect()
+                    continue
+                self._full_tree = full_tree
+                self._source_tree = remove_kinda_window(SourceTree(res))
+                return self._source_tree
+            self.at.java_driver.reconnect()
 
     @timeout(2, 0.5)
     def _get_current_views(self):
         self._current_views = self.at.java_driver.dump_all_views()
+        if not self._current_views:
+            logger.warning("当前页面没有任何控件, 重连后重试")
+            self.at.java_driver.reconnect()
+            self._current_views = self.at.java_driver.dump_all_views()
         return self._current_views
 
     def _get_view_from_current_view(self, el: ATElement):
         if not self.current_views:
             return None
         instance = el._selector.get(AtSelector.SELECTOR_INSTANCE, 0)
         for ui_view_list in self.current_views:
@@ -212,15 +364,18 @@
             if el.match_ui_view(view):
                 return True
         return False
 
     def _empty_base_screen_dir(self, dirname):
         if os.path.exists(dirname):
             if os.path.isdir(dirname):
-                shutil.rmtree(dirname)
+                try:
+                    shutil.rmtree(dirname)
+                except OSError:  # 不知道为什么not empty也会报错。。。
+                    pass
                 time.sleep(1)
             else:
                 os.remove(dirname)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
 
     def _deal_log(self, log):
@@ -275,39 +430,68 @@
             self.e.text(gallery_name).click()
             self.e.desc_contains("图片 1").click()
             self.e.text_contains("扫描中").wait_disappear()
 
     def screen_shot(self, filename, quality=30):
         return self._screen_shot(filename, quality)
 
-    def _screen_shot(self, filename, quality=30):
+    def _screen_shot(self, filename, quality=30, screen_type=None):
         """
         安卓截图有两种方式：
         1. via at
         2. via adb screencap
         via at现存问题: 可能因为网络、at进程被kill等问题, 截图时间超长
+
+        :return: filename / ""
         """
-        if self.screen_type == ScreenType.AT:
+        screen_type = screen_type or self.screen_type
+        if screen_type == ScreenType.AT:
             stime = time.time()
             try:
                 ret = self.at.device.screen_shot(filename, quality=quality)
             except (requests.ConnectionError, requests.ReadTimeout) as e:
                 logger.error("screen_shot error %s, try reconnect" % str(e))
                 self.at.java_driver.reconnect()
                 stime = time.time()
                 ret = self.at.device.screen_shot(filename, quality=quality)
             # ret = self.at.device.screen_shot(filename, quality=quality)
             if time.time() - stime > 50:  # 如果一次截图超过50s, 就切换截图类型
                 logger.warning(
                     "screen_shot cost bigger than 50s, change the screen type"
                 )
                 self.screen_type = ScreenType.ADB
-            return ret
-        elif self.screen_type == ScreenType.ADB:
-            return self.at.device.screen_shot(filename, quality=quality, display_id=0)
+            size = 0
+            if os.path.isfile(filename):
+                size = os.path.getsize(filename)
+                if size != 0:# 截图成功
+                    self._screen_fail_cnt = 0
+                    return filename
+            # 截图失败了
+            logger.warning(f"screen_shot {filename} exists: {os.path.isfile(filename)}, size: {size}")
+            self._screen_fail_cnt += 1
+            if self._screen_fail_cnt >= 3:
+                logger.warning(
+                    f"screen_shot fail {self._screen_fail_cnt} times, change the screen type"
+                )
+                self.screen_type = ScreenType.ADB
+            # 换一种方式试试
+            return self._screen_shot(filename, quality=quality, screen_type=ScreenType.ADB)
+        elif screen_type == ScreenType.ADB:
+            try:
+                return self.at.adb.screen(filename, display_id=self.display_id)
+            except TypeError:
+                logger.warning(
+                    "screen_shot via adb fail, response data empty"
+                )
+                # TypeError: replace() argument 1 must be str, not bytes
+                # 新版本at库, 部分机型截图返回空, 触发的bug, 本地修复无用, 从这里做兼容
+                # with open(filename, "w") as fd:
+                #     fd.write("")
+                # return filename
+                return ""
 
     def pick_media_file(
         self,
         cap_type="camera",
         media_type="photo",
         original=False,
         duration=5.0,
@@ -525,14 +709,19 @@
         elif modal_type is NativeModal.SUBSCRIBE:
             return self.allow_send_subscribe_message(answer)
         elif modal_type is NativeModal.OPENWERUN:
             return self.allow_get_we_run_data(answer)
         return False
     
     def allow_privacy(self, answer=True):
+        source = self.source()
+        view = source.xpath(WXAndroidNative.PRIVACY_ALLOW_XPATH if answer else WXAndroidNative.PRIVACY_DENY_XPATH)
+        if not view:
+            return False
+        return self.click_view(view[0])
         return self.e.text("同意" if answer else "拒绝").click_if_exists(0.5)
 
     def allow_authorize(self, answer=True):
         modal_type = self._check_auth_type(answer, 4)
         self._last_modal_type = modal_type  # 记录下即将处理的类型
         ret = self._handle_auth(modal_type, answer)
         if modal_type is NativeModal.PRIVACY and ret is True:  # 如果是【隐私弹窗】并处理成功, 则后面可能会再弹窗另外的授权弹窗
@@ -619,48 +808,59 @@
             if not self.e.text_matches("微信绑定号码|上次提供").click_if_exists(0.5):
                 return self._allow_authorize(answer)  # 兼容就逻辑
             return True
         return False
 
     def allow_send_subscribe_message(self, answer=True):
         """
-        允许发送订阅消息
+        允许/确定发送订阅消息
         """
         if answer:
 
+            def get_switch():
+                # android.widget.Switch / android.view.View
+                for ee in (
+                    (
+                        self.e.cls_name("android.view.View")
+                        .enabled(True)
+                        .clickable(True)
+                        .desc("")
+                    ),
+                    (
+                        self.e.cls_name("android.widget.Switch")
+                        .enabled(True)
+                        .desc("")
+                    )
+                ):
+                    views = ee.get_ui_views()
+                    if views:
+                        for v in reversed(views):  # 倒序遍历
+                            if v.rid:
+                                return ee, [v]
+                return ee, views
+
             def do():
                 e = (
                     self.e.cls_name("android.widget.Button")
                     .focusable(True)
                     .text_matches("允许|确定")
                 )
                 view = e.get_view(timeout=3)
                 if view and not view.enabled:  # 不能点击, 先enable一个通知
-                    ee = (
-                        self.e.cls_name("android.view.View")
-                        .enabled(True)
-                        .clickable(True)
-                        .desc("")
-                    )
-                    views = ee.get_ui_views()
+                    ee, views = get_switch()
                     if not views:
                         logger.warning("可能不存在可选择的模板消息")
                         return False
-                    if len(views) == 1:
-                        if not views[0].rid:
-                            logger.warning("可能不存在可选择的模板消息, 尝试选择")
-                        ee.click_if_exists(0.5)
+                    for v in reversed(views):  # 倒序遍历
+                        if v.rid:  # 有id的
+                            ee.rid(v.rid).click_if_exists(0.5)
+                            break
                     else:
-                        for v in reversed(views):  # 倒序遍历
-                            if v.rid:  # 有id的
-                                ee.rid(v.rid).click_if_exists(0.5)
-                                break
-                        else:
-                            logger.warning("可能不存在可选择的模板消息, 尝试选择")
-                            ee.click_if_exists(0.5)
+                        logger.warning("可能不存在可选择的模板消息, 尝试选择")
+                        ee.click_if_exists(0.5)
                 elif not view:
                     return False
                 return e.enabled(True).click_if_exists(1.5)
 
             try:
                 ret = do()
             except (requests.ConnectionError, requests.ReadTimeout) as e:
@@ -722,14 +922,15 @@
         return self.e.text_matches("创建(新的)?聊天").click_if_exists(timeout)
 
     def forward_miniprogram_inside(self, name, text=None, create_new_chat=True):
         if create_new_chat and self._create_new_chat():
             self.e.edit_text().enter(name)
             time.sleep(1)
             self.e.text_contains(name).click(True)
+            time.sleep(1)
             if self.e.text("确定(1)").exists():
                 self.e.text("确定(1)").enabled(True).click()
             else:
                 self.e.text("完成(1)").enabled(True).click()
         else:
             self.e.text("搜索").click()
             time.sleep(1)
@@ -804,16 +1005,18 @@
         ).click()
         if not enable:
             self.e.cls_name("android.widget.Button").text("关闭授权").click_if_exists(5)
 
     def release(self):
         super().release()
         if self.perf_flag:
+            logger.info("stop_get_perf")
             self.stop_get_perf()
         self.at.release()
+        self.at.adb.stop_app(at.core.config.TEST_APP_PKG)  # 把 weautomator也kill一下
         self._empty_base_screen_dir(self.outputs_screen)  # 清空截图目录
 
     def start_wechat(self):
         if self.at.adb.app_is_running(WECHAT_PACKAGE):
             if self.debug:
                 return
             self.at.adb.stop_app(WECHAT_PACKAGE)  # 先关掉
@@ -903,20 +1106,20 @@
                 used = int(m2.group(1)) / 1024
 
             # elif m1:
             #     logger.info("m1 is %s" % m1)
             #     used = int(m1) / 1024
         if used == 0:
             try:
-                used = self.get_mem_used_new_doudi(output_mem, pkg_name, pid)
+                used = self._get_mem_used_new_doudi(output_mem, pkg_name, pid)
             except Exception as e:
                 logger.error(e)
         return str(used)
 
-    def get_mem_used_new_doudi(self, output_mem, processname, pid):
+    def _get_mem_used_new_doudi(self, output_mem, processname, pid):
         used = 0
         if output_mem.find("Total PSS by process"):
             ls = re.split(r"[\r\n]+", output_mem)
             tag = processname + " (pid " + str(pid) + " / activities)"
             for line in ls:
                 if line.find(tag) > -1:
                     used_str = line.split("K: ")[0]
@@ -1083,25 +1286,48 @@
             except Exception:
                 self.perf_flag = False
                 return self.perf_flag
         else:
             self.perf_flag = False
             return self.perf_flag
 
-    def start_get_perf(self, timeinterval=15):
+    def start_get_perf(self, timeinterval=15) -> bool:
         if self.perf_flag:  # 一个线程就够了
             return True
         self.perf_thread = threading.Thread(
             target=self._start_get_perf,
             args=(timeinterval,),
+            name="GetPerformance",
+            daemon=True
         )
-        self.perf_thread.daemon = True
         self.perf_thread.start()
         return True
 
+    def start_get_start_up(self):
+        """
+        开始监听启动时间
+        """
+        self.logcat.start_record("get instanceid", "report 19175", "J2V8_Console")
+
+    def stop_get_start_up(self):
+        """
+        结束监听启动时间
+        :return: number
+        """
+        instanceid_log = self.logcat.get_lines("get instanceid")
+        # logger.debug(instanceid_log)
+        self.logcat.stop_record("get instanceid")
+        if instanceid_log:
+            self._deal_log(instanceid_log)
+            logger.info("start up: %s" % self.startup_time)
+        return self.startup_time
+
+    def get_start_up(self):
+        return self.startup_time
+
     def stop_get_perf(self):
         self.perf_flag = False
         if self.perf_thread:
             self.perf_thread.join()
         if self.perf_data:
             perf_data_str = json.dumps(self.perf_data)
             self.perf_data = []
@@ -1155,32 +1381,44 @@
 
         if self.e.text("支付成功").exists(10):
             self.e.text("完成").click(is_scroll=True)
         else:
             raise TypeError("支付失败")
 
     def close_payment_dialog(self):
+        if not self._is_in_payment():
+            logger.info("current views: %s", self._current_views)
+            logger.error("支付框不存在")
+            return True
+        if self._source_tree:
+            button = self._source_tree.xpath(WXAndroidNative.PAYMENT_RETURN_XPATH)
+            if button:
+                logger.info("找到零钱不足提示弹窗: %s", button[0])
+                self.click_view(button[0])
+                return
         if self.e.text_contains("￥").exists(10):
             if not self.e.desc("关闭").click_if_exists():
                 # 找不到关闭按钮试下直接返回
                 self._press_back()
+                return True
         else:
             if self.e.text_contains("支付方式").exists():
                 self.at.adb.press_back()  # 有可能找不到输入框，先后退尝试
                 return True
             logger.error("支付框不存在")
         return False
 
     def text_exists(self, text="", iscontain=False, wait_seconds=5):
+        logger.debug(f'check ui {"contain" if iscontain else "exists"} "{text}"')
         if iscontain:
-            return self.e.text_contains(text=text).exists(wait_seconds)
+            return self.e.text_contains(text).exists(wait_seconds)
         else:
-            return self.e.text(text=text).exists(wait_seconds)
+            return self.e.text(text).exists(wait_seconds)
 
-    def _is_visible(self, view: UiView) -> Rect or None:
+    def _is_visible(self, view: UiView) -> Optional[Rect]:
         """检查view是否可见
 
         :param UiView view: view
         :return Rect or None:
 
         判断两个矩形是否相交即可
         在x轴方向:A.center_x和B.center_x的距离一定小于或等于矩形A的宽度+矩形B的宽度的一半
@@ -1267,15 +1505,15 @@
         )
 
     def _is_in_target_miniprogram(self, appid: str):
         if not appid:
             return True
         appids = []
         for i in self.at.java_driver.dump_ui():
-            match = re.match("^(wx\w+):\w+$", i.content_desc)
+            match = re.match("^(wx\w+):.*$", i.content_desc)
             if match:
                 appids.append(match.group(1))
         return appids[-1] == appid if len(appids) > 0 else False
 
     def _close_miniprogram(self):
         return self._press_back()
 
@@ -1388,14 +1626,32 @@
             if modal.click_if_exists(0):
                 if not rid:
                     return ModalStatus.NotOfficialModal
                 return ModalStatus.OK
             return ModalStatus.Error
         return ModalStatus.Error
 
+    @decorator.cached_property
+    def display_id(self):
+        for cmd, kw in WXAndroidNative.GET_CURRENT_DISPLAY_CMD:
+            output = self.at.adb.run_adb(
+                [
+                    "shell",
+                    cmd,
+                ]
+            )
+            logger.debug(output)
+            for line in output.split("\n"):
+                line = line.strip()
+                m = re.search(r"%s=(\d+)" % kw, line)
+                if m:
+                    logger.info(f"current display id is {m.group(1)}")
+                    return int(m.group(1))
+        return 0
+
     def _get_current_activity(self):
         for i in range(len(WXAndroidNative.GET_CURRENT_ACTIVITY_CMD)):
             idx = (i + WXAndroidNative.GET_CURRENT_ACTIVITY_CMD_IDX) % len(WXAndroidNative.GET_CURRENT_ACTIVITY_CMD)
             WXAndroidNative.GET_CURRENT_ACTIVITY_CMD_IDX = idx  # 更新一下, 下次从这个开始检查
             cmd = WXAndroidNative.GET_CURRENT_ACTIVITY_CMD[idx]
             output = self.at.adb.run_adb(
                 [
@@ -1409,17 +1665,31 @@
                 m = re.search(r"((\w+?\.)+?(\w+)/(\.\w+)+)", line)
                 if m:
                     logger.info(f"current activity is {m.group(0)}")
                     return m.group(0)
         return ""
 
     def _is_in_payment(self):
-        return self.e.text_contains("￥").exists(0.5) or self.e.text_contains(
-            "支付方式"
-        ).exists(0.5)
+        source = self.source()
+        if source:
+            # 解绑了银行卡 + 零钱不足
+            button = source.xpath(WXAndroidNative.PAYMENT_RETURN_XPATH)
+            if button:
+                return True
+        try:
+            if self.pay_modal_version == 2:
+                self._get_current_views()
+                return self._el_exist_in_current_view(self.e.rid("com.tencent.mm:id/tenpay_keyboard_0"))
+            elif self.pay_modal_version == 1:
+                self._get_current_views()
+                return self._el_exist_in_current_view(self.e.text_contains("请输入支付密码")) and self._el_exist_in_current_view(self.e.text_contains("￥"))
+            self._check_pay_modal_version() 
+        except TypeError:
+            return False
+        return True
 
     def _get_number_point(self, number):
         """
         获取数字的中心坐标
         :param number:
         :return:
         """
@@ -1502,31 +1772,63 @@
             # raise Exception("No valid frames lengths found.")
             return 0
         return int(round((frame_count - 1) / seconds))
 
     @property
     def e(self):
         return self.at.e
+    
+    def click_view(self, view: Union[UiView, List[UiView]]):
+        if not view:
+            return False
+        input_interceptor = self.at.input_interceptor
+        if isinstance(view, UiView):
+            view = [view]
+        for v in view:
+            if input_interceptor:
+                input_interceptor.click(v.center_x, v.center_y)
+                continue
+            self.at.device.click_on_ui_view(v)
+        return True
+    
+    def log_all_nodes(self, nodes=None):
+        views_list = nodes or self._get_current_views()
+        logger.info("\n".join([str(node) for view in views_list for node in view ]))
 
     # 云环境上莫名其妙卡死在这里了。。。
     @wait(60, False)
     def check_connection(self, *args):
         # 检查atsub链接
         if self.at.java_driver.ping():
             return True
         # reconnect
         try:
             self.at.java_driver.close_remote()
+            self.at.adb.stop_app(at.core.config.TEST_APP_PKG)
             time.sleep(1)
             self.at.java_driver._init(True)
         except Exception as e:
             logger.exception(e)
             return False
         return self.at.java_driver.is_remote_running()
 
+    def check_connected(self):
+        """检查是否存在【连接断开】的情况，有则手动断开一下"""
+        s = self.source()
+        view = s.xpath('//node[@text="连接断开"]//following::node[@text="展开"]')
+        if not view:
+            return True
+        self.click_view(view)
+        time.sleep(1)
+        s = self.source()
+        if self.click_view(s.xpath('//node[@text="收起"]//preceding-sibling::node[@text="结束"]')):
+            time.sleep(2)
+            self.close_local_debug_modal()
+        return False
+
     def close_local_debug_modal(self):
         self.handle_modal(
             btn_text=WORDING.COMMON.MODAL_CONFIRM.value,
             title=WORDING.COMMON.LOCAL_DEBUG_MODAL_TITLE.value,
             force_title=True,
         ) or self.handle_modal(
             btn_text=WORDING.COMMON.MODAL_CONFIRM.value,
@@ -1561,15 +1863,16 @@
     
     @property
     def status_bar_height(self):
         if self._status_bar_height is None:
             try:
                 self._status_bar_height = self.at.device.status_bar_height()
             except:
-                return 0
+                logger.warning("get device status_bar_height fail, try use miniprogram api")
+                self.mini and self.mini.app.pixel_ratio
         return self._status_bar_height or 0
     
     # for h5
     def _mph5_visible(self, h5_url: str):
         """当前可见的小程序页面是h5页面
 
         :param str h5_url: 预期的h5链接
```

### Comparing `minium-1.5.3/minium/native/wx_native/basenative.py` & `minium-1.5.4/minium/native/wx_native/basenative.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 #!/usr/bin/env python3
 # Created by xiazeng on 2019-05-22
 
+import abc
 import logging
 import time
 import os
 import shutil
 import json
 import threading
 import types
 import typing
 from functools import wraps
 from enum import Enum, auto
 
 from ..exception import *
 from ...utils.emitter import ee
+from ...utils.lazyloader import check_package
 from .wording import Language, WORDING
+from typing import Union, Generic, TypeVar, List, cast, Type
 if typing.TYPE_CHECKING:
     import minium
+    from lxml import etree
+    from lxml import pyclasslookup
+else:
+    lxml = check_package("lxml")
+    if lxml is not None:
+        from lxml import etree
+        from lxml import pyclasslookup
+    else:
+        etree = None
+        pyclasslookup = None
 
 logger = logging.getLogger("minium")
 
 def mock_allow_privacy(allow_privacy):
     @wraps(allow_privacy)
     def wrapper(self: 'BaseNative', answer=True, *args, **kwargs):
         privacy_ret = allow_privacy(self, answer, *args, **kwargs)
@@ -43,20 +56,93 @@
 def call_funtion_log(func, name: str):
     @wraps(func)
     def wrapper(*args, **kwargs):
         logger.info(f"call {name}")
         result = func(*args, **kwargs)
         if name.find(".handle") > 0 or name.find(".allow") > 0:
             logger.info(f"{name} return {str(result)}")
-        logger.info(f"call {name} end")
+        logger.info(f"call {name} end {result if isinstance(result, bool) or result is None else ''}")
         return result
 
     return wrapper
 
 
+T = TypeVar("T", bound="NodeType")
+class NodeType(metaclass=abc.ABCMeta):
+    @classmethod
+    @abc.abstractmethod
+    def parse(cls, el: etree._Element) -> T: ...
+
+    @property
+    @abc.abstractmethod
+    def simple_text(self) -> str: ...
+    
+    @property
+    @abc.abstractmethod
+    def xml(self) -> str: ...
+
+    @abc.abstractmethod
+    def get_children(self) -> List[T]: ...
+
+
+def extend_node(source: T) -> List[T]:
+    # 递归展开
+    nodes = [source]
+    if not source.get_children():
+        return nodes
+    for node in source.get_children():
+        nodes.extend(extend_node(node))
+    return nodes
+
+def trans_tree_to_nodes(el: etree._Element, node_type: Type[T]) -> typing.List[T]:
+    if el.get("visible", 'false') == 'false' and not el.getchildren():
+        # filter not visible
+        return []
+    node = node_type.parse(el)
+    nodes = [node]
+    for child in (el.getchildren() or []):
+        nodes.extend(trans_tree_to_nodes(child, node_type))
+    return nodes
+
+class _SourceTree(Generic[T]):
+    node_type: Type[T] = NodeType
+    def __init__(self, source: Union[str, T]) -> None:
+        """实例化源代码树
+
+        :param str or T source: xml str or T
+        """
+        self._source = source
+        self._tree: etree._Element = None
+        self._nodes: typing.List[T] = None
+        
+
+    @property
+    def tree(self):
+        if self._tree is None:
+            if isinstance(self._source, self.node_type):
+                self._tree = etree.XML(self._source.xml.encode("utf8"), etree.XMLParser())
+            else:
+                self._tree = etree.XML(self._source.encode("utf8"), etree.XMLParser())
+        return self._tree
+
+    @property
+    def nodes(self):
+        if self._nodes is None:
+            if isinstance(self._source, self.node_type):
+                self._nodes = extend_node(self._source)
+            else:
+                self._nodes = trans_tree_to_nodes(self.tree, self.node_type)
+        return self._nodes
+
+    def xpath(self, xp: str) -> typing.List[T]:
+        els = self.tree.xpath(xp)
+        if not els:
+            return []
+        return [self.node_type.parse(el) for el in els]
+
 class NativeModal(Enum):
     """穷举有可能出现的原生弹窗"""
     NONE = auto()           # 没有弹窗
     NORMAL = auto()         # 通用
     LOGIN = auto()          # 登录
     RECORD = auto()         # 录音
     CAMERA = auto()         # 相机
@@ -77,15 +163,18 @@
     IMAGEPREVIEW = auto()   # 图片预览
     ALERT = auto()          # 系统弹窗
 
 
 class NativeMetaClass(type):
     def __new__(mcs, cls_name, bases, attr_dict: typing.Dict[str, typing.Any]):
         for k, v in attr_dict.items():
-            if isinstance(v, types.FunctionType) and not k.startswith("_"):
+            if isinstance(v, types.FunctionType) and not (
+                k.startswith("_") or
+                k == "screen_shot"
+            ):
                 if k == "allow_privacy":
                     attr_dict[k] = call_funtion_log(mock_allow_privacy(v), f"{cls_name}.{k}")
                 elif k.startswith("allow_") and k not in ("allow_authorize", "allow_send_subscribe_message"):  # `allow_authorize`自己处理`allow_privacy`
                     attr_dict[k] = call_funtion_log(hook_allow_method(v), f"{cls_name}.{k}")
                 else:
                     attr_dict[k] = call_funtion_log(v, f"{cls_name}.{k}")
         return type.__new__(mcs, cls_name, bases, attr_dict)
@@ -542,14 +631,21 @@
     def check_connection(self, *args):
         """
         检查真机调试通道是否还存在, 如果断连则重连
         :return: bool
         """
         return True
     
+    def check_connected(self, *args):
+        """检查真机调试通道建立过程是否出现"断开连接"提示
+
+        :return bool: true for 成功连接
+        """
+        return True
+    
     def get_websocket_debugger_url(self, *args):
         """获取chrome debugger websocket url
 
         :return str: debugger url
         """ 
         return ""
 
@@ -753,15 +849,16 @@
         :params answer: True: 自动同意, False: 自动拒绝
         :return: bool
         """
         self._auto_answer = answer
         if self.__auto_authorize_thread:
             return True
         self.__auto_authorize_thread = threading.Thread(
-            target=self.__op_auto_authorize
+            target=self.__op_auto_authorize,
+            name="AutoAuthorize",
         )
         self.__auto_authorize_thread.setDaemon(True)
         self.__auto_authorize_thread.start()
         ee.on("notify", self.notify)  # 监听相应函数
         return True
 
     def release_auto_authorize(self):
@@ -804,20 +901,27 @@
 
     def _auto_authorize_callback(self, answer=True):
         """
         处理authorize的逻辑, 可重载
         """
         ret = True
         cnt = 10  # 最大处理10个授权窗口，防止死循环(检测到有元素 & 可以click，但实际点不动)
-        while ret and cnt > 0:
+        handle_any = False
+        etime = time.time() + 3  # 如果从未检测到并处理过弹窗(handle_any == False), 则需要多检测几次，直到超过etime, 原因是这种情况可能是因为弹窗引起
+        while (ret and cnt > 0) or (not handle_any and etime > time.time()):
+            """
+            1. ret and cnt > 0: 处理弹窗成功, 且没有超过尝试次数, 可能仍然存在其他弹窗, 继续检测
+            2. not handle_any and etime > time.time(): 没有成功处理过弹窗(可能根本没有出现), 且没有到检测超时时间
+            """
             cnt -= 1
             try:
                 ret = self.allow_authorize(answer)
                 self._last_allow_ret = ret
                 if ret:
+                    handle_any = True  # 处理过
                     self._last_allow_time = time.time()
             except NotImplementedError:
                 #  未实现的处理方法，直接break进程
                 return False
             time.sleep(1)
         return cnt > 0
 
@@ -830,15 +934,15 @@
                 os.remove(dirname)
         if not os.path.exists(dirname):
             os.makedirs(dirname)
 
     def __notify(self):
         self.__auto_auth_lock.acquire()
         self.__auto_auth_lock.notify_all()
-        self.__last_notify_time = time.time() + 6  # 收到通知后6秒内还应该继续检测, 一般弹窗有滞后性
+        self.__last_notify_time = time.time() + 8  # 收到通知后6秒内还应该继续检测, 一般弹窗有滞后性
         self.__auto_auth_lock.release()
 
     def __op_auto_authorize(self):
         self.__auto_auth_flag = True
         while self.__auto_auth_flag:
             self.__auto_auth_lock.acquire()
             ret = self.__auto_auth_lock.wait(timeout=5)
```

### Comparing `minium-1.5.3/minium/native/wx_native/iosnative.py` & `minium-1.5.4/minium/native/wx_native/iosnative.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,58 +2,57 @@
 # Created by xiazeng on 2019-05-22
 import json
 import logging
 import threading
 import platform
 import typing
 from types import FunctionType
-from typing import Tuple
-from .basenative import BaseNative, NativeModal, ModalStatus
+from typing import Tuple, Union, List
+from .basenative import BaseNative, NativeModal, ModalStatus, NodeType, _SourceTree, etree
 from ...externlib.wx_wda import *
+import wda
 from .wording import WORDING, Language
-from minium.utils import Object, lazy_import, cost_debug
+from ...utils import Object, lazy_import, cost_debug, check_package, do_shell, wait, Version, WaitThread
+import re
+from enum import Enum
 
 canUseTidevice = {}
 if typing.TYPE_CHECKING:
     import tidevice
-    from lxml import etree
 else:
     tidevice = lazy_import("tidevice")
-    lxml = lazy_import("lxml")
-    if lxml is not None:
-        from lxml import etree
-    else:
-        etree = None
-    if tidevice is None or lxml is None:
-        raise ImportError('进行IOS测试需要安装额外依赖库, 请使用以下指令安装: `pip3 install "minium[ios]"`')
+    if tidevice is None:
+        logger.warning('进行IOS测试可能还需要安装额外依赖库, 请使用以下指令安装: `pip3 install "minium[ios]"`')
 OTHER_PACKAGE = "com.others.app"
 WECHAT_PACKAGE = "com.tencent.xin"
 WECHAT_ACTIVITY = "MainFrameViewController"
 MINIPROGRAM_ACTIVITY = "WAWebViewController"
 OTHER_ACTIVITY = "OtherActivity"
 WEBVIEW_ACTIVITY = "WAHTMLWebViewController"
 PHOTO_PREVIEW_ACTIVITY = "PhotoViewController"
 
+
 logger = logging.getLogger("minium")
 if "Windows" in platform.platform():
     isWindows = True
 else:
     isWindows = False
 
-class WDANode(dict):
+class WDANode(dict, NodeType):
     isEnabled = False
     isVisible = False
     isAccessible = False
     frame = ""
     rect = {}
     value = None
     label = ""
     type = ""
     name = ""
     rawIdentifier = None
+    rid = ""  # 8.0.43新加
     children = []
 
     def __init__(self, __map=None, **kwargs):
         if __map:
             kwargs.update(__map)
         extend = {}
         for k, v in kwargs.items():
@@ -136,36 +135,36 @@
         return cls(
             isEnabled = "1" if el.get("enabled") == 'true' else "0",
             isVisible = "1" if el.get("visible") == 'true' else "0",
             isAccessible = "1" if el.get("accessible") == 'true' else "0",
             frame = "{{%d, %d}, {%d, %d}}" % (rect["x"], rect["y"], rect["width"], rect["height"]),
             rect = rect,
             value = el.get("value", None),
-            label = el.get("value", ""),
-            type = el.get("type", ""),
+            label = el.get("label", ""),
+            type = el.get("type") or el.tag or "",
             name = el.get("name", ""),
             rawIdentifier = None,
         )
 
-def extend_node(source: WDANode):
-    # 递归展开
-    nodes = [source]
-    if not source.children:
-        return nodes
-    for node in source.get_children():
-        nodes.extend(extend_node(node))
-    return nodes
-    i = 0
-    while i < len(nodes):
-        node = nodes[i]
-        i += 1
-        if not node.children:
-            continue
-        nodes.extend(node.get_children())
-    return nodes
+# def extend_node(source: WDANode):
+#     # 递归展开
+#     nodes = [source]
+#     if not source.children:
+#         return nodes
+#     for node in source.get_children():
+#         nodes.extend(extend_node(node))
+#     return nodes
+#     i = 0
+#     while i < len(nodes):
+#         node = nodes[i]
+#         i += 1
+#         if not node.children:
+#             continue
+#         nodes.extend(node.get_children())
+#     return nodes
 
 def remove_invisible_child(source_data: WDANode, new_node=True):
     children_data = source_data.get('children', [])
     new_children = []
     if children_data:
         for child in children_data:
             new_child_data = remove_invisible_child(child, new_node)
@@ -181,24 +180,14 @@
         new_data = WDANode(source_data)  # copy, 防止把children改变, 影响source tree
         new_data.children = new_children
     else:
         new_data = source_data
         new_data.children = new_children
     return new_data
 
-def trans_tree_to_nodes(el: etree._Element) -> typing.List[WDANode]:
-    if el.get("visible", 'false') == 'false' and not el.getchildren():
-        # filter not visible
-        return []
-    node = WDANode.parse(el)
-    nodes = [node]
-    for child in (el.getchildren() or []):
-        nodes.extend(trans_tree_to_nodes(child))
-    return nodes
-
 class Selector(Object):
     """记录元素选择条件"""
     class_name = None
     text = None
     partial_text = None
     pattern = None
     xpath = None
@@ -229,87 +218,181 @@
             return False
         if self.partial_text and text.find(self.partial_text) < 0:
             return False
         if self.pattern and not re.search(self.pattern, text):
             return False
         return True
 
-class SourceTree(object):
-    def __init__(self, source: str or WDANode) -> None:
-        """实例化源代码树
-
-        :param str or WDANode source: xml str or WDANode
-        """
-        self._source = source
-        self._tree: etree._Element = None
-        self._nodes: typing.List[WDANode] = None
+class SourceTree(_SourceTree[WDANode]):
+    node_type = WDANode
+    def __init__(self, source: Union[str, WDANode]) -> None:
+        super().__init__(source)
         self._window: typing.List[WDANode] = None
 
     @property
-    def tree(self):
-        if self._tree is None:
-            if isinstance(self._source, WDANode):
-                self._tree = etree.XML(self._source.xml.encode("utf8"), etree.XMLParser())
-            else:
-                self._tree = etree.XML(self._source.encode("utf8"), etree.XMLParser())
-        return self._tree
-
-    @property
-    def nodes(self):
-        if self._nodes is None:
-            if isinstance(self._source, WDANode):
-                self._nodes = extend_node(self._source)
-            else:
-                self._nodes = trans_tree_to_nodes(self.tree)
-        return self._nodes
-    
-    @property
     def window(self) -> typing.List[WDANode]:
         """把window过滤出来
 
         :return typing.List[WDANode]: window nodes
         """
         if not self._window:
             self._window = list(filter(lambda x: x.type == "Window", self.nodes))
         return self._window
+    
+    # def __init__(self, source: Union[str, WDANode]) -> None:
+    #     """实例化源代码树
+
+    #     :param str or WDANode source: xml str or WDANode
+    #     """
+    #     self._source = source
+    #     self._tree: etree._Element = None
+    #     self._nodes: typing.List[WDANode] = None
+    #     self._window: typing.List[WDANode] = None
+
+    # @property
+    # def tree(self):
+    #     if self._tree is None:
+    #         if isinstance(self._source, WDANode):
+    #             self._tree = etree.XML(self._source.xml.encode("utf8"), etree.XMLParser())
+    #         else:
+    #             self._tree = etree.XML(self._source.encode("utf8"), etree.XMLParser())
+    #     return self._tree
+
+    # @property
+    # def nodes(self):
+    #     if self._nodes is None:
+    #         if isinstance(self._source, WDANode):
+    #             self._nodes = extend_node(self._source)
+    #         else:
+    #             self._nodes = trans_tree_to_nodes(self.tree)
+    #     return self._nodes
+    
+    # @property
+    # def window(self) -> typing.List[WDANode]:
+    #     """把window过滤出来
+
+    #     :return typing.List[WDANode]: window nodes
+    #     """
+    #     if not self._window:
+    #         self._window = list(filter(lambda x: x.type == "Window", self.nodes))
+    #     return self._window
+
+    # def xpath(self, xp: str) -> typing.List[WDANode]:
+    #     els = self.tree.xpath(xp)
+    #     if not els:
+    #         return []
+    #     return [WDANode.parse(el) for el in els]
+    
+def can_use_tidevice(udid):
+    if udid in canUseTidevice:
+        return canUseTidevice[udid]
+    if tidevice is None:
+        canUseTidevice[udid] = False
+        return False
+    device = DeviceTool(udid)
+    os_version = Version(device.os_version)
+    if os_version >= "17.0":  # 还是检查一下
+        t = tidevice.Device(udid)
+        try:
+            t.mount_developer_image()
+            canUseTidevice[udid] = True
+            return True
+        except:
+            canUseTidevice[udid] = False
+            return False
+    canUseTidevice[udid] = True
+    return True
+    
+
+class StateMode(Enum):
+    INITIALIZED = 0
+    STATE = 1  # /wda/apps/state
+    STATUS = 2  # /status
+
+def ping_driver(address, port=None, timeout=10, state_mode=StateMode.STATUS, return_json=False):
+    """ping driver状态，如果超时则返回False"""
+    if state_mode is StateMode.STATE:
+        url = f"{address}/wda/apps/state"
+    elif state_mode is StateMode.STATUS:
+        url = f"{address}/status"
+    else:
+        raise RuntimeError("not supported mode.")
+    if port:
+        url = re.sub(r":\d+", f":{port}", url)
+    try:
+        if state_mode is StateMode.STATUS:
+            res = requests.get(url, timeout=timeout)
+        else:
+            res = requests.post(url, json.dumps({
+                "bundleId": ""
+            }))
+        logger.info("ping WebDriver [%s]: %s, %s", url, res.status_code, res.text)
+        if not res.text:
+            return False
+        if return_json:
+            return res.json()
+        return res.status_code == requests.codes.ok
+    except Exception as e:
+        logger.warning(f"获取driver状态失败: {str(e)}")
+    return False
+
+WDA_BUNDLE_NAMES = [
+    r"com\.facebook\.WebDriverAgentRunner\.xctrunner",
+    r"com\.facebook\.\S+\.xctrunner",
+    r"com\.\S+\.WebDriverAgentRunner\.xctrunner",
+    r"com\.\S+\.xctrunner",
+]
+
+def restart_driver(wda_ip, wda_port, udid, wda_bundle=None) -> bool:
+    # 使用 tidevice 重启 driver
+    if not can_use_tidevice(udid):
+        logger.warning(f"不支持tidevice方式重启wda")
+        return False
+    device = TIDevice(udid, wda_bundle, wda_port, ip=wda_ip)
+    if not device.wda_bundle:
+        logger.warning(f"未找到设备上安装的 wda")
+        return False
+    logger.info(f"找到可能的 wda app: {device.wda_bundle}")
+    logger.info("starting wda...")
+    device.start_driver()
+    if not check_relay_port(udid, wda_port, device.remote_port):
+        device.listen_port(wda_port)
+    if ping_driver(f"http://{wda_ip}:{wda_port}", timeout=10):
+        return True
+    return False
 
-    def xpath(self, xp: str) -> typing.List[WDANode]:
-        els = self.tree.xpath(xp)
-        if not els:
-            return []
-        return [WDANode.parse(el) for el in els]
 
 
 class WXIOSNative(BaseNative):
     _require_conf_ = [
         # ("wda_project_path", "wda_bundle")
     ]
-    useTIDevice = False
+    stateMode = StateMode.INITIALIZED  # 0: init; 1: /wda/apps/state; 2: /status
 
     def __init__(self, json_conf: dict):
         if json_conf is None:
             json_conf = {}
         super(WXIOSNative, self).__init__(json_conf)
+        device_info = json_conf.get("device_info", {})
         # 目标设备, 目标app
-        device = DeviceTool(json_conf.get("device_info", {}).get("udid"))
+        device = DeviceTool(device_info.get("udid"))
         self.udid = device.udid
-        self.bundle_id = json_conf.get("device_info", {}).get(
-            "bundle_id", WECHAT_PACKAGE
-        )
+        self.bundle_id = device_info.get("bundle_id") or WECHAT_PACKAGE
         # 使用xcode + wda project需要以下信息
         self.wda_project_path = json_conf.get("wda_project_path")
         self.wda_runner = None
         # 使用tidevice
         self.wda_bundle = json_conf.get("wda_bundle", None)
         # 已经通过xcode启动好wda
-        self.wda_port = json_conf.get("device_info").get("wda_port")
-        self.wda_ip = json_conf.get("device_info").get("wda_ip")
+        self.wda_port = json_conf.get("wda_port") or device_info.get("wda_port")
+        self.wda_ip = json_conf.get("wda_ip") or device_info.get("wda_ip")
         # 目标app实例
         self.app = None
         # 当前页面源代码树
+        self._full_tree = None
         self._source_tree = None
         # 获取性能的实例
         self.perf_flag = False
         self.perf = None
         self.last_cpu = 0
         self.last_fps = 0
         self.last_mem = 0
@@ -396,31 +479,51 @@
                 ((Selector(partial_text = "获取你的昵称"),), NativeModal.USERINFO, lambda answer: allow_btn if answer else reject_btn,),
                 ((Selector(text="获取你的微信运动步数"),), NativeModal.WERUN, lambda answer: allow_btn if answer else reject_btn,),
                 ((Selector(text="使用你的蓝牙"),), NativeModal.BLUETOOTH, lambda answer: allow_btn if answer else reject_btn,),
             ),
         )
         self._last_modal_type = None
 
+        # 检查 wda 状态
+        wda_ip = self.wda_ip or WDA_DEFAULT_IP
+        wda_port = self.wda_port or pick_unuse_port()
+        if not check_iproxy_port(self.udid, wda_port, WDA_REMOTE_PORT):
+            listen_iproxy_port(self.udid, wda_port, WDA_REMOTE_PORT, wda_ip)
+        if ping_driver(f"http://{wda_ip}:{wda_port}", timeout=10):
+            self.wda_ip = wda_ip
+            self.wda_port = wda_port
+        elif not self.wda_project_path or isWindows:  # 没有 ping 通, 且没法使用 xcode 启动
+            if restart_driver(wda_ip, wda_port, self.udid):
+                self.wda_ip = wda_ip
+                self.wda_port = wda_port
+            else:
+                logger.warning(f"尝试启动 wda 失败")
+
     ###############################
     #                    interface                        #
     ###############################
     def start_wechat(self, new_session=True):
         """
         启动微信
         :return:
         """
+        wda_ip = self.wda_ip or WDA_DEFAULT_IP
         if self.wda_project_path and not isWindows:
-            self.wda_runner = WebDriverRunner(self.udid, self.wda_project_path, port=self.wda_port)
-        elif self.wda_ip and not self.wda_bundle:  # 配置了ip & 没有bundle, 说明已经启动好wda
-            self.wda_runner = WebDriverRunner(self.udid, self.wda_project_path, port=self.wda_port)
+            self.wda_runner = WebDriverRunner(self.udid, self.wda_project_path, port=self.wda_port, ip=wda_ip)
+        elif (self.wda_ip or self.wda_port) and not (self.wda_bundle and can_use_tidevice(self.udid)):
+            # 配置了ip/port & 不能使用 tidevice启动wda_bundle
+            self.wda_runner = WebDriverRunner(self.udid, self.wda_project_path, port=self.wda_port, ip=wda_ip)
         else:
+            if not can_use_tidevice(self.udid):
+                raise RuntimeError(f"tidevice 暂不支持此系统版本: {DeviceTool(self.udid).os_version}, 启动 wda 失败, 请使用 xcode 启动")
             self.wda_runner = TIDevice(self.udid, self.wda_bundle)
-            if self.udid is None:
-                self.udid = self.wda_runner.device_id
-            self.useTIDevice = True
+        if not ping_driver(f"http://{wda_ip}:{self.wda_runner.port}", timeout=10):
+            self.restart_driver()
+        if not self.wda_runner.find_app(self.bundle_id):
+            logger.warning(f"app {self.bundle_id} may not installed")
         for i in range(3):
             try:
                 logger.info("第 %d 次启动微信, 共3次机会" % (i + 1))
                 self.app = WdaUI(
                     server_url="http://%s:%s" % (self.wda_ip or "localhost", self.wda_runner.port),
                     bundle_id=self.bundle_id if new_session else None,
                 )
@@ -698,15 +801,15 @@
                     self._allow_authorize(answer, "获取你的微信运动步数")
                 # print("finish wait %f" % time.time())
                 self.check_done = True
                 self.health_modal_handle_thread = None
 
             self.stop_check = False
             self.check_done = False
-            self.health_modal_handle_thread = threading.Thread(target=check_health)
+            self.health_modal_handle_thread = threading.Thread(target=check_health, name="CheckHealth")
             self.health_modal_handle_thread.setDaemon(True)
             self.health_modal_handle_thread.start()
         if not self._wait(lambda: self.health_page_exists, timeout=10, interval=2):
             # print("health_page_exists wait fail %f" % time.time())
             ret = self._allow_authorize(answer, "获取你的微信运动步数")
             return answer if ret else True
         else:
@@ -806,46 +909,51 @@
     def modal_exists(self, title):
         """
         指定title的modal是否存在
         """
         return self.__modal_exists(title)
 
     def handle_modal(
-        self, btn_text="确定", title: str = None, index=-1, force_title=False
+        self, btn_text: Union[str, bool, WDASelector] =None, title: str = None, index=-1, force_title=False
     ):
         """
         处理模态弹窗
         :param title: 传入弹窗的 title 可以校验当前弹窗是否为预期弹窗
         :param btn_text: 根据传入的 文字 进行点击
         :param index: 当页面存在完全相同的两个控件时，通过指定 index 来选取
         :return:
         """
         if title and force_title:
             if not self.modal_exists(title):
                 return False
+        if not btn_text:
+            btn_text = "确定"
         logger.info(f"可能出现弹框：{title}, 自动选择【{btn_text}】")
         if isinstance(btn_text, bool):
             btn_text = "确定" if btn_text else "取消"
-        return self.app.session(
-            xpath='//Button//StaticText[@name="{btn_text}"]'.format(btn_text=btn_text),
-            index=index,
-        ).click_if_exists(timeout=5.0)
+        if isinstance(btn_text, str):
+            return self.app.session(
+                xpath='//Button//StaticText[@name="{btn_text}"]'.format(btn_text=btn_text),
+                index=index,
+            ).click_if_exists(timeout=5.0)
+        elif isinstance(btn_text, WDASelector):
+            return btn_text.click_if_exists(timeout=5.0)
 
     def handle_action_sheet(self, item):
         """
         处理上拉菜单
         :param item: 要选择的 item
         :return:
         """
         return self.app.session(class_name="ScrollView").subelems(
             class_name="Button", text=item
         ).click_if_exists(timeout=10.0)
 
     def forward_miniprogram(
-        self, name: str or list, text: str = None, create_new_chat: bool = True
+        self, name: Union[str, list], text: str = None, create_new_chat: bool = True
     ):
         """
         通过右上角更多菜单转发小程序
         ps: 好友太多会有性能问题
         :type text: 分享携带的内容
         :param names: 要分享的人
         :param create_new_chat: 是否创建群聊
@@ -863,23 +971,24 @@
         else:
             self.app.session(partial_text="关于").click(timeout=10.0)
             self.app.session(partial_text="推荐给朋友").click(timeout=10.0)
 
         return self.forward_miniprogram_inside(name, text, create_new_chat)
 
     def forward_miniprogram_inside(
-        self, name: str or list, text: str = None, create_new_chat: bool = True
+        self, name: Union[str, list], text: str = None, create_new_chat: bool = True
     ):
         """
         小程序内触发转发小程序
         ps: 好友太多会有性能问题
         :param names: 要分享的人
         :param create_new_chat: 是否创建群聊
         :return:
         """
+        ret = True
         if self.app.session(
             xpath='//Button[.//StaticText[@name="分享提示"]]'
         ).exists:  # 开发版会弹出分享提示
             self.handle_modal("确定")
 
         if isinstance(name, str):
             name = [name]
@@ -892,27 +1001,46 @@
                 for word in [ WORDING.IOS.CREATE_CHAT1, WORDING.IOS.CREATE_CHAT2 ]:
                     if self.app.session(class_name="StaticText", text=word.value).exists:
                         self._new_chat_wording = word
                         break
                 if not self._new_chat_wording:
                     raise RuntimeError("无法创建新聊天")
             self.app.session(class_name="StaticText", text=self._new_chat_wording.value).click(timeout=10.0)
+        search_text = WORDING.COMMON.SEARCH.value
         for _name in name:
-            self.app.session(
-                class_name="TextField" if create_new_chat else "SearchField", text=WORDING.COMMON.SEARCH.value
-            ).set_text(_name)
+            el = self.app.session(
+                class_name="TextField" if create_new_chat else "SearchField", text=search_text
+            )
+            if not el.exists and search_text:
+                el = self.app.session(class_name="TextField" if create_new_chat else "SearchField")
+                if el.exists:
+                    search_text = ""
+            el.set_text(_name)
             # count = 10
             time.sleep(1.5)  # 一定需要等待搜索出该用户
-            self.app.session(
-                class_name="StaticText", partial_text=_name, index=-1
-            ).click(timeout=10.0)
+            elements = self.app.session(class_name="StaticText", partial_text=_name).elements
+            for i in range(-1,-1 * (len(elements) + 1),-1):
+                self.app.session(
+                    class_name="StaticText", partial_text=_name, index=i
+                ).click(timeout=10.0)
+                if len(self.app.session(class_name="StaticText", partial_text=_name).elements) != len(elements):
+                    break
             # count -= 1
         if create_new_chat:
             self.app.session(class_name="Button", partial_text=WORDING.COMMON.DONE.value).click(timeout=10.0)
+        if text:
+            try:
+                self.app.session(class_name="TextView").set_text(text)
+            except wda.WDAElementNotFoundError:
+                ret = False
+            except Exception as e:
+                logger.warning("catch wda.WDAElementNotFoundError")
+                ret = False
         self.app.session(class_name="Button", text=WORDING.COMMON.SEND.value).click(timeout=10.0)
+        return ret
 
     def send_custom_message(self, message: str = None):
         """
         处理小程序 im 发送自定义消息
         :param message: 消息内容
         :return:
         """
@@ -1053,30 +1181,34 @@
         activity = []
         app_status = self.app.session.app_state(self.bundle_id)
         if app_status.value == AppState.RUNNING_IN_FOREGROUND.value:
             activity.append(self.bundle_id)
         else:
             activity.append(OTHER_PACKAGE)
         # 检查胶囊 和 webview，同时存在则在小程序中
-        capsule = self.app.session(
-            xpath='//Other/Button[@label="更多"]/following-sibling::XCUIElementTypeButton[@label="关闭"]'
-        )
-        webview = self.app.session(class_name="WebView")
+        source = self.source()
+        # 这个有可能被蒙层挡住
+        capsule_xpath = '//Other/Button[@label="更多"]/following-sibling::Button[@label="关闭"]'
+        # capsule = self.app.session(
+        #     xpath=capsule_xpath
+        # )
+        webview_xpath = "//WebView"
+        # webview = self.app.session(class_name="WebView")
         # 检查tabbar
         tabbar_items = ["微信", "通讯录", "发现", "我"]
-        main_frame_tabbar = self.app.session(
-            xpath='//TabBar/XCUIElementTypeButton[@label="%s"]/' % tabbar_items[0]
-            + "/".join(
-                'following-sibling::XCUIElementTypeButton[@label="%s"]' % item
+        main_frame_tabbar_xpath = f'//TabBar/Button[@label="{tabbar_items[0]}"]/' + "/".join(
+                'following-sibling::Button[@label="%s"]' % item
                 for item in tabbar_items[1:]
             )
-        )
-        if capsule.exists and webview.exists:
+        # main_frame_tabbar = self.app.session(
+        #     xpath=main_frame_tabbar_xpath
+        # )
+        if self._full_tree.xpath(capsule_xpath) and source.xpath(webview_xpath):
             activity.append(MINIPROGRAM_ACTIVITY)
-        elif main_frame_tabbar.exists:
+        elif source.xpath(main_frame_tabbar_xpath):
             activity.append(WECHAT_ACTIVITY)
         else:
             activity.append(OTHER_ACTIVITY)
         return "/".join(activity)
 
     def _is_in_wechat(self, activity: str):
         return activity.startswith(self.bundle_id)
@@ -1092,15 +1224,15 @@
         self.source()
         # check auth
         modal_type, node = self._check_auth_type(confirm, 0)
         if modal_type is not NativeModal.NONE:
             return (modal_type, confirm)
         # 兜底
         if self._search_el_from_source(class_name="Button", text="确定"):
-            return (NativeModal.MODAL, True)
+            return (NativeModal.MODAL, self.app.session(class_name="Button", text="确定"))
         # self.app.session.alert.click_button_if_exists("确定")  # 系统弹窗需要用这个才能判断
         return None
 
 
     def _get_any_modal_old(self, confirm=False):
         """
         confirm == True: 确认/允许
@@ -1181,14 +1313,15 @@
         remove port forward process
         :return:
         """
         super().release()
         if self.perf_flag:
             self.stop_get_perf()
         self.wda_runner.remove_iproxy()
+        self._empty_base_screen_dir(self.outputs_screen)
 
     ###############################
     #                      private                         #
     ###############################
 
     def _capture_photo(self, media_type, duration=10.0):
         """
@@ -1298,34 +1431,27 @@
             self.last_fps = value["value"]
         elif data_type == "memory":
             item.update(
                 {"mem": value["value"], "cpu": self.last_cpu, "fps": self.last_fps}
             )
             self.last_mem = value["value"]
 
-    def start_get_perf(self, timeinterval=15):
+    def start_get_perf(self, timeinterval=15) -> bool:
         """
         开始获取性能数据
         :param timeinterval: 抽样时间间隔
         :return: boolen
         """
         if self.perf_flag:
             return True
-        if not self.useTIDevice:
+        if not can_use_tidevice(self.udid):
             return False
         if tidevice is None:
             return False
         t = tidevice.Device(self.udid)
-        if not canUseTidevice.get(self.udid):  # 检查一下能不能使用
-            try:
-                t.mount_developer_image()
-                canUseTidevice[self.udid] = True
-            except:
-                self.useTIDevice = False
-                return False
         self.perf = tidevice.Performance(t, [tidevice.DataType.CPU, tidevice.DataType.MEMORY, tidevice.DataType.FPS])
         self.last_fps = 0
         self.last_cpu = 0
         self.last_mem = 0
         self.perf.start(self.bundle_id, callback=self._perf_callback)
         self.perf_flag = True
         return self.perf_flag
@@ -1342,40 +1468,107 @@
         result = json.dumps(self.perf_data)
         self.perf_data = []
         self.last_fps = 0
         self.last_cpu = 0
         self.last_mem = 0
         return result
 
+    def click_node(self, node: Union[WDANode, List[WDANode]]):
+        if not node:
+            return False
+        if isinstance(node, WDANode):
+            node = [node]
+        for n in node:
+            self.click_coordinate(n.center_x, n.center_y)
+        return True
+
+    def check_connected(self):
+        """检查是否存在【连接断开】的情况，有则手动断开一下"""
+        s = self.source()
+        view = s.xpath('//*[@name="连接断开"]/following-sibling::Button[@name="展开"]')
+        if not view:
+            return True
+        self.click_node(view)
+        time.sleep(1)
+        s = self.source()
+        if self.click_node(s.xpath('//Button[@name="收起"]//preceding-sibling::Button[@name="停止"]')):
+            time.sleep(2)
+            self.close_local_debug_modal()
+        return False
+
     @cost_debug(0.1)
-    def check_connection(self):
+    def check_connection(self, port=None):
         try:
-            return self.app.status()["state"] == "success"
+            ret = ping_driver(self.app.client.http.address, port, 10, StateMode.STATUS, return_json=True)
+            return (ret["value"]["state"] == "success")
         except:
             return False
 
     # 以下方法可能被重构
     @property
     @cost_debug(1)
     def source_json(self) -> dict:
-        return self.app.source(data_format="json")
+        try:
+            return self.app.source(data_format="json")
+        except (WDAEmptyResponseError, Exception) as e:
+            logger.warning("empty response for source cmd")
+            logger.info(f"{e.__class__.__name__}: {e}")
+            if self.check_connection():
+                logger.info(f"try to get accessible source from old wda port {self.wda_port}")
+                source = self.app.client.accessibleSource()
+                if source:
+                    return source
+            # 重新设置转发端口
+            new_wda_port = self.wda_runner.pick_unuse_port()
+            self.wda_runner.listen_port(port=new_wda_port, device_id=self.udid)
+            logger.info(do_shell("ps -ef|grep iproxy"))
+            if self.check_connection(new_wda_port):
+                logger.info(f"use new wda port {new_wda_port}")
+                self.wda_port = new_wda_port
+                self.wda_runner.port = new_wda_port
+                self.app.client.http.address = re.sub(r":\d+", f":{new_wda_port}", self.app.client.http.address)
+                self.app.session.http.address = re.sub(r":\d+", f":{new_wda_port}", self.app.session.http.address)
+            else:
+                logger.warning(f"ping new port fail, restart driver")
+                try:
+                    ret = self.restart_driver()
+                except RuntimeError:
+                    ret = restart_driver(self.wda_ip, self.wda_port, self.udid, wda_bundle=None)
+                if ret:
+                    logger.info("重启wda成功.")
+                else:
+                    raise wda.WDAError("WDA没有启动: 重启失败")
+            return self.app.source(data_format="json")
+        
+    def restart_driver(self):
+        wda_ip = self.wda_ip or WDA_DEFAULT_IP
+        self.wda_runner.remove_iproxy()
+        self.wda_runner.start_driver()
+        self.wda_runner.listen_port(ip=wda_ip)
+        if ping_driver(f"http://{wda_ip}:{self.wda_runner.port}", timeout=10):
+            self.wda_ip = wda_ip
+            self.wda_port = self.wda_runner.port
+            return True
+        else:
+            logger.warning(f"启动 wda 失败, wda 项目路径: {self.wda_project_path}")
+        return False
     
     @property
     @cost_debug(1)
     def source_xml(self) -> dict:
         return self.app.source(data_format="xml")
     
     @cost_debug(1)
     def source(self):
         """refresh source"""
         # xml比json返回慢进1倍, 使用source_json
         # 此函数可能需要高达2s左右的耗时
         root = WDANode(self.source_json)
         new_root = remove_invisible_child(root, True)
-        self._test_tree = SourceTree(root)
+        self._full_tree = SourceTree(root)
         self._source_tree = SourceTree(new_root)
         # remove_invisible_child(root, False)
         # self._source_tree = SourceTree(root)
         return self._source_tree
 
     def _get_source_list(self) -> typing.List[WDANode]:
         stime = time.time()
@@ -1500,15 +1693,19 @@
                 break
             time.sleep(1)
         else:
             return NativeModal.NONE, None
         return NativeModal.NORMAL, None
 
     def allow_privacy(self, answer=True):
-        return self.app.session(text="同意" if answer else "拒绝", index=-1).click_if_exists(0.5)
+        try:
+            return self.app.session(text="同意" if answer else "拒绝", index=-1).click_if_exists(0.5)
+        except WDAElementNotFoundError as e:
+            logger.warning(e)
+            return False
 
     def handle_alter_before_unload(self, answer=True):
         return self.handle_modal("确定" if answer else "取消")
 
     @cost_debug(1)
     def _handle_auth(self, modal_type: NativeModal, answer):
         # logger.info(f"处理 {modal_type.name} 弹窗")
```

### Comparing `minium-1.5.3/minium/native/wx_native/wording.py` & `minium-1.5.4/minium/native/wx_native/wording.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/emitter.py` & `minium-1.5.4/minium/utils/emitter.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/injectjs.py` & `minium-1.5.4/minium/utils/injectjs.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/createContext.js` & `minium-1.5.4/minium/utils/js/es5/createContext.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/getUni.js` & `minium-1.5.4/minium/utils/js/es5/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/helpers.js` & `minium-1.5.4/minium/utils/js/es5/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/hijackWxMethod.js` & `minium-1.5.4/minium/utils/js/es5/hijackWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/ideMockChooseLocation.js` & `minium-1.5.4/minium/utils/js/es5/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/ideMockGetLocation.js` & `minium-1.5.4/minium/utils/js/es5/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/ideMockGetWeRunData.js` & `minium-1.5.4/minium/utils/js/es5/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/ideMockModal.js` & `minium-1.5.4/minium/utils/js/es5/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/mockChooseImage.js` & `minium-1.5.4/minium/utils/js/es5/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/mockCloudCall.js` & `minium-1.5.4/minium/utils/js/es5/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/mockNetwork.js` & `minium-1.5.4/minium/utils/js/es5/mockNetwork.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -51,15 +51,15 @@
                     this.headersReceivedCallback.push(a)
                 }
             }, {
                 key: "onProgressUpdate",
                 value: function onProgressUpdate(a) {
                     this.progressUpdateCallback.push(a)
                 }
-            }]), a
+            }])
         }();
         global.__minium__["".concat(a, "Task")] = b;
         var c = new global.__minium__.MockRule("".concat(a, "_network_mock_rule"));
         global.__minium__.setMock(a, function(a) {
             var d = c.search(a);
             return d ? (console.log("@@@@rule match", d), a.__miniumMocked = !0, d.success) ? new b(d.success, void 0, function(b) {
                 a.success && a.success(b), a.complete && a.complete(b)
```

### Comparing `minium-1.5.3/minium/utils/js/es5/networkPannel.js` & `minium-1.5.4/minium/utils/js/es5/networkPannel.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -5,21 +5,22 @@
         var c = function(a, b) {
                 if (global && global.__minium__.get_mini_network_id && "https://weapp.tencent.com/jscov_driver/CollectCovTimer" != a.url) {
                     var c = global.__minium__.get_mini_network_id(),
                         d = Object.assign({}, a);
                     delete d.success, delete d.fail, delete d.complete;
                     var e, h = Date.now();
                     try {
-                        var j = JSON.stringify(d);
-                        e = f(j), g.has(e) && g.get(e) > h && (j = ""), g.set(e, h + 21e3), mini_send_request(c, j, h, e)
+                        var j, k = JSON.stringify(d);
+                        e = f(k), g.has(e) && g.get(e) > h && (k = ""), g.set(e, h + 21e3), mini_send_request(c, k, h, e, null === (j = getCurrentPages().pop()) || void 0 === j ? void 0 : j.__route__)
                     } catch (a) {
+                        var l;
                         mini_send_request(c, JSON.stringify({
                             url: d.url,
                             err: a.toString()
-                        }), h, 0)
+                        }), h, 0, null === (l = getCurrentPages().pop()) || void 0 === l ? void 0 : l.__route__)
                     }
                     i.set(b, {
                         nid: c,
                         obj: a
                     })
                 }
             },
```

### Comparing `minium-1.5.3/minium/utils/js/es5/requestStack.js` & `minium-1.5.4/minium/utils/js/es5/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/es5/testAsync.js` & `minium-1.5.4/minium/utils/js/es5/testAsync.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -77,15 +77,15 @@
             }
         })
     }
 
     function w(a, b, d) {
         var e = "suspendedStart";
         return function(f, g) {
-            if (e === "executing") throw new Error("Generator is already running");
+            if (e === "executing") throw Error("Generator is already running");
             if ("completed" === e) {
                 if ("throw" === f) throw g;
                 return {
                     value: D,
                     done: !0
                 }
             }
@@ -255,15 +255,15 @@
                 if (g.tryLoc <= this.prev) {
                     var j = t.call(g, "catchLoc"),
                         k = t.call(g, "finallyLoc");
                     if (j && k) {
                         if (this.prev < g.catchLoc) return d(g.catchLoc, !0);
                         if (this.prev < g.finallyLoc) return d(g.finallyLoc)
                     } else if (!j) {
-                        if (!k) throw new Error("try statement without catch or finally");
+                        if (!k) throw Error("try statement without catch or finally");
                         if (this.prev < g.finallyLoc) return d(g.finallyLoc)
                     } else if (this.prev < g.catchLoc) return d(g.catchLoc, !0)
                 }
             }
         },
         abrupt: function abrupt(b, c) {
             for (var d, e = this.tryEntries.length - 1; 0 <= e; --e)
@@ -287,15 +287,15 @@
                 if (b = this.tryEntries[c], b.tryLoc === a) {
                     var d = b.completion;
                     if ("throw" === d.type) {
                         var f = d.arg;
                         A(b)
                     }
                     return f
-                } throw new Error("illegal catch attempt")
+                } throw Error("illegal catch attempt")
         },
         delegateYield: function delegateYield(a, b, c) {
             return this.delegate = {
                 iterator: C(a),
                 resultName: b,
                 nextLoc: c
             }, "next" === this.method && (this.arg = D), G
```

### Comparing `minium-1.5.3/minium/utils/js/es5/utils.js` & `minium-1.5.4/minium/utils/js/es5/utils.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -119,15 +119,15 @@
                                 if ("success" != f && "fail" != f && "complete" != f && "_miniMockType" != f) {
                                     if (void 0 === c[f]) return !1;
                                     if (!a.isRuleMatched(b[f], c[f])) return !1
                                 } return !0
                     }
                     return !1
                 }
-            }]), a
+            }])
         }();
     global.__minium__.MockRule = d, global.__minium__.bind = function(a, b) {
         for (var c = arguments.length, d = Array(2 < c ? c - 2 : 0), e = 2; e < c; e++) d[e - 2] = arguments[e];
         return function() {
             for (var c = arguments.length, e = Array(c), f = 0; f < c; f++) e[f] = arguments[f];
             return a.apply(b, d.concat(e))
         }
```

### Comparing `minium-1.5.3/minium/utils/js/min/getUni.js` & `minium-1.5.4/minium/utils/js/min/getUni.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/helpers.js` & `minium-1.5.4/minium/utils/js/min/helpers.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/hijackWxMethod.js` & `minium-1.5.4/minium/utils/js/min/hijackWxMethod.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/ideMockChooseLocation.js` & `minium-1.5.4/minium/utils/js/min/ideMockChooseLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/ideMockGetLocation.js` & `minium-1.5.4/minium/utils/js/min/ideMockGetLocation.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/ideMockGetWeRunData.js` & `minium-1.5.4/minium/utils/js/min/ideMockGetWeRunData.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/ideMockModal.js` & `minium-1.5.4/minium/utils/js/min/ideMockModal.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/mockChooseImage.js` & `minium-1.5.4/minium/utils/js/min/mockChooseImage.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/mockCloudCall.js` & `minium-1.5.4/minium/utils/js/min/mockCloudCall.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/mockNetwork.js` & `minium-1.5.4/minium/utils/js/min/mockNetwork.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/networkPannel.js` & `minium-1.5.4/minium/utils/js/min/networkPannel.js`

 * *Files 14% similar despite different names*

#### js-beautify {}

```diff
@@ -10,49 +10,49 @@
         if (t && !1 === t.configurable) return void console.warn("[minitest] Cannot redefine property: request");
         let n = function(e) {
                 let t = 5381,
                     n = e.length;
                 for (; n;) t = 33 * t ^ e.charCodeAt(--n);
                 return t >>> 0
             },
-            i = new Map,
             r = new Map,
-            l = new Map;
+            i = new Map,
+            _ = new Map;
         global.__minium__.setCall("request", "networkPannel", {
             before: function(e, t) {
                 if (!global || !global.__minium__.get_mini_network_id) return;
                 if ("https://weapp.tencent.com/jscov_driver/CollectCovTimer" == e.url) return;
-                let r, o = global.__minium__.get_mini_network_id(),
-                    _ = Object.assign({}, e);
-                delete _.success, delete _.fail, delete _.complete;
+                let i, o = global.__minium__.get_mini_network_id(),
+                    l = Object.assign({}, e);
+                delete l.success, delete l.fail, delete l.complete;
                 let s = Date.now();
                 try {
-                    let e = JSON.stringify(_);
-                    r = n(e), i.has(r) && i.get(r) > s && (e = ""), i.set(r, s + 21e3), mini_send_request(o, e, s, r)
+                    let e = JSON.stringify(l);
+                    i = n(e), r.has(i) && r.get(i) > s && (e = ""), r.set(i, s + 21e3), mini_send_request(o, e, s, i, getCurrentPages().pop()?.__route__)
                 } catch (e) {
                     mini_send_request(o, JSON.stringify({
-                        url: _.url,
+                        url: l.url,
                         err: e.toString()
-                    }), s, 0)
+                    }), s, 0, getCurrentPages().pop()?.__route__)
                 }
-                l.set(t, {
+                _.set(t, {
                     nid: o,
                     obj: e
                 })
             },
             callback: function(e, t) {
-                if (!l.has(t)) return;
+                if (!_.has(t)) return;
                 const {
-                    nid: i,
+                    nid: r,
                     obj: o
-                } = l.get(t);
-                l.delete(t);
-                let _ = Object.assign({}, e);
-                delete _.profile;
-                let s = JSON.stringify(_),
+                } = _.get(t);
+                _.delete(t);
+                let l = Object.assign({}, e);
+                delete l.profile;
+                let s = JSON.stringify(l),
                     a = n(s),
                     u = Date.now();
-                r.has(a) && r.get(a) > u && (s = ""), r.set(a, u + 21e3), mini_request_callback(i, s, u, a, o.__miniumMocked)
+                i.has(a) && i.get(a) > u && (s = ""), i.set(a, u + 21e3), mini_request_callback(r, s, u, a, o.__miniumMocked)
             }
         }, !0)
     }
 }
```

### Comparing `minium-1.5.3/minium/utils/js/min/requestStack.js` & `minium-1.5.4/minium/utils/js/min/requestStack.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/js/min/utils.js` & `minium-1.5.4/minium/utils/js/min/utils.js`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium/utils/meta.py` & `minium-1.5.4/minium/utils/meta.py`

 * *Files identical despite different names*

### Comparing `minium-1.5.3/minium.egg-info/SOURCES.txt` & `minium-1.5.4/minium.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+MANIFEST.in
+requirements.txt
 setup.py
 minium/__init__.py
 minium.egg-info/PKG-INFO
 minium.egg-info/SOURCES.txt
 minium.egg-info/dependency_links.txt
 minium.egg-info/entry_points.txt
 minium.egg-info/requires.txt
@@ -111,23 +113,26 @@
 minium/externlib/wechat_mp_inspector/connection/websocketconn.py
 minium/externlib/wechat_mp_inspector/driver/__init__.py
 minium/externlib/wechat_mp_inspector/driver/androiddriver.py
 minium/externlib/wechat_mp_inspector/driver/basedriver.py
 minium/externlib/wechat_mp_inspector/driver/config.py
 minium/externlib/wechat_mp_inspector/driver/iosdriver.py
 minium/externlib/wechat_mp_inspector/driver/mpdriver.py
+minium/externlib/wechat_mp_inspector/driver/officialaccount.py
 minium/externlib/wechat_mp_inspector/inspector/__init__.py
 minium/externlib/wechat_mp_inspector/inspector/androidinspector.py
 minium/externlib/wechat_mp_inspector/inspector/androidwxainspector.py
 minium/externlib/wechat_mp_inspector/inspector/baseinspector.py
 minium/externlib/wechat_mp_inspector/inspector/iosinspector.py
 minium/externlib/wechat_mp_inspector/inspector/ioswxainspector.py
+minium/externlib/wechat_mp_inspector/inspector/wxainspector.py
 minium/externlib/wechat_mp_inspector/pages/__init__.py
 minium/externlib/wechat_mp_inspector/pages/basepage.py
 minium/externlib/wechat_mp_inspector/pages/chromepage.py
+minium/externlib/wechat_mp_inspector/pages/mppage.py
 minium/externlib/wechat_mp_inspector/pages/safaripage.py
 minium/externlib/wechat_mp_inspector/protocol/__init__.py
 minium/externlib/wechat_mp_inspector/protocol/baseprotocol.py
 minium/externlib/wechat_mp_inspector/protocol/basesession.py
 minium/externlib/wechat_mp_inspector/protocol/basewebkit.py
 minium/externlib/wechat_mp_inspector/protocol/cdp.py
 minium/externlib/wechat_mp_inspector/protocol/protocolcommand.py
@@ -136,15 +141,14 @@
 minium/externlib/wx_wda/__init__.py
 minium/externlib/wx_wda/wdaUI.py
 minium/externlib/wx_wda/webDriverTool.py
 minium/framework/__init__.py
 minium/framework/assertbase.py
 minium/framework/casedump.py
 minium/framework/caseinspect.py
-minium/framework/errorReport.py
 minium/framework/exception.py
 minium/framework/loader.py
 minium/framework/logcolor.py
 minium/framework/miniconfig.py
 minium/framework/miniddt.py
 minium/framework/minidoctor.py
 minium/framework/minilimit.py
@@ -182,14 +186,15 @@
 minium/miniprogram/base_driver/connection.py
 minium/miniprogram/base_driver/element.py
 minium/miniprogram/base_driver/h5_element.py
 minium/miniprogram/base_driver/minium.py
 minium/miniprogram/base_driver/minium_log.py
 minium/miniprogram/base_driver/minium_object.py
 minium/miniprogram/base_driver/prefixer.py
+minium/miniprogram/base_driver/selector.py
 minium/miniprogram/base_driver/version.json
 minium/miniprogram/base_driver/version.py
 minium/miniprogram/base_driver/waiter.py
 minium/miniprogram/base_driver/page/__init__.py
 minium/miniprogram/base_driver/page/h5page.py
 minium/miniprogram/base_driver/page/page.py
 minium/miniprogram/base_driver/page/skylinepage.py
@@ -236,14 +241,15 @@
 minium/utils/js/es5/evalMockChooseImage.js
 minium/utils/js/es5/getAppConfig.js
 minium/utils/js/es5/getCurrentPages.js
 minium/utils/js/es5/getUni.js
 minium/utils/js/es5/helpers.js
 minium/utils/js/es5/hijackWxMethod.js
 minium/utils/js/es5/hookCurrentPageMethod.js
+minium/utils/js/es5/hookNavigation.js
 minium/utils/js/es5/hookWxMethod.js
 minium/utils/js/es5/hookWxMethodWithId.js
 minium/utils/js/es5/ideHandleAuthModal.js
 minium/utils/js/es5/ideHandleMap.js
 minium/utils/js/es5/ideHandleModal.js
 minium/utils/js/es5/ideMockAuth.js
 minium/utils/js/es5/ideMockAuthSetting.js
@@ -282,14 +288,15 @@
 minium/utils/js/min/evalMockChooseImage.js
 minium/utils/js/min/getAppConfig.js
 minium/utils/js/min/getCurrentPages.js
 minium/utils/js/min/getUni.js
 minium/utils/js/min/helpers.js
 minium/utils/js/min/hijackWxMethod.js
 minium/utils/js/min/hookCurrentPageMethod.js
+minium/utils/js/min/hookNavigation.js
 minium/utils/js/min/hookWxMethod.js
 minium/utils/js/min/hookWxMethodWithId.js
 minium/utils/js/min/ideHandleAuthModal.js
 minium/utils/js/min/ideHandleMap.js
 minium/utils/js/min/ideHandleModal.js
 minium/utils/js/min/ideMockAuth.js
 minium/utils/js/min/ideMockAuthSetting.js
```

### Comparing `minium-1.5.3/setup.py` & `minium-1.5.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 '''
 Author: yopofeng
 Date: 2023-10-06 17:50:32
 LastEditors: yopofeng yopofeng@tencent.com
-LastEditTime: 2024-01-15 16:03:27
+LastEditTime: 2024-04-11 11:32:49
 FilePath: /py-minium/setup.py
 Description: 
 
 Copyright (c) 2023 by ${git_name_email}, All Rights Reserved. 
 '''
 #!/usr/bin/env python3
 import sys
 import os
 
-__version__ = "1.5.3"
+__version__ = "1.5.4"
 
 from setuptools import setup, find_packages
 
 # We do not support Python <3.8
 if sys.version_info < (3, 8):
     print(
         "Unfortunately, your python version is not supported!\n"
         "Please upgrade at least to Python 3.8!",
         file=sys.stderr,
     )
     sys.exit(1)
 
-install_requires = [
-    "ddt",
-    "pyyaml",
-    "websocket_client>=1.3,<1.4",  # 1.4.0后有个兼容报错
-    "requests",
-    "future",
-    "pyee",
-    "typing_extensions",
-    "websockets"
-]
+requirements_path = "requirements.txt"
+try:
+    import pkg_resources
+except ImportError:
+    # websocket_client # 1.4.0后有个兼容报错
+    with open(requirements_path, "r") as f:
+        install_requires = f.read().split("\n")
+else:
+    with open(requirements_path, "r") as f:
+        install_requires = [str(req) for req in pkg_resources.parse_requirements(f)]
 
 entry_points = {
     "console_scripts": [
         "minitest=minium.framework.loader:main",
         "minidoctor=minium.framework.minidoctor:main",
         "miniruntest=minium.framework.loader:main",
         "minireport=minium.framework.report:main",
@@ -51,25 +51,26 @@
         for filename in files:
             yield os.path.join(os.path.relpath(root, pkg), filename)
 
 config_path = "miniprogram/base_driver/version.json"
 package_data = {
     "minium": [
         config_path,
+        requirements_path,
         *list(find_data_files("minium", "externlib")),
         *list(find_data_files("minium", "framework/dist")),
         *list(find_data_files("minium", "native")),
         *list(find_data_files("minium", "utils/js/min")),
         *list(find_data_files("minium", "utils/js/es5")),
     ]
 }
 
 exclude_package_data = {"": ["*pyc", "readme.md", "build.py", "__pycache__"]}
 extras_require = {
-    "ios": ["tidevice==0.10.12", "lxml", "nest_asyncio", "pymobiledevice3"],
+    "ios": ["tidevice==0.12.0", "lxml", "nest_asyncio", "pymobiledevice3"],
 }
 
 long_description = """
 install:
 ```
 pip3 install minium
 ```
```

