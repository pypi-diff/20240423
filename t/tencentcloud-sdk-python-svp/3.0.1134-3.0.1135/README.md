# Comparing `tmp/tencentcloud-sdk-python-svp-3.0.1134.tar.gz` & `tmp/tencentcloud-sdk-python-svp-3.0.1135.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-svp-3.0.1134.tar", last modified: Mon Apr 22 21:25:34 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-svp-3.0.1135.tar", last modified: Tue Apr 23 21:02:52 2024, max compression
```

## Comparing `tencentcloud-sdk-python-svp-3.0.1134.tar` & `tencentcloud-sdk-python-svp-3.0.1135.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/
--rw-r--r--   0 root         (0) root         (0)     1896 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/svp_client.py
--rw-r--r--   0 root         (0) root         (0)      652 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5505 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/__init__.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1660 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/setup.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-04-22 21:25:34.000000 tencentcloud-sdk-python-svp-3.0.1134/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/
+-rw-r--r--   0 root         (0) root         (0)     1896 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/svp_client.py
+-rw-r--r--   0 root         (0) root         (0)      652 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5505 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/setup.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-04-23 21:02:52.000000 tencentcloud-sdk-python-svp-3.0.1135/README.rst
```

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/PKG-INFO` & `tencentcloud-sdk-python-svp-3.0.1135/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-svp
-Version: 3.0.1134
+Version: 3.0.1135
 Summary: Tencent Cloud Svp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/__init__.py` & `tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1134'
+__version__ = '3.0.1135'
```

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/svp_client.py` & `tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/svp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/errorcodes.py` & `tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/tencentcloud/svp/v20240125/models.py` & `tencentcloud-sdk-python-svp-3.0.1135/tencentcloud/svp/v20240125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/tencentcloud_sdk_python_svp.egg-info/PKG-INFO` & `tencentcloud-sdk-python-svp-3.0.1135/tencentcloud_sdk_python_svp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-svp
-Version: 3.0.1134
+Version: 3.0.1135
 Summary: Tencent Cloud Svp SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/setup.py` & `tencentcloud-sdk-python-svp-3.0.1135/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-svp',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1134"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1135"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Svp SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-svp-3.0.1134/README.rst` & `tencentcloud-sdk-python-svp-3.0.1135/README.rst`

 * *Files identical despite different names*
