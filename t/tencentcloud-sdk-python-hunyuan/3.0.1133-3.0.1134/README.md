# Comparing `tmp/tencentcloud-sdk-python-hunyuan-3.0.1133.tar.gz` & `tmp/tencentcloud-sdk-python-hunyuan-3.0.1134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1133.tar", last modified: Sun Apr 21 20:53:56 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hunyuan-3.0.1134.tar", last modified: Mon Apr 22 20:55:38 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133.tar` & `tencentcloud-sdk-python-hunyuan-3.0.1134.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/
--rw-r--r--   0 root         (0) root         (0)     2094 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    30308 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5295 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/hunyuan_client.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1081 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/setup.py
--rw-r--r--   0 root         (0) root         (0)      749 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1680 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      539 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-21 20:53:56.000000 tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/
+-rw-r--r--   0 root         (0) root         (0)     2094 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    30312 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5369 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/hunyuan_client.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1081 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/setup.py
+-rw-r--r--   0 root         (0) root         (0)      749 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      539 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-22 20:55:38.000000 tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/requires.txt
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1134/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1133
+Version: 3.0.1134
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1133'
+__version__ = '3.0.1134'
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/errorcodes.py` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/models.py` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,23 +620,23 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class EmbeddingUsage(AbstractModel):
-    """token 使用计数。
+    """Token 使用计数。
 
     """
 
     def __init__(self):
         r"""
-        :param _PromptTokens: 输入Token数。
+        :param _PromptTokens: 输入 Token 数。
         :type PromptTokens: int
-        :param _TotalTokens: 总Token数。
+        :param _TotalTokens: 总 Token 数。
         :type TotalTokens: int
         """
         self._PromptTokens = None
         self._TotalTokens = None
 
     @property
     def PromptTokens(self):
@@ -941,25 +941,25 @@
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class Usage(AbstractModel):
-    """token 数量
+    """Token 数量
 
     """
 
     def __init__(self):
         r"""
-        :param _PromptTokens: 输入 token 数量。
+        :param _PromptTokens: 输入 Token 数量。
         :type PromptTokens: int
-        :param _CompletionTokens: 输出 token 数量。
+        :param _CompletionTokens: 输出 Token 数量。
         :type CompletionTokens: int
-        :param _TotalTokens: 总 token 数量。
+        :param _TotalTokens: 总 Token 数量。
         :type TotalTokens: int
         """
         self._PromptTokens = None
         self._CompletionTokens = None
         self._TotalTokens = None
 
     @property
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud/hunyuan/v20230901/hunyuan_client.py` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud/hunyuan/v20230901/hunyuan_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         :param request: Request instance for ChatPro.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatProRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatProResponse`
 
         """
         try:
             params = request._serialize()
-            return self.call_sse("ChatPro", params, headers=request.headers)
+            return self._call_and_deserialize("ChatPro", params, models.ChatProResponse, headers=request.headers)
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
@@ -58,15 +58,15 @@
         :param request: Request instance for ChatStd.
         :type request: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdRequest`
         :rtype: :class:`tencentcloud.hunyuan.v20230901.models.ChatStdResponse`
 
         """
         try:
             params = request._serialize()
-            return self.call_sse("ChatStd", params, headers=request.headers)
+            return self._call_and_deserialize("ChatStd", params, models.ChatStdResponse, headers=request.headers)
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/setup.py` & `tencentcloud-sdk-python-hunyuan-3.0.1134/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hunyuan',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1133"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1134"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hunyuan SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/README.rst` & `tencentcloud-sdk-python-hunyuan-3.0.1134/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hunyuan
-Version: 3.0.1133
+Version: 3.0.1134
 Summary: Tencent Cloud Hunyuan SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hunyuan-3.0.1133/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-hunyuan-3.0.1134/tencentcloud_sdk_python_hunyuan.egg-info/SOURCES.txt`

 * *Files identical despite different names*
