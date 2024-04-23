# Comparing `tmp/libfwsi-python-20240417.tar.gz` & `tmp/libfwsi-python-20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfwsi-python-20240417.tar", last modified: Wed Apr 17 16:04:37 2024, max compression
+gzip compressed data, was "libfwsi-python-20240423.tar", last modified: Tue Apr 23 05:26:02 2024, max compression
```

## Comparing `libfwsi-python-20240417.tar` & `libfwsi-python-20240423.tar`

### file list

```diff
@@ -1,779 +1,779 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26787 2024-04-17 05:54:47.000000 libfwsi-20240417/libfole/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 05:54:34.000000 libfwsi-20240417/libfole/libfole_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-17 04:08:48.000000 libfwsi-20240417/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-17 05:54:47.000000 libfwsi-20240417/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 04:08:48.000000 libfwsi-20240417/NEWS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-04-17 04:08:48.000000 libfwsi-20240417/libfwsi.spec.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-17 05:54:47.000000 libfwsi-20240417/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26867 2024-04-17 05:54:47.000000 libfwsi-20240417/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 05:54:32.000000 libfwsi-20240417/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4187 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfole.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-17 05:54:43.000000 libfwsi-20240417/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10266 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfwps.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-17 05:54:43.000000 libfwsi-20240417/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-17 05:54:42.000000 libfwsi-20240417/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6400 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:43.000000 libfwsi-20240417/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-17 04:08:56.000000 libfwsi-20240417/m4/pthread.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-04-17 04:12:48.000000 libfwsi-20240417/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/include/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3262 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 04:09:35.000000 libfwsi-20240417/include/libfwsi/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-17 05:55:04.000000 libfwsi-20240417/include/libfwsi/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-04-17 04:08:52.000000 libfwsi-20240417/include/libfwsi/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25224 2024-04-17 05:54:47.000000 libfwsi-20240417/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_set.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_store.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1202 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_format_class_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_store.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_property_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_format_class_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_property_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7144 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_record.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83917 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_record.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_set.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29731 2024-04-17 05:54:47.000000 libfwsi-20240417/libfwps/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 05:54:35.000000 libfwsi-20240417/libfwps/libfwps_unused.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-17 04:08:51.000000 libfwsi-20240417/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-17 04:08:51.000000 libfwsi-20240417/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-17 04:08:51.000000 libfwsi-20240417/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-17 04:08:51.000000 libfwsi-20240417/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-17 04:08:51.000000 libfwsi-20240417/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-17 04:12:48.000000 libfwsi-20240417/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-17 04:08:51.000000 libfwsi-20240417/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-17 05:55:04.000000 libfwsi-20240417/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2024-04-17 05:54:46.000000 libfwsi-20240417/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2024-04-17 05:55:05.000000 libfwsi-20240417/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-17 04:08:51.000000 libfwsi-20240417/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-17 04:08:51.000000 libfwsi-20240417/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-17 04:08:51.000000 libfwsi-20240417/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22277 2024-04-17 05:54:47.000000 libfwsi-20240417/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27475 2024-04-17 05:54:47.000000 libfwsi-20240417/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-17 05:54:27.000000 libfwsi-20240417/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:35.000000 libfwsi-20240417/pyfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4381 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_root_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2888 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7439 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10914 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1681 2024-04-17 04:13:02.000000 libfwsi-20240417/pyfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9447 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1423 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8645 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_items.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_items.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16477 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11207 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_network_location.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_root_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15996 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1592 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22036 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62371 2024-04-17 05:54:47.000000 libfwsi-20240417/pyfwsi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-04-17 04:09:25.000000 libfwsi-20240417/pyfwsi/pyfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-04-17 04:08:54.000000 libfwsi-20240417/pyfwsi/pyfwsi_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-17 04:13:42.000000 libfwsi-20240417/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:40.000000 libfwsi-20240417/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-17 05:54:47.000000 libfwsi-20240417/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-17 04:08:56.000000 libfwsi-20240417/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-17 05:55:04.000000 libfwsi-20240417/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-17 04:08:48.000000 libfwsi-20240417/dpkg/libfwsi.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-17 05:55:04.000000 libfwsi-20240417/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-17 04:08:48.000000 libfwsi-20240417/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1560700 2024-04-17 05:54:46.000000 libfwsi-20240417/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-17 05:54:47.000000 libfwsi-20240417/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-17 05:54:47.000000 libfwsi-20240417/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfole/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfole/libfole.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfwps/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfwps/libfwps.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34936 2024-04-17 04:09:25.000000 libfwsi-20240417/msvscpp/libfwsi.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/pyfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8591 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/pyfwsi/pyfwsi.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2957 2024-04-17 04:13:50.000000 libfwsi-20240417/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5412 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15769 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfwsi/libfwsi.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_network_location_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_item/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22224 2024-04-17 05:54:47.000000 libfwsi-20240417/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_item_list/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/msvscpp/fwsi_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5204 2024-04-17 04:09:10.000000 libfwsi-20240417/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 04:08:51.000000 libfwsi-20240417/AUTHORS
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      301 2024-04-17 04:08:48.000000 libfwsi-20240417/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-17 05:54:47.000000 libfwsi-20240417/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:35.000000 libfwsi-20240417/libfwsi/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10702 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2824 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36252 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8008 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21171 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libfole.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi/libfwsi.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6785 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3733 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi/libfwsi_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11586 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1920 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7080 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_game_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2941 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13595 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4734 2024-04-17 04:14:05.000000 libfwsi-20240417/libfwsi/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17787 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12898 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52733 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_cdburn_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2383 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_web_site_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3735 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10306 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_web_site_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9361 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15636 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2059 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7535 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5814 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2465 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13461 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15825 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48490 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14142 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_uri_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libfwps.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24188 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_network_location.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16168 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_root_folder.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48575 2024-04-17 05:54:47.000000 libfwsi-20240417/libfwsi/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16451 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6198 2024-04-17 04:08:54.000000 libfwsi-20240417/libfwsi/libfwsi_users_property_view.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4141 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_item.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27275 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7576 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21723 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-17 04:08:53.000000 libfwsi-20240417/libfwsi/libfwsi_libcdata.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30221 2024-04-17 05:54:47.000000 libfwsi-20240417/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-17 05:54:25.000000 libfwsi-20240417/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-17 04:08:48.000000 libfwsi-20240417/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-17 04:08:48.000000 libfwsi-20240417/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-17 05:54:47.000000 libfwsi-20240417/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-17 04:08:48.000000 libfwsi-20240417/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-17 04:09:25.000000 libfwsi-20240417/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:40.000000 libfwsi-20240417/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-04-17 05:54:47.000000 libfwsi-20240417/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-17 05:54:30.000000 libfwsi-20240417/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-17 05:54:47.000000 libfwsi-20240417/test-driver
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-02-25 13:29:58.000000 libfwsi-20240417/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-17 04:14:14.000000 libfwsi-20240417/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22474 2024-04-17 05:54:47.000000 libfwsi-20240417/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11778 2024-04-17 04:08:55.000000 libfwsi-20240417/manuals/libfwsi.3
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_cpl_file_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0006_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0003_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_compressed_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17078 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_item.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_category_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef000a_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_item_list.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0000_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0001_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_mtp_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9733 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_delegate_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11852 2024-04-17 05:45:45.000000 libfwsi-20240417/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0025_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0014_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_cdburn_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_users_property_view_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_file_entry_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_root_folder_values.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4386 2024-04-17 04:11:21.000000 libfwsi-20240417/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_extension_block.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9818 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_control_panel_item_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_mtp_volume_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_root_folder.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0019_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0005_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_uri_sub_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0013_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_network_location.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_file_entry_extension_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_uri_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_file_entry.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_game_folder_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84392 2024-04-17 05:54:47.000000 libfwsi-20240417/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_extension_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_network_location_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/fwsi_test_item_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-17 04:08:55.000000 libfwsi-20240417/tests/fwsi_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2024-04-17 04:09:25.000000 libfwsi-20240417/tests/pyfwsi_test_item.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4761 2024-04-17 04:09:50.000000 libfwsi-20240417/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      818 2024-04-17 04:14:22.000000 libfwsi-20240417/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/ossfuzz_libfwsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/item_list_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-17 04:08:54.000000 libfwsi-20240417/ossfuzz/item_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30029 2024-04-17 05:54:47.000000 libfwsi-20240417/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-17 05:54:42.000000 libfwsi-20240417/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-17 04:08:48.000000 libfwsi-20240417/libfwsi.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:36.000000 libfwsi-20240417/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:44.000000 libfwsi-20240417/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:44.000000 libfwsi-20240417/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:44.000000 libfwsi-20240417/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:44.000000 libfwsi-20240417/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:44.000000 libfwsi-20240417/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:44.000000 libfwsi-20240417/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:44.000000 libfwsi-20240417/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:44.000000 libfwsi-20240417/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-17 05:55:04.000000 libfwsi-20240417/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:44.000000 libfwsi-20240417/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53987 2024-04-17 05:54:47.000000 libfwsi-20240417/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-17 05:54:38.000000 libfwsi-20240417/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37877 2024-04-17 05:54:47.000000 libfwsi-20240417/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:33.000000 libfwsi-20240417/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-17 05:54:29.000000 libfwsi-20240417/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-17 05:54:29.000000 libfwsi-20240417/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27344 2024-04-17 05:54:47.000000 libfwsi-20240417/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-17 05:54:28.000000 libfwsi-20240417/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:32.000000 libfwsi-20240417/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-17 05:54:26.000000 libfwsi-20240417/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26811 2024-04-17 05:54:47.000000 libfwsi-20240417/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-17 16:04:34.000000 libfwsi-20240417/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30395 2024-04-17 05:54:47.000000 libfwsi-20240417/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-17 05:54:31.000000 libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56679 2024-04-17 05:54:45.000000 libfwsi-20240417/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-17 04:08:48.000000 libfwsi-20240417/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-04-17 05:55:04.000000 libfwsi-20240417/libfwsi.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-04-17 16:04:37.411794 libfwsi-20240417/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:59.000000 libfwsi-20240423/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      661 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1407 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3793 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26787 2024-04-23 05:07:52.000000 libfwsi-20240423/libfole/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-23 05:07:38.000000 libfwsi-20240423/libfole/libfole_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-04-23 04:58:29.000000 libfwsi-20240423/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-04-23 05:07:52.000000 libfwsi-20240423/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 04:58:29.000000 libfwsi-20240423/NEWS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2593 2024-04-23 04:58:29.000000 libfwsi-20240423/libfwsi.spec.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-04-23 05:07:52.000000 libfwsi-20240423/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:59.000000 libfwsi-20240423/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26867 2024-04-23 05:07:52.000000 libfwsi-20240423/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-23 05:07:37.000000 libfwsi-20240423/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4187 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libfole.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-04-23 05:07:47.000000 libfwsi-20240423/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-04-23 05:07:47.000000 libfwsi-20240423/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10266 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libfwps.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-04-23 05:07:47.000000 libfwsi-20240423/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-04-23 05:07:47.000000 libfwsi-20240423/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-04-23 05:07:47.000000 libfwsi-20240423/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-04-20 14:07:26.000000 libfwsi-20240423/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:09:43.000000 libfwsi-20240423/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-17 04:08:56.000000 libfwsi-20240423/m4/pthread.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25612 2024-04-23 05:08:05.000000 libfwsi-20240423/include/libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-04-23 04:59:49.000000 libfwsi-20240423/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/include/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3262 2024-04-23 05:08:05.000000 libfwsi-20240423/include/libfwsi/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5015 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4884 2024-04-23 05:08:05.000000 libfwsi-20240423/include/libfwsi/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-23 04:59:49.000000 libfwsi-20240423/include/libfwsi/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6689 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1221 2024-04-23 05:08:05.000000 libfwsi-20240423/include/libfwsi/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5195 2024-04-23 04:58:32.000000 libfwsi-20240423/include/libfwsi/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25224 2024-04-23 05:07:52.000000 libfwsi-20240423/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:59.000000 libfwsi-20240423/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2490 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_set.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2104 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_store.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1202 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3827 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3731 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_format_class_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9704 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_store.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3967 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2244 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_property_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_format_class_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7534 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_property_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7144 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_record.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    83917 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_record.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16442 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_set.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29731 2024-04-23 05:07:52.000000 libfwsi-20240423/libfwps/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-23 05:07:39.000000 libfwsi-20240423/libfwps/libfwps_unused.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-04-23 04:58:32.000000 libfwsi-20240423/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-04-23 04:58:32.000000 libfwsi-20240423/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-04-23 04:58:32.000000 libfwsi-20240423/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-04-23 04:58:32.000000 libfwsi-20240423/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-04-23 04:58:32.000000 libfwsi-20240423/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-04-23 04:58:32.000000 libfwsi-20240423/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-04-23 04:58:32.000000 libfwsi-20240423/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-04-23 04:58:29.000000 libfwsi-20240423/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-04-23 04:58:32.000000 libfwsi-20240423/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-04-23 05:08:05.000000 libfwsi-20240423/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12626 2024-04-23 05:07:51.000000 libfwsi-20240423/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13364 2024-04-23 05:08:05.000000 libfwsi-20240423/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-04-23 04:58:32.000000 libfwsi-20240423/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-04-23 04:58:32.000000 libfwsi-20240423/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-04-23 04:58:32.000000 libfwsi-20240423/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22277 2024-04-23 05:07:52.000000 libfwsi-20240423/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:58.000000 libfwsi-20240423/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27475 2024-04-23 05:07:52.000000 libfwsi-20240423/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-04-23 05:07:32.000000 libfwsi-20240423/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:00.000000 libfwsi-20240423/pyfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2413 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_extension_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4381 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_control_panel_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4432 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_root_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2888 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8868 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7439 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_users_property_view.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9661 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_extension_blocks.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_control_panel_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10914 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1681 2024-04-17 04:13:02.000000 libfwsi-20240423/pyfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9447 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1423 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_compressed_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8645 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_items.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1862 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_control_panel_category.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8979 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_items.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2852 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16477 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_file_entry_extension.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11207 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1667 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_network_location.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1304 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1587 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_file_entry_extension.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5329 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_compressed_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4275 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_control_panel_category.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15996 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1592 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_users_property_view.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1493 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22036 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    62371 2024-04-23 05:07:52.000000 libfwsi-20240423/pyfwsi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11390 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1695 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-04-23 04:59:49.000000 libfwsi-20240423/pyfwsi/pyfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_extension_blocks.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-04-23 04:58:35.000000 libfwsi-20240423/pyfwsi/pyfwsi_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2024-04-17 04:13:42.000000 libfwsi-20240423/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:09:40.000000 libfwsi-20240423/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-04-23 05:07:52.000000 libfwsi-20240423/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-04-23 04:58:36.000000 libfwsi-20240423/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/libfwsi-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:57.000000 libfwsi-20240423/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1541 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      703 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-04-23 05:08:05.000000 libfwsi-20240423/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/libfwsi-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-04-23 04:58:29.000000 libfwsi-20240423/dpkg/libfwsi.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-04-23 05:08:05.000000 libfwsi-20240423/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-04-23 04:58:29.000000 libfwsi-20240423/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1560780 2024-04-23 05:07:50.000000 libfwsi-20240423/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-04-23 05:07:52.000000 libfwsi-20240423/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-04-23 05:07:52.000000 libfwsi-20240423/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_uri_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5376 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libfole/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4605 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libfole/libfole.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_game_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_compressed_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5418 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0014_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5391 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5118 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_error/fwsi_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libfwps/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6465 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libfwps/libfwps.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34936 2024-04-23 04:59:22.000000 libfwsi-20240423/msvscpp/libfwsi.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0019_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/pyfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8591 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/pyfwsi/pyfwsi.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2957 2024-04-23 04:59:22.000000 libfwsi-20240423/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_mtp_volume_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5397 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_root_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5400 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_cdburn_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5385 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0001_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0025_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_uri_sub_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5388 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_delegate_folder_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5412 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_category_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_item_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5421 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15769 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libfwsi/libfwsi.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_network_location_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5415 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_cpl_file_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5433 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0000_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_users_property_view_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5424 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0006_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5124 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_support/fwsi_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_file_entry_extension_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5427 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_item/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5358 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_item/fwsi_test_item.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_mtp_file_entry_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5409 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0013_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22224 2024-04-23 05:07:52.000000 libfwsi-20240423/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef000a_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_item_list/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5373 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0005_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0003_values/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5445 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/msvscpp/fwsi_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5204 2024-04-23 04:58:56.000000 libfwsi-20240423/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-23 04:58:32.000000 libfwsi-20240423/AUTHORS
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      301 2024-04-23 04:58:29.000000 libfwsi-20240423/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-04-23 05:07:52.000000 libfwsi-20240423/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:00.000000 libfwsi-20240423/libfwsi/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1888 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_cpl_file_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10702 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_compressed_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2824 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_category.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1076 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36252 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_known_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8008 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_delegate_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1609 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_uri_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0001_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21171 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0000_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1274 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libfole.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1771 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_users_property_view.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5770 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12685 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0003_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6750 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1074 2024-04-23 05:08:05.000000 libfwsi-20240423/libfwsi/libfwsi.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6785 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3733 2024-04-23 05:08:05.000000 libfwsi-20240423/libfwsi/libfwsi_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1377 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0013_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11586 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_known_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1395 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1920 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_compressed_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6330 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0027_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5972 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7080 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0026_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0025_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1712 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_game_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2941 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0014_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_category_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0029_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16884 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1578 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0006_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9231 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1762 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_root_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2305 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_extension_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13595 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_users_property_view_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4734 2024-04-17 04:14:05.000000 libfwsi-20240423/libfwsi/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5986 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0013_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6191 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0006_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17787 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11512 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1129 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12898 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_acronis_tib_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_category.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1348 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_root_folder.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52733 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_shell_folder_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5555 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0029_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1633 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_cdburn_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1673 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_uri_sub_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2139 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2421 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_item_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8940 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_cpl_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef000a_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2001 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0027_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5435 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_mtp_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2383 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_users_property_view_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2317 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6230 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0026_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2133 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_network_location_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_web_site_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16822 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_extension_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2742 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_acronis_tib_file_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3735 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26408 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_extension.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10306 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_web_site_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9361 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6603 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15636 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0019_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2059 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7535 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2666 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_compressed_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5814 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2465 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13461 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15825 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48490 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3228 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_volume_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3347 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2794 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14142 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_uri_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libfwps.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1723 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5656 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_file_entry_extension.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5798 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_root_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24188 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_network_location.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3432 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_network_location.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16168 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_mtp_file_entry_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3149 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_root_folder.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48575 2024-04-23 05:07:52.000000 libfwsi-20240423/libfwsi/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1963 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_delegate_folder_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0005_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16451 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_shell_folder_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6198 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_users_property_view.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4141 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_item.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27275 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7576 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5525 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0001_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21723 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_control_panel_item_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-04-23 04:58:34.000000 libfwsi-20240423/libfwsi/libfwsi_libcdata.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:58.000000 libfwsi-20240423/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30221 2024-04-23 05:07:52.000000 libfwsi-20240423/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-04-23 05:07:29.000000 libfwsi-20240423/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-04-23 04:58:29.000000 libfwsi-20240423/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-23 04:58:29.000000 libfwsi-20240423/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-04-23 05:07:52.000000 libfwsi-20240423/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-04-23 04:58:29.000000 libfwsi-20240423/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      752 2024-04-23 04:59:31.000000 libfwsi-20240423/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:09:40.000000 libfwsi-20240423/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:58.000000 libfwsi-20240423/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-04-23 05:07:52.000000 libfwsi-20240423/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-04-23 05:07:34.000000 libfwsi-20240423/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-04-23 05:07:52.000000 libfwsi-20240423/test-driver
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3395 2024-02-25 13:29:58.000000 libfwsi-20240423/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       97 2024-04-17 04:14:14.000000 libfwsi-20240423/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22474 2024-04-23 05:07:52.000000 libfwsi-20240423/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11778 2024-04-23 04:58:36.000000 libfwsi-20240423/manuals/libfwsi.3
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11887 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_control_panel_cpl_file_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10440 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0006_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10428 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0003_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6792 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_compressed_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17078 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_item.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7077 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_control_panel_category_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef000a_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_item_list.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2056 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10355 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0000_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0001_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13523 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_mtp_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9733 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_delegate_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11852 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10452 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0025_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12033 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0014_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9691 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_cdburn_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10058 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_users_property_view_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9508 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_file_entry_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9072 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_root_folder_values.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4405 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1426 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_extension_block.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9818 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_control_panel_item_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8871 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16618 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_mtp_volume_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1414 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_root_folder.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0019_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7305 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0005_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6222 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_uri_sub_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10525 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0013_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_network_location.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1190 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10376 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_file_entry_extension_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10824 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_uri_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_file_entry.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9145 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_game_folder_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84392 2024-04-23 05:07:52.000000 libfwsi-20240423/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11361 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_extension_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9721 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_network_location_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15227 2024-04-23 04:59:22.000000 libfwsi-20240423/tests/fwsi_test_item_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-04-23 04:58:36.000000 libfwsi-20240423/tests/fwsi_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1394 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/pyfwsi_test_item.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4761 2024-04-23 05:00:05.000000 libfwsi-20240423/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      818 2024-04-17 04:14:22.000000 libfwsi-20240423/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-04-23 04:58:34.000000 libfwsi-20240423/ossfuzz/ossfuzz_libfwsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1375 2024-04-23 04:58:34.000000 libfwsi-20240423/ossfuzz/item_list_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1330 2024-04-23 04:58:34.000000 libfwsi-20240423/ossfuzz/item_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30029 2024-04-23 05:07:52.000000 libfwsi-20240423/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-04-23 05:07:47.000000 libfwsi-20240423/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-04-23 04:58:29.000000 libfwsi-20240423/libfwsi.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:26:01.000000 libfwsi-20240423/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:09:44.000000 libfwsi-20240423/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:09:44.000000 libfwsi-20240423/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:09:44.000000 libfwsi-20240423/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:09:44.000000 libfwsi-20240423/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:09:44.000000 libfwsi-20240423/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:09:44.000000 libfwsi-20240423/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:09:44.000000 libfwsi-20240423/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:09:44.000000 libfwsi-20240423/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:09:44.000000 libfwsi-20240423/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-04-23 05:08:05.000000 libfwsi-20240423/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:09:44.000000 libfwsi-20240423/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:09:44.000000 libfwsi-20240423/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:59.000000 libfwsi-20240423/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53987 2024-04-23 05:07:52.000000 libfwsi-20240423/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-04-23 05:07:42.000000 libfwsi-20240423/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37877 2024-04-23 05:07:52.000000 libfwsi-20240423/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:58.000000 libfwsi-20240423/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27344 2024-04-23 05:07:52.000000 libfwsi-20240423/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-04-23 05:07:33.000000 libfwsi-20240423/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:58.000000 libfwsi-20240423/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-04-23 05:07:31.000000 libfwsi-20240423/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26811 2024-04-23 05:07:52.000000 libfwsi-20240423/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-04-23 05:25:59.000000 libfwsi-20240423/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30395 2024-04-23 05:07:52.000000 libfwsi-20240423/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-04-23 05:07:36.000000 libfwsi-20240423/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56679 2024-04-23 05:07:49.000000 libfwsi-20240423/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5751 2024-04-23 04:58:29.000000 libfwsi-20240423/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1956 2024-04-23 05:08:05.000000 libfwsi-20240423/libfwsi.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-04-23 05:26:02.408759 libfwsi-20240423/PKG-INFO
```

### Comparing `libfwsi-20240417/libfole/libfole_value_type.h` & `libfwsi-20240423/libfole/libfole_value_type.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_error.c` & `libfwsi-20240423/libfole/libfole_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/Makefile.am` & `libfwsi-20240423/libfole/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_definitions.h` & `libfwsi-20240423/libfole/libfole_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_error.h` & `libfwsi-20240423/libfole/libfole_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_support.h` & `libfwsi-20240423/libfole/libfole_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_types.h` & `libfwsi-20240423/libfole/libfole_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_support.c` & `libfwsi-20240423/libfole/libfole_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_value_type.c` & `libfwsi-20240423/libfole/libfole_value_type.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_unused.h` & `libfwsi-20240423/libfole/libfole_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_libcerror.h` & `libfwsi-20240423/libfole/libfole_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/Makefile.in` & `libfwsi-20240423/libfole/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfole/libfole_extern.h` & `libfwsi-20240423/libfole/libfole_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/COPYING` & `libfwsi-20240423/COPYING`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/install-sh` & `libfwsi-20240423/install-sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi.spec.in` & `libfwsi-20240423/libfwsi.spec.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/depcomp` & `libfwsi-20240423/depcomp`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_error.c` & `libfwsi-20240423/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_support.h` & `libfwsi-20240423/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_identifier.h` & `libfwsi-20240423/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_libcerror.h` & `libfwsi-20240423/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/Makefile.am` & `libfwsi-20240423/libfguid/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_unused.h` & `libfwsi-20240423/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_extern.h` & `libfwsi-20240423/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_types.h` & `libfwsi-20240423/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_identifier.c` & `libfwsi-20240423/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_support.c` & `libfwsi-20240423/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_definitions.h` & `libfwsi-20240423/libfguid/libfguid_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/Makefile.in` & `libfwsi-20240423/libfguid/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfguid/libfguid_error.h` & `libfwsi-20240423/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libfdatetime.m4` & `libfwsi-20240423/m4/libfdatetime.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/tests.m4` & `libfwsi-20240423/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/lib-prefix.m4` & `libfwsi-20240423/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/progtest.m4` & `libfwsi-20240423/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libuna.m4` & `libfwsi-20240423/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/gettext.m4` & `libfwsi-20240423/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/lib-ld.m4` & `libfwsi-20240423/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libfole.m4` & `libfwsi-20240423/m4/libfole.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libclocale.m4` & `libfwsi-20240423/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libcdata.m4` & `libfwsi-20240423/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/common.m4` & `libfwsi-20240423/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libcthreads.m4` & `libfwsi-20240423/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/ltversion.m4` & `libfwsi-20240423/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/ltsugar.m4` & `libfwsi-20240423/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/host-cpu-c-abi.m4` & `libfwsi-20240423/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libfwps.m4` & `libfwsi-20240423/m4/libfwps.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libtool.m4` & `libfwsi-20240423/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/po.m4` & `libfwsi-20240423/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libcerror.m4` & `libfwsi-20240423/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libcnotify.m4` & `libfwsi-20240423/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/libfguid.m4` & `libfwsi-20240423/m4/libfguid.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/intlmacosx.m4` & `libfwsi-20240423/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/lt~obsolete.m4` & `libfwsi-20240423/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/lib-link.m4` & `libfwsi-20240423/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/iconv.m4` & `libfwsi-20240423/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/ltoptions.m4` & `libfwsi-20240423/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/nls.m4` & `libfwsi-20240423/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/python.m4` & `libfwsi-20240423/m4/python.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20240416
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -74,17 +74,18 @@
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
     dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
-      [mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libfwsi-20240417/m4/types.m4` & `libfwsi-20240423/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/m4/pthread.m4` & `libfwsi-20240423/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi.h.in` & `libfwsi-20240423/include/libfwsi.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi.h` & `libfwsi-20240423/include/libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/definitions.h.in` & `libfwsi-20240423/include/libfwsi/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/definitions.h` & `libfwsi-20240423/include/libfwsi/definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBFWSI_DEFINITIONS_H )
 #define _LIBFWSI_DEFINITIONS_H
 
 #include <libfwsi/types.h>
 
-#define LIBFWSI_VERSION					20240417
+#define LIBFWSI_VERSION					20240423
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20240417"
+#define LIBFWSI_VERSION_STRING				"20240423"
 
 /* The byte order definitions
  */
 enum LIBFWSI_ENDIAN
 {
 	LIBFWSI_ENDIAN_BIG				= (int) 'b',
 	LIBFWSI_ENDIAN_LITTLE				= (int) 'l'
```

### Comparing `libfwsi-20240417/include/libfwsi/types.h.in` & `libfwsi-20240423/include/libfwsi/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/types.h` & `libfwsi-20240423/include/libfwsi/types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/features.h.in` & `libfwsi-20240423/include/libfwsi/features.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/error.h` & `libfwsi-20240423/include/libfwsi/error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/extern.h` & `libfwsi-20240423/include/libfwsi/extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/features.h` & `libfwsi-20240423/include/libfwsi/features.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/libfwsi/codepage.h` & `libfwsi-20240423/include/libfwsi/codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/include/Makefile.in` & `libfwsi-20240423/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_set.h` & `libfwsi-20240423/libfwps/libfwps_set.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_types.h` & `libfwsi-20240423/libfwps/libfwps_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_notify.h` & `libfwsi-20240423/libfwps/libfwps_notify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_libfguid.h` & `libfwsi-20240423/libfwps/libfwps_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_libcerror.h` & `libfwsi-20240423/libfwps/libfwps_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_libcnotify.h` & `libfwsi-20240423/libfwps/libfwps_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_store.h` & `libfwsi-20240423/libfwps/libfwps_store.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_libcdata.h` & `libfwsi-20240423/libfwps/libfwps_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_debug.h` & `libfwsi-20240423/libfwps/libfwps_debug.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_error.c` & `libfwsi-20240423/libfwps/libfwps_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/Makefile.am` & `libfwsi-20240423/libfwps/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_definitions.h` & `libfwsi-20240423/libfwps/libfwps_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_notify.c` & `libfwsi-20240423/libfwps/libfwps_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_error.h` & `libfwsi-20240423/libfwps/libfwps_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_libuna.h` & `libfwsi-20240423/libfwps/libfwps_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_support.h` & `libfwsi-20240423/libfwps/libfwps_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_format_class_identifier.c` & `libfwsi-20240423/libfwps/libfwps_format_class_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_codepage.h` & `libfwsi-20240423/libfwps/libfwps_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_support.c` & `libfwsi-20240423/libfwps/libfwps_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_extern.h` & `libfwsi-20240423/libfwps/libfwps_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_store.c` & `libfwsi-20240423/libfwps/libfwps_store.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_debug.c` & `libfwsi-20240423/libfwps/libfwps_debug.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_property_identifier.h` & `libfwsi-20240423/libfwps/libfwps_property_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_format_class_identifier.h` & `libfwsi-20240423/libfwps/libfwps_format_class_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_property_identifier.c` & `libfwsi-20240423/libfwps/libfwps_property_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_record.h` & `libfwsi-20240423/libfwps/libfwps_record.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_record.c` & `libfwsi-20240423/libfwps/libfwps_record.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_set.c` & `libfwsi-20240423/libfwps/libfwps_set.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/Makefile.in` & `libfwsi-20240423/libfwps/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwps/libfwps_unused.h` & `libfwsi-20240423/libfwps/libfwps_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/config_borlandc.h` & `libfwsi-20240423/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/file_stream.h` & `libfwsi-20240423/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/memory.h` & `libfwsi-20240423/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/byte_stream.h` & `libfwsi-20240423/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/common.h` & `libfwsi-20240423/common/common.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/config_winapi.h` & `libfwsi-20240423/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/system_string.h` & `libfwsi-20240423/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/types.h.in` & `libfwsi-20240423/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/types.h` & `libfwsi-20240423/common/types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/config.h.in` & `libfwsi-20240423/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/config.h` & `libfwsi-20240423/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -403,24 +403,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfwsi"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfwsi 20240417"
+#define PACKAGE_STRING "libfwsi 20240423"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfwsi"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240417"
+#define PACKAGE_VERSION "20240423"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -438,15 +438,15 @@
    backward compatibility; new code need not use it. */
 #define STDC_HEADERS 1
 
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Version number of package */
-#define VERSION "20240417"
+#define VERSION "20240423"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libfwsi-20240417/common/wide_string.h` & `libfwsi-20240423/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/narrow_string.h` & `libfwsi-20240423/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/config_msc.h` & `libfwsi-20240423/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/common/Makefile.in` & `libfwsi-20240423/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_wide_string.c` & `libfwsi-20240423/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_support.h` & `libfwsi-20240423/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/Makefile.am` & `libfwsi-20240423/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_definitions.h` & `libfwsi-20240423/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_unused.h` & `libfwsi-20240423/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_libcerror.h` & `libfwsi-20240423/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_locale.h` & `libfwsi-20240423/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_support.c` & `libfwsi-20240423/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_codepage.c` & `libfwsi-20240423/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_locale.c` & `libfwsi-20240423/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/Makefile.in` & `libfwsi-20240423/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_extern.h` & `libfwsi-20240423/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_wide_string.h` & `libfwsi-20240423/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libclocale/libclocale_codepage.h` & `libfwsi-20240423/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_codepage.c` & `libfwsi-20240423/pyfwsi/pyfwsi_codepage.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_extension_block.h` & `libfwsi-20240423/pyfwsi/pyfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.c` & `libfwsi-20240423/pyfwsi/pyfwsi_control_panel_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_root_folder.c` & `libfwsi-20240423/pyfwsi/pyfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_item.h` & `libfwsi-20240423/pyfwsi/pyfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_string.c` & `libfwsi-20240423/pyfwsi/pyfwsi_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.c` & `libfwsi-20240423/pyfwsi/pyfwsi_users_property_view.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_integer.h` & `libfwsi-20240423/pyfwsi/pyfwsi_integer.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.c` & `libfwsi-20240423/pyfwsi/pyfwsi_extension_blocks.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_item.h` & `libfwsi-20240423/pyfwsi/pyfwsi_control_panel_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_libclocale.h` & `libfwsi-20240423/pyfwsi/pyfwsi_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_network_location.c` & `libfwsi-20240423/pyfwsi/pyfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_codepage.h` & `libfwsi-20240423/pyfwsi/pyfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_datetime.h` & `libfwsi-20240423/pyfwsi/pyfwsi_datetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/Makefile.am` & `libfwsi-20240423/pyfwsi/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi.c` & `libfwsi-20240423/pyfwsi/pyfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_error.h` & `libfwsi-20240423/pyfwsi/pyfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.h` & `libfwsi-20240423/pyfwsi/pyfwsi_compressed_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_volume.c` & `libfwsi-20240423/pyfwsi/pyfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_items.h` & `libfwsi-20240423/pyfwsi/pyfwsi_items.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_file_entry.h` & `libfwsi-20240423/pyfwsi/pyfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.h` & `libfwsi-20240423/pyfwsi/pyfwsi_control_panel_category.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_items.c` & `libfwsi-20240423/pyfwsi/pyfwsi_items.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_guid.c` & `libfwsi-20240423/pyfwsi/pyfwsi_guid.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.c` & `libfwsi-20240423/pyfwsi/pyfwsi_file_entry_extension.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_extension_block.c` & `libfwsi-20240423/pyfwsi/pyfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_network_location.h` & `libfwsi-20240423/pyfwsi/pyfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_error.c` & `libfwsi-20240423/pyfwsi/pyfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi.h` & `libfwsi-20240423/pyfwsi/pyfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_integer.c` & `libfwsi-20240423/pyfwsi/pyfwsi_integer.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_volume.h` & `libfwsi-20240423/pyfwsi/pyfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_unused.h` & `libfwsi-20240423/pyfwsi/pyfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_root_folder.h` & `libfwsi-20240423/pyfwsi/pyfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_file_entry_extension.h` & `libfwsi-20240423/pyfwsi/pyfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_libcerror.h` & `libfwsi-20240423/pyfwsi/pyfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_python.h` & `libfwsi-20240423/pyfwsi/pyfwsi_python.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_compressed_folder.c` & `libfwsi-20240423/pyfwsi/pyfwsi_compressed_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_libfguid.h` & `libfwsi-20240423/pyfwsi/pyfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_control_panel_category.c` & `libfwsi-20240423/pyfwsi/pyfwsi_control_panel_category.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_libfwsi.h` & `libfwsi-20240423/pyfwsi/pyfwsi_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_item_list.c` & `libfwsi-20240423/pyfwsi/pyfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_users_property_view.h` & `libfwsi-20240423/pyfwsi/pyfwsi_users_property_view.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_string.h` & `libfwsi-20240423/pyfwsi/pyfwsi_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_item.c` & `libfwsi-20240423/pyfwsi/pyfwsi_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_guid.h` & `libfwsi-20240423/pyfwsi/pyfwsi_guid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/Makefile.in` & `libfwsi-20240423/pyfwsi/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_file_entry.c` & `libfwsi-20240423/pyfwsi/pyfwsi_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_libuna.h` & `libfwsi-20240423/pyfwsi/pyfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_item_list.h` & `libfwsi-20240423/pyfwsi/pyfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_extension_blocks.h` & `libfwsi-20240423/pyfwsi/pyfwsi_extension_blocks.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/pyfwsi/pyfwsi_datetime.c` & `libfwsi-20240423/pyfwsi/pyfwsi_datetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/Makefile.am` & `libfwsi-20240423/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/config.guess` & `libfwsi-20240423/config.guess`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/dpkg/copyright` & `libfwsi-20240423/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/dpkg/control` & `libfwsi-20240423/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/dpkg/rules` & `libfwsi-20240423/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/COPYING.LESSER` & `libfwsi-20240423/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/configure` & `libfwsi-20240423/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfwsi 20240417.
+# Generated by GNU Autoconf 2.71 for libfwsi 20240423.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libfwsi'
 PACKAGE_TARNAME='libfwsi'
-PACKAGE_VERSION='20240417'
-PACKAGE_STRING='libfwsi 20240417'
+PACKAGE_VERSION='20240423'
+PACKAGE_STRING='libfwsi 20240423'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfwsi.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1580,15 +1580,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfwsi 20240417 to adapt to many kinds of systems.
+\`configure' configures libfwsi 20240423 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1651,15 +1651,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfwsi 20240417:";;
+     short | recursive ) echo "Configuration of libfwsi 20240423:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1864,15 +1864,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfwsi configure 20240417
+libfwsi configure 20240423
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2585,15 +2585,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfwsi $as_me 20240417, which was
+It was created by libfwsi $as_me 20240423, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4074,15 +4074,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfwsi'
- VERSION='20240417'
+ VERSION='20240423'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -46314,18 +46314,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
-  mingw*) :
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -47260,15 +47262,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfwsi $as_me 20240417, which was
+This file was extended by libfwsi $as_me 20240423, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -47328,15 +47330,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfwsi config.status 20240417
+libfwsi config.status 20240423
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfwsi-20240417/compile` & `libfwsi-20240423/compile`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/missing` & `libfwsi-20240423/missing`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_file_entry_values/fwsi_test_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_uri_values/fwsi_test_uri_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfole/libfole.vcproj` & `libfwsi-20240423/msvscpp/libfole/libfole.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_game_folder_values/fwsi_test_game_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_volume_values/fwsi_test_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_compressed_folder_values/fwsi_test_compressed_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0014_values/fwsi_test_extension_block_0xbeef0014_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfguid/libfguid.vcproj` & `libfwsi-20240423/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block/fwsi_test_extension_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_error/fwsi_test_error.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_error/fwsi_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfwps/libfwps.vcproj` & `libfwsi-20240423/msvscpp/libfwps/libfwps.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfwsi.sln` & `libfwsi-20240423/msvscpp/libfwsi.sln`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0019_values/fwsi_test_extension_block_0xbeef0019_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libclocale/libclocale.vcproj` & `libfwsi-20240423/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/pyfwsi/pyfwsi.vcproj` & `libfwsi-20240423/msvscpp/pyfwsi/pyfwsi.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/Makefile.am` & `libfwsi-20240423/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_mtp_volume_values/fwsi_test_mtp_volume_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_root_folder_values/fwsi_test_root_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_cdburn_values/fwsi_test_cdburn_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0001_values/fwsi_test_extension_block_0xbeef0001_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0025_values/fwsi_test_extension_block_0xbeef0025_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_uri_sub_values/fwsi_test_uri_sub_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_delegate_folder_values/fwsi_test_delegate_folder_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_control_panel_category_values/fwsi_test_control_panel_category_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_control_panel_item_values/fwsi_test_control_panel_item_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfwsi/libfwsi.vcproj` & `libfwsi-20240423/msvscpp/libfwsi/libfwsi.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libcdata/libcdata.vcproj` & `libfwsi-20240423/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_network_location_values/fwsi_test_network_location_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_control_panel_cpl_file_values/fwsi_test_control_panel_cpl_file_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0000_values/fwsi_test_extension_block_0xbeef0000_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_users_property_view_values/fwsi_test_users_property_view_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0006_values/fwsi_test_extension_block_0xbeef0006_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_support/fwsi_test_support.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_support/fwsi_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libcthreads/libcthreads.vcproj` & `libfwsi-20240423/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_file_entry_extension_values/fwsi_test_file_entry_extension_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_item/fwsi_test_item.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_item/fwsi_test_item.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_mtp_file_entry_values/fwsi_test_mtp_file_entry_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0013_values/fwsi_test_extension_block_0xbeef0013_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libuna/libuna.vcproj` & `libfwsi-20240423/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/Makefile.in` & `libfwsi-20240423/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef000a_values/fwsi_test_extension_block_0xbeef000a_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libcnotify/libcnotify.vcproj` & `libfwsi-20240423/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libcerror/libcerror.vcproj` & `libfwsi-20240423/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/libfdatetime/libfdatetime.vcproj` & `libfwsi-20240423/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_item_list/fwsi_test_item_list.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0005_values/fwsi_test_extension_block_0xbeef0005_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_extension_block_0xbeef0003_values/fwsi_test_extension_block_0xbeef0003_values.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj` & `libfwsi-20240423/msvscpp/fwsi_test_notify/fwsi_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/INSTALL` & `libfwsi-20240423/INSTALL`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libcerror.h` & `libfwsi-20240423/libfwsi/libfwsi_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_cpl_file_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_compressed_folder.c` & `libfwsi-20240423/libfwsi/libfwsi_compressed_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_category.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_category.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_types.h` & `libfwsi-20240423/libfwsi/libfwsi_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi.rc.in` & `libfwsi-20240423/libfwsi/libfwsi.rc.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extern.h` & `libfwsi-20240423/libfwsi/libfwsi_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.c` & `libfwsi-20240423/libfwsi/libfwsi_known_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.c` & `libfwsi-20240423/libfwsi/libfwsi_delegate_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_uri_values.h` & `libfwsi-20240423/libfwsi/libfwsi_uri_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0001_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_values.c` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0000_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_error.h` & `libfwsi-20240423/libfwsi/libfwsi_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libfole.h` & `libfwsi-20240423/libfwsi/libfwsi_libfole.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_users_property_view.h` & `libfwsi-20240423/libfwsi/libfwsi_users_property_view.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_game_folder_values.c` & `libfwsi-20240423/libfwsi/libfwsi_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_item_list.c` & `libfwsi-20240423/libfwsi/libfwsi_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0003_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.c` & `libfwsi-20240423/libfwsi/libfwsi_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi.rc` & `libfwsi-20240423/libfwsi/libfwsi.rc`

 * *Files 11% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Windows Shell Item format\0"
-      VALUE "FileVersion",		"20240417" "\0"
+      VALUE "FileVersion",		"20240423" "\0"
       VALUE "InternalName",		"libfwsi.dll\0"
       VALUE "LegalCopyright",		"(C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfwsi.dll\0"
       VALUE "ProductName",		"libfwsi\0"
-      VALUE "ProductVersion",		"20240417" "\0"
+      VALUE "ProductVersion",		"20240423" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfwsi/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0000_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_definitions.h` & `libfwsi-20240423/libfwsi/libfwsi_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfwsi/definitions.h> are copied here
  * for local use of libfwsi
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFWSI_VERSION					20240417
+#define LIBFWSI_VERSION					20240423
 
 /* The version string
  */
-#define LIBFWSI_VERSION_STRING				"20240417"
+#define LIBFWSI_VERSION_STRING				"20240423"
 
 /* The byte order definitions
  */
 #define LIBFWSI_ENDIAN_BIG				_BYTE_STREAM_ENDIAN_BIG
 #define LIBFWSI_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The item type definitions
```

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0013_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_known_folder_identifier.h` & `libfwsi-20240423/libfwsi/libfwsi_known_folder_identifier.h`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFWSI_SHELL_FOLDER_IDENTIFIER_H )
-#define _LIBFWSI_SHELL_FOLDER_IDENTIFIER_H
+#if !defined( _LIBFWSI_KNOWN_FOLDER_IDENTIFIER_H )
+#define _LIBFWSI_KNOWN_FOLDER_IDENTIFIER_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libfwsi_extern.h"
 #include "libfwsi_libcerror.h"
 
@@ -199,9 +199,9 @@
 const char *libfwsi_known_folder_identifier_get_name(
              const uint8_t *known_folder_identifier );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBFWSI_SHELL_FOLDER_IDENTIFIER_H ) */
+#endif /* !defined( _LIBFWSI_KNOWN_FOLDER_IDENTIFIER_H ) */
```

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libfguid.h` & `libfwsi-20240423/libfwsi/libfwsi_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_compressed_folder.h` & `libfwsi-20240423/libfwsi/libfwsi_compressed_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0027_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0003_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_support.h` & `libfwsi-20240423/libfwsi/libfwsi_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0026_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0025_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_game_folder_values.h` & `libfwsi-20240423/libfwsi/libfwsi_game_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_values.h` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0014_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_category_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0029_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.c` & `libfwsi-20240423/libfwsi/libfwsi_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_notify.h` & `libfwsi-20240423/libfwsi/libfwsi_notify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_attributes.h` & `libfwsi-20240423/libfwsi/libfwsi_file_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0006_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0014_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_root_folder_values.h` & `libfwsi-20240423/libfwsi/libfwsi_root_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.h` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_extension_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.c` & `libfwsi-20240423/libfwsi/libfwsi_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/Makefile.am` & `libfwsi-20240423/libfwsi/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0013_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0006_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.c` & `libfwsi-20240423/libfwsi/libfwsi_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry.c` & `libfwsi-20240423/libfwsi/libfwsi_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_support.c` & `libfwsi-20240423/libfwsi/libfwsi_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.c` & `libfwsi-20240423/libfwsi/libfwsi_acronis_tib_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_category.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_category.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_root_folder.h` & `libfwsi-20240423/libfwsi/libfwsi_root_folder.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_unused.h` & `libfwsi-20240423/libfwsi/libfwsi_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.c` & `libfwsi-20240423/libfwsi/libfwsi_shell_folder_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0029_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0029_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_cdburn_values.h` & `libfwsi-20240423/libfwsi/libfwsi_cdburn_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_uri_sub_values.h` & `libfwsi-20240423/libfwsi/libfwsi_uri_sub_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_volume.h` & `libfwsi-20240423/libfwsi/libfwsi_volume.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_item_list.h` & `libfwsi-20240423/libfwsi/libfwsi_item_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_cpl_file_values.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef000a_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0027_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0027_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_mtp_volume_values.h` & `libfwsi-20240423/libfwsi/libfwsi_mtp_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_users_property_view_values.h` & `libfwsi-20240423/libfwsi/libfwsi_users_property_view_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry.h` & `libfwsi-20240423/libfwsi/libfwsi_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0026_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0026_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_error.c` & `libfwsi-20240423/libfwsi/libfwsi_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_network_location_values.h` & `libfwsi-20240423/libfwsi/libfwsi_network_location_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_web_site_values.h` & `libfwsi-20240423/libfwsi/libfwsi_web_site_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension_values.c` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_notify.c` & `libfwsi-20240423/libfwsi/libfwsi_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_acronis_tib_file_values.h` & `libfwsi-20240423/libfwsi/libfwsi_acronis_tib_file_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_definitions.h.in` & `libfwsi-20240423/libfwsi/libfwsi_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_codepage.h` & `libfwsi-20240423/libfwsi/libfwsi_codepage.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.c` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_extension.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_web_site_values.c` & `libfwsi-20240423/libfwsi/libfwsi_web_site_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_volume.c` & `libfwsi-20240423/libfwsi/libfwsi_volume.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0025_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.c` & `libfwsi-20240423/libfwsi/libfwsi_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0019_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0019_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_values.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_compressed_folder_values.h` & `libfwsi-20240423/libfwsi/libfwsi_compressed_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_cdburn_values.c` & `libfwsi-20240423/libfwsi/libfwsi_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_category_values.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_network_location_values.c` & `libfwsi-20240423/libfwsi/libfwsi_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_debug.c` & `libfwsi-20240423/libfwsi/libfwsi_debug.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_item.c` & `libfwsi-20240423/libfwsi/libfwsi_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_volume_values.h` & `libfwsi-20240423/libfwsi/libfwsi_volume_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_attributes.c` & `libfwsi-20240423/libfwsi/libfwsi_file_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_debug.h` & `libfwsi-20240423/libfwsi/libfwsi_debug.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_uri_values.c` & `libfwsi-20240423/libfwsi/libfwsi_uri_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libfwps.h` & `libfwsi-20240423/libfwsi/libfwsi_libfwps.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libfdatetime.h` & `libfwsi-20240423/libfwsi/libfwsi_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef000a_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_file_entry_extension.h` & `libfwsi-20240423/libfwsi/libfwsi_file_entry_extension.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_root_folder_values.c` & `libfwsi-20240423/libfwsi/libfwsi_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_network_location.c` & `libfwsi-20240423/libfwsi/libfwsi_network_location.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_network_location.h` & `libfwsi-20240423/libfwsi/libfwsi_network_location.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_volume_values.c` & `libfwsi-20240423/libfwsi/libfwsi_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi.c` & `libfwsi-20240423/libfwsi/libfwsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libuna.h` & `libfwsi-20240423/libfwsi/libfwsi_libuna.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_mtp_file_entry_values.h` & `libfwsi-20240423/libfwsi/libfwsi_mtp_file_entry_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_root_folder.c` & `libfwsi-20240423/libfwsi/libfwsi_root_folder.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/Makefile.in` & `libfwsi-20240423/libfwsi/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_delegate_folder_values.h` & `libfwsi-20240423/libfwsi/libfwsi_delegate_folder_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libcnotify.h` & `libfwsi-20240423/libfwsi/libfwsi_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0005_values.h` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0005_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_shell_folder_identifier.h` & `libfwsi-20240423/libfwsi/libfwsi_shell_folder_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_users_property_view.c` & `libfwsi-20240423/libfwsi/libfwsi_users_property_view.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_item.h` & `libfwsi-20240423/libfwsi/libfwsi_item.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.h` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item_identifier.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_extension_block_0xbeef0001_values.c` & `libfwsi-20240423/libfwsi/libfwsi_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_control_panel_item_identifier.c` & `libfwsi-20240423/libfwsi/libfwsi_control_panel_item_identifier.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfwsi/libfwsi_libcdata.h` & `libfwsi-20240423/libfwsi/libfwsi_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_list_element.h` & `libfwsi-20240423/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_array.h` & `libfwsi-20240423/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_definitions.h` & `libfwsi-20240423/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_libcerror.h` & `libfwsi-20240423/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_unused.h` & `libfwsi-20240423/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree.h` & `libfwsi-20240423/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree.c` & `libfwsi-20240423/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_support.c` & `libfwsi-20240423/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_list.c` & `libfwsi-20240423/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_extern.h` & `libfwsi-20240423/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_list.h` & `libfwsi-20240423/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree_values_list.h` & `libfwsi-20240423/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/Makefile.am` & `libfwsi-20240423/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree_node.h` & `libfwsi-20240423/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_range_list_value.h` & `libfwsi-20240423/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_range_list.h` & `libfwsi-20240423/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_range_list.c` & `libfwsi-20240423/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_array.c` & `libfwsi-20240423/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_list_element.c` & `libfwsi-20240423/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_libcthreads.h` & `libfwsi-20240423/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_tree_node.h` & `libfwsi-20240423/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_error.h` & `libfwsi-20240423/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_types.h` & `libfwsi-20240423/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree_node.c` & `libfwsi-20240423/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_tree_node.c` & `libfwsi-20240423/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_support.h` & `libfwsi-20240423/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/Makefile.in` & `libfwsi-20240423/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_range_list_value.c` & `libfwsi-20240423/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_btree_values_list.c` & `libfwsi-20240423/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcdata/libcdata_error.c` & `libfwsi-20240423/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/config.sub` & `libfwsi-20240423/config.sub`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/setup.py` & `libfwsi-20240423/setup.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/acinclude.m4` & `libfwsi-20240423/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/config.rpath` & `libfwsi-20240423/config.rpath`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread.h` & `libfwsi-20240423/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_read_write_lock.h` & `libfwsi-20240423/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread.c` & `libfwsi-20240423/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread_pool.h` & `libfwsi-20240423/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_support.h` & `libfwsi-20240423/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_lock.h` & `libfwsi-20240423/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_unused.h` & `libfwsi-20240423/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_lock.c` & `libfwsi-20240423/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_condition.h` & `libfwsi-20240423/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_repeating_thread.h` & `libfwsi-20240423/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/Makefile.am` & `libfwsi-20240423/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_support.c` & `libfwsi-20240423/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_mutex.c` & `libfwsi-20240423/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_queue.c` & `libfwsi-20240423/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_mutex.h` & `libfwsi-20240423/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_types.h` & `libfwsi-20240423/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread_attributes.h` & `libfwsi-20240423/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_condition.c` & `libfwsi-20240423/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_error.c` & `libfwsi-20240423/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_read_write_lock.c` & `libfwsi-20240423/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_libcerror.h` & `libfwsi-20240423/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_definitions.h` & `libfwsi-20240423/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread_pool.c` & `libfwsi-20240423/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_error.h` & `libfwsi-20240423/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_thread_attributes.c` & `libfwsi-20240423/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_extern.h` & `libfwsi-20240423/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_repeating_thread.c` & `libfwsi-20240423/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/Makefile.in` & `libfwsi-20240423/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcthreads/libcthreads_queue.h` & `libfwsi-20240423/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/test-driver` & `libfwsi-20240423/test-driver`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ChangeLog` & `libfwsi-20240423/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/manuals/Makefile.in` & `libfwsi-20240423/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/manuals/libfwsi.3` & `libfwsi-20240423/manuals/libfwsi.3`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_control_panel_cpl_file_values.c` & `libfwsi-20240423/tests/fwsi_test_control_panel_cpl_file_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0006_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0006_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0003_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0003_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_compressed_folder_values.c` & `libfwsi-20240423/tests/fwsi_test_compressed_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_item.c` & `libfwsi-20240423/tests/fwsi_test_item.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_control_panel_category_values.c` & `libfwsi-20240423/tests/fwsi_test_control_panel_category_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef000a_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef000a_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_item_list.py` & `libfwsi-20240423/tests/pyfwsi_test_item_list.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_support.c` & `libfwsi-20240423/tests/fwsi_test_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_libcerror.h` & `libfwsi-20240423/tests/fwsi_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0000_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0000_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0001_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0001_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_mtp_file_entry_values.c` & `libfwsi-20240423/tests/fwsi_test_mtp_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_delegate_folder_values.c` & `libfwsi-20240423/tests/fwsi_test_delegate_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/Makefile.am` & `libfwsi-20240423/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0025_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0025_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0014_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0014_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_cdburn_values.c` & `libfwsi-20240423/tests/fwsi_test_cdburn_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_users_property_view_values.c` & `libfwsi-20240423/tests/fwsi_test_users_property_view_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_file_entry_values.c` & `libfwsi-20240423/tests/fwsi_test_file_entry_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_root_folder_values.c` & `libfwsi-20240423/tests/fwsi_test_root_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/test_manpage.sh` & `libfwsi-20240423/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/test_python_module.sh` & `libfwsi-20240423/tests/test_python_module.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240416
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
@@ -139,17 +139,17 @@
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
 PLATFORM=`uname -s | sed 's/-.*$//'`;
 
-if test "${PLATFORM}" = "MINGW64_NT";
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
 then
-	cp ../${LIBRARY_NAME}/.libs/${LIBRARY_NAME}-1.dll ../${PYTHON_MODULE}/libs/;
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
 	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
 fi
 
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
```

### Comparing `libfwsi-20240417/tests/pyfwsi_test_extension_block.py` & `libfwsi-20240423/tests/pyfwsi_test_extension_block.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_control_panel_item_values.c` & `libfwsi-20240423/tests/fwsi_test_control_panel_item_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_volume_values.c` & `libfwsi-20240423/tests/fwsi_test_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_mtp_volume_values.c` & `libfwsi-20240423/tests/fwsi_test_mtp_volume_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_root_folder.py` & `libfwsi-20240423/tests/pyfwsi_test_root_folder.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_memory.h` & `libfwsi-20240423/tests/fwsi_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0019_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0019_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/test_runner.sh` & `libfwsi-20240423/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_error.c` & `libfwsi-20240423/tests/fwsi_test_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_macros.h` & `libfwsi-20240423/tests/fwsi_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_volume.py` & `libfwsi-20240423/tests/pyfwsi_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0005_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0005_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_uri_sub_values.c` & `libfwsi-20240423/tests/fwsi_test_uri_sub_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block_0xbeef0013_values.c` & `libfwsi-20240423/tests/fwsi_test_extension_block_0xbeef0013_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_network_location.py` & `libfwsi-20240423/tests/pyfwsi_test_network_location.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_notify.c` & `libfwsi-20240423/tests/fwsi_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_support.py` & `libfwsi-20240423/tests/pyfwsi_test_support.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_file_entry_extension_values.c` & `libfwsi-20240423/tests/fwsi_test_file_entry_extension_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_memory.c` & `libfwsi-20240423/tests/fwsi_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_uri_values.c` & `libfwsi-20240423/tests/fwsi_test_uri_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_file_entry.py` & `libfwsi-20240423/tests/pyfwsi_test_file_entry.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_game_folder_values.c` & `libfwsi-20240423/tests/fwsi_test_game_folder_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/Makefile.in` & `libfwsi-20240423/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_extension_block.c` & `libfwsi-20240423/tests/fwsi_test_extension_block.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_network_location_values.c` & `libfwsi-20240423/tests/fwsi_test_network_location_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_item_list.c` & `libfwsi-20240423/tests/fwsi_test_item_list.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_libfwsi.h` & `libfwsi-20240423/tests/fwsi_test_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/fwsi_test_unused.h` & `libfwsi-20240423/tests/fwsi_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/pyfwsi_test_item.py` & `libfwsi-20240423/tests/pyfwsi_test_item.py`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/tests/test_library.sh` & `libfwsi-20240423/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ossfuzz/Makefile.am` & `libfwsi-20240423/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ossfuzz/ossfuzz_libfwsi.h` & `libfwsi-20240423/ossfuzz/ossfuzz_libfwsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ossfuzz/item_list_fuzzer.cc` & `libfwsi-20240423/ossfuzz/item_list_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ossfuzz/item_fuzzer.cc` & `libfwsi-20240423/ossfuzz/item_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ossfuzz/Makefile.in` & `libfwsi-20240423/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/ltmain.sh` & `libfwsi-20240423/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/remove-potcdate.sin` & `libfwsi-20240423/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/Makefile.in.in` & `libfwsi-20240423/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/en@quot.header` & `libfwsi-20240423/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/en@boldquot.header` & `libfwsi-20240423/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/insert-header.sin` & `libfwsi-20240423/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/Makevars` & `libfwsi-20240423/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/Makevars.in` & `libfwsi-20240423/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/po/Rules-quot` & `libfwsi-20240423/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1251.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf16_string.c` & `libfwsi-20240423/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base16_stream.c` & `libfwsi-20240423/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf8_stream.h` & `libfwsi-20240423/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_932.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf8_string.c` & `libfwsi-20240423/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base64_stream.c` & `libfwsi-20240423/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_error.h` & `libfwsi-20240423/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_turkish.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_unicode_character.c` & `libfwsi-20240423/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_arabic.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_thai.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_874.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf8_string.h` & `libfwsi-20240423/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1255.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf7_stream.c` & `libfwsi-20240423/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_byte_stream.h` & `libfwsi-20240423/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_koi8_u.c` & `libfwsi-20240423/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_unused.h` & `libfwsi-20240423/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base64_stream.h` & `libfwsi-20240423/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_error.c` & `libfwsi-20240423/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_romanian.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_6.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_russian.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_dingbats.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_15.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_936.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_croatian.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_scsu.h` & `libfwsi-20240423/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/Makefile.am` & `libfwsi-20240423/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf32_stream.c` & `libfwsi-20240423/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_936.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_roman.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf7_stream.h` & `libfwsi-20240423/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_thai.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_farsi.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_inuit.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_932.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_874.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_10.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_definitions.h` & `libfwsi-20240423/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_url_stream.h` & `libfwsi-20240423/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_koi8_u.h` & `libfwsi-20240423/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf16_stream.c` & `libfwsi-20240423/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1253.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_greek.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_libcerror.h` & `libfwsi-20240423/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_centraleurroman.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1254.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1255.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_unicode_character.h` & `libfwsi-20240423/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_13.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_949.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_celtic.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_support.h` & `libfwsi-20240423/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_4.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_949.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf16_stream.h` & `libfwsi-20240423/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_symbol.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_roman.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1257.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1254.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_950.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_extern.h` & `libfwsi-20240423/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1256.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_types.h` & `libfwsi-20240423/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base32_stream.h` & `libfwsi-20240423/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1253.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_16.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf8_stream.c` & `libfwsi-20240423/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1250.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_2.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_support.c` & `libfwsi-20240423/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_koi8_r.c` & `libfwsi-20240423/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_5.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf16_string.h` & `libfwsi-20240423/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf32_string.c` & `libfwsi-20240423/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_icelandic.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1256.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf32_string.h` & `libfwsi-20240423/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_romanian.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_8.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_koi8_r.h` & `libfwsi-20240423/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_cyrillic.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_arabic.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_croatian.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_9.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_greek.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1258.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_7.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/Makefile.in` & `libfwsi-20240423/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_3.c` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1250.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_scsu.c` & `libfwsi-20240423/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1252.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_turkish.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_ukrainian.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_russian.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1258.c` & `libfwsi-20240423/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_celtic.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_byte_stream.c` & `libfwsi-20240423/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_gaelic.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_utf32_stream.h` & `libfwsi-20240423/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_symbol.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1257.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_inuit.h` & `libfwsi-20240423/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_mac_farsi.c` & `libfwsi-20240423/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_950.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_url_stream.c` & `libfwsi-20240423/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1251.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_windows_1252.h` & `libfwsi-20240423/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_codepage_iso_8859_14.h` & `libfwsi-20240423/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base16_stream.h` & `libfwsi-20240423/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libuna/libuna_base32_stream.c` & `libfwsi-20240423/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/Makefile.in` & `libfwsi-20240423/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_definitions.h` & `libfwsi-20240423/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_extern.h` & `libfwsi-20240423/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_support.c` & `libfwsi-20240423/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_stream.h` & `libfwsi-20240423/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/Makefile.am` & `libfwsi-20240423/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_unused.h` & `libfwsi-20240423/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_verbose.h` & `libfwsi-20240423/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_print.h` & `libfwsi-20240423/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_stream.c` & `libfwsi-20240423/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_support.h` & `libfwsi-20240423/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_verbose.c` & `libfwsi-20240423/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/Makefile.in` & `libfwsi-20240423/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_libcerror.h` & `libfwsi-20240423/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcnotify/libcnotify_print.c` & `libfwsi-20240423/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_system.c` & `libfwsi-20240423/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_error.c` & `libfwsi-20240423/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_extern.h` & `libfwsi-20240423/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/Makefile.am` & `libfwsi-20240423/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_types.h` & `libfwsi-20240423/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_support.h` & `libfwsi-20240423/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_error.h` & `libfwsi-20240423/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_system.h` & `libfwsi-20240423/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_definitions.h` & `libfwsi-20240423/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_support.c` & `libfwsi-20240423/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/libcerror_unused.h` & `libfwsi-20240423/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libcerror/Makefile.in` & `libfwsi-20240423/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.h` & `libfwsi-20240423/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.c` & `libfwsi-20240423/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_error.h` & `libfwsi-20240423/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_floatingtime.c` & `libfwsi-20240423/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_support.h` & `libfwsi-20240423/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.h` & `libfwsi-20240423/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_definitions.h` & `libfwsi-20240423/libfdatetime/libfdatetime_definitions.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_hfs_time.c` & `libfwsi-20240423/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/Makefile.am` & `libfwsi-20240423/libfdatetime/Makefile.am`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_filetime.c` & `libfwsi-20240423/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_systemtime.h` & `libfwsi-20240423/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_extern.h` & `libfwsi-20240423/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_posix_time.c` & `libfwsi-20240423/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_unused.h` & `libfwsi-20240423/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.h` & `libfwsi-20240423/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_systemtime.c` & `libfwsi-20240423/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_nsf_timedate.h` & `libfwsi-20240423/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_libcerror.h` & `libfwsi-20240423/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_support.c` & `libfwsi-20240423/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_error.c` & `libfwsi-20240423/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_posix_time.h` & `libfwsi-20240423/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.h` & `libfwsi-20240423/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_filetime.h` & `libfwsi-20240423/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_date_time_values.c` & `libfwsi-20240423/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_types.h` & `libfwsi-20240423/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/Makefile.in` & `libfwsi-20240423/libfdatetime/Makefile.in`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/libfdatetime/libfdatetime_fat_date_time.c` & `libfwsi-20240423/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/aclocal.m4` & `libfwsi-20240423/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfwsi-20240417/configure.ac` & `libfwsi-20240423/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfwsi],
- [20240417],
+ [20240423],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfwsi.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

### Comparing `libfwsi-20240417/libfwsi.spec` & `libfwsi-20240423/libfwsi.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfwsi
-Version: 20240417
+Version: 20240423
 Release: 1
 Summary: Library to access the Windows Shell Item format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfwsi
           
@@ -76,10 +76,10 @@
 %files -n libfwsi-python3
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_libdir}/python3*/site-packages/*.a
 %{_libdir}/python3*/site-packages/*.so
 
 %changelog
-* Wed Apr 17 2024 Joachim Metz <joachim.metz@gmail.com> 20240417-1
+* Tue Apr 23 2024 Joachim Metz <joachim.metz@gmail.com> 20240423-1
 - Auto-generated
```

