# Comparing `tmp/tencentcloud-sdk-python-lke-3.0.1133.tar.gz` & `tmp/tencentcloud-sdk-python-lke-3.0.1134.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1133.tar", last modified: Sun Apr 21 21:03:05 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-lke-3.0.1134.tar", last modified: Mon Apr 22 20:59:37 2024, max compression
```

## Comparing `tencentcloud-sdk-python-lke-3.0.1133.tar` & `tencentcloud-sdk-python-lke-3.0.1134.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/requires.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   362568 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/models.py
--rw-r--r--   0 root         (0) root         (0)    65316 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/lke_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/__init__.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-04-21 21:03:05.000000 tencentcloud-sdk-python-lke-3.0.1133/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   365878 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/models.py
+-rw-r--r--   0 root         (0) root         (0)    65638 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/lke_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-04-22 20:59:37.000000 tencentcloud-sdk-python-lke-3.0.1134/README.rst
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1134/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1133
+Version: 3.0.1134
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/tencentcloud_sdk_python_lke.egg-info/PKG-INFO` & `tencentcloud-sdk-python-lke-3.0.1134/tencentcloud_sdk_python_lke.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-lke
-Version: 3.0.1133
+Version: 3.0.1134
 Summary: Tencent Cloud Lke SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/__init__.py` & `tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/errorcodes.py` & `tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/models.py` & `tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -5265,29 +5265,40 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Data: 特征
         :type Data: list of EmbeddingObject
+        :param _Usage: 消耗量，返回TotalToken
+        :type Usage: :class:`tencentcloud.lke.v20231130.models.Usage`
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Data = None
+        self._Usage = None
         self._RequestId = None
 
     @property
     def Data(self):
         return self._Data
 
     @Data.setter
     def Data(self, Data):
         self._Data = Data
 
     @property
+    def Usage(self):
+        return self._Usage
+
+    @Usage.setter
+    def Usage(self, Usage):
+        self._Usage = Usage
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
@@ -5295,14 +5306,17 @@
     def _deserialize(self, params):
         if params.get("Data") is not None:
             self._Data = []
             for item in params.get("Data"):
                 obj = EmbeddingObject()
                 obj._deserialize(item)
                 self._Data.append(obj)
+        if params.get("Usage") is not None:
+            self._Usage = Usage()
+            self._Usage._deserialize(params.get("Usage"))
         self._RequestId = params.get("RequestId")
 
 
 class GetMsgRecordRequest(AbstractModel):
     """GetMsgRecord请求参数结构体
 
     """
@@ -10729,15 +10743,15 @@
         :type Name: str
         :param _Url: 文件下载链接 (支持的文件类型: docx, txt, markdown, pdf)
         :type Url: str
         :param _TaskId: 任务ID, 用于幂等去重, 业务自行定义(最大长度64字节)
         :type TaskId: str
         :param _Policy: 切分策略
         :type Policy: str
-        :param _Operate: 默认值: split
+        :param _Operate: 默认值: parse
         :type Operate: str
         """
         self._Name = None
         self._Url = None
         self._TaskId = None
         self._Policy = None
         self._Operate = None
@@ -10772,18 +10786,22 @@
 
     @Policy.setter
     def Policy(self, Policy):
         self._Policy = Policy
 
     @property
     def Operate(self):
+        warnings.warn("parameter `Operate` is deprecated", DeprecationWarning) 
+
         return self._Operate
 
     @Operate.setter
     def Operate(self, Operate):
+        warnings.warn("parameter `Operate` is deprecated", DeprecationWarning) 
+
         self._Operate = Operate
 
 
     def _deserialize(self, params):
         self._Name = params.get("Name")
         self._Url = params.get("Url")
         self._TaskId = params.get("TaskId")
@@ -11247,21 +11265,24 @@
         :type Status: str
         :param _Name: 解析后的文件内容
         :type Name: str
         :param _Url: 文件下载地址
         :type Url: str
         :param _Reason: 解析失败原因
         :type Reason: str
+        :param _Usage: 消耗量，输出页数
+        :type Usage: :class:`tencentcloud.lke.v20231130.models.Usage`
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Status = None
         self._Name = None
         self._Url = None
         self._Reason = None
+        self._Usage = None
         self._RequestId = None
 
     @property
     def Status(self):
         return self._Status
 
     @Status.setter
@@ -11289,27 +11310,38 @@
         return self._Reason
 
     @Reason.setter
     def Reason(self, Reason):
         self._Reason = Reason
 
     @property
+    def Usage(self):
+        return self._Usage
+
+    @Usage.setter
+    def Usage(self, Usage):
+        self._Usage = Usage
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._Status = params.get("Status")
         self._Name = params.get("Name")
         self._Url = params.get("Url")
         self._Reason = params.get("Reason")
+        if params.get("Usage") is not None:
+            self._Usage = Usage()
+            self._Usage._deserialize(params.get("Usage"))
         self._RequestId = params.get("RequestId")
 
 
 class QueryRewriteRequest(AbstractModel):
     """QueryRewrite请求参数结构体
 
     """
@@ -11376,39 +11408,53 @@
 
     """
 
     def __init__(self):
         r"""
         :param _Content: 改写结果
         :type Content: str
+        :param _Usage: 消耗量，返回输入token数，输出token数以及总token数
+        :type Usage: :class:`tencentcloud.lke.v20231130.models.Usage`
         :param _RequestId: 唯一请求 ID，由服务端生成，每次请求都会返回（若请求因其他原因未能抵达服务端，则该次请求不会获得 RequestId）。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
         self._Content = None
+        self._Usage = None
         self._RequestId = None
 
     @property
     def Content(self):
         return self._Content
 
     @Content.setter
     def Content(self, Content):
         self._Content = Content
 
     @property
+    def Usage(self):
+        return self._Usage
+
+    @Usage.setter
+    def Usage(self, Usage):
+        self._Usage = Usage
+
+    @property
     def RequestId(self):
         return self._RequestId
 
     @RequestId.setter
     def RequestId(self, RequestId):
         self._RequestId = RequestId
 
 
     def _deserialize(self, params):
         self._Content = params.get("Content")
+        if params.get("Usage") is not None:
+            self._Usage = Usage()
+            self._Usage._deserialize(params.get("Usage"))
         self._RequestId = params.get("RequestId")
 
 
 class RateMsgRecordRequest(AbstractModel):
     """RateMsgRecord请求参数结构体
 
     """
@@ -13267,14 +13313,83 @@
     def _deserialize(self, params):
         self._ErrorMsg = params.get("ErrorMsg")
         self._ErrorLink = params.get("ErrorLink")
         self._ErrorLinkText = params.get("ErrorLinkText")
         self._RequestId = params.get("RequestId")
 
 
+class Usage(AbstractModel):
+    """消耗量
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalPages: 文档页数
+        :type TotalPages: int
+        :param _InputTokens: 输入token数
+        :type InputTokens: int
+        :param _OutputTokens: 输出token数
+        :type OutputTokens: int
+        :param _TotalTokens: 总token数
+        :type TotalTokens: int
+        """
+        self._TotalPages = None
+        self._InputTokens = None
+        self._OutputTokens = None
+        self._TotalTokens = None
+
+    @property
+    def TotalPages(self):
+        return self._TotalPages
+
+    @TotalPages.setter
+    def TotalPages(self, TotalPages):
+        self._TotalPages = TotalPages
+
+    @property
+    def InputTokens(self):
+        return self._InputTokens
+
+    @InputTokens.setter
+    def InputTokens(self, InputTokens):
+        self._InputTokens = InputTokens
+
+    @property
+    def OutputTokens(self):
+        return self._OutputTokens
+
+    @OutputTokens.setter
+    def OutputTokens(self, OutputTokens):
+        self._OutputTokens = OutputTokens
+
+    @property
+    def TotalTokens(self):
+        return self._TotalTokens
+
+    @TotalTokens.setter
+    def TotalTokens(self, TotalTokens):
+        self._TotalTokens = TotalTokens
+
+
+    def _deserialize(self, params):
+        self._TotalPages = params.get("TotalPages")
+        self._InputTokens = params.get("InputTokens")
+        self._OutputTokens = params.get("OutputTokens")
+        self._TotalTokens = params.get("TotalTokens")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class VerifyQARequest(AbstractModel):
     """VerifyQA请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/tencentcloud/lke/v20231130/lke_client.py` & `tencentcloud-sdk-python-lke-3.0.1134/tencentcloud/lke/v20231130/lke_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -783,14 +783,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def GetEmbedding(self, request):
         """获取特征向量
+        本接口有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
 
         :param request: Request instance for GetEmbedding.
         :type request: :class:`tencentcloud.lke.v20231130.models.GetEmbeddingRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.GetEmbeddingResponse`
 
         """
         try:
@@ -1519,14 +1520,15 @@
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def QueryRewrite(self, request):
         """多轮改写
+        本接口有单账号调用上限控制，如您有提高并发限制的需求请 [联系我们](https://cloud.tencent.com/act/event/Online_service) 。
 
         :param request: Request instance for QueryRewrite.
         :type request: :class:`tencentcloud.lke.v20231130.models.QueryRewriteRequest`
         :rtype: :class:`tencentcloud.lke.v20231130.models.QueryRewriteResponse`
 
         """
         try:
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/setup.py` & `tencentcloud-sdk-python-lke-3.0.1134/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-lke',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1133"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1134"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Lke SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-lke-3.0.1133/README.rst` & `tencentcloud-sdk-python-lke-3.0.1134/README.rst`

 * *Files identical despite different names*

