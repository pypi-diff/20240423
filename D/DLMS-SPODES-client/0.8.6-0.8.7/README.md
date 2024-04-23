# Comparing `tmp/DLMS_SPODES_client-0.8.6.tar.gz` & `tmp/DLMS_SPODES_client-0.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DLMS_SPODES_client-0.8.6.tar", last modified: Mon Apr 22 08:35:40 2024, max compression
+gzip compressed data, was "DLMS_SPODES_client-0.8.7.tar", last modified: Tue Apr 23 11:04:07 2024, max compression
```

## Comparing `DLMS_SPODES_client-0.8.6.tar` & `DLMS_SPODES_client-0.8.7.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.797119 DLMS_SPODES_client-0.8.6/
--rw-rw-rw-   0        0        0      526 2024-04-22 08:35:40.797119 DLMS_SPODES_client-0.8.6/PKG-INFO
--rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.6/README.md
--rw-rw-rw-   0        0        0      836 2024-04-22 08:33:16.000000 DLMS_SPODES_client-0.8.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 08:35:40.798122 DLMS_SPODES_client-0.8.6/setup.cfg
--rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.647121 DLMS_SPODES_client-0.8.6/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.665122 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/
--rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/FCS16.py
--rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/__init__.py
--rw-rw-rw-   0        0        0   115215 2024-04-22 05:45:45.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/client.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.634121 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_common/
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.682122 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_common/enums/
--rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
--rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.728121 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/
--rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
--rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/CountType.py
--rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
--rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
--rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
--rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
--rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
--rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
--rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
--rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
--rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
--rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
--rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
--rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
--rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
--rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
--rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
--rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
--rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.782121 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/
--rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
--rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
--rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
--rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
--rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
--rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
--rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
--rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
--rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
--rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
--rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
--rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
--rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
--rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
--rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
--rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
--rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
--rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
--rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
--rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
--rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
--rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
--rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
--rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
--rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.784122 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/internal/
--rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
--rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/logger.py
--rw-rw-rw-   0        0        0     4992 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/servers.py
--rw-rw-rw-   0        0        0     3749 2024-04-22 08:32:27.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/services.py
--rw-rw-rw-   0        0        0    45655 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/task.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.678126 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/
--rw-rw-rw-   0        0        0      526 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3251 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       74 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2024-04-22 08:35:40.000000 DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.6/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-22 08:35:40.795121 DLMS_SPODES_client-0.8.6/test/
--rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.6/test/name2.csv
--rw-rw-rw-   0        0        0     9995 2024-04-22 05:57:16.000000 DLMS_SPODES_client-0.8.6/test/test_Client.py
--rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.6/test/test_logger.py
--rw-rw-rw-   0        0        0      360 2024-04-22 08:34:06.000000 DLMS_SPODES_client-0.8.6/test/test_services.py
--rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.6/test/конфигурация GSM.csv
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.090102 DLMS_SPODES_client-0.8.7/
+-rw-rw-rw-   0        0        0      526 2024-04-23 11:04:07.090102 DLMS_SPODES_client-0.8.7/PKG-INFO
+-rw-rw-rw-   0        0        0       15 2023-06-06 06:37:54.000000 DLMS_SPODES_client-0.8.7/README.md
+-rw-rw-rw-   0        0        0      836 2024-04-23 11:03:54.000000 DLMS_SPODES_client-0.8.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 11:04:07.091101 DLMS_SPODES_client-0.8.7/setup.cfg
+-rw-rw-rw-   0        0        0      447 2024-01-18 10:26:12.000000 DLMS_SPODES_client-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.919098 DLMS_SPODES_client-0.8.7/src/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.937106 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/
+-rw-rw-rw-   0        0        0     3117 2021-12-10 12:57:48.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/FCS16.py
+-rw-rw-rw-   0        0        0      449 2024-01-19 10:55:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/__init__.py
+-rw-rw-rw-   0        0        0   115215 2024-04-22 05:45:45.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/client.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.908098 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.958101 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/
+-rw-rw-rw-   0        0        0      521 2024-01-22 10:35:09.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py
+-rw-rw-rw-   0        0        0        0 2024-01-22 04:37:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.011101 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/
+-rw-rw-rw-   0        0        0     1429 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py
+-rw-rw-rw-   0        0        0      264 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/CountType.py
+-rw-rw-rw-   0        0        0    17702 2022-08-02 09:38:23.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py
+-rw-rw-rw-   0        0        0     5909 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py
+-rw-rw-rw-   0        0        0    17569 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py
+-rw-rw-rw-   0        0        0    10122 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py
+-rw-rw-rw-   0        0        0    45717 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py
+-rw-rw-rw-   0        0        0     3461 2024-01-24 13:02:57.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py
+-rw-rw-rw-   0        0        0     5814 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py
+-rw-rw-rw-   0        0        0     1419 2024-01-25 09:32:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py
+-rw-rw-rw-   0        0        0      699 2024-01-25 11:48:38.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py
+-rw-rw-rw-   0        0        0     8277 2024-04-10 09:20:48.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py
+-rw-rw-rw-   0        0        0     4476 2024-01-30 13:16:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py
+-rw-rw-rw-   0        0        0      193 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/HdlcControlFrame.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusCommand.py
+-rw-rw-rw-   0        0        0      623 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py
+-rw-rw-rw-   0        0        0      155 2024-01-22 08:54:46.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/ResponseType.py
+-rw-rw-rw-   0        0        0      483 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/SetResponseType.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/_HDLCInfo.py
+-rw-rw-rw-   0        0        0     3392 2024-04-10 09:20:47.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.073104 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/
+-rw-rw-rw-   0        0        0      241 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Access.py
+-rw-rw-rw-   0        0        0      358 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ApplicationReference.py
+-rw-rw-rw-   0        0        0      962 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py
+-rw-rw-rw-   0        0        0      819 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py
+-rw-rw-rw-   0        0        0    11492 2024-01-22 08:27:54.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py
+-rw-rw-rw-   0        0        0      224 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Definition.py
+-rw-rw-rw-   0        0        0      768 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py
+-rw-rw-rw-   0        0        0      237 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ExceptionServiceError.py
+-rw-rw-rw-   0        0        0      273 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/HardwareResource.py
+-rw-rw-rw-   0        0        0      143 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/HdlcFrameType.py
+-rw-rw-rw-   0        0        0      246 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Initiate.py
+-rw-rw-rw-   0        0        0      209 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/InterfaceType.py
+-rw-rw-rw-   0        0        0      330 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/LoadDataSet.py
+-rw-rw-rw-   0        0        0    11415 2024-01-22 09:18:13.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py
+-rw-rw-rw-   0        0        0      112 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Priority.py
+-rw-rw-rw-   0        0        0      235 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/RequestTypes.py
+-rw-rw-rw-   0        0        0      406 2024-01-22 07:03:42.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Security.py
+-rw-rw-rw-   0        0        0      371 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Service.py
+-rw-rw-rw-   0        0        0      173 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceClass.py
+-rw-rw-rw-   0        0        0      177 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ServiceError.py
+-rw-rw-rw-   0        0        0      545 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py
+-rw-rw-rw-   0        0        0      142 2024-01-22 07:59:03.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/StateError.py
+-rw-rw-rw-   0        0        0      199 2024-01-22 09:32:53.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Task.py
+-rw-rw-rw-   0        0        0      233 2024-01-22 09:32:52.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/VdeStateError.py
+-rw-rw-rw-   0        0        0     1356 2024-01-25 12:20:44.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.076102 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/
+-rw-rw-rw-   0        0        0    53226 2024-01-30 12:44:29.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py
+-rw-rw-rw-   0        0        0     1908 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/logger.py
+-rw-rw-rw-   0        0        0     4992 2024-04-22 07:11:32.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/servers.py
+-rw-rw-rw-   0        0        0     3749 2024-04-22 08:32:27.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/services.py
+-rw-rw-rw-   0        0        0    46225 2024-04-23 09:34:24.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/task.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:06.952123 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/
+-rw-rw-rw-   0        0        0      526 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3251 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       74 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2024-04-23 11:04:06.000000 DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-02-02 07:33:33.000000 DLMS_SPODES_client-0.8.7/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-23 11:04:07.087101 DLMS_SPODES_client-0.8.7/test/
+-rw-rw-rw-   0        0        0       30 2024-04-15 07:35:51.000000 DLMS_SPODES_client-0.8.7/test/name2.csv
+-rw-rw-rw-   0        0        0    10534 2024-04-23 10:56:23.000000 DLMS_SPODES_client-0.8.7/test/test_Client.py
+-rw-rw-rw-   0        0        0      167 2024-04-17 09:11:09.000000 DLMS_SPODES_client-0.8.7/test/test_logger.py
+-rw-rw-rw-   0        0        0      360 2024-04-22 08:34:06.000000 DLMS_SPODES_client-0.8.7/test/test_services.py
+-rw-rw-rw-   0        0        0      290 2024-04-15 08:24:50.000000 DLMS_SPODES_client-0.8.7/test/конфигурация GSM.csv
```

### Comparing `DLMS_SPODES_client-0.8.6/PKG-INFO` & `DLMS_SPODES_client-0.8.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS_SPODES_client
-Version: 0.8.6
+Version: 0.8.7
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.6/pyproject.toml` & `DLMS_SPODES_client-0.8.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 package-dir = {"" = "src"}
 
 [project]
 name = "DLMS_SPODES_client"
-version = "0.8.6"
+version = "0.8.7"
 authors = [
     {name="Serj Kotilevski", email="youserj@outlook.com"}
 ]
 dependencies = [
     "DLMS-SPODES == 0.69.6",
     "DLMS-SPODES-communications >= 1.2.4",
     "pycryptodomex>=3.15"
```

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/FCS16.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/FCS16.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/client.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/client.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_common/enums/TraceLevel.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/AesGcmParameter.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXByteBuffer.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXCiphering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMS.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChippering.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSChipperingStream.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSConfirmedServiceError.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSException.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSLNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSNParameters.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXDLMSSettings.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/GXReplyData.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/MBusEncryptionMode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/__init__.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Authentication.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/BerType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Command.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/ObjectType.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/Standard.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/gurux_dlms/internal/_GXCommon.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/logger.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/logger.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/servers.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/servers.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/services.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/services.py`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client/task.py` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,170 +42,158 @@
         if OSI.PHYSICAL not in c.level:
             if not c.media.is_open():
                 await c.media.open()
             c.level = OSI.PHYSICAL
             c.set_error(Transmit.OK, "Open port")
             c.log(logL.INFO, F"Open port communication channel: {c.media}")
             if c.objects is None:
-                await InitType().exchange(c, is_public=True)
+                await InitType().data_link(c, is_public=True)
                 await c.close()  # todo: change to DiscRequest, or make not closed
-            ret = await self.exchange(c, is_public=True if isinstance(self, InitType) else False)
+            ret = await self.data_link(c, is_public=True if isinstance(self, InitType) else False)
             await c.close()  # todo: change to DiscRequest
             return ret
 
-    async def exchange(self, c: Client, is_public: bool = False):
+    async def data_link(self, c: Client, is_public: bool = False):
         if OSI.DATA_LINK not in c.level:
-            if await get_HDLC(c, is_public) is False:
-                return False
-        return await self.exchange_HDLC(c, is_public)
+            c.status = Status.EXCHANGE
+            c.set_error(Transmit.OK, "Open port")
+            c.errors.clear()  # clear all last session errors
+            c.send_frames.clear()
+            # calculate addresses
+            c.DA = frame.Address(
+                upper_address=int(c.server_SAP),
+                lower_address=int(c.device_address) if c.device_address else None,
+                length=c.addr_size
+            )
+            c.SA = frame.Address(upper_address=0x10 if is_public else int(c.SAP))
+            c.log(logL.INFO, F"{c.SA=} {c.DA=}")
+            # initialize connection
+            c.reply.clear()
+            # replace this
+            if c.settings.cipher.security != Security.NONE:
+                c.log(logL.DEB, F"Security: {c.settings.cipher.security}/n"
+                                F"System title: {c.settings.cipher.systemTitle.hex()}"
+                                F"Authentication key: {c.settings.cipher.authenticationKey.hex()}"
+                                F"Block cipher key: {c.settings.cipher.blockCipherKey.hex()}")
+                if c.settings.cipher.dedicatedKey:
+                    c.log(logL.DEB, F"Dedicated key: {c.settings.cipher.dedicatedKey.hex()}")
+            # SNRM
+            c.get_SNRM_request()
+            c.status = Status.READ
+            await c.read_data_block()
+            c.status = Status.EXCHANGE
+            c.level = OSI.DATA_LINK
+            c.reply.clear()
+        return await self.application(c, is_public)
 
-    async def exchange_HDLC(self, c: Client, is_public: bool = False):
+    async def application(self, c: Client, is_public: bool = False):
         if OSI.APPLICATION not in c.level:
-            if await get_AARE(c, is_public) is False:
-                return False
-        return await self.exchange2(c)
-
-    @abstractmethod
-    async def exchange2(self, c: Client):
-        """common exchange in session"""
-
+            if c.invocationCounter and c.settings.cipher is not None and c.settings.cipher.security != Security.NONE:
+                # create IC object. TODO: remove it after close connection, maybe???
+                c.settings.proposedConformance |= Conformance.GENERAL_PROTECTION
+
+                # my block
+                IC: Data = c.objects.add_if_missing(ut.CosemClassId(1),
+                                                    logical_name=cst.LogicalName(bytearray((0, c.get_channel_index(), 43, 1,
+                                                                                            c.current_association.security_setup_reference.e, 255))),
+                                                    version=cdt.Unsigned(0))
+                tmp_client_SAP = c.current_association.associated_partners_id.client_SAP
+                challenge = c.settings.ctoSChallenge
+                try:
+                    c.objects.getIECHDLCSetup(c.get_channel_index()).set_from_info(c.reply.data.get_data())
+                    c.aarqRequest(c.m_id)
+                    await c.read_data_block()
+                    ret = c.parseAareResponse(c.reply.data)
+                    c.level |= OSI.APPLICATION  # todo: it's must be result of <ret> look down
+                    c.reply.clear()
+                    await c.read_attribute(IC, 2)
+                    c.settings.cipher.invocationCounter = 1 + IC.value.decode()
+                    c.log(logL.DEB, "Invocation counter: " + str(c.settings.cipher.invocationCounter))
+                    # disconnect
+                    if c.media and c.media.is_open():
+                        c.log(logL.DEB, "DisconnectRequest")
+                        await c.disconnect_request()
+                finally:
+                    c.SAP = tmp_client_SAP
+                    c.settings.useCustomChallenge = challenge is not None
+                    c.settings.ctoSChallenge = challenge
+
+                # gurux with several removed methods
+                # add = self.settings.clientAddress
+                # auth = self.settings.authentication
+                # security = self.client.ciphering.security
+                # challenge = self.client.ctoSChallenge
+                # try:
+                #     self.client.clientAddress = 16
+                #     self.settings.authentication = Authentication.NONE
+                #     self.client.ciphering.security = Security.NONE
+                #     reply = GXReplyData()
+                #     self.get_SNRM_request()
+                #     self.status = Status.READ
+                #     self.read_data_block2()
+                #     self.objects.IEC_HDLS_setup.set_from_info(self.reply.data.get_data())
+                #     self.connection_state = ConnectionState.HDLC
+                #     self.reply.clear()
+                #     self.aarqRequest()
+                #     self.read_data_block2()
+                #     self.parseAareResponse(reply.data)
+                #     reply.clear()
+                #     item = GXDLMSData(self.invocationCounter)
+                #     data = self.client.read(item, 2)[0]
+                #     reply = GXReplyData()
+                #     self.read_data_block(data, reply)
+                #     item.encodings[2] = reply.data.get_data()
+                #     Update data type on read.
+                #     if item.getDataType(2) == cdt.NullData.TAG:
+                #         item.setDataType(2, reply.valueType)
+                #     self.client.updateValue(item, 2, reply.value)
+                #     self.client.ciphering.invocationCounter = 1 + item.value
+                #     print("Invocation counter: " + str(self.client.ciphering.invocationCounter))
+                #     if self.media and self.media.isOpen():
+                #         self.log(logL.INFO, "DisconnectRequest")
+                #         self.disconnect_request()
+                # finally:
+                #     self.settings.clientAddress = add
+                #     self.settings.authentication = auth
+                #     self.client.ciphering.security = security
+                #     self.client.ctoSChallenge = challenge
 
-async def get_HDLC(c: Client, is_public: bool = False) -> bool:
-    c.status = Status.EXCHANGE
-    c.set_error(Transmit.OK, "Open port")
-    c.errors.clear()  # clear all last session errors
-    c.send_frames.clear()
-    # calculate addresses
-    c.DA = frame.Address(
-        upper_address=int(c.server_SAP),
-        lower_address=int(c.device_address) if c.device_address else None,
-        length=c.addr_size
-    )
-    c.SA = frame.Address(upper_address=0x10 if is_public else int(c.SAP))
-    c.log(logL.INFO, F"{c.SA=} {c.DA=}")
-    # initialize connection
-    c.reply.clear()
-    # replace this
-    if c.settings.cipher.security != Security.NONE:
-        c.log(logL.DEB, F"Security: {c.settings.cipher.security}/n"
-                           F"System title: {c.settings.cipher.systemTitle.hex()}"
-                           F"Authentication key: {c.settings.cipher.authenticationKey.hex()}"
-                           F"Block cipher key: {c.settings.cipher.blockCipherKey.hex()}")
-        if c.settings.cipher.dedicatedKey:
-            c.log(logL.DEB, F"Dedicated key: {c.settings.cipher.dedicatedKey.hex()}")
-    # SNRM
-    c.get_SNRM_request()
-    c.status = Status.READ
-    await c.read_data_block()
-    c.status = Status.EXCHANGE
-    c.level = OSI.DATA_LINK
-    c.reply.clear()
-    return True
-
-
-async def get_AARE(c: Client, is_public: bool = False) -> bool:
-    if c.invocationCounter and c.settings.cipher is not None and c.settings.cipher.security != Security.NONE:
-        # create IC object. TODO: remove it after close connection, maybe???
-        c.settings.proposedConformance |= Conformance.GENERAL_PROTECTION
-
-        # my block
-        IC: Data = c.objects.add_if_missing(ut.CosemClassId(1),
-                                            logical_name=cst.LogicalName(bytearray((0, c.get_channel_index(), 43, 1,
-                                                                                       c.current_association.security_setup_reference.e, 255))),
-                                            version=cdt.Unsigned(0))
-        tmp_client_SAP = c.current_association.associated_partners_id.client_SAP
-        challenge = c.settings.ctoSChallenge
-        try:
-            c.objects.getIECHDLCSetup(c.get_channel_index()).set_from_info(c.reply.data.get_data())
-            c.aarqRequest(c.m_id)
-            await c.read_data_block()
-            ret = c.parseAareResponse(c.reply.data)
-            c.level |= OSI.APPLICATION  # todo: it's must be result of <ret> look down
-            c.reply.clear()
-            await c.read_attribute(IC, 2)
-            c.settings.cipher.invocationCounter = 1 + IC.value.decode()
-            c.log(logL.DEB, "Invocation counter: " + str(c.settings.cipher.invocationCounter))
-            # disconnect
-            if c.media and c.media.is_open():
-                c.log(logL.DEB, "DisconnectRequest")
-                await c.disconnect_request()
-        finally:
-            c.SAP = tmp_client_SAP
-            c.settings.useCustomChallenge = challenge is not None
-            c.settings.ctoSChallenge = challenge
-
-        # gurux with several removed methods
-        # add = self.settings.clientAddress
-        # auth = self.settings.authentication
-        # security = self.client.ciphering.security
-        # challenge = self.client.ctoSChallenge
-        # try:
-        #     self.client.clientAddress = 16
-        #     self.settings.authentication = Authentication.NONE
-        #     self.client.ciphering.security = Security.NONE
-        #     reply = GXReplyData()
-        #     self.get_SNRM_request()
-        #     self.status = Status.READ
-        #     self.read_data_block2()
-        #     self.objects.IEC_HDLS_setup.set_from_info(self.reply.data.get_data())
-        #     self.connection_state = ConnectionState.HDLC
-        #     self.reply.clear()
-        #     self.aarqRequest()
-        #     self.read_data_block2()
-        #     self.parseAareResponse(reply.data)
-        #     reply.clear()
-        #     item = GXDLMSData(self.invocationCounter)
-        #     data = self.client.read(item, 2)[0]
-        #     reply = GXReplyData()
-        #     self.read_data_block(data, reply)
-        #     item.encodings[2] = reply.data.get_data()
-        #     Update data type on read.
-        #     if item.getDataType(2) == cdt.NullData.TAG:
-        #         item.setDataType(2, reply.valueType)
-        #     self.client.updateValue(item, 2, reply.value)
-        #     self.client.ciphering.invocationCounter = 1 + item.value
-        #     print("Invocation counter: " + str(self.client.ciphering.invocationCounter))
-        #     if self.media and self.media.isOpen():
-        #         self.log(logL.INFO, "DisconnectRequest")
-        #         self.disconnect_request()
-        # finally:
-        #     self.settings.clientAddress = add
-        #     self.settings.authentication = auth
-        #     self.client.ciphering.security = security
-        #     self.client.ctoSChallenge = challenge
-
-    c.aarqRequest(mechanism_id.NONE if is_public else c.m_id)
-    await c.read_data_block()
-        # await c.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
-    match c.parseAareResponse(c.reply.data):
-        case AcseServiceUser.NULL:
-            c.log(logL.INFO, 'Authentication success')
-            c.level |= OSI.APPLICATION
-        case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public:
-            c.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
-        case AcseServiceUser.AUTHENTICATION_REQUIRED:
-            c.reply.clear()
-            c.getApplicationAssociationRequest()
+            c.aarqRequest(mechanism_id.NONE if is_public else c.m_id)
             await c.read_data_block()
-            c.parseApplicationAssociationResponse()
-        case _ as diagnostic:
-            raise exc.AssociationResultError(diagnostic)
-    c.set_error(Transmit.OK, "Initialize connection")
-    # TODO: remove DIMA crutch dummy read for correct write
-    if c.objects is not None:
-        c.get_get_request_normal(c.objects.LDN.get_attr_descriptor(2))
-        await c.read_data_block()
-        c.matching_LDN(octet_string.LDN(c.reply.data.get_data()))
-    return True
+            # await c.read_attr(ut.CosemAttributeDescriptor((collection.ClassID.ASSOCIATION_LN, ut.CosemObjectInstanceId("0.0.40.0.0.255"), ut.CosemObjectAttributeId(6)))) # for test only
+            match c.parseAareResponse(c.reply.data):
+                case AcseServiceUser.NULL:
+                    c.log(logL.INFO, 'Authentication success')
+                    c.level |= OSI.APPLICATION
+                case AcseServiceUser.AUTHENTICATION_FAILURE as diag if is_public:
+                    c.log(logL.WARN, F'On Public connection type got {diag.name}, broad force turn ON')
+                case AcseServiceUser.AUTHENTICATION_REQUIRED:
+                    c.reply.clear()
+                    c.getApplicationAssociationRequest()
+                    await c.read_data_block()
+                    c.parseApplicationAssociationResponse()
+                case _ as diagnostic:
+                    raise exc.AssociationResultError(diagnostic)
+            c.set_error(Transmit.OK, "Initialize connection")
+            # TODO: remove DIMA crutch dummy read for correct write
+            if c.objects is not None:
+                c.get_get_request_normal(c.objects.LDN.get_attr_descriptor(2))
+                await c.read_data_block()
+                c.matching_LDN(octet_string.LDN(c.reply.data.get_data()))
+        return await self.exchange(c)
+
+    @abstractmethod
+    async def exchange(self, c: Client):
+        """application level exchange"""
 
 
 class Dummy(ExTask):
     """dummy task"""
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         """"""
         c.log(logL.INFO, "dummy task")
 
 
 @dataclass
 class Loop(ExTask):
     task: ExTask
@@ -218,15 +206,15 @@
         attempt = count()
         while not self.func(await super(Loop, self).run(c)):
             if next(attempt) == self.attempt_amount:
                 return False
             await asyncio.sleep(self.delay)
         return True
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         return await self.task.exchange(c)
 
 
 class Sequence(ExTask):
     """for exchange task sequence"""
     tasks: list[ExTask]
     __is_exchange: bool
@@ -238,15 +226,15 @@
 
     def append(self, task: ExTask):
         if not self.__is_exchange:
             self.tasks.append(task)
         else:
             raise RuntimeError(F"append to {self.__class__.__name__} not allowed, already exchange started")
 
-    async def exchange2(self, c: Client) -> list[cdt.CommonDataType | None]:
+    async def exchange(self, c: Client) -> list[cdt.CommonDataType | None]:
         ret = list()
         self.__is_exchange = True
         for t in self.tasks:
             # ret.append(await t.exchange(c))
             # TODO: remove in future try-except block with pleasure return value => ret.append(await t.exchange())
             try:
                 res = await t.exchange(c)
@@ -258,15 +246,15 @@
 
 class InitType(ExTask):
     """nothing params"""
     # async def exchange(self, c: Client, is_public: bool = False):
     #     await c.close()  # close hdlc before init
     #     return await super(InitType, self).exchange(c, is_public=True)
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         # read LDN
         data = await c.read_attr(collection.AttrDesc.LDN_VALUE)
         ldn = octet_string.LDN(data)
         # find device_id(type for Russia)
         type_value, _ = cdt.get_instance_and_pdu_from_value(await c.read_attr(ut.CosemAttributeDescriptor((1, "0.0.96.1.1.255", 2))))
         # find version data
         for desc in (ut.CosemAttributeDescriptor((1, "0.0.0.2.1.255", 2)), ut.CosemAttributeDescriptor((1, "0.0.96.1.2.255", 2))):
@@ -319,15 +307,15 @@
 
 
 @dataclass
 class ReadAttribute(ExTask):
     ln: collection.LNContaining
     index: int
 
-    async def exchange2(self, c: Client) -> cdt.CommonDataType:
+    async def exchange(self, c: Client) -> cdt.CommonDataType:
         # TODO: check is_readable
         obj = c.objects.get_object(self.ln)
         return await self.read_from_obj(c, obj, self.index)
 
     @staticmethod
     async def read_from_obj(c: Client, obj: collection.InterfaceClass, index: int) -> cdt.CommonDataType | ValueError:
         c.get_get_request_normal(
@@ -346,43 +334,43 @@
 
 @dataclass
 class ReadEmptyAttribute(ExTask):
     """read if attribute is empty"""
     ln: collection.LNContaining
     index: int
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         # TODO: check is_readable
         if c.objects.get_object(self.ln).get_attr(self.index) is None:
             data = await ReadAttribute(
                 ln=self.ln,
                 index=self.index).exchange(c)
 
 
 @dataclass
 class ReadAttributes(ExTask):
     ln: collection.LNContaining
     indexes: tuple[int, ...]
 
-    async def exchange2(self, c: Client) -> tuple[cdt.CommonDataType | ValueError]:
+    async def exchange(self, c: Client) -> tuple[cdt.CommonDataType | ValueError]:
         obj = c.objects.get_object(self.ln)
         ret: list[cdt.CommonDataType | ValueError] = list()
         # TODO: check for Get-Request-With-List
         for i in self.indexes:
             ret.append(await ReadAttribute.read_from_obj(c, obj, i))
         return tuple(ret)
 
 
 @dataclass
 class WriteAttribute(ExTask):
     ln: collection.LNContaining
     index: int
     value: bytes | str | int | list | tuple | datetime.datetime
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         obj = c.objects.get_object(self.ln)
         if isinstance(self.value, (str, int, list, tuple, datetime.datetime)):
             value2 = await c.encode(
                 obj=obj,
                 index=self.index,
                 value=self.value)
             enc = value2.encoding
@@ -397,15 +385,15 @@
 
 @dataclass
 class WriteAttributesOld(ExTask):
     """todo: use for write without value(from object) replace all to WriteAttribute in future."""
     ln: collection.LNContaining
     indexes: tuple[int, ...]
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         for i in self.indexes:
             if c.objects.is_writable(
                     ln=(obj := c.objects.get_object(self.ln)).logical_name,
                     index=i,
                     association_id=c.objects.get_association_id(c.SAP)):
                 data = c.get_set_request_normal(
                     obj=obj,
@@ -416,15 +404,15 @@
 
 
 @dataclass
 class ExecuteByDesc(ExTask):
     """execute method by method descriptor # TODO: rewrite this"""
     desc: ut.CosemMethodDescriptor
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         try:
             await c.execute_method(self.desc)
             c.set_error(Transmit.OK, F'Execute {self.desc}.')
         except Exception as e:
             c.log(logL.INFO, F'ERROR: Исполнение {self.desc}')
             c.set_error(Transmit.EXECUTE_ERROR, F'Исполнение {self.desc}')
 
@@ -432,15 +420,15 @@
 @dataclass
 class Execute(ExTask):
     """execute method by method descriptor # TODO: rewrite this with <value>"""
     ln: collection.LNContaining
     index: int
     value: str
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         obj = c.objects.get_object(self.ln)
         try:
             await c.execute_method(ut.CosemMethodDescriptor(
                 (obj.CLASS_ID,
                  ut.CosemObjectInstanceId(obj.logical_name.contents),
                  ut.CosemObjectMethodId(self.index))
             ))
@@ -449,15 +437,15 @@
             c.log(logL.INFO, F'ERROR: Исполнение {self.ln}: {self.index}')
             c.set_error(Transmit.EXECUTE_ERROR, F'Исполнение {self.ln}: {self.index}')
 
 
 class WriteTime(ExTask):
     """write Clock.time depend from transfer time"""
 
-    async def exchange2(self, c: Client):
+    async def exchange(self, c: Client):
         try:
             obj = c.objects.clock
             c.get_get_request_normal(obj.get_attr_descriptor(3))
             await c.read_data_block()
             tz = obj.get_attr_element(3).DATA_TYPE(c.reply.data.get_data())
             await WriteAttribute(
                 ln=obj.logical_name,
@@ -487,15 +475,15 @@
         return F"{self.message}: {self.position}/{self.max}"
 
 
 @dataclass
 class UpdateFirmware(ExTask):
     """only for KPZ now"""
 
-    async def exchange2(self, c: Client) -> bool:
+    async def exchange(self, c: Client) -> bool:
         # check available action todo: not work in 0.0.38
         # if c.current_association.object_list is None:
         #     await ReadAttribute(
         #         ln=c.current_association.logical_name,
         #         index=2
         #     ).exchange(c)
         # image_objects: collection.ImageTransfer = collection.get_filtered(objects=c.current_association.objects, keys=(overview.ClassID.IMAGE_TRANSFER, ))
```

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/PKG-INFO` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DLMS-SPODES-client
-Version: 0.8.6
+Version: 0.8.7
 Summary: dlms-spodes
 Home-page: https://github.com/youserj/SPODESclient_prj
 Author-email: Serj Kotilevski <youserj@outlook.com>
 Project-URL: Source, https://github.com/youserj/SPODESclient_prj
 Keywords: dlms,spodes,client
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `DLMS_SPODES_client-0.8.6/src/DLMS_SPODES_client.egg-info/SOURCES.txt` & `DLMS_SPODES_client-0.8.7/src/DLMS_SPODES_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DLMS_SPODES_client-0.8.6/test/test_Client.py` & `DLMS_SPODES_client-0.8.7/test/test_Client.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,42 @@
         c2 = Client(id_="d2", del_cb=id_factory.remove)
         del c2
         Client(id_=id_factory.create())
         Client()
         c3 = Client()
         print(c1.id, c3.id, id_factory.value)
 
-    def test_connect(self):
+    def test_lowest_connect(self):
         t_server = TransactionServer(
             clients=[c := Client(media=AsyncSerial(
                                 port="COM13",
                                 inactivity_timeout=3))],
             tsk=task.Dummy()
         )
         t_server.start()
         while not t_server.results.is_complete():
             time.sleep(1)
         print(c.objects)
 
+    def test_high_connect(self):
+        t_server = TransactionServer(
+            clients=[c := Client(
+                secret="30 30 30 30 30 30 30 30 30 30 30 30 30 30 30 31",
+                media=AsyncSerial(
+                    port="COM13",
+                    inactivity_timeout=3))],
+            tsk=task.Dummy()
+        )
+        t_server.start()
+        c.m_id.set(2)
+        c.SAP.set(0x30)  # for KPZ
+        while not t_server.results.is_complete():
+            time.sleep(1)
+        print(c.objects)
+
     def test_Loop(self):
         def foo(res):
             return res == cdt.Long(4)
 
         t_server = TransactionServer(
             clients=[
                 client := Client(
```

