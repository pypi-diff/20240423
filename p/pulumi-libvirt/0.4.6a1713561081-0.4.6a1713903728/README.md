# Comparing `tmp/pulumi_libvirt-0.4.6a1713561081.tar.gz` & `tmp/pulumi_libvirt-0.4.6a1713903728.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.4.6a1713561081.tar", last modified: Fri Apr 19 21:14:00 2024, max compression
+gzip compressed data, was "pulumi_libvirt-0.4.6a1713903728.tar", last modified: Tue Apr 23 20:29:14 2024, max compression
```

## Comparing `pulumi_libvirt-0.4.6a1713561081.tar` & `pulumi_libvirt-0.4.6a1713903728.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    50939 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    89513 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (127)    34091 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    44378 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16314 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    28986 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-19 21:14:00.000000 pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 21:13:54.000000 pulumi_libvirt-0.4.6a1713561081/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:14:00.661391 pulumi_libvirt-0.4.6a1713561081/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2049 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42947 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14573 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70503 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8813 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31821 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36652 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16158 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4666 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    28830 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-23 20:29:14.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-23 20:29:14.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:29:14.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-23 20:29:14.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-23 20:29:14.000000 pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-23 20:29:08.000000 pulumi_libvirt-0.4.6a1713903728/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:29:14.168706 pulumi_libvirt-0.4.6a1713903728/setup.cfg
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/PKG-INFO` & `pulumi_libvirt-0.4.6a1713903728/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.6a1713561081
+Version: 0.4.6a1713903728
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/README.md` & `pulumi_libvirt-0.4.6a1713903728/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/network.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,19 +37,15 @@
                the DHCP server.
                No DHCP server will be started if `addresses` is omitted.
         :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
                If not specified `false` is assumed.
         :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
                device which will be used to construct the virtual network (when not provided,
                it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input['NetworkDhcpArgs'] dhcp: DHCP configuration. 
-               You need to use it in conjuction with the adresses variable.
         :param pulumi.Input['NetworkDnsArgs'] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input['NetworkDnsmasqOptionsArgs'] dnsmasq_options: configuration of Dnsmasq options for the network
-               You need to provide a list of option name and value pairs.
         :param pulumi.Input[str] domain: The domain used by the DNS server.
         :param pulumi.Input[str] mode: One of:
         :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
                not supplied, libvirt will use the default for the interface, usually 1500.
                Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
@@ -124,18 +120,14 @@
     @bridge.setter
     def bridge(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bridge", value)
 
     @property
     @pulumi.getter
     def dhcp(self) -> Optional[pulumi.Input['NetworkDhcpArgs']]:
-        """
-        DHCP configuration. 
-        You need to use it in conjuction with the adresses variable.
-        """
         return pulumi.get(self, "dhcp")
 
     @dhcp.setter
     def dhcp(self, value: Optional[pulumi.Input['NetworkDhcpArgs']]):
         pulumi.set(self, "dhcp", value)
 
     @property
@@ -149,18 +141,14 @@
     @dns.setter
     def dns(self, value: Optional[pulumi.Input['NetworkDnsArgs']]):
         pulumi.set(self, "dns", value)
 
     @property
     @pulumi.getter(name="dnsmasqOptions")
     def dnsmasq_options(self) -> Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]:
-        """
-        configuration of Dnsmasq options for the network
-        You need to provide a list of option name and value pairs.
-        """
         return pulumi.get(self, "dnsmasq_options")
 
     @dnsmasq_options.setter
     def dnsmasq_options(self, value: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]):
         pulumi.set(self, "dnsmasq_options", value)
 
     @property
@@ -261,19 +249,15 @@
                the DHCP server.
                No DHCP server will be started if `addresses` is omitted.
         :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
                If not specified `false` is assumed.
         :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
                device which will be used to construct the virtual network (when not provided,
                it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input['NetworkDhcpArgs'] dhcp: DHCP configuration. 
-               You need to use it in conjuction with the adresses variable.
         :param pulumi.Input['NetworkDnsArgs'] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input['NetworkDnsmasqOptionsArgs'] dnsmasq_options: configuration of Dnsmasq options for the network
-               You need to provide a list of option name and value pairs.
         :param pulumi.Input[str] domain: The domain used by the DNS server.
         :param pulumi.Input[str] mode: One of:
         :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
                not supplied, libvirt will use the default for the interface, usually 1500.
                Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
@@ -348,18 +332,14 @@
     @bridge.setter
     def bridge(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "bridge", value)
 
     @property
     @pulumi.getter
     def dhcp(self) -> Optional[pulumi.Input['NetworkDhcpArgs']]:
-        """
-        DHCP configuration. 
-        You need to use it in conjuction with the adresses variable.
-        """
         return pulumi.get(self, "dhcp")
 
     @dhcp.setter
     def dhcp(self, value: Optional[pulumi.Input['NetworkDhcpArgs']]):
         pulumi.set(self, "dhcp", value)
 
     @property
@@ -373,18 +353,14 @@
     @dns.setter
     def dns(self, value: Optional[pulumi.Input['NetworkDnsArgs']]):
         pulumi.set(self, "dns", value)
 
     @property
     @pulumi.getter(name="dnsmasqOptions")
     def dnsmasq_options(self) -> Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]:
-        """
-        configuration of Dnsmasq options for the network
-        You need to provide a list of option name and value pairs.
-        """
         return pulumi.get(self, "dnsmasq_options")
 
     @dnsmasq_options.setter
     def dnsmasq_options(self, value: Optional[pulumi.Input['NetworkDnsmasqOptionsArgs']]):
         pulumi.set(self, "dnsmasq_options", value)
 
     @property
@@ -492,19 +468,15 @@
                the DHCP server.
                No DHCP server will be started if `addresses` is omitted.
         :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
                If not specified `false` is assumed.
         :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
                device which will be used to construct the virtual network (when not provided,
                it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input[pulumi.InputType['NetworkDhcpArgs']] dhcp: DHCP configuration. 
-               You need to use it in conjuction with the adresses variable.
         :param pulumi.Input[pulumi.InputType['NetworkDnsArgs']] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[pulumi.InputType['NetworkDnsmasqOptionsArgs']] dnsmasq_options: configuration of Dnsmasq options for the network
-               You need to provide a list of option name and value pairs.
         :param pulumi.Input[str] domain: The domain used by the DNS server.
         :param pulumi.Input[str] mode: One of:
         :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
                not supplied, libvirt will use the default for the interface, usually 1500.
                Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
@@ -605,19 +577,15 @@
                the DHCP server.
                No DHCP server will be started if `addresses` is omitted.
         :param pulumi.Input[bool] autostart: Set to `true` to start the network on host boot up.
                If not specified `false` is assumed.
         :param pulumi.Input[str] bridge: The bridge device defines the name of a bridge
                device which will be used to construct the virtual network (when not provided,
                it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
-        :param pulumi.Input[pulumi.InputType['NetworkDhcpArgs']] dhcp: DHCP configuration. 
-               You need to use it in conjuction with the adresses variable.
         :param pulumi.Input[pulumi.InputType['NetworkDnsArgs']] dns: configuration of DNS specific settings for the network
-        :param pulumi.Input[pulumi.InputType['NetworkDnsmasqOptionsArgs']] dnsmasq_options: configuration of Dnsmasq options for the network
-               You need to provide a list of option name and value pairs.
         :param pulumi.Input[str] domain: The domain used by the DNS server.
         :param pulumi.Input[str] mode: One of:
         :param pulumi.Input[int] mtu: The MTU to set for the underlying network interfaces. When
                not supplied, libvirt will use the default for the interface, usually 1500.
                Libvirt version 5.1 and greater will advertise this value to nodes via DHCP.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
                Changing this forces a new resource to be created.
@@ -673,35 +641,27 @@
         it will be automatically obtained by libvirt in `none`, `nat`, `route` and `open` modes).
         """
         return pulumi.get(self, "bridge")
 
     @property
     @pulumi.getter
     def dhcp(self) -> pulumi.Output['outputs.NetworkDhcp']:
-        """
-        DHCP configuration. 
-        You need to use it in conjuction with the adresses variable.
-        """
         return pulumi.get(self, "dhcp")
 
     @property
     @pulumi.getter
     def dns(self) -> pulumi.Output['outputs.NetworkDns']:
         """
         configuration of DNS specific settings for the network
         """
         return pulumi.get(self, "dns")
 
     @property
     @pulumi.getter(name="dnsmasqOptions")
     def dnsmasq_options(self) -> pulumi.Output[Optional['outputs.NetworkDnsmasqOptions']]:
-        """
-        configuration of Dnsmasq options for the network
-        You need to provide a list of option name and value pairs.
-        """
         return pulumi.get(self, "dnsmasq_options")
 
     @property
     @pulumi.getter
     def domain(self) -> pulumi.Output[Optional[str]]:
         """
         The domain used by the DNS server.
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -80,15 +80,15 @@
                  type: str,
                  source_host: Optional[str] = None,
                  source_path: Optional[str] = None,
                  source_service: Optional[str] = None,
                  target_type: Optional[str] = None):
         """
         :param str target_port: Target port
-        :param str type: The type of hypervisor to use for the domain.  Defaults to `kvm`, other values can be found [here](https://libvirt.org/formatdomain.html#id1)
+        :param str type: Console device type. Valid values are "pty" and "tcp".
         :param str source_host: IP address to listen on. Defaults to 127.0.0.1.
         :param str source_path: Source path
                
                Additional attributes when type is "tcp":
         :param str source_service: Port number or a service name. Defaults to a
                random port.
                
@@ -121,15 +121,15 @@
         """
         return pulumi.get(self, "target_port")
 
     @property
     @pulumi.getter
     def type(self) -> str:
         """
-        The type of hypervisor to use for the domain.  Defaults to `kvm`, other values can be found [here](https://libvirt.org/formatdomain.html#id1)
+        Console device type. Valid values are "pty" and "tcp".
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter(name="sourceHost")
     def source_host(self) -> Optional[str]:
         """
@@ -224,15 +224,14 @@
                model is set to `virtio-scsi`
         :param str url: The http url to use as the block device for this disk (read-only)
         :param str volume_id: The volume id to use for this disk.
         :param str wwn: Specify a WWN to use for the disk if the disk is using
                a scsi controller, if not specified then a random wwn is generated for the disk
                
                
-               <!--Start PulumiCodeChooser -->
                ```python
                import pulumi
                import pulumi_libvirt as libvirt
                
                leap = libvirt.Volume("leap",
                    name="leap",
                    source="http://someurl/openSUSE_Leap-42.1.qcow2")
@@ -253,15 +252,14 @@
                            file="/absolute/path/to/disk.iso",
                        ),
                        libvirt.DomainDiskArgs(
                            block_device="/dev/mapper/36005076802810e55400000000000145f",
                        ),
                    ])
                ```
-               <!--End PulumiCodeChooser -->
                
                Also note that the `disk` block is actually a list of maps, so it is possible to
                declare several of them by using either the literal list and map syntax as in
                the following examples:
         """
         if block_device is not None:
             pulumi.set(__self__, "block_device", block_device)
@@ -323,15 +321,14 @@
     @pulumi.getter
     def wwn(self) -> Optional[str]:
         """
         Specify a WWN to use for the disk if the disk is using
         a scsi controller, if not specified then a random wwn is generated for the disk
 
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         leap = libvirt.Volume("leap",
             name="leap",
             source="http://someurl/openSUSE_Leap-42.1.qcow2")
@@ -352,15 +349,14 @@
                     file="/absolute/path/to/disk.iso",
                 ),
                 libvirt.DomainDiskArgs(
                     block_device="/dev/mapper/36005076802810e55400000000000145f",
                 ),
             ])
         ```
-        <!--End PulumiCodeChooser -->
 
         Also note that the `disk` block is actually a list of maps, so it is possible to
         declare several of them by using either the literal list and map syntax as in
         the following examples:
         """
         return pulumi.get(self, "wwn")
 
@@ -368,67 +364,39 @@
 @pulumi.output_type
 class DomainFilesystem(dict):
     def __init__(__self__, *,
                  source: str,
                  target: str,
                  accessmode: Optional[str] = None,
                  readonly: Optional[bool] = None):
-        """
-        :param str source: the directory of the host to be shared with the guest.
-        :param str target: an arbitrary string tag that is exported to the guest as a hint for
-               where to mount the source.
-        :param str accessmode: specifies the security mode for accessing the source. By default
-               the `mapped` mode is chosen.
-        :param bool readonly: enables exporting filesystem as a readonly mount for guest, by
-               default read-only access is given.
-               
-               Example:
-        """
         pulumi.set(__self__, "source", source)
         pulumi.set(__self__, "target", target)
         if accessmode is not None:
             pulumi.set(__self__, "accessmode", accessmode)
         if readonly is not None:
             pulumi.set(__self__, "readonly", readonly)
 
     @property
     @pulumi.getter
     def source(self) -> str:
-        """
-        the directory of the host to be shared with the guest.
-        """
         return pulumi.get(self, "source")
 
     @property
     @pulumi.getter
     def target(self) -> str:
-        """
-        an arbitrary string tag that is exported to the guest as a hint for
-        where to mount the source.
-        """
         return pulumi.get(self, "target")
 
     @property
     @pulumi.getter
     def accessmode(self) -> Optional[str]:
-        """
-        specifies the security mode for accessing the source. By default
-        the `mapped` mode is chosen.
-        """
         return pulumi.get(self, "accessmode")
 
     @property
     @pulumi.getter
     def readonly(self) -> Optional[bool]:
-        """
-        enables exporting filesystem as a readonly mount for guest, by
-        default read-only access is given.
-
-        Example:
-        """
         return pulumi.get(self, "readonly")
 
 
 @pulumi.output_type
 class DomainGraphics(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -456,15 +424,15 @@
                  type: Optional[str] = None,
                  websocket: Optional[int] = None):
         """
         :param bool autoport: defaults to "yes"
         :param str listen_address: IP Address where the VNC listener should be started if
                `listen_type` is set to `address`. Defaults to 127.0.0.1
         :param str listen_type: "listen type", defaults to "none"
-        :param str type: The type of hypervisor to use for the domain.  Defaults to `kvm`, other values can be found [here](https://libvirt.org/formatdomain.html#id1)
+        :param str type: the type of graphics emulation (default is "spice")
         :param int websocket: Port to listen on for VNC WebSocket functionality (-1 meaning auto-allocation)
                
                On occasion we have found it necessary to set a `type` of `vnc` and a
                `listen_type` of `address` with certain builds of QEMU.
                
                With `listen_address` it is possible to specify a listener address for the virtual
                machines VNC server. Usually this is an IP of the host system.
@@ -507,15 +475,15 @@
         """
         return pulumi.get(self, "listen_type")
 
     @property
     @pulumi.getter
     def type(self) -> Optional[str]:
         """
-        The type of hypervisor to use for the domain.  Defaults to `kvm`, other values can be found [here](https://libvirt.org/formatdomain.html#id1)
+        the type of graphics emulation (default is "spice")
         """
         return pulumi.get(self, "type")
 
     @property
     @pulumi.getter
     def websocket(self) -> Optional[int]:
         """
@@ -562,46 +530,14 @@
                  mac: Optional[str] = None,
                  macvtap: Optional[str] = None,
                  network_id: Optional[str] = None,
                  network_name: Optional[str] = None,
                  passthrough: Optional[str] = None,
                  vepa: Optional[str] = None,
                  wait_for_lease: Optional[bool] = None):
-        """
-        :param Sequence[str] addresses: An IP address for this domain in this network.
-        :param str bridge: Provides a bridge from the VM directly to the LAN. This assumes
-               there is a bridge device on the host which has one or more of the hosts
-               physical NICs enslaved. The guest VM will have an associated _tun_ device
-               created and enslaved to the bridge. The IP range / network configuration is
-               whatever is used on the LAN. This provides the guest VM full incoming &
-               outgoing net access just like a physical machine.
-        :param str hostname: A hostname that will be assigned to this domain
-               resource in this network.
-        :param str mac: The specific MAC address to use for this interface.
-        :param str macvtap: Packets whose destination is on the same host as where they
-               originate from are directly delivered to the target macvtap device. Both
-               origin and destination devices need to be in bridge mode for direct delivery.
-               If either one of them is in vepa mode, a VEPA capable bridge is required.
-        :param str passthrough: This feature attaches a virtual function of a SRIOV capable
-               NIC directly to a VM without losing the migration capability. All packets are
-               sent to the VF/IF of the configured network device. Depending on the
-               capabilities of the device additional prerequisites or limitations may apply;
-               for example, on Linux this requires kernel 2.6.38 or newer.
-               
-               Example of a `macvtap` interface:
-        :param str vepa: All VMs' packets are sent to the external bridge. Packets whose
-               destination is a VM on the same host as where the packet originates from are
-               sent back to the host by the VEPA capable bridge (today's bridges are
-               typically not VEPA capable).
-        :param bool wait_for_lease: When creating the domain resource, wait until the
-               network interface gets a DHCP lease from libvirt, so that the computed IP
-               addresses will be available when the domain is up and the plan applied.
-               
-               When connecting to a LAN, users can specify a target device with:
-        """
         if addresses is not None:
             pulumi.set(__self__, "addresses", addresses)
         if bridge is not None:
             pulumi.set(__self__, "bridge", bridge)
         if hostname is not None:
             pulumi.set(__self__, "hostname", hostname)
         if mac is not None:
@@ -618,58 +554,34 @@
             pulumi.set(__self__, "vepa", vepa)
         if wait_for_lease is not None:
             pulumi.set(__self__, "wait_for_lease", wait_for_lease)
 
     @property
     @pulumi.getter
     def addresses(self) -> Optional[Sequence[str]]:
-        """
-        An IP address for this domain in this network.
-        """
         return pulumi.get(self, "addresses")
 
     @property
     @pulumi.getter
     def bridge(self) -> Optional[str]:
-        """
-        Provides a bridge from the VM directly to the LAN. This assumes
-        there is a bridge device on the host which has one or more of the hosts
-        physical NICs enslaved. The guest VM will have an associated _tun_ device
-        created and enslaved to the bridge. The IP range / network configuration is
-        whatever is used on the LAN. This provides the guest VM full incoming &
-        outgoing net access just like a physical machine.
-        """
         return pulumi.get(self, "bridge")
 
     @property
     @pulumi.getter
     def hostname(self) -> Optional[str]:
-        """
-        A hostname that will be assigned to this domain
-        resource in this network.
-        """
         return pulumi.get(self, "hostname")
 
     @property
     @pulumi.getter
     def mac(self) -> Optional[str]:
-        """
-        The specific MAC address to use for this interface.
-        """
         return pulumi.get(self, "mac")
 
     @property
     @pulumi.getter
     def macvtap(self) -> Optional[str]:
-        """
-        Packets whose destination is on the same host as where they
-        originate from are directly delivered to the target macvtap device. Both
-        origin and destination devices need to be in bridge mode for direct delivery.
-        If either one of them is in vepa mode, a VEPA capable bridge is required.
-        """
         return pulumi.get(self, "macvtap")
 
     @property
     @pulumi.getter(name="networkId")
     def network_id(self) -> Optional[str]:
         return pulumi.get(self, "network_id")
 
@@ -677,82 +589,44 @@
     @pulumi.getter(name="networkName")
     def network_name(self) -> Optional[str]:
         return pulumi.get(self, "network_name")
 
     @property
     @pulumi.getter
     def passthrough(self) -> Optional[str]:
-        """
-        This feature attaches a virtual function of a SRIOV capable
-        NIC directly to a VM without losing the migration capability. All packets are
-        sent to the VF/IF of the configured network device. Depending on the
-        capabilities of the device additional prerequisites or limitations may apply;
-        for example, on Linux this requires kernel 2.6.38 or newer.
-
-        Example of a `macvtap` interface:
-        """
         return pulumi.get(self, "passthrough")
 
     @property
     @pulumi.getter
     def vepa(self) -> Optional[str]:
-        """
-        All VMs' packets are sent to the external bridge. Packets whose
-        destination is a VM on the same host as where the packet originates from are
-        sent back to the host by the VEPA capable bridge (today's bridges are
-        typically not VEPA capable).
-        """
         return pulumi.get(self, "vepa")
 
     @property
     @pulumi.getter(name="waitForLease")
     def wait_for_lease(self) -> Optional[bool]:
-        """
-        When creating the domain resource, wait until the
-        network interface gets a DHCP lease from libvirt, so that the computed IP
-        addresses will be available when the domain is up and the plan applied.
-
-        When connecting to a LAN, users can specify a target device with:
-        """
         return pulumi.get(self, "wait_for_lease")
 
 
 @pulumi.output_type
 class DomainNvram(dict):
     def __init__(__self__, *,
                  file: str,
                  template: Optional[str] = None):
-        """
-        :param str file: The filename to use as the block device for this disk (read-only)
-        :param str template: path to the file used to override variables from the master NVRAM
-               store.
-               
-               So you should typically use the firmware as this,
-        """
         pulumi.set(__self__, "file", file)
         if template is not None:
             pulumi.set(__self__, "template", template)
 
     @property
     @pulumi.getter
     def file(self) -> str:
-        """
-        The filename to use as the block device for this disk (read-only)
-        """
         return pulumi.get(self, "file")
 
     @property
     @pulumi.getter
     def template(self) -> Optional[str]:
-        """
-        path to the file used to override variables from the master NVRAM
-        store.
-
-        So you should typically use the firmware as this,
-        """
         return pulumi.get(self, "template")
 
 
 @pulumi.output_type
 class DomainTpm(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -896,26 +770,20 @@
         return pulumi.get(self, "xslt")
 
 
 @pulumi.output_type
 class NetworkDhcp(dict):
     def __init__(__self__, *,
                  enabled: Optional[bool] = None):
-        """
-        :param bool enabled: when false, disable the DHCP server
-        """
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        when false, disable the DHCP server
-        """
         return pulumi.get(self, "enabled")
 
 
 @pulumi.output_type
 class NetworkDns(dict):
     @staticmethod
     def __key_warning(key: str):
@@ -937,15 +805,14 @@
     def __init__(__self__, *,
                  enabled: Optional[bool] = None,
                  forwarders: Optional[Sequence['outputs.NetworkDnsForwarder']] = None,
                  hosts: Optional[Sequence['outputs.NetworkDnsHost']] = None,
                  local_only: Optional[bool] = None,
                  srvs: Optional[Sequence['outputs.NetworkDnsSrv']] = None):
         """
-        :param bool enabled: when false, disable the DHCP server
         :param Sequence['NetworkDnsForwarderArgs'] forwarders: Either `address`, `domain`, or both must be set
         :param Sequence['NetworkDnsHostArgs'] hosts: a DNS host entry block. You can have one or more of these
                blocks in your DNS definition. You must specify both `ip` and `hostname`.
                
                An advanced example of round-robin DNS (using DNS host templates) follows:
         :param bool local_only: true/false: true means 'do not forward unresolved requests for this domain to the part DNS server
         :param Sequence['NetworkDnsSrvArgs'] srvs: a DNS SRV entry block. You can have one or more of these blocks
@@ -961,17 +828,14 @@
             pulumi.set(__self__, "local_only", local_only)
         if srvs is not None:
             pulumi.set(__self__, "srvs", srvs)
 
     @property
     @pulumi.getter
     def enabled(self) -> Optional[bool]:
-        """
-        when false, disable the DHCP server
-        """
         return pulumi.get(self, "enabled")
 
     @property
     @pulumi.getter
     def forwarders(self) -> Optional[Sequence['outputs.NetworkDnsForwarder']]:
         """
         Either `address`, `domain`, or both must be set
@@ -1122,34 +986,20 @@
         return pulumi.get(self, "weight")
 
 
 @pulumi.output_type
 class NetworkDnsmasqOptions(dict):
     def __init__(__self__, *,
                  options: Optional[Sequence['outputs.NetworkDnsmasqOptionsOption']] = None):
-        """
-        :param Sequence['NetworkDnsmasqOptionsOptionArgs'] options: a Dnsmasq option entry block. You can have one or more of these
-               blocks in your definition. You must specify `option_name` while `option_value` is
-               optional to support value-less options.
-               
-               An example of setting Dnsmasq options (using Dnsmasq option templates) follows:
-        """
         if options is not None:
             pulumi.set(__self__, "options", options)
 
     @property
     @pulumi.getter
     def options(self) -> Optional[Sequence['outputs.NetworkDnsmasqOptionsOption']]:
-        """
-        a Dnsmasq option entry block. You can have one or more of these
-        blocks in your definition. You must specify `option_name` while `option_value` is
-        optional to support value-less options.
-
-        An example of setting Dnsmasq options (using Dnsmasq option templates) follows:
-        """
         return pulumi.get(self, "options")
 
 
 @pulumi.output_type
 class NetworkDnsmasqOptionsOption(dict):
     @staticmethod
     def __key_warning(key: str):
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,30 +241,28 @@
         Manages a storage pool in libvirt. Currently only directory-based storage pool are supported. For more information on
         storage pools in libvirt, see [the official documentation](https://libvirt.org/formatstorage.html).
 
         **WARNING:** This is experimental API and may change in the future.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # A pool for all cluster volumes
         cluster = libvirt.Pool("cluster",
             name="cluster",
             type="dir",
             path="/home/user/cluster_storage")
         opensuse_leap = libvirt.Volume("opensuse_leap",
             name="opensuse_leap",
             pool=cluster.name,
             source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] name: A unique name for the resource, required by libvirt.
         :param pulumi.Input[str] path: The directory where the pool will keep all its volumes. This is only relevant to (and required by)
                the "dir" type pools.
         :param pulumi.Input[str] type: The type of the pool. Currently, only "dir" supported.
@@ -279,30 +277,28 @@
         Manages a storage pool in libvirt. Currently only directory-based storage pool are supported. For more information on
         storage pools in libvirt, see [the official documentation](https://libvirt.org/formatstorage.html).
 
         **WARNING:** This is experimental API and may change in the future.
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # A pool for all cluster volumes
         cluster = libvirt.Pool("cluster",
             name="cluster",
             type="dir",
             path="/home/user/cluster_storage")
         opensuse_leap = libvirt.Volume("opensuse_leap",
             name="opensuse_leap",
             pool=cluster.name,
             source="http://download.opensuse.org/repositories/Cloud:/Images:/Leap_42.1/images/openSUSE-Leap-42.1-OpenStack.x86_64.qcow2")
         ```
-        <!--End PulumiCodeChooser -->
 
         :param str resource_name: The name of the resource.
         :param PoolArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,14 @@
                  __props__=None):
         """
         Manages a storage volume in libvirt. For more information see
         [the official documentation](https://libvirt.org/formatstorage.html).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # Base OS image to use to create a cluster of different
         # nodes
         opensuse_leap = libvirt.Volume("opensuse_leap",
@@ -371,15 +370,14 @@
         # volumes to attach to the "workers" domains as main disk
         worker = []
         for range in [{"value": i} for i in range(0, workers_count)]:
             worker.append(libvirt.Volume(f"worker-{range['value']}",
                 name=f"worker_{range['value']}.qcow2",
                 base_volume_id=opensuse_leap.id))
         ```
-        <!--End PulumiCodeChooser -->
 
         > **Tip:** when provisioning multiple domains using the same base image, create
         a `Volume` for the base image and then define the domain specific ones
         as based on it. This way the image will not be modified and no extra disk space
         is going to be used for the base image.
 
         :param str resource_name: The name of the resource.
@@ -409,15 +407,14 @@
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         Manages a storage volume in libvirt. For more information see
         [the official documentation](https://libvirt.org/formatstorage.html).
 
         ## Example Usage
 
-        <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_libvirt as libvirt
 
         # Base OS image to use to create a cluster of different
         # nodes
         opensuse_leap = libvirt.Volume("opensuse_leap",
@@ -430,15 +427,14 @@
         # volumes to attach to the "workers" domains as main disk
         worker = []
         for range in [{"value": i} for i in range(0, workers_count)]:
             worker.append(libvirt.Volume(f"worker-{range['value']}",
                 name=f"worker_{range['value']}.qcow2",
                 base_volume_id=opensuse_leap.id))
         ```
-        <!--End PulumiCodeChooser -->
 
         > **Tip:** when provisioning multiple domains using the same base image, create
         a `Volume` for the base image and then define the domain specific ones
         as based on it. This way the image will not be modified and no extra disk space
         is going to be used for the base image.
 
         :param str resource_name: The name of the resource.
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.6a1713561081
+Version: 0.4.6a1713903728
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi,libvirt
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_libvirt-0.4.6a1713561081/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.4.6a1713903728/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.6a1713561081/pyproject.toml` & `pulumi_libvirt-0.4.6a1713903728/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_libvirt"
   description = "A Pulumi package for creating and managing libvirt cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "libvirt"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.4.6a1713561081"
+  version = "0.4.6a1713903728"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-libvirt"
 
 [build-system]
```

