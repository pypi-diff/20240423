# Comparing `tmp/pulumi_slack-0.4.5a1713673482.tar.gz` & `tmp/pulumi_slack-0.4.5a1713904890.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.5a1713673482.tar", last modified: Sun Apr 21 04:26:53 2024, max compression
+gzip compressed data, was "pulumi_slack-0.4.5a1713904890.tar", last modified: Tue Apr 23 20:47:37 2024, max compression
```

## Comparing `pulumi_slack-0.4.5a1713673482.tar` & `pulumi_slack-0.4.5a1713904890.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    39726 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10973 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4852 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6865 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-21 04:26:53.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-21 04:26:53.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 04:26:53.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-21 04:26:53.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-21 04:26:53.000000 pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-21 04:26:47.000000 pulumi_slack-0.4.5a1713673482/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 04:26:53.552577 pulumi_slack-0.4.5a1713673482/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39258 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    18172 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-23 20:47:37.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-23 20:47:37.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:47:37.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:47:37.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 20:47:37.000000 pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-23 20:47:31.000000 pulumi_slack-0.4.5a1713904890/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:47:37.600649 pulumi_slack-0.4.5a1713904890/setup.cfg
```

### Comparing `pulumi_slack-0.4.5a1713673482/PKG-INFO` & `pulumi_slack-0.4.5a1713904890/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1713673482
+Version: 0.4.5a1713904890
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1713673482/README.md` & `pulumi_slack-0.4.5a1713904890/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/__init__.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/conversation.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -493,54 +493,48 @@
         - [conversations.unarchive](https://api.slack.com/methods/conversations.unarchive)
 
         If you get `missing_scope` errors while using this resource check the scopes against
         the documentation for the methods above.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         test = slack.Conversation("test",
             name="my-channel",
             topic="The topic for my channel",
             permanent_members=[],
             is_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         nonadmin = slack.Conversation("nonadmin",
             name="my-channel01",
             topic="The channel won't be archived on destroy",
             permanent_members=[],
             is_private=True,
             action_on_destroy="none")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         adopted = slack.Conversation("adopted",
             name="my-channel02",
             topic="Adopt existing, don't kick members",
             permanent_members=[],
             adopt_existing_channel=True,
             action_on_update_permanent_members="none")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_conversation` can be imported using the ID of the conversation/channel, e.g.
 
         ```sh
         $ pulumi import slack:index/conversation:Conversation my_conversation C023X7QTFHQ
@@ -612,54 +606,48 @@
         - [conversations.unarchive](https://api.slack.com/methods/conversations.unarchive)
 
         If you get `missing_scope` errors while using this resource check the scopes against
         the documentation for the methods above.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         test = slack.Conversation("test",
             name="my-channel",
             topic="The topic for my channel",
             permanent_members=[],
             is_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         nonadmin = slack.Conversation("nonadmin",
             name="my-channel01",
             topic="The channel won't be archived on destroy",
             permanent_members=[],
             is_private=True,
             action_on_destroy="none")
         ```
-        <!--End PulumiCodeChooser -->
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         adopted = slack.Conversation("adopted",
             name="my-channel02",
             topic="Adopt existing, don't kick members",
             permanent_members=[],
             adopt_existing_channel=True,
             action_on_update_permanent_members="none")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_conversation` can be imported using the ID of the conversation/channel, e.g.
 
         ```sh
         $ pulumi import slack:index/conversation:Conversation my_conversation C023X7QTFHQ
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/get_conversation.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,23 +209,21 @@
     - [conversations.members](https://api.slack.com/methods/conversations.members)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     test = slack.get_conversation(channel_id="my-channel")
     test_name = slack.get_conversation(name="my-channel-name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str channel_id: The ID of the channel
     :param bool is_private: The conversation is privileged between two or more members
            
            Either `channel_id` or `name` must be provided. `is_private` only works in conjunction
            with `name`.
@@ -276,23 +274,21 @@
     - [conversations.members](https://api.slack.com/methods/conversations.members)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     test = slack.get_conversation(channel_id="my-channel")
     test_name = slack.get_conversation(name="my-channel-name")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str channel_id: The ID of the channel
     :param bool is_private: The conversation is privileged between two or more members
            
            Either `channel_id` or `name` must be provided. `is_private` only works in conjunction
            with `name`.
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/get_user.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/get_user.py`

 * *Files 13% similar despite different names*

```diff
@@ -82,23 +82,21 @@
     - [users.list](https://api.slack.com/methods/users.list)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     by_name = slack.get_user(name="my-user")
     by_email = slack.get_user(email="my-user@example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str email: The email of the user
            
            The data source expects exactly one of these fields, you can't set both.
     :param str name: The name of the user
     """
@@ -135,23 +133,21 @@
     - [users.list](https://api.slack.com/methods/users.list)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     by_name = slack.get_user(name="my-user")
     by_email = slack.get_user(email="my-user@example.com")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str email: The email of the user
            
            The data source expects exactly one of these fields, you can't set both.
     :param str name: The name of the user
     """
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/get_usergroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -129,23 +129,21 @@
     - [usergroups.list](https://api.slack.com/methods/usergroups.list)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     by_name = slack.get_usergroup(name="my-usergroup")
     by_id = slack.get_usergroup(usergroup_id="USERGROUP00")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the usergroup
     :param str usergroup_id: The id of the usergroup
            
            The data source expects exactly one of these fields, you can't set both.
     """
@@ -184,23 +182,21 @@
     - [usergroups.list](https://api.slack.com/methods/usergroups.list)
 
     If you get `missing_scope` errors while using this resource check the scopes against
     the documentation for the methods above.
 
     ## Example Usage
 
-    <!--Start PulumiCodeChooser -->
     ```python
     import pulumi
     import pulumi_slack as slack
 
     by_name = slack.get_usergroup(name="my-usergroup")
     by_id = slack.get_usergroup(usergroup_id="USERGROUP00")
     ```
-    <!--End PulumiCodeChooser -->
 
 
     :param str name: The name of the usergroup
     :param str usergroup_id: The id of the usergroup
            
            The data source expects exactly one of these fields, you can't set both.
     """
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/provider.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.5a1713904890/pulumi_slack/usergroup.py`

 * *Files 5% similar despite different names*

```diff
@@ -226,33 +226,30 @@
         - [usergroups.users.update](https://api.slack.com/methods/usergroups.users.update)
 
         If you get `missing_scope` errors while using this resource check the scopes against
         the documentation for the methods above.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         my_group = slack.Usergroup("my_group",
             name="TestGroup",
             handle="test",
             description="Test user group",
             users=["USER00"],
             channels=["CHANNEL00"])
         ```
-        <!--End PulumiCodeChooser -->
 
         Note that if a channel is removed from the `channels` list users are
         **not** removed from the channel. In order to keep the users in the
         groups and in the channel in sync set `permanent_users` in the channel:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         my_group = slack.Usergroup("my_group",
             name="TestGroup",
             handle="test",
@@ -260,15 +257,14 @@
             users=["USER00"])
         test = slack.Conversation("test",
             name="my-channel",
             topic="The topic for my channel",
             permanent_members=my_group.users,
             is_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_usergroup` can be imported using the ID of the group, e.g.
 
         ```sh
         $ pulumi import slack:index/usergroup:Usergroup my_group S022GE79E9G
@@ -310,33 +306,30 @@
         - [usergroups.users.update](https://api.slack.com/methods/usergroups.users.update)
 
         If you get `missing_scope` errors while using this resource check the scopes against
         the documentation for the methods above.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         my_group = slack.Usergroup("my_group",
             name="TestGroup",
             handle="test",
             description="Test user group",
             users=["USER00"],
             channels=["CHANNEL00"])
         ```
-        <!--End PulumiCodeChooser -->
 
         Note that if a channel is removed from the `channels` list users are
         **not** removed from the channel. In order to keep the users in the
         groups and in the channel in sync set `permanent_users` in the channel:
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_slack as slack
 
         my_group = slack.Usergroup("my_group",
             name="TestGroup",
             handle="test",
@@ -344,15 +337,14 @@
             users=["USER00"])
         test = slack.Conversation("test",
             name="my-channel",
             topic="The topic for my channel",
             permanent_members=my_group.users,
             is_private=True)
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         `slack_usergroup` can be imported using the ID of the group, e.g.
 
         ```sh
         $ pulumi import slack:index/usergroup:Usergroup my_group S022GE79E9G
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.5a1713673482
+Version: 0.4.5a1713904890
 Summary: A Pulumi package for managing Slack workspaces.
 License: Apache-2.0
 Project-URL: Homepage, https://www.pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi,slack,category/utility
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_slack-0.4.5a1713673482/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.5a1713904890/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.5a1713673482/pyproject.toml` & `pulumi_slack-0.4.5a1713904890/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_slack"
   description = "A Pulumi package for managing Slack workspaces."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "slack", "category/utility"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.4.5a1713673482"
+  version = "0.4.5a1713904890"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://www.pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-slack"
 
 [build-system]
```

