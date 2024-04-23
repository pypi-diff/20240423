# Comparing `tmp/aliyun-python-sdk-computenest-1.0.0.tar.gz` & `tmp/aliyun-python-sdk-computenest-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-computenest-1.0.0.tar", last modified: Tue May 16 06:11:15 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-computenest-1.0.1.tar", last modified: Tue Apr 23 09:14:47 2024, max compression
```

## Comparing `aliyun-python-sdk-computenest-1.0.0.tar` & `aliyun-python-sdk-computenest-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      575 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      543 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1577 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      982 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/
--rw-r--r--   0 root         (0) root         (0)     2356 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ContinueDeployServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     6084 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/CreateServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1826 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/DeleteServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1762 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/GetServiceInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1921 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3230 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2865 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstancesRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2492 2023-05-16 06:11:15.000000 aliyun-python-sdk-computenest-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      543 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1577 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1139 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2356 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ContinueDeployServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     6153 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/CreateServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1826 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/DeleteServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1762 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/GetServiceInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3847 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/GetServiceTemplateParameterConstraintsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceLogsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3525 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-23 09:14:47.000000 aliyun-python-sdk-computenest-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2492 2024-04-23 09:14:46.000000 aliyun-python-sdk-computenest-1.0.1/setup.py
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/LICENSE` & `aliyun-python-sdk-computenest-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/PKG-INFO` & `aliyun-python-sdk-computenest-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenest
-Version: 1.0.0
+Version: 1.0.1
 Summary: The computenest module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenest
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/README.rst` & `aliyun-python-sdk-computenest-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/PKG-INFO` & `aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-computenest
-Version: 1.0.0
+Version: 1.0.1
 Summary: The computenest module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-computenest
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyun_python_sdk_computenest.egg-info/SOURCES.txt` & `aliyun-python-sdk-computenest-1.0.1/aliyun_python_sdk_computenest.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 aliyun_python_sdk_computenest.egg-info/SOURCES.txt
 aliyun_python_sdk_computenest.egg-info/dependency_links.txt
 aliyun_python_sdk_computenest.egg-info/requires.txt
 aliyun_python_sdk_computenest.egg-info/top_level.txt
 aliyunsdkcomputenest/__init__.py
 aliyunsdkcomputenest/endpoint.py
 aliyunsdkcomputenest/request/__init__.py
+aliyunsdkcomputenest/request/v20210601/ChangeResourceGroupRequest.py
 aliyunsdkcomputenest/request/v20210601/ContinueDeployServiceInstanceRequest.py
 aliyunsdkcomputenest/request/v20210601/CreateServiceInstanceRequest.py
 aliyunsdkcomputenest/request/v20210601/DeleteServiceInstancesRequest.py
 aliyunsdkcomputenest/request/v20210601/GetServiceInstanceRequest.py
+aliyunsdkcomputenest/request/v20210601/GetServiceTemplateParameterConstraintsRequest.py
 aliyunsdkcomputenest/request/v20210601/ListServiceInstanceLogsRequest.py
 aliyunsdkcomputenest/request/v20210601/ListServiceInstanceResourcesRequest.py
 aliyunsdkcomputenest/request/v20210601/ListServiceInstancesRequest.py
 aliyunsdkcomputenest/request/v20210601/__init__.py
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/endpoint.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ContinueDeployServiceInstanceRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ContinueDeployServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/CreateServiceInstanceRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/CreateServiceInstanceRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -33,14 +33,18 @@
 
 	def get_Commodity(self): # Struct
 		return self.get_query_params().get('Commodity')
 
 	def set_Commodity(self, Commodity):  # Struct
 		if Commodity.get('PayPeriod') is not None:
 			self.add_query_param('Commodity.PayPeriod', Commodity.get('PayPeriod'))
+		if Commodity.get('AutoPay') is not None:
+			self.add_query_param('Commodity.AutoPay', Commodity.get('AutoPay'))
+		if Commodity.get('AutoRenew') is not None:
+			self.add_query_param('Commodity.AutoRenew', Commodity.get('AutoRenew'))
 		if Commodity.get('PayPeriodUnit') is not None:
 			self.add_query_param('Commodity.PayPeriodUnit', Commodity.get('PayPeriodUnit'))
 	def get_ContactGroup(self): # String
 		return self.get_query_params().get('ContactGroup')
 
 	def set_ContactGroup(self, ContactGroup):  # String
 		self.add_query_param('ContactGroup', ContactGroup)
@@ -114,19 +118,14 @@
 	def set_ServiceId(self, ServiceId):  # String
 		self.add_query_param('ServiceId', ServiceId)
 	def get_Parameters(self): # String
 		return self.get_query_params().get('Parameters')
 
 	def set_Parameters(self, Parameters):  # String
 		self.add_query_param('Parameters', Parameters)
-	def get_PayType(self): # Long
-		return self.get_query_params().get('PayType')
-
-	def set_PayType(self, PayType):  # Long
-		self.add_query_param('PayType', PayType)
 	def get_OperationMetadata(self): # Struct
 		return self.get_query_params().get('OperationMetadata')
 
 	def set_OperationMetadata(self, OperationMetadata):  # Struct
 		if OperationMetadata.get('EndTime') is not None:
 			self.add_query_param('OperationMetadata.EndTime', OperationMetadata.get('EndTime'))
 		if OperationMetadata.get('Resources') is not None:
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/DeleteServiceInstancesRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/DeleteServiceInstancesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/GetServiceInstanceRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/GetServiceInstanceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceLogsRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceLogsRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,12 +37,22 @@
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
 	def get_ServiceInstanceId(self): # String
 		return self.get_query_params().get('ServiceInstanceId')
 
 	def set_ServiceInstanceId(self, ServiceInstanceId):  # String
 		self.add_query_param('ServiceInstanceId', ServiceInstanceId)
-	def get_MaxResults(self): # String
+	def get_LogSource(self): # String
+		return self.get_query_params().get('LogSource')
+
+	def set_LogSource(self, LogSource):  # String
+		self.add_query_param('LogSource', LogSource)
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
+	def get_Logstore(self): # String
+		return self.get_query_params().get('Logstore')
+
+	def set_Logstore(self, Logstore):  # String
+		self.add_query_param('Logstore', Logstore)
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceResourcesRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstanceResourcesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 	def set_ExpireTimeEnd(self, ExpireTimeEnd):  # String
 		self.add_query_param('ExpireTimeEnd', ExpireTimeEnd)
 	def get_NextToken(self): # String
 		return self.get_query_params().get('NextToken')
 
 	def set_NextToken(self, NextToken):  # String
 		self.add_query_param('NextToken', NextToken)
+	def get_ServiceInstanceResourceType(self): # String
+		return self.get_query_params().get('ServiceInstanceResourceType')
+
+	def set_ServiceInstanceResourceType(self, ServiceInstanceResourceType):  # String
+		self.add_query_param('ServiceInstanceResourceType', ServiceInstanceResourceType)
 	def get_ResourceARNs(self): # RepeatList
 		return self.get_query_params().get('ResourceARN')
 
 	def set_ResourceARNs(self, ResourceARN):  # RepeatList
 		for depth1 in range(len(ResourceARN)):
 			self.add_query_param('ResourceARN.' + str(depth1 + 1), ResourceARN[depth1])
 	def get_Tags(self): # RepeatList
@@ -62,17 +67,17 @@
 	def set_ServiceInstanceId(self, ServiceInstanceId):  # String
 		self.add_query_param('ServiceInstanceId', ServiceInstanceId)
 	def get_ExpireTimeStart(self): # String
 		return self.get_query_params().get('ExpireTimeStart')
 
 	def set_ExpireTimeStart(self, ExpireTimeStart):  # String
 		self.add_query_param('ExpireTimeStart', ExpireTimeStart)
-	def get_MaxResults(self): # String
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
 	def get_PayType(self): # String
 		return self.get_query_params().get('PayType')
 
 	def set_PayType(self, PayType):  # String
 		self.add_query_param('PayType', PayType)
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/aliyunsdkcomputenest/request/v20210601/ListServiceInstancesRequest.py` & `aliyun-python-sdk-computenest-1.0.1/aliyunsdkcomputenest/request/v20210601/ListServiceInstancesRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,12 +56,12 @@
 	def set_Filters(self, Filter):  # RepeatList
 		for depth1 in range(len(Filter)):
 			if Filter[depth1].get('Name') is not None:
 				self.add_query_param('Filter.' + str(depth1 + 1) + '.Name', Filter[depth1].get('Name'))
 			if Filter[depth1].get('Value') is not None:
 				for depth2 in range(len(Filter[depth1].get('Value'))):
 					self.add_query_param('Filter.' + str(depth1 + 1) + '.Value.' + str(depth2 + 1), Filter[depth1].get('Value')[depth2])
-	def get_MaxResults(self): # String
+	def get_MaxResults(self): # Integer
 		return self.get_query_params().get('MaxResults')
 
-	def set_MaxResults(self, MaxResults):  # String
+	def set_MaxResults(self, MaxResults):  # Integer
 		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-computenest-1.0.0/setup.py` & `aliyun-python-sdk-computenest-1.0.1/setup.py`

 * *Files identical despite different names*

