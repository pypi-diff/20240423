# Comparing `tmp/napalm_panos-0.6.0.tar.gz` & `tmp/napalm_panos-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_panos-0.6.0.tar", max compression
+gzip compressed data, was "napalm_panos-0.6.1.tar", max compression
```

## Comparing `napalm_panos-0.6.0.tar` & `napalm_panos-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1766 2022-02-13 21:03:20.784568 napalm_panos-0.6.0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2022-02-13 21:03:20.784568 napalm_panos-0.6.0/LICENSE
--rw-r--r--   0        0        0     4002 2022-02-13 21:03:20.784568 napalm_panos-0.6.0/README.md
--rw-r--r--   0        0        0      769 2022-02-13 21:03:20.784568 napalm_panos-0.6.0/napalm_panos/__init__.py
--rw-r--r--   0        0        0    31601 2022-02-13 21:03:20.788568 napalm_panos-0.6.0/napalm_panos/panos.py
--rw-r--r--   0        0        0        0 2022-02-13 21:03:20.788568 napalm_panos-0.6.0/napalm_panos/templates/.placeholder
--rw-r--r--   0        0        0       46 2022-02-13 21:03:20.788568 napalm_panos-0.6.0/napalm_panos/templates/set_hostname.j2
--rw-r--r--   0        0        0       28 2022-02-13 21:03:20.788568 napalm_panos-0.6.0/napalm_panos/utils/__init__.py
--rw-r--r--   0        0        0        0 2022-02-13 21:03:20.788568 napalm_panos-0.6.0/napalm_panos/utils/textfsm_templates/.placeholder
--rw-r--r--   0        0        0     2913 2022-02-13 21:03:30.468509 napalm_panos-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5047 2022-02-13 21:03:31.702437 napalm_panos-0.6.0/setup.py
--rw-r--r--   0        0        0     5242 2022-02-13 21:03:31.703479 napalm_panos-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/AUTHORS
+-rw-r--r--   0        0        0     1959 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4012 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/README.md
+-rw-r--r--   0        0        0      769 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/__init__.py
+-rw-r--r--   0        0        0    31634 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/panos.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/templates/.placeholder
+-rw-r--r--   0        0        0       46 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/templates/set_hostname.j2
+-rw-r--r--   0        0        0       28 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/utils/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 01:52:25.182351 napalm_panos-0.6.1/napalm_panos/utils/textfsm_templates/.placeholder
+-rw-r--r--   0        0        0     2834 2024-04-23 01:52:32.378396 napalm_panos-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5215 1970-01-01 00:00:00.000000 napalm_panos-0.6.1/PKG-INFO
```

### Comparing `napalm_panos-0.6.0/CHANGELOG.md` & `napalm_panos-0.6.1/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+# 0.6.1 - 2024-04
+
+### Added
+- #108 Added Support for sdwan interfaces
+- #105 Include interface description for get_interfaces method
+
+
+### Fixed
+- #115 Update package dependencies, fix tests
+
 # 0.6.0 - 2022-02
 
 ### Added
 - #102 Added Support for get_arp_table method
 - #99 Added documentation of supported getters
 - #93 Added ability to lock config optionally
 - #104 Added change log document
```

### Comparing `napalm_panos-0.6.0/LICENSE` & `napalm_panos-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_panos-0.6.0/README.md` & `napalm_panos-0.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,39 +7,40 @@
 
 This is community version of [NAPALM](https://napalm.readthedocs.io/) for the Palo Alto firewall operating system. For standard tutorials and overview of NAPALM, please review their documentation.
 
 # Configuration Support
 
 This table identifies the currently available configuration methods supported:
 
-| Getter                    | Supported |
+| Feature                   | Supported |
 | ------------------------- | --------- |
 | Config Replace            | ✅        |
 | Commit Confirm            | ❌        |
 | Config Merge              | ✅        |
 | Compare Config            | ✅        |
 | Atomic Changes            | ✅        |
 | Rollback                  | ✅        |
 
 > Commit Confirm is not supported by the vendor at the time of this writing.
 
 Configuration Lock is also supported, but the `optional_args` `config_lock` key set to `True`. You can see in this example.
 
-```
+```python
 from napalm import get_network_driver
 
-panos_device = device"
+panos_device = "nyc-sw01"
 panos_user = "admin"
 panos_password = "pass123"
 driver = get_network_driver("panos")
 optional_args = {"config_lock": True}
 
 with driver(panos_device, panos_user, panos_password, optional_args=optional_args) as device:
     device.load_replace_candidate(filename="2022-01-01-intended-config.xml")
     device.commit_config()
+
 ```
 
 As shown in the example above, the use of NAPALM's context manager is supported and recommended to use. 
 
 The locks are acquired and released using XML API. Locks for config and commit lock are obtained and released separately from each other. Both locks are
 released automatically by the device when a commit is made on the device.
```

### Comparing `napalm_panos-0.6.0/napalm_panos/__init__.py` & `napalm_panos-0.6.1/napalm_panos/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # the License.
 
 """napalm_panos package."""
 
 # Import local modules
 from napalm_panos.panos import PANOSDriver
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 __all__ = ("PANOSDriver",)
```

### Comparing `napalm_panos-0.6.0/napalm_panos/panos.py` & `napalm_panos-0.6.1/napalm_panos/panos.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Napalm-panos."""
+
 # pylint: disable=abstract-method,raise-missing-from
 # Copyright 2016 Dravetech AB. All rights reserved.
 #
 # The contents of this file are licensed under the Apache License, Version 2.0
 # (the "License"); you may not use this file except in compliance with the
 # License. You may obtain a copy of the License at
 #
@@ -215,14 +216,15 @@
         url = f"https://{self.hostname}/api/"
         request = requests.post(
             url,
             verify=self.verify,
             params=params,
             headers={"Content-Type": mef.content_type},
             data=mef,
+            timeout=5,
         )
         # if something goes wrong just raise an exception
         request.raise_for_status()
         response = xml.etree.ElementTree.fromstring(request.content)  # nosec
 
         if response.attrib["status"] == "error":
             LOGGER.error("Error found in response: %s", request.content)
@@ -261,28 +263,28 @@
         cmd = f"<load><config><from>{path}</from></config></load>"
         self.device.op(cmd=cmd)
 
         if self.device.status != "success":
             raise ReplaceConfigException(f"Error while loading config from {path}")
         self.loaded = True
 
-    def _get_file_content(self, filename):  # pylint: disable=no-self-use
+    def _get_file_content(self, filename):
         """Convenience method to get file content."""
         try:
             with open(filename, "r", encoding="utf-8") as file:
                 content = file.read()
         except IOError:
             raise MergeConfigException(f"Error while opening {filename}. Make sure " "filename is correct.")
         return content
 
     def _send_merge_commands(self, config, file_config):
         """Netmiko is being used to push set commands."""
         if self.loaded is False:
             if self._save_backup() is False:
-                raise MergeConfigException("Error while storing backup " "config.")
+                raise MergeConfigException("Error while storing backup config.")
         if self.ssh_connection is False:
             self._open_ssh()
 
         if isinstance(config, str):
             if file_config:
                 config = config.splitlines()
             else:
@@ -339,15 +341,15 @@
             self._send_merge_commands(config, file_config)
 
         elif config:
             file_config = False
             self._send_merge_commands(config, file_config)
 
         else:
-            raise MergeConfigException("You must provide either a file " "or a set-format string")
+            raise MergeConfigException("You must provide either a file or a set-format string")
 
     def compare_config(self):
         """Netmiko is being used to obtain config diffs because pan-python doesn't support the needed command."""
         if self.ssh_connection is False:
             self._open_ssh()
 
         self.ssh_device.exit_config_mode()
@@ -410,15 +412,15 @@
                 self._open_ssh()
             try:
                 self.ssh_device.commit()
                 self.loaded = False
                 self.changed = False
                 self.merge_config = False
             except Exception:  # noqa pylint: disable=broad-except
-                ReplaceConfigException("Error while loading backup config")
+                raise ReplaceConfigException("Error while loading backup config")
 
     def _extract_interface_list(self):
         self.device.op(cmd="<show><interface>all</interface></show>")
         interfaces_xml = xmltodict.parse(self.device.xml_root())
         interfaces_json = json.dumps(interfaces_xml["response"]["result"])
         interfaces = json.loads(interfaces_json)
 
@@ -479,15 +481,15 @@
             system_info = json.loads(system_info_json)
         except AttributeError:
             system_info = {}
 
         if system_info:
             facts["hostname"] = system_info["hostname"]
             facts["vendor"] = "Palo Alto Networks"
-            facts["uptime"] = int(convert_uptime_string_seconds(system_info["uptime"]))
+            facts["uptime"] = float(convert_uptime_string_seconds(system_info["uptime"]))
             facts["os_version"] = system_info["sw-version"]
             facts["serial_number"] = system_info["serial"]
             facts["model"] = system_info["model"]
             facts["fqdn"] = "N/A"
             facts["interface_list"] = self._extract_interface_list()
 
             facts["interface_list"].sort()
@@ -614,21 +616,23 @@
         return routes
 
     def get_interfaces(self):  # pylint: disable=too-many-locals
         """PANOS version of `get_interfaces` method, see NAPALM for documentation."""
         subif_defaults = {
             "is_up": True,
             "is_enabled": True,
-            "speed": 0,
+            "speed": 0.0,
             "last_flapped": -1.0,
             "mac_address": "",
             "mtu": 0,
             "description": "",
         }
-        interface_pattern = re.compile(r"(ethernet\d+/\d+\.\d+)|(ae\d+\.\d+)|(loopback\.)|(tunnel\.)|(vlan\.)")
+        interface_pattern = re.compile(
+            r"(ethernet\d+/\d+\.\d+)|(ae\d+\.\d+)|(loopback\.)|(tunnel\.)|(vlan\.)|(sdwan\.)"
+        )
         interface_dict = {}
         interface_descr = {}
         interface_list = self._extract_interface_list()
 
         config = xml.etree.ElementTree.fromstring(self.get_config()["running"])  # nosec
         for eth_int in config.findall(".//ethernet/entry"):
             name = eth_int.attrib["name"]
@@ -672,21 +676,21 @@
                 raise RuntimeError(msg)
 
             interface["last_flapped"] = -1.0
             interface["mtu"] = 0
             interface["speed"] = interface_info.get("speed")
             # Loopback and down interfaces
             if interface["speed"] in ("[n/a]", "unknown"):
-                interface["speed"] = 0
+                interface["speed"] = 0.0
             else:
                 try:
-                    interface["speed"] = int(interface["speed"])
+                    interface["speed"] = float(interface["speed"])
                 except ValueError:
-                    # Handle when unable to convert a string to an integer, set it to 0 similar to the unknown state.
-                    interface["speed"] = 0
+                    # Handle when unable to convert a string to an float, set it to 0 similar to the unknown state.
+                    interface["speed"] = 0.0
             interface["mac_address"] = standardize_mac(interface_info.get("mac"))
             interface["description"] = interface_descr.get(intf, "")
             interface_dict[intf] = interface
 
         return interface_dict
 
     def get_interfaces_ip(self):
```

### Comparing `napalm_panos-0.6.0/pyproject.toml` & `napalm_panos-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 [tool.poetry]
 name = "napalm_panos"
-version = "v0.6.0"
+version = "v0.6.1"
 description = "Network Automation and Programmability Abstraction Layer with Multivendor support for PANOS."
 authors = ["Gabriele Gerbino <gabriele@networktocode.com>"]
 license = "Apache-2.0"
 homepage = "https://github.com/napalm-automation/napalm-panos"
 repository = "https://github.com/napalm-automation/napalm-panos"
 documentation = "https://github.com/napalm-automation/napalm-panos"
 readme = "README.md"
 keywords = ["napalm", "panos", "napalm-panos"]
 classifiers = [
     "Intended Audience :: Developers",
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 include = [
     "CHANGELOG.md",
     "LICENSE",
     "README.md",
     "napalm_panos/templates/*.j2",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = ">=3.8,<3.12"
 cryptography = "3.3.2"
-napalm = "^3.0"
-lxml = "4.6.5"
+napalm = "^4.0.0"
+lxml = "^5.0.0"
 pan-python = "*"
-netmiko = "^3.3.2"
+netmiko = "^4.0.0"
 requests-toolbelt = "*"
 xmltodict = "*"
 
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 bandit = "*"
-black = {version="^21.10b0", python="^3.6.2"}
 coverage = "*"
 invoke = "*"
 flake8 = "*"
-pylint = {version="2.12.2", python="^3.6.2"}
+pylint = "*"
 pytest = "*"
 pyyaml = "*"
 pydocstyle = "*"
 m2r2 = "*"
 sphinx = "*"
 sphinx-rtd-theme = "*"
 toml = "*"
 yamllint = "*"
 coveralls = "*"
 pytest-cov = "*"
 pytest-json = "*"
 pytest-pythonpath = "*"
 pylama = "*"
 flake8-import-order = "*"
+black = "*"
+
 
 [tool.black]
 line-length = 120
-target-version = ['py37']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 (
   /(
       \.eggs         # exclude a few common directories in the
     | \.git          # root of the project
     | \.hg
@@ -88,26 +88,26 @@
 good-names="i,ip,j,k,ex,Run,_"
 
 [tool.pylint.messages_control]
 # Line length is enforced by Black, so pylint doesn't need to check it.
 # Pylint and Black disagree about how to format multi-line arrays; Black wins.
 disable = """,
     line-too-long,
-    bad-continuation,
     consider-iterating-dictionary,
     too-many-statements,
     """
 
 [tool.pylint.miscellaneous]
 # Don't flag TODO as a failure, let us commit with things that still need to be done in the code
 notes = """,
     FIXME,
     XXX,
     """
 
 [tool.pytest.ini_options]
-python_paths = "./"
+pythonpaths = "./"
 testpaths = "tests/"
 addopts = "-vv --doctest-modules -p no:warnings --ignore-glob='*mock*'"
+
 [build-system]
-requires = ["poetry>=0.12"]
-build-backend = "poetry.masonry.api"
+requires = ["poetry_core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `napalm_panos-0.6.0/setup.py` & `napalm_panos-0.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,117 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: napalm_panos
+Version: 0.6.1
+Summary: Network Automation and Programmability Abstraction Layer with Multivendor support for PANOS.
+Home-page: https://github.com/napalm-automation/napalm-panos
+License: Apache-2.0
+Keywords: napalm,panos,napalm-panos
+Author: Gabriele Gerbino
+Author-email: gabriele@networktocode.com
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cryptography (==3.3.2)
+Requires-Dist: lxml (>=5.0.0,<6.0.0)
+Requires-Dist: napalm (>=4.0.0,<5.0.0)
+Requires-Dist: netmiko (>=4.0.0,<5.0.0)
+Requires-Dist: pan-python
+Requires-Dist: requests-toolbelt
+Requires-Dist: xmltodict
+Project-URL: Documentation, https://github.com/napalm-automation/napalm-panos
+Project-URL: Repository, https://github.com/napalm-automation/napalm-panos
+Description-Content-Type: text/markdown
+
+[![PyPI](https://img.shields.io/pypi/v/napalm-panos.svg)](https://pypi.python.org/pypi/napalm-panos)
+[![PyPI](https://img.shields.io/pypi/dm/napalm-panos.svg)](https://pypi.python.org/pypi/napalm-panos)
+[![Build Status](https://travis-ci.org/napalm-automation/napalm-panos.svg?branch=master)](https://travis-ci.org/napalm-automation/napalm-panos)
+[![Coverage Status](https://coveralls.io/repos/github/napalm-automation/napalm-panos/badge.svg?branch=develop)](https://coveralls.io/github/napalm-automation/napalm-panos?branch=develop)
+
+# NAPALM PANOS
+
+This is community version of [NAPALM](https://napalm.readthedocs.io/) for the Palo Alto firewall operating system. For standard tutorials and overview of NAPALM, please review their documentation.
+
+# Configuration Support
+
+This table identifies the currently available configuration methods supported:
+
+| Feature                   | Supported |
+| ------------------------- | --------- |
+| Config Replace            | ✅        |
+| Commit Confirm            | ❌        |
+| Config Merge              | ✅        |
+| Compare Config            | ✅        |
+| Atomic Changes            | ✅        |
+| Rollback                  | ✅        |
+
+> Commit Confirm is not supported by the vendor at the time of this writing.
+
+Configuration Lock is also supported, but the `optional_args` `config_lock` key set to `True`. You can see in this example.
+
+```python
+from napalm import get_network_driver
+
+panos_device = "nyc-sw01"
+panos_user = "admin"
+panos_password = "pass123"
+driver = get_network_driver("panos")
+optional_args = {"config_lock": True}
+
+with driver(panos_device, panos_user, panos_password, optional_args=optional_args) as device:
+    device.load_replace_candidate(filename="2022-01-01-intended-config.xml")
+    device.commit_config()
+
+```
+
+As shown in the example above, the use of NAPALM's context manager is supported and recommended to use. 
+
+The locks are acquired and released using XML API. Locks for config and commit lock are obtained and released separately from each other. Both locks are
+released automatically by the device when a commit is made on the device.
+
+For troubleshooting:
+- The code crashed in a way that the lock could not be removed?
+    - Remove the lock manually (CLI, API, Web UI). The lock can only be removed by the administrator who set it, or by a superuser.
+- The lock disappeared in the middle of program execution?
+    - Did someone do a commit on the device? The locks are removed automatically when the administrator who set the locks performs a commit operation on the device.
+
+# Supported Getters
+
+This table identifies the currently available getters and the support for each:
+
+| Getter                    | Supported |
+| ------------------------- | --------- |
+| get_arp_table             | ✅        |
+| get_bgp_config            | ❌        |
+| get_bgp_neighbors         | ❌        |
+| get_bgp_neighbors_detail  | ❌        |
+| get_config                | ✅        |
+| get_environment           | ❌        |
+| get_facts                 | ✅        |
+| get_firewall_policies     | ❌        |
+| get_interfaces            | ✅        |
+| get_interfaces_counters   | ❌        |
+| get_interfaces_ip         | ✅        |
+| get_ipv6_neighbors_table  | ❌        |
+| get_lldp_neighbors        | ✅        |
+| get_lldp_neighbors_detail | ❌        |
+| get_mac_address_table     | ❌        |
+| get_network_instances     | ❌        |
+| get_ntp_peers             | ❌        |
+| get_ntp_servers           | ❌        |
+| get_ntp_stats             | ❌        |
+| get_optics                | ❌        |
+| get_probes_config         | ❌        |
+| get_probes_results        | ❌        |
+| get_route_to              | ✅        |
+| get_snmp_information      | ❌        |
+| get_users                 | ❌        |
+| get_vlans                 | ❌        |
+| is_alive                  | ✅        |
+| ping                      | ❌        |
+| traceroute                | ❌        |
 
-packages = \
-['napalm_panos', 'napalm_panos.utils']
-
-package_data = \
-{'': ['*'],
- 'napalm_panos': ['templates/*'],
- 'napalm_panos.utils': ['textfsm_templates/*']}
-
-install_requires = \
-['cryptography==3.3.2',
- 'lxml==4.6.5',
- 'napalm>=3.0,<4.0',
- 'netmiko>=3.3.2,<4.0.0',
- 'pan-python',
- 'requests-toolbelt',
- 'xmltodict']
-
-setup_kwargs = {
-    'name': 'napalm-panos',
-    'version': '0.6.0',
-    'description': 'Network Automation and Programmability Abstraction Layer with Multivendor support for PANOS.',
-    'long_description': '[![PyPI](https://img.shields.io/pypi/v/napalm-panos.svg)](https://pypi.python.org/pypi/napalm-panos)\n[![PyPI](https://img.shields.io/pypi/dm/napalm-panos.svg)](https://pypi.python.org/pypi/napalm-panos)\n[![Build Status](https://travis-ci.org/napalm-automation/napalm-panos.svg?branch=master)](https://travis-ci.org/napalm-automation/napalm-panos)\n[![Coverage Status](https://coveralls.io/repos/github/napalm-automation/napalm-panos/badge.svg?branch=develop)](https://coveralls.io/github/napalm-automation/napalm-panos?branch=develop)\n\n# NAPALM PANOS\n\nThis is community version of [NAPALM](https://napalm.readthedocs.io/) for the Palo Alto firewall operating system. For standard tutorials and overview of NAPALM, please review their documentation.\n\n# Configuration Support\n\nThis table identifies the currently available configuration methods supported:\n\n| Getter                    | Supported |\n| ------------------------- | --------- |\n| Config Replace            | ✅        |\n| Commit Confirm            | ❌        |\n| Config Merge              | ✅        |\n| Compare Config            | ✅        |\n| Atomic Changes            | ✅        |\n| Rollback                  | ✅        |\n\n> Commit Confirm is not supported by the vendor at the time of this writing.\n\nConfiguration Lock is also supported, but the `optional_args` `config_lock` key set to `True`. You can see in this example.\n\n```\nfrom napalm import get_network_driver\n\npanos_device = device"\npanos_user = "admin"\npanos_password = "pass123"\ndriver = get_network_driver("panos")\noptional_args = {"config_lock": True}\n\nwith driver(panos_device, panos_user, panos_password, optional_args=optional_args) as device:\n    device.load_replace_candidate(filename="2022-01-01-intended-config.xml")\n    device.commit_config()\n```\n\nAs shown in the example above, the use of NAPALM\'s context manager is supported and recommended to use. \n\nThe locks are acquired and released using XML API. Locks for config and commit lock are obtained and released separately from each other. Both locks are\nreleased automatically by the device when a commit is made on the device.\n\nFor troubleshooting:\n- The code crashed in a way that the lock could not be removed?\n    - Remove the lock manually (CLI, API, Web UI). The lock can only be removed by the administrator who set it, or by a superuser.\n- The lock disappeared in the middle of program execution?\n    - Did someone do a commit on the device? The locks are removed automatically when the administrator who set the locks performs a commit operation on the device.\n\n# Supported Getters\n\nThis table identifies the currently available getters and the support for each:\n\n| Getter                    | Supported |\n| ------------------------- | --------- |\n| get_arp_table             | ✅        |\n| get_bgp_config            | ❌        |\n| get_bgp_neighbors         | ❌        |\n| get_bgp_neighbors_detail  | ❌        |\n| get_config                | ✅        |\n| get_environment           | ❌        |\n| get_facts                 | ✅        |\n| get_firewall_policies     | ❌        |\n| get_interfaces            | ✅        |\n| get_interfaces_counters   | ❌        |\n| get_interfaces_ip         | ✅        |\n| get_ipv6_neighbors_table  | ❌        |\n| get_lldp_neighbors        | ✅        |\n| get_lldp_neighbors_detail | ❌        |\n| get_mac_address_table     | ❌        |\n| get_network_instances     | ❌        |\n| get_ntp_peers             | ❌        |\n| get_ntp_servers           | ❌        |\n| get_ntp_stats             | ❌        |\n| get_optics                | ❌        |\n| get_probes_config         | ❌        |\n| get_probes_results        | ❌        |\n| get_route_to              | ✅        |\n| get_snmp_information      | ❌        |\n| get_users                 | ❌        |\n| get_vlans                 | ❌        |\n| is_alive                  | ✅        |\n| ping                      | ❌        |\n| traceroute                | ❌        |\n',
-    'author': 'Gabriele Gerbino',
-    'author_email': 'gabriele@networktocode.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/napalm-automation/napalm-panos',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.6,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

