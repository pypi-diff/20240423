# Comparing `tmp/mms_client-1.4.1.tar.gz` & `tmp/mms_client-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mms_client-1.4.1.tar", max compression
+gzip compressed data, was "mms_client-1.5.0.tar", max compression
```

## Comparing `mms_client-1.4.1.tar` & `mms_client-1.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1211 2024-04-19 07:44:07.809260 mms_client-1.4.1/LICENSE
--rw-r--r--   0        0        0    15070 2024-04-19 07:44:07.809260 mms_client-1.4.1/README.md
--rw-r--r--   0        0        0     2913 2024-04-19 07:44:07.813260 mms_client-1.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/__init__.py
--rw-r--r--   0        0        0      571 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/client.py
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/py.typed
--rw-r--r--   0        0        0    10702 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
--rw-r--r--   0        0        0     9894 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl
--rw-r--r--   0        0        0   109679 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/xsd/mi-market.xsd
--rw-r--r--   0        0        0    76166 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
--rw-r--r--   0        0        0    13276 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/xsd/mi-report.xsd
--rw-r--r--   0        0        0    69149 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/xsd/mpr.xsd
--rw-r--r--   0        0        0    31524 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/schemas/xsd/omi.xsd
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/security/__init__.py
--rw-r--r--   0        0        0     1489 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/security/certs.py
--rw-r--r--   0        0        0     2149 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/security/crypto.py
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/__init__.py
--rw-r--r--   0        0        0    26397 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/base.py
--rw-r--r--   0        0        0     7580 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/market.py
--rw-r--r--   0        0        0      521 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/omi.py
--rw-r--r--   0        0        0     3711 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/registration.py
--rw-r--r--   0        0        0      537 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/services/report.py
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/__init__.py
--rw-r--r--   0        0        0    14139 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/award.py
--rw-r--r--   0        0        0     9710 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/base.py
--rw-r--r--   0        0        0     1629 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/enums.py
--rw-r--r--   0        0        0    14785 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/fields.py
--rw-r--r--   0        0        0     2706 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/market.py
--rw-r--r--   0        0        0     6791 2024-04-19 07:44:07.813260 mms_client-1.4.1/src/mms_client/types/offer.py
--rw-r--r--   0        0        0     1381 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/types/registration.py
--rw-r--r--   0        0        0    65974 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/types/resource.py
--rw-r--r--   0        0        0     4399 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/types/transport.py
--rw-r--r--   0        0        0        0 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/utils/__init__.py
--rw-r--r--   0        0        0     1693 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/utils/auditing.py
--rw-r--r--   0        0        0     2475 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/utils/errors.py
--rw-r--r--   0        0        0    29534 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/utils/serialization.py
--rw-r--r--   0        0        0    10094 2024-04-19 07:44:07.817260 mms_client-1.4.1/src/mms_client/utils/web.py
--rw-r--r--   0        0        0    16354 1970-01-01 00:00:00.000000 mms_client-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-23 00:20:48.431840 mms_client-1.5.0/LICENSE
+-rw-r--r--   0        0        0    14703 2024-04-23 00:20:48.431840 mms_client-1.5.0/README.md
+-rw-r--r--   0        0        0     2913 2024-04-23 00:20:48.431840 mms_client-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/__init__.py
+-rw-r--r--   0        0        0      676 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/client.py
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/py.typed
+-rw-r--r--   0        0        0    10702 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl
+-rw-r--r--   0        0        0     9894 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl
+-rw-r--r--   0        0        0   109679 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-market.xsd
+-rw-r--r--   0        0        0    76166 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd
+-rw-r--r--   0        0        0    13276 2024-04-23 00:20:48.431840 mms_client-1.5.0/src/mms_client/schemas/xsd/mi-report.xsd
+-rw-r--r--   0        0        0    69149 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/schemas/xsd/mpr.xsd
+-rw-r--r--   0        0        0    31524 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/schemas/xsd/omi.xsd
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/__init__.py
+-rw-r--r--   0        0        0     1489 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/certs.py
+-rw-r--r--   0        0        0     2149 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/security/crypto.py
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/__init__.py
+-rw-r--r--   0        0        0    25897 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/base.py
+-rw-r--r--   0        0        0     7684 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/market.py
+-rw-r--r--   0        0        0      626 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/omi.py
+-rw-r--r--   0        0        0     3815 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/registration.py
+-rw-r--r--   0        0        0      642 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/services/report.py
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/__init__.py
+-rw-r--r--   0        0        0    14139 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/award.py
+-rw-r--r--   0        0        0     9710 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/base.py
+-rw-r--r--   0        0        0     1629 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/enums.py
+-rw-r--r--   0        0        0    14785 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/fields.py
+-rw-r--r--   0        0        0     2706 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/market.py
+-rw-r--r--   0        0        0     6791 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/offer.py
+-rw-r--r--   0        0        0     1381 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/registration.py
+-rw-r--r--   0        0        0    65974 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/resource.py
+-rw-r--r--   0        0        0     4399 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/types/transport.py
+-rw-r--r--   0        0        0        0 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/__init__.py
+-rw-r--r--   0        0        0     1797 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/auditing.py
+-rw-r--r--   0        0        0     2579 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/errors.py
+-rw-r--r--   0        0        0    29638 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/serialization.py
+-rw-r--r--   0        0        0    10033 2024-04-23 00:20:48.435840 mms_client-1.5.0/src/mms_client/utils/web.py
+-rw-r--r--   0        0        0    15987 1970-01-01 00:00:00.000000 mms_client-1.5.0/PKG-INFO
```

### Comparing `mms_client-1.4.1/LICENSE` & `mms_client-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/README.md` & `mms_client-1.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -150,23 +150,14 @@
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
-## Log Settings
-The client also supports injection of a custom logger. The default logger is named "MMS Client".
-
-```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
-```
-
-The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
-
 ## Auditing XML Requests & Responses
 A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
 
 ```python
 class TestAuditPlugin(AuditPlugin):
 
     def __init__(self):
```

### Comparing `mms_client-1.4.1/pyproject.toml` & `mms_client-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mms_client"
-version = "v1.4.1"
+version = "v1.5.0"
 description = "API client for accessing the MMS"
 authors = ["Ryan Wood <ryan.wood@electroroute.co.jp>"]
 readme = "README.md"
 packages = [{ include = "mms_client", from = "src" }]
 homepage = "https://github.com/ElectroRoute-Japan/mms-client"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `mms_client-1.4.1/src/mms_client/client.py` & `mms_client-1.5.0/src/mms_client/client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 """Contains the client layer for communicating with the MMS server."""
 
+from logging import getLogger
+
 from mms_client.services.base import BaseClient
 from mms_client.services.market import MarketClientMixin
 from mms_client.services.omi import OMIClientMixin
 from mms_client.services.registration import RegistrationClientMixin
 from mms_client.services.report import ReportClientMixin
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class MmsClient(BaseClient, MarketClientMixin, RegistrationClientMixin, ReportClientMixin, OMIClientMixin):
     """User client for the MMS server.
 
     This class is used to communicate with the MMS server.
     """
```

### Comparing `mms_client-1.4.1/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl` & `mms_client-1.5.0/src/mms_client/schemas/wsdl/mi-web-service-jbms.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/wsdl/omi-web-service.wsdl` & `mms_client-1.5.0/src/mms_client/schemas/wsdl/omi-web-service.wsdl`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/xsd/mi-market.xsd` & `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-market.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd` & `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-outbnd-reports.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/xsd/mi-report.xsd` & `mms_client-1.5.0/src/mms_client/schemas/xsd/mi-report.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/xsd/mpr.xsd` & `mms_client-1.5.0/src/mms_client/schemas/xsd/mpr.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/schemas/xsd/omi.xsd` & `mms_client-1.5.0/src/mms_client/schemas/xsd/omi.xsd`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/security/certs.py` & `mms_client-1.5.0/src/mms_client/security/certs.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/security/crypto.py` & `mms_client-1.5.0/src/mms_client/security/crypto.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/services/base.py` & `mms_client-1.5.0/src/mms_client/services/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Contains the client layer for communicating with the MMS server."""
 
 from dataclasses import dataclass
-from logging import Logger
 from logging import getLogger
 from typing import Dict
 from typing import Generic
 from typing import List
 from typing import Optional
 from typing import Protocol
 from typing import Tuple
@@ -33,15 +32,15 @@
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
 from mms_client.utils.web import Plugin
 from mms_client.utils.web import ZWrapper
 
 # Set the default logger for the MMS client
-default_logger = getLogger("MMS Client")
+logger = getLogger(__name__)
 
 
 @dataclass
 class ServiceConfiguration:
     """Configuration for a service on the MMS server."""
 
     # The interface for the service
@@ -81,18 +80,14 @@
     def participant(self) -> str:
         """Return the MMS code of the business entity to which the requesting user belongs."""
 
     @property
     def user(self) -> str:
         """Return the user name of the person making the request."""
 
-    @property
-    def logger(self) -> Logger:
-        """Return the logger for the client."""
-
     def verify_audience(self, config: EndpointConfiguration) -> None:
         """Verify that the client type is allowed.
 
         Some MMS endpoints are only accessible to certain client types. This method is used to verify that the client
         type is allowed to access the endpoint.
 
         Arguments:
@@ -162,25 +157,27 @@
     """
     # First, create the endpoint configuration from the given parameters
     config = EndpointConfiguration(name, allowed_clients, service, request_type, resp_envelope_type, resp_data_type)
 
     # Next, create a decorator that will add the endpoint configuration to the function
     def decorator(func):
         def wrapper(self: ClientProto, *args, **kwargs) -> Optional[P]:
+            logger.info(f"{config.name}: Called with args: {args[1:]}...")
 
             # First, verify that the client type is allowed
             self.verify_audience(config)
 
             # Next, call the wrapped function to get the envelope
             envelope = func(self, *args, **kwargs)
 
             # Now, submit the request to the MMS server and get the response
             resp, _ = self.request_one(envelope, args[0], config)
 
             # Finally, extract the data from the response and return it
+            logger.info(f"{config.name}: Returning {type(resp.data).__name__} data.")
             return resp.data
 
         return wrapper
 
     # Finally, return the decorator
     return decorator
 
@@ -217,27 +214,27 @@
     """
     # First, create the endpoint configuration from the given parameters
     config = EndpointConfiguration(name, allowed_clients, service, request_type, resp_envelope_type, resp_data_type)
 
     # Next, create a decorator that will add the endpoint configuration to the function
     def decorator(func):
         def wrapper(self: ClientProto, *args, **kwargs) -> List[P]:
-            self.logger.info(f"{config.name}: Called with args: {args[1:]}...")
+            logger.info(f"{config.name}: Called with args: {args[1:]}...")
 
             # First, verify that the client type is allowed
             self.verify_audience(config)
 
             # Next, call the wrapped function to get the envelope
             envelope = func(self, *args, **kwargs)
 
             # Now, submit the request to the MMS server and get the response
             resp, _ = self.request_many(envelope, args[0], config)
 
             # Finally, extract the data from the response and return it
-            self.logger.info(f"{config.name}: Returning {len(resp.data)} item(s).")
+            logger.info(f"{config.name}: Returning {len(resp.data)} item(s).")
             return resp.data
 
         return wrapper
 
     # Finally, return the decorator
     return decorator
 
@@ -250,28 +247,25 @@
 
     def __init__(
         self,
         participant: str,
         user: str,
         client_type: ClientType,
         cert: Certificate,
-        logger: Optional[Logger] = None,
         plugins: Optional[List[Plugin]] = None,
         is_admin: bool = False,
         test: bool = False,
     ):
         """Create a new MMS client with the given participant, user, client type, and authentication.
 
         Arguments:
         participant (str):          The MMS code of the business entity to which the requesting user belongs.
         user (str):                 The user name of the person making the request.
         client_type (ClientType):   The type of client to use for making requests to the MMS server.
         cert (Certificate):         The certificate to use for signing requests.
-        logger (Logger):            The logger to use for instrumentation. If this is not provided, then the default
-                                    logger will be used.
         plugins (List[Plugin]):     A list of plugins to add to the Zeep client. This can be useful for auditing or
                                     other purposes.
         is_admin (bool):            Whether the user is an admin (i.e. is a market operator).
         test (bool):                Whether to use the test server.
         """
         # First, save the base field associated with the client
         self._participant = participant
@@ -280,16 +274,15 @@
         self._is_admin = is_admin
         self._test = test
 
         # Next, save the security-related fields associated with the client
         self._cert = cert
         self._signer = CryptoWrapper(cert)
 
-        # Now, set our logger to either the provided logger or the default logger
-        self._logger = logger or default_logger
+        # Now, set the plugins we'll inject into the Zeep client
         self._plugins = plugins or []
 
         # Finally, create a list of wrappers for the different interfaces
         self._wrappers: Dict[Interface, ZWrapper] = {}
 
     @property
     def participant(self) -> str:
@@ -297,32 +290,27 @@
         return self._participant
 
     @property
     def user(self) -> str:
         """Return the user name of the person making the request."""
         return self._user
 
-    @property
-    def logger(self) -> Logger:
-        """Return the logger for the client."""
-        return self._logger
-
     def verify_audience(self, config: EndpointConfiguration) -> None:
         """Verify that the client type is allowed.
 
         Some MMS endpoints are only accessible to certain client types. This method is used to verify that the client
         type is allowed to access the endpoint.
 
         Arguments:
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Raises:
         ValueError: If the client type is not allowed.
         """
-        self._logger.debug(
+        logger.debug(
             f"{config.name}: Verifying audience. Allowed clients: "
             f"{config.allowed_clients if config.allowed_clients else 'Any'}."
         )
         if config.allowed_clients and (self._client_type not in config.allowed_clients):
             raise AudienceError(config.name, config.allowed_clients, self._client_type)
 
     def request_one(
@@ -337,15 +325,15 @@
         envelope (Envelope):            The payload envelope to submit to the MMS server.
         payload (Payload):              The data to submit to the MMS server.
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Returns:    The response from the MMS server.
         """
         # First, create the MMS request from the payload and data.
-        self._logger.debug(
+        logger.debug(
             f"{config.name}: Starting request. Envelope: {type(envelope).__name__}, Data: {type(payload).__name__}",
         )
         request = self._to_mms_request(config.request_type, config.service.serializer.serialize(envelope, payload))
 
         # Next, submit the request to the MMS server and get and verify the response.
         resp = self._get_wrapper(config.service).submit(request)
         self._verify_mms_response(resp, config)
@@ -356,15 +344,15 @@
         # Finally, deserialize and verify the response
         envelope_type = config.response_envelope_type or type(envelope)
         data_type = config.response_data_type or type(payload)
         data: Response[E, P] = config.service.serializer.deserialize(resp.payload, envelope_type, data_type)
         self._verify_response(data, config)
 
         # Return the response data and any attachments
-        self._logger.debug(
+        logger.debug(
             f"{config.name}: Returning response. Envelope: {envelope_type.__name__}, Data: {data_type.__name__}",
         )
         return data, attachments
 
     def request_many(
         self,
         envelope: E,
@@ -379,15 +367,15 @@
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Returns:    The multi-response from the MMS server.
         """
         # First, create the MMS request from the payload and data.
         is_list = isinstance(payload, list)
         data_type = type(payload[0]) if is_list else type(payload)  # type: ignore[index]
-        self._logger.debug(
+        logger.debug(
             (
                 f"{config.name}: Starting multi-request. Envelope: {type(envelope).__name__}, "
                 f"Data: {data_type.__name__}"
             ),
         )
         serialized = (
             config.service.serializer.serialize_multi(envelope, payload, data_type)  # type: ignore[arg-type]
@@ -410,15 +398,15 @@
             resp.payload,
             envelope_type,
             data_type,  # type: ignore[arg-type]
         )
         self._verify_multi_response(data, config)
 
         # Return the response data and any attachments
-        self._logger.debug(
+        logger.debug(
             f"{config.name}: Returning multi-response. Envelope: {envelope_type.__name__}, Data: {data_type.__name__}",
         )
         return data, attachments
 
     def _to_mms_request(
         self,
         req_type: RequestType,
@@ -443,15 +431,15 @@
                 for name, data in attachments.items()
             ]
             if attachments
             else []
         )
 
         # Embed the data and the attachments in the MMS request and return it
-        self._logger.debug(
+        logger.debug(
             f"Creating MMS request of type {req_type.name} to send {len(data)} bytes of data and "
             f"{len(attachment_data)} attachments."
         )
         return MmsRequest(
             requestType=req_type,
             adminRole=self._is_admin,
             requestDataType=RequestDataType.XML,
@@ -477,17 +465,17 @@
                 f"Invalid MMS response data type: {resp.data_type.name}. Only XML is supported.",
             )
         if resp.compressed:
             raise MMSClientError(config.name, "Invalid MMS response. Compressed responses are not supported.")
 
         # Check the response status flags and log any warnings or errors
         if resp.warnings:
-            self._logger.warning(f"{config.name}: MMS response contained warnings.")
+            logger.warning(f"{config.name}: MMS response contained warnings.")
         if not resp.success:
-            self._logger.error(f"{config.name}: MMS response was unsuccessful.")
+            logger.error(f"{config.name}: MMS response was unsuccessful.")
 
     def _verify_response(self, resp: Response[E, P], config: EndpointConfiguration) -> None:
         """Verify that the given response is valid.
 
         Arguments:
         resp (Response):    The response to verify.
 
@@ -540,15 +528,15 @@
         Arguments:
         resp (BaseResponse):            The base response to verify.
         config (EndpointConfiguration): The configuration for the endpoint.
 
         Returns:    True to indicate that the response is valid, False otherwise.
         """
         # Log the request's processing statistics
-        self._logger.info(
+        logger.info(
             f"{config.name} ({resp.statistics.timestamp_xml}): Recieved {resp.statistics.received}, "
             f"Valid: {resp.statistics.valid}, Invalid: {resp.statistics.invalid}, "
             f"Successful: {resp.statistics.successful}, Unsuccessful: {resp.statistics.unsuccessful} "
             f"in {resp.statistics.time_ms}ms"
         )
 
         # Check if the response is invalid and if the envelope had any validation issues. If not, then we have a
@@ -562,19 +550,19 @@
 
         Arguments:
         config (EndpointConfiguration): The configuration for the endpoint.
         resp (BaseResponse):            The response to verify.
         """
         for path, messages in resp.messages.items():
             for info in messages.information:
-                self._logger.info(f"{config.name} - {path}: {info.code}")
+                logger.info(f"{config.name} - {path}: {info.code}")
             for warning in messages.warnings:
-                self._logger.warning(f"{config.name} - {path}: {warning.code}")
+                logger.warning(f"{config.name} - {path}: {warning.code}")
             for error in messages.errors:
-                self._logger.error(f"{config.name} - {path}: {error.code}")
+                logger.error(f"{config.name} - {path}: {error.code}")
 
     def _verify_response_common(
         self, config: EndpointConfiguration, payload_type: type, resp: ResponseCommon, index: Optional[int] = None
     ) -> bool:
         """Verify the common response data in the given response.
 
         Arguments:
@@ -583,33 +571,32 @@
         resp (ResponseCommon):          The common response data to verify.
         index (int):                    The index of the response in the multi-response. This is None for single
                                         responses.
 
         Returns:    True to indicate that the response is valid, False otherwise.
         """
         # Log the status of the response validation
-        self._logger.info(
+        logger.info(
             f"{config.name}: {payload_type.__name__}{f'[{index}]' if index is not None else ''} was valid? "
             f"{resp.success} ({resp.validation.value})",
         )
 
         # Verify that the response was successful and that the validation status is not a failed status
         return resp.success and (resp.validation not in (ValidationStatus.FAILED, ValidationStatus.PASSED_PARTIAL))
 
     def _get_wrapper(self, service: ServiceConfiguration) -> ZWrapper:
         """Get the wrapper for the given service.
 
         Arguments:
         service (ServiceConfiguration):  The service for which to get the wrapper.
         """
         if service.interface not in self._wrappers:
-            self._logger.debug(f"Creating wrapper for {service.interface.name} interface.")
+            logger.debug(f"Creating wrapper for {service.interface.name} interface.")
             self._wrappers[service.interface] = ZWrapper(
                 self._client_type,
                 service.interface,
                 self._cert.to_adapter(),
-                self._logger,
                 self._plugins,
                 True,
                 self._test,
             )
         return self._wrappers[service.interface]
```

### Comparing `mms_client-1.4.1/src/mms_client/services/market.py` & `mms_client-1.5.0/src/mms_client/services/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains the client layer for making market requests to the MMS server."""
 
 from datetime import date as Date
+from logging import getLogger
 from typing import List
 from typing import Optional
 
 from mms_client.services.base import ClientProto
 from mms_client.services.base import ServiceConfiguration
 from mms_client.services.base import mms_endpoint
 from mms_client.services.base import mms_multi_endpoint
@@ -19,14 +20,17 @@
 from mms_client.types.offer import OfferQuery
 from mms_client.types.transport import RequestType
 from mms_client.utils.serialization import SchemaType
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class MarketClientMixin:  # pylint: disable=unused-argument
     """Market client for the MMS server."""
 
     # The configuration for the market service
     config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.MARKET, "MarketData"))
```

### Comparing `mms_client-1.4.1/src/mms_client/services/registration.py` & `mms_client-1.5.0/src/mms_client/services/registration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Contains the client layer for making registration requests to the MMS server."""
 
 from datetime import date as Date
+from logging import getLogger
 from typing import List
 from typing import Optional
 
 from mms_client.services.base import ClientProto
 from mms_client.services.base import ServiceConfiguration
 from mms_client.services.base import mms_endpoint
 from mms_client.services.base import mms_multi_endpoint
@@ -16,14 +17,17 @@
 from mms_client.types.resource import ResourceQuery
 from mms_client.types.transport import RequestType
 from mms_client.utils.serialization import SchemaType
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import ClientType
 from mms_client.utils.web import Interface
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class RegistrationClientMixin:  # pylint: disable=unused-argument
     """Registration client for the MMS server."""
 
     # The configuration for the registration service
     config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.REGISTRATION, "RegistrationData"))
```

### Comparing `mms_client-1.4.1/src/mms_client/services/report.py` & `mms_client-1.5.0/src/mms_client/services/omi.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,18 @@
-"""Contains the client layer for making report requests to the MMS server."""
+"""Contains the client layer for making OMI requests to the MMS server."""
+
+from logging import getLogger
 
 from mms_client.services.base import ServiceConfiguration
 from mms_client.utils.serialization import SchemaType
 from mms_client.utils.serialization import Serializer
 from mms_client.utils.web import Interface
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
-class ReportClientMixin:  # pylint: disable=unused-argument
-    """Report client for the MMS server."""
+class OMIClientMixin:  # pylint: disable=unused-argument
+    """OMI client for the MMS server."""
 
-    # The configuration for the report service
-    config = ServiceConfiguration(Interface.MI, Serializer(SchemaType.REPORT, "MarketReport"))
+    # The configuration for the OMI service
+    config = ServiceConfiguration(Interface.OMI, Serializer(SchemaType.OMI, "MarketData"))
```

### Comparing `mms_client-1.4.1/src/mms_client/types/award.py` & `mms_client-1.5.0/src/mms_client/types/award.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/base.py` & `mms_client-1.5.0/src/mms_client/types/base.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/enums.py` & `mms_client-1.5.0/src/mms_client/types/enums.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/fields.py` & `mms_client-1.5.0/src/mms_client/types/fields.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/market.py` & `mms_client-1.5.0/src/mms_client/types/market.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/offer.py` & `mms_client-1.5.0/src/mms_client/types/offer.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/registration.py` & `mms_client-1.5.0/src/mms_client/types/registration.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/resource.py` & `mms_client-1.5.0/src/mms_client/types/resource.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/types/transport.py` & `mms_client-1.5.0/src/mms_client/types/transport.py`

 * *Files identical despite different names*

### Comparing `mms_client-1.4.1/src/mms_client/utils/auditing.py` & `mms_client-1.5.0/src/mms_client/utils/auditing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 """Contains functions for auditability plugins."""
 
 from abc import ABC
 from abc import abstractmethod
+from logging import getLogger
 
 from lxml.etree import _Element as Element
 from lxml.etree import tostring
 from zeep import Plugin
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class AuditPlugin(ABC, Plugin):
     """Base class for audit plugins."""
 
     def egress(self, envelope: Element, http_headers: dict, operation, binding_options):
         """Handle the MMS request before it is sent.
```

### Comparing `mms_client-1.4.1/src/mms_client/utils/errors.py` & `mms_client-1.5.0/src/mms_client/utils/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """Contains error classes for the MMS client."""
 
+from logging import getLogger
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Union
 
 from mms_client.types.base import E
 from mms_client.types.base import Messages
 from mms_client.types.base import P
 from mms_client.utils.web import ClientType
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class AudienceError(ValueError):
     """Error raised when an invalid audience is provided."""
 
     def __init__(self, method: str, allowed: List[ClientType], audience: ClientType):
         """Initialize the error.
```

### Comparing `mms_client-1.4.1/src/mms_client/utils/serialization.py` & `mms_client-1.5.0/src/mms_client/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Contains objects for serialization and deserialization of MMS data."""
 
 from functools import lru_cache
 from io import BytesIO
+from logging import getLogger
 from pathlib import Path
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
 from typing import Type
 from typing import Union
@@ -28,14 +29,17 @@
 from mms_client.types.base import ResponseCommon
 from mms_client.types.base import ResponseData
 from mms_client.types.base import SchemaType
 
 # Directory containing all our XML schemas
 XSD_DIR = Path(__file__).parent.parent / "schemas" / "xsd"
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class Serializer:
     """Contains methods for serializing and deserializing MMS data."""
 
     def __init__(self, xsd: SchemaType, payload_key: str):
         """Create a new payload configuration with the given XSD schema, payload key, and interface type.
```

### Comparing `mms_client-1.4.1/src/mms_client/utils/web.py` & `mms_client-1.5.0/src/mms_client/utils/web.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Contains the HTTP/web layer for communicating with the MMS server."""
 
 from enum import StrEnum
-from logging import Logger
+from logging import getLogger
 from pathlib import Path
 from typing import List
 from typing import Optional
 
 from backoff import expo
 from backoff import on_exception
 from requests import Session
@@ -16,14 +16,17 @@
 from zeep.cache import SqliteCache
 from zeep.exceptions import TransportError
 from zeep.xsd.valueobjects import CompoundValue
 
 from mms_client.types.transport import MmsRequest
 from mms_client.types.transport import MmsResponse
 
+# Set the default logger for the MMS client
+logger = getLogger(__name__)
+
 
 class ClientType(StrEnum):
     """Identifies the type of client to use.
 
     The client can be either "bsp" (Balancing Service Provider), "mo" (Market Operator), or "tso" (Transmission System
     Operator).
     """
@@ -130,15 +133,14 @@
     """
 
     def __init__(
         self,
         client: ClientType,
         interface: Interface,
         adapter: Pkcs12Adapter,
-        logger: Logger,
         plugins: Optional[List[Plugin]] = None,
         cache: bool = True,
         test: bool = False,
     ):
         """Create a new Zeep wrapper object for a specific MMS service endpoint.
 
         Arguments:
@@ -146,15 +148,14 @@
                                     "tso" (Transmission System Operator). This will determine which service endpoint to
                                     use.
         interface (Interface):      The type of interface to use. This can be either "omi" (Other Market Initiator) or
                                     "mi" (Market Initiator). This will determine which service endpoint to use as well
                                     as the service and port to use.
         adapter (Pkcs12Adapter):    The PKCS12 adapter containing the certificate and private key to use for
                                     authenticating with the MMS server.
-        logger (Logger):            The logger to use for instrumentation.
         plugins (List[Plugin]):     A list of Zeep plugins to use with the client. This is useful for adding additional
                                     functionality to the client, such as auditing or logging.
         cache (bool):               If True, use a cache for the Zeep client. This is useful for avoiding repeated
                                     lookups of the WSDL file, which should result in lower latency.
         test (bool):                If True, use the test service endpoint. This is useful for testing the client.
         """
         # First, we'll check that the client is valid. If it's not, we'll raise a ValueError.
@@ -186,46 +187,45 @@
         sess = Session()
         sess.mount(self._endpoint.selected, adapter)
         if not test:
             sess.mount(self._endpoint.backup, adapter)
 
         # Finally, we create the Zeep client with the given WSDL file location, session, and cache settings and then,
         # from that client, we create the SOAP service with the given service binding and selected endpoint.
-        self._logger = logger
         self._client = Client(
             wsdl=str(location.resolve()),
             transport=Transport(cache=SqliteCache() if cache else None, session=sess),
             plugins=plugins,
         )
         self._create_service()
 
-    @on_exception(expo, TransportError, max_tries=3, giveup=fatal_code)  # type: ignore[arg-type]
+    @on_exception(expo, TransportError, max_tries=3, giveup=fatal_code, logger=logger)  # type: ignore[arg-type]
     def submit(self, req: MmsRequest) -> MmsResponse:
         """Submit the given request to the MMS server and return the response."""
         try:
-            self._logger.debug(f"Submitting MMS request request to {self._interface.name} service")
+            logger.debug(f"Submitting MMS request request to {self._interface.name} service")
 
             # Submit the request to the MMS server and retrieve the response
             resp: CompoundValue = self._service["submitAttachment"](**req.to_arguments())
 
             # Validate the response and return it
             return MmsResponse.model_validate(resp.__values__)
         except TransportError as e:
             # If we got a server fault error, then we'll switch to the backup endpoint. In any case, we'll raise the
             # exception so that our back-off can handle it or pass the exception up the stack.
-            self._logger.error(
+            logger.error(
                 f"MMS request to {self._interface.name} service failed with status code: {e.status_code}",
                 exc_info=e,
             )
             if e.status_code >= 500:
-                self._logger.warning(f"MMS server error, switching to backup endpoint: {self._endpoint.backup}")
+                logger.warning(f"MMS server error, switching to backup endpoint: {self._endpoint.backup}")
                 self._endpoint.select(error=True)
                 self._create_service()
             raise
 
     def _create_service(self):
         """Create a new SOAP service with the currently selected endpoint.
 
         This is useful for switching between the main and backup endpoints in case of an error.
         """
-        self._logger.debug(f"Creating new {self._interface.name} service with endpoint: {self._endpoint.selected}")
+        logger.debug(f"Creating new {self._interface.name} service with endpoint: {self._endpoint.selected}")
         self._service = self._client.create_service(SERVICE_BINDINGS[self._interface], self._endpoint.selected)
```

### Comparing `mms_client-1.4.1/PKG-INFO` & `mms_client-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mms-client
-Version: 1.4.1
+Version: 1.5.0
 Summary: API client for accessing the MMS
 Home-page: https://github.com/ElectroRoute-Japan/mms-client
 Author: Ryan Wood
 Author-email: ryan.wood@electroroute.co.jp
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pydantic :: 2
@@ -182,23 +182,14 @@
 ## Connecting as a Market Admin
 If you're connecting as a market operator (MO), you can connect in admin mode:
 
 ```python
 client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, is_admin=True)
 ```
 
-## Log Settings
-The client also supports injection of a custom logger. The default logger is named "MMS Client".
-
-```python
-client = MmsClient(participant="F100", user="FAKEUSER", client_type=ClientType.BSP, cert, logger=my_logger)
-```
-
-The client currently logs a number of informational, debug and error messages. You can freely change the logging level yourself.
-
 ## Auditing XML Requests & Responses
 A common requirement for this sort of library is recording or saving the raw XML requests and responses for audit/logging purposes. This library supports this workflow through the `mms_client.utils.auditing.AuditPlugin` object. This object intercepts the XML request at the Zeep client level right before it is sent to the MMS and, similarly, intercepts the XML response immediately after it is received from the MMS. Before passing these objects on, without modifying them, it records the XML data as a byte string and passes it to two methods: `audit_request` and `audit_response`. These can be overridden by any object that inherits from this class, allowing the user to direct this data to whatever store they prefer to use for auditing or logging.
 
 ```python
 class TestAuditPlugin(AuditPlugin):
 
     def __init__(self):
```

