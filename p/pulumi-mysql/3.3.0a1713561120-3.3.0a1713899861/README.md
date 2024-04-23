# Comparing `tmp/pulumi_mysql-3.3.0a1713561120.tar.gz` & `tmp/pulumi_mysql-3.3.0a1713899861.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_mysql-3.3.0a1713561120.tar", last modified: Fri Apr 19 21:18:17 2024, max compression
+gzip compressed data, was "pulumi_mysql-3.3.0a1713899861.tar", last modified: Tue Apr 23 19:49:25 2024, max compression
```

## Comparing `pulumi_mysql-3.3.0a1713561120.tar` & `pulumi_mysql-3.3.0a1713899861.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    17626 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/grant.py
--rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    23843 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    13656 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user_password.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-19 21:18:17.000000 pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-19 21:18:11.000000 pulumi_mysql-3.3.0a1713561120/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:18:17.510834 pulumi_mysql-3.3.0a1713561120/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:49:25.198495 pulumi_mysql-3.3.0a1713899861/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-23 19:49:25.198495 pulumi_mysql-3.3.0a1713899861/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:49:25.194495 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:49:25.198495 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17470 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26844 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10003 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5721 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23531 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13494 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql/user_password.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:49:25.198495 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-23 19:49:25.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-23 19:49:25.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:49:25.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 19:49:25.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-23 19:49:25.000000 pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-23 19:49:19.000000 pulumi_mysql-3.3.0a1713899861/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 19:49:25.198495 pulumi_mysql-3.3.0a1713899861/setup.cfg
```

### Comparing `pulumi_mysql-3.3.0a1713561120/PKG-INFO` & `pulumi_mysql-3.3.0a1713899861/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1713561120
+Version: 3.3.0a1713899861
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1713561120/README.md` & `pulumi_mysql-3.3.0a1713899861/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/__init__.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/_utilities.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/__init__.pyi` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/config/vars.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/database.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,22 +190,20 @@
                  __props__=None):
         """
         The ``Database`` resource creates and manages a database on a MySQL
         server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         app = mysql.Database("app", name="my_awesome_app")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Databases can be imported using their name, e.g.
 
         ```sh
         $ pulumi import mysql:index/database:Database example my-example-database
@@ -239,22 +237,20 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The ``Database`` resource creates and manages a database on a MySQL
         server.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         app = mysql.Database("app", name="my_awesome_app")
         ```
-        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Databases can be imported using their name, e.g.
 
         ```sh
         $ pulumi import mysql:index/database:Database example my-example-database
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/grant.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,15 +333,14 @@
         The ``Grant`` resource creates and manages privileges given to
         a user on a MySQL server.
 
         ## Examples
 
         ### Granting Privileges to a User
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
@@ -351,37 +350,33 @@
             host=jdoe.host,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Granting Privileges to a Role
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         developer = mysql.Role("developer", name="developer")
         developer_grant = mysql.Grant("developer",
             role=developer.name,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Adding a Role to a User
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
@@ -389,15 +384,14 @@
         developer = mysql.Role("developer", name="developer")
         developer_grant = mysql.Grant("developer",
             user=jdoe.user,
             host=jdoe.host,
             database="app",
             roles=[developer.name])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] database: The database to grant privileges on.
         :param pulumi.Input[bool] grant: Whether to also give the user privileges to grant the same privileges to other users.
         :param pulumi.Input[str] host: The source host of the user. Defaults to "localhost". Conflicts with `role`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] privileges: A list of privileges to grant to the user. Refer to a list of privileges (such as [here](https://dev.mysql.com/doc/refman/5.5/en/grant.html)) for applicable privileges. Conflicts with `roles`.
@@ -417,15 +411,14 @@
         The ``Grant`` resource creates and manages privileges given to
         a user on a MySQL server.
 
         ## Examples
 
         ### Granting Privileges to a User
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
@@ -435,37 +428,33 @@
             host=jdoe.host,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Granting Privileges to a Role
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         developer = mysql.Role("developer", name="developer")
         developer_grant = mysql.Grant("developer",
             role=developer.name,
             database="app",
             privileges=[
                 "SELECT",
                 "UPDATE",
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Adding a Role to a User
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
@@ -473,15 +462,14 @@
         developer = mysql.Role("developer", name="developer")
         developer_grant = mysql.Grant("developer",
             user=jdoe.user,
             host=jdoe.host,
             database="app",
             roles=[developer.name])
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param GrantArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/provider.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/role.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/role.py`

 * *Files 11% similar despite different names*

```diff
@@ -70,22 +70,20 @@
         The ``Role`` resource creates and manages a user on a MySQL
         server.
 
         > **Note:** MySQL introduced roles in version 8. They do not work on MySQL 5 and lower.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         developer = mysql.Role("developer", name="developer")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: The name of the role.
         """
         ...
     @overload
@@ -97,22 +95,20 @@
         The ``Role`` resource creates and manages a user on a MySQL
         server.
 
         > **Note:** MySQL introduced roles in version 8. They do not work on MySQL 5 and lower.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         developer = mysql.Role("developer", name="developer")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param RoleArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -254,39 +254,35 @@
         The ``User`` resource creates and manages a user on a MySQL
         server.
 
         ## Examples
 
         ### Basic Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
             plaintext_password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage with an Authentication Plugin
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         nologin = mysql.User("nologin",
             user="nologin",
             host="example.com",
             auth_plugin="mysql_no_login")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] auth_plugin: Use an [authentication plugin][ref-auth-plugins] to authenticate the user instead of using password authentication.  Description of the fields allowed in the block below. Conflicts with `password` and `plaintext_password`.
         :param pulumi.Input[str] host: The source host of the user. Defaults to "localhost".
         :param pulumi.Input[str] password: Deprecated alias of `plaintext_password`, whose value is *stored as plaintext in state*. Prefer to use `plaintext_password` instead, which stores the password as an unsalted hash. Conflicts with `auth_plugin`.
         :param pulumi.Input[str] plaintext_password: The password for the user. This must be provided in plain text, so the data source for it must be secured. An _unsalted_ hash of the provided password is stored in state. Conflicts with `auth_plugin`.
@@ -305,39 +301,35 @@
         The ``User`` resource creates and manages a user on a MySQL
         server.
 
         ## Examples
 
         ### Basic Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe",
             user="jdoe",
             host="example.com",
             plaintext_password="password")
         ```
-        <!--End PulumiCodeChooser -->
 
         ### Example Usage with an Authentication Plugin
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         nologin = mysql.User("nologin",
             user="nologin",
             host="example.com",
             auth_plugin="mysql_no_login")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql/user_password.py` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql/user_password.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,25 +171,23 @@
            storing unencrypted passwords in the provider state.
 
         > **NOTE on How Passwords are Created:** This resource **automatically**
            generates a **random** password. The password will be a random UUID.
 
         ## Example Usage
 
-         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe", user="jdoe")
         jdoe_user_password = mysql.UserPassword("jdoe",
-            user=jdoe.user,
-            pgp_key="keybase:joestump")
+           user=jdoe.user,
+           pgp_key="keybase:joestump")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] host: The source host of the user. Defaults to `localhost`.
         :param pulumi.Input[str] pgp_key: Either a base-64 encoded PGP public key, or a keybase username in the form `keybase:some_person_that_exists`.
         :param pulumi.Input[str] user: The IAM user to associate with this access key.
         """
@@ -208,25 +206,23 @@
            storing unencrypted passwords in the provider state.
 
         > **NOTE on How Passwords are Created:** This resource **automatically**
            generates a **random** password. The password will be a random UUID.
 
         ## Example Usage
 
-         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_mysql as mysql
 
         jdoe = mysql.User("jdoe", user="jdoe")
         jdoe_user_password = mysql.UserPassword("jdoe",
-            user=jdoe.user,
-            pgp_key="keybase:joestump")
+           user=jdoe.user,
+           pgp_key="keybase:joestump")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param UserPasswordArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/PKG-INFO` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_mysql
-Version: 3.3.0a1713561120
+Version: 3.3.0a1713899861
 Summary: A Pulumi package for creating and managing mysql cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-mysql
 Keywords: pulumi,mysql
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_mysql-3.3.0a1713561120/pulumi_mysql.egg-info/SOURCES.txt` & `pulumi_mysql-3.3.0a1713899861/pulumi_mysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_mysql-3.3.0a1713561120/pyproject.toml` & `pulumi_mysql-3.3.0a1713899861/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_mysql"
   description = "A Pulumi package for creating and managing mysql cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0a1,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "mysql"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.3.0a1713561120"
+  version = "3.3.0a1713899861"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-mysql"
 
 [build-system]
```

