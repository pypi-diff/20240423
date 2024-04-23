# Comparing `tmp/pulumi_opsgenie-1.4.0a1713561317.tar.gz` & `tmp/pulumi_opsgenie-1.4.0a1713903127.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_opsgenie-1.4.0a1713561317.tar", last modified: Fri Apr 19 21:22:41 2024, max compression
+gzip compressed data, was "pulumi_opsgenie-1.4.0a1713903127.tar", last modified: Tue Apr 23 20:21:23 2024, max compression
```

## Comparing `pulumi_opsgenie-1.4.0a1713561317.tar` & `pulumi_opsgenie-1.4.0a1713903127.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.455259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   180603 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    58334 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/alert_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30384 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/api_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15615 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/custom_role.py
--rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/email_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    20208 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6512 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_escalation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10267 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)     6408 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4614 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_team.py
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24070 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (127)    24073 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/incident_template.py
--rw-r--r--   0 runner    (1001) docker     (127)    28522 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/integration_action.py
--rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/maintenance.py
--rw-r--r--   0 runner    (1001) docker     (127)    36241 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    30668 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)   161038 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)    25481 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13330 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service_incident_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    19745 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team.py
--rw-r--r--   0 runner    (1001) docker     (127)    28280 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team_routing_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)    26411 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13250 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user_contact.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:22:41.000000 pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 21:22:35.000000 pulumi_opsgenie-1.4.0a1713561317/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:22:41.459259 pulumi_opsgenie-1.4.0a1713561317/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   170966 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58178 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/alert_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30384 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/api_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15459 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/custom_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19644 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/email_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19896 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_escalation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10127 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6268 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_team.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6719 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23914 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23476 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/incident_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28366 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/integration_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11796 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/maintenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36085 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/notification_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29962 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/notification_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152017 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5100 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13728 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25325 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/schedule_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13174 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13102 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/service_incident_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19589 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/team.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28124 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/team_routing_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26255 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/user_contact.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-04-23 20:21:23.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-23 20:21:23.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:21:23.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:21:23.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 20:21:23.000000 pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-23 20:21:14.000000 pulumi_opsgenie-1.4.0a1713903127/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:21:23.539188 pulumi_opsgenie-1.4.0a1713903127/setup.cfg
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/PKG-INFO` & `pulumi_opsgenie-1.4.0a1713903127/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1713561317
+Version: 1.4.0a1713903127
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/README.md` & `pulumi_opsgenie-1.4.0a1713903127/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/__init__.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_inputs.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -552,40 +552,36 @@
 
 @pulumi.input_type
 class EmailIntegrationResponderArgs:
     def __init__(__self__, *,
                  id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] id: The id of the responder.
-        :param pulumi.Input[str] type: The responder type.
+        :param pulumi.Input[str] id: The ID of the Opsgenie Email based Integration.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[pulumi.Input[str]]:
         """
-        The id of the responder.
+        The ID of the Opsgenie Email based Integration.
         """
         return pulumi.get(self, "id")
 
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
@@ -747,54 +743,50 @@
 @pulumi.input_type
 class IncidentTemplateStakeholderPropertyArgs:
     def __init__(__self__, *,
                  message: pulumi.Input[str],
                  description: Optional[pulumi.Input[str]] = None,
                  enable: Optional[pulumi.Input[bool]] = None):
         """
-        :param pulumi.Input[str] message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
-        :param pulumi.Input[str] description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
-        :param pulumi.Input[bool] enable: Option to enable stakeholder notifications.Default value is true.
+        :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
+        :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         """
         pulumi.set(__self__, "message", message)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enable is not None:
             pulumi.set(__self__, "enable", enable)
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Input[str]:
         """
-        Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        Message of the related incident template. This field must not be longer than 130 characters.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: pulumi.Input[str]):
         pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        Description field of the incident template. This field must not be longer than 10000 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def enable(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Option to enable stakeholder notifications.Default value is true.
-        """
         return pulumi.get(self, "enable")
 
     @enable.setter
     def enable(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable", value)
 
 
@@ -813,15 +805,14 @@
         :param pulumi.Input[str] alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeFilterArgs']]] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param pulumi.Input[str] note: Additional alert action note.
         :param pulumi.Input[int] order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
         :param pulumi.Input[str] user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -896,17 +887,14 @@
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
@@ -923,27 +911,21 @@
 
 
 @pulumi.input_type
 class IntegrationActionAcknowledgeFilterArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  conditions: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAcknowledgeFilterConditionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1052,15 +1034,14 @@
         :param pulumi.Input[str] alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteFilterArgs']]] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param pulumi.Input[str] note: Additional alert action note.
         :param pulumi.Input[int] order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
         :param pulumi.Input[str] user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -1135,17 +1116,14 @@
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1162,27 +1140,21 @@
 
 
 @pulumi.input_type
 class IntegrationActionAddNoteFilterArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  conditions: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionAddNoteFilterConditionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1291,15 +1263,14 @@
         :param pulumi.Input[str] alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseFilterArgs']]] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param pulumi.Input[str] note: Additional alert action note.
         :param pulumi.Input[int] order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
         :param pulumi.Input[str] user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -1374,17 +1345,14 @@
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1401,27 +1369,21 @@
 
 
 @pulumi.input_type
 class IntegrationActionCloseFilterArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  conditions: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCloseFilterConditionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1540,32 +1502,20 @@
                  source: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  type: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] name: Name of the integration action.
         :param pulumi.Input[str] alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
-        :param pulumi.Input[str] custom_priority: Custom alert priority. e.g. ``{{message.substring(0,2)}}``
-        :param pulumi.Input[str] description: Detailed description of the alert, anything that may not have fit in the `message` field.
-        :param pulumi.Input[str] entity: The entity the alert is related to.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] extra_properties: Set of user defined properties specified as a map.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateFilterArgs']]] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
-        :param pulumi.Input[bool] ignore_responders_from_payload: If enabled, the integration will ignore responders sent in request payloads.
-        :param pulumi.Input[bool] ignore_teams_from_payload: If enabled, the integration will ignore teams sent in request payloads.
-        :param pulumi.Input[str] message: Alert text limited to 130 characters.
         :param pulumi.Input[str] note: Additional alert action note.
         :param pulumi.Input[int] order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param pulumi.Input[str] priority: Alert priority.
-        :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateResponderArgs']]] responders: User, schedule, teams or escalation names to calculate which users will receive notifications of the alert.
-        :param pulumi.Input[str] source: User defined field to specify source of action.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Comma separated list of labels to be attached to the alert.
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
         :param pulumi.Input[str] user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alert_actions is not None:
             pulumi.set(__self__, "alert_actions", alert_actions)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
@@ -1651,53 +1601,41 @@
     @append_attachments.setter
     def append_attachments(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "append_attachments", value)
 
     @property
     @pulumi.getter(name="customPriority")
     def custom_priority(self) -> Optional[pulumi.Input[str]]:
-        """
-        Custom alert priority. e.g. ``{{message.substring(0,2)}}``
-        """
         return pulumi.get(self, "custom_priority")
 
     @custom_priority.setter
     def custom_priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_priority", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
-        """
-        Detailed description of the alert, anything that may not have fit in the `message` field.
-        """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
     @property
     @pulumi.getter
     def entity(self) -> Optional[pulumi.Input[str]]:
-        """
-        The entity the alert is related to.
-        """
         return pulumi.get(self, "entity")
 
     @entity.setter
     def entity(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "entity", value)
 
     @property
     @pulumi.getter(name="extraProperties")
     def extra_properties(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
-        """
-        Set of user defined properties specified as a map.
-        """
         return pulumi.get(self, "extra_properties")
 
     @extra_properties.setter
     def extra_properties(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "extra_properties", value)
 
     @property
@@ -1732,17 +1670,14 @@
     @ignore_extra_properties_from_payload.setter
     def ignore_extra_properties_from_payload(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_extra_properties_from_payload", value)
 
     @property
     @pulumi.getter(name="ignoreRespondersFromPayload")
     def ignore_responders_from_payload(self) -> Optional[pulumi.Input[bool]]:
-        """
-        If enabled, the integration will ignore responders sent in request payloads.
-        """
         return pulumi.get(self, "ignore_responders_from_payload")
 
     @ignore_responders_from_payload.setter
     def ignore_responders_from_payload(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_responders_from_payload", value)
 
     @property
@@ -1753,29 +1688,23 @@
     @ignore_tags_from_payload.setter
     def ignore_tags_from_payload(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_tags_from_payload", value)
 
     @property
     @pulumi.getter(name="ignoreTeamsFromPayload")
     def ignore_teams_from_payload(self) -> Optional[pulumi.Input[bool]]:
-        """
-        If enabled, the integration will ignore teams sent in request payloads.
-        """
         return pulumi.get(self, "ignore_teams_from_payload")
 
     @ignore_teams_from_payload.setter
     def ignore_teams_from_payload(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_teams_from_payload", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
-        """
-        Alert text limited to 130 characters.
-        """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
     @property
@@ -1801,65 +1730,50 @@
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[pulumi.Input[str]]:
-        """
-        Alert priority.
-        """
         return pulumi.get(self, "priority")
 
     @priority.setter
     def priority(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "priority", value)
 
     @property
     @pulumi.getter
     def responders(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateResponderArgs']]]]:
-        """
-        User, schedule, teams or escalation names to calculate which users will receive notifications of the alert.
-        """
         return pulumi.get(self, "responders")
 
     @responders.setter
     def responders(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateResponderArgs']]]]):
         pulumi.set(self, "responders", value)
 
     @property
     @pulumi.getter
     def source(self) -> Optional[pulumi.Input[str]]:
-        """
-        User defined field to specify source of action.
-        """
         return pulumi.get(self, "source")
 
     @source.setter
     def source(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "source", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Comma separated list of labels to be attached to the alert.
-        """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
@@ -1876,27 +1790,21 @@
 
 
 @pulumi.input_type
 class IntegrationActionCreateFilterArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  conditions: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionCreateFilterConditionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -2037,15 +1945,14 @@
         """
         :param pulumi.Input[str] name: Name of the integration action.
         :param pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreFilterArgs']]] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param pulumi.Input[int] order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
         """
         pulumi.set(__self__, "name", name)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
         if order is not None:
             pulumi.set(__self__, "order", order)
         if type is not None:
@@ -2089,42 +1996,33 @@
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
     @pulumi.getter
     def type(self) -> Optional[pulumi.Input[str]]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
 
 @pulumi.input_type
 class IntegrationActionIgnoreFilterArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  conditions: Optional[pulumi.Input[Sequence[pulumi.Input['IntegrationActionIgnoreFilterConditionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -2297,55 +2195,41 @@
 
 @pulumi.input_type
 class MaintenanceTimeArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  end_date: Optional[pulumi.Input[str]] = None,
                  start_date: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] type: The type of the entity that maintenance will be applied. It can be either integration or policy.
-        :param pulumi.Input[str] end_date: This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        :param pulumi.Input[str] start_date: This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         pulumi.set(__self__, "type", type)
         if end_date is not None:
             pulumi.set(__self__, "end_date", end_date)
         if start_date is not None:
             pulumi.set(__self__, "start_date", start_date)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        The type of the entity that maintenance will be applied. It can be either integration or policy.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
     @pulumi.getter(name="endDate")
     def end_date(self) -> Optional[pulumi.Input[str]]:
-        """
-        This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         return pulumi.get(self, "end_date")
 
     @end_date.setter
     def end_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "end_date", value)
 
     @property
     @pulumi.getter(name="startDate")
     def start_date(self) -> Optional[pulumi.Input[str]]:
-        """
-        This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         return pulumi.get(self, "start_date")
 
     @start_date.setter
     def start_date(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "start_date", value)
 
 
@@ -3217,15 +3101,14 @@
 @pulumi.input_type
 class NotificationRuleScheduleArgs:
     def __init__(__self__, *,
                  name: pulumi.Input[str],
                  type: pulumi.Input[str]):
         """
         :param pulumi.Input[str] name: Name of the notification policy
-        :param pulumi.Input[str] type: Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
@@ -3237,17 +3120,14 @@
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
 
@@ -3344,29 +3224,23 @@
 
 @pulumi.input_type
 class NotificationRuleTimeRestrictionArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  restriction: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionRestrictionArgs']]]] = None,
                  restrictions: Optional[pulumi.Input[Sequence[pulumi.Input['NotificationRuleTimeRestrictionRestrictionArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restrictions is not None:
             pulumi.set(__self__, "restrictions", restrictions)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
@@ -3502,15 +3376,14 @@
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  restriction: Optional[pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionArgs']]]] = None,
                  restriction_list: Optional[pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionListArgs']]]] = None):
         """
         :param pulumi.Input[str] type: This parameter should be set to `time-of-day` or `weekday-and-time-of-day`.
         :param pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionArgs']]] restriction: It is a restriction object which is described below. In this case startDay/endDay fields are not supported. This can be used only if time restriction type is `time-of-day`.
-        :param pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionListArgs']]] restriction_list: It is a restriction object which is described below. This can be used only if time restriction type is `weekday-and-time-of-day`.
         """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restriction_list is not None:
             pulumi.set(__self__, "restriction_list", restriction_list)
 
@@ -3537,84 +3410,63 @@
     @restriction.setter
     def restriction(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionArgs']]]]):
         pulumi.set(self, "restriction", value)
 
     @property
     @pulumi.getter(name="restrictionList")
     def restriction_list(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionListArgs']]]]:
-        """
-        It is a restriction object which is described below. This can be used only if time restriction type is `weekday-and-time-of-day`.
-        """
         return pulumi.get(self, "restriction_list")
 
     @restriction_list.setter
     def restriction_list(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ScheduleRotationTimeRestrictionRestrictionListArgs']]]]):
         pulumi.set(self, "restriction_list", value)
 
 
 @pulumi.input_type
 class ScheduleRotationTimeRestrictionRestrictionArgs:
     def __init__(__self__, *,
                  end_hour: pulumi.Input[int],
                  end_min: pulumi.Input[int],
                  start_hour: pulumi.Input[int],
                  start_min: pulumi.Input[int]):
-        """
-        :param pulumi.Input[int] end_hour: Value of the hour that frame will end.
-        :param pulumi.Input[int] end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        :param pulumi.Input[int] start_hour: Value of the hour that frame will start.
-        :param pulumi.Input[int] start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> pulumi.Input[int]:
-        """
-        Value of the hour that frame will end.
-        """
         return pulumi.get(self, "end_hour")
 
     @end_hour.setter
     def end_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_hour", value)
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> pulumi.Input[int]:
-        """
-        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "end_min")
 
     @end_min.setter
     def end_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_min", value)
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> pulumi.Input[int]:
-        """
-        Value of the hour that frame will start.
-        """
         return pulumi.get(self, "start_hour")
 
     @start_hour.setter
     def start_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_hour", value)
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> pulumi.Input[int]:
-        """
-        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "start_min")
 
     @start_min.setter
     def start_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_min", value)
 
 
@@ -3623,99 +3475,69 @@
     def __init__(__self__, *,
                  end_day: pulumi.Input[str],
                  end_hour: pulumi.Input[int],
                  end_min: pulumi.Input[int],
                  start_day: pulumi.Input[str],
                  start_hour: pulumi.Input[int],
                  start_min: pulumi.Input[int]):
-        """
-        :param pulumi.Input[str] end_day: Value of the day that frame will end.
-        :param pulumi.Input[int] end_hour: Value of the hour that frame will end.
-        :param pulumi.Input[int] end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-               
-               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
-        :param pulumi.Input[str] start_day: Value of the day that frame will start.
-        :param pulumi.Input[int] start_hour: Value of the hour that frame will start
-        :param pulumi.Input[int] start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_day", start_day)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endDay")
     def end_day(self) -> pulumi.Input[str]:
-        """
-        Value of the day that frame will end.
-        """
         return pulumi.get(self, "end_day")
 
     @end_day.setter
     def end_day(self, value: pulumi.Input[str]):
         pulumi.set(self, "end_day", value)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> pulumi.Input[int]:
-        """
-        Value of the hour that frame will end.
-        """
         return pulumi.get(self, "end_hour")
 
     @end_hour.setter
     def end_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_hour", value)
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> pulumi.Input[int]:
-        """
-        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-
-        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
-        """
         return pulumi.get(self, "end_min")
 
     @end_min.setter
     def end_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "end_min", value)
 
     @property
     @pulumi.getter(name="startDay")
     def start_day(self) -> pulumi.Input[str]:
-        """
-        Value of the day that frame will start.
-        """
         return pulumi.get(self, "start_day")
 
     @start_day.setter
     def start_day(self, value: pulumi.Input[str]):
         pulumi.set(self, "start_day", value)
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> pulumi.Input[int]:
-        """
-        Value of the hour that frame will start
-        """
         return pulumi.get(self, "start_hour")
 
     @start_hour.setter
     def start_hour(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_hour", value)
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> pulumi.Input[int]:
-        """
-        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "start_min")
 
     @start_min.setter
     def start_min(self, value: pulumi.Input[int]):
         pulumi.set(self, "start_min", value)
 
 
@@ -4239,29 +4061,23 @@
 
 @pulumi.input_type
 class TeamRoutingRuleTimeRestrictionArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  restriction: Optional[pulumi.Input[Sequence[pulumi.Input['TeamRoutingRuleTimeRestrictionRestrictionArgs']]]] = None,
                  restriction_list: Optional[pulumi.Input[Sequence[pulumi.Input['TeamRoutingRuleTimeRestrictionRestrictionListArgs']]]] = None):
-        """
-        :param pulumi.Input[str] type: Type of the operation will be applied on conditions. Should be one of `match-all`, `match-any-condition` or `match-all-conditions`.
-        """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restriction_list is not None:
             pulumi.set(__self__, "restriction_list", restriction_list)
 
     @property
     @pulumi.getter
     def type(self) -> pulumi.Input[str]:
-        """
-        Type of the operation will be applied on conditions. Should be one of `match-all`, `match-any-condition` or `match-all-conditions`.
-        """
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: pulumi.Input[str]):
         pulumi.set(self, "type", value)
 
     @property
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/_utilities.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/alert_policy.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/alert_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -695,15 +695,14 @@
                  time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['AlertPolicyTimeRestrictionArgs']]]]] = None,
                  __props__=None):
         """
         Manages a Alert Policy within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example team",
             description="This team deals with all the things")
@@ -731,15 +730,14 @@
                         start_day="monday",
                         start_hour=22,
                         start_min=0,
                     ),
                 ],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alert policies can be imported using the `team_id/policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/alertPolicy:AlertPolicy test team_id/policy_id`
@@ -781,15 +779,14 @@
                  args: AlertPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Alert Policy within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example team",
             description="This team deals with all the things")
@@ -817,15 +814,14 @@
                         start_day="monday",
                         start_hour=22,
                         start_min=0,
                     ),
                 ],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Alert policies can be imported using the `team_id/policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/alertPolicy:AlertPolicy test team_id/policy_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/api_integration.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/api_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/config/vars.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/custom_role.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/custom_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,29 +165,27 @@
                  role_name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages custom user roles within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.CustomRole("test",
             role_name="genierole",
             extended_role="user",
             granted_rights=["alert-delete"],
             disallowed_rights=[
                 "profile-edit",
                 "contacts-edit",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] disallowed_rights: The rights this role cannot have. For allowed values please refer [User Right Prerequisites](https://docs.opsgenie.com/docs/custom-user-role-api#section-user-right-prerequisites)
         :param pulumi.Input[str] extended_role: The role from which this role has been derived. Allowed Values: "user", "observer", "stakeholder".
         :param pulumi.Input[Sequence[pulumi.Input[str]]] granted_rights: The rights granted to this role. For allowed values please refer [User Right Prerequisites](https://docs.opsgenie.com/docs/custom-user-role-api#section-user-right-prerequisites)
         :param pulumi.Input[str] role_name: Name of the custom role.
@@ -199,29 +197,27 @@
                  args: CustomRoleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages custom user roles within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.CustomRole("test",
             role_name="genierole",
             extended_role="user",
             granted_rights=["alert-delete"],
             disallowed_rights=[
                 "profile-edit",
                 "contacts-edit",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param CustomRoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/email_integration.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/email_integration.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/escalation.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/escalation.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,14 @@
         """
         Manages an Escalation within Opsgenie.
 
         ## Example Usage
 
         An escalation with a single rule
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
             name="genieescalation",
             rules=[opsgenie.EscalationRuleArgs(
@@ -219,19 +218,17 @@
                 delay=1,
                 recipients=[opsgenie.EscalationRuleRecipientArgs(
                     type="user",
                     id=test["id"],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         An escalation with a multiple rules
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
             name="genieescalation",
             description="test",
@@ -268,15 +265,14 @@
             repeats=[opsgenie.EscalationRepeatArgs(
                 wait_interval=10,
                 count=1,
                 reset_recipient_states=True,
                 close_alert_after_all=False,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Escalations can be imported using the `escalation_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/escalation:Escalation test escalation_id`
@@ -299,15 +295,14 @@
         """
         Manages an Escalation within Opsgenie.
 
         ## Example Usage
 
         An escalation with a single rule
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
             name="genieescalation",
             rules=[opsgenie.EscalationRuleArgs(
@@ -316,19 +311,17 @@
                 delay=1,
                 recipients=[opsgenie.EscalationRuleRecipientArgs(
                     type="user",
                     id=test["id"],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         An escalation with a multiple rules
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         default = opsgenie.Escalation("default",
             name="genieescalation",
             description="test",
@@ -365,15 +358,14 @@
             repeats=[opsgenie.EscalationRepeatArgs(
                 wait_interval=10,
                 count=1,
                 reset_recipient_states=True,
                 close_alert_after_all=False,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Escalations can be imported using the `escalation_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/escalation:Escalation test escalation_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_escalation.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_escalation.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,22 +110,20 @@
                    rules: Optional[Sequence[pulumi.InputType['GetEscalationRuleArgs']]] = None,
                    opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetEscalationResult:
     """
     Manages an Escalation within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_escalation(name="existing-escalation")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Escalation Description
     :param str name: Name of the escalation.
     :param str owner_team_id: If owner team exist the id of the team is exported
     :param Sequence[pulumi.InputType['GetEscalationRepeatArgs']] repeats: Escalation repeat preferences
     :param Sequence[pulumi.InputType['GetEscalationRuleArgs']] rules: Escalation rules
@@ -156,22 +154,20 @@
                           rules: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetEscalationRuleArgs']]]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEscalationResult]:
     """
     Manages an Escalation within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_escalation(name="existing-escalation")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Escalation Description
     :param str name: Name of the escalation.
     :param str owner_team_id: If owner team exist the id of the team is exported
     :param Sequence[pulumi.InputType['GetEscalationRepeatArgs']] repeats: Escalation repeat preferences
     :param Sequence[pulumi.InputType['GetEscalationRuleArgs']] rules: Escalation rules
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_heartbeat.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,22 +160,20 @@
                   owner_team_id: Optional[str] = None,
                   opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetHeartbeatResult:
     """
     Manages existing heartbeat within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_heartbeat(name="genieheartbeat-existing")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str alert_message: Specifies the alert message for heartbeat expiration alert. If this is not provided, default alert message is "HeartbeatName is expired".
     :param str alert_priority: Specifies the alert priority for heartbeat expiration alert. If this is not provided, default priority is P3.
     :param Sequence[str] alert_tags: Specifies the alert tags for heartbeat expiration alert.
     :param str description: An optional description of the heartbeat
     :param bool enabled: Enable/disable heartbeat monitoring.
@@ -222,22 +220,20 @@
                          owner_team_id: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetHeartbeatResult]:
     """
     Manages existing heartbeat within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_heartbeat(name="genieheartbeat-existing")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str alert_message: Specifies the alert message for heartbeat expiration alert. If this is not provided, default alert message is "HeartbeatName is expired".
     :param str alert_priority: Specifies the alert priority for heartbeat expiration alert. If this is not provided, default priority is P3.
     :param Sequence[str] alert_tags: Specifies the alert tags for heartbeat expiration alert.
     :param str description: An optional description of the heartbeat
     :param bool enabled: Enable/disable heartbeat monitoring.
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_schedule.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,22 +108,20 @@
                  timezone: Optional[str] = None,
                  opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetScheduleResult:
     """
     Manages a Schedule within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_schedule(name="sre-team schedule")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Timezone of schedule. Please look at [Supported Timezone Ids](https://docs.opsgenie.com/docs/supported-timezone-ids) for available timezones - Default: `America/New_York`.
     :param bool enabled: Enable/disable state of schedule
     :param str name: Name of the schedule.
     :param str owner_team_id: Owner team id of the schedule.
     :param str timezone: The description of schedule.
@@ -154,22 +152,20 @@
                         timezone: Optional[pulumi.Input[Optional[str]]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetScheduleResult]:
     """
     Manages a Schedule within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_schedule(name="sre-team schedule")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Timezone of schedule. Please look at [Supported Timezone Ids](https://docs.opsgenie.com/docs/supported-timezone-ids) for available timezones - Default: `America/New_York`.
     :param bool enabled: Enable/disable state of schedule
     :param str name: Name of the schedule.
     :param str owner_team_id: Owner team id of the schedule.
     :param str timezone: The description of schedule.
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_service.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,22 +76,20 @@
                 team_id: Optional[str] = None,
                 opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetServiceResult:
     """
     Manages existing Service within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     this = opsgenie.get_service(name="Payment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Description field of the service that is generally used to provide a detailed information about the service.
     :param str name: Name of the service. This field must not be longer than 100 characters.
            
            The following attributes are exported:
     :param str team_id: Team id of the service.
@@ -116,22 +114,20 @@
                        team_id: Optional[pulumi.Input[Optional[str]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServiceResult]:
     """
     Manages existing Service within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     this = opsgenie.get_service(name="Payment")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: Description field of the service that is generally used to provide a detailed information about the service.
     :param str name: Name of the service. This field must not be longer than 100 characters.
            
            The following attributes are exported:
     :param str team_id: Team id of the service.
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_team.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_team.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,22 +78,20 @@
              name: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetTeamResult:
     """
     Manages existing Team within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     sre_team = opsgenie.get_team(name="sre-team")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: A description for this team.
     :param Sequence[pulumi.InputType['GetTeamMemberArgs']] members: A Member block as documented below.
     :param str name: The name associated with this team. Opsgenie defines that this must not be longer than 100 characters.
            
            The following attributes are exported:
@@ -118,22 +116,20 @@
                     name: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTeamResult]:
     """
     Manages existing Team within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     sre_team = opsgenie.get_team(name="sre-team")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str description: A description for this team.
     :param Sequence[pulumi.InputType['GetTeamMemberArgs']] members: A Member block as documented below.
     :param str name: The name associated with this team. Opsgenie defines that this must not be longer than 100 characters.
            
            The following attributes are exported:
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/get_user.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/get_user.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,22 +108,20 @@
              username: Optional[str] = None,
              opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetUserResult:
     """
     Manages existing User within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_user(username="user@domain.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: The Full Name of the User.
     :param str locale: Location information for the user. Please look at [Supported Locale Ids](https://docs.opsgenie.com/docs/supported-locales) for available locales.
     :param str role: The Role assigned to the User. Either a built-in such as 'Owner', 'Admin' or 'User' - or the name of a custom role.
     :param str timezone: Timezone information of the user. Please look at [Supported Timezone Ids](https://docs.opsgenie.com/docs/supported-timezone-ids) for available timezones.
     :param str username: The email address associated with this user. Opsgenie defines that this must not be longer than 100 characters.
@@ -154,22 +152,20 @@
                     username: Optional[pulumi.Input[str]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserResult]:
     """
     Manages existing User within Opsgenie.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_opsgenie as opsgenie
 
     test = opsgenie.get_user(username="user@domain.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str full_name: The Full Name of the User.
     :param str locale: Location information for the user. Please look at [Supported Locale Ids](https://docs.opsgenie.com/docs/supported-locales) for available locales.
     :param str role: The Role assigned to the User. Either a built-in such as 'Owner', 'Admin' or 'User' - or the name of a custom role.
     :param str timezone: Timezone information of the user. Please look at [Supported Timezone Ids](https://docs.opsgenie.com/docs/supported-timezone-ids) for available timezones.
     :param str username: The email address associated with this user. Opsgenie defines that this must not be longer than 100 characters.
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/heartbeat.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/heartbeat.py`

 * *Files 2% similar despite different names*

```diff
@@ -328,15 +328,14 @@
                  owner_team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages heartbeat within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Heartbeat("test",
             name="genieheartbeat-test",
             description="test opsgenie heartbeat terraform",
@@ -347,15 +346,14 @@
             alert_priority="P3",
             alert_tags=[
                 "test",
                 "fahri",
             ],
             owner_team_id=test_opsgenie_team["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Heartbeat Integrations can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/heartbeat:Heartbeat test name`
@@ -380,15 +378,14 @@
                  args: HeartbeatArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages heartbeat within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Heartbeat("test",
             name="genieheartbeat-test",
             description="test opsgenie heartbeat terraform",
@@ -399,15 +396,14 @@
             alert_priority="P3",
             alert_tags=[
                 "test",
                 "fahri",
             ],
             owner_team_id=test_opsgenie_team["id"])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Heartbeat Integrations can be imported using the `name`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/heartbeat:Heartbeat test name`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/incident_template.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/incident_template.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,17 +22,17 @@
                  description: Optional[pulumi.Input[str]] = None,
                  details: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  impacted_services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a IncidentTemplate resource.
-        :param pulumi.Input[str] message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
-        :param pulumi.Input[str] description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         pulumi.set(__self__, "message", message)
         pulumi.set(__self__, "priority", priority)
         pulumi.set(__self__, "stakeholder_properties", stakeholder_properties)
@@ -47,15 +47,15 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Input[str]:
         """
-        Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        Message of the related incident template. This field must not be longer than 130 characters.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: pulumi.Input[str]):
         pulumi.set(self, "message", value)
 
@@ -80,15 +80,15 @@
     def stakeholder_properties(self, value: pulumi.Input[Sequence[pulumi.Input['IncidentTemplateStakeholderPropertyArgs']]]):
         pulumi.set(self, "stakeholder_properties", value)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        Description field of the incident template. This field must not be longer than 10000 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -147,17 +147,17 @@
                  message: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  priority: Optional[pulumi.Input[str]] = None,
                  stakeholder_properties: Optional[pulumi.Input[Sequence[pulumi.Input['IncidentTemplateStakeholderPropertyArgs']]]] = None,
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
         Input properties used for looking up and filtering IncidentTemplate resources.
-        :param pulumi.Input[str] description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
-        :param pulumi.Input[str] message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         if description is not None:
             pulumi.set(__self__, "description", description)
         if details is not None:
@@ -175,15 +175,15 @@
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter
     def description(self) -> Optional[pulumi.Input[str]]:
         """
-        Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        Description field of the incident template. This field must not be longer than 10000 characters.
         """
         return pulumi.get(self, "description")
 
     @description.setter
     def description(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "description", value)
 
@@ -208,15 +208,15 @@
     def impacted_services(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "impacted_services", value)
 
     @property
     @pulumi.getter
     def message(self) -> Optional[pulumi.Input[str]]:
         """
-        Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        Message of the related incident template. This field must not be longer than 130 characters.
         """
         return pulumi.get(self, "message")
 
     @message.setter
     def message(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "message", value)
 
@@ -281,15 +281,14 @@
                  tags: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         Manages an Incident Template within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="genietest-team",
             description="This team deals with all the things")
@@ -312,29 +311,28 @@
             description="Incident Description",
             details={
                 "key1": "value1",
                 "key2": "value2",
             },
             impacted_services=[test_service.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service can be imported using the `template_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/incidentTemplate:IncidentTemplate test template_id`
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
-        :param pulumi.Input[str] message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         ...
     @overload
     def __init__(__self__,
@@ -342,15 +340,14 @@
                  args: IncidentTemplateArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages an Incident Template within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="genietest-team",
             description="This team deals with all the things")
@@ -373,15 +370,14 @@
             description="Incident Description",
             details={
                 "key1": "value1",
                 "key2": "value2",
             },
             impacted_services=[test_service.id])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service can be imported using the `template_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/incidentTemplate:IncidentTemplate test template_id`
@@ -454,17 +450,17 @@
         """
         Get an existing IncidentTemplate resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[str] description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        :param pulumi.Input[str] description: Description field of the incident template. This field must not be longer than 10000 characters.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] details: Map of key-value pairs to use as custom properties of the incident template. This field must not be longer than 8000 characters.
-        :param pulumi.Input[str] message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        :param pulumi.Input[str] message: Message of the related incident template. This field must not be longer than 130 characters.
         :param pulumi.Input[str] name: Name of the incident template.
         :param pulumi.Input[str] priority: Priority level of the incident. Possible values are `P1`, `P2`, `P3`, `P4` and `P5`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] tags: Tags of the incident template.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _IncidentTemplateState.__new__(_IncidentTemplateState)
@@ -479,15 +475,15 @@
         __props__.__dict__["tags"] = tags
         return IncidentTemplate(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
     def description(self) -> pulumi.Output[Optional[str]]:
         """
-        Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        Description field of the incident template. This field must not be longer than 10000 characters.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def details(self) -> pulumi.Output[Optional[Mapping[str, str]]]:
         """
@@ -500,15 +496,15 @@
     def impacted_services(self) -> pulumi.Output[Optional[Sequence[str]]]:
         return pulumi.get(self, "impacted_services")
 
     @property
     @pulumi.getter
     def message(self) -> pulumi.Output[str]:
         """
-        Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        Message of the related incident template. This field must not be longer than 130 characters.
         """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/integration_action.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/integration_action.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,15 +202,14 @@
         * `close`
         * `acknowledge`
         * `add_note`
         * `ignore`
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
         import pulumi_std as std
 
         test_action = opsgenie.IntegrationAction("test_action",
             integration_id=test_opsgenie_api_integration["id"],
@@ -346,15 +345,14 @@
                         field="tags",
                         operation="contains",
                         expected_value="ignore",
                     )],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] integration_id: ID of the parent integration resource to bind to.
         """
         ...
     @overload
@@ -372,15 +370,14 @@
         * `close`
         * `acknowledge`
         * `add_note`
         * `ignore`
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
         import pulumi_std as std
 
         test_action = opsgenie.IntegrationAction("test_action",
             integration_id=test_opsgenie_api_integration["id"],
@@ -516,15 +513,14 @@
                         field="tags",
                         operation="contains",
                         expected_value="ignore",
                     )],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param IntegrationActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/maintenance.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/maintenance.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_policy.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/notification_policy.py`

 * *Files 1% similar despite different names*

```diff
@@ -397,15 +397,14 @@
                  time_restrictions: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationPolicyTimeRestrictionArgs']]]]] = None,
                  __props__=None):
         """
         Manages a Notification Policy within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example team",
             description="This team deals with all the things")
@@ -416,15 +415,14 @@
             policy_description="This policy has a delay action",
             delay_actions=[opsgenie.NotificationPolicyDelayActionArgs(
                 delay_option="next-time",
                 until_minute=1,
                 until_hour=9,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `team_id` and `notification_policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/notificationPolicy:NotificationPolicy test team_id/notification_policy_id`
@@ -451,15 +449,14 @@
                  args: NotificationPolicyArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Notification Policy within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example team",
             description="This team deals with all the things")
@@ -470,15 +467,14 @@
             policy_description="This policy has a delay action",
             delay_actions=[opsgenie.NotificationPolicyDelayActionArgs(
                 delay_option="next-time",
                 until_minute=1,
                 until_hour=9,
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `team_id` and `notification_policy_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/notificationPolicy:NotificationPolicy test team_id/notification_policy_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/notification_rule.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/notification_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         """
         The set of arguments for constructing a NotificationRule resource.
         :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
         :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
         :param pulumi.Input[str] name: Name of the notification policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
-        :param pulumi.Input[int] order: Order of the condition in conditions list
         :param pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
         """
         pulumi.set(__self__, "action_type", action_type)
         pulumi.set(__self__, "username", username)
         if criterias is not None:
             pulumi.set(__self__, "criterias", criterias)
         if enabled is not None:
@@ -126,17 +125,14 @@
     @notification_times.setter
     def notification_times(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notification_times", value)
 
     @property
     @pulumi.getter
     def order(self) -> Optional[pulumi.Input[int]]:
-        """
-        Order of the condition in conditions list
-        """
         return pulumi.get(self, "order")
 
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
@@ -195,15 +191,14 @@
                  username: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering NotificationRule resources.
         :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
         :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
         :param pulumi.Input[str] name: Name of the notification policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
-        :param pulumi.Input[int] order: Order of the condition in conditions list
         :param pulumi.Input[Sequence[pulumi.Input['NotificationRuleStepArgs']]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
         :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
         if action_type is not None:
             pulumi.set(__self__, "action_type", action_type)
         if criterias is not None:
             pulumi.set(__self__, "criterias", criterias)
@@ -282,17 +277,14 @@
     @notification_times.setter
     def notification_times(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "notification_times", value)
 
     @property
     @pulumi.getter
     def order(self) -> Optional[pulumi.Input[int]]:
-        """
-        Order of the condition in conditions list
-        """
         return pulumi.get(self, "order")
 
     @order.setter
     def order(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "order", value)
 
     @property
@@ -365,15 +357,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Notification Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
             username="Example user",
             full_name="Name Lastname",
@@ -389,15 +380,14 @@
             steps=[opsgenie.NotificationRuleStepArgs(
                 contacts=[opsgenie.NotificationRuleStepContactArgs(
                     method="email",
                     to="example@user.com",
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `user_id/notification_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/notificationRule:NotificationRule test user_id/notification_rule_id`
@@ -405,30 +395,28 @@
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
         :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
         :param pulumi.Input[str] name: Name of the notification policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
-        :param pulumi.Input[int] order: Order of the condition in conditions list
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
         :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: NotificationRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Notification Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
             username="Example user",
             full_name="Name Lastname",
@@ -444,15 +432,14 @@
             steps=[opsgenie.NotificationRuleStepArgs(
                 contacts=[opsgenie.NotificationRuleStepContactArgs(
                     method="email",
                     to="example@user.com",
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Notification policies can be imported using the `user_id/notification_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/notificationRule:NotificationRule test user_id/notification_rule_id`
@@ -536,15 +523,14 @@
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action_type: Type of the action that notification rule will have. Allowed values: `create-alert`, `acknowledged-alert`, `closed-alert`, `assigned-alert`, `add-note`, `schedule-start`, `schedule-end`, `incoming-call-routing`
         :param pulumi.Input[bool] enabled: If policy should be enabled. Default: `true`
         :param pulumi.Input[str] name: Name of the notification policy
         :param pulumi.Input[Sequence[pulumi.Input[str]]] notification_times: List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
-        :param pulumi.Input[int] order: Order of the condition in conditions list
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['NotificationRuleStepArgs']]]] steps: Notification rule steps to take (eg. SMS or email message). This is a block, structure is documented below.
         :param pulumi.Input[str] username: Username of user to which this notification rule belongs to.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _NotificationRuleState.__new__(_NotificationRuleState)
 
@@ -597,17 +583,14 @@
         List of Time Periods that notification for schedule start/end will be sent. Allowed values: `just-before`, `15-minutes-ago`, `1-hour-ago`, `1-day-ago`. If `action_type` is `schedule-start` or `schedule-end` then it is required.
         """
         return pulumi.get(self, "notification_times")
 
     @property
     @pulumi.getter
     def order(self) -> pulumi.Output[int]:
-        """
-        Order of the condition in conditions list
-        """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def repeats(self) -> pulumi.Output[Optional[Sequence['outputs.NotificationRuleRepeat']]]:
         return pulumi.get(self, "repeats")
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/outputs.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/outputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -531,36 +531,32 @@
 
 @pulumi.output_type
 class EmailIntegrationResponder(dict):
     def __init__(__self__, *,
                  id: Optional[str] = None,
                  type: Optional[str] = None):
         """
-        :param str id: The id of the responder.
-        :param str type: The responder type.
+        :param str id: The ID of the Opsgenie Email based Integration.
         """
         if id is not None:
             pulumi.set(__self__, "id", id)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
-        The id of the responder.
+        The ID of the Opsgenie Email based Integration.
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type.
-        """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class EscalationRepeat(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -716,46 +712,42 @@
 @pulumi.output_type
 class IncidentTemplateStakeholderProperty(dict):
     def __init__(__self__, *,
                  message: str,
                  description: Optional[str] = None,
                  enable: Optional[bool] = None):
         """
-        :param str message: Message that is to be passed to audience that is generally used to provide a content information about the alert.
-        :param str description: Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
-        :param bool enable: Option to enable stakeholder notifications.Default value is true.
+        :param str message: Message of the related incident template. This field must not be longer than 130 characters.
+        :param str description: Description field of the incident template. This field must not be longer than 10000 characters.
         """
         pulumi.set(__self__, "message", message)
         if description is not None:
             pulumi.set(__self__, "description", description)
         if enable is not None:
             pulumi.set(__self__, "enable", enable)
 
     @property
     @pulumi.getter
     def message(self) -> str:
         """
-        Message that is to be passed to audience that is generally used to provide a content information about the alert.
+        Message of the related incident template. This field must not be longer than 130 characters.
         """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
         """
-        Description that is generally used to provide a detailed information about the alert. This field must not be longer than 15000 characters.
+        Description field of the incident template. This field must not be longer than 10000 characters.
         """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def enable(self) -> Optional[bool]:
-        """
-        Option to enable stakeholder notifications.Default value is true.
-        """
         return pulumi.get(self, "enable")
 
 
 @pulumi.output_type
 class IntegrationActionAcknowledge(dict):
     def __init__(__self__, *,
                  name: str,
@@ -770,15 +762,14 @@
         :param str alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param Sequence['IntegrationActionAcknowledgeFilterArgs'] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param str note: Additional alert action note.
         :param int order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
         :param str user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -833,17 +824,14 @@
         Integer value that defines in which order the action will be performed. Default: `1`.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
         Owner of the execution for integration action.
@@ -852,27 +840,21 @@
 
 
 @pulumi.output_type
 class IntegrationActionAcknowledgeFilter(dict):
     def __init__(__self__, *,
                  type: str,
                  conditions: Optional[Sequence['outputs.IntegrationActionAcknowledgeFilterCondition']] = None):
-        """
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def conditions(self) -> Optional[Sequence['outputs.IntegrationActionAcknowledgeFilterCondition']]:
         return pulumi.get(self, "conditions")
 
@@ -968,15 +950,14 @@
         :param str alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param Sequence['IntegrationActionAddNoteFilterArgs'] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param str note: Additional alert action note.
         :param int order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
         :param str user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -1031,17 +1012,14 @@
         Integer value that defines in which order the action will be performed. Default: `1`.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
         Owner of the execution for integration action.
@@ -1050,27 +1028,21 @@
 
 
 @pulumi.output_type
 class IntegrationActionAddNoteFilter(dict):
     def __init__(__self__, *,
                  type: str,
                  conditions: Optional[Sequence['outputs.IntegrationActionAddNoteFilterCondition']] = None):
-        """
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def conditions(self) -> Optional[Sequence['outputs.IntegrationActionAddNoteFilterCondition']]:
         return pulumi.get(self, "conditions")
 
@@ -1166,15 +1138,14 @@
         :param str alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
         :param Sequence['IntegrationActionCloseFilterArgs'] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param str note: Additional alert action note.
         :param int order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
         :param str user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
@@ -1229,17 +1200,14 @@
         Integer value that defines in which order the action will be performed. Default: `1`.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
         Owner of the execution for integration action.
@@ -1248,27 +1216,21 @@
 
 
 @pulumi.output_type
 class IntegrationActionCloseFilter(dict):
     def __init__(__self__, *,
                  type: str,
                  conditions: Optional[Sequence['outputs.IntegrationActionCloseFilterCondition']] = None):
-        """
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def conditions(self) -> Optional[Sequence['outputs.IntegrationActionCloseFilterCondition']]:
         return pulumi.get(self, "conditions")
 
@@ -1407,32 +1369,20 @@
                  source: Optional[str] = None,
                  tags: Optional[Sequence[str]] = None,
                  type: Optional[str] = None,
                  user: Optional[str] = None):
         """
         :param str name: Name of the integration action.
         :param str alias: An identifier that is used for alert deduplication. Default: `{{alias}}`.
-        :param str custom_priority: Custom alert priority. e.g. ``{{message.substring(0,2)}}``
-        :param str description: Detailed description of the alert, anything that may not have fit in the `message` field.
-        :param str entity: The entity the alert is related to.
-        :param Mapping[str, str] extra_properties: Set of user defined properties specified as a map.
         :param Sequence['IntegrationActionCreateFilterArgs'] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
-        :param bool ignore_responders_from_payload: If enabled, the integration will ignore responders sent in request payloads.
-        :param bool ignore_teams_from_payload: If enabled, the integration will ignore teams sent in request payloads.
-        :param str message: Alert text limited to 130 characters.
         :param str note: Additional alert action note.
         :param int order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param str priority: Alert priority.
-        :param Sequence['IntegrationActionCreateResponderArgs'] responders: User, schedule, teams or escalation names to calculate which users will receive notifications of the alert.
-        :param str source: User defined field to specify source of action.
-        :param Sequence[str] tags: Comma separated list of labels to be attached to the alert.
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
         :param str user: Owner of the execution for integration action.
         """
         pulumi.set(__self__, "name", name)
         if alert_actions is not None:
             pulumi.set(__self__, "alert_actions", alert_actions)
         if alias is not None:
             pulumi.set(__self__, "alias", alias)
@@ -1502,41 +1452,29 @@
     @pulumi.getter(name="appendAttachments")
     def append_attachments(self) -> Optional[bool]:
         return pulumi.get(self, "append_attachments")
 
     @property
     @pulumi.getter(name="customPriority")
     def custom_priority(self) -> Optional[str]:
-        """
-        Custom alert priority. e.g. ``{{message.substring(0,2)}}``
-        """
         return pulumi.get(self, "custom_priority")
 
     @property
     @pulumi.getter
     def description(self) -> Optional[str]:
-        """
-        Detailed description of the alert, anything that may not have fit in the `message` field.
-        """
         return pulumi.get(self, "description")
 
     @property
     @pulumi.getter
     def entity(self) -> Optional[str]:
-        """
-        The entity the alert is related to.
-        """
         return pulumi.get(self, "entity")
 
     @property
     @pulumi.getter(name="extraProperties")
     def extra_properties(self) -> Optional[Mapping[str, str]]:
-        """
-        Set of user defined properties specified as a map.
-        """
         return pulumi.get(self, "extra_properties")
 
     @property
     @pulumi.getter
     def filters(self) -> Optional[Sequence['outputs.IntegrationActionCreateFilter']]:
         """
         Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
@@ -1555,38 +1493,29 @@
     @pulumi.getter(name="ignoreExtraPropertiesFromPayload")
     def ignore_extra_properties_from_payload(self) -> Optional[bool]:
         return pulumi.get(self, "ignore_extra_properties_from_payload")
 
     @property
     @pulumi.getter(name="ignoreRespondersFromPayload")
     def ignore_responders_from_payload(self) -> Optional[bool]:
-        """
-        If enabled, the integration will ignore responders sent in request payloads.
-        """
         return pulumi.get(self, "ignore_responders_from_payload")
 
     @property
     @pulumi.getter(name="ignoreTagsFromPayload")
     def ignore_tags_from_payload(self) -> Optional[bool]:
         return pulumi.get(self, "ignore_tags_from_payload")
 
     @property
     @pulumi.getter(name="ignoreTeamsFromPayload")
     def ignore_teams_from_payload(self) -> Optional[bool]:
-        """
-        If enabled, the integration will ignore teams sent in request payloads.
-        """
         return pulumi.get(self, "ignore_teams_from_payload")
 
     @property
     @pulumi.getter
     def message(self) -> Optional[str]:
-        """
-        Alert text limited to 130 characters.
-        """
         return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def note(self) -> Optional[str]:
         """
         Additional alert action note.
@@ -1600,49 +1529,34 @@
         Integer value that defines in which order the action will be performed. Default: `1`.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def priority(self) -> Optional[str]:
-        """
-        Alert priority.
-        """
         return pulumi.get(self, "priority")
 
     @property
     @pulumi.getter
     def responders(self) -> Optional[Sequence['outputs.IntegrationActionCreateResponder']]:
-        """
-        User, schedule, teams or escalation names to calculate which users will receive notifications of the alert.
-        """
         return pulumi.get(self, "responders")
 
     @property
     @pulumi.getter
     def source(self) -> Optional[str]:
-        """
-        User defined field to specify source of action.
-        """
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[Sequence[str]]:
-        """
-        Comma separated list of labels to be attached to the alert.
-        """
         return pulumi.get(self, "tags")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
         Owner of the execution for integration action.
@@ -1651,27 +1565,21 @@
 
 
 @pulumi.output_type
 class IntegrationActionCreateFilter(dict):
     def __init__(__self__, *,
                  type: str,
                  conditions: Optional[Sequence['outputs.IntegrationActionCreateFilterCondition']] = None):
-        """
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def conditions(self) -> Optional[Sequence['outputs.IntegrationActionCreateFilterCondition']]:
         return pulumi.get(self, "conditions")
 
@@ -1791,15 +1699,14 @@
         """
         :param str name: Name of the integration action.
         :param Sequence['IntegrationActionIgnoreFilterArgs'] filters: Used to specify rules for matching alerts and the filter type. Please note that depending on the integration type the field names in the filter conditions are:
                * For SNS integration: `actions`, `alias`, `entity`, `Message`, `recipients`, `responders`, `Subject`, `tags`, `teams`, `eventType`, `Timestamp`, `TopicArn`.
                * For API integration: `message`, `alias`, `description`, `source`, `entity`, `tags`, `actions`, `details`, `extra-properties`, `recipients`, `teams`, `priority`, `eventType`.
                * For Email integration: `from_address`, `from_name`, `conversationSubject`, `subject`
         :param int order: Integer value that defines in which order the action will be performed. Default: `1`.
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
         """
         pulumi.set(__self__, "name", name)
         if filters is not None:
             pulumi.set(__self__, "filters", filters)
         if order is not None:
             pulumi.set(__self__, "order", order)
         if type is not None:
@@ -1831,38 +1738,29 @@
         Integer value that defines in which order the action will be performed. Default: `1`.
         """
         return pulumi.get(self, "order")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class IntegrationActionIgnoreFilter(dict):
     def __init__(__self__, *,
                  type: str,
                  conditions: Optional[Sequence['outputs.IntegrationActionIgnoreFilterCondition']] = None):
-        """
-        :param str type: The responder type - can be `escalation`, `team` or `user`.
-        """
         pulumi.set(__self__, "type", type)
         if conditions is not None:
             pulumi.set(__self__, "conditions", conditions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The responder type - can be `escalation`, `team` or `user`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def conditions(self) -> Optional[Sequence['outputs.IntegrationActionIgnoreFilterCondition']]:
         return pulumi.get(self, "conditions")
 
@@ -2025,47 +1923,33 @@
         MaintenanceTime.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  type: str,
                  end_date: Optional[str] = None,
                  start_date: Optional[str] = None):
-        """
-        :param str type: The type of the entity that maintenance will be applied. It can be either integration or policy.
-        :param str end_date: This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        :param str start_date: This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         pulumi.set(__self__, "type", type)
         if end_date is not None:
             pulumi.set(__self__, "end_date", end_date)
         if start_date is not None:
             pulumi.set(__self__, "start_date", start_date)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        The type of the entity that maintenance will be applied. It can be either integration or policy.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="endDate")
     def end_date(self) -> Optional[str]:
-        """
-        This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         return pulumi.get(self, "end_date")
 
     @property
     @pulumi.getter(name="startDate")
     def start_date(self) -> Optional[str]:
-        """
-        This parameter takes a date format as (yyyy-MM-dd'T'HH:mm:ssZ) (e.g. 2019-06-11T08:00:00+02:00).
-        """
         return pulumi.get(self, "start_date")
 
 
 @pulumi.output_type
 class NotificationPolicyAutoCloseAction(dict):
     def __init__(__self__, *,
                  durations: Sequence['outputs.NotificationPolicyAutoCloseActionDuration']):
@@ -2990,15 +2874,14 @@
 @pulumi.output_type
 class NotificationRuleSchedule(dict):
     def __init__(__self__, *,
                  name: str,
                  type: str):
         """
         :param str name: Name of the notification policy
-        :param str type: Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
         """
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter
     def name(self) -> str:
@@ -3006,17 +2889,14 @@
         Name of the notification policy
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         return pulumi.get(self, "type")
 
 
 @pulumi.output_type
 class NotificationRuleStep(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3106,29 +2986,23 @@
 
 @pulumi.output_type
 class NotificationRuleTimeRestriction(dict):
     def __init__(__self__, *,
                  type: str,
                  restriction: Optional[Sequence['outputs.NotificationRuleTimeRestrictionRestriction']] = None,
                  restrictions: Optional[Sequence['outputs.NotificationRuleTimeRestrictionRestriction']] = None):
-        """
-        :param str type: Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restrictions is not None:
             pulumi.set(__self__, "restrictions", restrictions)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Kind of matching filter. Possible values: `match-all`, `match-any-condition`, `match-all-conditions`
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def restriction(self) -> Optional[Sequence['outputs.NotificationRuleTimeRestrictionRestriction']]:
         return pulumi.get(self, "restriction")
 
@@ -3264,15 +3138,14 @@
     def __init__(__self__, *,
                  type: str,
                  restriction: Optional[Sequence['outputs.ScheduleRotationTimeRestrictionRestriction']] = None,
                  restriction_list: Optional[Sequence['outputs.ScheduleRotationTimeRestrictionRestrictionList']] = None):
         """
         :param str type: This parameter should be set to `time-of-day` or `weekday-and-time-of-day`.
         :param Sequence['ScheduleRotationTimeRestrictionRestrictionArgs'] restriction: It is a restriction object which is described below. In this case startDay/endDay fields are not supported. This can be used only if time restriction type is `time-of-day`.
-        :param Sequence['ScheduleRotationTimeRestrictionRestrictionListArgs'] restriction_list: It is a restriction object which is described below. This can be used only if time restriction type is `weekday-and-time-of-day`.
         """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restriction_list is not None:
             pulumi.set(__self__, "restriction_list", restriction_list)
 
@@ -3291,17 +3164,14 @@
         It is a restriction object which is described below. In this case startDay/endDay fields are not supported. This can be used only if time restriction type is `time-of-day`.
         """
         return pulumi.get(self, "restriction")
 
     @property
     @pulumi.getter(name="restrictionList")
     def restriction_list(self) -> Optional[Sequence['outputs.ScheduleRotationTimeRestrictionRestrictionList']]:
-        """
-        It is a restriction object which is described below. This can be used only if time restriction type is `weekday-and-time-of-day`.
-        """
         return pulumi.get(self, "restriction_list")
 
 
 @pulumi.output_type
 class ScheduleRotationTimeRestrictionRestriction(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3327,55 +3197,37 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  end_hour: int,
                  end_min: int,
                  start_hour: int,
                  start_min: int):
-        """
-        :param int end_hour: Value of the hour that frame will end.
-        :param int end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        :param int start_hour: Value of the hour that frame will start.
-        :param int start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> int:
-        """
-        Value of the hour that frame will end.
-        """
         return pulumi.get(self, "end_hour")
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> int:
-        """
-        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "end_min")
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> int:
-        """
-        Value of the hour that frame will start.
-        """
         return pulumi.get(self, "start_hour")
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> int:
-        """
-        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "start_min")
 
 
 @pulumi.output_type
 class ScheduleRotationTimeRestrictionRestrictionList(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3407,79 +3259,49 @@
     def __init__(__self__, *,
                  end_day: str,
                  end_hour: int,
                  end_min: int,
                  start_day: str,
                  start_hour: int,
                  start_min: int):
-        """
-        :param str end_day: Value of the day that frame will end.
-        :param int end_hour: Value of the hour that frame will end.
-        :param int end_min: Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-               
-               Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
-        :param str start_day: Value of the day that frame will start.
-        :param int start_hour: Value of the hour that frame will start
-        :param int start_min: Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         pulumi.set(__self__, "end_day", end_day)
         pulumi.set(__self__, "end_hour", end_hour)
         pulumi.set(__self__, "end_min", end_min)
         pulumi.set(__self__, "start_day", start_day)
         pulumi.set(__self__, "start_hour", start_hour)
         pulumi.set(__self__, "start_min", start_min)
 
     @property
     @pulumi.getter(name="endDay")
     def end_day(self) -> str:
-        """
-        Value of the day that frame will end.
-        """
         return pulumi.get(self, "end_day")
 
     @property
     @pulumi.getter(name="endHour")
     def end_hour(self) -> int:
-        """
-        Value of the hour that frame will end.
-        """
         return pulumi.get(self, "end_hour")
 
     @property
     @pulumi.getter(name="endMin")
     def end_min(self) -> int:
-        """
-        Value of the minute that frame will end. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-
-        Both `start_day` and `end_day` can assume only `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, or `sunday` values.
-        """
         return pulumi.get(self, "end_min")
 
     @property
     @pulumi.getter(name="startDay")
     def start_day(self) -> str:
-        """
-        Value of the day that frame will start.
-        """
         return pulumi.get(self, "start_day")
 
     @property
     @pulumi.getter(name="startHour")
     def start_hour(self) -> int:
-        """
-        Value of the hour that frame will start
-        """
         return pulumi.get(self, "start_hour")
 
     @property
     @pulumi.getter(name="startMin")
     def start_min(self) -> int:
-        """
-        Value of the minute that frame will start. Minutes may take 0 or 30 as value. Otherwise they will be converted to nearest 0 or 30 automatically.
-        """
         return pulumi.get(self, "start_min")
 
 
 @pulumi.output_type
 class ServiceIncidentRuleIncidentRule(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3966,29 +3788,23 @@
         TeamRoutingRuleTimeRestriction.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  type: str,
                  restriction: Optional[Sequence['outputs.TeamRoutingRuleTimeRestrictionRestriction']] = None,
                  restriction_list: Optional[Sequence['outputs.TeamRoutingRuleTimeRestrictionRestrictionList']] = None):
-        """
-        :param str type: Type of the operation will be applied on conditions. Should be one of `match-all`, `match-any-condition` or `match-all-conditions`.
-        """
         pulumi.set(__self__, "type", type)
         if restriction is not None:
             pulumi.set(__self__, "restriction", restriction)
         if restriction_list is not None:
             pulumi.set(__self__, "restriction_list", restriction_list)
 
     @property
     @pulumi.getter
     def type(self) -> str:
-        """
-        Type of the operation will be applied on conditions. Should be one of `match-all`, `match-any-condition` or `match-all-conditions`.
-        """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def restriction(self) -> Optional[Sequence['outputs.TeamRoutingRuleTimeRestrictionRestriction']]:
         return pulumi.get(self, "restriction")
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/provider.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/schedule_rotation.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/schedule_rotation.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,14 @@
                  type: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Schedule Rotation within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             schedule_id=test_opsgenie_schedule["id"],
             name="test",
@@ -314,15 +313,14 @@
                     start_hour=1,
                     start_min=1,
                     end_hour=10,
                     end_min=1,
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Schedule Rotations can be imported using the `schedule_id/rotation_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/scheduleRotation:ScheduleRotation * `opsgenie_schedule_rotation.test schedule_id/rotation_id`
@@ -345,15 +343,14 @@
                  args: ScheduleRotationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Schedule Rotation within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.ScheduleRotation("test",
             schedule_id=test_opsgenie_schedule["id"],
             name="test",
@@ -371,15 +368,14 @@
                     start_hour=1,
                     start_min=1,
                     end_hour=10,
                     end_min=1,
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Schedule Rotations can be imported using the `schedule_id/rotation_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/scheduleRotation:ScheduleRotation * `opsgenie_schedule_rotation.test schedule_id/rotation_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,27 +165,25 @@
                  team_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Service within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         payment = opsgenie.Team("payment",
             name="example",
             description="This team deals with all the things")
         this = opsgenie.Service("this",
             name="Payment",
             team_id="$opsgenie_team.payment.id")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `service_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/service:Service this service_id`
@@ -205,27 +203,25 @@
                  args: ServiceArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Service within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         payment = opsgenie.Team("payment",
             name="example",
             description="This team deals with all the things")
         this = opsgenie.Service("this",
             name="Payment",
             team_id="$opsgenie_team.payment.id")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `service_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/service:Service this service_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/service_incident_rule.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/service_incident_rule.py`

 * *Files 7% similar despite different names*

```diff
@@ -100,15 +100,14 @@
                  service_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Service Incident Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example-team",
             description="This team deals with all the things")
@@ -139,15 +138,14 @@
                     stakeholder_properties=[opsgenie.ServiceIncidentRuleIncidentRuleIncidentPropertyStakeholderPropertyArgs(
                         message="Message for stakeholders",
                         enable=True,
                     )],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Incident Rule can be imported using the `service_id/service_incident_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/serviceIncidentRule:ServiceIncidentRule this service_id/service_incident_rule_id`
@@ -165,15 +163,14 @@
                  args: ServiceIncidentRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Service Incident Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Team("test",
             name="example-team",
             description="This team deals with all the things")
@@ -204,15 +201,14 @@
                     stakeholder_properties=[opsgenie.ServiceIncidentRuleIncidentRuleIncidentPropertyStakeholderPropertyArgs(
                         message="Message for stakeholders",
                         enable=True,
                     )],
                 )],
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Service Incident Rule can be imported using the `service_id/service_incident_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/serviceIncidentRule:ServiceIncidentRule this service_id/service_incident_rule_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/team.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,15 +201,14 @@
                  name: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Team within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         first = opsgenie.User("first",
             username="user@domain.com",
             full_name="name ",
@@ -233,15 +232,14 @@
             ])
         self_service = opsgenie.Team("self-service",
             name="Self Service",
             description="Membership in this team is managed via OpsGenie web UI only",
             ignore_members=True,
             delete_default_resources=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `team_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/team:Team team1 team_id`
@@ -262,15 +260,14 @@
                  args: Optional[TeamArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Team within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         first = opsgenie.User("first",
             username="user@domain.com",
             full_name="name ",
@@ -294,15 +291,14 @@
             ])
         self_service = opsgenie.Team("self-service",
             name="Self Service",
             description="Membership in this team is managed via OpsGenie web UI only",
             ignore_members=True,
             delete_default_resources=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Teams can be imported using the `team_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/team:Team team1 team_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/team_routing_rule.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/team_routing_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,15 +298,14 @@
                  timezone: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a Team Routing Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Schedule("test",
             name="genieschedule",
             description="schedule test",
@@ -341,15 +340,14 @@
                 )],
             )],
             notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
                 name=test.name,
                 type="schedule",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Team Routing Rules can be imported using the `team_id/routing_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/teamRoutingRule:TeamRoutingRule ruletest team_id/routing_rule_id`
@@ -373,15 +371,14 @@
                  args: TeamRoutingRuleArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a Team Routing Rule within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.Schedule("test",
             name="genieschedule",
             description="schedule test",
@@ -416,15 +413,14 @@
                 )],
             )],
             notifies=[opsgenie.TeamRoutingRuleNotifyArgs(
                 name=test.name,
                 type="schedule",
             )])
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Team Routing Rules can be imported using the `team_id/routing_rule_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/teamRoutingRule:TeamRoutingRule ruletest team_id/routing_rule_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,15 +330,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a User within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
             username="user@domain.com",
             full_name="Test User",
@@ -358,15 +357,14 @@
                 zipcode="998877",
             )],
             user_details={
                 "key1": "val1,val2",
                 "key2": "val3,val4",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `user_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/user:User user user_id`
@@ -391,15 +389,14 @@
                  args: UserArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a User within Opsgenie.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         test = opsgenie.User("test",
             username="user@domain.com",
             full_name="Test User",
@@ -419,15 +416,14 @@
                 zipcode="998877",
             )],
             user_details={
                 "key1": "val1,val2",
                 "key2": "val3,val4",
             })
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `user_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/user:User user user_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie/user_contact.py` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie/user_contact.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,14 @@
                  username: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Manages a User Contact.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         sms = opsgenie.UserContact("sms",
             username=exampleuser["username"],
             to="39-123",
@@ -181,15 +180,14 @@
             to="fahri@opsgenie.com",
             method="email")
         voice = opsgenie.UserContact("voice",
             username=exampleuser["username"],
             to="39-123",
             method="voice")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `username/contact_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/userContact:UserContact testcontact username/contact_id`
@@ -209,15 +207,14 @@
                  args: UserContactArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a User Contact.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_opsgenie as opsgenie
 
         sms = opsgenie.UserContact("sms",
             username=exampleuser["username"],
             to="39-123",
@@ -227,15 +224,14 @@
             to="fahri@opsgenie.com",
             method="email")
         voice = opsgenie.UserContact("voice",
             username=exampleuser["username"],
             to="39-123",
             method="voice")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Users can be imported using the `username/contact_id`, e.g.
 
         ```sh
         $ pulumi import opsgenie:index/userContact:UserContact testcontact username/contact_id`
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/PKG-INFO` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_opsgenie
-Version: 1.4.0a1713561317
+Version: 1.4.0a1713903127
 Summary: A Pulumi package for creating and managing opsgenie cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-opsgenie
 Keywords: pulumi,opsgenie
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pulumi_opsgenie.egg-info/SOURCES.txt` & `pulumi_opsgenie-1.4.0a1713903127/pulumi_opsgenie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_opsgenie-1.4.0a1713561317/pyproject.toml` & `pulumi_opsgenie-1.4.0a1713903127/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_opsgenie"
   description = "A Pulumi package for creating and managing opsgenie cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "opsgenie"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "1.4.0a1713561317"
+  version = "1.4.0a1713903127"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-opsgenie"
 
 [build-system]
```

