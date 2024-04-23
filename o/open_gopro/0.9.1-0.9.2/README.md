# Comparing `tmp/open_gopro-0.9.1.tar.gz` & `tmp/open_gopro-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_gopro-0.9.1.tar", max compression
+gzip compressed data, was "open_gopro-0.9.2.tar", max compression
```

## Comparing `open_gopro-0.9.1.tar` & `open_gopro-0.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0      649 2022-05-18 18:02:05.525778 open_gopro-0.9.1/open_gopro/__init__.py
--rw-r--r--   0        0        0      377 2022-02-07 21:15:19.771803 open_gopro-0.9.1/open_gopro/api/__init__.py
--rw-r--r--   0        0        0     1058 2022-05-26 19:13:09.342380 open_gopro-0.9.1/open_gopro/api/api.py
--rw-r--r--   0        0        0    34551 2022-05-26 19:13:09.343380 open_gopro-0.9.1/open_gopro/api/ble_commands.py
--rw-r--r--   0        0        0    30686 2022-05-26 19:13:09.343380 open_gopro-0.9.1/open_gopro/api/builders.py
--rw-r--r--   0        0        0     5413 2022-05-26 19:13:09.344380 open_gopro-0.9.1/open_gopro/api/params.py
--rw-r--r--   0        0        0    16789 2022-05-26 19:13:09.344380 open_gopro-0.9.1/open_gopro/api/wifi_commands.py
--rw-r--r--   0        0        0      558 2022-02-07 21:15:19.774802 open_gopro-0.9.1/open_gopro/ble/__init__.py
--rw-r--r--   0        0        0      287 2022-02-07 21:15:19.775802 open_gopro-0.9.1/open_gopro/ble/adapters/__init__.py
--rw-r--r--   0        0        0    16789 2022-05-26 19:13:09.345380 open_gopro-0.9.1/open_gopro/ble/adapters/bleak_wrapper.py
--rw-r--r--   0        0        0     7426 2022-05-26 19:13:09.346380 open_gopro-0.9.1/open_gopro/ble/client.py
--rw-r--r--   0        0        0     4287 2022-05-20 17:53:53.629594 open_gopro-0.9.1/open_gopro/ble/controller.py
--rw-r--r--   0        0        0    21278 2022-05-26 19:13:09.346380 open_gopro-0.9.1/open_gopro/ble/services.py
--rw-r--r--   0        0        0     5818 2022-05-26 19:13:09.347380 open_gopro-0.9.1/open_gopro/communication_client.py
--rw-r--r--   0        0        0    10057 2022-05-16 20:18:18.779238 open_gopro-0.9.1/open_gopro/constants.py
--rw-r--r--   0        0        0      223 2022-02-07 21:15:19.778802 open_gopro-0.9.1/open_gopro/demos/__init__.py
--rw-r--r--   0        0        0     2529 2022-05-20 17:53:41.487153 open_gopro-0.9.1/open_gopro/demos/connect_wifi.py
--rw-r--r--   0        0        0     6558 2022-05-26 22:48:27.829373 open_gopro-0.9.1/open_gopro/demos/log_battery.py
--rw-r--r--   0        0        0     4273 2022-05-26 19:13:09.348378 open_gopro-0.9.1/open_gopro/demos/photo.py
--rw-r--r--   0        0        0     3279 2022-05-20 17:53:41.489155 open_gopro-0.9.1/open_gopro/demos/stream.py
--rw-r--r--   0        0        0     4079 2022-05-20 17:53:41.489155 open_gopro-0.9.1/open_gopro/demos/video.py
--rw-r--r--   0        0        0     2362 2022-02-07 22:04:28.390238 open_gopro-0.9.1/open_gopro/exceptions.py
--rw-r--r--   0        0        0    31169 2022-05-26 19:13:09.349377 open_gopro-0.9.1/open_gopro/gopro.py
--rw-r--r--   0        0        0      569 2022-02-07 21:15:19.782804 open_gopro-0.9.1/open_gopro/proto/__init__.py
--rw-r--r--   0        0        0     5627 2022-05-18 17:15:41.063285 open_gopro-0.9.1/open_gopro/proto/preset_status_pb.py
--rw-r--r--   0        0        0      781 2022-05-18 17:15:41.064183 open_gopro-0.9.1/open_gopro/proto/request_get_preset_status_pb.py
--rw-r--r--   0        0        0      688 2022-05-18 17:15:41.064183 open_gopro-0.9.1/open_gopro/proto/response_generic_pb.py
--rw-r--r--   0        0        0      651 2022-05-18 17:15:41.065183 open_gopro-0.9.1/open_gopro/proto/set_camera_control_status_pb.py
--rw-r--r--   0        0        0      459 2022-05-18 17:15:41.066183 open_gopro-0.9.1/open_gopro/proto/turbo_transfer_pb.py
--rw-r--r--   0        0        0    20364 2022-05-26 19:13:09.349377 open_gopro-0.9.1/open_gopro/responses.py
--rw-r--r--   0        0        0    16724 2022-05-27 18:57:34.879418 open_gopro-0.9.1/open_gopro/util.py
--rw-r--r--   0        0        0      310 2022-02-07 21:15:19.786802 open_gopro-0.9.1/open_gopro/wifi/__init__.py
--rw-r--r--   0        0        0      274 2022-02-07 21:15:19.786802 open_gopro-0.9.1/open_gopro/wifi/adapters/__init__.py
--rw-r--r--   0        0        0    29079 2022-05-26 19:13:09.351761 open_gopro-0.9.1/open_gopro/wifi/adapters/wireless.py
--rw-r--r--   0        0        0     2278 2022-05-26 19:13:09.351761 open_gopro-0.9.1/open_gopro/wifi/client.py
--rw-r--r--   0        0        0     4323 2022-05-26 19:13:09.352727 open_gopro-0.9.1/open_gopro/wifi/controller.py
--rw-r--r--   0        0        0     7811 2022-05-27 18:57:34.879418 open_gopro-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     5088 2022-02-07 22:04:28.377234 open_gopro-0.9.1/README.md
--rw-r--r--   0        0        0     6777 2022-05-27 18:57:53.543648 open_gopro-0.9.1/setup.py
--rw-r--r--   0        0        0     6459 2022-05-27 18:57:53.544648 open_gopro-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0      506 2022-06-06 21:59:09.181953 open_gopro-0.9.2/open_gopro/__init__.py
+-rw-r--r--   0        0        0      377 2022-02-07 21:15:19.771803 open_gopro-0.9.2/open_gopro/api/__init__.py
+-rw-r--r--   0        0        0     1058 2022-05-26 19:13:09.342380 open_gopro-0.9.2/open_gopro/api/api.py
+-rw-r--r--   0        0        0    34551 2022-05-26 19:13:09.343380 open_gopro-0.9.2/open_gopro/api/ble_commands.py
+-rw-r--r--   0        0        0    30686 2022-05-26 19:13:09.343380 open_gopro-0.9.2/open_gopro/api/builders.py
+-rw-r--r--   0        0        0     5413 2022-05-26 19:13:09.344380 open_gopro-0.9.2/open_gopro/api/params.py
+-rw-r--r--   0        0        0    16789 2022-05-26 19:13:09.344380 open_gopro-0.9.2/open_gopro/api/wifi_commands.py
+-rw-r--r--   0        0        0      558 2022-02-07 21:15:19.774802 open_gopro-0.9.2/open_gopro/ble/__init__.py
+-rw-r--r--   0        0        0      287 2022-02-07 21:15:19.775802 open_gopro-0.9.2/open_gopro/ble/adapters/__init__.py
+-rw-r--r--   0        0        0    16789 2022-05-26 19:13:09.345380 open_gopro-0.9.2/open_gopro/ble/adapters/bleak_wrapper.py
+-rw-r--r--   0        0        0     7426 2022-05-26 19:13:09.346380 open_gopro-0.9.2/open_gopro/ble/client.py
+-rw-r--r--   0        0        0     4287 2022-05-20 17:53:53.629594 open_gopro-0.9.2/open_gopro/ble/controller.py
+-rw-r--r--   0        0        0    21278 2022-05-26 19:13:09.346380 open_gopro-0.9.2/open_gopro/ble/services.py
+-rw-r--r--   0        0        0     5818 2022-05-26 19:13:09.347380 open_gopro-0.9.2/open_gopro/communication_client.py
+-rw-r--r--   0        0        0    10057 2022-05-16 20:18:18.779238 open_gopro-0.9.2/open_gopro/constants.py
+-rw-r--r--   0        0        0      223 2022-02-07 21:15:19.778802 open_gopro-0.9.2/open_gopro/demos/__init__.py
+-rw-r--r--   0        0        0     2529 2022-05-20 17:53:41.487153 open_gopro-0.9.2/open_gopro/demos/connect_wifi.py
+-rw-r--r--   0        0        0     6558 2022-05-27 22:37:01.147405 open_gopro-0.9.2/open_gopro/demos/log_battery.py
+-rw-r--r--   0        0        0     4273 2022-05-26 19:13:09.348378 open_gopro-0.9.2/open_gopro/demos/photo.py
+-rw-r--r--   0        0        0     3279 2022-05-20 17:53:41.489155 open_gopro-0.9.2/open_gopro/demos/stream.py
+-rw-r--r--   0        0        0     4079 2022-05-20 17:53:41.489155 open_gopro-0.9.2/open_gopro/demos/video.py
+-rw-r--r--   0        0        0     2362 2022-02-07 22:04:28.390238 open_gopro-0.9.2/open_gopro/exceptions.py
+-rw-r--r--   0        0        0    31169 2022-05-26 19:13:09.349377 open_gopro-0.9.2/open_gopro/gopro.py
+-rw-r--r--   0        0        0      569 2022-02-07 21:15:19.782804 open_gopro-0.9.2/open_gopro/proto/__init__.py
+-rw-r--r--   0        0        0     5627 2022-05-18 17:15:41.063285 open_gopro-0.9.2/open_gopro/proto/preset_status_pb.py
+-rw-r--r--   0        0        0      781 2022-05-18 17:15:41.064183 open_gopro-0.9.2/open_gopro/proto/request_get_preset_status_pb.py
+-rw-r--r--   0        0        0      688 2022-05-18 17:15:41.064183 open_gopro-0.9.2/open_gopro/proto/response_generic_pb.py
+-rw-r--r--   0        0        0      651 2022-05-18 17:15:41.065183 open_gopro-0.9.2/open_gopro/proto/set_camera_control_status_pb.py
+-rw-r--r--   0        0        0      459 2022-05-18 17:15:41.066183 open_gopro-0.9.2/open_gopro/proto/turbo_transfer_pb.py
+-rw-r--r--   0        0        0    20364 2022-05-26 19:13:09.349377 open_gopro-0.9.2/open_gopro/responses.py
+-rw-r--r--   0        0        0    16724 2022-05-27 18:57:34.879418 open_gopro-0.9.2/open_gopro/util.py
+-rw-r--r--   0        0        0      310 2022-02-07 21:15:19.786802 open_gopro-0.9.2/open_gopro/wifi/__init__.py
+-rw-r--r--   0        0        0      274 2022-02-07 21:15:19.786802 open_gopro-0.9.2/open_gopro/wifi/adapters/__init__.py
+-rw-r--r--   0        0        0    29079 2022-05-26 19:13:09.351761 open_gopro-0.9.2/open_gopro/wifi/adapters/wireless.py
+-rw-r--r--   0        0        0     2278 2022-05-26 19:13:09.351761 open_gopro-0.9.2/open_gopro/wifi/client.py
+-rw-r--r--   0        0        0     4323 2022-05-26 19:13:09.352727 open_gopro-0.9.2/open_gopro/wifi/controller.py
+-rw-r--r--   0        0        0     7811 2022-06-06 22:11:05.426202 open_gopro-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     5088 2022-02-07 22:04:28.377234 open_gopro-0.9.2/README.md
+-rw-r--r--   0        0        0     6777 2022-06-06 22:11:35.744831 open_gopro-0.9.2/setup.py
+-rw-r--r--   0        0        0     6459 2022-06-06 22:11:35.744831 open_gopro-0.9.2/PKG-INFO
```

### Comparing `open_gopro-0.9.1/open_gopro/api/api.py` & `open_gopro-0.9.2/open_gopro/api/api.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/api/ble_commands.py` & `open_gopro-0.9.2/open_gopro/api/ble_commands.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/api/builders.py` & `open_gopro-0.9.2/open_gopro/api/builders.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/api/params.py` & `open_gopro-0.9.2/open_gopro/api/params.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/api/wifi_commands.py` & `open_gopro-0.9.2/open_gopro/api/wifi_commands.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/ble/__init__.py` & `open_gopro-0.9.2/open_gopro/ble/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/ble/adapters/bleak_wrapper.py` & `open_gopro-0.9.2/open_gopro/ble/adapters/bleak_wrapper.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/ble/client.py` & `open_gopro-0.9.2/open_gopro/ble/client.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/ble/controller.py` & `open_gopro-0.9.2/open_gopro/ble/controller.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/ble/services.py` & `open_gopro-0.9.2/open_gopro/ble/services.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/communication_client.py` & `open_gopro-0.9.2/open_gopro/communication_client.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/constants.py` & `open_gopro-0.9.2/open_gopro/constants.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/demos/connect_wifi.py` & `open_gopro-0.9.2/open_gopro/demos/connect_wifi.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/demos/log_battery.py` & `open_gopro-0.9.2/open_gopro/demos/log_battery.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/demos/photo.py` & `open_gopro-0.9.2/open_gopro/demos/photo.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/demos/stream.py` & `open_gopro-0.9.2/open_gopro/demos/stream.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/demos/video.py` & `open_gopro-0.9.2/open_gopro/demos/video.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/exceptions.py` & `open_gopro-0.9.2/open_gopro/exceptions.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/gopro.py` & `open_gopro-0.9.2/open_gopro/gopro.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/proto/__init__.py` & `open_gopro-0.9.2/open_gopro/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/proto/preset_status_pb.py` & `open_gopro-0.9.2/open_gopro/proto/preset_status_pb.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/proto/request_get_preset_status_pb.py` & `open_gopro-0.9.2/open_gopro/proto/request_get_preset_status_pb.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/proto/response_generic_pb.py` & `open_gopro-0.9.2/open_gopro/proto/response_generic_pb.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/proto/set_camera_control_status_pb.py` & `open_gopro-0.9.2/open_gopro/proto/set_camera_control_status_pb.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/responses.py` & `open_gopro-0.9.2/open_gopro/responses.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/util.py` & `open_gopro-0.9.2/open_gopro/util.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/wifi/adapters/wireless.py` & `open_gopro-0.9.2/open_gopro/wifi/adapters/wireless.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/wifi/client.py` & `open_gopro-0.9.2/open_gopro/wifi/client.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/open_gopro/wifi/controller.py` & `open_gopro-0.9.2/open_gopro/wifi/controller.py`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/pyproject.toml` & `open_gopro-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #=======================================================================================
 #============================= PACKAGE CONFIGURATION  ==================================
 #=======================================================================================
 [tool.poetry]
 name = "open_gopro"
-version = "0.9.1"
+version = "0.9.2"
 description = "Open GoPro API and Examples"
 authors = ["Tim Camise <tcamise@gopro.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/gopro/OpenGoPro/tree/main/demos/python/sdk_wireless_camera_control"
 documentation = "https://gopro.github.io/OpenGoPro/"
 classifiers = [
```

### Comparing `open_gopro-0.9.1/README.md` & `open_gopro-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `open_gopro-0.9.1/setup.py` & `open_gopro-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                      'gopro-photo = open_gopro.demos.photo:entrypoint',
                      'gopro-stream = open_gopro.demos.stream:main',
                      'gopro-video = open_gopro.demos.video:main',
                      'gopro-wifi = open_gopro.demos.connect_wifi:main']}
 
 setup_kwargs = {
     'name': 'open-gopro',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Open GoPro API and Examples',
     'long_description': '# Open GoPro Python SDK\n\n<img alt="GoPro Logo" src="https://raw.githubusercontent.com/gopro/OpenGoPro/main/docs/assets/images/logos/logo.png" width="50%" style="max-width: 500px;"/>\n\n[![Build and Test](https://img.shields.io/github/workflow/status/gopro/OpenGoPro/Python%20SDK%20Testing?label=Build%20and%20Test)](https://github.com/gopro/OpenGoPro/actions/workflows/python_sdk_test.yml)\n[![Build Docs](https://img.shields.io/github/workflow/status/gopro/OpenGoPro/Python%20SDK%20Docs%20Build%20and%20Deploy?label=Docs)](https://github.com/gopro/OpenGoPro/actions/workflows/python_sdk_deploy_docs.yml)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![PyPI](https://img.shields.io/pypi/v/open-gopro)](https://pypi.org/project/open-gopro/)\n[![MIT License](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/gopro/OpenGoPro/blob/main/LICENSE)\n![Coverage](https://raw.githubusercontent.com/gopro/OpenGoPro/main/demos/python/sdk_wireless_camera_control/docs/_static/coverage.svg)\n\nThis is a Python package that provides an interface for the user to exercise the Open GoPro Bluetooth Low\nEnergy (BLE) and Wi-Fi API\'s as well as install command line interfaces to take photos, videos, and view\nthe preview stream.\n\n-   Free software: MIT license\n-   Documentation: [View on Open GoPro](https://gopro.github.io/OpenGoPro/python_sdk/)\n-   View on [Github](https://github.com/gopro/OpenGoPro/tree/main/demos/python/sdk_wireless_camera_control)\n\n## Documentation\n\n> Note! This README is only an overview of the package.\n\nComplete documentation can be found on [Open GoPro](https://gopro.github.io/OpenGoPro/python_sdk/)\n\n## Features\n\n-   Top-level GoPro class interface to use both BLE / WiFi\n-   Cross-platform (tested on MacOS Big Sur, Windows 10, and Ubuntu 20.04)\n    -   BLE implemented using [bleak](https://pypi.org/project/bleak/)\n    -   Wi-Fi controller provided in the Open GoPro package (loosely based on the [Wireless Library](https://pypi.org/project/wireless/)\n-   Supports all commands, settings, and statuses from the [Open GoPro API](https://gopro.github.io/OpenGoPro/)\n-   Supports all versions of the Open GoPro API\n-   Automatically handles connection maintenance:\n    -   manage camera ready / encoding\n    -   periodically sends keep alive signals\n-   Includes detailed logging for each module\n-   Includes demo scripts installed as command-line applications to show BLE and WiFi functionality\n    -   Take a photo\n    -   Take a video\n    -   View the live stream\n    -   Log the battery\n\n## Installation\n\n> Note! This package requires Python >= 3.8\n\n```console\n    $ pip install open-gopro\n```\n\n## Usage\n\nTo automatically connect to GoPro device via BLE and WiFI, set the preset, set video parameters, take a\nvideo, and download all files:\n\n```python\nimport time\nfrom open_gopro import GoPro, Params\n\nwith GoPro() as gopro:\n    gopro.ble_command.load_preset(Params.Preset.CINEMATIC)\n    gopro.ble_setting.resolution.set(Params.Resolution.RES_4K)\n    gopro.ble_setting.fps.set(Params.FPS.FPS_30)\n    gopro.ble_command.set_shutter(Params.Shutter.ON)\n    time.sleep(2) # Record for 2 seconds\n    gopro.ble_command.set_shutter(Params.Shutter.OFF)\n\n    # Download all of the files from the camera\n    media_list = [x["n"] for x in gopro.wifi_command.get_media_list().flatten\n    for file in media_list:\n        gopro.wifi_command.download_file(camera_file=file)\n```\n\nAnd much more!\n\n## Demos\n\n> Note! These demos can be found on [Github](https://github.com/gopro/OpenGoPro/tree/main/demos/python/sdk_wireless_camera_control/open_gopro/demos)\n\nDemos can be found in the installed package in the "demos" folder. They are installed as a CLI entrypoint\nand can be run via:\n\nCapture a photo and download it to your computer:\n\n```bash\n$ gopro-photo\n```\n\nCapture a video and download it to your computer:\n\n```bash\n$ gopro-video\n```\n\nStart the preview stream and view it with [VLC](https://www.videolan.org/):\n\n```bash\n$ gopro-stream\n```\n\nConnect to the GoPro and log battery consumption in to a .csv:\n\n```bash\n$ gopro-log-battery\n```\n\nConnect to the GoPro\'s Wi-Fi AP and maintain the connection:\n\n```bash\n$ gopro-wifi\n```\n\nFor more information on each, try running with help as such:\n\n```bash\n$ gopro-photo --help\n\nusage: gopro-photo [-h] [-i IDENTIFIER] [-l LOG] [-o OUTPUT] [-w WIFI_INTERFACE]\n\nConnect to a GoPro camera, take a photo, then download it.\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -i IDENTIFIER, --identifier IDENTIFIER\n                        Last 4 digits of GoPro serial number, which is the last 4 digits of the default camera SSID. If not used, first\n                        discovered GoPro will be connected to\n  -l LOG, --log LOG     Location to store detailed log\n  -o OUTPUT, --output OUTPUT\n                        Where to write the photo to. If not set, write to \'photo.jpg\'\n  -w WIFI_INTERFACE, --wifi_interface WIFI_INTERFACE\n                        System Wifi Interface. If not set, first discovered interface will be used.\n```\n',
     'author': 'Tim Camise',
     'author_email': 'tcamise@gopro.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/gopro/OpenGoPro/tree/main/demos/python/sdk_wireless_camera_control',
```

### Comparing `open_gopro-0.9.1/PKG-INFO` & `open_gopro-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-gopro
-Version: 0.9.1
+Version: 0.9.2
 Summary: Open GoPro API and Examples
 Home-page: https://github.com/gopro/OpenGoPro/tree/main/demos/python/sdk_wireless_camera_control
 License: MIT
 Author: Tim Camise
 Author-email: tcamise@gopro.com
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

