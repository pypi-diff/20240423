# Comparing `tmp/pulumi_rke-3.5.0a1713561359.tar.gz` & `tmp/pulumi_rke-3.5.0a1713905146.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_rke-3.5.0a1713561359.tar", last modified: Fri Apr 19 21:25:39 2024, max compression
+gzip compressed data, was "pulumi_rke-3.5.0a1713905146.tar", last modified: Tue Apr 23 20:55:09 2024, max compression
```

## Comparing `pulumi_rke-3.5.0a1713561359.tar` & `pulumi_rke-3.5.0a1713905146.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/pulumi_rke/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   398152 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)   139188 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/pulumi_rke/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)   359046 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-19 21:25:39.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-19 21:25:39.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:25:39.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:25:39.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-19 21:25:39.000000 pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-19 21:25:33.000000 pulumi_rke-3.5.0a1713561359/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:25:39.336151 pulumi_rke-3.5.0a1713561359/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/pulumi_rke/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   338457 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138960 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/pulumi_rke/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304657 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5178 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-04-23 20:55:09.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 20:55:09.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:55:09.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:55:09.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 20:55:09.000000 pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-23 20:55:02.000000 pulumi_rke-3.5.0a1713905146/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:55:09.887452 pulumi_rke-3.5.0a1713905146/setup.cfg
```

### Comparing `pulumi_rke-3.5.0a1713561359/PKG-INFO` & `pulumi_rke-3.5.0a1713905146/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.5.0a1713561359
+Version: 3.5.0a1713905146
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.5.0a1713561359/README.md` & `pulumi_rke-3.5.0a1713905146/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/__init__.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/_inputs.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/_inputs.py`

 * *Files 7% similar despite different names*

```diff
@@ -101,132 +101,128 @@
 @pulumi.input_type
 class ClusterAuthenticationArgs:
     def __init__(__self__, *,
                  sans: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  strategy: Optional[pulumi.Input[str]] = None,
                  webhook: Optional[pulumi.Input['ClusterAuthenticationWebhookArgs']] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of additional hostnames and IPs to include in the api server PKI cert (list)
-        :param pulumi.Input[str] strategy: Authentication strategy that will be used in RKE k8s cluster. Default: `x509` (string)
-        :param pulumi.Input['ClusterAuthenticationWebhookArgs'] webhook: Webhook configuration options (list maxitem: 1)
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] sans: List of additional hostnames and IPs to include in the api server PKI cert
+        :param pulumi.Input[str] strategy: Authentication strategy that will be used in RKE k8s cluster
+        :param pulumi.Input['ClusterAuthenticationWebhookArgs'] webhook: Webhook configuration options
         """
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
         if strategy is not None:
             pulumi.set(__self__, "strategy", strategy)
         if webhook is not None:
             pulumi.set(__self__, "webhook", webhook)
 
     @property
     @pulumi.getter
     def sans(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        List of additional hostnames and IPs to include in the api server PKI cert (list)
+        List of additional hostnames and IPs to include in the api server PKI cert
         """
         return pulumi.get(self, "sans")
 
     @sans.setter
     def sans(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "sans", value)
 
     @property
     @pulumi.getter
     def strategy(self) -> Optional[pulumi.Input[str]]:
         """
-        Authentication strategy that will be used in RKE k8s cluster. Default: `x509` (string)
+        Authentication strategy that will be used in RKE k8s cluster
         """
         return pulumi.get(self, "strategy")
 
     @strategy.setter
     def strategy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "strategy", value)
 
     @property
     @pulumi.getter
     def webhook(self) -> Optional[pulumi.Input['ClusterAuthenticationWebhookArgs']]:
         """
-        Webhook configuration options (list maxitem: 1)
+        Webhook configuration options
         """
         return pulumi.get(self, "webhook")
 
     @webhook.setter
     def webhook(self, value: Optional[pulumi.Input['ClusterAuthenticationWebhookArgs']]):
         pulumi.set(self, "webhook", value)
 
 
 @pulumi.input_type
 class ClusterAuthenticationWebhookArgs:
     def __init__(__self__, *,
                  cache_timeout: Optional[pulumi.Input[str]] = None,
                  config_file: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] cache_timeout: Controls how long to cache authentication decisions (string)
-        :param pulumi.Input[str] config_file: Multiline string that represent a custom webhook config file (string)
+        :param pulumi.Input[str] cache_timeout: Controls how long to cache authentication decisions
+        :param pulumi.Input[str] config_file: Multiline string that represent a custom webhook config file
         """
         if cache_timeout is not None:
             pulumi.set(__self__, "cache_timeout", cache_timeout)
         if config_file is not None:
             pulumi.set(__self__, "config_file", config_file)
 
     @property
     @pulumi.getter(name="cacheTimeout")
     def cache_timeout(self) -> Optional[pulumi.Input[str]]:
         """
-        Controls how long to cache authentication decisions (string)
+        Controls how long to cache authentication decisions
         """
         return pulumi.get(self, "cache_timeout")
 
     @cache_timeout.setter
     def cache_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cache_timeout", value)
 
     @property
     @pulumi.getter(name="configFile")
     def config_file(self) -> Optional[pulumi.Input[str]]:
         """
-        Multiline string that represent a custom webhook config file (string)
+        Multiline string that represent a custom webhook config file
         """
         return pulumi.get(self, "config_file")
 
     @config_file.setter
     def config_file(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "config_file", value)
 
 
 @pulumi.input_type
 class ClusterAuthorizationArgs:
     def __init__(__self__, *,
                  mode: Optional[pulumi.Input[str]] = None,
                  options: Optional[pulumi.Input[Mapping[str, Any]]] = None):
         """
-        :param pulumi.Input[str] mode: RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
-        :param pulumi.Input[Mapping[str, Any]] options: Network provider options (map)
+        :param pulumi.Input[Mapping[str, Any]] options: Authorization mode options
         """
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if options is not None:
             pulumi.set(__self__, "options", options)
 
     @property
     @pulumi.getter
     def mode(self) -> Optional[pulumi.Input[str]]:
-        """
-        RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
-        """
         return pulumi.get(self, "mode")
 
     @mode.setter
     def mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "mode", value)
 
     @property
     @pulumi.getter
     def options(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Network provider options (map)
+        Authorization mode options
         """
         return pulumi.get(self, "options")
 
     @options.setter
     def options(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "options", value)
 
@@ -240,22 +236,22 @@
                  port: Optional[pulumi.Input[str]] = None,
                  ssh_agent_auth: Optional[pulumi.Input[bool]] = None,
                  ssh_cert: Optional[pulumi.Input[str]] = None,
                  ssh_cert_path: Optional[pulumi.Input[str]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  ssh_key_path: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[bool] ignore_proxy_env_vars: Ignore proxy env vars at Bastion Host? Default: `false` (bool)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
+        :param pulumi.Input[str] address: Address of Bastion Host
+        :param pulumi.Input[str] user: SSH User to Bastion Host
+        :param pulumi.Input[bool] ignore_proxy_env_vars: Ignore proxy env vars at Bastion Host?
+        :param pulumi.Input[str] port: SSH Port of Bastion Host
         :param pulumi.Input[bool] ssh_agent_auth: SSH Agent Auth enable (bool)
-        :param pulumi.Input[str] ssh_cert: SSH Certificate (string)
+        :param pulumi.Input[str] ssh_cert: SSH Certificate Key
         :param pulumi.Input[str] ssh_cert_path: SSH Certificate Path (string)
-        :param pulumi.Input[str] ssh_key: SSH Private Key (string)
+        :param pulumi.Input[str] ssh_key: SSH Private Key
         :param pulumi.Input[str] ssh_key_path: SSH Private Key Path (string)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "user", user)
         if ignore_proxy_env_vars is not None:
             pulumi.set(__self__, "ignore_proxy_env_vars", ignore_proxy_env_vars)
         if port is not None:
@@ -271,51 +267,51 @@
         if ssh_key_path is not None:
             pulumi.set(__self__, "ssh_key_path", ssh_key_path)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Input[str]:
         """
-        Address ip for node (string)
+        Address of Bastion Host
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Input[str]:
         """
-        Registry user (string)
+        SSH User to Bastion Host
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="ignoreProxyEnvVars")
     def ignore_proxy_env_vars(self) -> Optional[pulumi.Input[bool]]:
         """
-        Ignore proxy env vars at Bastion Host? Default: `false` (bool)
+        Ignore proxy env vars at Bastion Host?
         """
         return pulumi.get(self, "ignore_proxy_env_vars")
 
     @ignore_proxy_env_vars.setter
     def ignore_proxy_env_vars(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_proxy_env_vars", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
         """
-        Port used for SSH communication (string)
+        SSH Port of Bastion Host
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
@@ -331,15 +327,15 @@
     def ssh_agent_auth(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssh_agent_auth", value)
 
     @property
     @pulumi.getter(name="sshCert")
     def ssh_cert(self) -> Optional[pulumi.Input[str]]:
         """
-        SSH Certificate (string)
+        SSH Certificate Key
         """
         return pulumi.get(self, "ssh_cert")
 
     @ssh_cert.setter
     def ssh_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_cert", value)
 
@@ -355,15 +351,15 @@
     def ssh_cert_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_cert_path", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        SSH Private Key (string)
+        SSH Private Key
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -394,17 +390,14 @@
                  key_env_name: Optional[pulumi.Input[str]] = None,
                  key_path: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  ou_name: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] id: (Computed) The ID of the resource (string)
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param pulumi.Input[str] path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         """
         if certificate is not None:
             pulumi.set(__self__, "certificate", certificate)
         if common_name is not None:
             pulumi.set(__self__, "common_name", common_name)
         if config is not None:
             pulumi.set(__self__, "config", config)
@@ -494,17 +487,14 @@
     @id.setter
     def id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "id", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
@@ -524,17 +514,14 @@
     @key_path.setter
     def key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key_path", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
@@ -545,17 +532,14 @@
     @ou_name.setter
     def ou_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ou_name", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
 
@@ -570,25 +554,19 @@
                  custom_cloud_config: Optional[pulumi.Input[str]] = None,
                  custom_cloud_provider: Optional[pulumi.Input[str]] = None,
                  openstack_cloud_config: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigArgs']] = None,
                  openstack_cloud_provider: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderArgs']] = None,
                  vsphere_cloud_config: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigArgs']] = None,
                  vsphere_cloud_provider: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderArgs']] = None):
         """
-        :param pulumi.Input[str] name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param pulumi.Input['ClusterCloudProviderAwsCloudConfigArgs'] aws_cloud_config: Use aws_cloud_provider instead
-        :param pulumi.Input['ClusterCloudProviderAwsCloudProviderArgs'] aws_cloud_provider: AWS Cloud Provider config [rke-aws-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/aws/) (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderAzureCloudConfigArgs'] azure_cloud_config: Use azure_cloud_provider instead
-        :param pulumi.Input['ClusterCloudProviderAzureCloudProviderArgs'] azure_cloud_provider: Azure Cloud Provider config [rke-azure-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/azure/) (list maxitems:1)
-        :param pulumi.Input[str] custom_cloud_config: Use custom_cloud_provider instead
-        :param pulumi.Input[str] custom_cloud_provider: Custom Cloud Provider config (string)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigArgs'] openstack_cloud_config: Use openstack_cloud_provider instead
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderArgs'] openstack_cloud_provider: Openstack Cloud Provider config [rke-openstack-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/openstack/) (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudConfigArgs'] vsphere_cloud_config: Use vsphere_cloud_provider instead
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderArgs'] vsphere_cloud_provider: Vsphere Cloud Provider config [rke-vsphere-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/vsphere/) Extra argument `name` is required on `virtual_center` configuration. (list maxitems:1)
+        :param pulumi.Input['ClusterCloudProviderAwsCloudProviderArgs'] aws_cloud_provider: AWS Cloud Provider config
+        :param pulumi.Input['ClusterCloudProviderAzureCloudProviderArgs'] azure_cloud_provider: Azure Cloud Provider config
+        :param pulumi.Input[str] custom_cloud_provider: Custom Cloud Provider config
+        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderArgs'] openstack_cloud_provider: Openstack Cloud Provider config
+        :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderArgs'] vsphere_cloud_provider: Vsphere Cloud Provider config
         """
         pulumi.set(__self__, "name", name)
         if aws_cloud_config is not None:
             warnings.warn("""Use aws_cloud_provider instead""", DeprecationWarning)
             pulumi.log.warn("""aws_cloud_config is deprecated: Use aws_cloud_provider instead""")
         if aws_cloud_config is not None:
             pulumi.set(__self__, "aws_cloud_config", aws_cloud_config)
@@ -622,191 +600,163 @@
             pulumi.set(__self__, "vsphere_cloud_config", vsphere_cloud_config)
         if vsphere_cloud_provider is not None:
             pulumi.set(__self__, "vsphere_cloud_provider", vsphere_cloud_provider)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter(name="awsCloudConfig")
     def aws_cloud_config(self) -> Optional[pulumi.Input['ClusterCloudProviderAwsCloudConfigArgs']]:
-        """
-        Use aws_cloud_provider instead
-        """
         warnings.warn("""Use aws_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""aws_cloud_config is deprecated: Use aws_cloud_provider instead""")
 
         return pulumi.get(self, "aws_cloud_config")
 
     @aws_cloud_config.setter
     def aws_cloud_config(self, value: Optional[pulumi.Input['ClusterCloudProviderAwsCloudConfigArgs']]):
         pulumi.set(self, "aws_cloud_config", value)
 
     @property
     @pulumi.getter(name="awsCloudProvider")
     def aws_cloud_provider(self) -> Optional[pulumi.Input['ClusterCloudProviderAwsCloudProviderArgs']]:
         """
-        AWS Cloud Provider config [rke-aws-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/aws/) (list maxitems:1)
+        AWS Cloud Provider config
         """
         return pulumi.get(self, "aws_cloud_provider")
 
     @aws_cloud_provider.setter
     def aws_cloud_provider(self, value: Optional[pulumi.Input['ClusterCloudProviderAwsCloudProviderArgs']]):
         pulumi.set(self, "aws_cloud_provider", value)
 
     @property
     @pulumi.getter(name="azureCloudConfig")
     def azure_cloud_config(self) -> Optional[pulumi.Input['ClusterCloudProviderAzureCloudConfigArgs']]:
-        """
-        Use azure_cloud_provider instead
-        """
         warnings.warn("""Use azure_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""azure_cloud_config is deprecated: Use azure_cloud_provider instead""")
 
         return pulumi.get(self, "azure_cloud_config")
 
     @azure_cloud_config.setter
     def azure_cloud_config(self, value: Optional[pulumi.Input['ClusterCloudProviderAzureCloudConfigArgs']]):
         pulumi.set(self, "azure_cloud_config", value)
 
     @property
     @pulumi.getter(name="azureCloudProvider")
     def azure_cloud_provider(self) -> Optional[pulumi.Input['ClusterCloudProviderAzureCloudProviderArgs']]:
         """
-        Azure Cloud Provider config [rke-azure-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/azure/) (list maxitems:1)
+        Azure Cloud Provider config
         """
         return pulumi.get(self, "azure_cloud_provider")
 
     @azure_cloud_provider.setter
     def azure_cloud_provider(self, value: Optional[pulumi.Input['ClusterCloudProviderAzureCloudProviderArgs']]):
         pulumi.set(self, "azure_cloud_provider", value)
 
     @property
     @pulumi.getter(name="customCloudConfig")
     def custom_cloud_config(self) -> Optional[pulumi.Input[str]]:
-        """
-        Use custom_cloud_provider instead
-        """
         warnings.warn("""Use custom_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""custom_cloud_config is deprecated: Use custom_cloud_provider instead""")
 
         return pulumi.get(self, "custom_cloud_config")
 
     @custom_cloud_config.setter
     def custom_cloud_config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_cloud_config", value)
 
     @property
     @pulumi.getter(name="customCloudProvider")
     def custom_cloud_provider(self) -> Optional[pulumi.Input[str]]:
         """
-        Custom Cloud Provider config (string)
+        Custom Cloud Provider config
         """
         return pulumi.get(self, "custom_cloud_provider")
 
     @custom_cloud_provider.setter
     def custom_cloud_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_cloud_provider", value)
 
     @property
     @pulumi.getter(name="openstackCloudConfig")
     def openstack_cloud_config(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigArgs']]:
-        """
-        Use openstack_cloud_provider instead
-        """
         warnings.warn("""Use openstack_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""openstack_cloud_config is deprecated: Use openstack_cloud_provider instead""")
 
         return pulumi.get(self, "openstack_cloud_config")
 
     @openstack_cloud_config.setter
     def openstack_cloud_config(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigArgs']]):
         pulumi.set(self, "openstack_cloud_config", value)
 
     @property
     @pulumi.getter(name="openstackCloudProvider")
     def openstack_cloud_provider(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderArgs']]:
         """
-        Openstack Cloud Provider config [rke-openstack-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/openstack/) (list maxitems:1)
+        Openstack Cloud Provider config
         """
         return pulumi.get(self, "openstack_cloud_provider")
 
     @openstack_cloud_provider.setter
     def openstack_cloud_provider(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderArgs']]):
         pulumi.set(self, "openstack_cloud_provider", value)
 
     @property
     @pulumi.getter(name="vsphereCloudConfig")
     def vsphere_cloud_config(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigArgs']]:
-        """
-        Use vsphere_cloud_provider instead
-        """
         warnings.warn("""Use vsphere_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""vsphere_cloud_config is deprecated: Use vsphere_cloud_provider instead""")
 
         return pulumi.get(self, "vsphere_cloud_config")
 
     @vsphere_cloud_config.setter
     def vsphere_cloud_config(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigArgs']]):
         pulumi.set(self, "vsphere_cloud_config", value)
 
     @property
     @pulumi.getter(name="vsphereCloudProvider")
     def vsphere_cloud_provider(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderArgs']]:
         """
-        Vsphere Cloud Provider config [rke-vsphere-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/vsphere/) Extra argument `name` is required on `virtual_center` configuration. (list maxitems:1)
+        Vsphere Cloud Provider config
         """
         return pulumi.get(self, "vsphere_cloud_provider")
 
     @vsphere_cloud_provider.setter
     def vsphere_cloud_provider(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderArgs']]):
         pulumi.set(self, "vsphere_cloud_provider", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderAwsCloudConfigArgs:
     def __init__(__self__, *,
                  global_: Optional[pulumi.Input['ClusterCloudProviderAwsCloudConfigGlobalArgs']] = None,
                  service_overrides: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudConfigServiceOverrideArgs']]]] = None):
-        """
-        :param pulumi.Input['ClusterCloudProviderAwsCloudConfigGlobalArgs'] global_: (list maxitems:1)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudConfigServiceOverrideArgs']]] service_overrides: (list)
-        """
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if service_overrides is not None:
             pulumi.set(__self__, "service_overrides", service_overrides)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional[pulumi.Input['ClusterCloudProviderAwsCloudConfigGlobalArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: Optional[pulumi.Input['ClusterCloudProviderAwsCloudConfigGlobalArgs']]):
         pulumi.set(self, "global_", value)
 
     @property
     @pulumi.getter(name="serviceOverrides")
     def service_overrides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudConfigServiceOverrideArgs']]]]:
-        """
-        (list)
-        """
         return pulumi.get(self, "service_overrides")
 
     @service_overrides.setter
     def service_overrides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudConfigServiceOverrideArgs']]]]):
         pulumi.set(self, "service_overrides", value)
 
 
@@ -820,24 +770,24 @@
                  kubernetes_cluster_tag: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  route_table_id: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  vpc: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] disable_security_group_ingress: Disables the automatic ingress creation. Default `false` (bool)
-        :param pulumi.Input[bool] disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
-        :param pulumi.Input[str] elb_security_group: Use these ELB security groups instead create new (string)
-        :param pulumi.Input[str] kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources (string)
-        :param pulumi.Input[str] kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources (string)
-        :param pulumi.Input[str] role_arn: IAM role to assume when interaction with AWS APIs (string)
-        :param pulumi.Input[str] route_table_id: Enables using a specific RouteTable (string)
-        :param pulumi.Input[str] subnet_id: (string)
-        :param pulumi.Input[str] vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
-        :param pulumi.Input[str] zone: The AWS zone (string)
+        :param pulumi.Input[bool] disable_security_group_ingress: Disables the automatic ingress creation
+        :param pulumi.Input[bool] disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped
+        :param pulumi.Input[str] elb_security_group: Use these ELB security groups instead create new
+        :param pulumi.Input[str] kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources
+        :param pulumi.Input[str] kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources
+        :param pulumi.Input[str] role_arn: IAM role to assume when interaction with AWS APIs
+        :param pulumi.Input[str] route_table_id: Enables using a specific RouteTable
+        :param pulumi.Input[str] subnet_id: Enables using a specific subnet to use for ELB's
+        :param pulumi.Input[str] vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
+        :param pulumi.Input[str] zone: The AWS zone
         """
         if disable_security_group_ingress is not None:
             pulumi.set(__self__, "disable_security_group_ingress", disable_security_group_ingress)
         if disable_strict_zone_check is not None:
             pulumi.set(__self__, "disable_strict_zone_check", disable_strict_zone_check)
         if elb_security_group is not None:
             pulumi.set(__self__, "elb_security_group", elb_security_group)
@@ -856,123 +806,123 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="disableSecurityGroupIngress")
     def disable_security_group_ingress(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disables the automatic ingress creation. Default `false` (bool)
+        Disables the automatic ingress creation
         """
         return pulumi.get(self, "disable_security_group_ingress")
 
     @disable_security_group_ingress.setter
     def disable_security_group_ingress(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_security_group_ingress", value)
 
     @property
     @pulumi.getter(name="disableStrictZoneCheck")
     def disable_strict_zone_check(self) -> Optional[pulumi.Input[bool]]:
         """
-        Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
+        Setting this to true will disable the check and provide a warning that the check was skipped
         """
         return pulumi.get(self, "disable_strict_zone_check")
 
     @disable_strict_zone_check.setter
     def disable_strict_zone_check(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_strict_zone_check", value)
 
     @property
     @pulumi.getter(name="elbSecurityGroup")
     def elb_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        Use these ELB security groups instead create new (string)
+        Use these ELB security groups instead create new
         """
         return pulumi.get(self, "elb_security_group")
 
     @elb_security_group.setter
     def elb_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elb_security_group", value)
 
     @property
     @pulumi.getter(name="kubernetesClusterId")
     def kubernetes_cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The cluster id we'll use to identify our cluster resources (string)
+        The cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_id")
 
     @kubernetes_cluster_id.setter
     def kubernetes_cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_cluster_id", value)
 
     @property
     @pulumi.getter(name="kubernetesClusterTag")
     def kubernetes_cluster_tag(self) -> Optional[pulumi.Input[str]]:
         """
-        Legacy cluster id we'll use to identify our cluster resources (string)
+        Legacy cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_tag")
 
     @kubernetes_cluster_tag.setter
     def kubernetes_cluster_tag(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_cluster_tag", value)
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         """
-        IAM role to assume when interaction with AWS APIs (string)
+        IAM role to assume when interaction with AWS APIs
         """
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
     @property
     @pulumi.getter(name="routeTableId")
     def route_table_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Enables using a specific RouteTable (string)
+        Enables using a specific RouteTable
         """
         return pulumi.get(self, "route_table_id")
 
     @route_table_id.setter
     def route_table_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "route_table_id", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        Enables using a specific subnet to use for ELB's
         """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
     @property
     @pulumi.getter
     def vpc(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
+        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
         """
         return pulumi.get(self, "vpc")
 
     @vpc.setter
     def vpc(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vpc", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS zone (string)
+        The AWS zone
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -983,23 +933,14 @@
                  service: pulumi.Input[str],
                  key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  signing_method: Optional[pulumi.Input[str]] = None,
                  signing_name: Optional[pulumi.Input[str]] = None,
                  signing_region: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] service: (string)
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] signing_method: (string)
-        :param pulumi.Input[str] signing_name: (string)
-        :param pulumi.Input[str] signing_region: (string)
-        :param pulumi.Input[str] url: Registry URL (string)
-        """
         pulumi.set(__self__, "service", service)
         if key is not None:
             warnings.warn("""Use service instead""", DeprecationWarning)
             pulumi.log.warn("""key is deprecated: Use service instead""")
         if key is not None:
             pulumi.set(__self__, "key", key)
         if region is not None:
@@ -1012,131 +953,100 @@
             pulumi.set(__self__, "signing_region", signing_region)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def service(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "service")
 
     @service.setter
     def service(self, value: pulumi.Input[str]):
         pulumi.set(self, "service", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS key for etcd service (string)
-        """
         warnings.warn("""Use service instead""", DeprecationWarning)
         pulumi.log.warn("""key is deprecated: Use service instead""")
 
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="signingMethod")
     def signing_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_method")
 
     @signing_method.setter
     def signing_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_method", value)
 
     @property
     @pulumi.getter(name="signingName")
     def signing_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_name")
 
     @signing_name.setter
     def signing_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_name", value)
 
     @property
     @pulumi.getter(name="signingRegion")
     def signing_region(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_region")
 
     @signing_region.setter
     def signing_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_region", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry URL (string)
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderAwsCloudProviderArgs:
     def __init__(__self__, *,
                  global_: Optional[pulumi.Input['ClusterCloudProviderAwsCloudProviderGlobalArgs']] = None,
                  service_overrides: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudProviderServiceOverrideArgs']]]] = None):
-        """
-        :param pulumi.Input['ClusterCloudProviderAwsCloudProviderGlobalArgs'] global_: (list maxitems:1)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudProviderServiceOverrideArgs']]] service_overrides: (list)
-        """
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if service_overrides is not None:
             pulumi.set(__self__, "service_overrides", service_overrides)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional[pulumi.Input['ClusterCloudProviderAwsCloudProviderGlobalArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: Optional[pulumi.Input['ClusterCloudProviderAwsCloudProviderGlobalArgs']]):
         pulumi.set(self, "global_", value)
 
     @property
     @pulumi.getter(name="serviceOverrides")
     def service_overrides(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudProviderServiceOverrideArgs']]]]:
-        """
-        (list)
-        """
         return pulumi.get(self, "service_overrides")
 
     @service_overrides.setter
     def service_overrides(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderAwsCloudProviderServiceOverrideArgs']]]]):
         pulumi.set(self, "service_overrides", value)
 
 
@@ -1150,24 +1060,24 @@
                  kubernetes_cluster_tag: Optional[pulumi.Input[str]] = None,
                  role_arn: Optional[pulumi.Input[str]] = None,
                  route_table_id: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  vpc: Optional[pulumi.Input[str]] = None,
                  zone: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] disable_security_group_ingress: Disables the automatic ingress creation. Default `false` (bool)
-        :param pulumi.Input[bool] disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
-        :param pulumi.Input[str] elb_security_group: Use these ELB security groups instead create new (string)
-        :param pulumi.Input[str] kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources (string)
-        :param pulumi.Input[str] kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources (string)
-        :param pulumi.Input[str] role_arn: IAM role to assume when interaction with AWS APIs (string)
-        :param pulumi.Input[str] route_table_id: Enables using a specific RouteTable (string)
-        :param pulumi.Input[str] subnet_id: (string)
-        :param pulumi.Input[str] vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
-        :param pulumi.Input[str] zone: The AWS zone (string)
+        :param pulumi.Input[bool] disable_security_group_ingress: Disables the automatic ingress creation
+        :param pulumi.Input[bool] disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped
+        :param pulumi.Input[str] elb_security_group: Use these ELB security groups instead create new
+        :param pulumi.Input[str] kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources
+        :param pulumi.Input[str] kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources
+        :param pulumi.Input[str] role_arn: IAM role to assume when interaction with AWS APIs
+        :param pulumi.Input[str] route_table_id: Enables using a specific RouteTable
+        :param pulumi.Input[str] subnet_id: Enables using a specific subnet to use for ELB's
+        :param pulumi.Input[str] vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
+        :param pulumi.Input[str] zone: The AWS zone
         """
         if disable_security_group_ingress is not None:
             pulumi.set(__self__, "disable_security_group_ingress", disable_security_group_ingress)
         if disable_strict_zone_check is not None:
             pulumi.set(__self__, "disable_strict_zone_check", disable_strict_zone_check)
         if elb_security_group is not None:
             pulumi.set(__self__, "elb_security_group", elb_security_group)
@@ -1186,123 +1096,123 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="disableSecurityGroupIngress")
     def disable_security_group_ingress(self) -> Optional[pulumi.Input[bool]]:
         """
-        Disables the automatic ingress creation. Default `false` (bool)
+        Disables the automatic ingress creation
         """
         return pulumi.get(self, "disable_security_group_ingress")
 
     @disable_security_group_ingress.setter
     def disable_security_group_ingress(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_security_group_ingress", value)
 
     @property
     @pulumi.getter(name="disableStrictZoneCheck")
     def disable_strict_zone_check(self) -> Optional[pulumi.Input[bool]]:
         """
-        Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
+        Setting this to true will disable the check and provide a warning that the check was skipped
         """
         return pulumi.get(self, "disable_strict_zone_check")
 
     @disable_strict_zone_check.setter
     def disable_strict_zone_check(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "disable_strict_zone_check", value)
 
     @property
     @pulumi.getter(name="elbSecurityGroup")
     def elb_security_group(self) -> Optional[pulumi.Input[str]]:
         """
-        Use these ELB security groups instead create new (string)
+        Use these ELB security groups instead create new
         """
         return pulumi.get(self, "elb_security_group")
 
     @elb_security_group.setter
     def elb_security_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "elb_security_group", value)
 
     @property
     @pulumi.getter(name="kubernetesClusterId")
     def kubernetes_cluster_id(self) -> Optional[pulumi.Input[str]]:
         """
-        The cluster id we'll use to identify our cluster resources (string)
+        The cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_id")
 
     @kubernetes_cluster_id.setter
     def kubernetes_cluster_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_cluster_id", value)
 
     @property
     @pulumi.getter(name="kubernetesClusterTag")
     def kubernetes_cluster_tag(self) -> Optional[pulumi.Input[str]]:
         """
-        Legacy cluster id we'll use to identify our cluster resources (string)
+        Legacy cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_tag")
 
     @kubernetes_cluster_tag.setter
     def kubernetes_cluster_tag(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_cluster_tag", value)
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[pulumi.Input[str]]:
         """
-        IAM role to assume when interaction with AWS APIs (string)
+        IAM role to assume when interaction with AWS APIs
         """
         return pulumi.get(self, "role_arn")
 
     @role_arn.setter
     def role_arn(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "role_arn", value)
 
     @property
     @pulumi.getter(name="routeTableId")
     def route_table_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Enables using a specific RouteTable (string)
+        Enables using a specific RouteTable
         """
         return pulumi.get(self, "route_table_id")
 
     @route_table_id.setter
     def route_table_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "route_table_id", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        Enables using a specific subnet to use for ELB's
         """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
     @property
     @pulumi.getter
     def vpc(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
+        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
         """
         return pulumi.get(self, "vpc")
 
     @vpc.setter
     def vpc(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vpc", value)
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[pulumi.Input[str]]:
         """
-        The AWS zone (string)
+        The AWS zone
         """
         return pulumi.get(self, "zone")
 
     @zone.setter
     def zone(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "zone", value)
 
@@ -1313,23 +1223,14 @@
                  service: pulumi.Input[str],
                  key: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  signing_method: Optional[pulumi.Input[str]] = None,
                  signing_name: Optional[pulumi.Input[str]] = None,
                  signing_region: Optional[pulumi.Input[str]] = None,
                  url: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] service: (string)
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] signing_method: (string)
-        :param pulumi.Input[str] signing_name: (string)
-        :param pulumi.Input[str] signing_region: (string)
-        :param pulumi.Input[str] url: Registry URL (string)
-        """
         pulumi.set(__self__, "service", service)
         if key is not None:
             warnings.warn("""Use service instead""", DeprecationWarning)
             pulumi.log.warn("""key is deprecated: Use service instead""")
         if key is not None:
             pulumi.set(__self__, "key", key)
         if region is not None:
@@ -1342,92 +1243,71 @@
             pulumi.set(__self__, "signing_region", signing_region)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def service(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "service")
 
     @service.setter
     def service(self, value: pulumi.Input[str]):
         pulumi.set(self, "service", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS key for etcd service (string)
-        """
         warnings.warn("""Use service instead""", DeprecationWarning)
         pulumi.log.warn("""key is deprecated: Use service instead""")
 
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="signingMethod")
     def signing_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_method")
 
     @signing_method.setter
     def signing_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_method", value)
 
     @property
     @pulumi.getter(name="signingName")
     def signing_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_name")
 
     @signing_name.setter
     def signing_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_name", value)
 
     @property
     @pulumi.getter(name="signingRegion")
     def signing_region(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_region")
 
     @signing_region.setter
     def signing_region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "signing_region", value)
 
     @property
     @pulumi.getter
     def url(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry URL (string)
-        """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "url", value)
 
 
@@ -1460,43 +1340,42 @@
                  subnet_name: Optional[pulumi.Input[str]] = None,
                  use_instance_metadata: Optional[pulumi.Input[bool]] = None,
                  use_managed_identity_extension: Optional[pulumi.Input[bool]] = None,
                  vm_type: Optional[pulumi.Input[str]] = None,
                  vnet_name: Optional[pulumi.Input[str]] = None,
                  vnet_resource_group: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] aad_client_id: (string)
-        :param pulumi.Input[str] aad_client_secret: (string)
-        :param pulumi.Input[str] subscription_id: (string)
-        :param pulumi.Input[str] tenant_id: Required if `tenant_name` not provided. (string)
-        :param pulumi.Input[str] aad_client_cert_password: (string)
-        :param pulumi.Input[str] aad_client_cert_path: (string)
-        :param pulumi.Input[str] cloud: (string)
-        :param pulumi.Input[bool] cloud_provider_backoff: (bool)
-        :param pulumi.Input[int] cloud_provider_backoff_duration: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_exponent: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_jitter: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_retries: (int)
-        :param pulumi.Input[bool] cloud_provider_rate_limit: (bool)
-        :param pulumi.Input[int] cloud_provider_rate_limit_bucket: (int)
-        :param pulumi.Input[int] cloud_provider_rate_limit_qps: (int)
+        :param pulumi.Input[str] aad_client_id: The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] aad_client_secret: The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] subscription_id: The ID of the Azure Subscription that the cluster is deployed in
+        :param pulumi.Input[str] tenant_id: The AAD Tenant ID for the Subscription that the cluster is deployed in
+        :param pulumi.Input[str] aad_client_cert_password: The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] aad_client_cert_path: The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] cloud: The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
+        :param pulumi.Input[bool] cloud_provider_backoff: Enable exponential backoff to manage resource request retries
+        :param pulumi.Input[int] cloud_provider_backoff_duration: Backoff duration
+        :param pulumi.Input[int] cloud_provider_backoff_exponent: Backoff exponent
+        :param pulumi.Input[int] cloud_provider_backoff_jitter: Backoff jitter
+        :param pulumi.Input[int] cloud_provider_backoff_retries: Backoff retry limit
+        :param pulumi.Input[bool] cloud_provider_rate_limit: Enable rate limiting
+        :param pulumi.Input[int] cloud_provider_rate_limit_qps: Rate limit QPS
         :param pulumi.Input[str] load_balancer_sku: Load balancer type (basic | standard). Must be standard for auto-scaling
-        :param pulumi.Input[str] location: (string)
-        :param pulumi.Input[int] maximum_load_balancer_rule_count: (int)
-        :param pulumi.Input[str] primary_availability_set_name: (string)
-        :param pulumi.Input[str] primary_scale_set_name: (string)
-        :param pulumi.Input[str] resource_group: (string)
-        :param pulumi.Input[str] route_table_name: (string)
-        :param pulumi.Input[str] security_group_name: (string)
-        :param pulumi.Input[str] subnet_name: (string)
-        :param pulumi.Input[bool] use_instance_metadata: (bool)
-        :param pulumi.Input[bool] use_managed_identity_extension: (bool)
-        :param pulumi.Input[str] vm_type: (string)
-        :param pulumi.Input[str] vnet_name: (string)
-        :param pulumi.Input[str] vnet_resource_group: (string)
+        :param pulumi.Input[str] location: The location of the resource group that the cluster is deployed in
+        :param pulumi.Input[int] maximum_load_balancer_rule_count: Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
+        :param pulumi.Input[str] primary_availability_set_name: The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
+        :param pulumi.Input[str] primary_scale_set_name: The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
+        :param pulumi.Input[str] resource_group: The name of the resource group that the cluster is deployed in
+        :param pulumi.Input[str] route_table_name: (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
+        :param pulumi.Input[str] security_group_name: The name of the security group attached to the cluster's subnet
+        :param pulumi.Input[str] subnet_name: The name of the Subnet that the cluster is deployed in
+        :param pulumi.Input[bool] use_instance_metadata: Use instance metadata service where possible
+        :param pulumi.Input[bool] use_managed_identity_extension: Use managed service identity for the virtual machine to access Azure ARM APIs
+        :param pulumi.Input[str] vm_type: The type of azure nodes. If not set, it will be default to standard.
+        :param pulumi.Input[str] vnet_name: The name of the VNet that the cluster is deployed in
+        :param pulumi.Input[str] vnet_resource_group: The name of the resource group that the Vnet is deployed in
         """
         pulumi.set(__self__, "aad_client_id", aad_client_id)
         pulumi.set(__self__, "aad_client_secret", aad_client_secret)
         pulumi.set(__self__, "subscription_id", subscription_id)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if aad_client_cert_password is not None:
             pulumi.set(__self__, "aad_client_cert_password", aad_client_cert_password)
@@ -1549,183 +1428,180 @@
         if vnet_resource_group is not None:
             pulumi.set(__self__, "vnet_resource_group", vnet_resource_group)
 
     @property
     @pulumi.getter(name="aadClientId")
     def aad_client_id(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_id")
 
     @aad_client_id.setter
     def aad_client_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "aad_client_id", value)
 
     @property
     @pulumi.getter(name="aadClientSecret")
     def aad_client_secret(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_secret")
 
     @aad_client_secret.setter
     def aad_client_secret(self, value: pulumi.Input[str]):
         pulumi.set(self, "aad_client_secret", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ID of the Azure Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
     def subscription_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> pulumi.Input[str]:
         """
-        Required if `tenant_name` not provided. (string)
+        The AAD Tenant ID for the Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter(name="aadClientCertPassword")
     def aad_client_cert_password(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_password")
 
     @aad_client_cert_password.setter
     def aad_client_cert_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aad_client_cert_password", value)
 
     @property
     @pulumi.getter(name="aadClientCertPath")
     def aad_client_cert_path(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_path")
 
     @aad_client_cert_path.setter
     def aad_client_cert_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aad_client_cert_path", value)
 
     @property
     @pulumi.getter
     def cloud(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
         """
         return pulumi.get(self, "cloud")
 
     @cloud.setter
     def cloud(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoff")
     def cloud_provider_backoff(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Enable exponential backoff to manage resource request retries
         """
         return pulumi.get(self, "cloud_provider_backoff")
 
     @cloud_provider_backoff.setter
     def cloud_provider_backoff(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "cloud_provider_backoff", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffDuration")
     def cloud_provider_backoff_duration(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff duration
         """
         return pulumi.get(self, "cloud_provider_backoff_duration")
 
     @cloud_provider_backoff_duration.setter
     def cloud_provider_backoff_duration(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_duration", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffExponent")
     def cloud_provider_backoff_exponent(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff exponent
         """
         return pulumi.get(self, "cloud_provider_backoff_exponent")
 
     @cloud_provider_backoff_exponent.setter
     def cloud_provider_backoff_exponent(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_exponent", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffJitter")
     def cloud_provider_backoff_jitter(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff jitter
         """
         return pulumi.get(self, "cloud_provider_backoff_jitter")
 
     @cloud_provider_backoff_jitter.setter
     def cloud_provider_backoff_jitter(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_jitter", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffRetries")
     def cloud_provider_backoff_retries(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff retry limit
         """
         return pulumi.get(self, "cloud_provider_backoff_retries")
 
     @cloud_provider_backoff_retries.setter
     def cloud_provider_backoff_retries(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_retries", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimit")
     def cloud_provider_rate_limit(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Enable rate limiting
         """
         return pulumi.get(self, "cloud_provider_rate_limit")
 
     @cloud_provider_rate_limit.setter
     def cloud_provider_rate_limit(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "cloud_provider_rate_limit", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitBucket")
     def cloud_provider_rate_limit_bucket(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "cloud_provider_rate_limit_bucket")
 
     @cloud_provider_rate_limit_bucket.setter
     def cloud_provider_rate_limit_bucket(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_rate_limit_bucket", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitQps")
     def cloud_provider_rate_limit_qps(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Rate limit QPS
         """
         return pulumi.get(self, "cloud_provider_rate_limit_qps")
 
     @cloud_provider_rate_limit_qps.setter
     def cloud_provider_rate_limit_qps(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_rate_limit_qps", value)
 
@@ -1741,159 +1617,159 @@
     def load_balancer_sku(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "load_balancer_sku", value)
 
     @property
     @pulumi.getter
     def location(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The location of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "location")
 
     @location.setter
     def location(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "location", value)
 
     @property
     @pulumi.getter(name="maximumLoadBalancerRuleCount")
     def maximum_load_balancer_rule_count(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
         """
         return pulumi.get(self, "maximum_load_balancer_rule_count")
 
     @maximum_load_balancer_rule_count.setter
     def maximum_load_balancer_rule_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "maximum_load_balancer_rule_count", value)
 
     @property
     @pulumi.getter(name="primaryAvailabilitySetName")
     def primary_availability_set_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_availability_set_name")
 
     @primary_availability_set_name.setter
     def primary_availability_set_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_availability_set_name", value)
 
     @property
     @pulumi.getter(name="primaryScaleSetName")
     def primary_scale_set_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_scale_set_name")
 
     @primary_scale_set_name.setter
     def primary_scale_set_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_scale_set_name", value)
 
     @property
     @pulumi.getter(name="resourceGroup")
     def resource_group(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "resource_group")
 
     @resource_group.setter
     def resource_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "resource_group", value)
 
     @property
     @pulumi.getter(name="routeTableName")
     def route_table_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
         """
         return pulumi.get(self, "route_table_name")
 
     @route_table_name.setter
     def route_table_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "route_table_name", value)
 
     @property
     @pulumi.getter(name="securityGroupName")
     def security_group_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the security group attached to the cluster's subnet
         """
         return pulumi.get(self, "security_group_name")
 
     @security_group_name.setter
     def security_group_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_name", value)
 
     @property
     @pulumi.getter(name="subnetName")
     def subnet_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the Subnet that the cluster is deployed in
         """
         return pulumi.get(self, "subnet_name")
 
     @subnet_name.setter
     def subnet_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_name", value)
 
     @property
     @pulumi.getter(name="useInstanceMetadata")
     def use_instance_metadata(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Use instance metadata service where possible
         """
         return pulumi.get(self, "use_instance_metadata")
 
     @use_instance_metadata.setter
     def use_instance_metadata(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_instance_metadata", value)
 
     @property
     @pulumi.getter(name="useManagedIdentityExtension")
     def use_managed_identity_extension(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Use managed service identity for the virtual machine to access Azure ARM APIs
         """
         return pulumi.get(self, "use_managed_identity_extension")
 
     @use_managed_identity_extension.setter
     def use_managed_identity_extension(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_managed_identity_extension", value)
 
     @property
     @pulumi.getter(name="vmType")
     def vm_type(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The type of azure nodes. If not set, it will be default to standard.
         """
         return pulumi.get(self, "vm_type")
 
     @vm_type.setter
     def vm_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_type", value)
 
     @property
     @pulumi.getter(name="vnetName")
     def vnet_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the VNet that the cluster is deployed in
         """
         return pulumi.get(self, "vnet_name")
 
     @vnet_name.setter
     def vnet_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vnet_name", value)
 
     @property
     @pulumi.getter(name="vnetResourceGroup")
     def vnet_resource_group(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the resource group that the Vnet is deployed in
         """
         return pulumi.get(self, "vnet_resource_group")
 
     @vnet_resource_group.setter
     def vnet_resource_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vnet_resource_group", value)
 
@@ -1927,43 +1803,42 @@
                  subnet_name: Optional[pulumi.Input[str]] = None,
                  use_instance_metadata: Optional[pulumi.Input[bool]] = None,
                  use_managed_identity_extension: Optional[pulumi.Input[bool]] = None,
                  vm_type: Optional[pulumi.Input[str]] = None,
                  vnet_name: Optional[pulumi.Input[str]] = None,
                  vnet_resource_group: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] aad_client_id: (string)
-        :param pulumi.Input[str] aad_client_secret: (string)
-        :param pulumi.Input[str] subscription_id: (string)
-        :param pulumi.Input[str] tenant_id: Required if `tenant_name` not provided. (string)
-        :param pulumi.Input[str] aad_client_cert_password: (string)
-        :param pulumi.Input[str] aad_client_cert_path: (string)
-        :param pulumi.Input[str] cloud: (string)
-        :param pulumi.Input[bool] cloud_provider_backoff: (bool)
-        :param pulumi.Input[int] cloud_provider_backoff_duration: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_exponent: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_jitter: (int)
-        :param pulumi.Input[int] cloud_provider_backoff_retries: (int)
-        :param pulumi.Input[bool] cloud_provider_rate_limit: (bool)
-        :param pulumi.Input[int] cloud_provider_rate_limit_bucket: (int)
-        :param pulumi.Input[int] cloud_provider_rate_limit_qps: (int)
+        :param pulumi.Input[str] aad_client_id: The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] aad_client_secret: The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] subscription_id: The ID of the Azure Subscription that the cluster is deployed in
+        :param pulumi.Input[str] tenant_id: The AAD Tenant ID for the Subscription that the cluster is deployed in
+        :param pulumi.Input[str] aad_client_cert_password: The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] aad_client_cert_path: The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param pulumi.Input[str] cloud: The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
+        :param pulumi.Input[bool] cloud_provider_backoff: Enable exponential backoff to manage resource request retries
+        :param pulumi.Input[int] cloud_provider_backoff_duration: Backoff duration
+        :param pulumi.Input[int] cloud_provider_backoff_exponent: Backoff exponent
+        :param pulumi.Input[int] cloud_provider_backoff_jitter: Backoff jitter
+        :param pulumi.Input[int] cloud_provider_backoff_retries: Backoff retry limit
+        :param pulumi.Input[bool] cloud_provider_rate_limit: Enable rate limiting
+        :param pulumi.Input[int] cloud_provider_rate_limit_qps: Rate limit QPS
         :param pulumi.Input[str] load_balancer_sku: Load balancer type (basic | standard). Must be standard for auto-scaling
-        :param pulumi.Input[str] location: (string)
-        :param pulumi.Input[int] maximum_load_balancer_rule_count: (int)
-        :param pulumi.Input[str] primary_availability_set_name: (string)
-        :param pulumi.Input[str] primary_scale_set_name: (string)
-        :param pulumi.Input[str] resource_group: (string)
-        :param pulumi.Input[str] route_table_name: (string)
-        :param pulumi.Input[str] security_group_name: (string)
-        :param pulumi.Input[str] subnet_name: (string)
-        :param pulumi.Input[bool] use_instance_metadata: (bool)
-        :param pulumi.Input[bool] use_managed_identity_extension: (bool)
-        :param pulumi.Input[str] vm_type: (string)
-        :param pulumi.Input[str] vnet_name: (string)
-        :param pulumi.Input[str] vnet_resource_group: (string)
+        :param pulumi.Input[str] location: The location of the resource group that the cluster is deployed in
+        :param pulumi.Input[int] maximum_load_balancer_rule_count: Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
+        :param pulumi.Input[str] primary_availability_set_name: The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
+        :param pulumi.Input[str] primary_scale_set_name: The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
+        :param pulumi.Input[str] resource_group: The name of the resource group that the cluster is deployed in
+        :param pulumi.Input[str] route_table_name: (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
+        :param pulumi.Input[str] security_group_name: The name of the security group attached to the cluster's subnet
+        :param pulumi.Input[str] subnet_name: The name of the Subnet that the cluster is deployed in
+        :param pulumi.Input[bool] use_instance_metadata: Use instance metadata service where possible
+        :param pulumi.Input[bool] use_managed_identity_extension: Use managed service identity for the virtual machine to access Azure ARM APIs
+        :param pulumi.Input[str] vm_type: The type of azure nodes. If not set, it will be default to standard.
+        :param pulumi.Input[str] vnet_name: The name of the VNet that the cluster is deployed in
+        :param pulumi.Input[str] vnet_resource_group: The name of the resource group that the Vnet is deployed in
         """
         pulumi.set(__self__, "aad_client_id", aad_client_id)
         pulumi.set(__self__, "aad_client_secret", aad_client_secret)
         pulumi.set(__self__, "subscription_id", subscription_id)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if aad_client_cert_password is not None:
             pulumi.set(__self__, "aad_client_cert_password", aad_client_cert_password)
@@ -2016,183 +1891,180 @@
         if vnet_resource_group is not None:
             pulumi.set(__self__, "vnet_resource_group", vnet_resource_group)
 
     @property
     @pulumi.getter(name="aadClientId")
     def aad_client_id(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_id")
 
     @aad_client_id.setter
     def aad_client_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "aad_client_id", value)
 
     @property
     @pulumi.getter(name="aadClientSecret")
     def aad_client_secret(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_secret")
 
     @aad_client_secret.setter
     def aad_client_secret(self, value: pulumi.Input[str]):
         pulumi.set(self, "aad_client_secret", value)
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> pulumi.Input[str]:
         """
-        (string)
+        The ID of the Azure Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "subscription_id")
 
     @subscription_id.setter
     def subscription_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "subscription_id", value)
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> pulumi.Input[str]:
         """
-        Required if `tenant_name` not provided. (string)
+        The AAD Tenant ID for the Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter(name="aadClientCertPassword")
     def aad_client_cert_password(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_password")
 
     @aad_client_cert_password.setter
     def aad_client_cert_password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aad_client_cert_password", value)
 
     @property
     @pulumi.getter(name="aadClientCertPath")
     def aad_client_cert_path(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_path")
 
     @aad_client_cert_path.setter
     def aad_client_cert_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aad_client_cert_path", value)
 
     @property
     @pulumi.getter
     def cloud(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
         """
         return pulumi.get(self, "cloud")
 
     @cloud.setter
     def cloud(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cloud", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoff")
     def cloud_provider_backoff(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Enable exponential backoff to manage resource request retries
         """
         return pulumi.get(self, "cloud_provider_backoff")
 
     @cloud_provider_backoff.setter
     def cloud_provider_backoff(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "cloud_provider_backoff", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffDuration")
     def cloud_provider_backoff_duration(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff duration
         """
         return pulumi.get(self, "cloud_provider_backoff_duration")
 
     @cloud_provider_backoff_duration.setter
     def cloud_provider_backoff_duration(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_duration", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffExponent")
     def cloud_provider_backoff_exponent(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff exponent
         """
         return pulumi.get(self, "cloud_provider_backoff_exponent")
 
     @cloud_provider_backoff_exponent.setter
     def cloud_provider_backoff_exponent(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_exponent", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffJitter")
     def cloud_provider_backoff_jitter(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff jitter
         """
         return pulumi.get(self, "cloud_provider_backoff_jitter")
 
     @cloud_provider_backoff_jitter.setter
     def cloud_provider_backoff_jitter(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_jitter", value)
 
     @property
     @pulumi.getter(name="cloudProviderBackoffRetries")
     def cloud_provider_backoff_retries(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Backoff retry limit
         """
         return pulumi.get(self, "cloud_provider_backoff_retries")
 
     @cloud_provider_backoff_retries.setter
     def cloud_provider_backoff_retries(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_backoff_retries", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimit")
     def cloud_provider_rate_limit(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Enable rate limiting
         """
         return pulumi.get(self, "cloud_provider_rate_limit")
 
     @cloud_provider_rate_limit.setter
     def cloud_provider_rate_limit(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "cloud_provider_rate_limit", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitBucket")
     def cloud_provider_rate_limit_bucket(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "cloud_provider_rate_limit_bucket")
 
     @cloud_provider_rate_limit_bucket.setter
     def cloud_provider_rate_limit_bucket(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_rate_limit_bucket", value)
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitQps")
     def cloud_provider_rate_limit_qps(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Rate limit QPS
         """
         return pulumi.get(self, "cloud_provider_rate_limit_qps")
 
     @cloud_provider_rate_limit_qps.setter
     def cloud_provider_rate_limit_qps(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "cloud_provider_rate_limit_qps", value)
 
@@ -2208,159 +2080,159 @@
     def load_balancer_sku(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "load_balancer_sku", value)
 
     @property
     @pulumi.getter
     def location(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The location of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "location")
 
     @location.setter
     def location(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "location", value)
 
     @property
     @pulumi.getter(name="maximumLoadBalancerRuleCount")
     def maximum_load_balancer_rule_count(self) -> Optional[pulumi.Input[int]]:
         """
-        (int)
+        Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
         """
         return pulumi.get(self, "maximum_load_balancer_rule_count")
 
     @maximum_load_balancer_rule_count.setter
     def maximum_load_balancer_rule_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "maximum_load_balancer_rule_count", value)
 
     @property
     @pulumi.getter(name="primaryAvailabilitySetName")
     def primary_availability_set_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_availability_set_name")
 
     @primary_availability_set_name.setter
     def primary_availability_set_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_availability_set_name", value)
 
     @property
     @pulumi.getter(name="primaryScaleSetName")
     def primary_scale_set_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_scale_set_name")
 
     @primary_scale_set_name.setter
     def primary_scale_set_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "primary_scale_set_name", value)
 
     @property
     @pulumi.getter(name="resourceGroup")
     def resource_group(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "resource_group")
 
     @resource_group.setter
     def resource_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "resource_group", value)
 
     @property
     @pulumi.getter(name="routeTableName")
     def route_table_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
         """
         return pulumi.get(self, "route_table_name")
 
     @route_table_name.setter
     def route_table_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "route_table_name", value)
 
     @property
     @pulumi.getter(name="securityGroupName")
     def security_group_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the security group attached to the cluster's subnet
         """
         return pulumi.get(self, "security_group_name")
 
     @security_group_name.setter
     def security_group_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "security_group_name", value)
 
     @property
     @pulumi.getter(name="subnetName")
     def subnet_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the Subnet that the cluster is deployed in
         """
         return pulumi.get(self, "subnet_name")
 
     @subnet_name.setter
     def subnet_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_name", value)
 
     @property
     @pulumi.getter(name="useInstanceMetadata")
     def use_instance_metadata(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Use instance metadata service where possible
         """
         return pulumi.get(self, "use_instance_metadata")
 
     @use_instance_metadata.setter
     def use_instance_metadata(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_instance_metadata", value)
 
     @property
     @pulumi.getter(name="useManagedIdentityExtension")
     def use_managed_identity_extension(self) -> Optional[pulumi.Input[bool]]:
         """
-        (bool)
+        Use managed service identity for the virtual machine to access Azure ARM APIs
         """
         return pulumi.get(self, "use_managed_identity_extension")
 
     @use_managed_identity_extension.setter
     def use_managed_identity_extension(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_managed_identity_extension", value)
 
     @property
     @pulumi.getter(name="vmType")
     def vm_type(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The type of azure nodes. If not set, it will be default to standard.
         """
         return pulumi.get(self, "vm_type")
 
     @vm_type.setter
     def vm_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_type", value)
 
     @property
     @pulumi.getter(name="vnetName")
     def vnet_name(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the VNet that the cluster is deployed in
         """
         return pulumi.get(self, "vnet_name")
 
     @vnet_name.setter
     def vnet_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vnet_name", value)
 
     @property
     @pulumi.getter(name="vnetResourceGroup")
     def vnet_resource_group(self) -> Optional[pulumi.Input[str]]:
         """
-        (string)
+        The name of the resource group that the Vnet is deployed in
         """
         return pulumi.get(self, "vnet_resource_group")
 
     @vnet_resource_group.setter
     def vnet_resource_group(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vnet_resource_group", value)
 
@@ -2369,140 +2241,104 @@
 class ClusterCloudProviderOpenstackCloudConfigArgs:
     def __init__(__self__, *,
                  global_: pulumi.Input['ClusterCloudProviderOpenstackCloudConfigGlobalArgs'],
                  block_storage: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs']] = None,
                  load_balancer: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigLoadBalancerArgs']] = None,
                  metadata: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigMetadataArgs']] = None,
                  route: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigRouteArgs']] = None):
-        """
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigGlobalArgs'] global_: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs'] block_storage: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigLoadBalancerArgs'] load_balancer: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigMetadataArgs'] metadata: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudConfigRouteArgs'] route: (list maxitems:1)
-        """
         pulumi.set(__self__, "global_", global_)
         if block_storage is not None:
             pulumi.set(__self__, "block_storage", block_storage)
         if load_balancer is not None:
             pulumi.set(__self__, "load_balancer", load_balancer)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if route is not None:
             pulumi.set(__self__, "route", route)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> pulumi.Input['ClusterCloudProviderOpenstackCloudConfigGlobalArgs']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: pulumi.Input['ClusterCloudProviderOpenstackCloudConfigGlobalArgs']):
         pulumi.set(self, "global_", value)
 
     @property
     @pulumi.getter(name="blockStorage")
     def block_storage(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "block_storage")
 
     @block_storage.setter
     def block_storage(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs']]):
         pulumi.set(self, "block_storage", value)
 
     @property
     @pulumi.getter(name="loadBalancer")
     def load_balancer(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigLoadBalancerArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "load_balancer")
 
     @load_balancer.setter
     def load_balancer(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigLoadBalancerArgs']]):
         pulumi.set(self, "load_balancer", value)
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigMetadataArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "metadata")
 
     @metadata.setter
     def metadata(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigMetadataArgs']]):
         pulumi.set(self, "metadata", value)
 
     @property
     @pulumi.getter
     def route(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigRouteArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "route")
 
     @route.setter
     def route(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudConfigRouteArgs']]):
         pulumi.set(self, "route", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs:
     def __init__(__self__, *,
                  bs_version: Optional[pulumi.Input[str]] = None,
                  ignore_volume_az: Optional[pulumi.Input[bool]] = None,
                  trust_device_path: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] bs_version: (string)
-        :param pulumi.Input[bool] ignore_volume_az: (string)
-        :param pulumi.Input[bool] trust_device_path: (string)
-        """
         if bs_version is not None:
             pulumi.set(__self__, "bs_version", bs_version)
         if ignore_volume_az is not None:
             pulumi.set(__self__, "ignore_volume_az", ignore_volume_az)
         if trust_device_path is not None:
             pulumi.set(__self__, "trust_device_path", trust_device_path)
 
     @property
     @pulumi.getter(name="bsVersion")
     def bs_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "bs_version")
 
     @bs_version.setter
     def bs_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bs_version", value)
 
     @property
     @pulumi.getter(name="ignoreVolumeAz")
     def ignore_volume_az(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ignore_volume_az")
 
     @ignore_volume_az.setter
     def ignore_volume_az(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_volume_az", value)
 
     @property
     @pulumi.getter(name="trustDevicePath")
     def trust_device_path(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_device_path")
 
     @trust_device_path.setter
     def trust_device_path(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "trust_device_path", value)
 
 
@@ -2516,27 +2352,14 @@
                  domain_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  trust_id: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] auth_url: (string)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] ca_file: (string)
-        :param pulumi.Input[str] domain_id: Required if `domain_name` not provided. (string)
-        :param pulumi.Input[str] domain_name: Required if `domain_id` not provided. (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] tenant_id: Required if `tenant_name` not provided. (string)
-        :param pulumi.Input[str] tenant_name: Required if `tenant_id` not provided. (string)
-        :param pulumi.Input[str] trust_id: (string)
-        :param pulumi.Input[str] user_id: Required if `username` not provided. (string)
-        :param pulumi.Input[str] username: Required if `user_id` not provided. (string)
-        """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "password", password)
         if ca_file is not None:
             pulumi.set(__self__, "ca_file", ca_file)
         if domain_id is not None:
             pulumi.set(__self__, "domain_id", domain_id)
         if domain_name is not None:
@@ -2553,137 +2376,104 @@
             pulumi.set(__self__, "user_id", user_id)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authUrl")
     def auth_url(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "auth_url")
 
     @auth_url.setter
     def auth_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "auth_url", value)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="caFile")
     def ca_file(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ca_file")
 
     @ca_file.setter
     def ca_file(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_file", value)
 
     @property
     @pulumi.getter(name="domainId")
     def domain_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `domain_name` not provided. (string)
-        """
         return pulumi.get(self, "domain_id")
 
     @domain_id.setter
     def domain_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_id", value)
 
     @property
     @pulumi.getter(name="domainName")
     def domain_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `domain_id` not provided. (string)
-        """
         return pulumi.get(self, "domain_name")
 
     @domain_name.setter
     def domain_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_name", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `tenant_name` not provided. (string)
-        """
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `tenant_id` not provided. (string)
-        """
         return pulumi.get(self, "tenant_name")
 
     @tenant_name.setter
     def tenant_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_name", value)
 
     @property
     @pulumi.getter(name="trustId")
     def trust_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_id")
 
     @trust_id.setter
     def trust_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "trust_id", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `username` not provided. (string)
-        """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_id", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `user_id` not provided. (string)
-        """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
@@ -2697,27 +2487,14 @@
                  lb_version: Optional[pulumi.Input[str]] = None,
                  manage_security_groups: Optional[pulumi.Input[bool]] = None,
                  monitor_delay: Optional[pulumi.Input[str]] = None,
                  monitor_max_retries: Optional[pulumi.Input[int]] = None,
                  monitor_timeout: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  use_octavia: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[bool] create_monitor: (bool)
-        :param pulumi.Input[str] floating_network_id: (string)
-        :param pulumi.Input[str] lb_method: (string)
-        :param pulumi.Input[str] lb_provider: (string)
-        :param pulumi.Input[str] lb_version: (string)
-        :param pulumi.Input[bool] manage_security_groups: (bool)
-        :param pulumi.Input[str] monitor_delay: (string)
-        :param pulumi.Input[int] monitor_max_retries: (int)
-        :param pulumi.Input[str] monitor_timeout: (string)
-        :param pulumi.Input[str] subnet_id: (string)
-        :param pulumi.Input[bool] use_octavia: (bool)
-        """
         if create_monitor is not None:
             pulumi.set(__self__, "create_monitor", create_monitor)
         if floating_network_id is not None:
             pulumi.set(__self__, "floating_network_id", floating_network_id)
         if lb_method is not None:
             pulumi.set(__self__, "lb_method", lb_method)
         if lb_provider is not None:
@@ -2736,199 +2513,150 @@
             pulumi.set(__self__, "subnet_id", subnet_id)
         if use_octavia is not None:
             pulumi.set(__self__, "use_octavia", use_octavia)
 
     @property
     @pulumi.getter(name="createMonitor")
     def create_monitor(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "create_monitor")
 
     @create_monitor.setter
     def create_monitor(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_monitor", value)
 
     @property
     @pulumi.getter(name="floatingNetworkId")
     def floating_network_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "floating_network_id")
 
     @floating_network_id.setter
     def floating_network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "floating_network_id", value)
 
     @property
     @pulumi.getter(name="lbMethod")
     def lb_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_method")
 
     @lb_method.setter
     def lb_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_method", value)
 
     @property
     @pulumi.getter(name="lbProvider")
     def lb_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_provider")
 
     @lb_provider.setter
     def lb_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_provider", value)
 
     @property
     @pulumi.getter(name="lbVersion")
     def lb_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_version")
 
     @lb_version.setter
     def lb_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_version", value)
 
     @property
     @pulumi.getter(name="manageSecurityGroups")
     def manage_security_groups(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "manage_security_groups")
 
     @manage_security_groups.setter
     def manage_security_groups(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "manage_security_groups", value)
 
     @property
     @pulumi.getter(name="monitorDelay")
     def monitor_delay(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_delay")
 
     @monitor_delay.setter
     def monitor_delay(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "monitor_delay", value)
 
     @property
     @pulumi.getter(name="monitorMaxRetries")
     def monitor_max_retries(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "monitor_max_retries")
 
     @monitor_max_retries.setter
     def monitor_max_retries(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "monitor_max_retries", value)
 
     @property
     @pulumi.getter(name="monitorTimeout")
     def monitor_timeout(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_timeout")
 
     @monitor_timeout.setter
     def monitor_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "monitor_timeout", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
     @property
     @pulumi.getter(name="useOctavia")
     def use_octavia(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "use_octavia")
 
     @use_octavia.setter
     def use_octavia(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_octavia", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudConfigMetadataArgs:
     def __init__(__self__, *,
                  request_timeout: Optional[pulumi.Input[int]] = None,
                  search_order: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[int] request_timeout: (int)
-        :param pulumi.Input[str] search_order: (string)
-        """
         if request_timeout is not None:
             pulumi.set(__self__, "request_timeout", request_timeout)
         if search_order is not None:
             pulumi.set(__self__, "search_order", search_order)
 
     @property
     @pulumi.getter(name="requestTimeout")
     def request_timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "request_timeout")
 
     @request_timeout.setter
     def request_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "request_timeout", value)
 
     @property
     @pulumi.getter(name="searchOrder")
     def search_order(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "search_order")
 
     @search_order.setter
     def search_order(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "search_order", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudConfigRouteArgs:
     def __init__(__self__, *,
                  router_id: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] router_id: (string)
-        """
         if router_id is not None:
             pulumi.set(__self__, "router_id", router_id)
 
     @property
     @pulumi.getter(name="routerId")
     def router_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "router_id")
 
     @router_id.setter
     def router_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "router_id", value)
 
 
@@ -2936,140 +2664,104 @@
 class ClusterCloudProviderOpenstackCloudProviderArgs:
     def __init__(__self__, *,
                  global_: pulumi.Input['ClusterCloudProviderOpenstackCloudProviderGlobalArgs'],
                  block_storage: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs']] = None,
                  load_balancer: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderLoadBalancerArgs']] = None,
                  metadata: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderMetadataArgs']] = None,
                  route: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderRouteArgs']] = None):
-        """
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderGlobalArgs'] global_: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs'] block_storage: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderLoadBalancerArgs'] load_balancer: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderMetadataArgs'] metadata: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderOpenstackCloudProviderRouteArgs'] route: (list maxitems:1)
-        """
         pulumi.set(__self__, "global_", global_)
         if block_storage is not None:
             pulumi.set(__self__, "block_storage", block_storage)
         if load_balancer is not None:
             pulumi.set(__self__, "load_balancer", load_balancer)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if route is not None:
             pulumi.set(__self__, "route", route)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> pulumi.Input['ClusterCloudProviderOpenstackCloudProviderGlobalArgs']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: pulumi.Input['ClusterCloudProviderOpenstackCloudProviderGlobalArgs']):
         pulumi.set(self, "global_", value)
 
     @property
     @pulumi.getter(name="blockStorage")
     def block_storage(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "block_storage")
 
     @block_storage.setter
     def block_storage(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs']]):
         pulumi.set(self, "block_storage", value)
 
     @property
     @pulumi.getter(name="loadBalancer")
     def load_balancer(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderLoadBalancerArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "load_balancer")
 
     @load_balancer.setter
     def load_balancer(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderLoadBalancerArgs']]):
         pulumi.set(self, "load_balancer", value)
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderMetadataArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "metadata")
 
     @metadata.setter
     def metadata(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderMetadataArgs']]):
         pulumi.set(self, "metadata", value)
 
     @property
     @pulumi.getter
     def route(self) -> Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderRouteArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "route")
 
     @route.setter
     def route(self, value: Optional[pulumi.Input['ClusterCloudProviderOpenstackCloudProviderRouteArgs']]):
         pulumi.set(self, "route", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs:
     def __init__(__self__, *,
                  bs_version: Optional[pulumi.Input[str]] = None,
                  ignore_volume_az: Optional[pulumi.Input[bool]] = None,
                  trust_device_path: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] bs_version: (string)
-        :param pulumi.Input[bool] ignore_volume_az: (string)
-        :param pulumi.Input[bool] trust_device_path: (string)
-        """
         if bs_version is not None:
             pulumi.set(__self__, "bs_version", bs_version)
         if ignore_volume_az is not None:
             pulumi.set(__self__, "ignore_volume_az", ignore_volume_az)
         if trust_device_path is not None:
             pulumi.set(__self__, "trust_device_path", trust_device_path)
 
     @property
     @pulumi.getter(name="bsVersion")
     def bs_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "bs_version")
 
     @bs_version.setter
     def bs_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bs_version", value)
 
     @property
     @pulumi.getter(name="ignoreVolumeAz")
     def ignore_volume_az(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ignore_volume_az")
 
     @ignore_volume_az.setter
     def ignore_volume_az(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_volume_az", value)
 
     @property
     @pulumi.getter(name="trustDevicePath")
     def trust_device_path(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_device_path")
 
     @trust_device_path.setter
     def trust_device_path(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "trust_device_path", value)
 
 
@@ -3083,27 +2775,14 @@
                  domain_name: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  tenant_id: Optional[pulumi.Input[str]] = None,
                  tenant_name: Optional[pulumi.Input[str]] = None,
                  trust_id: Optional[pulumi.Input[str]] = None,
                  user_id: Optional[pulumi.Input[str]] = None,
                  username: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] auth_url: (string)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] ca_file: (string)
-        :param pulumi.Input[str] domain_id: Required if `domain_name` not provided. (string)
-        :param pulumi.Input[str] domain_name: Required if `domain_id` not provided. (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] tenant_id: Required if `tenant_name` not provided. (string)
-        :param pulumi.Input[str] tenant_name: Required if `tenant_id` not provided. (string)
-        :param pulumi.Input[str] trust_id: (string)
-        :param pulumi.Input[str] user_id: Required if `username` not provided. (string)
-        :param pulumi.Input[str] username: Required if `user_id` not provided. (string)
-        """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "password", password)
         if ca_file is not None:
             pulumi.set(__self__, "ca_file", ca_file)
         if domain_id is not None:
             pulumi.set(__self__, "domain_id", domain_id)
         if domain_name is not None:
@@ -3120,137 +2799,104 @@
             pulumi.set(__self__, "user_id", user_id)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authUrl")
     def auth_url(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "auth_url")
 
     @auth_url.setter
     def auth_url(self, value: pulumi.Input[str]):
         pulumi.set(self, "auth_url", value)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter(name="caFile")
     def ca_file(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ca_file")
 
     @ca_file.setter
     def ca_file(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_file", value)
 
     @property
     @pulumi.getter(name="domainId")
     def domain_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `domain_name` not provided. (string)
-        """
         return pulumi.get(self, "domain_id")
 
     @domain_id.setter
     def domain_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_id", value)
 
     @property
     @pulumi.getter(name="domainName")
     def domain_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `domain_id` not provided. (string)
-        """
         return pulumi.get(self, "domain_name")
 
     @domain_name.setter
     def domain_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "domain_name", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `tenant_name` not provided. (string)
-        """
         return pulumi.get(self, "tenant_id")
 
     @tenant_id.setter
     def tenant_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_id", value)
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `tenant_id` not provided. (string)
-        """
         return pulumi.get(self, "tenant_name")
 
     @tenant_name.setter
     def tenant_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tenant_name", value)
 
     @property
     @pulumi.getter(name="trustId")
     def trust_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_id")
 
     @trust_id.setter
     def trust_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "trust_id", value)
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `username` not provided. (string)
-        """
         return pulumi.get(self, "user_id")
 
     @user_id.setter
     def user_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user_id", value)
 
     @property
     @pulumi.getter
     def username(self) -> Optional[pulumi.Input[str]]:
-        """
-        Required if `user_id` not provided. (string)
-        """
         return pulumi.get(self, "username")
 
     @username.setter
     def username(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "username", value)
 
 
@@ -3264,27 +2910,14 @@
                  lb_version: Optional[pulumi.Input[str]] = None,
                  manage_security_groups: Optional[pulumi.Input[bool]] = None,
                  monitor_delay: Optional[pulumi.Input[str]] = None,
                  monitor_max_retries: Optional[pulumi.Input[int]] = None,
                  monitor_timeout: Optional[pulumi.Input[str]] = None,
                  subnet_id: Optional[pulumi.Input[str]] = None,
                  use_octavia: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[bool] create_monitor: (bool)
-        :param pulumi.Input[str] floating_network_id: (string)
-        :param pulumi.Input[str] lb_method: (string)
-        :param pulumi.Input[str] lb_provider: (string)
-        :param pulumi.Input[str] lb_version: (string)
-        :param pulumi.Input[bool] manage_security_groups: (bool)
-        :param pulumi.Input[str] monitor_delay: (string)
-        :param pulumi.Input[int] monitor_max_retries: (int)
-        :param pulumi.Input[str] monitor_timeout: (string)
-        :param pulumi.Input[str] subnet_id: (string)
-        :param pulumi.Input[bool] use_octavia: (bool)
-        """
         if create_monitor is not None:
             pulumi.set(__self__, "create_monitor", create_monitor)
         if floating_network_id is not None:
             pulumi.set(__self__, "floating_network_id", floating_network_id)
         if lb_method is not None:
             pulumi.set(__self__, "lb_method", lb_method)
         if lb_provider is not None:
@@ -3303,199 +2936,150 @@
             pulumi.set(__self__, "subnet_id", subnet_id)
         if use_octavia is not None:
             pulumi.set(__self__, "use_octavia", use_octavia)
 
     @property
     @pulumi.getter(name="createMonitor")
     def create_monitor(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "create_monitor")
 
     @create_monitor.setter
     def create_monitor(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "create_monitor", value)
 
     @property
     @pulumi.getter(name="floatingNetworkId")
     def floating_network_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "floating_network_id")
 
     @floating_network_id.setter
     def floating_network_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "floating_network_id", value)
 
     @property
     @pulumi.getter(name="lbMethod")
     def lb_method(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_method")
 
     @lb_method.setter
     def lb_method(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_method", value)
 
     @property
     @pulumi.getter(name="lbProvider")
     def lb_provider(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_provider")
 
     @lb_provider.setter
     def lb_provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_provider", value)
 
     @property
     @pulumi.getter(name="lbVersion")
     def lb_version(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_version")
 
     @lb_version.setter
     def lb_version(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "lb_version", value)
 
     @property
     @pulumi.getter(name="manageSecurityGroups")
     def manage_security_groups(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "manage_security_groups")
 
     @manage_security_groups.setter
     def manage_security_groups(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "manage_security_groups", value)
 
     @property
     @pulumi.getter(name="monitorDelay")
     def monitor_delay(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_delay")
 
     @monitor_delay.setter
     def monitor_delay(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "monitor_delay", value)
 
     @property
     @pulumi.getter(name="monitorMaxRetries")
     def monitor_max_retries(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "monitor_max_retries")
 
     @monitor_max_retries.setter
     def monitor_max_retries(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "monitor_max_retries", value)
 
     @property
     @pulumi.getter(name="monitorTimeout")
     def monitor_timeout(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_timeout")
 
     @monitor_timeout.setter
     def monitor_timeout(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "monitor_timeout", value)
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "subnet_id")
 
     @subnet_id.setter
     def subnet_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "subnet_id", value)
 
     @property
     @pulumi.getter(name="useOctavia")
     def use_octavia(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "use_octavia")
 
     @use_octavia.setter
     def use_octavia(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_octavia", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudProviderMetadataArgs:
     def __init__(__self__, *,
                  request_timeout: Optional[pulumi.Input[int]] = None,
                  search_order: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[int] request_timeout: (int)
-        :param pulumi.Input[str] search_order: (string)
-        """
         if request_timeout is not None:
             pulumi.set(__self__, "request_timeout", request_timeout)
         if search_order is not None:
             pulumi.set(__self__, "search_order", search_order)
 
     @property
     @pulumi.getter(name="requestTimeout")
     def request_timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "request_timeout")
 
     @request_timeout.setter
     def request_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "request_timeout", value)
 
     @property
     @pulumi.getter(name="searchOrder")
     def search_order(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "search_order")
 
     @search_order.setter
     def search_order(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "search_order", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderOpenstackCloudProviderRouteArgs:
     def __init__(__self__, *,
                  router_id: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] router_id: (string)
-        """
         if router_id is not None:
             pulumi.set(__self__, "router_id", router_id)
 
     @property
     @pulumi.getter(name="routerId")
     def router_id(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "router_id")
 
     @router_id.setter
     def router_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "router_id", value)
 
 
@@ -3504,71 +3088,55 @@
     def __init__(__self__, *,
                  virtual_centers: pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudConfigVirtualCenterArgs']]],
                  workspace: pulumi.Input['ClusterCloudProviderVsphereCloudConfigWorkspaceArgs'],
                  disk: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigDiskArgs']] = None,
                  global_: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigGlobalArgs']] = None,
                  network: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigNetworkArgs']] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudConfigVirtualCenterArgs']]] virtual_centers: (List)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudConfigWorkspaceArgs'] workspace: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudConfigDiskArgs'] disk: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudConfigGlobalArgs'] global_: (list maxitems:1)
         :param pulumi.Input['ClusterCloudProviderVsphereCloudConfigNetworkArgs'] network: RKE k8s cluster network configuration (list maxitems:1)
         """
         pulumi.set(__self__, "virtual_centers", virtual_centers)
         pulumi.set(__self__, "workspace", workspace)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if network is not None:
             pulumi.set(__self__, "network", network)
 
     @property
     @pulumi.getter(name="virtualCenters")
     def virtual_centers(self) -> pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudConfigVirtualCenterArgs']]]:
-        """
-        (List)
-        """
         return pulumi.get(self, "virtual_centers")
 
     @virtual_centers.setter
     def virtual_centers(self, value: pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudConfigVirtualCenterArgs']]]):
         pulumi.set(self, "virtual_centers", value)
 
     @property
     @pulumi.getter
     def workspace(self) -> pulumi.Input['ClusterCloudProviderVsphereCloudConfigWorkspaceArgs']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "workspace")
 
     @workspace.setter
     def workspace(self, value: pulumi.Input['ClusterCloudProviderVsphereCloudConfigWorkspaceArgs']):
         pulumi.set(self, "workspace", value)
 
     @property
     @pulumi.getter
     def disk(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigDiskArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigDiskArgs']]):
         pulumi.set(self, "disk", value)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigGlobalArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudConfigGlobalArgs']]):
         pulumi.set(self, "global_", value)
 
     @property
@@ -3584,26 +3152,20 @@
         pulumi.set(self, "network", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderVsphereCloudConfigDiskArgs:
     def __init__(__self__, *,
                  scsi_controller_type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] scsi_controller_type: (string)
-        """
         if scsi_controller_type is not None:
             pulumi.set(__self__, "scsi_controller_type", scsi_controller_type)
 
     @property
     @pulumi.getter(name="scsiControllerType")
     def scsi_controller_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "scsi_controller_type")
 
     @scsi_controller_type.setter
     def scsi_controller_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scsi_controller_type", value)
 
 
@@ -3617,27 +3179,14 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  soap_roundtrip_count: Optional[pulumi.Input[int]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  vm_name: Optional[pulumi.Input[str]] = None,
                  vm_uuid: Optional[pulumi.Input[str]] = None,
                  working_dir: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] datacenter: (string)
-        :param pulumi.Input[str] datacenters: (string)
-        :param pulumi.Input[str] datastore: (string)
-        :param pulumi.Input[bool] insecure_flag: (bool)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
-        :param pulumi.Input[int] soap_roundtrip_count: (int)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[str] vm_name: (string)
-        :param pulumi.Input[str] vm_uuid: (string)
-        :param pulumi.Input[str] working_dir: (string)
-        """
         if datacenter is not None:
             pulumi.set(__self__, "datacenter", datacenter)
         if datacenters is not None:
             pulumi.set(__self__, "datacenters", datacenters)
         if datastore is not None:
             pulumi.set(__self__, "datastore", datastore)
         if insecure_flag is not None:
@@ -3656,160 +3205,121 @@
             pulumi.set(__self__, "vm_uuid", vm_uuid)
         if working_dir is not None:
             pulumi.set(__self__, "working_dir", working_dir)
 
     @property
     @pulumi.getter
     def datacenter(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @datacenter.setter
     def datacenter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datacenter", value)
 
     @property
     @pulumi.getter
     def datacenters(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @datacenters.setter
     def datacenters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datacenters", value)
 
     @property
     @pulumi.getter
     def datastore(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datastore")
 
     @datastore.setter
     def datastore(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore", value)
 
     @property
     @pulumi.getter(name="insecureFlag")
     def insecure_flag(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "insecure_flag")
 
     @insecure_flag.setter
     def insecure_flag(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "insecure_flag", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @soap_roundtrip_count.setter
     def soap_roundtrip_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "soap_roundtrip_count", value)
 
     @property
     @pulumi.getter
     def user(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="vmName")
     def vm_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_name")
 
     @vm_name.setter
     def vm_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_name", value)
 
     @property
     @pulumi.getter(name="vmUuid")
     def vm_uuid(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_uuid")
 
     @vm_uuid.setter
     def vm_uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_uuid", value)
 
     @property
     @pulumi.getter(name="workingDir")
     def working_dir(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "working_dir")
 
     @working_dir.setter
     def working_dir(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "working_dir", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderVsphereCloudConfigNetworkArgs:
     def __init__(__self__, *,
                  public_network: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] public_network: (string)
-        """
         if public_network is not None:
             pulumi.set(__self__, "public_network", public_network)
 
     @property
     @pulumi.getter(name="publicNetwork")
     def public_network(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "public_network")
 
     @public_network.setter
     def public_network(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_network", value)
 
 
@@ -3818,97 +3328,71 @@
     def __init__(__self__, *,
                  datacenters: pulumi.Input[str],
                  name: pulumi.Input[str],
                  password: pulumi.Input[str],
                  user: pulumi.Input[str],
                  port: Optional[pulumi.Input[str]] = None,
                  soap_roundtrip_count: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[str] datacenters: (string)
-        :param pulumi.Input[str] name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
-        :param pulumi.Input[int] soap_roundtrip_count: (int)
-        """
         pulumi.set(__self__, "datacenters", datacenters)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if soap_roundtrip_count is not None:
             pulumi.set(__self__, "soap_roundtrip_count", soap_roundtrip_count)
 
     @property
     @pulumi.getter
     def datacenters(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @datacenters.setter
     def datacenters(self, value: pulumi.Input[str]):
         pulumi.set(self, "datacenters", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Input[str]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @soap_roundtrip_count.setter
     def soap_roundtrip_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "soap_roundtrip_count", value)
 
 
@@ -3916,84 +3400,62 @@
 class ClusterCloudProviderVsphereCloudConfigWorkspaceArgs:
     def __init__(__self__, *,
                  datacenter: pulumi.Input[str],
                  server: pulumi.Input[str],
                  default_datastore: Optional[pulumi.Input[str]] = None,
                  folder: Optional[pulumi.Input[str]] = None,
                  resourcepool_path: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] datacenter: (string)
-        :param pulumi.Input[str] server: (string)
-        :param pulumi.Input[str] default_datastore: (string)
-        :param pulumi.Input[str] folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param pulumi.Input[str] resourcepool_path: (string)
-        """
         pulumi.set(__self__, "datacenter", datacenter)
         pulumi.set(__self__, "server", server)
         if default_datastore is not None:
             pulumi.set(__self__, "default_datastore", default_datastore)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if resourcepool_path is not None:
             pulumi.set(__self__, "resourcepool_path", resourcepool_path)
 
     @property
     @pulumi.getter
     def datacenter(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @datacenter.setter
     def datacenter(self, value: pulumi.Input[str]):
         pulumi.set(self, "datacenter", value)
 
     @property
     @pulumi.getter
     def server(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: pulumi.Input[str]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter(name="defaultDatastore")
     def default_datastore(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "default_datastore")
 
     @default_datastore.setter
     def default_datastore(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_datastore", value)
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[pulumi.Input[str]]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @folder.setter
     def folder(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "folder", value)
 
     @property
     @pulumi.getter(name="resourcepoolPath")
     def resourcepool_path(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "resourcepool_path")
 
     @resourcepool_path.setter
     def resourcepool_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "resourcepool_path", value)
 
 
@@ -4002,71 +3464,55 @@
     def __init__(__self__, *,
                  virtual_centers: pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudProviderVirtualCenterArgs']]],
                  workspace: pulumi.Input['ClusterCloudProviderVsphereCloudProviderWorkspaceArgs'],
                  disk: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderDiskArgs']] = None,
                  global_: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderGlobalArgs']] = None,
                  network: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderNetworkArgs']] = None):
         """
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudProviderVirtualCenterArgs']]] virtual_centers: (List)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderWorkspaceArgs'] workspace: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderDiskArgs'] disk: (list maxitems:1)
-        :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderGlobalArgs'] global_: (list maxitems:1)
         :param pulumi.Input['ClusterCloudProviderVsphereCloudProviderNetworkArgs'] network: RKE k8s cluster network configuration (list maxitems:1)
         """
         pulumi.set(__self__, "virtual_centers", virtual_centers)
         pulumi.set(__self__, "workspace", workspace)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if network is not None:
             pulumi.set(__self__, "network", network)
 
     @property
     @pulumi.getter(name="virtualCenters")
     def virtual_centers(self) -> pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudProviderVirtualCenterArgs']]]:
-        """
-        (List)
-        """
         return pulumi.get(self, "virtual_centers")
 
     @virtual_centers.setter
     def virtual_centers(self, value: pulumi.Input[Sequence[pulumi.Input['ClusterCloudProviderVsphereCloudProviderVirtualCenterArgs']]]):
         pulumi.set(self, "virtual_centers", value)
 
     @property
     @pulumi.getter
     def workspace(self) -> pulumi.Input['ClusterCloudProviderVsphereCloudProviderWorkspaceArgs']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "workspace")
 
     @workspace.setter
     def workspace(self, value: pulumi.Input['ClusterCloudProviderVsphereCloudProviderWorkspaceArgs']):
         pulumi.set(self, "workspace", value)
 
     @property
     @pulumi.getter
     def disk(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderDiskArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "disk")
 
     @disk.setter
     def disk(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderDiskArgs']]):
         pulumi.set(self, "disk", value)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderGlobalArgs']]:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @global_.setter
     def global_(self, value: Optional[pulumi.Input['ClusterCloudProviderVsphereCloudProviderGlobalArgs']]):
         pulumi.set(self, "global_", value)
 
     @property
@@ -4082,26 +3528,20 @@
         pulumi.set(self, "network", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderVsphereCloudProviderDiskArgs:
     def __init__(__self__, *,
                  scsi_controller_type: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] scsi_controller_type: (string)
-        """
         if scsi_controller_type is not None:
             pulumi.set(__self__, "scsi_controller_type", scsi_controller_type)
 
     @property
     @pulumi.getter(name="scsiControllerType")
     def scsi_controller_type(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "scsi_controller_type")
 
     @scsi_controller_type.setter
     def scsi_controller_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "scsi_controller_type", value)
 
 
@@ -4115,27 +3555,14 @@
                  password: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[str]] = None,
                  soap_roundtrip_count: Optional[pulumi.Input[int]] = None,
                  user: Optional[pulumi.Input[str]] = None,
                  vm_name: Optional[pulumi.Input[str]] = None,
                  vm_uuid: Optional[pulumi.Input[str]] = None,
                  working_dir: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] datacenter: (string)
-        :param pulumi.Input[str] datacenters: (string)
-        :param pulumi.Input[str] datastore: (string)
-        :param pulumi.Input[bool] insecure_flag: (bool)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
-        :param pulumi.Input[int] soap_roundtrip_count: (int)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[str] vm_name: (string)
-        :param pulumi.Input[str] vm_uuid: (string)
-        :param pulumi.Input[str] working_dir: (string)
-        """
         if datacenter is not None:
             pulumi.set(__self__, "datacenter", datacenter)
         if datacenters is not None:
             pulumi.set(__self__, "datacenters", datacenters)
         if datastore is not None:
             pulumi.set(__self__, "datastore", datastore)
         if insecure_flag is not None:
@@ -4154,160 +3581,121 @@
             pulumi.set(__self__, "vm_uuid", vm_uuid)
         if working_dir is not None:
             pulumi.set(__self__, "working_dir", working_dir)
 
     @property
     @pulumi.getter
     def datacenter(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @datacenter.setter
     def datacenter(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datacenter", value)
 
     @property
     @pulumi.getter
     def datacenters(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @datacenters.setter
     def datacenters(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datacenters", value)
 
     @property
     @pulumi.getter
     def datastore(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datastore")
 
     @datastore.setter
     def datastore(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "datastore", value)
 
     @property
     @pulumi.getter(name="insecureFlag")
     def insecure_flag(self) -> Optional[pulumi.Input[bool]]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "insecure_flag")
 
     @insecure_flag.setter
     def insecure_flag(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "insecure_flag", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @soap_roundtrip_count.setter
     def soap_roundtrip_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "soap_roundtrip_count", value)
 
     @property
     @pulumi.getter
     def user(self) -> Optional[pulumi.Input[str]]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="vmName")
     def vm_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_name")
 
     @vm_name.setter
     def vm_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_name", value)
 
     @property
     @pulumi.getter(name="vmUuid")
     def vm_uuid(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_uuid")
 
     @vm_uuid.setter
     def vm_uuid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "vm_uuid", value)
 
     @property
     @pulumi.getter(name="workingDir")
     def working_dir(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "working_dir")
 
     @working_dir.setter
     def working_dir(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "working_dir", value)
 
 
 @pulumi.input_type
 class ClusterCloudProviderVsphereCloudProviderNetworkArgs:
     def __init__(__self__, *,
                  public_network: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] public_network: (string)
-        """
         if public_network is not None:
             pulumi.set(__self__, "public_network", public_network)
 
     @property
     @pulumi.getter(name="publicNetwork")
     def public_network(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "public_network")
 
     @public_network.setter
     def public_network(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "public_network", value)
 
 
@@ -4316,97 +3704,71 @@
     def __init__(__self__, *,
                  datacenters: pulumi.Input[str],
                  name: pulumi.Input[str],
                  password: pulumi.Input[str],
                  user: pulumi.Input[str],
                  port: Optional[pulumi.Input[str]] = None,
                  soap_roundtrip_count: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[str] datacenters: (string)
-        :param pulumi.Input[str] name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
-        :param pulumi.Input[int] soap_roundtrip_count: (int)
-        """
         pulumi.set(__self__, "datacenters", datacenters)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if soap_roundtrip_count is not None:
             pulumi.set(__self__, "soap_roundtrip_count", soap_roundtrip_count)
 
     @property
     @pulumi.getter
     def datacenters(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @datacenters.setter
     def datacenters(self, value: pulumi.Input[str]):
         pulumi.set(self, "datacenters", value)
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Input[str]:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: pulumi.Input[str]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Input[str]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[pulumi.Input[int]]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @soap_roundtrip_count.setter
     def soap_roundtrip_count(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "soap_roundtrip_count", value)
 
 
@@ -4414,123 +3776,91 @@
 class ClusterCloudProviderVsphereCloudProviderWorkspaceArgs:
     def __init__(__self__, *,
                  datacenter: pulumi.Input[str],
                  server: pulumi.Input[str],
                  default_datastore: Optional[pulumi.Input[str]] = None,
                  folder: Optional[pulumi.Input[str]] = None,
                  resourcepool_path: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] datacenter: (string)
-        :param pulumi.Input[str] server: (string)
-        :param pulumi.Input[str] default_datastore: (string)
-        :param pulumi.Input[str] folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param pulumi.Input[str] resourcepool_path: (string)
-        """
         pulumi.set(__self__, "datacenter", datacenter)
         pulumi.set(__self__, "server", server)
         if default_datastore is not None:
             pulumi.set(__self__, "default_datastore", default_datastore)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if resourcepool_path is not None:
             pulumi.set(__self__, "resourcepool_path", resourcepool_path)
 
     @property
     @pulumi.getter
     def datacenter(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @datacenter.setter
     def datacenter(self, value: pulumi.Input[str]):
         pulumi.set(self, "datacenter", value)
 
     @property
     @pulumi.getter
     def server(self) -> pulumi.Input[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "server")
 
     @server.setter
     def server(self, value: pulumi.Input[str]):
         pulumi.set(self, "server", value)
 
     @property
     @pulumi.getter(name="defaultDatastore")
     def default_datastore(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "default_datastore")
 
     @default_datastore.setter
     def default_datastore(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "default_datastore", value)
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[pulumi.Input[str]]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @folder.setter
     def folder(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "folder", value)
 
     @property
     @pulumi.getter(name="resourcepoolPath")
     def resourcepool_path(self) -> Optional[pulumi.Input[str]]:
-        """
-        (string)
-        """
         return pulumi.get(self, "resourcepool_path")
 
     @resourcepool_path.setter
     def resourcepool_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "resourcepool_path", value)
 
 
 @pulumi.input_type
 class ClusterControlPlaneHostArgs:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
 
@@ -4539,19 +3869,19 @@
     def __init__(__self__, *,
                  node_selector: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  nodelocal: Optional[pulumi.Input['ClusterDnsNodelocalArgs']] = None,
                  provider: Optional[pulumi.Input[str]] = None,
                  reverse_cidrs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  upstream_nameservers: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair (map)
-        :param pulumi.Input['ClusterDnsNodelocalArgs'] nodelocal: Docker image for nodelocal (string)
-        :param pulumi.Input[str] provider: Monitoring provider (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] reverse_cidrs: Reverse CIDRs  (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] upstream_nameservers: Upstream nameservers  (list)
+        :param pulumi.Input[Mapping[str, Any]] node_selector: NodeSelector key pair
+        :param pulumi.Input['ClusterDnsNodelocalArgs'] nodelocal: Nodelocal dns
+        :param pulumi.Input[str] provider: DNS provider
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] reverse_cidrs: ReverseCIDRs
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] upstream_nameservers: Upstream nameservers
         """
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
         if nodelocal is not None:
             pulumi.set(__self__, "nodelocal", nodelocal)
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
@@ -4560,181 +3890,157 @@
         if upstream_nameservers is not None:
             pulumi.set(__self__, "upstream_nameservers", upstream_nameservers)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Node selector key pair (map)
+        NodeSelector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @node_selector.setter
     def node_selector(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "node_selector", value)
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional[pulumi.Input['ClusterDnsNodelocalArgs']]:
         """
-        Docker image for nodelocal (string)
+        Nodelocal dns
         """
         return pulumi.get(self, "nodelocal")
 
     @nodelocal.setter
     def nodelocal(self, value: Optional[pulumi.Input['ClusterDnsNodelocalArgs']]):
         pulumi.set(self, "nodelocal", value)
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[pulumi.Input[str]]:
         """
-        Monitoring provider (string)
+        DNS provider
         """
         return pulumi.get(self, "provider")
 
     @provider.setter
     def provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "provider", value)
 
     @property
     @pulumi.getter(name="reverseCidrs")
     def reverse_cidrs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Reverse CIDRs  (list)
+        ReverseCIDRs
         """
         return pulumi.get(self, "reverse_cidrs")
 
     @reverse_cidrs.setter
     def reverse_cidrs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "reverse_cidrs", value)
 
     @property
     @pulumi.getter(name="upstreamNameservers")
     def upstream_nameservers(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Upstream nameservers  (list)
+        Upstream nameservers
         """
         return pulumi.get(self, "upstream_nameservers")
 
     @upstream_nameservers.setter
     def upstream_nameservers(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "upstream_nameservers", value)
 
 
 @pulumi.input_type
 class ClusterDnsNodelocalArgs:
     def __init__(__self__, *,
                  ip_address: Optional[pulumi.Input[str]] = None,
                  node_selector: Optional[pulumi.Input[Mapping[str, Any]]] = None):
         """
-        :param pulumi.Input[str] ip_address: Nodelocal dns ip address (string)
-        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair (map)
+        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair
         """
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[pulumi.Input[str]]:
-        """
-        Nodelocal dns ip address (string)
-        """
         return pulumi.get(self, "ip_address")
 
     @ip_address.setter
     def ip_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address", value)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @node_selector.setter
     def node_selector(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "node_selector", value)
 
 
 @pulumi.input_type
 class ClusterEtcdHostArgs:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
 
 @pulumi.input_type
 class ClusterInactiveHostArgs:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
 
@@ -4748,22 +4054,22 @@
                  https_port: Optional[pulumi.Input[int]] = None,
                  network_mode: Optional[pulumi.Input[str]] = None,
                  node_selector: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  provider: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] default_backend: Ingress Default Backend
-        :param pulumi.Input[str] dns_policy: Ingress controller DNS policy. `ClusterFirstWithHostNet`, `ClusterFirst`, `Default`, and `None` are supported. [K8S dns Policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pod-s-dns-policy) (string)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[int] http_port: Ingress controller http port (int)
-        :param pulumi.Input[int] https_port: Ingress controller https port (int)
-        :param pulumi.Input[str] network_mode: Networt mode for the ingress controller. `hostNetwork`, `hostPort` and `none` are supported (string)
-        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair (map)
-        :param pulumi.Input[Mapping[str, Any]] options: Network provider options (map)
-        :param pulumi.Input[str] provider: Monitoring provider (string)
+        :param pulumi.Input[str] dns_policy: Ingress controller dns policy
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for the ingress controller
+        :param pulumi.Input[int] http_port: Ingress controller http port
+        :param pulumi.Input[int] https_port: Ingress controller https port
+        :param pulumi.Input[str] network_mode: Ingress controller network mode
+        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair
+        :param pulumi.Input[Mapping[str, Any]] options: Ingress controller options
+        :param pulumi.Input[str] provider: Ingress controller provider
         """
         if default_backend is not None:
             pulumi.set(__self__, "default_backend", default_backend)
         if dns_policy is not None:
             pulumi.set(__self__, "dns_policy", dns_policy)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -4792,99 +4098,99 @@
     def default_backend(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "default_backend", value)
 
     @property
     @pulumi.getter(name="dnsPolicy")
     def dns_policy(self) -> Optional[pulumi.Input[str]]:
         """
-        Ingress controller DNS policy. `ClusterFirstWithHostNet`, `ClusterFirst`, `Default`, and `None` are supported. [K8S dns Policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pod-s-dns-policy) (string)
+        Ingress controller dns policy
         """
         return pulumi.get(self, "dns_policy")
 
     @dns_policy.setter
     def dns_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_policy", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments for the ingress controller
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="httpPort")
     def http_port(self) -> Optional[pulumi.Input[int]]:
         """
-        Ingress controller http port (int)
+        Ingress controller http port
         """
         return pulumi.get(self, "http_port")
 
     @http_port.setter
     def http_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "http_port", value)
 
     @property
     @pulumi.getter(name="httpsPort")
     def https_port(self) -> Optional[pulumi.Input[int]]:
         """
-        Ingress controller https port (int)
+        Ingress controller https port
         """
         return pulumi.get(self, "https_port")
 
     @https_port.setter
     def https_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "https_port", value)
 
     @property
     @pulumi.getter(name="networkMode")
     def network_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        Networt mode for the ingress controller. `hostNetwork`, `hostPort` and `none` are supported (string)
+        Ingress controller network mode
         """
         return pulumi.get(self, "network_mode")
 
     @network_mode.setter
     def network_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "network_mode", value)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @node_selector.setter
     def node_selector(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "node_selector", value)
 
     @property
     @pulumi.getter
     def options(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Network provider options (map)
+        Ingress controller options
         """
         return pulumi.get(self, "options")
 
     @options.setter
     def options(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "options", value)
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[pulumi.Input[str]]:
         """
-        Monitoring provider (string)
+        Ingress controller provider
         """
         return pulumi.get(self, "provider")
 
     @provider.setter
     def provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "provider", value)
 
@@ -4892,54 +4198,54 @@
 @pulumi.input_type
 class ClusterMonitoringArgs:
     def __init__(__self__, *,
                  node_selector: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  provider: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair (map)
-        :param pulumi.Input[Mapping[str, Any]] options: Network provider options (map)
-        :param pulumi.Input[str] provider: Monitoring provider (string)
+        :param pulumi.Input[Mapping[str, Any]] node_selector: Node selector key pair
+        :param pulumi.Input[Mapping[str, Any]] options: Monitoring options
+        :param pulumi.Input[str] provider: Monitoring provider
         """
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
         if options is not None:
             pulumi.set(__self__, "options", options)
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @node_selector.setter
     def node_selector(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "node_selector", value)
 
     @property
     @pulumi.getter
     def options(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Network provider options (map)
+        Monitoring options
         """
         return pulumi.get(self, "options")
 
     @options.setter
     def options(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "options", value)
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[pulumi.Input[str]]:
         """
-        Monitoring provider (string)
+        Monitoring provider
         """
         return pulumi.get(self, "provider")
 
     @provider.setter
     def provider(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "provider", value)
 
@@ -4952,22 +4258,22 @@
                  canal_network_provider: Optional[pulumi.Input['ClusterNetworkCanalNetworkProviderArgs']] = None,
                  flannel_network_provider: Optional[pulumi.Input['ClusterNetworkFlannelNetworkProviderArgs']] = None,
                  mtu: Optional[pulumi.Input[int]] = None,
                  options: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  plugin: Optional[pulumi.Input[str]] = None,
                  weave_network_provider: Optional[pulumi.Input['ClusterNetworkWeaveNetworkProviderArgs']] = None):
         """
-        :param pulumi.Input['ClusterNetworkAciNetworkProviderArgs'] aci_network_provider: Aci network provider config (list maxitems:1)
-        :param pulumi.Input['ClusterNetworkCalicoNetworkProviderArgs'] calico_network_provider: Calico network provider config (list maxitems:1)
-        :param pulumi.Input['ClusterNetworkCanalNetworkProviderArgs'] canal_network_provider: Canal network provider config (list maxitems:1)
-        :param pulumi.Input['ClusterNetworkFlannelNetworkProviderArgs'] flannel_network_provider: Flannel network provider config (list maxitems:1)
-        :param pulumi.Input[int] mtu: Network provider MTU. Default `0` (int)
-        :param pulumi.Input[Mapping[str, Any]] options: Network provider options (map)
-        :param pulumi.Input[str] plugin: Network provider plugin. `calico`, `canal` (default), `flannel`, `none` and `weave` are supported. (string)
-        :param pulumi.Input['ClusterNetworkWeaveNetworkProviderArgs'] weave_network_provider: Weave network provider config (list maxitems:1)
+        :param pulumi.Input['ClusterNetworkAciNetworkProviderArgs'] aci_network_provider: Aci network provider config
+        :param pulumi.Input['ClusterNetworkCalicoNetworkProviderArgs'] calico_network_provider: Calico network provider config
+        :param pulumi.Input['ClusterNetworkCanalNetworkProviderArgs'] canal_network_provider: Canal network provider config
+        :param pulumi.Input['ClusterNetworkFlannelNetworkProviderArgs'] flannel_network_provider: Flannel network provider config
+        :param pulumi.Input[int] mtu: Network provider MTU
+        :param pulumi.Input[Mapping[str, Any]] options: Network provider options
+        :param pulumi.Input[str] plugin: Network provider plugin
+        :param pulumi.Input['ClusterNetworkWeaveNetworkProviderArgs'] weave_network_provider: Weave network provider config
         """
         if aci_network_provider is not None:
             pulumi.set(__self__, "aci_network_provider", aci_network_provider)
         if calico_network_provider is not None:
             pulumi.set(__self__, "calico_network_provider", calico_network_provider)
         if canal_network_provider is not None:
             pulumi.set(__self__, "canal_network_provider", canal_network_provider)
@@ -4982,99 +4288,99 @@
         if weave_network_provider is not None:
             pulumi.set(__self__, "weave_network_provider", weave_network_provider)
 
     @property
     @pulumi.getter(name="aciNetworkProvider")
     def aci_network_provider(self) -> Optional[pulumi.Input['ClusterNetworkAciNetworkProviderArgs']]:
         """
-        Aci network provider config (list maxitems:1)
+        Aci network provider config
         """
         return pulumi.get(self, "aci_network_provider")
 
     @aci_network_provider.setter
     def aci_network_provider(self, value: Optional[pulumi.Input['ClusterNetworkAciNetworkProviderArgs']]):
         pulumi.set(self, "aci_network_provider", value)
 
     @property
     @pulumi.getter(name="calicoNetworkProvider")
     def calico_network_provider(self) -> Optional[pulumi.Input['ClusterNetworkCalicoNetworkProviderArgs']]:
         """
-        Calico network provider config (list maxitems:1)
+        Calico network provider config
         """
         return pulumi.get(self, "calico_network_provider")
 
     @calico_network_provider.setter
     def calico_network_provider(self, value: Optional[pulumi.Input['ClusterNetworkCalicoNetworkProviderArgs']]):
         pulumi.set(self, "calico_network_provider", value)
 
     @property
     @pulumi.getter(name="canalNetworkProvider")
     def canal_network_provider(self) -> Optional[pulumi.Input['ClusterNetworkCanalNetworkProviderArgs']]:
         """
-        Canal network provider config (list maxitems:1)
+        Canal network provider config
         """
         return pulumi.get(self, "canal_network_provider")
 
     @canal_network_provider.setter
     def canal_network_provider(self, value: Optional[pulumi.Input['ClusterNetworkCanalNetworkProviderArgs']]):
         pulumi.set(self, "canal_network_provider", value)
 
     @property
     @pulumi.getter(name="flannelNetworkProvider")
     def flannel_network_provider(self) -> Optional[pulumi.Input['ClusterNetworkFlannelNetworkProviderArgs']]:
         """
-        Flannel network provider config (list maxitems:1)
+        Flannel network provider config
         """
         return pulumi.get(self, "flannel_network_provider")
 
     @flannel_network_provider.setter
     def flannel_network_provider(self, value: Optional[pulumi.Input['ClusterNetworkFlannelNetworkProviderArgs']]):
         pulumi.set(self, "flannel_network_provider", value)
 
     @property
     @pulumi.getter
     def mtu(self) -> Optional[pulumi.Input[int]]:
         """
-        Network provider MTU. Default `0` (int)
+        Network provider MTU
         """
         return pulumi.get(self, "mtu")
 
     @mtu.setter
     def mtu(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "mtu", value)
 
     @property
     @pulumi.getter
     def options(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Network provider options (map)
+        Network provider options
         """
         return pulumi.get(self, "options")
 
     @options.setter
     def options(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "options", value)
 
     @property
     @pulumi.getter
     def plugin(self) -> Optional[pulumi.Input[str]]:
         """
-        Network provider plugin. `calico`, `canal` (default), `flannel`, `none` and `weave` are supported. (string)
+        Network provider plugin
         """
         return pulumi.get(self, "plugin")
 
     @plugin.setter
     def plugin(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "plugin", value)
 
     @property
     @pulumi.getter(name="weaveNetworkProvider")
     def weave_network_provider(self) -> Optional[pulumi.Input['ClusterNetworkWeaveNetworkProviderArgs']]:
         """
-        Weave network provider config (list maxitems:1)
+        Weave network provider config
         """
         return pulumi.get(self, "weave_network_provider")
 
     @weave_network_provider.setter
     def weave_network_provider(self, value: Optional[pulumi.Input['ClusterNetworkWeaveNetworkProviderArgs']]):
         pulumi.set(self, "weave_network_provider", value)
 
@@ -5102,40 +4408,14 @@
                  system_id: pulumi.Input[str],
                  token: pulumi.Input[str],
                  vrf_name: pulumi.Input[str],
                  vrf_tenant: pulumi.Input[str],
                  snat_port_range_end: Optional[pulumi.Input[str]] = None,
                  snat_port_range_start: Optional[pulumi.Input[str]] = None,
                  snat_ports_per_node: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] aep: Attachment entity profile name on aci (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] apic_hosts: Ip address for apic hosts (list)
-        :param pulumi.Input[str] apic_user_crt: Base64 encoded certificate for aci apic user (string)
-        :param pulumi.Input[str] apic_user_key: Base64 encoded private key for aci apic user (string)
-        :param pulumi.Input[str] apic_user_name: User name for aci apic (string)
-        :param pulumi.Input[str] encap_type: One of the supported encap types for aci(vlan/vxlan) (string)
-        :param pulumi.Input[str] extern_dynamic: Subnet to use for dynamic external IPs on aci (string)
-               * `extern_static"` - (Required) Subnet to use for static external IPs on aci (string)
-        :param pulumi.Input[str] infra_vlan: Vlan for infra network on aci (string)
-        :param pulumi.Input[str] kube_api_vlan: Vlan for node network on aci (string)
-        :param pulumi.Input[str] l3out: L3Out on aci (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] l3out_external_networks: L3out external networks on aci (list)
-        :param pulumi.Input[str] mcast_range_end: Mcast range end address for endpoint groups on aci (string)
-        :param pulumi.Input[str] mcast_range_start: Mcast range start address for endpoint groups on aci (string)
-        :param pulumi.Input[str] node_subnet: Kubernetes node address subnet (string)
-        :param pulumi.Input[str] node_svc_subnet: Subnet to use for service graph endpoints on aci (string)
-        :param pulumi.Input[str] service_vlan: Vlan for service graph nodes on aci (string)
-        :param pulumi.Input[str] system_id: Unique suffix for all cluster related objects in aci (string)
-        :param pulumi.Input[str] token: UUID for this version of the input configuration (string)
-        :param pulumi.Input[str] vrf_name: VRF Name on aci (string)
-        :param pulumi.Input[str] vrf_tenant: Tenant for VRF on aci (string)
-        :param pulumi.Input[str] snat_port_range_end: Port end range for Source Network Address Translation on aci (string)
-        :param pulumi.Input[str] snat_port_range_start: Port start range for Source Network Address Translation on aci (string)
-        :param pulumi.Input[str] snat_ports_per_node: Ports per node for Source Network Address Translation on aci (string)
-        """
         pulumi.set(__self__, "aep", aep)
         pulumi.set(__self__, "apic_hosts", apic_hosts)
         pulumi.set(__self__, "apic_user_crt", apic_user_crt)
         pulumi.set(__self__, "apic_user_key", apic_user_key)
         pulumi.set(__self__, "apic_user_name", apic_user_name)
         pulumi.set(__self__, "encap_type", encap_type)
         pulumi.set(__self__, "extern_dynamic", extern_dynamic)
@@ -5159,90 +4439,68 @@
             pulumi.set(__self__, "snat_port_range_start", snat_port_range_start)
         if snat_ports_per_node is not None:
             pulumi.set(__self__, "snat_ports_per_node", snat_ports_per_node)
 
     @property
     @pulumi.getter
     def aep(self) -> pulumi.Input[str]:
-        """
-        Attachment entity profile name on aci (string)
-        """
         return pulumi.get(self, "aep")
 
     @aep.setter
     def aep(self, value: pulumi.Input[str]):
         pulumi.set(self, "aep", value)
 
     @property
     @pulumi.getter(name="apicHosts")
     def apic_hosts(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        Ip address for apic hosts (list)
-        """
         return pulumi.get(self, "apic_hosts")
 
     @apic_hosts.setter
     def apic_hosts(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "apic_hosts", value)
 
     @property
     @pulumi.getter(name="apicUserCrt")
     def apic_user_crt(self) -> pulumi.Input[str]:
-        """
-        Base64 encoded certificate for aci apic user (string)
-        """
         return pulumi.get(self, "apic_user_crt")
 
     @apic_user_crt.setter
     def apic_user_crt(self, value: pulumi.Input[str]):
         pulumi.set(self, "apic_user_crt", value)
 
     @property
     @pulumi.getter(name="apicUserKey")
     def apic_user_key(self) -> pulumi.Input[str]:
-        """
-        Base64 encoded private key for aci apic user (string)
-        """
         return pulumi.get(self, "apic_user_key")
 
     @apic_user_key.setter
     def apic_user_key(self, value: pulumi.Input[str]):
         pulumi.set(self, "apic_user_key", value)
 
     @property
     @pulumi.getter(name="apicUserName")
     def apic_user_name(self) -> pulumi.Input[str]:
-        """
-        User name for aci apic (string)
-        """
         return pulumi.get(self, "apic_user_name")
 
     @apic_user_name.setter
     def apic_user_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "apic_user_name", value)
 
     @property
     @pulumi.getter(name="encapType")
     def encap_type(self) -> pulumi.Input[str]:
-        """
-        One of the supported encap types for aci(vlan/vxlan) (string)
-        """
         return pulumi.get(self, "encap_type")
 
     @encap_type.setter
     def encap_type(self, value: pulumi.Input[str]):
         pulumi.set(self, "encap_type", value)
 
     @property
     @pulumi.getter(name="externDynamic")
     def extern_dynamic(self) -> pulumi.Input[str]:
-        """
-        Subnet to use for dynamic external IPs on aci (string)
-        * `extern_static"` - (Required) Subnet to use for static external IPs on aci (string)
-        """
         return pulumi.get(self, "extern_dynamic")
 
     @extern_dynamic.setter
     def extern_dynamic(self, value: pulumi.Input[str]):
         pulumi.set(self, "extern_dynamic", value)
 
     @property
@@ -5253,197 +4511,149 @@
     @extern_static.setter
     def extern_static(self, value: pulumi.Input[str]):
         pulumi.set(self, "extern_static", value)
 
     @property
     @pulumi.getter(name="infraVlan")
     def infra_vlan(self) -> pulumi.Input[str]:
-        """
-        Vlan for infra network on aci (string)
-        """
         return pulumi.get(self, "infra_vlan")
 
     @infra_vlan.setter
     def infra_vlan(self, value: pulumi.Input[str]):
         pulumi.set(self, "infra_vlan", value)
 
     @property
     @pulumi.getter(name="kubeApiVlan")
     def kube_api_vlan(self) -> pulumi.Input[str]:
-        """
-        Vlan for node network on aci (string)
-        """
         return pulumi.get(self, "kube_api_vlan")
 
     @kube_api_vlan.setter
     def kube_api_vlan(self, value: pulumi.Input[str]):
         pulumi.set(self, "kube_api_vlan", value)
 
     @property
     @pulumi.getter
     def l3out(self) -> pulumi.Input[str]:
-        """
-        L3Out on aci (string)
-        """
         return pulumi.get(self, "l3out")
 
     @l3out.setter
     def l3out(self, value: pulumi.Input[str]):
         pulumi.set(self, "l3out", value)
 
     @property
     @pulumi.getter(name="l3outExternalNetworks")
     def l3out_external_networks(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
-        """
-        L3out external networks on aci (list)
-        """
         return pulumi.get(self, "l3out_external_networks")
 
     @l3out_external_networks.setter
     def l3out_external_networks(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "l3out_external_networks", value)
 
     @property
     @pulumi.getter(name="mcastRangeEnd")
     def mcast_range_end(self) -> pulumi.Input[str]:
-        """
-        Mcast range end address for endpoint groups on aci (string)
-        """
         return pulumi.get(self, "mcast_range_end")
 
     @mcast_range_end.setter
     def mcast_range_end(self, value: pulumi.Input[str]):
         pulumi.set(self, "mcast_range_end", value)
 
     @property
     @pulumi.getter(name="mcastRangeStart")
     def mcast_range_start(self) -> pulumi.Input[str]:
-        """
-        Mcast range start address for endpoint groups on aci (string)
-        """
         return pulumi.get(self, "mcast_range_start")
 
     @mcast_range_start.setter
     def mcast_range_start(self, value: pulumi.Input[str]):
         pulumi.set(self, "mcast_range_start", value)
 
     @property
     @pulumi.getter(name="nodeSubnet")
     def node_subnet(self) -> pulumi.Input[str]:
-        """
-        Kubernetes node address subnet (string)
-        """
         return pulumi.get(self, "node_subnet")
 
     @node_subnet.setter
     def node_subnet(self, value: pulumi.Input[str]):
         pulumi.set(self, "node_subnet", value)
 
     @property
     @pulumi.getter(name="nodeSvcSubnet")
     def node_svc_subnet(self) -> pulumi.Input[str]:
-        """
-        Subnet to use for service graph endpoints on aci (string)
-        """
         return pulumi.get(self, "node_svc_subnet")
 
     @node_svc_subnet.setter
     def node_svc_subnet(self, value: pulumi.Input[str]):
         pulumi.set(self, "node_svc_subnet", value)
 
     @property
     @pulumi.getter(name="serviceVlan")
     def service_vlan(self) -> pulumi.Input[str]:
-        """
-        Vlan for service graph nodes on aci (string)
-        """
         return pulumi.get(self, "service_vlan")
 
     @service_vlan.setter
     def service_vlan(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_vlan", value)
 
     @property
     @pulumi.getter(name="systemId")
     def system_id(self) -> pulumi.Input[str]:
-        """
-        Unique suffix for all cluster related objects in aci (string)
-        """
         return pulumi.get(self, "system_id")
 
     @system_id.setter
     def system_id(self, value: pulumi.Input[str]):
         pulumi.set(self, "system_id", value)
 
     @property
     @pulumi.getter
     def token(self) -> pulumi.Input[str]:
-        """
-        UUID for this version of the input configuration (string)
-        """
         return pulumi.get(self, "token")
 
     @token.setter
     def token(self, value: pulumi.Input[str]):
         pulumi.set(self, "token", value)
 
     @property
     @pulumi.getter(name="vrfName")
     def vrf_name(self) -> pulumi.Input[str]:
-        """
-        VRF Name on aci (string)
-        """
         return pulumi.get(self, "vrf_name")
 
     @vrf_name.setter
     def vrf_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "vrf_name", value)
 
     @property
     @pulumi.getter(name="vrfTenant")
     def vrf_tenant(self) -> pulumi.Input[str]:
-        """
-        Tenant for VRF on aci (string)
-        """
         return pulumi.get(self, "vrf_tenant")
 
     @vrf_tenant.setter
     def vrf_tenant(self, value: pulumi.Input[str]):
         pulumi.set(self, "vrf_tenant", value)
 
     @property
     @pulumi.getter(name="snatPortRangeEnd")
     def snat_port_range_end(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port end range for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_port_range_end")
 
     @snat_port_range_end.setter
     def snat_port_range_end(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snat_port_range_end", value)
 
     @property
     @pulumi.getter(name="snatPortRangeStart")
     def snat_port_range_start(self) -> Optional[pulumi.Input[str]]:
-        """
-        Port start range for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_port_range_start")
 
     @snat_port_range_start.setter
     def snat_port_range_start(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snat_port_range_start", value)
 
     @property
     @pulumi.getter(name="snatPortsPerNode")
     def snat_ports_per_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Ports per node for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_ports_per_node")
 
     @snat_ports_per_node.setter
     def snat_ports_per_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snat_ports_per_node", value)
 
 
@@ -5470,71 +4680,53 @@
         pulumi.set(self, "cloud_provider", value)
 
 
 @pulumi.input_type
 class ClusterNetworkCanalNetworkProviderArgs:
     def __init__(__self__, *,
                  iface: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] iface: Flannel network interface (string)
-        """
         if iface is not None:
             pulumi.set(__self__, "iface", iface)
 
     @property
     @pulumi.getter
     def iface(self) -> Optional[pulumi.Input[str]]:
-        """
-        Flannel network interface (string)
-        """
         return pulumi.get(self, "iface")
 
     @iface.setter
     def iface(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "iface", value)
 
 
 @pulumi.input_type
 class ClusterNetworkFlannelNetworkProviderArgs:
     def __init__(__self__, *,
                  iface: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] iface: Flannel network interface (string)
-        """
         if iface is not None:
             pulumi.set(__self__, "iface", iface)
 
     @property
     @pulumi.getter
     def iface(self) -> Optional[pulumi.Input[str]]:
-        """
-        Flannel network interface (string)
-        """
         return pulumi.get(self, "iface")
 
     @iface.setter
     def iface(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "iface", value)
 
 
 @pulumi.input_type
 class ClusterNetworkWeaveNetworkProviderArgs:
     def __init__(__self__, *,
                  password: pulumi.Input[str]):
-        """
-        :param pulumi.Input[str] password: Registry password (string)
-        """
         pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def password(self) -> pulumi.Input[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: pulumi.Input[str]):
         pulumi.set(self, "password", value)
 
 
@@ -5554,30 +4746,30 @@
                  ssh_agent_auth: Optional[pulumi.Input[bool]] = None,
                  ssh_cert: Optional[pulumi.Input[str]] = None,
                  ssh_cert_path: Optional[pulumi.Input[str]] = None,
                  ssh_key: Optional[pulumi.Input[str]] = None,
                  ssh_key_path: Optional[pulumi.Input[str]] = None,
                  taints: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterNodeTaintArgs']]]] = None):
         """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Node roles in k8s cluster. `controlplane`, `etcd` and `worker` are supported. (list)
-        :param pulumi.Input[str] user: Registry user (string)
-        :param pulumi.Input[str] docker_socket: Docker socket on the node that will be used in tunneling (string)
-        :param pulumi.Input[str] hostname_override: Hostname override for node (string)
-        :param pulumi.Input[str] internal_address: Internal address that will be used for components communication (string)
-        :param pulumi.Input[Mapping[str, Any]] labels: Node labels (map)
-        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine (string)
-        :param pulumi.Input[str] port: Port used for SSH communication (string)
+        :param pulumi.Input[str] address: IP or FQDN that is fully resolvable and used for SSH communication
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] roles: Node roles in k8s cluster [controlplane/worker/etcd])
+        :param pulumi.Input[str] user: SSH user that will be used by RKE
+        :param pulumi.Input[str] docker_socket: Docker socket on the node that will be used in tunneling
+        :param pulumi.Input[str] hostname_override: Hostname override
+        :param pulumi.Input[str] internal_address: Internal address that will be used for components communication
+        :param pulumi.Input[Mapping[str, Any]] labels: Node Labels
+        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine
+        :param pulumi.Input[str] port: Port used for SSH communication
         :param pulumi.Input[str] roles_deprecated: Node role in kubernetes cluster [controlplane/worker/etcd], specified by a comma-separated string
         :param pulumi.Input[bool] ssh_agent_auth: SSH Agent Auth enable (bool)
-        :param pulumi.Input[str] ssh_cert: SSH Certificate (string)
+        :param pulumi.Input[str] ssh_cert: SSH Certificate
         :param pulumi.Input[str] ssh_cert_path: SSH Certificate Path (string)
-        :param pulumi.Input[str] ssh_key: SSH Private Key (string)
+        :param pulumi.Input[str] ssh_key: SSH Private Key
         :param pulumi.Input[str] ssh_key_path: SSH Private Key Path (string)
-        :param pulumi.Input[Sequence[pulumi.Input['ClusterNodeTaintArgs']]] taints: Node taints (list)
+        :param pulumi.Input[Sequence[pulumi.Input['ClusterNodeTaintArgs']]] taints: Node taints
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "roles", roles)
         pulumi.set(__self__, "user", user)
         if docker_socket is not None:
             pulumi.set(__self__, "docker_socket", docker_socket)
         if hostname_override is not None:
@@ -5608,111 +4800,111 @@
         if taints is not None:
             pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter
     def address(self) -> pulumi.Input[str]:
         """
-        Address ip for node (string)
+        IP or FQDN that is fully resolvable and used for SSH communication
         """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: pulumi.Input[str]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter
     def roles(self) -> pulumi.Input[Sequence[pulumi.Input[str]]]:
         """
-        Node roles in k8s cluster. `controlplane`, `etcd` and `worker` are supported. (list)
+        Node roles in k8s cluster [controlplane/worker/etcd])
         """
         return pulumi.get(self, "roles")
 
     @roles.setter
     def roles(self, value: pulumi.Input[Sequence[pulumi.Input[str]]]):
         pulumi.set(self, "roles", value)
 
     @property
     @pulumi.getter
     def user(self) -> pulumi.Input[str]:
         """
-        Registry user (string)
+        SSH user that will be used by RKE
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: pulumi.Input[str]):
         pulumi.set(self, "user", value)
 
     @property
     @pulumi.getter(name="dockerSocket")
     def docker_socket(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker socket on the node that will be used in tunneling (string)
+        Docker socket on the node that will be used in tunneling
         """
         return pulumi.get(self, "docker_socket")
 
     @docker_socket.setter
     def docker_socket(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "docker_socket", value)
 
     @property
     @pulumi.getter(name="hostnameOverride")
     def hostname_override(self) -> Optional[pulumi.Input[str]]:
         """
-        Hostname override for node (string)
+        Hostname override
         """
         return pulumi.get(self, "hostname_override")
 
     @hostname_override.setter
     def hostname_override(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "hostname_override", value)
 
     @property
     @pulumi.getter(name="internalAddress")
     def internal_address(self) -> Optional[pulumi.Input[str]]:
         """
-        Internal address that will be used for components communication (string)
+        Internal address that will be used for components communication
         """
         return pulumi.get(self, "internal_address")
 
     @internal_address.setter
     def internal_address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "internal_address", value)
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Node labels (map)
+        Node Labels
         """
         return pulumi.get(self, "labels")
 
     @labels.setter
     def labels(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "labels", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Name of the host provisioned via docker machine (string)
+        Name of the host provisioned via docker machine
         """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
     @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[str]]:
         """
-        Port used for SSH communication (string)
+        Port used for SSH communication
         """
         return pulumi.get(self, "port")
 
     @port.setter
     def port(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "port", value)
 
@@ -5743,15 +4935,15 @@
     def ssh_agent_auth(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ssh_agent_auth", value)
 
     @property
     @pulumi.getter(name="sshCert")
     def ssh_cert(self) -> Optional[pulumi.Input[str]]:
         """
-        SSH Certificate (string)
+        SSH Certificate
         """
         return pulumi.get(self, "ssh_cert")
 
     @ssh_cert.setter
     def ssh_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_cert", value)
 
@@ -5767,15 +4959,15 @@
     def ssh_cert_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_cert_path", value)
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[pulumi.Input[str]]:
         """
-        SSH Private Key (string)
+        SSH Private Key
         """
         return pulumi.get(self, "ssh_key")
 
     @ssh_key.setter
     def ssh_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key", value)
 
@@ -5791,69 +4983,55 @@
     def ssh_key_path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ssh_key_path", value)
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ClusterNodeTaintArgs']]]]:
         """
-        Node taints (list)
+        Node taints
         """
         return pulumi.get(self, "taints")
 
     @taints.setter
     def taints(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ClusterNodeTaintArgs']]]]):
         pulumi.set(self, "taints", value)
 
 
 @pulumi.input_type
 class ClusterNodeTaintArgs:
     def __init__(__self__, *,
                  key: pulumi.Input[str],
                  value: pulumi.Input[str],
                  effect: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] value: Taint value (string)
-        :param pulumi.Input[str] effect: Taint effect. `NoExecute`, `NoSchedule` (default) and `PreferNoSchedule` are supported (string)
-        """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
 
     @property
     @pulumi.getter
     def key(self) -> pulumi.Input[str]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: pulumi.Input[str]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def value(self) -> pulumi.Input[str]:
-        """
-        Taint value (string)
-        """
         return pulumi.get(self, "value")
 
     @value.setter
     def value(self, value: pulumi.Input[str]):
         pulumi.set(self, "value", value)
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[pulumi.Input[str]]:
-        """
-        Taint effect. `NoExecute`, `NoSchedule` (default) and `PreferNoSchedule` are supported (string)
-        """
         return pulumi.get(self, "effect")
 
     @effect.setter
     def effect(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "effect", value)
 
 
@@ -5861,68 +5039,68 @@
 class ClusterPrivateRegistryArgs:
     def __init__(__self__, *,
                  url: pulumi.Input[str],
                  is_default: Optional[pulumi.Input[bool]] = None,
                  password: Optional[pulumi.Input[str]] = None,
                  user: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] url: Registry URL (string)
-        :param pulumi.Input[bool] is_default: Set as default registry. Default `false` (bool)
-        :param pulumi.Input[str] password: Registry password (string)
-        :param pulumi.Input[str] user: Registry user (string)
+        :param pulumi.Input[str] url: Registry URL
+        :param pulumi.Input[bool] is_default: Set as default registry
+        :param pulumi.Input[str] password: Registry password
+        :param pulumi.Input[str] user: Registry user
         """
         pulumi.set(__self__, "url", url)
         if is_default is not None:
             pulumi.set(__self__, "is_default", is_default)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if user is not None:
             pulumi.set(__self__, "user", user)
 
     @property
     @pulumi.getter
     def url(self) -> pulumi.Input[str]:
         """
-        Registry URL (string)
+        Registry URL
         """
         return pulumi.get(self, "url")
 
     @url.setter
     def url(self, value: pulumi.Input[str]):
         pulumi.set(self, "url", value)
 
     @property
     @pulumi.getter(name="isDefault")
     def is_default(self) -> Optional[pulumi.Input[bool]]:
         """
-        Set as default registry. Default `false` (bool)
+        Set as default registry
         """
         return pulumi.get(self, "is_default")
 
     @is_default.setter
     def is_default(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "is_default", value)
 
     @property
     @pulumi.getter
     def password(self) -> Optional[pulumi.Input[str]]:
         """
-        Registry password (string)
+        Registry password
         """
         return pulumi.get(self, "password")
 
     @password.setter
     def password(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "password", value)
 
     @property
     @pulumi.getter
     def user(self) -> Optional[pulumi.Input[str]]:
         """
-        Registry user (string)
+        Registry user
         """
         return pulumi.get(self, "user")
 
     @user.setter
     def user(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "user", value)
 
@@ -5930,15 +5108,15 @@
 @pulumi.input_type
 class ClusterRestoreArgs:
     def __init__(__self__, *,
                  restore: Optional[pulumi.Input[bool]] = None,
                  snapshot_name: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[bool] restore: RKE k8s cluster restore configuration (list maxitems:1)
-        :param pulumi.Input[str] snapshot_name: Snapshot name (string)
+        :param pulumi.Input[str] snapshot_name: Snapshot name
         """
         if restore is not None:
             pulumi.set(__self__, "restore", restore)
         if snapshot_name is not None:
             pulumi.set(__self__, "snapshot_name", snapshot_name)
 
     @property
@@ -5953,42 +5131,42 @@
     def restore(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "restore", value)
 
     @property
     @pulumi.getter(name="snapshotName")
     def snapshot_name(self) -> Optional[pulumi.Input[str]]:
         """
-        Snapshot name (string)
+        Snapshot name
         """
         return pulumi.get(self, "snapshot_name")
 
     @snapshot_name.setter
     def snapshot_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "snapshot_name", value)
 
 
 @pulumi.input_type
 class ClusterRotateCertificatesArgs:
     def __init__(__self__, *,
                  ca_certificates: Optional[pulumi.Input[bool]] = None,
                  services: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
-        :param pulumi.Input[bool] ca_certificates: Rotate CA Certificates. Default `false` (bool)
+        :param pulumi.Input[bool] ca_certificates: Rotate CA Certificates
         :param pulumi.Input[Sequence[pulumi.Input[str]]] services: RKE k8s cluster services (list maxitems:1)
         """
         if ca_certificates is not None:
             pulumi.set(__self__, "ca_certificates", ca_certificates)
         if services is not None:
             pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter(name="caCertificates")
     def ca_certificates(self) -> Optional[pulumi.Input[bool]]:
         """
-        Rotate CA Certificates. Default `false` (bool)
+        Rotate CA Certificates
         """
         return pulumi.get(self, "ca_certificates")
 
     @ca_certificates.setter
     def ca_certificates(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ca_certificates", value)
 
@@ -6042,51 +5220,15 @@
                  nginx_proxy: Optional[pulumi.Input[str]] = None,
                  nodelocal: Optional[pulumi.Input[str]] = None,
                  pod_infra_container: Optional[pulumi.Input[str]] = None,
                  weave_cni: Optional[pulumi.Input[str]] = None,
                  weave_node: Optional[pulumi.Input[str]] = None,
                  windows_pod_infra_container: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] aci_cni_deploy_container: Docker image for aci_cni_deploy_container (string)
-        :param pulumi.Input[str] aci_controller_container: Docker image for aci_controller_container (string)
-        :param pulumi.Input[str] aci_host_container: Docker image for aci_host_container (string)
-        :param pulumi.Input[str] aci_mcast_container: Docker image for aci_mcast_container (string)
-        :param pulumi.Input[str] aci_opflex_container: Docker image for aci_opflex_container (string)
-        :param pulumi.Input[str] aci_ovs_container: Docker image for aci_ovs_container (string)
-        :param pulumi.Input[str] alpine: Docker image for alpine (string)
-        :param pulumi.Input[str] calico_cni: Docker image for calico_cni (string)
-        :param pulumi.Input[str] calico_controllers: Docker image for calico_controllers (string)
-        :param pulumi.Input[str] calico_ctl: Docker image for calico_ctl (string)
-        :param pulumi.Input[str] calico_flex_vol: Docker image for calico_flex_vol (string)
-        :param pulumi.Input[str] calico_node: Docker image for calico_node (string)
-        :param pulumi.Input[str] canal_cni: Docker image for canal_cni (string)
-        :param pulumi.Input[str] canal_flannel: Docker image for canal_flannel (string)
-        :param pulumi.Input[str] canal_flex_vol: Docker image for canal_flex_vol (string)
-        :param pulumi.Input[str] canal_node: Docker image for canal_node (string)
-        :param pulumi.Input[str] cert_downloader: Docker image for cert_downloader (string)
-        :param pulumi.Input[str] coredns: Docker image for coredns (string)
-        :param pulumi.Input[str] coredns_autoscaler: Docker image for coredns_autoscaler (string)
-        :param pulumi.Input[str] dnsmasq: Docker image for dnsmasq (string)
-        :param pulumi.Input[str] etcd: Docker image for etcd (string)
-        :param pulumi.Input[str] flannel: Docker image for flannel (string)
-        :param pulumi.Input[str] flannel_cni: Docker image for flannel_cni (string)
         :param pulumi.Input[str] ingress: RKE k8s cluster ingress controller configuration (list maxitems:1)
-        :param pulumi.Input[str] ingress_backend: Docker image for ingress_backend (string)
-        :param pulumi.Input[str] kube_dns: Docker image for kube_dns (string)
-        :param pulumi.Input[str] kube_dns_autoscaler: Docker image for kube_dns_autoscaler (string)
-        :param pulumi.Input[str] kube_dns_sidecar: Docker image for kube_dns_sidecar (string)
-        :param pulumi.Input[str] kubernetes: Docker image for kubernetes (string)
-        :param pulumi.Input[str] kubernetes_services_sidecar: Docker image for kubernetes_services_sidecar (string)
-        :param pulumi.Input[str] metrics_server: Docker image for metrics_server (string)
-        :param pulumi.Input[str] nginx_proxy: Docker image for nginx_proxy (string)
-        :param pulumi.Input[str] nodelocal: Docker image for nodelocal (string)
-        :param pulumi.Input[str] pod_infra_container: Docker image for pod_infra_container (string)
-        :param pulumi.Input[str] weave_cni: Docker image for weave_cni (string)
-        :param pulumi.Input[str] weave_node: Docker image for weave_node (string)
-        :param pulumi.Input[str] windows_pod_infra_container: Docker image for windows_pod_infra_container (string)
         """
         if aci_cni_deploy_container is not None:
             pulumi.set(__self__, "aci_cni_deploy_container", aci_cni_deploy_container)
         if aci_controller_container is not None:
             pulumi.set(__self__, "aci_controller_container", aci_controller_container)
         if aci_host_container is not None:
             pulumi.set(__self__, "aci_host_container", aci_host_container)
@@ -6158,281 +5300,212 @@
             pulumi.set(__self__, "weave_node", weave_node)
         if windows_pod_infra_container is not None:
             pulumi.set(__self__, "windows_pod_infra_container", windows_pod_infra_container)
 
     @property
     @pulumi.getter(name="aciCniDeployContainer")
     def aci_cni_deploy_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_cni_deploy_container (string)
-        """
         return pulumi.get(self, "aci_cni_deploy_container")
 
     @aci_cni_deploy_container.setter
     def aci_cni_deploy_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_cni_deploy_container", value)
 
     @property
     @pulumi.getter(name="aciControllerContainer")
     def aci_controller_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_controller_container (string)
-        """
         return pulumi.get(self, "aci_controller_container")
 
     @aci_controller_container.setter
     def aci_controller_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_controller_container", value)
 
     @property
     @pulumi.getter(name="aciHostContainer")
     def aci_host_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_host_container (string)
-        """
         return pulumi.get(self, "aci_host_container")
 
     @aci_host_container.setter
     def aci_host_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_host_container", value)
 
     @property
     @pulumi.getter(name="aciMcastContainer")
     def aci_mcast_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_mcast_container (string)
-        """
         return pulumi.get(self, "aci_mcast_container")
 
     @aci_mcast_container.setter
     def aci_mcast_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_mcast_container", value)
 
     @property
     @pulumi.getter(name="aciOpflexContainer")
     def aci_opflex_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_opflex_container (string)
-        """
         return pulumi.get(self, "aci_opflex_container")
 
     @aci_opflex_container.setter
     def aci_opflex_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_opflex_container", value)
 
     @property
     @pulumi.getter(name="aciOvsContainer")
     def aci_ovs_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_ovs_container (string)
-        """
         return pulumi.get(self, "aci_ovs_container")
 
     @aci_ovs_container.setter
     def aci_ovs_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_ovs_container", value)
 
     @property
     @pulumi.getter
     def alpine(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for alpine (string)
-        """
         return pulumi.get(self, "alpine")
 
     @alpine.setter
     def alpine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alpine", value)
 
     @property
     @pulumi.getter(name="calicoCni")
     def calico_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_cni (string)
-        """
         return pulumi.get(self, "calico_cni")
 
     @calico_cni.setter
     def calico_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_cni", value)
 
     @property
     @pulumi.getter(name="calicoControllers")
     def calico_controllers(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_controllers (string)
-        """
         return pulumi.get(self, "calico_controllers")
 
     @calico_controllers.setter
     def calico_controllers(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_controllers", value)
 
     @property
     @pulumi.getter(name="calicoCtl")
     def calico_ctl(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_ctl (string)
-        """
         return pulumi.get(self, "calico_ctl")
 
     @calico_ctl.setter
     def calico_ctl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_ctl", value)
 
     @property
     @pulumi.getter(name="calicoFlexVol")
     def calico_flex_vol(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_flex_vol (string)
-        """
         return pulumi.get(self, "calico_flex_vol")
 
     @calico_flex_vol.setter
     def calico_flex_vol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_flex_vol", value)
 
     @property
     @pulumi.getter(name="calicoNode")
     def calico_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_node (string)
-        """
         return pulumi.get(self, "calico_node")
 
     @calico_node.setter
     def calico_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_node", value)
 
     @property
     @pulumi.getter(name="canalCni")
     def canal_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_cni (string)
-        """
         return pulumi.get(self, "canal_cni")
 
     @canal_cni.setter
     def canal_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_cni", value)
 
     @property
     @pulumi.getter(name="canalFlannel")
     def canal_flannel(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_flannel (string)
-        """
         return pulumi.get(self, "canal_flannel")
 
     @canal_flannel.setter
     def canal_flannel(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_flannel", value)
 
     @property
     @pulumi.getter(name="canalFlexVol")
     def canal_flex_vol(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_flex_vol (string)
-        """
         return pulumi.get(self, "canal_flex_vol")
 
     @canal_flex_vol.setter
     def canal_flex_vol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_flex_vol", value)
 
     @property
     @pulumi.getter(name="canalNode")
     def canal_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_node (string)
-        """
         return pulumi.get(self, "canal_node")
 
     @canal_node.setter
     def canal_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_node", value)
 
     @property
     @pulumi.getter(name="certDownloader")
     def cert_downloader(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for cert_downloader (string)
-        """
         return pulumi.get(self, "cert_downloader")
 
     @cert_downloader.setter
     def cert_downloader(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_downloader", value)
 
     @property
     @pulumi.getter
     def coredns(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for coredns (string)
-        """
         return pulumi.get(self, "coredns")
 
     @coredns.setter
     def coredns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "coredns", value)
 
     @property
     @pulumi.getter(name="corednsAutoscaler")
     def coredns_autoscaler(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for coredns_autoscaler (string)
-        """
         return pulumi.get(self, "coredns_autoscaler")
 
     @coredns_autoscaler.setter
     def coredns_autoscaler(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "coredns_autoscaler", value)
 
     @property
     @pulumi.getter
     def dnsmasq(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for dnsmasq (string)
-        """
         return pulumi.get(self, "dnsmasq")
 
     @dnsmasq.setter
     def dnsmasq(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dnsmasq", value)
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @etcd.setter
     def etcd(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "etcd", value)
 
     @property
     @pulumi.getter
     def flannel(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for flannel (string)
-        """
         return pulumi.get(self, "flannel")
 
     @flannel.setter
     def flannel(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "flannel", value)
 
     @property
     @pulumi.getter(name="flannelCni")
     def flannel_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for flannel_cni (string)
-        """
         return pulumi.get(self, "flannel_cni")
 
     @flannel_cni.setter
     def flannel_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "flannel_cni", value)
 
     @property
@@ -6446,161 +5519,122 @@
     @ingress.setter
     def ingress(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ingress", value)
 
     @property
     @pulumi.getter(name="ingressBackend")
     def ingress_backend(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for ingress_backend (string)
-        """
         return pulumi.get(self, "ingress_backend")
 
     @ingress_backend.setter
     def ingress_backend(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ingress_backend", value)
 
     @property
     @pulumi.getter(name="kubeDns")
     def kube_dns(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns (string)
-        """
         return pulumi.get(self, "kube_dns")
 
     @kube_dns.setter
     def kube_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns", value)
 
     @property
     @pulumi.getter(name="kubeDnsAutoscaler")
     def kube_dns_autoscaler(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns_autoscaler (string)
-        """
         return pulumi.get(self, "kube_dns_autoscaler")
 
     @kube_dns_autoscaler.setter
     def kube_dns_autoscaler(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns_autoscaler", value)
 
     @property
     @pulumi.getter(name="kubeDnsSidecar")
     def kube_dns_sidecar(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns_sidecar (string)
-        """
         return pulumi.get(self, "kube_dns_sidecar")
 
     @kube_dns_sidecar.setter
     def kube_dns_sidecar(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns_sidecar", value)
 
     @property
     @pulumi.getter
     def kubernetes(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kubernetes (string)
-        """
         return pulumi.get(self, "kubernetes")
 
     @kubernetes.setter
     def kubernetes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes", value)
 
     @property
     @pulumi.getter(name="kubernetesServicesSidecar")
     def kubernetes_services_sidecar(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kubernetes_services_sidecar (string)
-        """
         return pulumi.get(self, "kubernetes_services_sidecar")
 
     @kubernetes_services_sidecar.setter
     def kubernetes_services_sidecar(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_services_sidecar", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for metrics_server (string)
-        """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metrics_server", value)
 
     @property
     @pulumi.getter(name="nginxProxy")
     def nginx_proxy(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for nginx_proxy (string)
-        """
         return pulumi.get(self, "nginx_proxy")
 
     @nginx_proxy.setter
     def nginx_proxy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nginx_proxy", value)
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for nodelocal (string)
-        """
         return pulumi.get(self, "nodelocal")
 
     @nodelocal.setter
     def nodelocal(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nodelocal", value)
 
     @property
     @pulumi.getter(name="podInfraContainer")
     def pod_infra_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for pod_infra_container (string)
-        """
         return pulumi.get(self, "pod_infra_container")
 
     @pod_infra_container.setter
     def pod_infra_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pod_infra_container", value)
 
     @property
     @pulumi.getter(name="weaveCni")
     def weave_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for weave_cni (string)
-        """
         return pulumi.get(self, "weave_cni")
 
     @weave_cni.setter
     def weave_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "weave_cni", value)
 
     @property
     @pulumi.getter(name="weaveNode")
     def weave_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for weave_node (string)
-        """
         return pulumi.get(self, "weave_node")
 
     @weave_node.setter
     def weave_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "weave_node", value)
 
     @property
     @pulumi.getter(name="windowsPodInfraContainer")
     def windows_pod_infra_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for windows_pod_infra_container (string)
-        """
         return pulumi.get(self, "windows_pod_infra_container")
 
     @windows_pod_infra_container.setter
     def windows_pod_infra_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "windows_pod_infra_container", value)
 
 
@@ -6609,22 +5643,14 @@
     def __init__(__self__, *,
                  etcd: Optional[pulumi.Input['ClusterServicesEtcdArgs']] = None,
                  kube_api: Optional[pulumi.Input['ClusterServicesKubeApiArgs']] = None,
                  kube_controller: Optional[pulumi.Input['ClusterServicesKubeControllerArgs']] = None,
                  kubelet: Optional[pulumi.Input['ClusterServicesKubeletArgs']] = None,
                  kubeproxy: Optional[pulumi.Input['ClusterServicesKubeproxyArgs']] = None,
                  scheduler: Optional[pulumi.Input['ClusterServicesSchedulerArgs']] = None):
-        """
-        :param pulumi.Input['ClusterServicesEtcdArgs'] etcd: Docker image for etcd (string)
-        :param pulumi.Input['ClusterServicesKubeApiArgs'] kube_api: Kube API options for RKE services (list maxitems:1)
-        :param pulumi.Input['ClusterServicesKubeControllerArgs'] kube_controller: Kube Controller options for RKE services (list maxitems:1)
-        :param pulumi.Input['ClusterServicesKubeletArgs'] kubelet: Kubelet options for RKE services (list maxitems:1)
-        :param pulumi.Input['ClusterServicesKubeproxyArgs'] kubeproxy: Kubeproxy options for RKE services (list maxitems:1)
-        :param pulumi.Input['ClusterServicesSchedulerArgs'] scheduler: Scheduler options for RKE services (list maxitems:1)
-        """
         if etcd is not None:
             pulumi.set(__self__, "etcd", etcd)
         if kube_api is not None:
             pulumi.set(__self__, "kube_api", kube_api)
         if kube_controller is not None:
             pulumi.set(__self__, "kube_controller", kube_controller)
         if kubelet is not None:
@@ -6633,77 +5659,59 @@
             pulumi.set(__self__, "kubeproxy", kubeproxy)
         if scheduler is not None:
             pulumi.set(__self__, "scheduler", scheduler)
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional[pulumi.Input['ClusterServicesEtcdArgs']]:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @etcd.setter
     def etcd(self, value: Optional[pulumi.Input['ClusterServicesEtcdArgs']]):
         pulumi.set(self, "etcd", value)
 
     @property
     @pulumi.getter(name="kubeApi")
     def kube_api(self) -> Optional[pulumi.Input['ClusterServicesKubeApiArgs']]:
-        """
-        Kube API options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kube_api")
 
     @kube_api.setter
     def kube_api(self, value: Optional[pulumi.Input['ClusterServicesKubeApiArgs']]):
         pulumi.set(self, "kube_api", value)
 
     @property
     @pulumi.getter(name="kubeController")
     def kube_controller(self) -> Optional[pulumi.Input['ClusterServicesKubeControllerArgs']]:
-        """
-        Kube Controller options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kube_controller")
 
     @kube_controller.setter
     def kube_controller(self, value: Optional[pulumi.Input['ClusterServicesKubeControllerArgs']]):
         pulumi.set(self, "kube_controller", value)
 
     @property
     @pulumi.getter
     def kubelet(self) -> Optional[pulumi.Input['ClusterServicesKubeletArgs']]:
-        """
-        Kubelet options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kubelet")
 
     @kubelet.setter
     def kubelet(self, value: Optional[pulumi.Input['ClusterServicesKubeletArgs']]):
         pulumi.set(self, "kubelet", value)
 
     @property
     @pulumi.getter
     def kubeproxy(self) -> Optional[pulumi.Input['ClusterServicesKubeproxyArgs']]:
-        """
-        Kubeproxy options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kubeproxy")
 
     @kubeproxy.setter
     def kubeproxy(self, value: Optional[pulumi.Input['ClusterServicesKubeproxyArgs']]):
         pulumi.set(self, "kubeproxy", value)
 
     @property
     @pulumi.getter
     def scheduler(self) -> Optional[pulumi.Input['ClusterServicesSchedulerArgs']]:
-        """
-        Scheduler options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "scheduler")
 
     @scheduler.setter
     def scheduler(self, value: Optional[pulumi.Input['ClusterServicesSchedulerArgs']]):
         pulumi.set(self, "scheduler", value)
 
 
@@ -6721,31 +5729,14 @@
                  gid: Optional[pulumi.Input[int]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  retention: Optional[pulumi.Input[str]] = None,
                  snapshot: Optional[pulumi.Input[bool]] = None,
                  uid: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input['ClusterServicesEtcdBackupConfigArgs'] backup_config: Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
-        :param pulumi.Input[str] cert: TLS certificate for etcd service (string)
-        :param pulumi.Input[str] creation: Creation option for etcd service (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_urls: External urls for etcd service (list)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[int] gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param pulumi.Input[str] retention: Retention for etcd backup. Default `6` (int)
-        :param pulumi.Input[bool] snapshot: Snapshot option for etcd service. Default `true` (bool)
-        :param pulumi.Input[int] uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if creation is not None:
@@ -6772,185 +5763,140 @@
             pulumi.set(__self__, "snapshot", snapshot)
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional[pulumi.Input['ClusterServicesEtcdBackupConfigArgs']]:
-        """
-        Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        """
         return pulumi.get(self, "backup_config")
 
     @backup_config.setter
     def backup_config(self, value: Optional[pulumi.Input['ClusterServicesEtcdBackupConfigArgs']]):
         pulumi.set(self, "backup_config", value)
 
     @property
     @pulumi.getter(name="caCert")
     def ca_cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS CA certificate for etcd service (string)
-        """
         return pulumi.get(self, "ca_cert")
 
     @ca_cert.setter
     def ca_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_cert", value)
 
     @property
     @pulumi.getter
     def cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS certificate for etcd service (string)
-        """
         return pulumi.get(self, "cert")
 
     @cert.setter
     def cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert", value)
 
     @property
     @pulumi.getter
     def creation(self) -> Optional[pulumi.Input[str]]:
-        """
-        Creation option for etcd service (string)
-        """
         return pulumi.get(self, "creation")
 
     @creation.setter
     def creation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "creation", value)
 
     @property
     @pulumi.getter(name="externalUrls")
     def external_urls(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        External urls for etcd service (list)
-        """
         return pulumi.get(self, "external_urls")
 
     @external_urls.setter
     def external_urls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_urls", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Extra arguments for scheduler service (map)
-        """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Extra binds for scheduler service (list)
-        """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Extra environment for scheduler service (list)
-        """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[pulumi.Input[int]]:
-        """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "gid")
 
     @gid.setter
     def gid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "gid", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[pulumi.Input[str]]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @retention.setter
     def retention(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "retention", value)
 
     @property
     @pulumi.getter
     def snapshot(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Snapshot option for etcd service. Default `true` (bool)
-        """
         return pulumi.get(self, "snapshot")
 
     @snapshot.setter
     def snapshot(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "snapshot", value)
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[pulumi.Input[int]]:
-        """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "uid")
 
     @uid.setter
     def uid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "uid", value)
 
 
@@ -6959,22 +5905,14 @@
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  interval_hours: Optional[pulumi.Input[int]] = None,
                  retention: Optional[pulumi.Input[int]] = None,
                  s3_backup_config: Optional[pulumi.Input['ClusterServicesEtcdBackupConfigS3BackupConfigArgs']] = None,
                  safe_timestamp: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        :param pulumi.Input[int] interval_hours: Interval hours for etcd backup. Default `12` (int)
-        :param pulumi.Input[int] retention: Retention for etcd backup. Default `6` (int)
-        :param pulumi.Input['ClusterServicesEtcdBackupConfigS3BackupConfigArgs'] s3_backup_config: S3 config options for etcd backup (list maxitems:1)
-        :param pulumi.Input[bool] safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param pulumi.Input[int] timeout: RKE node drain timeout (int)
-        """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
         if s3_backup_config is not None:
@@ -6983,77 +5921,59 @@
             pulumi.set(__self__, "safe_timestamp", safe_timestamp)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="intervalHours")
     def interval_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        Interval hours for etcd backup. Default `12` (int)
-        """
         return pulumi.get(self, "interval_hours")
 
     @interval_hours.setter
     def interval_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval_hours", value)
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[pulumi.Input[int]]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @retention.setter
     def retention(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retention", value)
 
     @property
     @pulumi.getter(name="s3BackupConfig")
     def s3_backup_config(self) -> Optional[pulumi.Input['ClusterServicesEtcdBackupConfigS3BackupConfigArgs']]:
-        """
-        S3 config options for etcd backup (list maxitems:1)
-        """
         return pulumi.get(self, "s3_backup_config")
 
     @s3_backup_config.setter
     def s3_backup_config(self, value: Optional[pulumi.Input['ClusterServicesEtcdBackupConfigS3BackupConfigArgs']]):
         pulumi.set(self, "s3_backup_config", value)
 
     @property
     @pulumi.getter(name="safeTimestamp")
     def safe_timestamp(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Safe timestamp for etcd backup. Default: `false` (bool)
-        """
         return pulumi.get(self, "safe_timestamp")
 
     @safe_timestamp.setter
     def safe_timestamp(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "safe_timestamp", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
@@ -7063,23 +5983,14 @@
                  access_key: Optional[pulumi.Input[str]] = None,
                  bucket_name: Optional[pulumi.Input[str]] = None,
                  custom_ca: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  folder: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] access_key: Access key for S3 service (string)
-        :param pulumi.Input[str] bucket_name: Bucket name for S3 service (string)
-        :param pulumi.Input[str] custom_ca: Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        :param pulumi.Input[str] endpoint: Endpoint for S3 service (string)
-        :param pulumi.Input[str] folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] secret_key: Secret key for S3 service (string)
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if custom_ca is not None:
             pulumi.set(__self__, "custom_ca", custom_ca)
         if endpoint is not None:
@@ -7090,89 +6001,68 @@
             pulumi.set(__self__, "region", region)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Access key for S3 service (string)
-        """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter(name="bucketName")
     def bucket_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Bucket name for S3 service (string)
-        """
         return pulumi.get(self, "bucket_name")
 
     @bucket_name.setter
     def bucket_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bucket_name", value)
 
     @property
     @pulumi.getter(name="customCa")
     def custom_ca(self) -> Optional[pulumi.Input[str]]:
-        """
-        Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        """
         return pulumi.get(self, "custom_ca")
 
     @custom_ca.setter
     def custom_ca(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_ca", value)
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
-        """
-        Endpoint for S3 service (string)
-        """
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[pulumi.Input[str]]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @folder.setter
     def folder(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "folder", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret key for S3 service (string)
-        """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
 
@@ -7190,31 +6080,14 @@
                  gid: Optional[pulumi.Input[int]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  key: Optional[pulumi.Input[str]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  retention: Optional[pulumi.Input[str]] = None,
                  snapshot: Optional[pulumi.Input[bool]] = None,
                  uid: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigArgs'] backup_config: Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        :param pulumi.Input[str] ca_cert: TLS CA certificate for etcd service (string)
-        :param pulumi.Input[str] cert: TLS certificate for etcd service (string)
-        :param pulumi.Input[str] creation: Creation option for etcd service (string)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] external_urls: External urls for etcd service (list)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[int] gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] key: TLS key for etcd service (string)
-        :param pulumi.Input[str] path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param pulumi.Input[str] retention: Retention for etcd backup. Default `6` (int)
-        :param pulumi.Input[bool] snapshot: Snapshot option for etcd service. Default `true` (bool)
-        :param pulumi.Input[int] uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if creation is not None:
@@ -7241,185 +6114,140 @@
             pulumi.set(__self__, "snapshot", snapshot)
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional[pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigArgs']]:
-        """
-        Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        """
         return pulumi.get(self, "backup_config")
 
     @backup_config.setter
     def backup_config(self, value: Optional[pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigArgs']]):
         pulumi.set(self, "backup_config", value)
 
     @property
     @pulumi.getter(name="caCert")
     def ca_cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS CA certificate for etcd service (string)
-        """
         return pulumi.get(self, "ca_cert")
 
     @ca_cert.setter
     def ca_cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ca_cert", value)
 
     @property
     @pulumi.getter
     def cert(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS certificate for etcd service (string)
-        """
         return pulumi.get(self, "cert")
 
     @cert.setter
     def cert(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert", value)
 
     @property
     @pulumi.getter
     def creation(self) -> Optional[pulumi.Input[str]]:
-        """
-        Creation option for etcd service (string)
-        """
         return pulumi.get(self, "creation")
 
     @creation.setter
     def creation(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "creation", value)
 
     @property
     @pulumi.getter(name="externalUrls")
     def external_urls(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        External urls for etcd service (list)
-        """
         return pulumi.get(self, "external_urls")
 
     @external_urls.setter
     def external_urls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "external_urls", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
-        """
-        Extra arguments for scheduler service (map)
-        """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Extra binds for scheduler service (list)
-        """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
-        """
-        Extra environment for scheduler service (list)
-        """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[pulumi.Input[int]]:
-        """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "gid")
 
     @gid.setter
     def gid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "gid", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter
     def key(self) -> Optional[pulumi.Input[str]]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @key.setter
     def key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "key", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[pulumi.Input[str]]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @retention.setter
     def retention(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "retention", value)
 
     @property
     @pulumi.getter
     def snapshot(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Snapshot option for etcd service. Default `true` (bool)
-        """
         return pulumi.get(self, "snapshot")
 
     @snapshot.setter
     def snapshot(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "snapshot", value)
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[pulumi.Input[int]]:
-        """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "uid")
 
     @uid.setter
     def uid(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "uid", value)
 
 
@@ -7428,22 +6256,14 @@
     def __init__(__self__, *,
                  enabled: Optional[pulumi.Input[bool]] = None,
                  interval_hours: Optional[pulumi.Input[int]] = None,
                  retention: Optional[pulumi.Input[int]] = None,
                  s3_backup_config: Optional[pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfigArgs']] = None,
                  safe_timestamp: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        :param pulumi.Input[int] interval_hours: Interval hours for etcd backup. Default `12` (int)
-        :param pulumi.Input[int] retention: Retention for etcd backup. Default `6` (int)
-        :param pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfigArgs'] s3_backup_config: S3 config options for etcd backup (list maxitems:1)
-        :param pulumi.Input[bool] safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param pulumi.Input[int] timeout: RKE node drain timeout (int)
-        """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
         if s3_backup_config is not None:
@@ -7452,77 +6272,59 @@
             pulumi.set(__self__, "safe_timestamp", safe_timestamp)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
     @property
     @pulumi.getter(name="intervalHours")
     def interval_hours(self) -> Optional[pulumi.Input[int]]:
-        """
-        Interval hours for etcd backup. Default `12` (int)
-        """
         return pulumi.get(self, "interval_hours")
 
     @interval_hours.setter
     def interval_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "interval_hours", value)
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[pulumi.Input[int]]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @retention.setter
     def retention(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "retention", value)
 
     @property
     @pulumi.getter(name="s3BackupConfig")
     def s3_backup_config(self) -> Optional[pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfigArgs']]:
-        """
-        S3 config options for etcd backup (list maxitems:1)
-        """
         return pulumi.get(self, "s3_backup_config")
 
     @s3_backup_config.setter
     def s3_backup_config(self, value: Optional[pulumi.Input['ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfigArgs']]):
         pulumi.set(self, "s3_backup_config", value)
 
     @property
     @pulumi.getter(name="safeTimestamp")
     def safe_timestamp(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Safe timestamp for etcd backup. Default: `false` (bool)
-        """
         return pulumi.get(self, "safe_timestamp")
 
     @safe_timestamp.setter
     def safe_timestamp(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "safe_timestamp", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
@@ -7532,23 +6334,14 @@
                  access_key: Optional[pulumi.Input[str]] = None,
                  bucket_name: Optional[pulumi.Input[str]] = None,
                  custom_ca: Optional[pulumi.Input[str]] = None,
                  endpoint: Optional[pulumi.Input[str]] = None,
                  folder: Optional[pulumi.Input[str]] = None,
                  region: Optional[pulumi.Input[str]] = None,
                  secret_key: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] access_key: Access key for S3 service (string)
-        :param pulumi.Input[str] bucket_name: Bucket name for S3 service (string)
-        :param pulumi.Input[str] custom_ca: Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        :param pulumi.Input[str] endpoint: Endpoint for S3 service (string)
-        :param pulumi.Input[str] folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param pulumi.Input[str] region: Region for S3 service (string)
-        :param pulumi.Input[str] secret_key: Secret key for S3 service (string)
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if custom_ca is not None:
             pulumi.set(__self__, "custom_ca", custom_ca)
         if endpoint is not None:
@@ -7559,89 +6352,68 @@
             pulumi.set(__self__, "region", region)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Access key for S3 service (string)
-        """
         return pulumi.get(self, "access_key")
 
     @access_key.setter
     def access_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_key", value)
 
     @property
     @pulumi.getter(name="bucketName")
     def bucket_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Bucket name for S3 service (string)
-        """
         return pulumi.get(self, "bucket_name")
 
     @bucket_name.setter
     def bucket_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bucket_name", value)
 
     @property
     @pulumi.getter(name="customCa")
     def custom_ca(self) -> Optional[pulumi.Input[str]]:
-        """
-        Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        """
         return pulumi.get(self, "custom_ca")
 
     @custom_ca.setter
     def custom_ca(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_ca", value)
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[pulumi.Input[str]]:
-        """
-        Endpoint for S3 service (string)
-        """
         return pulumi.get(self, "endpoint")
 
     @endpoint.setter
     def endpoint(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "endpoint", value)
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[pulumi.Input[str]]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @folder.setter
     def folder(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "folder", value)
 
     @property
     @pulumi.getter
     def region(self) -> Optional[pulumi.Input[str]]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @region.setter
     def region(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "region", value)
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secret key for S3 service (string)
-        """
         return pulumi.get(self, "secret_key")
 
     @secret_key.setter
     def secret_key(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "secret_key", value)
 
 
@@ -7657,26 +6429,22 @@
                  image: Optional[pulumi.Input[str]] = None,
                  pod_security_configuration: Optional[pulumi.Input[str]] = None,
                  pod_security_policy: Optional[pulumi.Input[bool]] = None,
                  secrets_encryption_config: Optional[pulumi.Input['ClusterServicesKubeApiSecretsEncryptionConfigArgs']] = None,
                  service_cluster_ip_range: Optional[pulumi.Input[str]] = None,
                  service_node_port_range: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
-        :param pulumi.Input['ClusterServicesKubeApiAuditLogArgs'] audit_log: K8s audit log configuration. (list maxitem: 1)
-        :param pulumi.Input['ClusterServicesKubeApiEventRateLimitArgs'] event_rate_limit: K8s event rate limit configuration. (list maxitem: 1)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[bool] always_pull_images: Enable/Disable AlwaysPullImages admissions plugin
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kube-api services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
         :param pulumi.Input[str] pod_security_configuration: Built-in PodSecurityPolicy (privileged or restricted)
-        :param pulumi.Input[bool] pod_security_policy: Pod Security Policy option for kube API service (bool)
-        :param pulumi.Input['ClusterServicesKubeApiSecretsEncryptionConfigArgs'] secrets_encryption_config: [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        :param pulumi.Input[str] service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
-        :param pulumi.Input[str] service_node_port_range: Service Node Port Range option for kube API service (string)
+        :param pulumi.Input[bool] pod_security_policy: Enabled/Disable PodSecurityPolicy
+        :param pulumi.Input[str] service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
+        :param pulumi.Input[str] service_node_port_range: Port range for services defined with NodePort type
         """
         if always_pull_images is not None:
             pulumi.set(__self__, "always_pull_images", always_pull_images)
         if audit_log is not None:
             pulumi.set(__self__, "audit_log", audit_log)
         if event_rate_limit is not None:
             pulumi.set(__self__, "event_rate_limit", event_rate_limit)
@@ -7699,88 +6467,79 @@
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
+        Enable/Disable AlwaysPullImages admissions plugin
         """
         return pulumi.get(self, "always_pull_images")
 
     @always_pull_images.setter
     def always_pull_images(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "always_pull_images", value)
 
     @property
     @pulumi.getter(name="auditLog")
     def audit_log(self) -> Optional[pulumi.Input['ClusterServicesKubeApiAuditLogArgs']]:
-        """
-        K8s audit log configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "audit_log")
 
     @audit_log.setter
     def audit_log(self, value: Optional[pulumi.Input['ClusterServicesKubeApiAuditLogArgs']]):
         pulumi.set(self, "audit_log", value)
 
     @property
     @pulumi.getter(name="eventRateLimit")
     def event_rate_limit(self) -> Optional[pulumi.Input['ClusterServicesKubeApiEventRateLimitArgs']]:
-        """
-        K8s event rate limit configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "event_rate_limit")
 
     @event_rate_limit.setter
     def event_rate_limit(self, value: Optional[pulumi.Input['ClusterServicesKubeApiEventRateLimitArgs']]):
         pulumi.set(self, "event_rate_limit", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-api services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
@@ -7795,91 +6554,78 @@
     def pod_security_configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pod_security_configuration", value)
 
     @property
     @pulumi.getter(name="podSecurityPolicy")
     def pod_security_policy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Pod Security Policy option for kube API service (bool)
+        Enabled/Disable PodSecurityPolicy
         """
         return pulumi.get(self, "pod_security_policy")
 
     @pod_security_policy.setter
     def pod_security_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pod_security_policy", value)
 
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional[pulumi.Input['ClusterServicesKubeApiSecretsEncryptionConfigArgs']]:
-        """
-        [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        """
         return pulumi.get(self, "secrets_encryption_config")
 
     @secrets_encryption_config.setter
     def secrets_encryption_config(self, value: Optional[pulumi.Input['ClusterServicesKubeApiSecretsEncryptionConfigArgs']]):
         pulumi.set(self, "secrets_encryption_config", value)
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @service_cluster_ip_range.setter
     def service_cluster_ip_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_cluster_ip_range", value)
 
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Node Port Range option for kube API service (string)
+        Port range for services defined with NodePort type
         """
         return pulumi.get(self, "service_node_port_range")
 
     @service_node_port_range.setter
     def service_node_port_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_node_port_range", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterServicesKubeApiAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input['ClusterServicesKubeApiAuditLogConfigurationArgs'] configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input['ClusterServicesKubeApiAuditLogConfigurationArgs']]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input['ClusterServicesKubeApiAuditLogConfigurationArgs']]):
         pulumi.set(self, "configuration", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
@@ -7888,22 +6634,14 @@
     def __init__(__self__, *,
                  format: Optional[pulumi.Input[str]] = None,
                  max_age: Optional[pulumi.Input[int]] = None,
                  max_backup: Optional[pulumi.Input[int]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  policy: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] format: Audit log format (string)
-        :param pulumi.Input[int] max_age: Audit log max age (int)
-        :param pulumi.Input[int] max_backup: Audit log max backup. Default: `10` (int)
-        :param pulumi.Input[int] max_size: Audit log max size. Default: `100` (int)
-        :param pulumi.Input[str] path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param pulumi.Input[str] policy: Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
         if max_size is not None:
@@ -7912,77 +6650,59 @@
             pulumi.set(__self__, "path", path)
         if policy is not None:
             pulumi.set(__self__, "policy", policy)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log format (string)
-        """
         return pulumi.get(self, "format")
 
     @format.setter
     def format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "format", value)
 
     @property
     @pulumi.getter(name="maxAge")
     def max_age(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max age (int)
-        """
         return pulumi.get(self, "max_age")
 
     @max_age.setter
     def max_age(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_age", value)
 
     @property
     @pulumi.getter(name="maxBackup")
     def max_backup(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max backup. Default: `10` (int)
-        """
         return pulumi.get(self, "max_backup")
 
     @max_backup.setter
     def max_backup(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_backup", value)
 
     @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max size. Default: `100` (int)
-        """
         return pulumi.get(self, "max_size")
 
     @max_size.setter
     def max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_size", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         return pulumi.get(self, "policy")
 
     @policy.setter
     def policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy", value)
 
 
@@ -7998,26 +6718,22 @@
                  image: Optional[pulumi.Input[str]] = None,
                  pod_security_configuration: Optional[pulumi.Input[str]] = None,
                  pod_security_policy: Optional[pulumi.Input[bool]] = None,
                  secrets_encryption_config: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs']] = None,
                  service_cluster_ip_range: Optional[pulumi.Input[str]] = None,
                  service_node_port_range: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[bool] always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
-        :param pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogArgs'] audit_log: K8s audit log configuration. (list maxitem: 1)
-        :param pulumi.Input['ClusterServicesKubeApiDeprecatedEventRateLimitArgs'] event_rate_limit: K8s event rate limit configuration. (list maxitem: 1)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[bool] always_pull_images: Enable/Disable AlwaysPullImages admissions plugin
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kube-api services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
         :param pulumi.Input[str] pod_security_configuration: Built-in PodSecurityPolicy (privileged or restricted)
-        :param pulumi.Input[bool] pod_security_policy: Pod Security Policy option for kube API service (bool)
-        :param pulumi.Input['ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs'] secrets_encryption_config: [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        :param pulumi.Input[str] service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
-        :param pulumi.Input[str] service_node_port_range: Service Node Port Range option for kube API service (string)
+        :param pulumi.Input[bool] pod_security_policy: Enabled/Disable PodSecurityPolicy
+        :param pulumi.Input[str] service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
+        :param pulumi.Input[str] service_node_port_range: Port range for services defined with NodePort type
         """
         if always_pull_images is not None:
             pulumi.set(__self__, "always_pull_images", always_pull_images)
         if audit_log is not None:
             pulumi.set(__self__, "audit_log", audit_log)
         if event_rate_limit is not None:
             pulumi.set(__self__, "event_rate_limit", event_rate_limit)
@@ -8040,88 +6756,79 @@
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
+        Enable/Disable AlwaysPullImages admissions plugin
         """
         return pulumi.get(self, "always_pull_images")
 
     @always_pull_images.setter
     def always_pull_images(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "always_pull_images", value)
 
     @property
     @pulumi.getter(name="auditLog")
     def audit_log(self) -> Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogArgs']]:
-        """
-        K8s audit log configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "audit_log")
 
     @audit_log.setter
     def audit_log(self, value: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogArgs']]):
         pulumi.set(self, "audit_log", value)
 
     @property
     @pulumi.getter(name="eventRateLimit")
     def event_rate_limit(self) -> Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedEventRateLimitArgs']]:
-        """
-        K8s event rate limit configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "event_rate_limit")
 
     @event_rate_limit.setter
     def event_rate_limit(self, value: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedEventRateLimitArgs']]):
         pulumi.set(self, "event_rate_limit", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-api services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
@@ -8136,91 +6843,78 @@
     def pod_security_configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pod_security_configuration", value)
 
     @property
     @pulumi.getter(name="podSecurityPolicy")
     def pod_security_policy(self) -> Optional[pulumi.Input[bool]]:
         """
-        Pod Security Policy option for kube API service (bool)
+        Enabled/Disable PodSecurityPolicy
         """
         return pulumi.get(self, "pod_security_policy")
 
     @pod_security_policy.setter
     def pod_security_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pod_security_policy", value)
 
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs']]:
-        """
-        [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        """
         return pulumi.get(self, "secrets_encryption_config")
 
     @secrets_encryption_config.setter
     def secrets_encryption_config(self, value: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs']]):
         pulumi.set(self, "secrets_encryption_config", value)
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @service_cluster_ip_range.setter
     def service_cluster_ip_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_cluster_ip_range", value)
 
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Node Port Range option for kube API service (string)
+        Port range for services defined with NodePort type
         """
         return pulumi.get(self, "service_node_port_range")
 
     @service_node_port_range.setter
     def service_node_port_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_node_port_range", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiDeprecatedAuditLogArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogConfigurationArgs']] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogConfigurationArgs'] configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogConfigurationArgs']]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input['ClusterServicesKubeApiDeprecatedAuditLogConfigurationArgs']]):
         pulumi.set(self, "configuration", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
@@ -8229,22 +6923,14 @@
     def __init__(__self__, *,
                  format: Optional[pulumi.Input[str]] = None,
                  max_age: Optional[pulumi.Input[int]] = None,
                  max_backup: Optional[pulumi.Input[int]] = None,
                  max_size: Optional[pulumi.Input[int]] = None,
                  path: Optional[pulumi.Input[str]] = None,
                  policy: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] format: Audit log format (string)
-        :param pulumi.Input[int] max_age: Audit log max age (int)
-        :param pulumi.Input[int] max_backup: Audit log max backup. Default: `10` (int)
-        :param pulumi.Input[int] max_size: Audit log max size. Default: `100` (int)
-        :param pulumi.Input[str] path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param pulumi.Input[str] policy: Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
         if max_size is not None:
@@ -8253,233 +6939,175 @@
             pulumi.set(__self__, "path", path)
         if policy is not None:
             pulumi.set(__self__, "policy", policy)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log format (string)
-        """
         return pulumi.get(self, "format")
 
     @format.setter
     def format(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "format", value)
 
     @property
     @pulumi.getter(name="maxAge")
     def max_age(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max age (int)
-        """
         return pulumi.get(self, "max_age")
 
     @max_age.setter
     def max_age(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_age", value)
 
     @property
     @pulumi.getter(name="maxBackup")
     def max_backup(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max backup. Default: `10` (int)
-        """
         return pulumi.get(self, "max_backup")
 
     @max_backup.setter
     def max_backup(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_backup", value)
 
     @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[pulumi.Input[int]]:
-        """
-        Audit log max size. Default: `100` (int)
-        """
         return pulumi.get(self, "max_size")
 
     @max_size.setter
     def max_size(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "max_size", value)
 
     @property
     @pulumi.getter
     def path(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @path.setter
     def path(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "path", value)
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[pulumi.Input[str]]:
-        """
-        Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         return pulumi.get(self, "policy")
 
     @policy.setter
     def policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "policy", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiDeprecatedEventRateLimitArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs:
     def __init__(__self__, *,
                  custom_config: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        """
         return pulumi.get(self, "custom_config")
 
     @custom_config.setter
     def custom_config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_config", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiEventRateLimitArgs:
     def __init__(__self__, *,
                  configuration: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[pulumi.Input[str]]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @configuration.setter
     def configuration(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "configuration", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
 @pulumi.input_type
 class ClusterServicesKubeApiSecretsEncryptionConfigArgs:
     def __init__(__self__, *,
                  custom_config: Optional[pulumi.Input[str]] = None,
                  enabled: Optional[pulumi.Input[bool]] = None):
-        """
-        :param pulumi.Input[str] custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        :param pulumi.Input[bool] enabled: Enable secrets encryption (bool)
-        """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[pulumi.Input[str]]:
-        """
-        Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        """
         return pulumi.get(self, "custom_config")
 
     @custom_config.setter
     def custom_config(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_config", value)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @enabled.setter
     def enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enabled", value)
 
 
@@ -8489,20 +7117,20 @@
                  cluster_cidr: Optional[pulumi.Input[str]] = None,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  service_cluster_ip_range: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
+        :param pulumi.Input[str] cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kube-controller service
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
+        :param pulumi.Input[str] image: Docker image of the kube-controller service
+        :param pulumi.Input[str] service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
         """
         if cluster_cidr is not None:
             pulumi.set(__self__, "cluster_cidr", cluster_cidr)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
@@ -8513,75 +7141,75 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @cluster_cidr.setter
     def cluster_cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_cidr", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-controller service
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kube-controller service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @service_cluster_ip_range.setter
     def service_cluster_ip_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_cluster_ip_range", value)
 
@@ -8592,20 +7220,20 @@
                  cluster_cidr: Optional[pulumi.Input[str]] = None,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  service_cluster_ip_range: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
+        :param pulumi.Input[str] cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kube-controller service
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
+        :param pulumi.Input[str] image: Docker image of the kube-controller service
+        :param pulumi.Input[str] service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
         """
         if cluster_cidr is not None:
             pulumi.set(__self__, "cluster_cidr", cluster_cidr)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
@@ -8616,75 +7244,75 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @cluster_cidr.setter
     def cluster_cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_cidr", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-controller service
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kube-controller service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[pulumi.Input[str]]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @service_cluster_ip_range.setter
     def service_cluster_ip_range(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "service_cluster_ip_range", value)
 
@@ -8693,69 +7321,69 @@
 class ClusterServicesKubeProxyDeprecatedArgs:
     def __init__(__self__, *,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kubeproxy services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the worker nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the worker nodes
+        :param pulumi.Input[str] image: Docker image of the kubeproxy service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubeproxy services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the worker nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubeproxy service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
@@ -8764,69 +7392,69 @@
 class ClusterServicesKubeSchedulerDeprecatedArgs:
     def __init__(__self__, *,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the scheduler services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
+        :param pulumi.Input[str] image: Docker image of the scheduler service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the scheduler services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the scheduler service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
@@ -8840,23 +7468,22 @@
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  fail_swap_on: Optional[pulumi.Input[bool]] = None,
                  generate_serving_certificate: Optional[pulumi.Input[bool]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  infra_container_image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param pulumi.Input[str] cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[bool] fail_swap_on: Enable or disable failing when swap on is not supported (bool)
-        :param pulumi.Input[bool] generate_serving_certificate: [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] infra_container_image: Infra container image for kubelet service (string)
+        :param pulumi.Input[str] cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param pulumi.Input[str] cluster_domain: (Computed) RKE k8s cluster domain (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kubelet services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the worker nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the nodes
+        :param pulumi.Input[bool] fail_swap_on: Fail if swap is enabled
+        :param pulumi.Input[str] image: Docker image of the kubelet service
+        :param pulumi.Input[str] infra_container_image: The image whose network/ipc namespaces containers in each pod will use
         """
         if cluster_dns_server is not None:
             pulumi.set(__self__, "cluster_dns_server", cluster_dns_server)
         if cluster_domain is not None:
             pulumi.set(__self__, "cluster_domain", cluster_domain)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -8873,111 +7500,108 @@
         if infra_container_image is not None:
             pulumi.set(__self__, "infra_container_image", infra_container_image)
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @cluster_dns_server.setter
     def cluster_dns_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_dns_server", value)
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @cluster_domain.setter
     def cluster_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_domain", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubelet services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter(name="failSwapOn")
     def fail_swap_on(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable or disable failing when swap on is not supported (bool)
+        Fail if swap is enabled
         """
         return pulumi.get(self, "fail_swap_on")
 
     @fail_swap_on.setter
     def fail_swap_on(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "fail_swap_on", value)
 
     @property
     @pulumi.getter(name="generateServingCertificate")
     def generate_serving_certificate(self) -> Optional[pulumi.Input[bool]]:
-        """
-        [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        """
         return pulumi.get(self, "generate_serving_certificate")
 
     @generate_serving_certificate.setter
     def generate_serving_certificate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "generate_serving_certificate", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubelet service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter(name="infraContainerImage")
     def infra_container_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Infra container image for kubelet service (string)
+        The image whose network/ipc namespaces containers in each pod will use
         """
         return pulumi.get(self, "infra_container_image")
 
     @infra_container_image.setter
     def infra_container_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "infra_container_image", value)
 
@@ -8991,23 +7615,22 @@
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  fail_swap_on: Optional[pulumi.Input[bool]] = None,
                  generate_serving_certificate: Optional[pulumi.Input[bool]] = None,
                  image: Optional[pulumi.Input[str]] = None,
                  infra_container_image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param pulumi.Input[str] cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[bool] fail_swap_on: Enable or disable failing when swap on is not supported (bool)
-        :param pulumi.Input[bool] generate_serving_certificate: [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
-        :param pulumi.Input[str] infra_container_image: Infra container image for kubelet service (string)
+        :param pulumi.Input[str] cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param pulumi.Input[str] cluster_domain: (Computed) RKE k8s cluster domain (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kubelet services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the worker nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the nodes
+        :param pulumi.Input[bool] fail_swap_on: Fail if swap is enabled
+        :param pulumi.Input[str] image: Docker image of the kubelet service
+        :param pulumi.Input[str] infra_container_image: The image whose network/ipc namespaces containers in each pod will use
         """
         if cluster_dns_server is not None:
             pulumi.set(__self__, "cluster_dns_server", cluster_dns_server)
         if cluster_domain is not None:
             pulumi.set(__self__, "cluster_domain", cluster_domain)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -9024,111 +7647,108 @@
         if infra_container_image is not None:
             pulumi.set(__self__, "infra_container_image", infra_container_image)
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @cluster_dns_server.setter
     def cluster_dns_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_dns_server", value)
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @cluster_domain.setter
     def cluster_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_domain", value)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubelet services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter(name="failSwapOn")
     def fail_swap_on(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable or disable failing when swap on is not supported (bool)
+        Fail if swap is enabled
         """
         return pulumi.get(self, "fail_swap_on")
 
     @fail_swap_on.setter
     def fail_swap_on(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "fail_swap_on", value)
 
     @property
     @pulumi.getter(name="generateServingCertificate")
     def generate_serving_certificate(self) -> Optional[pulumi.Input[bool]]:
-        """
-        [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        """
         return pulumi.get(self, "generate_serving_certificate")
 
     @generate_serving_certificate.setter
     def generate_serving_certificate(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "generate_serving_certificate", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubelet service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
     @property
     @pulumi.getter(name="infraContainerImage")
     def infra_container_image(self) -> Optional[pulumi.Input[str]]:
         """
-        Infra container image for kubelet service (string)
+        The image whose network/ipc namespaces containers in each pod will use
         """
         return pulumi.get(self, "infra_container_image")
 
     @infra_container_image.setter
     def infra_container_image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "infra_container_image", value)
 
@@ -9137,69 +7757,69 @@
 class ClusterServicesKubeproxyArgs:
     def __init__(__self__, *,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the kubeproxy services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the worker nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the worker nodes
+        :param pulumi.Input[str] image: Docker image of the kubeproxy service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubeproxy services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the worker nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubeproxy service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
@@ -9208,69 +7828,69 @@
 class ClusterServicesSchedulerArgs:
     def __init__(__self__, *,
                  extra_args: Optional[pulumi.Input[Mapping[str, Any]]] = None,
                  extra_binds: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  extra_envs: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  image: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments for scheduler service (map)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds for scheduler service (list)
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra environment for scheduler service (list)
-        :param pulumi.Input[str] image: Docker image for scheduler service (string)
+        :param pulumi.Input[Mapping[str, Any]] extra_args: Extra arguments that are added to the scheduler services
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_binds: Extra binds added to the controlplane nodes
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] extra_envs: Extra env added to the controlplane nodes
+        :param pulumi.Input[str] image: Docker image of the scheduler service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[pulumi.Input[Mapping[str, Any]]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the scheduler services
         """
         return pulumi.get(self, "extra_args")
 
     @extra_args.setter
     def extra_args(self, value: Optional[pulumi.Input[Mapping[str, Any]]]):
         pulumi.set(self, "extra_args", value)
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @extra_binds.setter
     def extra_binds(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_binds", value)
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @extra_envs.setter
     def extra_envs(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "extra_envs", value)
 
     @property
     @pulumi.getter
     def image(self) -> Optional[pulumi.Input[str]]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the scheduler service
         """
         return pulumi.get(self, "image")
 
     @image.setter
     def image(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "image", value)
 
@@ -9312,51 +7932,15 @@
                  nginx_proxy: Optional[pulumi.Input[str]] = None,
                  nodelocal: Optional[pulumi.Input[str]] = None,
                  pod_infra_container: Optional[pulumi.Input[str]] = None,
                  weave_cni: Optional[pulumi.Input[str]] = None,
                  weave_node: Optional[pulumi.Input[str]] = None,
                  windows_pod_infra_container: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] aci_cni_deploy_container: Docker image for aci_cni_deploy_container (string)
-        :param pulumi.Input[str] aci_controller_container: Docker image for aci_controller_container (string)
-        :param pulumi.Input[str] aci_host_container: Docker image for aci_host_container (string)
-        :param pulumi.Input[str] aci_mcast_container: Docker image for aci_mcast_container (string)
-        :param pulumi.Input[str] aci_opflex_container: Docker image for aci_opflex_container (string)
-        :param pulumi.Input[str] aci_ovs_container: Docker image for aci_ovs_container (string)
-        :param pulumi.Input[str] alpine: Docker image for alpine (string)
-        :param pulumi.Input[str] calico_cni: Docker image for calico_cni (string)
-        :param pulumi.Input[str] calico_controllers: Docker image for calico_controllers (string)
-        :param pulumi.Input[str] calico_ctl: Docker image for calico_ctl (string)
-        :param pulumi.Input[str] calico_flex_vol: Docker image for calico_flex_vol (string)
-        :param pulumi.Input[str] calico_node: Docker image for calico_node (string)
-        :param pulumi.Input[str] canal_cni: Docker image for canal_cni (string)
-        :param pulumi.Input[str] canal_flannel: Docker image for canal_flannel (string)
-        :param pulumi.Input[str] canal_flex_vol: Docker image for canal_flex_vol (string)
-        :param pulumi.Input[str] canal_node: Docker image for canal_node (string)
-        :param pulumi.Input[str] cert_downloader: Docker image for cert_downloader (string)
-        :param pulumi.Input[str] coredns: Docker image for coredns (string)
-        :param pulumi.Input[str] coredns_autoscaler: Docker image for coredns_autoscaler (string)
-        :param pulumi.Input[str] dnsmasq: Docker image for dnsmasq (string)
-        :param pulumi.Input[str] etcd: Docker image for etcd (string)
-        :param pulumi.Input[str] flannel: Docker image for flannel (string)
-        :param pulumi.Input[str] flannel_cni: Docker image for flannel_cni (string)
         :param pulumi.Input[str] ingress: RKE k8s cluster ingress controller configuration (list maxitems:1)
-        :param pulumi.Input[str] ingress_backend: Docker image for ingress_backend (string)
-        :param pulumi.Input[str] kube_dns: Docker image for kube_dns (string)
-        :param pulumi.Input[str] kube_dns_autoscaler: Docker image for kube_dns_autoscaler (string)
-        :param pulumi.Input[str] kube_dns_sidecar: Docker image for kube_dns_sidecar (string)
-        :param pulumi.Input[str] kubernetes: Docker image for kubernetes (string)
-        :param pulumi.Input[str] kubernetes_services_sidecar: Docker image for kubernetes_services_sidecar (string)
-        :param pulumi.Input[str] metrics_server: Docker image for metrics_server (string)
-        :param pulumi.Input[str] nginx_proxy: Docker image for nginx_proxy (string)
-        :param pulumi.Input[str] nodelocal: Docker image for nodelocal (string)
-        :param pulumi.Input[str] pod_infra_container: Docker image for pod_infra_container (string)
-        :param pulumi.Input[str] weave_cni: Docker image for weave_cni (string)
-        :param pulumi.Input[str] weave_node: Docker image for weave_node (string)
-        :param pulumi.Input[str] windows_pod_infra_container: Docker image for windows_pod_infra_container (string)
         """
         if aci_cni_deploy_container is not None:
             pulumi.set(__self__, "aci_cni_deploy_container", aci_cni_deploy_container)
         if aci_controller_container is not None:
             pulumi.set(__self__, "aci_controller_container", aci_controller_container)
         if aci_host_container is not None:
             pulumi.set(__self__, "aci_host_container", aci_host_container)
@@ -9428,281 +8012,212 @@
             pulumi.set(__self__, "weave_node", weave_node)
         if windows_pod_infra_container is not None:
             pulumi.set(__self__, "windows_pod_infra_container", windows_pod_infra_container)
 
     @property
     @pulumi.getter(name="aciCniDeployContainer")
     def aci_cni_deploy_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_cni_deploy_container (string)
-        """
         return pulumi.get(self, "aci_cni_deploy_container")
 
     @aci_cni_deploy_container.setter
     def aci_cni_deploy_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_cni_deploy_container", value)
 
     @property
     @pulumi.getter(name="aciControllerContainer")
     def aci_controller_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_controller_container (string)
-        """
         return pulumi.get(self, "aci_controller_container")
 
     @aci_controller_container.setter
     def aci_controller_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_controller_container", value)
 
     @property
     @pulumi.getter(name="aciHostContainer")
     def aci_host_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_host_container (string)
-        """
         return pulumi.get(self, "aci_host_container")
 
     @aci_host_container.setter
     def aci_host_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_host_container", value)
 
     @property
     @pulumi.getter(name="aciMcastContainer")
     def aci_mcast_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_mcast_container (string)
-        """
         return pulumi.get(self, "aci_mcast_container")
 
     @aci_mcast_container.setter
     def aci_mcast_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_mcast_container", value)
 
     @property
     @pulumi.getter(name="aciOpflexContainer")
     def aci_opflex_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_opflex_container (string)
-        """
         return pulumi.get(self, "aci_opflex_container")
 
     @aci_opflex_container.setter
     def aci_opflex_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_opflex_container", value)
 
     @property
     @pulumi.getter(name="aciOvsContainer")
     def aci_ovs_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for aci_ovs_container (string)
-        """
         return pulumi.get(self, "aci_ovs_container")
 
     @aci_ovs_container.setter
     def aci_ovs_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "aci_ovs_container", value)
 
     @property
     @pulumi.getter
     def alpine(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for alpine (string)
-        """
         return pulumi.get(self, "alpine")
 
     @alpine.setter
     def alpine(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "alpine", value)
 
     @property
     @pulumi.getter(name="calicoCni")
     def calico_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_cni (string)
-        """
         return pulumi.get(self, "calico_cni")
 
     @calico_cni.setter
     def calico_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_cni", value)
 
     @property
     @pulumi.getter(name="calicoControllers")
     def calico_controllers(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_controllers (string)
-        """
         return pulumi.get(self, "calico_controllers")
 
     @calico_controllers.setter
     def calico_controllers(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_controllers", value)
 
     @property
     @pulumi.getter(name="calicoCtl")
     def calico_ctl(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_ctl (string)
-        """
         return pulumi.get(self, "calico_ctl")
 
     @calico_ctl.setter
     def calico_ctl(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_ctl", value)
 
     @property
     @pulumi.getter(name="calicoFlexVol")
     def calico_flex_vol(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_flex_vol (string)
-        """
         return pulumi.get(self, "calico_flex_vol")
 
     @calico_flex_vol.setter
     def calico_flex_vol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_flex_vol", value)
 
     @property
     @pulumi.getter(name="calicoNode")
     def calico_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for calico_node (string)
-        """
         return pulumi.get(self, "calico_node")
 
     @calico_node.setter
     def calico_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "calico_node", value)
 
     @property
     @pulumi.getter(name="canalCni")
     def canal_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_cni (string)
-        """
         return pulumi.get(self, "canal_cni")
 
     @canal_cni.setter
     def canal_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_cni", value)
 
     @property
     @pulumi.getter(name="canalFlannel")
     def canal_flannel(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_flannel (string)
-        """
         return pulumi.get(self, "canal_flannel")
 
     @canal_flannel.setter
     def canal_flannel(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_flannel", value)
 
     @property
     @pulumi.getter(name="canalFlexVol")
     def canal_flex_vol(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_flex_vol (string)
-        """
         return pulumi.get(self, "canal_flex_vol")
 
     @canal_flex_vol.setter
     def canal_flex_vol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_flex_vol", value)
 
     @property
     @pulumi.getter(name="canalNode")
     def canal_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for canal_node (string)
-        """
         return pulumi.get(self, "canal_node")
 
     @canal_node.setter
     def canal_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "canal_node", value)
 
     @property
     @pulumi.getter(name="certDownloader")
     def cert_downloader(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for cert_downloader (string)
-        """
         return pulumi.get(self, "cert_downloader")
 
     @cert_downloader.setter
     def cert_downloader(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cert_downloader", value)
 
     @property
     @pulumi.getter
     def coredns(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for coredns (string)
-        """
         return pulumi.get(self, "coredns")
 
     @coredns.setter
     def coredns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "coredns", value)
 
     @property
     @pulumi.getter(name="corednsAutoscaler")
     def coredns_autoscaler(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for coredns_autoscaler (string)
-        """
         return pulumi.get(self, "coredns_autoscaler")
 
     @coredns_autoscaler.setter
     def coredns_autoscaler(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "coredns_autoscaler", value)
 
     @property
     @pulumi.getter
     def dnsmasq(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for dnsmasq (string)
-        """
         return pulumi.get(self, "dnsmasq")
 
     @dnsmasq.setter
     def dnsmasq(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dnsmasq", value)
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @etcd.setter
     def etcd(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "etcd", value)
 
     @property
     @pulumi.getter
     def flannel(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for flannel (string)
-        """
         return pulumi.get(self, "flannel")
 
     @flannel.setter
     def flannel(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "flannel", value)
 
     @property
     @pulumi.getter(name="flannelCni")
     def flannel_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for flannel_cni (string)
-        """
         return pulumi.get(self, "flannel_cni")
 
     @flannel_cni.setter
     def flannel_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "flannel_cni", value)
 
     @property
@@ -9716,232 +8231,175 @@
     @ingress.setter
     def ingress(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ingress", value)
 
     @property
     @pulumi.getter(name="ingressBackend")
     def ingress_backend(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for ingress_backend (string)
-        """
         return pulumi.get(self, "ingress_backend")
 
     @ingress_backend.setter
     def ingress_backend(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ingress_backend", value)
 
     @property
     @pulumi.getter(name="kubeDns")
     def kube_dns(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns (string)
-        """
         return pulumi.get(self, "kube_dns")
 
     @kube_dns.setter
     def kube_dns(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns", value)
 
     @property
     @pulumi.getter(name="kubeDnsAutoscaler")
     def kube_dns_autoscaler(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns_autoscaler (string)
-        """
         return pulumi.get(self, "kube_dns_autoscaler")
 
     @kube_dns_autoscaler.setter
     def kube_dns_autoscaler(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns_autoscaler", value)
 
     @property
     @pulumi.getter(name="kubeDnsSidecar")
     def kube_dns_sidecar(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kube_dns_sidecar (string)
-        """
         return pulumi.get(self, "kube_dns_sidecar")
 
     @kube_dns_sidecar.setter
     def kube_dns_sidecar(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kube_dns_sidecar", value)
 
     @property
     @pulumi.getter
     def kubernetes(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kubernetes (string)
-        """
         return pulumi.get(self, "kubernetes")
 
     @kubernetes.setter
     def kubernetes(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes", value)
 
     @property
     @pulumi.getter(name="kubernetesServicesSidecar")
     def kubernetes_services_sidecar(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for kubernetes_services_sidecar (string)
-        """
         return pulumi.get(self, "kubernetes_services_sidecar")
 
     @kubernetes_services_sidecar.setter
     def kubernetes_services_sidecar(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kubernetes_services_sidecar", value)
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for metrics_server (string)
-        """
         return pulumi.get(self, "metrics_server")
 
     @metrics_server.setter
     def metrics_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "metrics_server", value)
 
     @property
     @pulumi.getter(name="nginxProxy")
     def nginx_proxy(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for nginx_proxy (string)
-        """
         return pulumi.get(self, "nginx_proxy")
 
     @nginx_proxy.setter
     def nginx_proxy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nginx_proxy", value)
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for nodelocal (string)
-        """
         return pulumi.get(self, "nodelocal")
 
     @nodelocal.setter
     def nodelocal(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "nodelocal", value)
 
     @property
     @pulumi.getter(name="podInfraContainer")
     def pod_infra_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for pod_infra_container (string)
-        """
         return pulumi.get(self, "pod_infra_container")
 
     @pod_infra_container.setter
     def pod_infra_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "pod_infra_container", value)
 
     @property
     @pulumi.getter(name="weaveCni")
     def weave_cni(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for weave_cni (string)
-        """
         return pulumi.get(self, "weave_cni")
 
     @weave_cni.setter
     def weave_cni(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "weave_cni", value)
 
     @property
     @pulumi.getter(name="weaveNode")
     def weave_node(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for weave_node (string)
-        """
         return pulumi.get(self, "weave_node")
 
     @weave_node.setter
     def weave_node(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "weave_node", value)
 
     @property
     @pulumi.getter(name="windowsPodInfraContainer")
     def windows_pod_infra_container(self) -> Optional[pulumi.Input[str]]:
-        """
-        Docker image for windows_pod_infra_container (string)
-        """
         return pulumi.get(self, "windows_pod_infra_container")
 
     @windows_pod_infra_container.setter
     def windows_pod_infra_container(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "windows_pod_infra_container", value)
 
 
 @pulumi.input_type
 class ClusterUpgradeStrategyArgs:
     def __init__(__self__, *,
                  drain: Optional[pulumi.Input[bool]] = None,
                  drain_input: Optional[pulumi.Input['ClusterUpgradeStrategyDrainInputArgs']] = None,
                  max_unavailable_controlplane: Optional[pulumi.Input[str]] = None,
                  max_unavailable_worker: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[bool] drain: RKE drain nodes (bool)
-        :param pulumi.Input['ClusterUpgradeStrategyDrainInputArgs'] drain_input: RKE drain node input (list Maxitems: 1)
-        :param pulumi.Input[str] max_unavailable_controlplane: RKE max unavailable controlplane nodes (string)
-        :param pulumi.Input[str] max_unavailable_worker: RKE max unavailable worker nodes (string)
-        """
         if drain is not None:
             pulumi.set(__self__, "drain", drain)
         if drain_input is not None:
             pulumi.set(__self__, "drain_input", drain_input)
         if max_unavailable_controlplane is not None:
             pulumi.set(__self__, "max_unavailable_controlplane", max_unavailable_controlplane)
         if max_unavailable_worker is not None:
             pulumi.set(__self__, "max_unavailable_worker", max_unavailable_worker)
 
     @property
     @pulumi.getter
     def drain(self) -> Optional[pulumi.Input[bool]]:
-        """
-        RKE drain nodes (bool)
-        """
         return pulumi.get(self, "drain")
 
     @drain.setter
     def drain(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drain", value)
 
     @property
     @pulumi.getter(name="drainInput")
     def drain_input(self) -> Optional[pulumi.Input['ClusterUpgradeStrategyDrainInputArgs']]:
-        """
-        RKE drain node input (list Maxitems: 1)
-        """
         return pulumi.get(self, "drain_input")
 
     @drain_input.setter
     def drain_input(self, value: Optional[pulumi.Input['ClusterUpgradeStrategyDrainInputArgs']]):
         pulumi.set(self, "drain_input", value)
 
     @property
     @pulumi.getter(name="maxUnavailableControlplane")
     def max_unavailable_controlplane(self) -> Optional[pulumi.Input[str]]:
-        """
-        RKE max unavailable controlplane nodes (string)
-        """
         return pulumi.get(self, "max_unavailable_controlplane")
 
     @max_unavailable_controlplane.setter
     def max_unavailable_controlplane(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "max_unavailable_controlplane", value)
 
     @property
     @pulumi.getter(name="maxUnavailableWorker")
     def max_unavailable_worker(self) -> Optional[pulumi.Input[str]]:
-        """
-        RKE max unavailable worker nodes (string)
-        """
         return pulumi.get(self, "max_unavailable_worker")
 
     @max_unavailable_worker.setter
     def max_unavailable_worker(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "max_unavailable_worker", value)
 
 
@@ -9949,125 +8407,93 @@
 class ClusterUpgradeStrategyDrainInputArgs:
     def __init__(__self__, *,
                  delete_local_data: Optional[pulumi.Input[bool]] = None,
                  force: Optional[pulumi.Input[bool]] = None,
                  grace_period: Optional[pulumi.Input[int]] = None,
                  ignore_daemon_sets: Optional[pulumi.Input[bool]] = None,
                  timeout: Optional[pulumi.Input[int]] = None):
-        """
-        :param pulumi.Input[bool] delete_local_data: Delete RKE node local data (bool)
-        :param pulumi.Input[bool] force: Force RKE node drain (bool)
-        :param pulumi.Input[int] grace_period: RKE node drain grace period (int)
-        :param pulumi.Input[bool] ignore_daemon_sets: Ignore RKE daemon sets (bool)
-        :param pulumi.Input[int] timeout: RKE node drain timeout (int)
-        """
         if delete_local_data is not None:
             pulumi.set(__self__, "delete_local_data", delete_local_data)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if grace_period is not None:
             pulumi.set(__self__, "grace_period", grace_period)
         if ignore_daemon_sets is not None:
             pulumi.set(__self__, "ignore_daemon_sets", ignore_daemon_sets)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter(name="deleteLocalData")
     def delete_local_data(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Delete RKE node local data (bool)
-        """
         return pulumi.get(self, "delete_local_data")
 
     @delete_local_data.setter
     def delete_local_data(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "delete_local_data", value)
 
     @property
     @pulumi.getter
     def force(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Force RKE node drain (bool)
-        """
         return pulumi.get(self, "force")
 
     @force.setter
     def force(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "force", value)
 
     @property
     @pulumi.getter(name="gracePeriod")
     def grace_period(self) -> Optional[pulumi.Input[int]]:
-        """
-        RKE node drain grace period (int)
-        """
         return pulumi.get(self, "grace_period")
 
     @grace_period.setter
     def grace_period(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "grace_period", value)
 
     @property
     @pulumi.getter(name="ignoreDaemonSets")
     def ignore_daemon_sets(self) -> Optional[pulumi.Input[bool]]:
-        """
-        Ignore RKE daemon sets (bool)
-        """
         return pulumi.get(self, "ignore_daemon_sets")
 
     @ignore_daemon_sets.setter
     def ignore_daemon_sets(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "ignore_daemon_sets", value)
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[pulumi.Input[int]]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
     @timeout.setter
     def timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "timeout", value)
 
 
 @pulumi.input_type
 class ClusterWorkerHostArgs:
     def __init__(__self__, *,
                  address: Optional[pulumi.Input[str]] = None,
                  node_name: Optional[pulumi.Input[str]] = None):
-        """
-        :param pulumi.Input[str] address: Address ip for node (string)
-        :param pulumi.Input[str] node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[pulumi.Input[str]]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @address.setter
     def address(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "address", value)
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[pulumi.Input[str]]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
```

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/_utilities.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/cluster.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -805,17 +805,17 @@
         :param pulumi.Input['ClusterBastionHostArgs'] bastion_host: RKE k8s cluster bastion Host configuration (list maxitems:1)
         :param pulumi.Input[str] ca_crt: (Computed/Sensitive) RKE k8s cluster CA certificate (string)
         :param pulumi.Input[str] cert_dir: Specify a certificate dir path (string)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterCertificateArgs']]] certificates: (Computed/Sensitive) RKE k8s cluster certificates (string)
         :param pulumi.Input[str] client_cert: (Computed/Sensitive) RKE k8s cluster client certificate (string)
         :param pulumi.Input[str] client_key: (Computed/Sensitive) RKE k8s cluster client key (string)
         :param pulumi.Input['ClusterCloudProviderArgs'] cloud_provider: RKE k8s cluster cloud provider configuration [rke-cloud-providers](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/) (list maxitems:1)
-        :param pulumi.Input[str] cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param pulumi.Input[str] cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param pulumi.Input[str] cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        :param pulumi.Input[str] cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param pulumi.Input[str] cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param pulumi.Input[str] cluster_domain: (Computed) RKE k8s cluster domain (string)
         :param pulumi.Input[str] cluster_name: RKE k8s cluster name used in the kube config (string)
         :param pulumi.Input[str] cluster_yaml: RKE k8s cluster config yaml encoded. Provider arguments take precedence over this one (string)
         :param pulumi.Input[Sequence[pulumi.Input['ClusterControlPlaneHostArgs']]] control_plane_hosts: (Computed) RKE k8s cluster control plane nodes (list)
         :param pulumi.Input[bool] custom_certs: Use custom certificates from a cert dir (string)
         :param pulumi.Input[int] delay_on_creation: RKE k8s cluster delay on creation (int)
         :param pulumi.Input[bool] dind: Deploy RKE cluster on a dind environment. Default: `false` (bool)
         :param pulumi.Input[str] dind_dns_server: DinD RKE cluster dns (string)
@@ -1157,39 +1157,39 @@
     def cloud_provider(self, value: Optional[pulumi.Input['ClusterCloudProviderArgs']]):
         pulumi.set(self, "cloud_provider", value)
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @cluster_cidr.setter
     def cluster_cidr(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_cidr", value)
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @cluster_dns_server.setter
     def cluster_dns_server(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_dns_server", value)
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> Optional[pulumi.Input[str]]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @cluster_domain.setter
     def cluster_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "cluster_domain", value)
 
@@ -2083,17 +2083,17 @@
         :param pulumi.Input[pulumi.InputType['ClusterBastionHostArgs']] bastion_host: RKE k8s cluster bastion Host configuration (list maxitems:1)
         :param pulumi.Input[str] ca_crt: (Computed/Sensitive) RKE k8s cluster CA certificate (string)
         :param pulumi.Input[str] cert_dir: Specify a certificate dir path (string)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterCertificateArgs']]]] certificates: (Computed/Sensitive) RKE k8s cluster certificates (string)
         :param pulumi.Input[str] client_cert: (Computed/Sensitive) RKE k8s cluster client certificate (string)
         :param pulumi.Input[str] client_key: (Computed/Sensitive) RKE k8s cluster client key (string)
         :param pulumi.Input[pulumi.InputType['ClusterCloudProviderArgs']] cloud_provider: RKE k8s cluster cloud provider configuration [rke-cloud-providers](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/) (list maxitems:1)
-        :param pulumi.Input[str] cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param pulumi.Input[str] cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param pulumi.Input[str] cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        :param pulumi.Input[str] cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param pulumi.Input[str] cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param pulumi.Input[str] cluster_domain: (Computed) RKE k8s cluster domain (string)
         :param pulumi.Input[str] cluster_name: RKE k8s cluster name used in the kube config (string)
         :param pulumi.Input[str] cluster_yaml: RKE k8s cluster config yaml encoded. Provider arguments take precedence over this one (string)
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ClusterControlPlaneHostArgs']]]] control_plane_hosts: (Computed) RKE k8s cluster control plane nodes (list)
         :param pulumi.Input[bool] custom_certs: Use custom certificates from a cert dir (string)
         :param pulumi.Input[int] delay_on_creation: RKE k8s cluster delay on creation (int)
         :param pulumi.Input[bool] dind: Deploy RKE cluster on a dind environment. Default: `false` (bool)
         :param pulumi.Input[str] dind_dns_server: DinD RKE cluster dns (string)
@@ -2304,31 +2304,31 @@
         """
         return pulumi.get(self, "cloud_provider")
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> pulumi.Output[str]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> pulumi.Output[str]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> pulumi.Output[str]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @property
     @pulumi.getter(name="clusterName")
     def cluster_name(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/config/vars.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/outputs.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/outputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -102,46 +102,46 @@
 @pulumi.output_type
 class ClusterAuthentication(dict):
     def __init__(__self__, *,
                  sans: Optional[Sequence[str]] = None,
                  strategy: Optional[str] = None,
                  webhook: Optional['outputs.ClusterAuthenticationWebhook'] = None):
         """
-        :param Sequence[str] sans: List of additional hostnames and IPs to include in the api server PKI cert (list)
-        :param str strategy: Authentication strategy that will be used in RKE k8s cluster. Default: `x509` (string)
-        :param 'ClusterAuthenticationWebhookArgs' webhook: Webhook configuration options (list maxitem: 1)
+        :param Sequence[str] sans: List of additional hostnames and IPs to include in the api server PKI cert
+        :param str strategy: Authentication strategy that will be used in RKE k8s cluster
+        :param 'ClusterAuthenticationWebhookArgs' webhook: Webhook configuration options
         """
         if sans is not None:
             pulumi.set(__self__, "sans", sans)
         if strategy is not None:
             pulumi.set(__self__, "strategy", strategy)
         if webhook is not None:
             pulumi.set(__self__, "webhook", webhook)
 
     @property
     @pulumi.getter
     def sans(self) -> Optional[Sequence[str]]:
         """
-        List of additional hostnames and IPs to include in the api server PKI cert (list)
+        List of additional hostnames and IPs to include in the api server PKI cert
         """
         return pulumi.get(self, "sans")
 
     @property
     @pulumi.getter
     def strategy(self) -> Optional[str]:
         """
-        Authentication strategy that will be used in RKE k8s cluster. Default: `x509` (string)
+        Authentication strategy that will be used in RKE k8s cluster
         """
         return pulumi.get(self, "strategy")
 
     @property
     @pulumi.getter
     def webhook(self) -> Optional['outputs.ClusterAuthenticationWebhook']:
         """
-        Webhook configuration options (list maxitem: 1)
+        Webhook configuration options
         """
         return pulumi.get(self, "webhook")
 
 
 @pulumi.output_type
 class ClusterAuthenticationWebhook(dict):
     @staticmethod
@@ -163,66 +163,62 @@
         ClusterAuthenticationWebhook.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  cache_timeout: Optional[str] = None,
                  config_file: Optional[str] = None):
         """
-        :param str cache_timeout: Controls how long to cache authentication decisions (string)
-        :param str config_file: Multiline string that represent a custom webhook config file (string)
+        :param str cache_timeout: Controls how long to cache authentication decisions
+        :param str config_file: Multiline string that represent a custom webhook config file
         """
         if cache_timeout is not None:
             pulumi.set(__self__, "cache_timeout", cache_timeout)
         if config_file is not None:
             pulumi.set(__self__, "config_file", config_file)
 
     @property
     @pulumi.getter(name="cacheTimeout")
     def cache_timeout(self) -> Optional[str]:
         """
-        Controls how long to cache authentication decisions (string)
+        Controls how long to cache authentication decisions
         """
         return pulumi.get(self, "cache_timeout")
 
     @property
     @pulumi.getter(name="configFile")
     def config_file(self) -> Optional[str]:
         """
-        Multiline string that represent a custom webhook config file (string)
+        Multiline string that represent a custom webhook config file
         """
         return pulumi.get(self, "config_file")
 
 
 @pulumi.output_type
 class ClusterAuthorization(dict):
     def __init__(__self__, *,
                  mode: Optional[str] = None,
                  options: Optional[Mapping[str, Any]] = None):
         """
-        :param str mode: RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
-        :param Mapping[str, Any] options: Network provider options (map)
+        :param Mapping[str, Any] options: Authorization mode options
         """
         if mode is not None:
             pulumi.set(__self__, "mode", mode)
         if options is not None:
             pulumi.set(__self__, "options", options)
 
     @property
     @pulumi.getter
     def mode(self) -> Optional[str]:
-        """
-        RKE mode for authorization. `rbac` and `none` modes are available. Default `rbac` (string)
-        """
         return pulumi.get(self, "mode")
 
     @property
     @pulumi.getter
     def options(self) -> Optional[Mapping[str, Any]]:
         """
-        Network provider options (map)
+        Authorization mode options
         """
         return pulumi.get(self, "options")
 
 
 @pulumi.output_type
 class ClusterBastionHost(dict):
     @staticmethod
@@ -259,22 +255,22 @@
                  port: Optional[str] = None,
                  ssh_agent_auth: Optional[bool] = None,
                  ssh_cert: Optional[str] = None,
                  ssh_cert_path: Optional[str] = None,
                  ssh_key: Optional[str] = None,
                  ssh_key_path: Optional[str] = None):
         """
-        :param str address: Address ip for node (string)
-        :param str user: Registry user (string)
-        :param bool ignore_proxy_env_vars: Ignore proxy env vars at Bastion Host? Default: `false` (bool)
-        :param str port: Port used for SSH communication (string)
+        :param str address: Address of Bastion Host
+        :param str user: SSH User to Bastion Host
+        :param bool ignore_proxy_env_vars: Ignore proxy env vars at Bastion Host?
+        :param str port: SSH Port of Bastion Host
         :param bool ssh_agent_auth: SSH Agent Auth enable (bool)
-        :param str ssh_cert: SSH Certificate (string)
+        :param str ssh_cert: SSH Certificate Key
         :param str ssh_cert_path: SSH Certificate Path (string)
-        :param str ssh_key: SSH Private Key (string)
+        :param str ssh_key: SSH Private Key
         :param str ssh_key_path: SSH Private Key Path (string)
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "user", user)
         if ignore_proxy_env_vars is not None:
             pulumi.set(__self__, "ignore_proxy_env_vars", ignore_proxy_env_vars)
         if port is not None:
@@ -290,39 +286,39 @@
         if ssh_key_path is not None:
             pulumi.set(__self__, "ssh_key_path", ssh_key_path)
 
     @property
     @pulumi.getter
     def address(self) -> str:
         """
-        Address ip for node (string)
+        Address of Bastion Host
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def user(self) -> str:
         """
-        Registry user (string)
+        SSH User to Bastion Host
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="ignoreProxyEnvVars")
     def ignore_proxy_env_vars(self) -> Optional[bool]:
         """
-        Ignore proxy env vars at Bastion Host? Default: `false` (bool)
+        Ignore proxy env vars at Bastion Host?
         """
         return pulumi.get(self, "ignore_proxy_env_vars")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
         """
-        Port used for SSH communication (string)
+        SSH Port of Bastion Host
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="sshAgentAuth")
     def ssh_agent_auth(self) -> Optional[bool]:
         """
@@ -330,15 +326,15 @@
         """
         return pulumi.get(self, "ssh_agent_auth")
 
     @property
     @pulumi.getter(name="sshCert")
     def ssh_cert(self) -> Optional[str]:
         """
-        SSH Certificate (string)
+        SSH Certificate Key
         """
         return pulumi.get(self, "ssh_cert")
 
     @property
     @pulumi.getter(name="sshCertPath")
     def ssh_cert_path(self) -> Optional[str]:
         """
@@ -346,15 +342,15 @@
         """
         return pulumi.get(self, "ssh_cert_path")
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[str]:
         """
-        SSH Private Key (string)
+        SSH Private Key
         """
         return pulumi.get(self, "ssh_key")
 
     @property
     @pulumi.getter(name="sshKeyPath")
     def ssh_key_path(self) -> Optional[str]:
         """
@@ -406,17 +402,14 @@
                  key_env_name: Optional[str] = None,
                  key_path: Optional[str] = None,
                  name: Optional[str] = None,
                  ou_name: Optional[str] = None,
                  path: Optional[str] = None):
         """
         :param str id: (Computed) The ID of the resource (string)
-        :param str key: TLS key for etcd service (string)
-        :param str name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param str path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
         """
         if certificate is not None:
             pulumi.set(__self__, "certificate", certificate)
         if common_name is not None:
             pulumi.set(__self__, "common_name", common_name)
         if config is not None:
             pulumi.set(__self__, "config", config)
@@ -478,17 +471,14 @@
         (Computed) The ID of the resource (string)
         """
         return pulumi.get(self, "id")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter(name="keyEnvName")
     def key_env_name(self) -> Optional[str]:
         return pulumi.get(self, "key_env_name")
 
@@ -496,30 +486,24 @@
     @pulumi.getter(name="keyPath")
     def key_path(self) -> Optional[str]:
         return pulumi.get(self, "key_path")
 
     @property
     @pulumi.getter
     def name(self) -> Optional[str]:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="ouName")
     def ou_name(self) -> Optional[str]:
         return pulumi.get(self, "ou_name")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
 
 @pulumi.output_type
 class ClusterCloudProvider(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -565,25 +549,19 @@
                  custom_cloud_config: Optional[str] = None,
                  custom_cloud_provider: Optional[str] = None,
                  openstack_cloud_config: Optional['outputs.ClusterCloudProviderOpenstackCloudConfig'] = None,
                  openstack_cloud_provider: Optional['outputs.ClusterCloudProviderOpenstackCloudProvider'] = None,
                  vsphere_cloud_config: Optional['outputs.ClusterCloudProviderVsphereCloudConfig'] = None,
                  vsphere_cloud_provider: Optional['outputs.ClusterCloudProviderVsphereCloudProvider'] = None):
         """
-        :param str name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param 'ClusterCloudProviderAwsCloudConfigArgs' aws_cloud_config: Use aws_cloud_provider instead
-        :param 'ClusterCloudProviderAwsCloudProviderArgs' aws_cloud_provider: AWS Cloud Provider config [rke-aws-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/aws/) (list maxitems:1)
-        :param 'ClusterCloudProviderAzureCloudConfigArgs' azure_cloud_config: Use azure_cloud_provider instead
-        :param 'ClusterCloudProviderAzureCloudProviderArgs' azure_cloud_provider: Azure Cloud Provider config [rke-azure-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/azure/) (list maxitems:1)
-        :param str custom_cloud_config: Use custom_cloud_provider instead
-        :param str custom_cloud_provider: Custom Cloud Provider config (string)
-        :param 'ClusterCloudProviderOpenstackCloudConfigArgs' openstack_cloud_config: Use openstack_cloud_provider instead
-        :param 'ClusterCloudProviderOpenstackCloudProviderArgs' openstack_cloud_provider: Openstack Cloud Provider config [rke-openstack-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/openstack/) (list maxitems:1)
-        :param 'ClusterCloudProviderVsphereCloudConfigArgs' vsphere_cloud_config: Use vsphere_cloud_provider instead
-        :param 'ClusterCloudProviderVsphereCloudProviderArgs' vsphere_cloud_provider: Vsphere Cloud Provider config [rke-vsphere-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/vsphere/) Extra argument `name` is required on `virtual_center` configuration. (list maxitems:1)
+        :param 'ClusterCloudProviderAwsCloudProviderArgs' aws_cloud_provider: AWS Cloud Provider config
+        :param 'ClusterCloudProviderAzureCloudProviderArgs' azure_cloud_provider: Azure Cloud Provider config
+        :param str custom_cloud_provider: Custom Cloud Provider config
+        :param 'ClusterCloudProviderOpenstackCloudProviderArgs' openstack_cloud_provider: Openstack Cloud Provider config
+        :param 'ClusterCloudProviderVsphereCloudProviderArgs' vsphere_cloud_provider: Vsphere Cloud Provider config
         """
         pulumi.set(__self__, "name", name)
         if aws_cloud_config is not None:
             pulumi.set(__self__, "aws_cloud_config", aws_cloud_config)
         if aws_cloud_provider is not None:
             pulumi.set(__self__, "aws_cloud_provider", aws_cloud_provider)
         if azure_cloud_config is not None:
@@ -602,111 +580,93 @@
             pulumi.set(__self__, "vsphere_cloud_config", vsphere_cloud_config)
         if vsphere_cloud_provider is not None:
             pulumi.set(__self__, "vsphere_cloud_provider", vsphere_cloud_provider)
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="awsCloudConfig")
     def aws_cloud_config(self) -> Optional['outputs.ClusterCloudProviderAwsCloudConfig']:
-        """
-        Use aws_cloud_provider instead
-        """
         warnings.warn("""Use aws_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""aws_cloud_config is deprecated: Use aws_cloud_provider instead""")
 
         return pulumi.get(self, "aws_cloud_config")
 
     @property
     @pulumi.getter(name="awsCloudProvider")
     def aws_cloud_provider(self) -> Optional['outputs.ClusterCloudProviderAwsCloudProvider']:
         """
-        AWS Cloud Provider config [rke-aws-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/aws/) (list maxitems:1)
+        AWS Cloud Provider config
         """
         return pulumi.get(self, "aws_cloud_provider")
 
     @property
     @pulumi.getter(name="azureCloudConfig")
     def azure_cloud_config(self) -> Optional['outputs.ClusterCloudProviderAzureCloudConfig']:
-        """
-        Use azure_cloud_provider instead
-        """
         warnings.warn("""Use azure_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""azure_cloud_config is deprecated: Use azure_cloud_provider instead""")
 
         return pulumi.get(self, "azure_cloud_config")
 
     @property
     @pulumi.getter(name="azureCloudProvider")
     def azure_cloud_provider(self) -> Optional['outputs.ClusterCloudProviderAzureCloudProvider']:
         """
-        Azure Cloud Provider config [rke-azure-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/azure/) (list maxitems:1)
+        Azure Cloud Provider config
         """
         return pulumi.get(self, "azure_cloud_provider")
 
     @property
     @pulumi.getter(name="customCloudConfig")
     def custom_cloud_config(self) -> Optional[str]:
-        """
-        Use custom_cloud_provider instead
-        """
         warnings.warn("""Use custom_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""custom_cloud_config is deprecated: Use custom_cloud_provider instead""")
 
         return pulumi.get(self, "custom_cloud_config")
 
     @property
     @pulumi.getter(name="customCloudProvider")
     def custom_cloud_provider(self) -> Optional[str]:
         """
-        Custom Cloud Provider config (string)
+        Custom Cloud Provider config
         """
         return pulumi.get(self, "custom_cloud_provider")
 
     @property
     @pulumi.getter(name="openstackCloudConfig")
     def openstack_cloud_config(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudConfig']:
-        """
-        Use openstack_cloud_provider instead
-        """
         warnings.warn("""Use openstack_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""openstack_cloud_config is deprecated: Use openstack_cloud_provider instead""")
 
         return pulumi.get(self, "openstack_cloud_config")
 
     @property
     @pulumi.getter(name="openstackCloudProvider")
     def openstack_cloud_provider(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudProvider']:
         """
-        Openstack Cloud Provider config [rke-openstack-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/openstack/) (list maxitems:1)
+        Openstack Cloud Provider config
         """
         return pulumi.get(self, "openstack_cloud_provider")
 
     @property
     @pulumi.getter(name="vsphereCloudConfig")
     def vsphere_cloud_config(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudConfig']:
-        """
-        Use vsphere_cloud_provider instead
-        """
         warnings.warn("""Use vsphere_cloud_provider instead""", DeprecationWarning)
         pulumi.log.warn("""vsphere_cloud_config is deprecated: Use vsphere_cloud_provider instead""")
 
         return pulumi.get(self, "vsphere_cloud_config")
 
     @property
     @pulumi.getter(name="vsphereCloudProvider")
     def vsphere_cloud_provider(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudProvider']:
         """
-        Vsphere Cloud Provider config [rke-vsphere-cloud-provider](https://rancher.com/docs/rke/latest/en/config-options/cloud-providers/vsphere/) Extra argument `name` is required on `virtual_center` configuration. (list maxitems:1)
+        Vsphere Cloud Provider config
         """
         return pulumi.get(self, "vsphere_cloud_provider")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudConfig(dict):
     @staticmethod
@@ -727,37 +687,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderAwsCloudConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  global_: Optional['outputs.ClusterCloudProviderAwsCloudConfigGlobal'] = None,
                  service_overrides: Optional[Sequence['outputs.ClusterCloudProviderAwsCloudConfigServiceOverride']] = None):
-        """
-        :param 'ClusterCloudProviderAwsCloudConfigGlobalArgs' global_: (list maxitems:1)
-        :param Sequence['ClusterCloudProviderAwsCloudConfigServiceOverrideArgs'] service_overrides: (list)
-        """
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if service_overrides is not None:
             pulumi.set(__self__, "service_overrides", service_overrides)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional['outputs.ClusterCloudProviderAwsCloudConfigGlobal']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter(name="serviceOverrides")
     def service_overrides(self) -> Optional[Sequence['outputs.ClusterCloudProviderAwsCloudConfigServiceOverride']]:
-        """
-        (list)
-        """
         return pulumi.get(self, "service_overrides")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudConfigGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -798,24 +748,24 @@
                  kubernetes_cluster_tag: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  route_table_id: Optional[str] = None,
                  subnet_id: Optional[str] = None,
                  vpc: Optional[str] = None,
                  zone: Optional[str] = None):
         """
-        :param bool disable_security_group_ingress: Disables the automatic ingress creation. Default `false` (bool)
-        :param bool disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
-        :param str elb_security_group: Use these ELB security groups instead create new (string)
-        :param str kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources (string)
-        :param str kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources (string)
-        :param str role_arn: IAM role to assume when interaction with AWS APIs (string)
-        :param str route_table_id: Enables using a specific RouteTable (string)
-        :param str subnet_id: (string)
-        :param str vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
-        :param str zone: The AWS zone (string)
+        :param bool disable_security_group_ingress: Disables the automatic ingress creation
+        :param bool disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped
+        :param str elb_security_group: Use these ELB security groups instead create new
+        :param str kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources
+        :param str kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources
+        :param str role_arn: IAM role to assume when interaction with AWS APIs
+        :param str route_table_id: Enables using a specific RouteTable
+        :param str subnet_id: Enables using a specific subnet to use for ELB's
+        :param str vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
+        :param str zone: The AWS zone
         """
         if disable_security_group_ingress is not None:
             pulumi.set(__self__, "disable_security_group_ingress", disable_security_group_ingress)
         if disable_strict_zone_check is not None:
             pulumi.set(__self__, "disable_strict_zone_check", disable_strict_zone_check)
         if elb_security_group is not None:
             pulumi.set(__self__, "elb_security_group", elb_security_group)
@@ -834,87 +784,87 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="disableSecurityGroupIngress")
     def disable_security_group_ingress(self) -> Optional[bool]:
         """
-        Disables the automatic ingress creation. Default `false` (bool)
+        Disables the automatic ingress creation
         """
         return pulumi.get(self, "disable_security_group_ingress")
 
     @property
     @pulumi.getter(name="disableStrictZoneCheck")
     def disable_strict_zone_check(self) -> Optional[bool]:
         """
-        Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
+        Setting this to true will disable the check and provide a warning that the check was skipped
         """
         return pulumi.get(self, "disable_strict_zone_check")
 
     @property
     @pulumi.getter(name="elbSecurityGroup")
     def elb_security_group(self) -> Optional[str]:
         """
-        Use these ELB security groups instead create new (string)
+        Use these ELB security groups instead create new
         """
         return pulumi.get(self, "elb_security_group")
 
     @property
     @pulumi.getter(name="kubernetesClusterId")
     def kubernetes_cluster_id(self) -> Optional[str]:
         """
-        The cluster id we'll use to identify our cluster resources (string)
+        The cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_id")
 
     @property
     @pulumi.getter(name="kubernetesClusterTag")
     def kubernetes_cluster_tag(self) -> Optional[str]:
         """
-        Legacy cluster id we'll use to identify our cluster resources (string)
+        Legacy cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_tag")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
         """
-        IAM role to assume when interaction with AWS APIs (string)
+        IAM role to assume when interaction with AWS APIs
         """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="routeTableId")
     def route_table_id(self) -> Optional[str]:
         """
-        Enables using a specific RouteTable (string)
+        Enables using a specific RouteTable
         """
         return pulumi.get(self, "route_table_id")
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[str]:
         """
-        (string)
+        Enables using a specific subnet to use for ELB's
         """
         return pulumi.get(self, "subnet_id")
 
     @property
     @pulumi.getter
     def vpc(self) -> Optional[str]:
         """
-        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
+        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
         """
         return pulumi.get(self, "vpc")
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[str]:
         """
-        The AWS zone (string)
+        The AWS zone
         """
         return pulumi.get(self, "zone")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudConfigServiceOverride(dict):
     @staticmethod
@@ -942,23 +892,14 @@
                  service: str,
                  key: Optional[str] = None,
                  region: Optional[str] = None,
                  signing_method: Optional[str] = None,
                  signing_name: Optional[str] = None,
                  signing_region: Optional[str] = None,
                  url: Optional[str] = None):
-        """
-        :param str service: (string)
-        :param str key: TLS key for etcd service (string)
-        :param str region: Region for S3 service (string)
-        :param str signing_method: (string)
-        :param str signing_name: (string)
-        :param str signing_region: (string)
-        :param str url: Registry URL (string)
-        """
         pulumi.set(__self__, "service", service)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if signing_method is not None:
             pulumi.set(__self__, "signing_method", signing_method)
@@ -968,68 +909,47 @@
             pulumi.set(__self__, "signing_region", signing_region)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def service(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        TLS key for etcd service (string)
-        """
         warnings.warn("""Use service instead""", DeprecationWarning)
         pulumi.log.warn("""key is deprecated: Use service instead""")
 
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="signingMethod")
     def signing_method(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_method")
 
     @property
     @pulumi.getter(name="signingName")
     def signing_name(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_name")
 
     @property
     @pulumi.getter(name="signingRegion")
     def signing_region(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_region")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
-        """
-        Registry URL (string)
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudProvider(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1049,37 +969,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderAwsCloudProvider.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  global_: Optional['outputs.ClusterCloudProviderAwsCloudProviderGlobal'] = None,
                  service_overrides: Optional[Sequence['outputs.ClusterCloudProviderAwsCloudProviderServiceOverride']] = None):
-        """
-        :param 'ClusterCloudProviderAwsCloudProviderGlobalArgs' global_: (list maxitems:1)
-        :param Sequence['ClusterCloudProviderAwsCloudProviderServiceOverrideArgs'] service_overrides: (list)
-        """
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if service_overrides is not None:
             pulumi.set(__self__, "service_overrides", service_overrides)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional['outputs.ClusterCloudProviderAwsCloudProviderGlobal']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter(name="serviceOverrides")
     def service_overrides(self) -> Optional[Sequence['outputs.ClusterCloudProviderAwsCloudProviderServiceOverride']]:
-        """
-        (list)
-        """
         return pulumi.get(self, "service_overrides")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudProviderGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1120,24 +1030,24 @@
                  kubernetes_cluster_tag: Optional[str] = None,
                  role_arn: Optional[str] = None,
                  route_table_id: Optional[str] = None,
                  subnet_id: Optional[str] = None,
                  vpc: Optional[str] = None,
                  zone: Optional[str] = None):
         """
-        :param bool disable_security_group_ingress: Disables the automatic ingress creation. Default `false` (bool)
-        :param bool disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
-        :param str elb_security_group: Use these ELB security groups instead create new (string)
-        :param str kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources (string)
-        :param str kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources (string)
-        :param str role_arn: IAM role to assume when interaction with AWS APIs (string)
-        :param str route_table_id: Enables using a specific RouteTable (string)
-        :param str subnet_id: (string)
-        :param str vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
-        :param str zone: The AWS zone (string)
+        :param bool disable_security_group_ingress: Disables the automatic ingress creation
+        :param bool disable_strict_zone_check: Setting this to true will disable the check and provide a warning that the check was skipped
+        :param str elb_security_group: Use these ELB security groups instead create new
+        :param str kubernetes_cluster_id: The cluster id we'll use to identify our cluster resources
+        :param str kubernetes_cluster_tag: Legacy cluster id we'll use to identify our cluster resources
+        :param str role_arn: IAM role to assume when interaction with AWS APIs
+        :param str route_table_id: Enables using a specific RouteTable
+        :param str subnet_id: Enables using a specific subnet to use for ELB's
+        :param str vpc: The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
+        :param str zone: The AWS zone
         """
         if disable_security_group_ingress is not None:
             pulumi.set(__self__, "disable_security_group_ingress", disable_security_group_ingress)
         if disable_strict_zone_check is not None:
             pulumi.set(__self__, "disable_strict_zone_check", disable_strict_zone_check)
         if elb_security_group is not None:
             pulumi.set(__self__, "elb_security_group", elb_security_group)
@@ -1156,87 +1066,87 @@
         if zone is not None:
             pulumi.set(__self__, "zone", zone)
 
     @property
     @pulumi.getter(name="disableSecurityGroupIngress")
     def disable_security_group_ingress(self) -> Optional[bool]:
         """
-        Disables the automatic ingress creation. Default `false` (bool)
+        Disables the automatic ingress creation
         """
         return pulumi.get(self, "disable_security_group_ingress")
 
     @property
     @pulumi.getter(name="disableStrictZoneCheck")
     def disable_strict_zone_check(self) -> Optional[bool]:
         """
-        Setting this to true will disable the check and provide a warning that the check was skipped. Default `false` (bool)
+        Setting this to true will disable the check and provide a warning that the check was skipped
         """
         return pulumi.get(self, "disable_strict_zone_check")
 
     @property
     @pulumi.getter(name="elbSecurityGroup")
     def elb_security_group(self) -> Optional[str]:
         """
-        Use these ELB security groups instead create new (string)
+        Use these ELB security groups instead create new
         """
         return pulumi.get(self, "elb_security_group")
 
     @property
     @pulumi.getter(name="kubernetesClusterId")
     def kubernetes_cluster_id(self) -> Optional[str]:
         """
-        The cluster id we'll use to identify our cluster resources (string)
+        The cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_id")
 
     @property
     @pulumi.getter(name="kubernetesClusterTag")
     def kubernetes_cluster_tag(self) -> Optional[str]:
         """
-        Legacy cluster id we'll use to identify our cluster resources (string)
+        Legacy cluster id we'll use to identify our cluster resources
         """
         return pulumi.get(self, "kubernetes_cluster_tag")
 
     @property
     @pulumi.getter(name="roleArn")
     def role_arn(self) -> Optional[str]:
         """
-        IAM role to assume when interaction with AWS APIs (string)
+        IAM role to assume when interaction with AWS APIs
         """
         return pulumi.get(self, "role_arn")
 
     @property
     @pulumi.getter(name="routeTableId")
     def route_table_id(self) -> Optional[str]:
         """
-        Enables using a specific RouteTable (string)
+        Enables using a specific RouteTable
         """
         return pulumi.get(self, "route_table_id")
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[str]:
         """
-        (string)
+        Enables using a specific subnet to use for ELB's
         """
         return pulumi.get(self, "subnet_id")
 
     @property
     @pulumi.getter
     def vpc(self) -> Optional[str]:
         """
-        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided (string)
+        The AWS VPC flag enables the possibility to run the master components on a different aws account, on a different cloud provider or on-premises. If the flag is set also the KubernetesClusterTag must be provided
         """
         return pulumi.get(self, "vpc")
 
     @property
     @pulumi.getter
     def zone(self) -> Optional[str]:
         """
-        The AWS zone (string)
+        The AWS zone
         """
         return pulumi.get(self, "zone")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAwsCloudProviderServiceOverride(dict):
     @staticmethod
@@ -1264,23 +1174,14 @@
                  service: str,
                  key: Optional[str] = None,
                  region: Optional[str] = None,
                  signing_method: Optional[str] = None,
                  signing_name: Optional[str] = None,
                  signing_region: Optional[str] = None,
                  url: Optional[str] = None):
-        """
-        :param str service: (string)
-        :param str key: TLS key for etcd service (string)
-        :param str region: Region for S3 service (string)
-        :param str signing_method: (string)
-        :param str signing_name: (string)
-        :param str signing_region: (string)
-        :param str url: Registry URL (string)
-        """
         pulumi.set(__self__, "service", service)
         if key is not None:
             pulumi.set(__self__, "key", key)
         if region is not None:
             pulumi.set(__self__, "region", region)
         if signing_method is not None:
             pulumi.set(__self__, "signing_method", signing_method)
@@ -1290,68 +1191,47 @@
             pulumi.set(__self__, "signing_region", signing_region)
         if url is not None:
             pulumi.set(__self__, "url", url)
 
     @property
     @pulumi.getter
     def service(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "service")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        TLS key for etcd service (string)
-        """
         warnings.warn("""Use service instead""", DeprecationWarning)
         pulumi.log.warn("""key is deprecated: Use service instead""")
 
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="signingMethod")
     def signing_method(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_method")
 
     @property
     @pulumi.getter(name="signingName")
     def signing_name(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_name")
 
     @property
     @pulumi.getter(name="signingRegion")
     def signing_region(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "signing_region")
 
     @property
     @pulumi.getter
     def url(self) -> Optional[str]:
-        """
-        Registry URL (string)
-        """
         return pulumi.get(self, "url")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAzureCloudConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -1449,43 +1329,42 @@
                  subnet_name: Optional[str] = None,
                  use_instance_metadata: Optional[bool] = None,
                  use_managed_identity_extension: Optional[bool] = None,
                  vm_type: Optional[str] = None,
                  vnet_name: Optional[str] = None,
                  vnet_resource_group: Optional[str] = None):
         """
-        :param str aad_client_id: (string)
-        :param str aad_client_secret: (string)
-        :param str subscription_id: (string)
-        :param str tenant_id: Required if `tenant_name` not provided. (string)
-        :param str aad_client_cert_password: (string)
-        :param str aad_client_cert_path: (string)
-        :param str cloud: (string)
-        :param bool cloud_provider_backoff: (bool)
-        :param int cloud_provider_backoff_duration: (int)
-        :param int cloud_provider_backoff_exponent: (int)
-        :param int cloud_provider_backoff_jitter: (int)
-        :param int cloud_provider_backoff_retries: (int)
-        :param bool cloud_provider_rate_limit: (bool)
-        :param int cloud_provider_rate_limit_bucket: (int)
-        :param int cloud_provider_rate_limit_qps: (int)
+        :param str aad_client_id: The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str aad_client_secret: The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str subscription_id: The ID of the Azure Subscription that the cluster is deployed in
+        :param str tenant_id: The AAD Tenant ID for the Subscription that the cluster is deployed in
+        :param str aad_client_cert_password: The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str aad_client_cert_path: The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str cloud: The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
+        :param bool cloud_provider_backoff: Enable exponential backoff to manage resource request retries
+        :param int cloud_provider_backoff_duration: Backoff duration
+        :param int cloud_provider_backoff_exponent: Backoff exponent
+        :param int cloud_provider_backoff_jitter: Backoff jitter
+        :param int cloud_provider_backoff_retries: Backoff retry limit
+        :param bool cloud_provider_rate_limit: Enable rate limiting
+        :param int cloud_provider_rate_limit_qps: Rate limit QPS
         :param str load_balancer_sku: Load balancer type (basic | standard). Must be standard for auto-scaling
-        :param str location: (string)
-        :param int maximum_load_balancer_rule_count: (int)
-        :param str primary_availability_set_name: (string)
-        :param str primary_scale_set_name: (string)
-        :param str resource_group: (string)
-        :param str route_table_name: (string)
-        :param str security_group_name: (string)
-        :param str subnet_name: (string)
-        :param bool use_instance_metadata: (bool)
-        :param bool use_managed_identity_extension: (bool)
-        :param str vm_type: (string)
-        :param str vnet_name: (string)
-        :param str vnet_resource_group: (string)
+        :param str location: The location of the resource group that the cluster is deployed in
+        :param int maximum_load_balancer_rule_count: Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
+        :param str primary_availability_set_name: The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
+        :param str primary_scale_set_name: The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
+        :param str resource_group: The name of the resource group that the cluster is deployed in
+        :param str route_table_name: (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
+        :param str security_group_name: The name of the security group attached to the cluster's subnet
+        :param str subnet_name: The name of the Subnet that the cluster is deployed in
+        :param bool use_instance_metadata: Use instance metadata service where possible
+        :param bool use_managed_identity_extension: Use managed service identity for the virtual machine to access Azure ARM APIs
+        :param str vm_type: The type of azure nodes. If not set, it will be default to standard.
+        :param str vnet_name: The name of the VNet that the cluster is deployed in
+        :param str vnet_resource_group: The name of the resource group that the Vnet is deployed in
         """
         pulumi.set(__self__, "aad_client_id", aad_client_id)
         pulumi.set(__self__, "aad_client_secret", aad_client_secret)
         pulumi.set(__self__, "subscription_id", subscription_id)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if aad_client_cert_password is not None:
             pulumi.set(__self__, "aad_client_cert_password", aad_client_cert_password)
@@ -1538,127 +1417,124 @@
         if vnet_resource_group is not None:
             pulumi.set(__self__, "vnet_resource_group", vnet_resource_group)
 
     @property
     @pulumi.getter(name="aadClientId")
     def aad_client_id(self) -> str:
         """
-        (string)
+        The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_id")
 
     @property
     @pulumi.getter(name="aadClientSecret")
     def aad_client_secret(self) -> str:
         """
-        (string)
+        The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_secret")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> str:
         """
-        (string)
+        The ID of the Azure Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> str:
         """
-        Required if `tenant_name` not provided. (string)
+        The AAD Tenant ID for the Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter(name="aadClientCertPassword")
     def aad_client_cert_password(self) -> Optional[str]:
         """
-        (string)
+        The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_password")
 
     @property
     @pulumi.getter(name="aadClientCertPath")
     def aad_client_cert_path(self) -> Optional[str]:
         """
-        (string)
+        The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_path")
 
     @property
     @pulumi.getter
     def cloud(self) -> Optional[str]:
         """
-        (string)
+        The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
         """
         return pulumi.get(self, "cloud")
 
     @property
     @pulumi.getter(name="cloudProviderBackoff")
     def cloud_provider_backoff(self) -> Optional[bool]:
         """
-        (bool)
+        Enable exponential backoff to manage resource request retries
         """
         return pulumi.get(self, "cloud_provider_backoff")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffDuration")
     def cloud_provider_backoff_duration(self) -> Optional[int]:
         """
-        (int)
+        Backoff duration
         """
         return pulumi.get(self, "cloud_provider_backoff_duration")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffExponent")
     def cloud_provider_backoff_exponent(self) -> Optional[int]:
         """
-        (int)
+        Backoff exponent
         """
         return pulumi.get(self, "cloud_provider_backoff_exponent")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffJitter")
     def cloud_provider_backoff_jitter(self) -> Optional[int]:
         """
-        (int)
+        Backoff jitter
         """
         return pulumi.get(self, "cloud_provider_backoff_jitter")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffRetries")
     def cloud_provider_backoff_retries(self) -> Optional[int]:
         """
-        (int)
+        Backoff retry limit
         """
         return pulumi.get(self, "cloud_provider_backoff_retries")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimit")
     def cloud_provider_rate_limit(self) -> Optional[bool]:
         """
-        (bool)
+        Enable rate limiting
         """
         return pulumi.get(self, "cloud_provider_rate_limit")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitBucket")
     def cloud_provider_rate_limit_bucket(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "cloud_provider_rate_limit_bucket")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitQps")
     def cloud_provider_rate_limit_qps(self) -> Optional[int]:
         """
-        (int)
+        Rate limit QPS
         """
         return pulumi.get(self, "cloud_provider_rate_limit_qps")
 
     @property
     @pulumi.getter(name="loadBalancerSku")
     def load_balancer_sku(self) -> Optional[str]:
         """
@@ -1666,111 +1542,111 @@
         """
         return pulumi.get(self, "load_balancer_sku")
 
     @property
     @pulumi.getter
     def location(self) -> Optional[str]:
         """
-        (string)
+        The location of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "location")
 
     @property
     @pulumi.getter(name="maximumLoadBalancerRuleCount")
     def maximum_load_balancer_rule_count(self) -> Optional[int]:
         """
-        (int)
+        Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
         """
         return pulumi.get(self, "maximum_load_balancer_rule_count")
 
     @property
     @pulumi.getter(name="primaryAvailabilitySetName")
     def primary_availability_set_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_availability_set_name")
 
     @property
     @pulumi.getter(name="primaryScaleSetName")
     def primary_scale_set_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_scale_set_name")
 
     @property
     @pulumi.getter(name="resourceGroup")
     def resource_group(self) -> Optional[str]:
         """
-        (string)
+        The name of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "resource_group")
 
     @property
     @pulumi.getter(name="routeTableName")
     def route_table_name(self) -> Optional[str]:
         """
-        (string)
+        (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
         """
         return pulumi.get(self, "route_table_name")
 
     @property
     @pulumi.getter(name="securityGroupName")
     def security_group_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the security group attached to the cluster's subnet
         """
         return pulumi.get(self, "security_group_name")
 
     @property
     @pulumi.getter(name="subnetName")
     def subnet_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the Subnet that the cluster is deployed in
         """
         return pulumi.get(self, "subnet_name")
 
     @property
     @pulumi.getter(name="useInstanceMetadata")
     def use_instance_metadata(self) -> Optional[bool]:
         """
-        (bool)
+        Use instance metadata service where possible
         """
         return pulumi.get(self, "use_instance_metadata")
 
     @property
     @pulumi.getter(name="useManagedIdentityExtension")
     def use_managed_identity_extension(self) -> Optional[bool]:
         """
-        (bool)
+        Use managed service identity for the virtual machine to access Azure ARM APIs
         """
         return pulumi.get(self, "use_managed_identity_extension")
 
     @property
     @pulumi.getter(name="vmType")
     def vm_type(self) -> Optional[str]:
         """
-        (string)
+        The type of azure nodes. If not set, it will be default to standard.
         """
         return pulumi.get(self, "vm_type")
 
     @property
     @pulumi.getter(name="vnetName")
     def vnet_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the VNet that the cluster is deployed in
         """
         return pulumi.get(self, "vnet_name")
 
     @property
     @pulumi.getter(name="vnetResourceGroup")
     def vnet_resource_group(self) -> Optional[str]:
         """
-        (string)
+        The name of the resource group that the Vnet is deployed in
         """
         return pulumi.get(self, "vnet_resource_group")
 
 
 @pulumi.output_type
 class ClusterCloudProviderAzureCloudProvider(dict):
     @staticmethod
@@ -1869,43 +1745,42 @@
                  subnet_name: Optional[str] = None,
                  use_instance_metadata: Optional[bool] = None,
                  use_managed_identity_extension: Optional[bool] = None,
                  vm_type: Optional[str] = None,
                  vnet_name: Optional[str] = None,
                  vnet_resource_group: Optional[str] = None):
         """
-        :param str aad_client_id: (string)
-        :param str aad_client_secret: (string)
-        :param str subscription_id: (string)
-        :param str tenant_id: Required if `tenant_name` not provided. (string)
-        :param str aad_client_cert_password: (string)
-        :param str aad_client_cert_path: (string)
-        :param str cloud: (string)
-        :param bool cloud_provider_backoff: (bool)
-        :param int cloud_provider_backoff_duration: (int)
-        :param int cloud_provider_backoff_exponent: (int)
-        :param int cloud_provider_backoff_jitter: (int)
-        :param int cloud_provider_backoff_retries: (int)
-        :param bool cloud_provider_rate_limit: (bool)
-        :param int cloud_provider_rate_limit_bucket: (int)
-        :param int cloud_provider_rate_limit_qps: (int)
+        :param str aad_client_id: The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str aad_client_secret: The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str subscription_id: The ID of the Azure Subscription that the cluster is deployed in
+        :param str tenant_id: The AAD Tenant ID for the Subscription that the cluster is deployed in
+        :param str aad_client_cert_password: The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str aad_client_cert_path: The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
+        :param str cloud: The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
+        :param bool cloud_provider_backoff: Enable exponential backoff to manage resource request retries
+        :param int cloud_provider_backoff_duration: Backoff duration
+        :param int cloud_provider_backoff_exponent: Backoff exponent
+        :param int cloud_provider_backoff_jitter: Backoff jitter
+        :param int cloud_provider_backoff_retries: Backoff retry limit
+        :param bool cloud_provider_rate_limit: Enable rate limiting
+        :param int cloud_provider_rate_limit_qps: Rate limit QPS
         :param str load_balancer_sku: Load balancer type (basic | standard). Must be standard for auto-scaling
-        :param str location: (string)
-        :param int maximum_load_balancer_rule_count: (int)
-        :param str primary_availability_set_name: (string)
-        :param str primary_scale_set_name: (string)
-        :param str resource_group: (string)
-        :param str route_table_name: (string)
-        :param str security_group_name: (string)
-        :param str subnet_name: (string)
-        :param bool use_instance_metadata: (bool)
-        :param bool use_managed_identity_extension: (bool)
-        :param str vm_type: (string)
-        :param str vnet_name: (string)
-        :param str vnet_resource_group: (string)
+        :param str location: The location of the resource group that the cluster is deployed in
+        :param int maximum_load_balancer_rule_count: Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
+        :param str primary_availability_set_name: The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
+        :param str primary_scale_set_name: The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
+        :param str resource_group: The name of the resource group that the cluster is deployed in
+        :param str route_table_name: (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
+        :param str security_group_name: The name of the security group attached to the cluster's subnet
+        :param str subnet_name: The name of the Subnet that the cluster is deployed in
+        :param bool use_instance_metadata: Use instance metadata service where possible
+        :param bool use_managed_identity_extension: Use managed service identity for the virtual machine to access Azure ARM APIs
+        :param str vm_type: The type of azure nodes. If not set, it will be default to standard.
+        :param str vnet_name: The name of the VNet that the cluster is deployed in
+        :param str vnet_resource_group: The name of the resource group that the Vnet is deployed in
         """
         pulumi.set(__self__, "aad_client_id", aad_client_id)
         pulumi.set(__self__, "aad_client_secret", aad_client_secret)
         pulumi.set(__self__, "subscription_id", subscription_id)
         pulumi.set(__self__, "tenant_id", tenant_id)
         if aad_client_cert_password is not None:
             pulumi.set(__self__, "aad_client_cert_password", aad_client_cert_password)
@@ -1958,127 +1833,124 @@
         if vnet_resource_group is not None:
             pulumi.set(__self__, "vnet_resource_group", vnet_resource_group)
 
     @property
     @pulumi.getter(name="aadClientId")
     def aad_client_id(self) -> str:
         """
-        (string)
+        The ClientID for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_id")
 
     @property
     @pulumi.getter(name="aadClientSecret")
     def aad_client_secret(self) -> str:
         """
-        (string)
+        The ClientSecret for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_secret")
 
     @property
     @pulumi.getter(name="subscriptionId")
     def subscription_id(self) -> str:
         """
-        (string)
+        The ID of the Azure Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "subscription_id")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> str:
         """
-        Required if `tenant_name` not provided. (string)
+        The AAD Tenant ID for the Subscription that the cluster is deployed in
         """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter(name="aadClientCertPassword")
     def aad_client_cert_password(self) -> Optional[str]:
         """
-        (string)
+        The password of the client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_password")
 
     @property
     @pulumi.getter(name="aadClientCertPath")
     def aad_client_cert_path(self) -> Optional[str]:
         """
-        (string)
+        The path of a client certificate for an AAD application with RBAC access to talk to Azure RM APIs
         """
         return pulumi.get(self, "aad_client_cert_path")
 
     @property
     @pulumi.getter
     def cloud(self) -> Optional[str]:
         """
-        (string)
+        The cloud environment identifier. Takes values from https://github.com/Azure/go-autorest/blob/ec5f4903f77ed9927ac95b19ab8e44ada64c1356/autorest/azure/environments.go#L13
         """
         return pulumi.get(self, "cloud")
 
     @property
     @pulumi.getter(name="cloudProviderBackoff")
     def cloud_provider_backoff(self) -> Optional[bool]:
         """
-        (bool)
+        Enable exponential backoff to manage resource request retries
         """
         return pulumi.get(self, "cloud_provider_backoff")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffDuration")
     def cloud_provider_backoff_duration(self) -> Optional[int]:
         """
-        (int)
+        Backoff duration
         """
         return pulumi.get(self, "cloud_provider_backoff_duration")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffExponent")
     def cloud_provider_backoff_exponent(self) -> Optional[int]:
         """
-        (int)
+        Backoff exponent
         """
         return pulumi.get(self, "cloud_provider_backoff_exponent")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffJitter")
     def cloud_provider_backoff_jitter(self) -> Optional[int]:
         """
-        (int)
+        Backoff jitter
         """
         return pulumi.get(self, "cloud_provider_backoff_jitter")
 
     @property
     @pulumi.getter(name="cloudProviderBackoffRetries")
     def cloud_provider_backoff_retries(self) -> Optional[int]:
         """
-        (int)
+        Backoff retry limit
         """
         return pulumi.get(self, "cloud_provider_backoff_retries")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimit")
     def cloud_provider_rate_limit(self) -> Optional[bool]:
         """
-        (bool)
+        Enable rate limiting
         """
         return pulumi.get(self, "cloud_provider_rate_limit")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitBucket")
     def cloud_provider_rate_limit_bucket(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "cloud_provider_rate_limit_bucket")
 
     @property
     @pulumi.getter(name="cloudProviderRateLimitQps")
     def cloud_provider_rate_limit_qps(self) -> Optional[int]:
         """
-        (int)
+        Rate limit QPS
         """
         return pulumi.get(self, "cloud_provider_rate_limit_qps")
 
     @property
     @pulumi.getter(name="loadBalancerSku")
     def load_balancer_sku(self) -> Optional[str]:
         """
@@ -2086,111 +1958,111 @@
         """
         return pulumi.get(self, "load_balancer_sku")
 
     @property
     @pulumi.getter
     def location(self) -> Optional[str]:
         """
-        (string)
+        The location of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "location")
 
     @property
     @pulumi.getter(name="maximumLoadBalancerRuleCount")
     def maximum_load_balancer_rule_count(self) -> Optional[int]:
         """
-        (int)
+        Maximum allowed LoadBalancer Rule Count is the limit enforced by Azure Load balancer
         """
         return pulumi.get(self, "maximum_load_balancer_rule_count")
 
     @property
     @pulumi.getter(name="primaryAvailabilitySetName")
     def primary_availability_set_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the availability set that should be used as the load balancer backendIf this is set, the Azure cloudprovider will only add nodes from that availability set to the loadbalancer backend pool. If this is not set, and multiple agent pools (availability sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (availability sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_availability_set_name")
 
     @property
     @pulumi.getter(name="primaryScaleSetName")
     def primary_scale_set_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the scale set that should be used as the load balancer backend.If this is set, the Azure cloudprovider will only add nodes from that scale set to the loadbalancer backend pool. If this is not set, and multiple agent pools (scale sets) are used, thenthe cloudprovider will try to add all nodes to a single backend pool which is forbidden.In other words, if you use multiple agent pools (scale sets), you MUST set this field.
         """
         return pulumi.get(self, "primary_scale_set_name")
 
     @property
     @pulumi.getter(name="resourceGroup")
     def resource_group(self) -> Optional[str]:
         """
-        (string)
+        The name of the resource group that the cluster is deployed in
         """
         return pulumi.get(self, "resource_group")
 
     @property
     @pulumi.getter(name="routeTableName")
     def route_table_name(self) -> Optional[str]:
         """
-        (string)
+        (Optional in 1.6) The name of the route table attached to the subnet that the cluster is deployed in
         """
         return pulumi.get(self, "route_table_name")
 
     @property
     @pulumi.getter(name="securityGroupName")
     def security_group_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the security group attached to the cluster's subnet
         """
         return pulumi.get(self, "security_group_name")
 
     @property
     @pulumi.getter(name="subnetName")
     def subnet_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the Subnet that the cluster is deployed in
         """
         return pulumi.get(self, "subnet_name")
 
     @property
     @pulumi.getter(name="useInstanceMetadata")
     def use_instance_metadata(self) -> Optional[bool]:
         """
-        (bool)
+        Use instance metadata service where possible
         """
         return pulumi.get(self, "use_instance_metadata")
 
     @property
     @pulumi.getter(name="useManagedIdentityExtension")
     def use_managed_identity_extension(self) -> Optional[bool]:
         """
-        (bool)
+        Use managed service identity for the virtual machine to access Azure ARM APIs
         """
         return pulumi.get(self, "use_managed_identity_extension")
 
     @property
     @pulumi.getter(name="vmType")
     def vm_type(self) -> Optional[str]:
         """
-        (string)
+        The type of azure nodes. If not set, it will be default to standard.
         """
         return pulumi.get(self, "vm_type")
 
     @property
     @pulumi.getter(name="vnetName")
     def vnet_name(self) -> Optional[str]:
         """
-        (string)
+        The name of the VNet that the cluster is deployed in
         """
         return pulumi.get(self, "vnet_name")
 
     @property
     @pulumi.getter(name="vnetResourceGroup")
     def vnet_resource_group(self) -> Optional[str]:
         """
-        (string)
+        The name of the resource group that the Vnet is deployed in
         """
         return pulumi.get(self, "vnet_resource_group")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfig(dict):
     @staticmethod
@@ -2216,69 +2088,47 @@
 
     def __init__(__self__, *,
                  global_: 'outputs.ClusterCloudProviderOpenstackCloudConfigGlobal',
                  block_storage: Optional['outputs.ClusterCloudProviderOpenstackCloudConfigBlockStorage'] = None,
                  load_balancer: Optional['outputs.ClusterCloudProviderOpenstackCloudConfigLoadBalancer'] = None,
                  metadata: Optional['outputs.ClusterCloudProviderOpenstackCloudConfigMetadata'] = None,
                  route: Optional['outputs.ClusterCloudProviderOpenstackCloudConfigRoute'] = None):
-        """
-        :param 'ClusterCloudProviderOpenstackCloudConfigGlobalArgs' global_: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudConfigBlockStorageArgs' block_storage: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudConfigLoadBalancerArgs' load_balancer: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudConfigMetadataArgs' metadata: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudConfigRouteArgs' route: (list maxitems:1)
-        """
         pulumi.set(__self__, "global_", global_)
         if block_storage is not None:
             pulumi.set(__self__, "block_storage", block_storage)
         if load_balancer is not None:
             pulumi.set(__self__, "load_balancer", load_balancer)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if route is not None:
             pulumi.set(__self__, "route", route)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> 'outputs.ClusterCloudProviderOpenstackCloudConfigGlobal':
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter(name="blockStorage")
     def block_storage(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudConfigBlockStorage']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "block_storage")
 
     @property
     @pulumi.getter(name="loadBalancer")
     def load_balancer(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudConfigLoadBalancer']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "load_balancer")
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudConfigMetadata']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "metadata")
 
     @property
     @pulumi.getter
     def route(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudConfigRoute']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "route")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfigBlockStorage(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2301,48 +2151,34 @@
         ClusterCloudProviderOpenstackCloudConfigBlockStorage.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bs_version: Optional[str] = None,
                  ignore_volume_az: Optional[bool] = None,
                  trust_device_path: Optional[bool] = None):
-        """
-        :param str bs_version: (string)
-        :param bool ignore_volume_az: (string)
-        :param bool trust_device_path: (string)
-        """
         if bs_version is not None:
             pulumi.set(__self__, "bs_version", bs_version)
         if ignore_volume_az is not None:
             pulumi.set(__self__, "ignore_volume_az", ignore_volume_az)
         if trust_device_path is not None:
             pulumi.set(__self__, "trust_device_path", trust_device_path)
 
     @property
     @pulumi.getter(name="bsVersion")
     def bs_version(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "bs_version")
 
     @property
     @pulumi.getter(name="ignoreVolumeAz")
     def ignore_volume_az(self) -> Optional[bool]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ignore_volume_az")
 
     @property
     @pulumi.getter(name="trustDevicePath")
     def trust_device_path(self) -> Optional[bool]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_device_path")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfigGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2383,27 +2219,14 @@
                  domain_name: Optional[str] = None,
                  region: Optional[str] = None,
                  tenant_id: Optional[str] = None,
                  tenant_name: Optional[str] = None,
                  trust_id: Optional[str] = None,
                  user_id: Optional[str] = None,
                  username: Optional[str] = None):
-        """
-        :param str auth_url: (string)
-        :param str password: Registry password (string)
-        :param str ca_file: (string)
-        :param str domain_id: Required if `domain_name` not provided. (string)
-        :param str domain_name: Required if `domain_id` not provided. (string)
-        :param str region: Region for S3 service (string)
-        :param str tenant_id: Required if `tenant_name` not provided. (string)
-        :param str tenant_name: Required if `tenant_id` not provided. (string)
-        :param str trust_id: (string)
-        :param str user_id: Required if `username` not provided. (string)
-        :param str username: Required if `user_id` not provided. (string)
-        """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "password", password)
         if ca_file is not None:
             pulumi.set(__self__, "ca_file", ca_file)
         if domain_id is not None:
             pulumi.set(__self__, "domain_id", domain_id)
         if domain_name is not None:
@@ -2420,97 +2243,64 @@
             pulumi.set(__self__, "user_id", user_id)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authUrl")
     def auth_url(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "auth_url")
 
     @property
     @pulumi.getter
     def password(self) -> str:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="caFile")
     def ca_file(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ca_file")
 
     @property
     @pulumi.getter(name="domainId")
     def domain_id(self) -> Optional[str]:
-        """
-        Required if `domain_name` not provided. (string)
-        """
         return pulumi.get(self, "domain_id")
 
     @property
     @pulumi.getter(name="domainName")
     def domain_name(self) -> Optional[str]:
-        """
-        Required if `domain_id` not provided. (string)
-        """
         return pulumi.get(self, "domain_name")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
-        """
-        Required if `tenant_name` not provided. (string)
-        """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[str]:
-        """
-        Required if `tenant_id` not provided. (string)
-        """
         return pulumi.get(self, "tenant_name")
 
     @property
     @pulumi.getter(name="trustId")
     def trust_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_id")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[str]:
-        """
-        Required if `username` not provided. (string)
-        """
         return pulumi.get(self, "user_id")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
-        """
-        Required if `user_id` not provided. (string)
-        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfigLoadBalancer(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2557,27 +2347,14 @@
                  lb_version: Optional[str] = None,
                  manage_security_groups: Optional[bool] = None,
                  monitor_delay: Optional[str] = None,
                  monitor_max_retries: Optional[int] = None,
                  monitor_timeout: Optional[str] = None,
                  subnet_id: Optional[str] = None,
                  use_octavia: Optional[bool] = None):
-        """
-        :param bool create_monitor: (bool)
-        :param str floating_network_id: (string)
-        :param str lb_method: (string)
-        :param str lb_provider: (string)
-        :param str lb_version: (string)
-        :param bool manage_security_groups: (bool)
-        :param str monitor_delay: (string)
-        :param int monitor_max_retries: (int)
-        :param str monitor_timeout: (string)
-        :param str subnet_id: (string)
-        :param bool use_octavia: (bool)
-        """
         if create_monitor is not None:
             pulumi.set(__self__, "create_monitor", create_monitor)
         if floating_network_id is not None:
             pulumi.set(__self__, "floating_network_id", floating_network_id)
         if lb_method is not None:
             pulumi.set(__self__, "lb_method", lb_method)
         if lb_provider is not None:
@@ -2596,97 +2373,64 @@
             pulumi.set(__self__, "subnet_id", subnet_id)
         if use_octavia is not None:
             pulumi.set(__self__, "use_octavia", use_octavia)
 
     @property
     @pulumi.getter(name="createMonitor")
     def create_monitor(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "create_monitor")
 
     @property
     @pulumi.getter(name="floatingNetworkId")
     def floating_network_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "floating_network_id")
 
     @property
     @pulumi.getter(name="lbMethod")
     def lb_method(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_method")
 
     @property
     @pulumi.getter(name="lbProvider")
     def lb_provider(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_provider")
 
     @property
     @pulumi.getter(name="lbVersion")
     def lb_version(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_version")
 
     @property
     @pulumi.getter(name="manageSecurityGroups")
     def manage_security_groups(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "manage_security_groups")
 
     @property
     @pulumi.getter(name="monitorDelay")
     def monitor_delay(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_delay")
 
     @property
     @pulumi.getter(name="monitorMaxRetries")
     def monitor_max_retries(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "monitor_max_retries")
 
     @property
     @pulumi.getter(name="monitorTimeout")
     def monitor_timeout(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_timeout")
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "subnet_id")
 
     @property
     @pulumi.getter(name="useOctavia")
     def use_octavia(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "use_octavia")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfigMetadata(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2706,37 +2450,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderOpenstackCloudConfigMetadata.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  request_timeout: Optional[int] = None,
                  search_order: Optional[str] = None):
-        """
-        :param int request_timeout: (int)
-        :param str search_order: (string)
-        """
         if request_timeout is not None:
             pulumi.set(__self__, "request_timeout", request_timeout)
         if search_order is not None:
             pulumi.set(__self__, "search_order", search_order)
 
     @property
     @pulumi.getter(name="requestTimeout")
     def request_timeout(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "request_timeout")
 
     @property
     @pulumi.getter(name="searchOrder")
     def search_order(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "search_order")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudConfigRoute(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2753,26 +2487,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderOpenstackCloudConfigRoute.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  router_id: Optional[str] = None):
-        """
-        :param str router_id: (string)
-        """
         if router_id is not None:
             pulumi.set(__self__, "router_id", router_id)
 
     @property
     @pulumi.getter(name="routerId")
     def router_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "router_id")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProvider(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2797,69 +2525,47 @@
 
     def __init__(__self__, *,
                  global_: 'outputs.ClusterCloudProviderOpenstackCloudProviderGlobal',
                  block_storage: Optional['outputs.ClusterCloudProviderOpenstackCloudProviderBlockStorage'] = None,
                  load_balancer: Optional['outputs.ClusterCloudProviderOpenstackCloudProviderLoadBalancer'] = None,
                  metadata: Optional['outputs.ClusterCloudProviderOpenstackCloudProviderMetadata'] = None,
                  route: Optional['outputs.ClusterCloudProviderOpenstackCloudProviderRoute'] = None):
-        """
-        :param 'ClusterCloudProviderOpenstackCloudProviderGlobalArgs' global_: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudProviderBlockStorageArgs' block_storage: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudProviderLoadBalancerArgs' load_balancer: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudProviderMetadataArgs' metadata: (list maxitems:1)
-        :param 'ClusterCloudProviderOpenstackCloudProviderRouteArgs' route: (list maxitems:1)
-        """
         pulumi.set(__self__, "global_", global_)
         if block_storage is not None:
             pulumi.set(__self__, "block_storage", block_storage)
         if load_balancer is not None:
             pulumi.set(__self__, "load_balancer", load_balancer)
         if metadata is not None:
             pulumi.set(__self__, "metadata", metadata)
         if route is not None:
             pulumi.set(__self__, "route", route)
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> 'outputs.ClusterCloudProviderOpenstackCloudProviderGlobal':
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter(name="blockStorage")
     def block_storage(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudProviderBlockStorage']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "block_storage")
 
     @property
     @pulumi.getter(name="loadBalancer")
     def load_balancer(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudProviderLoadBalancer']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "load_balancer")
 
     @property
     @pulumi.getter
     def metadata(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudProviderMetadata']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "metadata")
 
     @property
     @pulumi.getter
     def route(self) -> Optional['outputs.ClusterCloudProviderOpenstackCloudProviderRoute']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "route")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProviderBlockStorage(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2882,48 +2588,34 @@
         ClusterCloudProviderOpenstackCloudProviderBlockStorage.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  bs_version: Optional[str] = None,
                  ignore_volume_az: Optional[bool] = None,
                  trust_device_path: Optional[bool] = None):
-        """
-        :param str bs_version: (string)
-        :param bool ignore_volume_az: (string)
-        :param bool trust_device_path: (string)
-        """
         if bs_version is not None:
             pulumi.set(__self__, "bs_version", bs_version)
         if ignore_volume_az is not None:
             pulumi.set(__self__, "ignore_volume_az", ignore_volume_az)
         if trust_device_path is not None:
             pulumi.set(__self__, "trust_device_path", trust_device_path)
 
     @property
     @pulumi.getter(name="bsVersion")
     def bs_version(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "bs_version")
 
     @property
     @pulumi.getter(name="ignoreVolumeAz")
     def ignore_volume_az(self) -> Optional[bool]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ignore_volume_az")
 
     @property
     @pulumi.getter(name="trustDevicePath")
     def trust_device_path(self) -> Optional[bool]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_device_path")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProviderGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -2964,27 +2656,14 @@
                  domain_name: Optional[str] = None,
                  region: Optional[str] = None,
                  tenant_id: Optional[str] = None,
                  tenant_name: Optional[str] = None,
                  trust_id: Optional[str] = None,
                  user_id: Optional[str] = None,
                  username: Optional[str] = None):
-        """
-        :param str auth_url: (string)
-        :param str password: Registry password (string)
-        :param str ca_file: (string)
-        :param str domain_id: Required if `domain_name` not provided. (string)
-        :param str domain_name: Required if `domain_id` not provided. (string)
-        :param str region: Region for S3 service (string)
-        :param str tenant_id: Required if `tenant_name` not provided. (string)
-        :param str tenant_name: Required if `tenant_id` not provided. (string)
-        :param str trust_id: (string)
-        :param str user_id: Required if `username` not provided. (string)
-        :param str username: Required if `user_id` not provided. (string)
-        """
         pulumi.set(__self__, "auth_url", auth_url)
         pulumi.set(__self__, "password", password)
         if ca_file is not None:
             pulumi.set(__self__, "ca_file", ca_file)
         if domain_id is not None:
             pulumi.set(__self__, "domain_id", domain_id)
         if domain_name is not None:
@@ -3001,97 +2680,64 @@
             pulumi.set(__self__, "user_id", user_id)
         if username is not None:
             pulumi.set(__self__, "username", username)
 
     @property
     @pulumi.getter(name="authUrl")
     def auth_url(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "auth_url")
 
     @property
     @pulumi.getter
     def password(self) -> str:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter(name="caFile")
     def ca_file(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "ca_file")
 
     @property
     @pulumi.getter(name="domainId")
     def domain_id(self) -> Optional[str]:
-        """
-        Required if `domain_name` not provided. (string)
-        """
         return pulumi.get(self, "domain_id")
 
     @property
     @pulumi.getter(name="domainName")
     def domain_name(self) -> Optional[str]:
-        """
-        Required if `domain_id` not provided. (string)
-        """
         return pulumi.get(self, "domain_name")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="tenantId")
     def tenant_id(self) -> Optional[str]:
-        """
-        Required if `tenant_name` not provided. (string)
-        """
         return pulumi.get(self, "tenant_id")
 
     @property
     @pulumi.getter(name="tenantName")
     def tenant_name(self) -> Optional[str]:
-        """
-        Required if `tenant_id` not provided. (string)
-        """
         return pulumi.get(self, "tenant_name")
 
     @property
     @pulumi.getter(name="trustId")
     def trust_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "trust_id")
 
     @property
     @pulumi.getter(name="userId")
     def user_id(self) -> Optional[str]:
-        """
-        Required if `username` not provided. (string)
-        """
         return pulumi.get(self, "user_id")
 
     @property
     @pulumi.getter
     def username(self) -> Optional[str]:
-        """
-        Required if `user_id` not provided. (string)
-        """
         return pulumi.get(self, "username")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProviderLoadBalancer(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3138,27 +2784,14 @@
                  lb_version: Optional[str] = None,
                  manage_security_groups: Optional[bool] = None,
                  monitor_delay: Optional[str] = None,
                  monitor_max_retries: Optional[int] = None,
                  monitor_timeout: Optional[str] = None,
                  subnet_id: Optional[str] = None,
                  use_octavia: Optional[bool] = None):
-        """
-        :param bool create_monitor: (bool)
-        :param str floating_network_id: (string)
-        :param str lb_method: (string)
-        :param str lb_provider: (string)
-        :param str lb_version: (string)
-        :param bool manage_security_groups: (bool)
-        :param str monitor_delay: (string)
-        :param int monitor_max_retries: (int)
-        :param str monitor_timeout: (string)
-        :param str subnet_id: (string)
-        :param bool use_octavia: (bool)
-        """
         if create_monitor is not None:
             pulumi.set(__self__, "create_monitor", create_monitor)
         if floating_network_id is not None:
             pulumi.set(__self__, "floating_network_id", floating_network_id)
         if lb_method is not None:
             pulumi.set(__self__, "lb_method", lb_method)
         if lb_provider is not None:
@@ -3177,97 +2810,64 @@
             pulumi.set(__self__, "subnet_id", subnet_id)
         if use_octavia is not None:
             pulumi.set(__self__, "use_octavia", use_octavia)
 
     @property
     @pulumi.getter(name="createMonitor")
     def create_monitor(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "create_monitor")
 
     @property
     @pulumi.getter(name="floatingNetworkId")
     def floating_network_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "floating_network_id")
 
     @property
     @pulumi.getter(name="lbMethod")
     def lb_method(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_method")
 
     @property
     @pulumi.getter(name="lbProvider")
     def lb_provider(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_provider")
 
     @property
     @pulumi.getter(name="lbVersion")
     def lb_version(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "lb_version")
 
     @property
     @pulumi.getter(name="manageSecurityGroups")
     def manage_security_groups(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "manage_security_groups")
 
     @property
     @pulumi.getter(name="monitorDelay")
     def monitor_delay(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_delay")
 
     @property
     @pulumi.getter(name="monitorMaxRetries")
     def monitor_max_retries(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "monitor_max_retries")
 
     @property
     @pulumi.getter(name="monitorTimeout")
     def monitor_timeout(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "monitor_timeout")
 
     @property
     @pulumi.getter(name="subnetId")
     def subnet_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "subnet_id")
 
     @property
     @pulumi.getter(name="useOctavia")
     def use_octavia(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "use_octavia")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProviderMetadata(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3287,37 +2887,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderOpenstackCloudProviderMetadata.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  request_timeout: Optional[int] = None,
                  search_order: Optional[str] = None):
-        """
-        :param int request_timeout: (int)
-        :param str search_order: (string)
-        """
         if request_timeout is not None:
             pulumi.set(__self__, "request_timeout", request_timeout)
         if search_order is not None:
             pulumi.set(__self__, "search_order", search_order)
 
     @property
     @pulumi.getter(name="requestTimeout")
     def request_timeout(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "request_timeout")
 
     @property
     @pulumi.getter(name="searchOrder")
     def search_order(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "search_order")
 
 
 @pulumi.output_type
 class ClusterCloudProviderOpenstackCloudProviderRoute(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3334,26 +2924,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderOpenstackCloudProviderRoute.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  router_id: Optional[str] = None):
-        """
-        :param str router_id: (string)
-        """
         if router_id is not None:
             pulumi.set(__self__, "router_id", router_id)
 
     @property
     @pulumi.getter(name="routerId")
     def router_id(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "router_id")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3377,59 +2961,43 @@
     def __init__(__self__, *,
                  virtual_centers: Sequence['outputs.ClusterCloudProviderVsphereCloudConfigVirtualCenter'],
                  workspace: 'outputs.ClusterCloudProviderVsphereCloudConfigWorkspace',
                  disk: Optional['outputs.ClusterCloudProviderVsphereCloudConfigDisk'] = None,
                  global_: Optional['outputs.ClusterCloudProviderVsphereCloudConfigGlobal'] = None,
                  network: Optional['outputs.ClusterCloudProviderVsphereCloudConfigNetwork'] = None):
         """
-        :param Sequence['ClusterCloudProviderVsphereCloudConfigVirtualCenterArgs'] virtual_centers: (List)
-        :param 'ClusterCloudProviderVsphereCloudConfigWorkspaceArgs' workspace: (list maxitems:1)
-        :param 'ClusterCloudProviderVsphereCloudConfigDiskArgs' disk: (list maxitems:1)
-        :param 'ClusterCloudProviderVsphereCloudConfigGlobalArgs' global_: (list maxitems:1)
         :param 'ClusterCloudProviderVsphereCloudConfigNetworkArgs' network: RKE k8s cluster network configuration (list maxitems:1)
         """
         pulumi.set(__self__, "virtual_centers", virtual_centers)
         pulumi.set(__self__, "workspace", workspace)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if network is not None:
             pulumi.set(__self__, "network", network)
 
     @property
     @pulumi.getter(name="virtualCenters")
     def virtual_centers(self) -> Sequence['outputs.ClusterCloudProviderVsphereCloudConfigVirtualCenter']:
-        """
-        (List)
-        """
         return pulumi.get(self, "virtual_centers")
 
     @property
     @pulumi.getter
     def workspace(self) -> 'outputs.ClusterCloudProviderVsphereCloudConfigWorkspace':
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "workspace")
 
     @property
     @pulumi.getter
     def disk(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudConfigDisk']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "disk")
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudConfigGlobal']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter
     def network(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudConfigNetwork']:
         """
         RKE k8s cluster network configuration (list maxitems:1)
@@ -3454,26 +3022,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderVsphereCloudConfigDisk.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  scsi_controller_type: Optional[str] = None):
-        """
-        :param str scsi_controller_type: (string)
-        """
         if scsi_controller_type is not None:
             pulumi.set(__self__, "scsi_controller_type", scsi_controller_type)
 
     @property
     @pulumi.getter(name="scsiControllerType")
     def scsi_controller_type(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "scsi_controller_type")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudConfigGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3508,27 +3070,14 @@
                  password: Optional[str] = None,
                  port: Optional[str] = None,
                  soap_roundtrip_count: Optional[int] = None,
                  user: Optional[str] = None,
                  vm_name: Optional[str] = None,
                  vm_uuid: Optional[str] = None,
                  working_dir: Optional[str] = None):
-        """
-        :param str datacenter: (string)
-        :param str datacenters: (string)
-        :param str datastore: (string)
-        :param bool insecure_flag: (bool)
-        :param str password: Registry password (string)
-        :param str port: Port used for SSH communication (string)
-        :param int soap_roundtrip_count: (int)
-        :param str user: Registry user (string)
-        :param str vm_name: (string)
-        :param str vm_uuid: (string)
-        :param str working_dir: (string)
-        """
         if datacenter is not None:
             pulumi.set(__self__, "datacenter", datacenter)
         if datacenters is not None:
             pulumi.set(__self__, "datacenters", datacenters)
         if datastore is not None:
             pulumi.set(__self__, "datastore", datastore)
         if insecure_flag is not None:
@@ -3547,97 +3096,64 @@
             pulumi.set(__self__, "vm_uuid", vm_uuid)
         if working_dir is not None:
             pulumi.set(__self__, "working_dir", working_dir)
 
     @property
     @pulumi.getter
     def datacenter(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @property
     @pulumi.getter
     def datacenters(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @property
     @pulumi.getter
     def datastore(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datastore")
 
     @property
     @pulumi.getter(name="insecureFlag")
     def insecure_flag(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "insecure_flag")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="vmName")
     def vm_name(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_name")
 
     @property
     @pulumi.getter(name="vmUuid")
     def vm_uuid(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_uuid")
 
     @property
     @pulumi.getter(name="workingDir")
     def working_dir(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "working_dir")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudConfigNetwork(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3654,26 +3170,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderVsphereCloudConfigNetwork.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  public_network: Optional[str] = None):
-        """
-        :param str public_network: (string)
-        """
         if public_network is not None:
             pulumi.set(__self__, "public_network", public_network)
 
     @property
     @pulumi.getter(name="publicNetwork")
     def public_network(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "public_network")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudConfigVirtualCenter(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3695,77 +3205,51 @@
     def __init__(__self__, *,
                  datacenters: str,
                  name: str,
                  password: str,
                  user: str,
                  port: Optional[str] = None,
                  soap_roundtrip_count: Optional[int] = None):
-        """
-        :param str datacenters: (string)
-        :param str name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param str password: Registry password (string)
-        :param str user: Registry user (string)
-        :param str port: Port used for SSH communication (string)
-        :param int soap_roundtrip_count: (int)
-        """
         pulumi.set(__self__, "datacenters", datacenters)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if soap_roundtrip_count is not None:
             pulumi.set(__self__, "soap_roundtrip_count", soap_roundtrip_count)
 
     @property
     @pulumi.getter
     def datacenters(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> str:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def user(self) -> str:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudConfigWorkspace(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3788,68 +3272,46 @@
 
     def __init__(__self__, *,
                  datacenter: str,
                  server: str,
                  default_datastore: Optional[str] = None,
                  folder: Optional[str] = None,
                  resourcepool_path: Optional[str] = None):
-        """
-        :param str datacenter: (string)
-        :param str server: (string)
-        :param str default_datastore: (string)
-        :param str folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param str resourcepool_path: (string)
-        """
         pulumi.set(__self__, "datacenter", datacenter)
         pulumi.set(__self__, "server", server)
         if default_datastore is not None:
             pulumi.set(__self__, "default_datastore", default_datastore)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if resourcepool_path is not None:
             pulumi.set(__self__, "resourcepool_path", resourcepool_path)
 
     @property
     @pulumi.getter
     def datacenter(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @property
     @pulumi.getter
     def server(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter(name="defaultDatastore")
     def default_datastore(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "default_datastore")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @property
     @pulumi.getter(name="resourcepoolPath")
     def resourcepool_path(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "resourcepool_path")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudProvider(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -3873,59 +3335,43 @@
     def __init__(__self__, *,
                  virtual_centers: Sequence['outputs.ClusterCloudProviderVsphereCloudProviderVirtualCenter'],
                  workspace: 'outputs.ClusterCloudProviderVsphereCloudProviderWorkspace',
                  disk: Optional['outputs.ClusterCloudProviderVsphereCloudProviderDisk'] = None,
                  global_: Optional['outputs.ClusterCloudProviderVsphereCloudProviderGlobal'] = None,
                  network: Optional['outputs.ClusterCloudProviderVsphereCloudProviderNetwork'] = None):
         """
-        :param Sequence['ClusterCloudProviderVsphereCloudProviderVirtualCenterArgs'] virtual_centers: (List)
-        :param 'ClusterCloudProviderVsphereCloudProviderWorkspaceArgs' workspace: (list maxitems:1)
-        :param 'ClusterCloudProviderVsphereCloudProviderDiskArgs' disk: (list maxitems:1)
-        :param 'ClusterCloudProviderVsphereCloudProviderGlobalArgs' global_: (list maxitems:1)
         :param 'ClusterCloudProviderVsphereCloudProviderNetworkArgs' network: RKE k8s cluster network configuration (list maxitems:1)
         """
         pulumi.set(__self__, "virtual_centers", virtual_centers)
         pulumi.set(__self__, "workspace", workspace)
         if disk is not None:
             pulumi.set(__self__, "disk", disk)
         if global_ is not None:
             pulumi.set(__self__, "global_", global_)
         if network is not None:
             pulumi.set(__self__, "network", network)
 
     @property
     @pulumi.getter(name="virtualCenters")
     def virtual_centers(self) -> Sequence['outputs.ClusterCloudProviderVsphereCloudProviderVirtualCenter']:
-        """
-        (List)
-        """
         return pulumi.get(self, "virtual_centers")
 
     @property
     @pulumi.getter
     def workspace(self) -> 'outputs.ClusterCloudProviderVsphereCloudProviderWorkspace':
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "workspace")
 
     @property
     @pulumi.getter
     def disk(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudProviderDisk']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "disk")
 
     @property
     @pulumi.getter(name="global")
     def global_(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudProviderGlobal']:
-        """
-        (list maxitems:1)
-        """
         return pulumi.get(self, "global_")
 
     @property
     @pulumi.getter
     def network(self) -> Optional['outputs.ClusterCloudProviderVsphereCloudProviderNetwork']:
         """
         RKE k8s cluster network configuration (list maxitems:1)
@@ -3950,26 +3396,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderVsphereCloudProviderDisk.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  scsi_controller_type: Optional[str] = None):
-        """
-        :param str scsi_controller_type: (string)
-        """
         if scsi_controller_type is not None:
             pulumi.set(__self__, "scsi_controller_type", scsi_controller_type)
 
     @property
     @pulumi.getter(name="scsiControllerType")
     def scsi_controller_type(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "scsi_controller_type")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudProviderGlobal(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4004,27 +3444,14 @@
                  password: Optional[str] = None,
                  port: Optional[str] = None,
                  soap_roundtrip_count: Optional[int] = None,
                  user: Optional[str] = None,
                  vm_name: Optional[str] = None,
                  vm_uuid: Optional[str] = None,
                  working_dir: Optional[str] = None):
-        """
-        :param str datacenter: (string)
-        :param str datacenters: (string)
-        :param str datastore: (string)
-        :param bool insecure_flag: (bool)
-        :param str password: Registry password (string)
-        :param str port: Port used for SSH communication (string)
-        :param int soap_roundtrip_count: (int)
-        :param str user: Registry user (string)
-        :param str vm_name: (string)
-        :param str vm_uuid: (string)
-        :param str working_dir: (string)
-        """
         if datacenter is not None:
             pulumi.set(__self__, "datacenter", datacenter)
         if datacenters is not None:
             pulumi.set(__self__, "datacenters", datacenters)
         if datastore is not None:
             pulumi.set(__self__, "datastore", datastore)
         if insecure_flag is not None:
@@ -4043,97 +3470,64 @@
             pulumi.set(__self__, "vm_uuid", vm_uuid)
         if working_dir is not None:
             pulumi.set(__self__, "working_dir", working_dir)
 
     @property
     @pulumi.getter
     def datacenter(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @property
     @pulumi.getter
     def datacenters(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @property
     @pulumi.getter
     def datastore(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "datastore")
 
     @property
     @pulumi.getter(name="insecureFlag")
     def insecure_flag(self) -> Optional[bool]:
-        """
-        (bool)
-        """
         return pulumi.get(self, "insecure_flag")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="vmName")
     def vm_name(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_name")
 
     @property
     @pulumi.getter(name="vmUuid")
     def vm_uuid(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "vm_uuid")
 
     @property
     @pulumi.getter(name="workingDir")
     def working_dir(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "working_dir")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudProviderNetwork(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4150,26 +3544,20 @@
 
     def get(self, key: str, default = None) -> Any:
         ClusterCloudProviderVsphereCloudProviderNetwork.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  public_network: Optional[str] = None):
-        """
-        :param str public_network: (string)
-        """
         if public_network is not None:
             pulumi.set(__self__, "public_network", public_network)
 
     @property
     @pulumi.getter(name="publicNetwork")
     def public_network(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "public_network")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudProviderVirtualCenter(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4191,77 +3579,51 @@
     def __init__(__self__, *,
                  datacenters: str,
                  name: str,
                  password: str,
                  user: str,
                  port: Optional[str] = None,
                  soap_roundtrip_count: Optional[int] = None):
-        """
-        :param str datacenters: (string)
-        :param str name: Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        :param str password: Registry password (string)
-        :param str user: Registry user (string)
-        :param str port: Port used for SSH communication (string)
-        :param int soap_roundtrip_count: (int)
-        """
         pulumi.set(__self__, "datacenters", datacenters)
         pulumi.set(__self__, "name", name)
         pulumi.set(__self__, "password", password)
         pulumi.set(__self__, "user", user)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if soap_roundtrip_count is not None:
             pulumi.set(__self__, "soap_roundtrip_count", soap_roundtrip_count)
 
     @property
     @pulumi.getter
     def datacenters(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenters")
 
     @property
     @pulumi.getter
     def name(self) -> str:
-        """
-        Name of virtualcenter config for Vsphere Cloud Provider config (string)
-        """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def password(self) -> str:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def user(self) -> str:
-        """
-        Registry user (string)
-        """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
-        """
-        Port used for SSH communication (string)
-        """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="soapRoundtripCount")
     def soap_roundtrip_count(self) -> Optional[int]:
-        """
-        (int)
-        """
         return pulumi.get(self, "soap_roundtrip_count")
 
 
 @pulumi.output_type
 class ClusterCloudProviderVsphereCloudProviderWorkspace(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4284,68 +3646,46 @@
 
     def __init__(__self__, *,
                  datacenter: str,
                  server: str,
                  default_datastore: Optional[str] = None,
                  folder: Optional[str] = None,
                  resourcepool_path: Optional[str] = None):
-        """
-        :param str datacenter: (string)
-        :param str server: (string)
-        :param str default_datastore: (string)
-        :param str folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param str resourcepool_path: (string)
-        """
         pulumi.set(__self__, "datacenter", datacenter)
         pulumi.set(__self__, "server", server)
         if default_datastore is not None:
             pulumi.set(__self__, "default_datastore", default_datastore)
         if folder is not None:
             pulumi.set(__self__, "folder", folder)
         if resourcepool_path is not None:
             pulumi.set(__self__, "resourcepool_path", resourcepool_path)
 
     @property
     @pulumi.getter
     def datacenter(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "datacenter")
 
     @property
     @pulumi.getter
     def server(self) -> str:
-        """
-        (string)
-        """
         return pulumi.get(self, "server")
 
     @property
     @pulumi.getter(name="defaultDatastore")
     def default_datastore(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "default_datastore")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @property
     @pulumi.getter(name="resourcepoolPath")
     def resourcepool_path(self) -> Optional[str]:
-        """
-        (string)
-        """
         return pulumi.get(self, "resourcepool_path")
 
 
 @pulumi.output_type
 class ClusterControlPlaneHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4363,37 +3703,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterControlPlaneHost.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  node_name: Optional[str] = None):
-        """
-        :param str address: Address ip for node (string)
-        :param str node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
 
 @pulumi.output_type
 class ClusterDns(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4419,19 +3749,19 @@
     def __init__(__self__, *,
                  node_selector: Optional[Mapping[str, Any]] = None,
                  nodelocal: Optional['outputs.ClusterDnsNodelocal'] = None,
                  provider: Optional[str] = None,
                  reverse_cidrs: Optional[Sequence[str]] = None,
                  upstream_nameservers: Optional[Sequence[str]] = None):
         """
-        :param Mapping[str, Any] node_selector: Node selector key pair (map)
-        :param 'ClusterDnsNodelocalArgs' nodelocal: Docker image for nodelocal (string)
-        :param str provider: Monitoring provider (string)
-        :param Sequence[str] reverse_cidrs: Reverse CIDRs  (list)
-        :param Sequence[str] upstream_nameservers: Upstream nameservers  (list)
+        :param Mapping[str, Any] node_selector: NodeSelector key pair
+        :param 'ClusterDnsNodelocalArgs' nodelocal: Nodelocal dns
+        :param str provider: DNS provider
+        :param Sequence[str] reverse_cidrs: ReverseCIDRs
+        :param Sequence[str] upstream_nameservers: Upstream nameservers
         """
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
         if nodelocal is not None:
             pulumi.set(__self__, "nodelocal", nodelocal)
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
@@ -4440,47 +3770,47 @@
         if upstream_nameservers is not None:
             pulumi.set(__self__, "upstream_nameservers", upstream_nameservers)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[Mapping[str, Any]]:
         """
-        Node selector key pair (map)
+        NodeSelector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional['outputs.ClusterDnsNodelocal']:
         """
-        Docker image for nodelocal (string)
+        Nodelocal dns
         """
         return pulumi.get(self, "nodelocal")
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[str]:
         """
-        Monitoring provider (string)
+        DNS provider
         """
         return pulumi.get(self, "provider")
 
     @property
     @pulumi.getter(name="reverseCidrs")
     def reverse_cidrs(self) -> Optional[Sequence[str]]:
         """
-        Reverse CIDRs  (list)
+        ReverseCIDRs
         """
         return pulumi.get(self, "reverse_cidrs")
 
     @property
     @pulumi.getter(name="upstreamNameservers")
     def upstream_nameservers(self) -> Optional[Sequence[str]]:
         """
-        Upstream nameservers  (list)
+        Upstream nameservers
         """
         return pulumi.get(self, "upstream_nameservers")
 
 
 @pulumi.output_type
 class ClusterDnsNodelocal(dict):
     @staticmethod
@@ -4502,35 +3832,31 @@
         ClusterDnsNodelocal.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  ip_address: Optional[str] = None,
                  node_selector: Optional[Mapping[str, Any]] = None):
         """
-        :param str ip_address: Nodelocal dns ip address (string)
-        :param Mapping[str, Any] node_selector: Node selector key pair (map)
+        :param Mapping[str, Any] node_selector: Node selector key pair
         """
         if ip_address is not None:
             pulumi.set(__self__, "ip_address", ip_address)
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
 
     @property
     @pulumi.getter(name="ipAddress")
     def ip_address(self) -> Optional[str]:
-        """
-        Nodelocal dns ip address (string)
-        """
         return pulumi.get(self, "ip_address")
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[Mapping[str, Any]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
 
 @pulumi.output_type
 class ClusterEtcdHost(dict):
     @staticmethod
@@ -4549,37 +3875,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterEtcdHost.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  node_name: Optional[str] = None):
-        """
-        :param str address: Address ip for node (string)
-        :param str node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
 
 @pulumi.output_type
 class ClusterInactiveHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4597,37 +3913,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterInactiveHost.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  node_name: Optional[str] = None):
-        """
-        :param str address: Address ip for node (string)
-        :param str node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
 
 
 @pulumi.output_type
 class ClusterIngress(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -4666,22 +3972,22 @@
                  https_port: Optional[int] = None,
                  network_mode: Optional[str] = None,
                  node_selector: Optional[Mapping[str, Any]] = None,
                  options: Optional[Mapping[str, Any]] = None,
                  provider: Optional[str] = None):
         """
         :param bool default_backend: Ingress Default Backend
-        :param str dns_policy: Ingress controller DNS policy. `ClusterFirstWithHostNet`, `ClusterFirst`, `Default`, and `None` are supported. [K8S dns Policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pod-s-dns-policy) (string)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param int http_port: Ingress controller http port (int)
-        :param int https_port: Ingress controller https port (int)
-        :param str network_mode: Networt mode for the ingress controller. `hostNetwork`, `hostPort` and `none` are supported (string)
-        :param Mapping[str, Any] node_selector: Node selector key pair (map)
-        :param Mapping[str, Any] options: Network provider options (map)
-        :param str provider: Monitoring provider (string)
+        :param str dns_policy: Ingress controller dns policy
+        :param Mapping[str, Any] extra_args: Extra arguments for the ingress controller
+        :param int http_port: Ingress controller http port
+        :param int https_port: Ingress controller https port
+        :param str network_mode: Ingress controller network mode
+        :param Mapping[str, Any] node_selector: Node selector key pair
+        :param Mapping[str, Any] options: Ingress controller options
+        :param str provider: Ingress controller provider
         """
         if default_backend is not None:
             pulumi.set(__self__, "default_backend", default_backend)
         if dns_policy is not None:
             pulumi.set(__self__, "dns_policy", dns_policy)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -4706,71 +4012,71 @@
         """
         return pulumi.get(self, "default_backend")
 
     @property
     @pulumi.getter(name="dnsPolicy")
     def dns_policy(self) -> Optional[str]:
         """
-        Ingress controller DNS policy. `ClusterFirstWithHostNet`, `ClusterFirst`, `Default`, and `None` are supported. [K8S dns Policy](https://kubernetes.io/docs/concepts/services-networking/dns-pod-service/#pod-s-dns-policy) (string)
+        Ingress controller dns policy
         """
         return pulumi.get(self, "dns_policy")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments for the ingress controller
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="httpPort")
     def http_port(self) -> Optional[int]:
         """
-        Ingress controller http port (int)
+        Ingress controller http port
         """
         return pulumi.get(self, "http_port")
 
     @property
     @pulumi.getter(name="httpsPort")
     def https_port(self) -> Optional[int]:
         """
-        Ingress controller https port (int)
+        Ingress controller https port
         """
         return pulumi.get(self, "https_port")
 
     @property
     @pulumi.getter(name="networkMode")
     def network_mode(self) -> Optional[str]:
         """
-        Networt mode for the ingress controller. `hostNetwork`, `hostPort` and `none` are supported (string)
+        Ingress controller network mode
         """
         return pulumi.get(self, "network_mode")
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[Mapping[str, Any]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @property
     @pulumi.getter
     def options(self) -> Optional[Mapping[str, Any]]:
         """
-        Network provider options (map)
+        Ingress controller options
         """
         return pulumi.get(self, "options")
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[str]:
         """
-        Monitoring provider (string)
+        Ingress controller provider
         """
         return pulumi.get(self, "provider")
 
 
 @pulumi.output_type
 class ClusterMonitoring(dict):
     @staticmethod
@@ -4791,46 +4097,46 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  node_selector: Optional[Mapping[str, Any]] = None,
                  options: Optional[Mapping[str, Any]] = None,
                  provider: Optional[str] = None):
         """
-        :param Mapping[str, Any] node_selector: Node selector key pair (map)
-        :param Mapping[str, Any] options: Network provider options (map)
-        :param str provider: Monitoring provider (string)
+        :param Mapping[str, Any] node_selector: Node selector key pair
+        :param Mapping[str, Any] options: Monitoring options
+        :param str provider: Monitoring provider
         """
         if node_selector is not None:
             pulumi.set(__self__, "node_selector", node_selector)
         if options is not None:
             pulumi.set(__self__, "options", options)
         if provider is not None:
             pulumi.set(__self__, "provider", provider)
 
     @property
     @pulumi.getter(name="nodeSelector")
     def node_selector(self) -> Optional[Mapping[str, Any]]:
         """
-        Node selector key pair (map)
+        Node selector key pair
         """
         return pulumi.get(self, "node_selector")
 
     @property
     @pulumi.getter
     def options(self) -> Optional[Mapping[str, Any]]:
         """
-        Network provider options (map)
+        Monitoring options
         """
         return pulumi.get(self, "options")
 
     @property
     @pulumi.getter
     def provider(self) -> Optional[str]:
         """
-        Monitoring provider (string)
+        Monitoring provider
         """
         return pulumi.get(self, "provider")
 
 
 @pulumi.output_type
 class ClusterNetwork(dict):
     @staticmethod
@@ -4864,22 +4170,22 @@
                  canal_network_provider: Optional['outputs.ClusterNetworkCanalNetworkProvider'] = None,
                  flannel_network_provider: Optional['outputs.ClusterNetworkFlannelNetworkProvider'] = None,
                  mtu: Optional[int] = None,
                  options: Optional[Mapping[str, Any]] = None,
                  plugin: Optional[str] = None,
                  weave_network_provider: Optional['outputs.ClusterNetworkWeaveNetworkProvider'] = None):
         """
-        :param 'ClusterNetworkAciNetworkProviderArgs' aci_network_provider: Aci network provider config (list maxitems:1)
-        :param 'ClusterNetworkCalicoNetworkProviderArgs' calico_network_provider: Calico network provider config (list maxitems:1)
-        :param 'ClusterNetworkCanalNetworkProviderArgs' canal_network_provider: Canal network provider config (list maxitems:1)
-        :param 'ClusterNetworkFlannelNetworkProviderArgs' flannel_network_provider: Flannel network provider config (list maxitems:1)
-        :param int mtu: Network provider MTU. Default `0` (int)
-        :param Mapping[str, Any] options: Network provider options (map)
-        :param str plugin: Network provider plugin. `calico`, `canal` (default), `flannel`, `none` and `weave` are supported. (string)
-        :param 'ClusterNetworkWeaveNetworkProviderArgs' weave_network_provider: Weave network provider config (list maxitems:1)
+        :param 'ClusterNetworkAciNetworkProviderArgs' aci_network_provider: Aci network provider config
+        :param 'ClusterNetworkCalicoNetworkProviderArgs' calico_network_provider: Calico network provider config
+        :param 'ClusterNetworkCanalNetworkProviderArgs' canal_network_provider: Canal network provider config
+        :param 'ClusterNetworkFlannelNetworkProviderArgs' flannel_network_provider: Flannel network provider config
+        :param int mtu: Network provider MTU
+        :param Mapping[str, Any] options: Network provider options
+        :param str plugin: Network provider plugin
+        :param 'ClusterNetworkWeaveNetworkProviderArgs' weave_network_provider: Weave network provider config
         """
         if aci_network_provider is not None:
             pulumi.set(__self__, "aci_network_provider", aci_network_provider)
         if calico_network_provider is not None:
             pulumi.set(__self__, "calico_network_provider", calico_network_provider)
         if canal_network_provider is not None:
             pulumi.set(__self__, "canal_network_provider", canal_network_provider)
@@ -4894,71 +4200,71 @@
         if weave_network_provider is not None:
             pulumi.set(__self__, "weave_network_provider", weave_network_provider)
 
     @property
     @pulumi.getter(name="aciNetworkProvider")
     def aci_network_provider(self) -> Optional['outputs.ClusterNetworkAciNetworkProvider']:
         """
-        Aci network provider config (list maxitems:1)
+        Aci network provider config
         """
         return pulumi.get(self, "aci_network_provider")
 
     @property
     @pulumi.getter(name="calicoNetworkProvider")
     def calico_network_provider(self) -> Optional['outputs.ClusterNetworkCalicoNetworkProvider']:
         """
-        Calico network provider config (list maxitems:1)
+        Calico network provider config
         """
         return pulumi.get(self, "calico_network_provider")
 
     @property
     @pulumi.getter(name="canalNetworkProvider")
     def canal_network_provider(self) -> Optional['outputs.ClusterNetworkCanalNetworkProvider']:
         """
-        Canal network provider config (list maxitems:1)
+        Canal network provider config
         """
         return pulumi.get(self, "canal_network_provider")
 
     @property
     @pulumi.getter(name="flannelNetworkProvider")
     def flannel_network_provider(self) -> Optional['outputs.ClusterNetworkFlannelNetworkProvider']:
         """
-        Flannel network provider config (list maxitems:1)
+        Flannel network provider config
         """
         return pulumi.get(self, "flannel_network_provider")
 
     @property
     @pulumi.getter
     def mtu(self) -> Optional[int]:
         """
-        Network provider MTU. Default `0` (int)
+        Network provider MTU
         """
         return pulumi.get(self, "mtu")
 
     @property
     @pulumi.getter
     def options(self) -> Optional[Mapping[str, Any]]:
         """
-        Network provider options (map)
+        Network provider options
         """
         return pulumi.get(self, "options")
 
     @property
     @pulumi.getter
     def plugin(self) -> Optional[str]:
         """
-        Network provider plugin. `calico`, `canal` (default), `flannel`, `none` and `weave` are supported. (string)
+        Network provider plugin
         """
         return pulumi.get(self, "plugin")
 
     @property
     @pulumi.getter(name="weaveNetworkProvider")
     def weave_network_provider(self) -> Optional['outputs.ClusterNetworkWeaveNetworkProvider']:
         """
-        Weave network provider config (list maxitems:1)
+        Weave network provider config
         """
         return pulumi.get(self, "weave_network_provider")
 
 
 @pulumi.output_type
 class ClusterNetworkAciNetworkProvider(dict):
     @staticmethod
@@ -5039,40 +4345,14 @@
                  system_id: str,
                  token: str,
                  vrf_name: str,
                  vrf_tenant: str,
                  snat_port_range_end: Optional[str] = None,
                  snat_port_range_start: Optional[str] = None,
                  snat_ports_per_node: Optional[str] = None):
-        """
-        :param str aep: Attachment entity profile name on aci (string)
-        :param Sequence[str] apic_hosts: Ip address for apic hosts (list)
-        :param str apic_user_crt: Base64 encoded certificate for aci apic user (string)
-        :param str apic_user_key: Base64 encoded private key for aci apic user (string)
-        :param str apic_user_name: User name for aci apic (string)
-        :param str encap_type: One of the supported encap types for aci(vlan/vxlan) (string)
-        :param str extern_dynamic: Subnet to use for dynamic external IPs on aci (string)
-               * `extern_static"` - (Required) Subnet to use for static external IPs on aci (string)
-        :param str infra_vlan: Vlan for infra network on aci (string)
-        :param str kube_api_vlan: Vlan for node network on aci (string)
-        :param str l3out: L3Out on aci (string)
-        :param Sequence[str] l3out_external_networks: L3out external networks on aci (list)
-        :param str mcast_range_end: Mcast range end address for endpoint groups on aci (string)
-        :param str mcast_range_start: Mcast range start address for endpoint groups on aci (string)
-        :param str node_subnet: Kubernetes node address subnet (string)
-        :param str node_svc_subnet: Subnet to use for service graph endpoints on aci (string)
-        :param str service_vlan: Vlan for service graph nodes on aci (string)
-        :param str system_id: Unique suffix for all cluster related objects in aci (string)
-        :param str token: UUID for this version of the input configuration (string)
-        :param str vrf_name: VRF Name on aci (string)
-        :param str vrf_tenant: Tenant for VRF on aci (string)
-        :param str snat_port_range_end: Port end range for Source Network Address Translation on aci (string)
-        :param str snat_port_range_start: Port start range for Source Network Address Translation on aci (string)
-        :param str snat_ports_per_node: Ports per node for Source Network Address Translation on aci (string)
-        """
         pulumi.set(__self__, "aep", aep)
         pulumi.set(__self__, "apic_hosts", apic_hosts)
         pulumi.set(__self__, "apic_user_crt", apic_user_crt)
         pulumi.set(__self__, "apic_user_key", apic_user_key)
         pulumi.set(__self__, "apic_user_name", apic_user_name)
         pulumi.set(__self__, "encap_type", encap_type)
         pulumi.set(__self__, "extern_dynamic", extern_dynamic)
@@ -5096,199 +4376,129 @@
             pulumi.set(__self__, "snat_port_range_start", snat_port_range_start)
         if snat_ports_per_node is not None:
             pulumi.set(__self__, "snat_ports_per_node", snat_ports_per_node)
 
     @property
     @pulumi.getter
     def aep(self) -> str:
-        """
-        Attachment entity profile name on aci (string)
-        """
         return pulumi.get(self, "aep")
 
     @property
     @pulumi.getter(name="apicHosts")
     def apic_hosts(self) -> Sequence[str]:
-        """
-        Ip address for apic hosts (list)
-        """
         return pulumi.get(self, "apic_hosts")
 
     @property
     @pulumi.getter(name="apicUserCrt")
     def apic_user_crt(self) -> str:
-        """
-        Base64 encoded certificate for aci apic user (string)
-        """
         return pulumi.get(self, "apic_user_crt")
 
     @property
     @pulumi.getter(name="apicUserKey")
     def apic_user_key(self) -> str:
-        """
-        Base64 encoded private key for aci apic user (string)
-        """
         return pulumi.get(self, "apic_user_key")
 
     @property
     @pulumi.getter(name="apicUserName")
     def apic_user_name(self) -> str:
-        """
-        User name for aci apic (string)
-        """
         return pulumi.get(self, "apic_user_name")
 
     @property
     @pulumi.getter(name="encapType")
     def encap_type(self) -> str:
-        """
-        One of the supported encap types for aci(vlan/vxlan) (string)
-        """
         return pulumi.get(self, "encap_type")
 
     @property
     @pulumi.getter(name="externDynamic")
     def extern_dynamic(self) -> str:
-        """
-        Subnet to use for dynamic external IPs on aci (string)
-        * `extern_static"` - (Required) Subnet to use for static external IPs on aci (string)
-        """
         return pulumi.get(self, "extern_dynamic")
 
     @property
     @pulumi.getter(name="externStatic")
     def extern_static(self) -> str:
         return pulumi.get(self, "extern_static")
 
     @property
     @pulumi.getter(name="infraVlan")
     def infra_vlan(self) -> str:
-        """
-        Vlan for infra network on aci (string)
-        """
         return pulumi.get(self, "infra_vlan")
 
     @property
     @pulumi.getter(name="kubeApiVlan")
     def kube_api_vlan(self) -> str:
-        """
-        Vlan for node network on aci (string)
-        """
         return pulumi.get(self, "kube_api_vlan")
 
     @property
     @pulumi.getter
     def l3out(self) -> str:
-        """
-        L3Out on aci (string)
-        """
         return pulumi.get(self, "l3out")
 
     @property
     @pulumi.getter(name="l3outExternalNetworks")
     def l3out_external_networks(self) -> Sequence[str]:
-        """
-        L3out external networks on aci (list)
-        """
         return pulumi.get(self, "l3out_external_networks")
 
     @property
     @pulumi.getter(name="mcastRangeEnd")
     def mcast_range_end(self) -> str:
-        """
-        Mcast range end address for endpoint groups on aci (string)
-        """
         return pulumi.get(self, "mcast_range_end")
 
     @property
     @pulumi.getter(name="mcastRangeStart")
     def mcast_range_start(self) -> str:
-        """
-        Mcast range start address for endpoint groups on aci (string)
-        """
         return pulumi.get(self, "mcast_range_start")
 
     @property
     @pulumi.getter(name="nodeSubnet")
     def node_subnet(self) -> str:
-        """
-        Kubernetes node address subnet (string)
-        """
         return pulumi.get(self, "node_subnet")
 
     @property
     @pulumi.getter(name="nodeSvcSubnet")
     def node_svc_subnet(self) -> str:
-        """
-        Subnet to use for service graph endpoints on aci (string)
-        """
         return pulumi.get(self, "node_svc_subnet")
 
     @property
     @pulumi.getter(name="serviceVlan")
     def service_vlan(self) -> str:
-        """
-        Vlan for service graph nodes on aci (string)
-        """
         return pulumi.get(self, "service_vlan")
 
     @property
     @pulumi.getter(name="systemId")
     def system_id(self) -> str:
-        """
-        Unique suffix for all cluster related objects in aci (string)
-        """
         return pulumi.get(self, "system_id")
 
     @property
     @pulumi.getter
     def token(self) -> str:
-        """
-        UUID for this version of the input configuration (string)
-        """
         return pulumi.get(self, "token")
 
     @property
     @pulumi.getter(name="vrfName")
     def vrf_name(self) -> str:
-        """
-        VRF Name on aci (string)
-        """
         return pulumi.get(self, "vrf_name")
 
     @property
     @pulumi.getter(name="vrfTenant")
     def vrf_tenant(self) -> str:
-        """
-        Tenant for VRF on aci (string)
-        """
         return pulumi.get(self, "vrf_tenant")
 
     @property
     @pulumi.getter(name="snatPortRangeEnd")
     def snat_port_range_end(self) -> Optional[str]:
-        """
-        Port end range for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_port_range_end")
 
     @property
     @pulumi.getter(name="snatPortRangeStart")
     def snat_port_range_start(self) -> Optional[str]:
-        """
-        Port start range for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_port_range_start")
 
     @property
     @pulumi.getter(name="snatPortsPerNode")
     def snat_ports_per_node(self) -> Optional[str]:
-        """
-        Ports per node for Source Network Address Translation on aci (string)
-        """
         return pulumi.get(self, "snat_ports_per_node")
 
 
 @pulumi.output_type
 class ClusterNetworkCalicoNetworkProvider(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5324,63 +4534,45 @@
         return pulumi.get(self, "cloud_provider")
 
 
 @pulumi.output_type
 class ClusterNetworkCanalNetworkProvider(dict):
     def __init__(__self__, *,
                  iface: Optional[str] = None):
-        """
-        :param str iface: Flannel network interface (string)
-        """
         if iface is not None:
             pulumi.set(__self__, "iface", iface)
 
     @property
     @pulumi.getter
     def iface(self) -> Optional[str]:
-        """
-        Flannel network interface (string)
-        """
         return pulumi.get(self, "iface")
 
 
 @pulumi.output_type
 class ClusterNetworkFlannelNetworkProvider(dict):
     def __init__(__self__, *,
                  iface: Optional[str] = None):
-        """
-        :param str iface: Flannel network interface (string)
-        """
         if iface is not None:
             pulumi.set(__self__, "iface", iface)
 
     @property
     @pulumi.getter
     def iface(self) -> Optional[str]:
-        """
-        Flannel network interface (string)
-        """
         return pulumi.get(self, "iface")
 
 
 @pulumi.output_type
 class ClusterNetworkWeaveNetworkProvider(dict):
     def __init__(__self__, *,
                  password: str):
-        """
-        :param str password: Registry password (string)
-        """
         pulumi.set(__self__, "password", password)
 
     @property
     @pulumi.getter
     def password(self) -> str:
-        """
-        Registry password (string)
-        """
         return pulumi.get(self, "password")
 
 
 @pulumi.output_type
 class ClusterNode(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5431,30 +4623,30 @@
                  ssh_agent_auth: Optional[bool] = None,
                  ssh_cert: Optional[str] = None,
                  ssh_cert_path: Optional[str] = None,
                  ssh_key: Optional[str] = None,
                  ssh_key_path: Optional[str] = None,
                  taints: Optional[Sequence['outputs.ClusterNodeTaint']] = None):
         """
-        :param str address: Address ip for node (string)
-        :param Sequence[str] roles: Node roles in k8s cluster. `controlplane`, `etcd` and `worker` are supported. (list)
-        :param str user: Registry user (string)
-        :param str docker_socket: Docker socket on the node that will be used in tunneling (string)
-        :param str hostname_override: Hostname override for node (string)
-        :param str internal_address: Internal address that will be used for components communication (string)
-        :param Mapping[str, Any] labels: Node labels (map)
-        :param str node_name: Name of the host provisioned via docker machine (string)
-        :param str port: Port used for SSH communication (string)
+        :param str address: IP or FQDN that is fully resolvable and used for SSH communication
+        :param Sequence[str] roles: Node roles in k8s cluster [controlplane/worker/etcd])
+        :param str user: SSH user that will be used by RKE
+        :param str docker_socket: Docker socket on the node that will be used in tunneling
+        :param str hostname_override: Hostname override
+        :param str internal_address: Internal address that will be used for components communication
+        :param Mapping[str, Any] labels: Node Labels
+        :param str node_name: Name of the host provisioned via docker machine
+        :param str port: Port used for SSH communication
         :param str roles_deprecated: Node role in kubernetes cluster [controlplane/worker/etcd], specified by a comma-separated string
         :param bool ssh_agent_auth: SSH Agent Auth enable (bool)
-        :param str ssh_cert: SSH Certificate (string)
+        :param str ssh_cert: SSH Certificate
         :param str ssh_cert_path: SSH Certificate Path (string)
-        :param str ssh_key: SSH Private Key (string)
+        :param str ssh_key: SSH Private Key
         :param str ssh_key_path: SSH Private Key Path (string)
-        :param Sequence['ClusterNodeTaintArgs'] taints: Node taints (list)
+        :param Sequence['ClusterNodeTaintArgs'] taints: Node taints
         """
         pulumi.set(__self__, "address", address)
         pulumi.set(__self__, "roles", roles)
         pulumi.set(__self__, "user", user)
         if docker_socket is not None:
             pulumi.set(__self__, "docker_socket", docker_socket)
         if hostname_override is not None:
@@ -5482,79 +4674,79 @@
         if taints is not None:
             pulumi.set(__self__, "taints", taints)
 
     @property
     @pulumi.getter
     def address(self) -> str:
         """
-        Address ip for node (string)
+        IP or FQDN that is fully resolvable and used for SSH communication
         """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter
     def roles(self) -> Sequence[str]:
         """
-        Node roles in k8s cluster. `controlplane`, `etcd` and `worker` are supported. (list)
+        Node roles in k8s cluster [controlplane/worker/etcd])
         """
         return pulumi.get(self, "roles")
 
     @property
     @pulumi.getter
     def user(self) -> str:
         """
-        Registry user (string)
+        SSH user that will be used by RKE
         """
         return pulumi.get(self, "user")
 
     @property
     @pulumi.getter(name="dockerSocket")
     def docker_socket(self) -> Optional[str]:
         """
-        Docker socket on the node that will be used in tunneling (string)
+        Docker socket on the node that will be used in tunneling
         """
         return pulumi.get(self, "docker_socket")
 
     @property
     @pulumi.getter(name="hostnameOverride")
     def hostname_override(self) -> Optional[str]:
         """
-        Hostname override for node (string)
+        Hostname override
         """
         return pulumi.get(self, "hostname_override")
 
     @property
     @pulumi.getter(name="internalAddress")
     def internal_address(self) -> Optional[str]:
         """
-        Internal address that will be used for components communication (string)
+        Internal address that will be used for components communication
         """
         return pulumi.get(self, "internal_address")
 
     @property
     @pulumi.getter
     def labels(self) -> Optional[Mapping[str, Any]]:
         """
-        Node labels (map)
+        Node Labels
         """
         return pulumi.get(self, "labels")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
         """
-        Name of the host provisioned via docker machine (string)
+        Name of the host provisioned via docker machine
         """
         return pulumi.get(self, "node_name")
 
     @property
     @pulumi.getter
     def port(self) -> Optional[str]:
         """
-        Port used for SSH communication (string)
+        Port used for SSH communication
         """
         return pulumi.get(self, "port")
 
     @property
     @pulumi.getter(name="rolesDeprecated")
     def roles_deprecated(self) -> Optional[str]:
         """
@@ -5573,15 +4765,15 @@
         """
         return pulumi.get(self, "ssh_agent_auth")
 
     @property
     @pulumi.getter(name="sshCert")
     def ssh_cert(self) -> Optional[str]:
         """
-        SSH Certificate (string)
+        SSH Certificate
         """
         return pulumi.get(self, "ssh_cert")
 
     @property
     @pulumi.getter(name="sshCertPath")
     def ssh_cert_path(self) -> Optional[str]:
         """
@@ -5589,15 +4781,15 @@
         """
         return pulumi.get(self, "ssh_cert_path")
 
     @property
     @pulumi.getter(name="sshKey")
     def ssh_key(self) -> Optional[str]:
         """
-        SSH Private Key (string)
+        SSH Private Key
         """
         return pulumi.get(self, "ssh_key")
 
     @property
     @pulumi.getter(name="sshKeyPath")
     def ssh_key_path(self) -> Optional[str]:
         """
@@ -5605,57 +4797,43 @@
         """
         return pulumi.get(self, "ssh_key_path")
 
     @property
     @pulumi.getter
     def taints(self) -> Optional[Sequence['outputs.ClusterNodeTaint']]:
         """
-        Node taints (list)
+        Node taints
         """
         return pulumi.get(self, "taints")
 
 
 @pulumi.output_type
 class ClusterNodeTaint(dict):
     def __init__(__self__, *,
                  key: str,
                  value: str,
                  effect: Optional[str] = None):
-        """
-        :param str key: TLS key for etcd service (string)
-        :param str value: Taint value (string)
-        :param str effect: Taint effect. `NoExecute`, `NoSchedule` (default) and `PreferNoSchedule` are supported (string)
-        """
         pulumi.set(__self__, "key", key)
         pulumi.set(__self__, "value", value)
         if effect is not None:
             pulumi.set(__self__, "effect", effect)
 
     @property
     @pulumi.getter
     def key(self) -> str:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def value(self) -> str:
-        """
-        Taint value (string)
-        """
         return pulumi.get(self, "value")
 
     @property
     @pulumi.getter
     def effect(self) -> Optional[str]:
-        """
-        Taint effect. `NoExecute`, `NoSchedule` (default) and `PreferNoSchedule` are supported (string)
-        """
         return pulumi.get(self, "effect")
 
 
 @pulumi.output_type
 class ClusterPrivateRegistry(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -5676,56 +4854,56 @@
 
     def __init__(__self__, *,
                  url: str,
                  is_default: Optional[bool] = None,
                  password: Optional[str] = None,
                  user: Optional[str] = None):
         """
-        :param str url: Registry URL (string)
-        :param bool is_default: Set as default registry. Default `false` (bool)
-        :param str password: Registry password (string)
-        :param str user: Registry user (string)
+        :param str url: Registry URL
+        :param bool is_default: Set as default registry
+        :param str password: Registry password
+        :param str user: Registry user
         """
         pulumi.set(__self__, "url", url)
         if is_default is not None:
             pulumi.set(__self__, "is_default", is_default)
         if password is not None:
             pulumi.set(__self__, "password", password)
         if user is not None:
             pulumi.set(__self__, "user", user)
 
     @property
     @pulumi.getter
     def url(self) -> str:
         """
-        Registry URL (string)
+        Registry URL
         """
         return pulumi.get(self, "url")
 
     @property
     @pulumi.getter(name="isDefault")
     def is_default(self) -> Optional[bool]:
         """
-        Set as default registry. Default `false` (bool)
+        Set as default registry
         """
         return pulumi.get(self, "is_default")
 
     @property
     @pulumi.getter
     def password(self) -> Optional[str]:
         """
-        Registry password (string)
+        Registry password
         """
         return pulumi.get(self, "password")
 
     @property
     @pulumi.getter
     def user(self) -> Optional[str]:
         """
-        Registry user (string)
+        Registry user
         """
         return pulumi.get(self, "user")
 
 
 @pulumi.output_type
 class ClusterRestore(dict):
     @staticmethod
@@ -5746,15 +4924,15 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  restore: Optional[bool] = None,
                  snapshot_name: Optional[str] = None):
         """
         :param bool restore: RKE k8s cluster restore configuration (list maxitems:1)
-        :param str snapshot_name: Snapshot name (string)
+        :param str snapshot_name: Snapshot name
         """
         if restore is not None:
             pulumi.set(__self__, "restore", restore)
         if snapshot_name is not None:
             pulumi.set(__self__, "snapshot_name", snapshot_name)
 
     @property
@@ -5765,15 +4943,15 @@
         """
         return pulumi.get(self, "restore")
 
     @property
     @pulumi.getter(name="snapshotName")
     def snapshot_name(self) -> Optional[str]:
         """
-        Snapshot name (string)
+        Snapshot name
         """
         return pulumi.get(self, "snapshot_name")
 
 
 @pulumi.output_type
 class ClusterRotateCertificates(dict):
     @staticmethod
@@ -5793,27 +4971,27 @@
         ClusterRotateCertificates.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  ca_certificates: Optional[bool] = None,
                  services: Optional[Sequence[str]] = None):
         """
-        :param bool ca_certificates: Rotate CA Certificates. Default `false` (bool)
+        :param bool ca_certificates: Rotate CA Certificates
         :param Sequence[str] services: RKE k8s cluster services (list maxitems:1)
         """
         if ca_certificates is not None:
             pulumi.set(__self__, "ca_certificates", ca_certificates)
         if services is not None:
             pulumi.set(__self__, "services", services)
 
     @property
     @pulumi.getter(name="caCertificates")
     def ca_certificates(self) -> Optional[bool]:
         """
-        Rotate CA Certificates. Default `false` (bool)
+        Rotate CA Certificates
         """
         return pulumi.get(self, "ca_certificates")
 
     @property
     @pulumi.getter
     def services(self) -> Optional[Sequence[str]]:
         """
@@ -5932,51 +5110,15 @@
                  nginx_proxy: Optional[str] = None,
                  nodelocal: Optional[str] = None,
                  pod_infra_container: Optional[str] = None,
                  weave_cni: Optional[str] = None,
                  weave_node: Optional[str] = None,
                  windows_pod_infra_container: Optional[str] = None):
         """
-        :param str aci_cni_deploy_container: Docker image for aci_cni_deploy_container (string)
-        :param str aci_controller_container: Docker image for aci_controller_container (string)
-        :param str aci_host_container: Docker image for aci_host_container (string)
-        :param str aci_mcast_container: Docker image for aci_mcast_container (string)
-        :param str aci_opflex_container: Docker image for aci_opflex_container (string)
-        :param str aci_ovs_container: Docker image for aci_ovs_container (string)
-        :param str alpine: Docker image for alpine (string)
-        :param str calico_cni: Docker image for calico_cni (string)
-        :param str calico_controllers: Docker image for calico_controllers (string)
-        :param str calico_ctl: Docker image for calico_ctl (string)
-        :param str calico_flex_vol: Docker image for calico_flex_vol (string)
-        :param str calico_node: Docker image for calico_node (string)
-        :param str canal_cni: Docker image for canal_cni (string)
-        :param str canal_flannel: Docker image for canal_flannel (string)
-        :param str canal_flex_vol: Docker image for canal_flex_vol (string)
-        :param str canal_node: Docker image for canal_node (string)
-        :param str cert_downloader: Docker image for cert_downloader (string)
-        :param str coredns: Docker image for coredns (string)
-        :param str coredns_autoscaler: Docker image for coredns_autoscaler (string)
-        :param str dnsmasq: Docker image for dnsmasq (string)
-        :param str etcd: Docker image for etcd (string)
-        :param str flannel: Docker image for flannel (string)
-        :param str flannel_cni: Docker image for flannel_cni (string)
         :param str ingress: RKE k8s cluster ingress controller configuration (list maxitems:1)
-        :param str ingress_backend: Docker image for ingress_backend (string)
-        :param str kube_dns: Docker image for kube_dns (string)
-        :param str kube_dns_autoscaler: Docker image for kube_dns_autoscaler (string)
-        :param str kube_dns_sidecar: Docker image for kube_dns_sidecar (string)
-        :param str kubernetes: Docker image for kubernetes (string)
-        :param str kubernetes_services_sidecar: Docker image for kubernetes_services_sidecar (string)
-        :param str metrics_server: Docker image for metrics_server (string)
-        :param str nginx_proxy: Docker image for nginx_proxy (string)
-        :param str nodelocal: Docker image for nodelocal (string)
-        :param str pod_infra_container: Docker image for pod_infra_container (string)
-        :param str weave_cni: Docker image for weave_cni (string)
-        :param str weave_node: Docker image for weave_node (string)
-        :param str windows_pod_infra_container: Docker image for windows_pod_infra_container (string)
         """
         if aci_cni_deploy_container is not None:
             pulumi.set(__self__, "aci_cni_deploy_container", aci_cni_deploy_container)
         if aci_controller_container is not None:
             pulumi.set(__self__, "aci_controller_container", aci_controller_container)
         if aci_host_container is not None:
             pulumi.set(__self__, "aci_host_container", aci_host_container)
@@ -6048,305 +5190,197 @@
             pulumi.set(__self__, "weave_node", weave_node)
         if windows_pod_infra_container is not None:
             pulumi.set(__self__, "windows_pod_infra_container", windows_pod_infra_container)
 
     @property
     @pulumi.getter(name="aciCniDeployContainer")
     def aci_cni_deploy_container(self) -> Optional[str]:
-        """
-        Docker image for aci_cni_deploy_container (string)
-        """
         return pulumi.get(self, "aci_cni_deploy_container")
 
     @property
     @pulumi.getter(name="aciControllerContainer")
     def aci_controller_container(self) -> Optional[str]:
-        """
-        Docker image for aci_controller_container (string)
-        """
         return pulumi.get(self, "aci_controller_container")
 
     @property
     @pulumi.getter(name="aciHostContainer")
     def aci_host_container(self) -> Optional[str]:
-        """
-        Docker image for aci_host_container (string)
-        """
         return pulumi.get(self, "aci_host_container")
 
     @property
     @pulumi.getter(name="aciMcastContainer")
     def aci_mcast_container(self) -> Optional[str]:
-        """
-        Docker image for aci_mcast_container (string)
-        """
         return pulumi.get(self, "aci_mcast_container")
 
     @property
     @pulumi.getter(name="aciOpflexContainer")
     def aci_opflex_container(self) -> Optional[str]:
-        """
-        Docker image for aci_opflex_container (string)
-        """
         return pulumi.get(self, "aci_opflex_container")
 
     @property
     @pulumi.getter(name="aciOvsContainer")
     def aci_ovs_container(self) -> Optional[str]:
-        """
-        Docker image for aci_ovs_container (string)
-        """
         return pulumi.get(self, "aci_ovs_container")
 
     @property
     @pulumi.getter
     def alpine(self) -> Optional[str]:
-        """
-        Docker image for alpine (string)
-        """
         return pulumi.get(self, "alpine")
 
     @property
     @pulumi.getter(name="calicoCni")
     def calico_cni(self) -> Optional[str]:
-        """
-        Docker image for calico_cni (string)
-        """
         return pulumi.get(self, "calico_cni")
 
     @property
     @pulumi.getter(name="calicoControllers")
     def calico_controllers(self) -> Optional[str]:
-        """
-        Docker image for calico_controllers (string)
-        """
         return pulumi.get(self, "calico_controllers")
 
     @property
     @pulumi.getter(name="calicoCtl")
     def calico_ctl(self) -> Optional[str]:
-        """
-        Docker image for calico_ctl (string)
-        """
         return pulumi.get(self, "calico_ctl")
 
     @property
     @pulumi.getter(name="calicoFlexVol")
     def calico_flex_vol(self) -> Optional[str]:
-        """
-        Docker image for calico_flex_vol (string)
-        """
         return pulumi.get(self, "calico_flex_vol")
 
     @property
     @pulumi.getter(name="calicoNode")
     def calico_node(self) -> Optional[str]:
-        """
-        Docker image for calico_node (string)
-        """
         return pulumi.get(self, "calico_node")
 
     @property
     @pulumi.getter(name="canalCni")
     def canal_cni(self) -> Optional[str]:
-        """
-        Docker image for canal_cni (string)
-        """
         return pulumi.get(self, "canal_cni")
 
     @property
     @pulumi.getter(name="canalFlannel")
     def canal_flannel(self) -> Optional[str]:
-        """
-        Docker image for canal_flannel (string)
-        """
         return pulumi.get(self, "canal_flannel")
 
     @property
     @pulumi.getter(name="canalFlexVol")
     def canal_flex_vol(self) -> Optional[str]:
-        """
-        Docker image for canal_flex_vol (string)
-        """
         return pulumi.get(self, "canal_flex_vol")
 
     @property
     @pulumi.getter(name="canalNode")
     def canal_node(self) -> Optional[str]:
-        """
-        Docker image for canal_node (string)
-        """
         return pulumi.get(self, "canal_node")
 
     @property
     @pulumi.getter(name="certDownloader")
     def cert_downloader(self) -> Optional[str]:
-        """
-        Docker image for cert_downloader (string)
-        """
         return pulumi.get(self, "cert_downloader")
 
     @property
     @pulumi.getter
     def coredns(self) -> Optional[str]:
-        """
-        Docker image for coredns (string)
-        """
         return pulumi.get(self, "coredns")
 
     @property
     @pulumi.getter(name="corednsAutoscaler")
     def coredns_autoscaler(self) -> Optional[str]:
-        """
-        Docker image for coredns_autoscaler (string)
-        """
         return pulumi.get(self, "coredns_autoscaler")
 
     @property
     @pulumi.getter
     def dnsmasq(self) -> Optional[str]:
-        """
-        Docker image for dnsmasq (string)
-        """
         return pulumi.get(self, "dnsmasq")
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional[str]:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @property
     @pulumi.getter
     def flannel(self) -> Optional[str]:
-        """
-        Docker image for flannel (string)
-        """
         return pulumi.get(self, "flannel")
 
     @property
     @pulumi.getter(name="flannelCni")
     def flannel_cni(self) -> Optional[str]:
-        """
-        Docker image for flannel_cni (string)
-        """
         return pulumi.get(self, "flannel_cni")
 
     @property
     @pulumi.getter
     def ingress(self) -> Optional[str]:
         """
         RKE k8s cluster ingress controller configuration (list maxitems:1)
         """
         return pulumi.get(self, "ingress")
 
     @property
     @pulumi.getter(name="ingressBackend")
     def ingress_backend(self) -> Optional[str]:
-        """
-        Docker image for ingress_backend (string)
-        """
         return pulumi.get(self, "ingress_backend")
 
     @property
     @pulumi.getter(name="kubeDns")
     def kube_dns(self) -> Optional[str]:
-        """
-        Docker image for kube_dns (string)
-        """
         return pulumi.get(self, "kube_dns")
 
     @property
     @pulumi.getter(name="kubeDnsAutoscaler")
     def kube_dns_autoscaler(self) -> Optional[str]:
-        """
-        Docker image for kube_dns_autoscaler (string)
-        """
         return pulumi.get(self, "kube_dns_autoscaler")
 
     @property
     @pulumi.getter(name="kubeDnsSidecar")
     def kube_dns_sidecar(self) -> Optional[str]:
-        """
-        Docker image for kube_dns_sidecar (string)
-        """
         return pulumi.get(self, "kube_dns_sidecar")
 
     @property
     @pulumi.getter
     def kubernetes(self) -> Optional[str]:
-        """
-        Docker image for kubernetes (string)
-        """
         return pulumi.get(self, "kubernetes")
 
     @property
     @pulumi.getter(name="kubernetesServicesSidecar")
     def kubernetes_services_sidecar(self) -> Optional[str]:
-        """
-        Docker image for kubernetes_services_sidecar (string)
-        """
         return pulumi.get(self, "kubernetes_services_sidecar")
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[str]:
-        """
-        Docker image for metrics_server (string)
-        """
         return pulumi.get(self, "metrics_server")
 
     @property
     @pulumi.getter(name="nginxProxy")
     def nginx_proxy(self) -> Optional[str]:
-        """
-        Docker image for nginx_proxy (string)
-        """
         return pulumi.get(self, "nginx_proxy")
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional[str]:
-        """
-        Docker image for nodelocal (string)
-        """
         return pulumi.get(self, "nodelocal")
 
     @property
     @pulumi.getter(name="podInfraContainer")
     def pod_infra_container(self) -> Optional[str]:
-        """
-        Docker image for pod_infra_container (string)
-        """
         return pulumi.get(self, "pod_infra_container")
 
     @property
     @pulumi.getter(name="weaveCni")
     def weave_cni(self) -> Optional[str]:
-        """
-        Docker image for weave_cni (string)
-        """
         return pulumi.get(self, "weave_cni")
 
     @property
     @pulumi.getter(name="weaveNode")
     def weave_node(self) -> Optional[str]:
-        """
-        Docker image for weave_node (string)
-        """
         return pulumi.get(self, "weave_node")
 
     @property
     @pulumi.getter(name="windowsPodInfraContainer")
     def windows_pod_infra_container(self) -> Optional[str]:
-        """
-        Docker image for windows_pod_infra_container (string)
-        """
         return pulumi.get(self, "windows_pod_infra_container")
 
 
 @pulumi.output_type
 class ClusterServices(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6370,22 +5404,14 @@
     def __init__(__self__, *,
                  etcd: Optional['outputs.ClusterServicesEtcd'] = None,
                  kube_api: Optional['outputs.ClusterServicesKubeApi'] = None,
                  kube_controller: Optional['outputs.ClusterServicesKubeController'] = None,
                  kubelet: Optional['outputs.ClusterServicesKubelet'] = None,
                  kubeproxy: Optional['outputs.ClusterServicesKubeproxy'] = None,
                  scheduler: Optional['outputs.ClusterServicesScheduler'] = None):
-        """
-        :param 'ClusterServicesEtcdArgs' etcd: Docker image for etcd (string)
-        :param 'ClusterServicesKubeApiArgs' kube_api: Kube API options for RKE services (list maxitems:1)
-        :param 'ClusterServicesKubeControllerArgs' kube_controller: Kube Controller options for RKE services (list maxitems:1)
-        :param 'ClusterServicesKubeletArgs' kubelet: Kubelet options for RKE services (list maxitems:1)
-        :param 'ClusterServicesKubeproxyArgs' kubeproxy: Kubeproxy options for RKE services (list maxitems:1)
-        :param 'ClusterServicesSchedulerArgs' scheduler: Scheduler options for RKE services (list maxitems:1)
-        """
         if etcd is not None:
             pulumi.set(__self__, "etcd", etcd)
         if kube_api is not None:
             pulumi.set(__self__, "kube_api", kube_api)
         if kube_controller is not None:
             pulumi.set(__self__, "kube_controller", kube_controller)
         if kubelet is not None:
@@ -6394,57 +5420,39 @@
             pulumi.set(__self__, "kubeproxy", kubeproxy)
         if scheduler is not None:
             pulumi.set(__self__, "scheduler", scheduler)
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional['outputs.ClusterServicesEtcd']:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @property
     @pulumi.getter(name="kubeApi")
     def kube_api(self) -> Optional['outputs.ClusterServicesKubeApi']:
-        """
-        Kube API options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kube_api")
 
     @property
     @pulumi.getter(name="kubeController")
     def kube_controller(self) -> Optional['outputs.ClusterServicesKubeController']:
-        """
-        Kube Controller options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kube_controller")
 
     @property
     @pulumi.getter
     def kubelet(self) -> Optional['outputs.ClusterServicesKubelet']:
-        """
-        Kubelet options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kubelet")
 
     @property
     @pulumi.getter
     def kubeproxy(self) -> Optional['outputs.ClusterServicesKubeproxy']:
-        """
-        Kubeproxy options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "kubeproxy")
 
     @property
     @pulumi.getter
     def scheduler(self) -> Optional['outputs.ClusterServicesScheduler']:
-        """
-        Scheduler options for RKE services (list maxitems:1)
-        """
         return pulumi.get(self, "scheduler")
 
 
 @pulumi.output_type
 class ClusterServicesEtcd(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6485,31 +5493,14 @@
                  gid: Optional[int] = None,
                  image: Optional[str] = None,
                  key: Optional[str] = None,
                  path: Optional[str] = None,
                  retention: Optional[str] = None,
                  snapshot: Optional[bool] = None,
                  uid: Optional[int] = None):
-        """
-        :param 'ClusterServicesEtcdBackupConfigArgs' backup_config: Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        :param str ca_cert: TLS CA certificate for etcd service (string)
-        :param str cert: TLS certificate for etcd service (string)
-        :param str creation: Creation option for etcd service (string)
-        :param Sequence[str] external_urls: External urls for etcd service (list)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param int gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        :param str image: Docker image for scheduler service (string)
-        :param str key: TLS key for etcd service (string)
-        :param str path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param str retention: Retention for etcd backup. Default `6` (int)
-        :param bool snapshot: Snapshot option for etcd service. Default `true` (bool)
-        :param int uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if creation is not None:
@@ -6536,129 +5527,84 @@
             pulumi.set(__self__, "snapshot", snapshot)
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional['outputs.ClusterServicesEtcdBackupConfig']:
-        """
-        Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        """
         return pulumi.get(self, "backup_config")
 
     @property
     @pulumi.getter(name="caCert")
     def ca_cert(self) -> Optional[str]:
-        """
-        TLS CA certificate for etcd service (string)
-        """
         return pulumi.get(self, "ca_cert")
 
     @property
     @pulumi.getter
     def cert(self) -> Optional[str]:
-        """
-        TLS certificate for etcd service (string)
-        """
         return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter
     def creation(self) -> Optional[str]:
-        """
-        Creation option for etcd service (string)
-        """
         return pulumi.get(self, "creation")
 
     @property
     @pulumi.getter(name="externalUrls")
     def external_urls(self) -> Optional[Sequence[str]]:
-        """
-        External urls for etcd service (list)
-        """
         return pulumi.get(self, "external_urls")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
-        """
-        Extra arguments for scheduler service (map)
-        """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
-        """
-        Extra binds for scheduler service (list)
-        """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
-        """
-        Extra environment for scheduler service (list)
-        """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[int]:
-        """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "gid")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[str]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @property
     @pulumi.getter
     def snapshot(self) -> Optional[bool]:
-        """
-        Snapshot option for etcd service. Default `true` (bool)
-        """
         return pulumi.get(self, "snapshot")
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[int]:
-        """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "uid")
 
 
 @pulumi.output_type
 class ClusterServicesEtcdBackupConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6684,22 +5630,14 @@
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  interval_hours: Optional[int] = None,
                  retention: Optional[int] = None,
                  s3_backup_config: Optional['outputs.ClusterServicesEtcdBackupConfigS3BackupConfig'] = None,
                  safe_timestamp: Optional[bool] = None,
                  timeout: Optional[int] = None):
-        """
-        :param bool enabled: Enable secrets encryption (bool)
-        :param int interval_hours: Interval hours for etcd backup. Default `12` (int)
-        :param int retention: Retention for etcd backup. Default `6` (int)
-        :param 'ClusterServicesEtcdBackupConfigS3BackupConfigArgs' s3_backup_config: S3 config options for etcd backup (list maxitems:1)
-        :param bool safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param int timeout: RKE node drain timeout (int)
-        """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
         if s3_backup_config is not None:
@@ -6708,57 +5646,39 @@
             pulumi.set(__self__, "safe_timestamp", safe_timestamp)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="intervalHours")
     def interval_hours(self) -> Optional[int]:
-        """
-        Interval hours for etcd backup. Default `12` (int)
-        """
         return pulumi.get(self, "interval_hours")
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[int]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @property
     @pulumi.getter(name="s3BackupConfig")
     def s3_backup_config(self) -> Optional['outputs.ClusterServicesEtcdBackupConfigS3BackupConfig']:
-        """
-        S3 config options for etcd backup (list maxitems:1)
-        """
         return pulumi.get(self, "s3_backup_config")
 
     @property
     @pulumi.getter(name="safeTimestamp")
     def safe_timestamp(self) -> Optional[bool]:
-        """
-        Safe timestamp for etcd backup. Default: `false` (bool)
-        """
         return pulumi.get(self, "safe_timestamp")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class ClusterServicesEtcdBackupConfigS3BackupConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6787,23 +5707,14 @@
                  access_key: Optional[str] = None,
                  bucket_name: Optional[str] = None,
                  custom_ca: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  folder: Optional[str] = None,
                  region: Optional[str] = None,
                  secret_key: Optional[str] = None):
-        """
-        :param str access_key: Access key for S3 service (string)
-        :param str bucket_name: Bucket name for S3 service (string)
-        :param str custom_ca: Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        :param str endpoint: Endpoint for S3 service (string)
-        :param str folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param str region: Region for S3 service (string)
-        :param str secret_key: Secret key for S3 service (string)
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if custom_ca is not None:
             pulumi.set(__self__, "custom_ca", custom_ca)
         if endpoint is not None:
@@ -6814,65 +5725,44 @@
             pulumi.set(__self__, "region", region)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
-        """
-        Access key for S3 service (string)
-        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bucketName")
     def bucket_name(self) -> Optional[str]:
-        """
-        Bucket name for S3 service (string)
-        """
         return pulumi.get(self, "bucket_name")
 
     @property
     @pulumi.getter(name="customCa")
     def custom_ca(self) -> Optional[str]:
-        """
-        Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        """
         return pulumi.get(self, "custom_ca")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
-        """
-        Endpoint for S3 service (string)
-        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
-        """
-        Secret key for S3 service (string)
-        """
         return pulumi.get(self, "secret_key")
 
 
 @pulumi.output_type
 class ClusterServicesEtcdDeprecated(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -6913,31 +5803,14 @@
                  gid: Optional[int] = None,
                  image: Optional[str] = None,
                  key: Optional[str] = None,
                  path: Optional[str] = None,
                  retention: Optional[str] = None,
                  snapshot: Optional[bool] = None,
                  uid: Optional[int] = None):
-        """
-        :param 'ClusterServicesEtcdDeprecatedBackupConfigArgs' backup_config: Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        :param str ca_cert: TLS CA certificate for etcd service (string)
-        :param str cert: TLS certificate for etcd service (string)
-        :param str creation: Creation option for etcd service (string)
-        :param Sequence[str] external_urls: External urls for etcd service (list)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param int gid: Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        :param str image: Docker image for scheduler service (string)
-        :param str key: TLS key for etcd service (string)
-        :param str path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param str retention: Retention for etcd backup. Default `6` (int)
-        :param bool snapshot: Snapshot option for etcd service. Default `true` (bool)
-        :param int uid: Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         if backup_config is not None:
             pulumi.set(__self__, "backup_config", backup_config)
         if ca_cert is not None:
             pulumi.set(__self__, "ca_cert", ca_cert)
         if cert is not None:
             pulumi.set(__self__, "cert", cert)
         if creation is not None:
@@ -6964,129 +5837,84 @@
             pulumi.set(__self__, "snapshot", snapshot)
         if uid is not None:
             pulumi.set(__self__, "uid", uid)
 
     @property
     @pulumi.getter(name="backupConfig")
     def backup_config(self) -> Optional['outputs.ClusterServicesEtcdDeprecatedBackupConfig']:
-        """
-        Backup options for etcd service. For Rancher v2.2.x and above (list maxitems:1)
-        """
         return pulumi.get(self, "backup_config")
 
     @property
     @pulumi.getter(name="caCert")
     def ca_cert(self) -> Optional[str]:
-        """
-        TLS CA certificate for etcd service (string)
-        """
         return pulumi.get(self, "ca_cert")
 
     @property
     @pulumi.getter
     def cert(self) -> Optional[str]:
-        """
-        TLS certificate for etcd service (string)
-        """
         return pulumi.get(self, "cert")
 
     @property
     @pulumi.getter
     def creation(self) -> Optional[str]:
-        """
-        Creation option for etcd service (string)
-        """
         return pulumi.get(self, "creation")
 
     @property
     @pulumi.getter(name="externalUrls")
     def external_urls(self) -> Optional[Sequence[str]]:
-        """
-        External urls for etcd service (list)
-        """
         return pulumi.get(self, "external_urls")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
-        """
-        Extra arguments for scheduler service (map)
-        """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
-        """
-        Extra binds for scheduler service (list)
-        """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
-        """
-        Extra environment for scheduler service (list)
-        """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def gid(self) -> Optional[int]:
-        """
-        Etcd service GID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "gid")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter
     def key(self) -> Optional[str]:
-        """
-        TLS key for etcd service (string)
-        """
         return pulumi.get(self, "key")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[str]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @property
     @pulumi.getter
     def snapshot(self) -> Optional[bool]:
-        """
-        Snapshot option for etcd service. Default `true` (bool)
-        """
         return pulumi.get(self, "snapshot")
 
     @property
     @pulumi.getter
     def uid(self) -> Optional[int]:
-        """
-        Etcd service UID. Default: `0`. For Rancher v2.3.x and above (int)
-        """
         return pulumi.get(self, "uid")
 
 
 @pulumi.output_type
 class ClusterServicesEtcdDeprecatedBackupConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7112,22 +5940,14 @@
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  interval_hours: Optional[int] = None,
                  retention: Optional[int] = None,
                  s3_backup_config: Optional['outputs.ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfig'] = None,
                  safe_timestamp: Optional[bool] = None,
                  timeout: Optional[int] = None):
-        """
-        :param bool enabled: Enable secrets encryption (bool)
-        :param int interval_hours: Interval hours for etcd backup. Default `12` (int)
-        :param int retention: Retention for etcd backup. Default `6` (int)
-        :param 'ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfigArgs' s3_backup_config: S3 config options for etcd backup (list maxitems:1)
-        :param bool safe_timestamp: Safe timestamp for etcd backup. Default: `false` (bool)
-        :param int timeout: RKE node drain timeout (int)
-        """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if interval_hours is not None:
             pulumi.set(__self__, "interval_hours", interval_hours)
         if retention is not None:
             pulumi.set(__self__, "retention", retention)
         if s3_backup_config is not None:
@@ -7136,57 +5956,39 @@
             pulumi.set(__self__, "safe_timestamp", safe_timestamp)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter(name="intervalHours")
     def interval_hours(self) -> Optional[int]:
-        """
-        Interval hours for etcd backup. Default `12` (int)
-        """
         return pulumi.get(self, "interval_hours")
 
     @property
     @pulumi.getter
     def retention(self) -> Optional[int]:
-        """
-        Retention for etcd backup. Default `6` (int)
-        """
         return pulumi.get(self, "retention")
 
     @property
     @pulumi.getter(name="s3BackupConfig")
     def s3_backup_config(self) -> Optional['outputs.ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfig']:
-        """
-        S3 config options for etcd backup (list maxitems:1)
-        """
         return pulumi.get(self, "s3_backup_config")
 
     @property
     @pulumi.getter(name="safeTimestamp")
     def safe_timestamp(self) -> Optional[bool]:
-        """
-        Safe timestamp for etcd backup. Default: `false` (bool)
-        """
         return pulumi.get(self, "safe_timestamp")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class ClusterServicesEtcdDeprecatedBackupConfigS3BackupConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7215,23 +6017,14 @@
                  access_key: Optional[str] = None,
                  bucket_name: Optional[str] = None,
                  custom_ca: Optional[str] = None,
                  endpoint: Optional[str] = None,
                  folder: Optional[str] = None,
                  region: Optional[str] = None,
                  secret_key: Optional[str] = None):
-        """
-        :param str access_key: Access key for S3 service (string)
-        :param str bucket_name: Bucket name for S3 service (string)
-        :param str custom_ca: Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        :param str endpoint: Endpoint for S3 service (string)
-        :param str folder: Folder for S3 service. Available from Rancher v2.2.7 (string)
-        :param str region: Region for S3 service (string)
-        :param str secret_key: Secret key for S3 service (string)
-        """
         if access_key is not None:
             pulumi.set(__self__, "access_key", access_key)
         if bucket_name is not None:
             pulumi.set(__self__, "bucket_name", bucket_name)
         if custom_ca is not None:
             pulumi.set(__self__, "custom_ca", custom_ca)
         if endpoint is not None:
@@ -7242,65 +6035,44 @@
             pulumi.set(__self__, "region", region)
         if secret_key is not None:
             pulumi.set(__self__, "secret_key", secret_key)
 
     @property
     @pulumi.getter(name="accessKey")
     def access_key(self) -> Optional[str]:
-        """
-        Access key for S3 service (string)
-        """
         return pulumi.get(self, "access_key")
 
     @property
     @pulumi.getter(name="bucketName")
     def bucket_name(self) -> Optional[str]:
-        """
-        Bucket name for S3 service (string)
-        """
         return pulumi.get(self, "bucket_name")
 
     @property
     @pulumi.getter(name="customCa")
     def custom_ca(self) -> Optional[str]:
-        """
-        Base64 encoded custom CA for S3 service. Use filebase64(<FILE>) for encoding file. Available from Rancher v2.2.5 (string)
-        """
         return pulumi.get(self, "custom_ca")
 
     @property
     @pulumi.getter
     def endpoint(self) -> Optional[str]:
-        """
-        Endpoint for S3 service (string)
-        """
         return pulumi.get(self, "endpoint")
 
     @property
     @pulumi.getter
     def folder(self) -> Optional[str]:
-        """
-        Folder for S3 service. Available from Rancher v2.2.7 (string)
-        """
         return pulumi.get(self, "folder")
 
     @property
     @pulumi.getter
     def region(self) -> Optional[str]:
-        """
-        Region for S3 service (string)
-        """
         return pulumi.get(self, "region")
 
     @property
     @pulumi.getter(name="secretKey")
     def secret_key(self) -> Optional[str]:
-        """
-        Secret key for S3 service (string)
-        """
         return pulumi.get(self, "secret_key")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApi(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7349,26 +6121,22 @@
                  image: Optional[str] = None,
                  pod_security_configuration: Optional[str] = None,
                  pod_security_policy: Optional[bool] = None,
                  secrets_encryption_config: Optional['outputs.ClusterServicesKubeApiSecretsEncryptionConfig'] = None,
                  service_cluster_ip_range: Optional[str] = None,
                  service_node_port_range: Optional[str] = None):
         """
-        :param bool always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
-        :param 'ClusterServicesKubeApiAuditLogArgs' audit_log: K8s audit log configuration. (list maxitem: 1)
-        :param 'ClusterServicesKubeApiEventRateLimitArgs' event_rate_limit: K8s event rate limit configuration. (list maxitem: 1)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param bool always_pull_images: Enable/Disable AlwaysPullImages admissions plugin
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kube-api services
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
         :param str pod_security_configuration: Built-in PodSecurityPolicy (privileged or restricted)
-        :param bool pod_security_policy: Pod Security Policy option for kube API service (bool)
-        :param 'ClusterServicesKubeApiSecretsEncryptionConfigArgs' secrets_encryption_config: [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        :param str service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
-        :param str service_node_port_range: Service Node Port Range option for kube API service (string)
+        :param bool pod_security_policy: Enabled/Disable PodSecurityPolicy
+        :param str service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
+        :param str service_node_port_range: Port range for services defined with NodePort type
         """
         if always_pull_images is not None:
             pulumi.set(__self__, "always_pull_images", always_pull_images)
         if audit_log is not None:
             pulumi.set(__self__, "audit_log", audit_log)
         if event_rate_limit is not None:
             pulumi.set(__self__, "event_rate_limit", event_rate_limit)
@@ -7391,135 +6159,113 @@
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[bool]:
         """
-        Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
+        Enable/Disable AlwaysPullImages admissions plugin
         """
         return pulumi.get(self, "always_pull_images")
 
     @property
     @pulumi.getter(name="auditLog")
     def audit_log(self) -> Optional['outputs.ClusterServicesKubeApiAuditLog']:
-        """
-        K8s audit log configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "audit_log")
 
     @property
     @pulumi.getter(name="eventRateLimit")
     def event_rate_limit(self) -> Optional['outputs.ClusterServicesKubeApiEventRateLimit']:
-        """
-        K8s event rate limit configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "event_rate_limit")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-api services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="podSecurityConfiguration")
     def pod_security_configuration(self) -> Optional[str]:
         """
         Built-in PodSecurityPolicy (privileged or restricted)
         """
         return pulumi.get(self, "pod_security_configuration")
 
     @property
     @pulumi.getter(name="podSecurityPolicy")
     def pod_security_policy(self) -> Optional[bool]:
         """
-        Pod Security Policy option for kube API service (bool)
+        Enabled/Disable PodSecurityPolicy
         """
         return pulumi.get(self, "pod_security_policy")
 
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional['outputs.ClusterServicesKubeApiSecretsEncryptionConfig']:
-        """
-        [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        """
         return pulumi.get(self, "secrets_encryption_config")
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[str]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> Optional[str]:
         """
-        Service Node Port Range option for kube API service (string)
+        Port range for services defined with NodePort type
         """
         return pulumi.get(self, "service_node_port_range")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterServicesKubeApiAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param 'ClusterServicesKubeApiAuditLogConfigurationArgs' configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional['outputs.ClusterServicesKubeApiAuditLogConfiguration']:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiAuditLogConfiguration(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7545,22 +6291,14 @@
     def __init__(__self__, *,
                  format: Optional[str] = None,
                  max_age: Optional[int] = None,
                  max_backup: Optional[int] = None,
                  max_size: Optional[int] = None,
                  path: Optional[str] = None,
                  policy: Optional[str] = None):
-        """
-        :param str format: Audit log format (string)
-        :param int max_age: Audit log max age (int)
-        :param int max_backup: Audit log max backup. Default: `10` (int)
-        :param int max_size: Audit log max size. Default: `100` (int)
-        :param str path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param str policy: Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
         if max_size is not None:
@@ -7569,57 +6307,39 @@
             pulumi.set(__self__, "path", path)
         if policy is not None:
             pulumi.set(__self__, "policy", policy)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
-        """
-        Audit log format (string)
-        """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter(name="maxAge")
     def max_age(self) -> Optional[int]:
-        """
-        Audit log max age (int)
-        """
         return pulumi.get(self, "max_age")
 
     @property
     @pulumi.getter(name="maxBackup")
     def max_backup(self) -> Optional[int]:
-        """
-        Audit log max backup. Default: `10` (int)
-        """
         return pulumi.get(self, "max_backup")
 
     @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[int]:
-        """
-        Audit log max size. Default: `100` (int)
-        """
         return pulumi.get(self, "max_size")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[str]:
-        """
-        Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         return pulumi.get(self, "policy")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiDeprecated(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7668,26 +6388,22 @@
                  image: Optional[str] = None,
                  pod_security_configuration: Optional[str] = None,
                  pod_security_policy: Optional[bool] = None,
                  secrets_encryption_config: Optional['outputs.ClusterServicesKubeApiDeprecatedSecretsEncryptionConfig'] = None,
                  service_cluster_ip_range: Optional[str] = None,
                  service_node_port_range: Optional[str] = None):
         """
-        :param bool always_pull_images: Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
-        :param 'ClusterServicesKubeApiDeprecatedAuditLogArgs' audit_log: K8s audit log configuration. (list maxitem: 1)
-        :param 'ClusterServicesKubeApiDeprecatedEventRateLimitArgs' event_rate_limit: K8s event rate limit configuration. (list maxitem: 1)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param bool always_pull_images: Enable/Disable AlwaysPullImages admissions plugin
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kube-api services
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
         :param str pod_security_configuration: Built-in PodSecurityPolicy (privileged or restricted)
-        :param bool pod_security_policy: Pod Security Policy option for kube API service (bool)
-        :param 'ClusterServicesKubeApiDeprecatedSecretsEncryptionConfigArgs' secrets_encryption_config: [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        :param str service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
-        :param str service_node_port_range: Service Node Port Range option for kube API service (string)
+        :param bool pod_security_policy: Enabled/Disable PodSecurityPolicy
+        :param str service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
+        :param str service_node_port_range: Port range for services defined with NodePort type
         """
         if always_pull_images is not None:
             pulumi.set(__self__, "always_pull_images", always_pull_images)
         if audit_log is not None:
             pulumi.set(__self__, "audit_log", audit_log)
         if event_rate_limit is not None:
             pulumi.set(__self__, "event_rate_limit", event_rate_limit)
@@ -7710,135 +6426,113 @@
         if service_node_port_range is not None:
             pulumi.set(__self__, "service_node_port_range", service_node_port_range)
 
     @property
     @pulumi.getter(name="alwaysPullImages")
     def always_pull_images(self) -> Optional[bool]:
         """
-        Enable [AlwaysPullImages](https://kubernetes.io/docs/reference/access-authn-authz/admission-controllers/#alwayspullimages) Admission controller plugin. [Rancher docs](https://rancher.com/docs/rke/latest/en/config-options/services/#kubernetes-api-server-options) (bool)
+        Enable/Disable AlwaysPullImages admissions plugin
         """
         return pulumi.get(self, "always_pull_images")
 
     @property
     @pulumi.getter(name="auditLog")
     def audit_log(self) -> Optional['outputs.ClusterServicesKubeApiDeprecatedAuditLog']:
-        """
-        K8s audit log configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "audit_log")
 
     @property
     @pulumi.getter(name="eventRateLimit")
     def event_rate_limit(self) -> Optional['outputs.ClusterServicesKubeApiDeprecatedEventRateLimit']:
-        """
-        K8s event rate limit configuration. (list maxitem: 1)
-        """
         return pulumi.get(self, "event_rate_limit")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-api services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
-        """
-        Docker image for scheduler service (string)
-        """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="podSecurityConfiguration")
     def pod_security_configuration(self) -> Optional[str]:
         """
         Built-in PodSecurityPolicy (privileged or restricted)
         """
         return pulumi.get(self, "pod_security_configuration")
 
     @property
     @pulumi.getter(name="podSecurityPolicy")
     def pod_security_policy(self) -> Optional[bool]:
         """
-        Pod Security Policy option for kube API service (bool)
+        Enabled/Disable PodSecurityPolicy
         """
         return pulumi.get(self, "pod_security_policy")
 
     @property
     @pulumi.getter(name="secretsEncryptionConfig")
     def secrets_encryption_config(self) -> Optional['outputs.ClusterServicesKubeApiDeprecatedSecretsEncryptionConfig']:
-        """
-        [Encrypt k8s secret data configration](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/). (list maxitem: 1)
-        """
         return pulumi.get(self, "secrets_encryption_config")
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[str]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
     @property
     @pulumi.getter(name="serviceNodePortRange")
     def service_node_port_range(self) -> Optional[str]:
         """
-        Service Node Port Range option for kube API service (string)
+        Port range for services defined with NodePort type
         """
         return pulumi.get(self, "service_node_port_range")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiDeprecatedAuditLog(dict):
     def __init__(__self__, *,
                  configuration: Optional['outputs.ClusterServicesKubeApiDeprecatedAuditLogConfiguration'] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param 'ClusterServicesKubeApiDeprecatedAuditLogConfigurationArgs' configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional['outputs.ClusterServicesKubeApiDeprecatedAuditLogConfiguration']:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiDeprecatedAuditLogConfiguration(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7864,22 +6558,14 @@
     def __init__(__self__, *,
                  format: Optional[str] = None,
                  max_age: Optional[int] = None,
                  max_backup: Optional[int] = None,
                  max_size: Optional[int] = None,
                  path: Optional[str] = None,
                  policy: Optional[str] = None):
-        """
-        :param str format: Audit log format (string)
-        :param int max_age: Audit log max age (int)
-        :param int max_backup: Audit log max backup. Default: `10` (int)
-        :param int max_size: Audit log max size. Default: `100` (int)
-        :param str path: Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        :param str policy: Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         if format is not None:
             pulumi.set(__self__, "format", format)
         if max_age is not None:
             pulumi.set(__self__, "max_age", max_age)
         if max_backup is not None:
             pulumi.set(__self__, "max_backup", max_backup)
         if max_size is not None:
@@ -7888,88 +6574,60 @@
             pulumi.set(__self__, "path", path)
         if policy is not None:
             pulumi.set(__self__, "policy", policy)
 
     @property
     @pulumi.getter
     def format(self) -> Optional[str]:
-        """
-        Audit log format (string)
-        """
         return pulumi.get(self, "format")
 
     @property
     @pulumi.getter(name="maxAge")
     def max_age(self) -> Optional[int]:
-        """
-        Audit log max age (int)
-        """
         return pulumi.get(self, "max_age")
 
     @property
     @pulumi.getter(name="maxBackup")
     def max_backup(self) -> Optional[int]:
-        """
-        Audit log max backup. Default: `10` (int)
-        """
         return pulumi.get(self, "max_backup")
 
     @property
     @pulumi.getter(name="maxSize")
     def max_size(self) -> Optional[int]:
-        """
-        Audit log max size. Default: `100` (int)
-        """
         return pulumi.get(self, "max_size")
 
     @property
     @pulumi.getter
     def path(self) -> Optional[str]:
-        """
-        Audit log path. Default: `/var/log/kube-audit/audit-log.json` (string)
-        """
         return pulumi.get(self, "path")
 
     @property
     @pulumi.getter
     def policy(self) -> Optional[str]:
-        """
-        Audit policy json encoded definition. `"apiVersion"` and `"kind":"Policy","rules"` fields are required in the json. Ex. `jsonencode({"apiVersion":"audit.k8s.io/v1","kind":"Policy","rules":[{"level":"RequestResponse","resources":[{"group":"","resources":["pods"]}]}]})` [More info](https://rancher.com/docs/rke/latest/en/config-options/audit-log/) (string)
-        """
         return pulumi.get(self, "policy")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiDeprecatedEventRateLimit(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param str configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiDeprecatedSecretsEncryptionConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -7987,68 +6645,48 @@
     def get(self, key: str, default = None) -> Any:
         ClusterServicesKubeApiDeprecatedSecretsEncryptionConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  custom_config: Optional[str] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param str custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[str]:
-        """
-        Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        """
         return pulumi.get(self, "custom_config")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiEventRateLimit(dict):
     def __init__(__self__, *,
                  configuration: Optional[str] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param str configuration: Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if configuration is not None:
             pulumi.set(__self__, "configuration", configuration)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def configuration(self) -> Optional[str]:
-        """
-        Event rate limit yaml encoded configuration. `"apiVersion"` and `"kind":"Configuration"` fields are required in the yaml. Ex. `apiVersion: eventratelimit.admission.k8s.io/v1alpha1\\nkind: Configuration\\nlimits:\\n- type: Server\\n  burst: 30000\\n  qps: 6000\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/rate-limiting/) (string)
-        """
         return pulumi.get(self, "configuration")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeApiSecretsEncryptionConfig(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8066,37 +6704,27 @@
     def get(self, key: str, default = None) -> Any:
         ClusterServicesKubeApiSecretsEncryptionConfig.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  custom_config: Optional[str] = None,
                  enabled: Optional[bool] = None):
-        """
-        :param str custom_config: Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        :param bool enabled: Enable secrets encryption (bool)
-        """
         if custom_config is not None:
             pulumi.set(__self__, "custom_config", custom_config)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter(name="customConfig")
     def custom_config(self) -> Optional[str]:
-        """
-        Secrets encryption yaml encoded custom configuration. `"apiVersion"` and `"kind":"EncryptionConfiguration"` fields are required in the yaml. Ex. `apiVersion: apiserver.config.k8s.io/v1\\nkind: EncryptionConfiguration\\nresources:\\n- resources:\\n  - secrets\\n  providers:\\n  - aescbc:\\n      keys:\\n      - name: k-fw5hn\\n        secret: RTczRjFDODMwQzAyMDVBREU4NDJBMUZFNDhCNzM5N0I=\\n    identity: {}\\n` [More info](https://rancher.com/docs/rke/latest/en/config-options/secrets-encryption/) (string)
-        """
         return pulumi.get(self, "custom_config")
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        Enable secrets encryption (bool)
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class ClusterServicesKubeController(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -8127,20 +6755,20 @@
                  cluster_cidr: Optional[str] = None,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None,
                  service_cluster_ip_range: Optional[str] = None):
         """
-        :param str cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
-        :param str service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
+        :param str cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kube-controller service
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
+        :param str image: Docker image of the kube-controller service
+        :param str service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
         """
         if cluster_cidr is not None:
             pulumi.set(__self__, "cluster_cidr", cluster_cidr)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
@@ -8151,55 +6779,55 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> Optional[str]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-controller service
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kube-controller service
         """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[str]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
 
 @pulumi.output_type
 class ClusterServicesKubeControllerDeprecated(dict):
     @staticmethod
@@ -8231,20 +6859,20 @@
                  cluster_cidr: Optional[str] = None,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None,
                  service_cluster_ip_range: Optional[str] = None):
         """
-        :param str cluster_cidr: Cluster CIDR option for kube controller service (string)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
-        :param str service_cluster_ip_range: Service Cluster ip Range option for kube controller service (string)
+        :param str cluster_cidr: (Computed) RKE k8s cluster cidr (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kube-controller service
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
+        :param str image: Docker image of the kube-controller service
+        :param str service_cluster_ip_range: Virtual IP range that will be used by Kubernetes services
         """
         if cluster_cidr is not None:
             pulumi.set(__self__, "cluster_cidr", cluster_cidr)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
@@ -8255,55 +6883,55 @@
         if service_cluster_ip_range is not None:
             pulumi.set(__self__, "service_cluster_ip_range", service_cluster_ip_range)
 
     @property
     @pulumi.getter(name="clusterCidr")
     def cluster_cidr(self) -> Optional[str]:
         """
-        Cluster CIDR option for kube controller service (string)
+        (Computed) RKE k8s cluster cidr (string)
         """
         return pulumi.get(self, "cluster_cidr")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kube-controller service
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kube-controller service
         """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="serviceClusterIpRange")
     def service_cluster_ip_range(self) -> Optional[str]:
         """
-        Service Cluster ip Range option for kube controller service (string)
+        Virtual IP range that will be used by Kubernetes services
         """
         return pulumi.get(self, "service_cluster_ip_range")
 
 
 @pulumi.output_type
 class ClusterServicesKubeProxyDeprecated(dict):
     @staticmethod
@@ -8329,57 +6957,57 @@
 
     def __init__(__self__, *,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None):
         """
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kubeproxy services
+        :param Sequence[str] extra_binds: Extra binds added to the worker nodes
+        :param Sequence[str] extra_envs: Extra env added to the worker nodes
+        :param str image: Docker image of the kubeproxy service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubeproxy services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the worker nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubeproxy service
         """
         return pulumi.get(self, "image")
 
 
 @pulumi.output_type
 class ClusterServicesKubeSchedulerDeprecated(dict):
     @staticmethod
@@ -8405,57 +7033,57 @@
 
     def __init__(__self__, *,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None):
         """
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the scheduler services
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
+        :param str image: Docker image of the scheduler service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the scheduler services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the scheduler service
         """
         return pulumi.get(self, "image")
 
 
 @pulumi.output_type
 class ClusterServicesKubelet(dict):
     @staticmethod
@@ -8496,23 +7124,22 @@
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  fail_swap_on: Optional[bool] = None,
                  generate_serving_certificate: Optional[bool] = None,
                  image: Optional[str] = None,
                  infra_container_image: Optional[str] = None):
         """
-        :param str cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param str cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param bool fail_swap_on: Enable or disable failing when swap on is not supported (bool)
-        :param bool generate_serving_certificate: [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        :param str image: Docker image for scheduler service (string)
-        :param str infra_container_image: Infra container image for kubelet service (string)
+        :param str cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param str cluster_domain: (Computed) RKE k8s cluster domain (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kubelet services
+        :param Sequence[str] extra_binds: Extra binds added to the worker nodes
+        :param Sequence[str] extra_envs: Extra env added to the nodes
+        :param bool fail_swap_on: Fail if swap is enabled
+        :param str image: Docker image of the kubelet service
+        :param str infra_container_image: The image whose network/ipc namespaces containers in each pod will use
         """
         if cluster_dns_server is not None:
             pulumi.set(__self__, "cluster_dns_server", cluster_dns_server)
         if cluster_domain is not None:
             pulumi.set(__self__, "cluster_domain", cluster_domain)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -8529,79 +7156,76 @@
         if infra_container_image is not None:
             pulumi.set(__self__, "infra_container_image", infra_container_image)
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> Optional[str]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> Optional[str]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubelet services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter(name="failSwapOn")
     def fail_swap_on(self) -> Optional[bool]:
         """
-        Enable or disable failing when swap on is not supported (bool)
+        Fail if swap is enabled
         """
         return pulumi.get(self, "fail_swap_on")
 
     @property
     @pulumi.getter(name="generateServingCertificate")
     def generate_serving_certificate(self) -> Optional[bool]:
-        """
-        [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        """
         return pulumi.get(self, "generate_serving_certificate")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubelet service
         """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="infraContainerImage")
     def infra_container_image(self) -> Optional[str]:
         """
-        Infra container image for kubelet service (string)
+        The image whose network/ipc namespaces containers in each pod will use
         """
         return pulumi.get(self, "infra_container_image")
 
 
 @pulumi.output_type
 class ClusterServicesKubeletDeprecated(dict):
     @staticmethod
@@ -8642,23 +7266,22 @@
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  fail_swap_on: Optional[bool] = None,
                  generate_serving_certificate: Optional[bool] = None,
                  image: Optional[str] = None,
                  infra_container_image: Optional[str] = None):
         """
-        :param str cluster_dns_server: Cluster DNS Server option for kubelet service (string)
-        :param str cluster_domain: Cluster Domain option for kubelet service. Default `cluster.local` (string)
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param bool fail_swap_on: Enable or disable failing when swap on is not supported (bool)
-        :param bool generate_serving_certificate: [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        :param str image: Docker image for scheduler service (string)
-        :param str infra_container_image: Infra container image for kubelet service (string)
+        :param str cluster_dns_server: (Computed) RKE k8s cluster dns server (string)
+        :param str cluster_domain: (Computed) RKE k8s cluster domain (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kubelet services
+        :param Sequence[str] extra_binds: Extra binds added to the worker nodes
+        :param Sequence[str] extra_envs: Extra env added to the nodes
+        :param bool fail_swap_on: Fail if swap is enabled
+        :param str image: Docker image of the kubelet service
+        :param str infra_container_image: The image whose network/ipc namespaces containers in each pod will use
         """
         if cluster_dns_server is not None:
             pulumi.set(__self__, "cluster_dns_server", cluster_dns_server)
         if cluster_domain is not None:
             pulumi.set(__self__, "cluster_domain", cluster_domain)
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
@@ -8675,79 +7298,76 @@
         if infra_container_image is not None:
             pulumi.set(__self__, "infra_container_image", infra_container_image)
 
     @property
     @pulumi.getter(name="clusterDnsServer")
     def cluster_dns_server(self) -> Optional[str]:
         """
-        Cluster DNS Server option for kubelet service (string)
+        (Computed) RKE k8s cluster dns server (string)
         """
         return pulumi.get(self, "cluster_dns_server")
 
     @property
     @pulumi.getter(name="clusterDomain")
     def cluster_domain(self) -> Optional[str]:
         """
-        Cluster Domain option for kubelet service. Default `cluster.local` (string)
+        (Computed) RKE k8s cluster domain (string)
         """
         return pulumi.get(self, "cluster_domain")
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubelet services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter(name="failSwapOn")
     def fail_swap_on(self) -> Optional[bool]:
         """
-        Enable or disable failing when swap on is not supported (bool)
+        Fail if swap is enabled
         """
         return pulumi.get(self, "fail_swap_on")
 
     @property
     @pulumi.getter(name="generateServingCertificate")
     def generate_serving_certificate(self) -> Optional[bool]:
-        """
-        [Generate a certificate signed by the kube-ca](https://rancher.com/docs/rke/latest/en/config-options/services/#kubelet-serving-certificate-requirements). Default `false` (bool)
-        """
         return pulumi.get(self, "generate_serving_certificate")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubelet service
         """
         return pulumi.get(self, "image")
 
     @property
     @pulumi.getter(name="infraContainerImage")
     def infra_container_image(self) -> Optional[str]:
         """
-        Infra container image for kubelet service (string)
+        The image whose network/ipc namespaces containers in each pod will use
         """
         return pulumi.get(self, "infra_container_image")
 
 
 @pulumi.output_type
 class ClusterServicesKubeproxy(dict):
     @staticmethod
@@ -8773,57 +7393,57 @@
 
     def __init__(__self__, *,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None):
         """
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the kubeproxy services
+        :param Sequence[str] extra_binds: Extra binds added to the worker nodes
+        :param Sequence[str] extra_envs: Extra env added to the worker nodes
+        :param str image: Docker image of the kubeproxy service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the kubeproxy services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the worker nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the worker nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the kubeproxy service
         """
         return pulumi.get(self, "image")
 
 
 @pulumi.output_type
 class ClusterServicesScheduler(dict):
     @staticmethod
@@ -8849,57 +7469,57 @@
 
     def __init__(__self__, *,
                  extra_args: Optional[Mapping[str, Any]] = None,
                  extra_binds: Optional[Sequence[str]] = None,
                  extra_envs: Optional[Sequence[str]] = None,
                  image: Optional[str] = None):
         """
-        :param Mapping[str, Any] extra_args: Extra arguments for scheduler service (map)
-        :param Sequence[str] extra_binds: Extra binds for scheduler service (list)
-        :param Sequence[str] extra_envs: Extra environment for scheduler service (list)
-        :param str image: Docker image for scheduler service (string)
+        :param Mapping[str, Any] extra_args: Extra arguments that are added to the scheduler services
+        :param Sequence[str] extra_binds: Extra binds added to the controlplane nodes
+        :param Sequence[str] extra_envs: Extra env added to the controlplane nodes
+        :param str image: Docker image of the scheduler service
         """
         if extra_args is not None:
             pulumi.set(__self__, "extra_args", extra_args)
         if extra_binds is not None:
             pulumi.set(__self__, "extra_binds", extra_binds)
         if extra_envs is not None:
             pulumi.set(__self__, "extra_envs", extra_envs)
         if image is not None:
             pulumi.set(__self__, "image", image)
 
     @property
     @pulumi.getter(name="extraArgs")
     def extra_args(self) -> Optional[Mapping[str, Any]]:
         """
-        Extra arguments for scheduler service (map)
+        Extra arguments that are added to the scheduler services
         """
         return pulumi.get(self, "extra_args")
 
     @property
     @pulumi.getter(name="extraBinds")
     def extra_binds(self) -> Optional[Sequence[str]]:
         """
-        Extra binds for scheduler service (list)
+        Extra binds added to the controlplane nodes
         """
         return pulumi.get(self, "extra_binds")
 
     @property
     @pulumi.getter(name="extraEnvs")
     def extra_envs(self) -> Optional[Sequence[str]]:
         """
-        Extra environment for scheduler service (list)
+        Extra env added to the controlplane nodes
         """
         return pulumi.get(self, "extra_envs")
 
     @property
     @pulumi.getter
     def image(self) -> Optional[str]:
         """
-        Docker image for scheduler service (string)
+        Docker image of the scheduler service
         """
         return pulumi.get(self, "image")
 
 
 @pulumi.output_type
 class ClusterSystemImages(dict):
     @staticmethod
@@ -9010,51 +7630,15 @@
                  nginx_proxy: Optional[str] = None,
                  nodelocal: Optional[str] = None,
                  pod_infra_container: Optional[str] = None,
                  weave_cni: Optional[str] = None,
                  weave_node: Optional[str] = None,
                  windows_pod_infra_container: Optional[str] = None):
         """
-        :param str aci_cni_deploy_container: Docker image for aci_cni_deploy_container (string)
-        :param str aci_controller_container: Docker image for aci_controller_container (string)
-        :param str aci_host_container: Docker image for aci_host_container (string)
-        :param str aci_mcast_container: Docker image for aci_mcast_container (string)
-        :param str aci_opflex_container: Docker image for aci_opflex_container (string)
-        :param str aci_ovs_container: Docker image for aci_ovs_container (string)
-        :param str alpine: Docker image for alpine (string)
-        :param str calico_cni: Docker image for calico_cni (string)
-        :param str calico_controllers: Docker image for calico_controllers (string)
-        :param str calico_ctl: Docker image for calico_ctl (string)
-        :param str calico_flex_vol: Docker image for calico_flex_vol (string)
-        :param str calico_node: Docker image for calico_node (string)
-        :param str canal_cni: Docker image for canal_cni (string)
-        :param str canal_flannel: Docker image for canal_flannel (string)
-        :param str canal_flex_vol: Docker image for canal_flex_vol (string)
-        :param str canal_node: Docker image for canal_node (string)
-        :param str cert_downloader: Docker image for cert_downloader (string)
-        :param str coredns: Docker image for coredns (string)
-        :param str coredns_autoscaler: Docker image for coredns_autoscaler (string)
-        :param str dnsmasq: Docker image for dnsmasq (string)
-        :param str etcd: Docker image for etcd (string)
-        :param str flannel: Docker image for flannel (string)
-        :param str flannel_cni: Docker image for flannel_cni (string)
         :param str ingress: RKE k8s cluster ingress controller configuration (list maxitems:1)
-        :param str ingress_backend: Docker image for ingress_backend (string)
-        :param str kube_dns: Docker image for kube_dns (string)
-        :param str kube_dns_autoscaler: Docker image for kube_dns_autoscaler (string)
-        :param str kube_dns_sidecar: Docker image for kube_dns_sidecar (string)
-        :param str kubernetes: Docker image for kubernetes (string)
-        :param str kubernetes_services_sidecar: Docker image for kubernetes_services_sidecar (string)
-        :param str metrics_server: Docker image for metrics_server (string)
-        :param str nginx_proxy: Docker image for nginx_proxy (string)
-        :param str nodelocal: Docker image for nodelocal (string)
-        :param str pod_infra_container: Docker image for pod_infra_container (string)
-        :param str weave_cni: Docker image for weave_cni (string)
-        :param str weave_node: Docker image for weave_node (string)
-        :param str windows_pod_infra_container: Docker image for windows_pod_infra_container (string)
         """
         if aci_cni_deploy_container is not None:
             pulumi.set(__self__, "aci_cni_deploy_container", aci_cni_deploy_container)
         if aci_controller_container is not None:
             pulumi.set(__self__, "aci_controller_container", aci_controller_container)
         if aci_host_container is not None:
             pulumi.set(__self__, "aci_host_container", aci_host_container)
@@ -9126,305 +7710,197 @@
             pulumi.set(__self__, "weave_node", weave_node)
         if windows_pod_infra_container is not None:
             pulumi.set(__self__, "windows_pod_infra_container", windows_pod_infra_container)
 
     @property
     @pulumi.getter(name="aciCniDeployContainer")
     def aci_cni_deploy_container(self) -> Optional[str]:
-        """
-        Docker image for aci_cni_deploy_container (string)
-        """
         return pulumi.get(self, "aci_cni_deploy_container")
 
     @property
     @pulumi.getter(name="aciControllerContainer")
     def aci_controller_container(self) -> Optional[str]:
-        """
-        Docker image for aci_controller_container (string)
-        """
         return pulumi.get(self, "aci_controller_container")
 
     @property
     @pulumi.getter(name="aciHostContainer")
     def aci_host_container(self) -> Optional[str]:
-        """
-        Docker image for aci_host_container (string)
-        """
         return pulumi.get(self, "aci_host_container")
 
     @property
     @pulumi.getter(name="aciMcastContainer")
     def aci_mcast_container(self) -> Optional[str]:
-        """
-        Docker image for aci_mcast_container (string)
-        """
         return pulumi.get(self, "aci_mcast_container")
 
     @property
     @pulumi.getter(name="aciOpflexContainer")
     def aci_opflex_container(self) -> Optional[str]:
-        """
-        Docker image for aci_opflex_container (string)
-        """
         return pulumi.get(self, "aci_opflex_container")
 
     @property
     @pulumi.getter(name="aciOvsContainer")
     def aci_ovs_container(self) -> Optional[str]:
-        """
-        Docker image for aci_ovs_container (string)
-        """
         return pulumi.get(self, "aci_ovs_container")
 
     @property
     @pulumi.getter
     def alpine(self) -> Optional[str]:
-        """
-        Docker image for alpine (string)
-        """
         return pulumi.get(self, "alpine")
 
     @property
     @pulumi.getter(name="calicoCni")
     def calico_cni(self) -> Optional[str]:
-        """
-        Docker image for calico_cni (string)
-        """
         return pulumi.get(self, "calico_cni")
 
     @property
     @pulumi.getter(name="calicoControllers")
     def calico_controllers(self) -> Optional[str]:
-        """
-        Docker image for calico_controllers (string)
-        """
         return pulumi.get(self, "calico_controllers")
 
     @property
     @pulumi.getter(name="calicoCtl")
     def calico_ctl(self) -> Optional[str]:
-        """
-        Docker image for calico_ctl (string)
-        """
         return pulumi.get(self, "calico_ctl")
 
     @property
     @pulumi.getter(name="calicoFlexVol")
     def calico_flex_vol(self) -> Optional[str]:
-        """
-        Docker image for calico_flex_vol (string)
-        """
         return pulumi.get(self, "calico_flex_vol")
 
     @property
     @pulumi.getter(name="calicoNode")
     def calico_node(self) -> Optional[str]:
-        """
-        Docker image for calico_node (string)
-        """
         return pulumi.get(self, "calico_node")
 
     @property
     @pulumi.getter(name="canalCni")
     def canal_cni(self) -> Optional[str]:
-        """
-        Docker image for canal_cni (string)
-        """
         return pulumi.get(self, "canal_cni")
 
     @property
     @pulumi.getter(name="canalFlannel")
     def canal_flannel(self) -> Optional[str]:
-        """
-        Docker image for canal_flannel (string)
-        """
         return pulumi.get(self, "canal_flannel")
 
     @property
     @pulumi.getter(name="canalFlexVol")
     def canal_flex_vol(self) -> Optional[str]:
-        """
-        Docker image for canal_flex_vol (string)
-        """
         return pulumi.get(self, "canal_flex_vol")
 
     @property
     @pulumi.getter(name="canalNode")
     def canal_node(self) -> Optional[str]:
-        """
-        Docker image for canal_node (string)
-        """
         return pulumi.get(self, "canal_node")
 
     @property
     @pulumi.getter(name="certDownloader")
     def cert_downloader(self) -> Optional[str]:
-        """
-        Docker image for cert_downloader (string)
-        """
         return pulumi.get(self, "cert_downloader")
 
     @property
     @pulumi.getter
     def coredns(self) -> Optional[str]:
-        """
-        Docker image for coredns (string)
-        """
         return pulumi.get(self, "coredns")
 
     @property
     @pulumi.getter(name="corednsAutoscaler")
     def coredns_autoscaler(self) -> Optional[str]:
-        """
-        Docker image for coredns_autoscaler (string)
-        """
         return pulumi.get(self, "coredns_autoscaler")
 
     @property
     @pulumi.getter
     def dnsmasq(self) -> Optional[str]:
-        """
-        Docker image for dnsmasq (string)
-        """
         return pulumi.get(self, "dnsmasq")
 
     @property
     @pulumi.getter
     def etcd(self) -> Optional[str]:
-        """
-        Docker image for etcd (string)
-        """
         return pulumi.get(self, "etcd")
 
     @property
     @pulumi.getter
     def flannel(self) -> Optional[str]:
-        """
-        Docker image for flannel (string)
-        """
         return pulumi.get(self, "flannel")
 
     @property
     @pulumi.getter(name="flannelCni")
     def flannel_cni(self) -> Optional[str]:
-        """
-        Docker image for flannel_cni (string)
-        """
         return pulumi.get(self, "flannel_cni")
 
     @property
     @pulumi.getter
     def ingress(self) -> Optional[str]:
         """
         RKE k8s cluster ingress controller configuration (list maxitems:1)
         """
         return pulumi.get(self, "ingress")
 
     @property
     @pulumi.getter(name="ingressBackend")
     def ingress_backend(self) -> Optional[str]:
-        """
-        Docker image for ingress_backend (string)
-        """
         return pulumi.get(self, "ingress_backend")
 
     @property
     @pulumi.getter(name="kubeDns")
     def kube_dns(self) -> Optional[str]:
-        """
-        Docker image for kube_dns (string)
-        """
         return pulumi.get(self, "kube_dns")
 
     @property
     @pulumi.getter(name="kubeDnsAutoscaler")
     def kube_dns_autoscaler(self) -> Optional[str]:
-        """
-        Docker image for kube_dns_autoscaler (string)
-        """
         return pulumi.get(self, "kube_dns_autoscaler")
 
     @property
     @pulumi.getter(name="kubeDnsSidecar")
     def kube_dns_sidecar(self) -> Optional[str]:
-        """
-        Docker image for kube_dns_sidecar (string)
-        """
         return pulumi.get(self, "kube_dns_sidecar")
 
     @property
     @pulumi.getter
     def kubernetes(self) -> Optional[str]:
-        """
-        Docker image for kubernetes (string)
-        """
         return pulumi.get(self, "kubernetes")
 
     @property
     @pulumi.getter(name="kubernetesServicesSidecar")
     def kubernetes_services_sidecar(self) -> Optional[str]:
-        """
-        Docker image for kubernetes_services_sidecar (string)
-        """
         return pulumi.get(self, "kubernetes_services_sidecar")
 
     @property
     @pulumi.getter(name="metricsServer")
     def metrics_server(self) -> Optional[str]:
-        """
-        Docker image for metrics_server (string)
-        """
         return pulumi.get(self, "metrics_server")
 
     @property
     @pulumi.getter(name="nginxProxy")
     def nginx_proxy(self) -> Optional[str]:
-        """
-        Docker image for nginx_proxy (string)
-        """
         return pulumi.get(self, "nginx_proxy")
 
     @property
     @pulumi.getter
     def nodelocal(self) -> Optional[str]:
-        """
-        Docker image for nodelocal (string)
-        """
         return pulumi.get(self, "nodelocal")
 
     @property
     @pulumi.getter(name="podInfraContainer")
     def pod_infra_container(self) -> Optional[str]:
-        """
-        Docker image for pod_infra_container (string)
-        """
         return pulumi.get(self, "pod_infra_container")
 
     @property
     @pulumi.getter(name="weaveCni")
     def weave_cni(self) -> Optional[str]:
-        """
-        Docker image for weave_cni (string)
-        """
         return pulumi.get(self, "weave_cni")
 
     @property
     @pulumi.getter(name="weaveNode")
     def weave_node(self) -> Optional[str]:
-        """
-        Docker image for weave_node (string)
-        """
         return pulumi.get(self, "weave_node")
 
     @property
     @pulumi.getter(name="windowsPodInfraContainer")
     def windows_pod_infra_container(self) -> Optional[str]:
-        """
-        Docker image for windows_pod_infra_container (string)
-        """
         return pulumi.get(self, "windows_pod_infra_container")
 
 
 @pulumi.output_type
 class ClusterUpgradeStrategy(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9448,59 +7924,41 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  drain: Optional[bool] = None,
                  drain_input: Optional['outputs.ClusterUpgradeStrategyDrainInput'] = None,
                  max_unavailable_controlplane: Optional[str] = None,
                  max_unavailable_worker: Optional[str] = None):
-        """
-        :param bool drain: RKE drain nodes (bool)
-        :param 'ClusterUpgradeStrategyDrainInputArgs' drain_input: RKE drain node input (list Maxitems: 1)
-        :param str max_unavailable_controlplane: RKE max unavailable controlplane nodes (string)
-        :param str max_unavailable_worker: RKE max unavailable worker nodes (string)
-        """
         if drain is not None:
             pulumi.set(__self__, "drain", drain)
         if drain_input is not None:
             pulumi.set(__self__, "drain_input", drain_input)
         if max_unavailable_controlplane is not None:
             pulumi.set(__self__, "max_unavailable_controlplane", max_unavailable_controlplane)
         if max_unavailable_worker is not None:
             pulumi.set(__self__, "max_unavailable_worker", max_unavailable_worker)
 
     @property
     @pulumi.getter
     def drain(self) -> Optional[bool]:
-        """
-        RKE drain nodes (bool)
-        """
         return pulumi.get(self, "drain")
 
     @property
     @pulumi.getter(name="drainInput")
     def drain_input(self) -> Optional['outputs.ClusterUpgradeStrategyDrainInput']:
-        """
-        RKE drain node input (list Maxitems: 1)
-        """
         return pulumi.get(self, "drain_input")
 
     @property
     @pulumi.getter(name="maxUnavailableControlplane")
     def max_unavailable_controlplane(self) -> Optional[str]:
-        """
-        RKE max unavailable controlplane nodes (string)
-        """
         return pulumi.get(self, "max_unavailable_controlplane")
 
     @property
     @pulumi.getter(name="maxUnavailableWorker")
     def max_unavailable_worker(self) -> Optional[str]:
-        """
-        RKE max unavailable worker nodes (string)
-        """
         return pulumi.get(self, "max_unavailable_worker")
 
 
 @pulumi.output_type
 class ClusterUpgradeStrategyDrainInput(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9525,70 +7983,48 @@
 
     def __init__(__self__, *,
                  delete_local_data: Optional[bool] = None,
                  force: Optional[bool] = None,
                  grace_period: Optional[int] = None,
                  ignore_daemon_sets: Optional[bool] = None,
                  timeout: Optional[int] = None):
-        """
-        :param bool delete_local_data: Delete RKE node local data (bool)
-        :param bool force: Force RKE node drain (bool)
-        :param int grace_period: RKE node drain grace period (int)
-        :param bool ignore_daemon_sets: Ignore RKE daemon sets (bool)
-        :param int timeout: RKE node drain timeout (int)
-        """
         if delete_local_data is not None:
             pulumi.set(__self__, "delete_local_data", delete_local_data)
         if force is not None:
             pulumi.set(__self__, "force", force)
         if grace_period is not None:
             pulumi.set(__self__, "grace_period", grace_period)
         if ignore_daemon_sets is not None:
             pulumi.set(__self__, "ignore_daemon_sets", ignore_daemon_sets)
         if timeout is not None:
             pulumi.set(__self__, "timeout", timeout)
 
     @property
     @pulumi.getter(name="deleteLocalData")
     def delete_local_data(self) -> Optional[bool]:
-        """
-        Delete RKE node local data (bool)
-        """
         return pulumi.get(self, "delete_local_data")
 
     @property
     @pulumi.getter
     def force(self) -> Optional[bool]:
-        """
-        Force RKE node drain (bool)
-        """
         return pulumi.get(self, "force")
 
     @property
     @pulumi.getter(name="gracePeriod")
     def grace_period(self) -> Optional[int]:
-        """
-        RKE node drain grace period (int)
-        """
         return pulumi.get(self, "grace_period")
 
     @property
     @pulumi.getter(name="ignoreDaemonSets")
     def ignore_daemon_sets(self) -> Optional[bool]:
-        """
-        Ignore RKE daemon sets (bool)
-        """
         return pulumi.get(self, "ignore_daemon_sets")
 
     @property
     @pulumi.getter
     def timeout(self) -> Optional[int]:
-        """
-        RKE node drain timeout (int)
-        """
         return pulumi.get(self, "timeout")
 
 
 @pulumi.output_type
 class ClusterWorkerHost(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -9606,33 +8042,23 @@
     def get(self, key: str, default = None) -> Any:
         ClusterWorkerHost.__key_warning(key)
         return super().get(key, default)
 
     def __init__(__self__, *,
                  address: Optional[str] = None,
                  node_name: Optional[str] = None):
-        """
-        :param str address: Address ip for node (string)
-        :param str node_name: Name of the host provisioned via docker machine (string)
-        """
         if address is not None:
             pulumi.set(__self__, "address", address)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
 
     @property
     @pulumi.getter
     def address(self) -> Optional[str]:
-        """
-        Address ip for node (string)
-        """
         return pulumi.get(self, "address")
 
     @property
     @pulumi.getter(name="nodeName")
     def node_name(self) -> Optional[str]:
-        """
-        Name of the host provisioned via docker machine (string)
-        """
         return pulumi.get(self, "node_name")
```

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke/provider.py` & `pulumi_rke-3.5.0a1713905146/pulumi_rke/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_rke-3.5.0a1713561359/pulumi_rke.egg-info/PKG-INFO` & `pulumi_rke-3.5.0a1713905146/pulumi_rke.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_rke
-Version: 3.5.0a1713561359
+Version: 3.5.0a1713905146
 Summary: A Pulumi package for creating and managing rke cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-rke
 Keywords: pulumi,rke
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_rke-3.5.0a1713561359/pyproject.toml` & `pulumi_rke-3.5.0a1713905146/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_rke"
   description = "A Pulumi package for creating and managing rke cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "rke"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "3.5.0a1713561359"
+  version = "3.5.0a1713905146"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-rke"
 
 [build-system]
```

