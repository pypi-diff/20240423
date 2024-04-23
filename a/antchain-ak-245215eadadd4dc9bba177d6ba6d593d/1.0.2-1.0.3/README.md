# Comparing `tmp/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar.gz` & `tmp/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar", last modified: Thu Apr 11 03:38:57 2024, max compression
+gzip compressed data, was "dist/antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3.tar", last modified: Tue Apr 23 06:06:26 2024, max compression
```

## Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2.tar` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2354 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      900 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2354 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      579 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      108 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24398 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py
--rw-r--r--   0 root         (0) root         (0)    39483 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-11 03:38:57.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2024-04-11 03:38:56.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/
+-rw-r--r--   0 root         (0) root         (0)      600 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      900 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2354 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      579 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      108 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24398 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py
+-rw-r--r--   0 root         (0) root         (0)    40027 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2651 2024-04-23 06:06:26.000000 antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/setup.py
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/LICENSE` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/PKG-INFO` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain_ak_245215eadadd4dc9bba177d6ba6d593d
-Version: 1.0.2
+Name: antchain-ak-245215eadadd4dc9bba177d6ba6d593d
+Version: 1.0.3
 Summary: Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README-CN.md` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/README.md` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/PKG-INFO` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: antchain-ak-245215eadadd4dc9bba177d6ba6d593d
-Version: 1.0.2
+Name: antchain_ak_245215eadadd4dc9bba177d6ba6d593d
+Version: 1.0.3
 Summary: Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_ak_245215eadadd4dc9bba177d6ba6d593d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_245215eadadd4dc9bba177d6ba6d593d',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.0.2',
+                    'sdk_version': '1.0.3',
                     '_prod_code': 'ak_245215eadadd4dc9bba177d6ba6d593d',
                     '_prod_channel': 'saas'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,28 +203,31 @@
         self,
         avatar_id: str = None,
         name: str = None,
         type: str = None,
         conf: str = None,
         pic_url: str = None,
         bg_url: str = None,
+        thumb_url: str = None,
     ):
         # 190087
         self.avatar_id = avatar_id
         # 数字人形象名称
         self.name = name
         # CUSTOM---定制；
         # PRESET---预置
         self.type = type
         # 位置信息等配置信息
         self.conf = conf
         # 数字人形象图片
         self.pic_url = pic_url
         # 背景图片地址
         self.bg_url = bg_url
+        # 形象thumb图Url
+        self.thumb_url = thumb_url
 
     def validate(self):
         self.validate_required(self.avatar_id, 'avatar_id')
         self.validate_required(self.name, 'name')
         self.validate_required(self.type, 'type')
         self.validate_required(self.pic_url, 'pic_url')
 
@@ -242,14 +245,16 @@
             result['type'] = self.type
         if self.conf is not None:
             result['conf'] = self.conf
         if self.pic_url is not None:
             result['pic_url'] = self.pic_url
         if self.bg_url is not None:
             result['bg_url'] = self.bg_url
+        if self.thumb_url is not None:
+            result['thumb_url'] = self.thumb_url
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('avatar_id') is not None:
             self.avatar_id = m.get('avatar_id')
         if m.get('name') is not None:
@@ -258,14 +263,16 @@
             self.type = m.get('type')
         if m.get('conf') is not None:
             self.conf = m.get('conf')
         if m.get('pic_url') is not None:
             self.pic_url = m.get('pic_url')
         if m.get('bg_url') is not None:
             self.bg_url = m.get('bg_url')
+        if m.get('thumb_url') is not None:
+            self.thumb_url = m.get('thumb_url')
         return self
 
 
 class Paster(TeaModel):
     def __init__(
         self,
         x: int = None,
@@ -930,14 +937,15 @@
         profile_info: ProfileInfo = None,
         script_voice_config: ScriptVoiceConfig = None,
         open_captions: bool = None,
         captions_info: CaptionsInfo = None,
         replace_sensitive: bool = None,
         background: Background = None,
         pasters: List[Paster] = None,
+        format: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 数字人id
         self.avatar_id = avatar_id
         # text/audio, 合成驱动--文本/音频
@@ -952,14 +960,16 @@
         self.captions_info = captions_info
         # 是否替换字幕敏感词
         self.replace_sensitive = replace_sensitive
         # 背景信息
         self.background = background
         # 贴片元素信息
         self.pasters = pasters
+        # 数字人视频生成格式，默认不填
+        self.format = format
 
     def validate(self):
         self.validate_required(self.avatar_id, 'avatar_id')
         self.validate_required(self.driver_type, 'driver_type')
         if self.profile_info:
             self.profile_info.validate()
         self.validate_required(self.script_voice_config, 'script_voice_config')
@@ -1001,14 +1011,16 @@
             result['replace_sensitive'] = self.replace_sensitive
         if self.background is not None:
             result['background'] = self.background.to_map()
         result['pasters'] = []
         if self.pasters is not None:
             for k in self.pasters:
                 result['pasters'].append(k.to_map() if k else None)
+        if self.format is not None:
+            result['format'] = self.format
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
@@ -1034,14 +1046,16 @@
             temp_model = Background()
             self.background = temp_model.from_map(m['background'])
         self.pasters = []
         if m.get('pasters') is not None:
             for k in m.get('pasters'):
                 temp_model = Paster()
                 self.pasters.append(temp_model.from_map(k))
+        if m.get('format') is not None:
+            self.format = m.get('format')
         return self
 
 
 class CreateUniversalsaasDigitalhumanVideoTaskResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
```

### Comparing `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.2/setup.py` & `antchain_ak_245215eadadd4dc9bba177d6ba6d593d-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_ak_245215eadadd4dc9bba177d6ba6d593d.
 
-Created on 11/04/2024
+Created on 23/04/2024
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_ak_245215eadadd4dc9bba177d6ba6d593d"
 NAME = "antchain_ak_245215eadadd4dc9bba177d6ba6d593d" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain Ak_245215eadadd4dc9bba177d6ba6d593d SDK Library for Python"
```

