# Comparing `tmp/my_functions_beatzaplenty-1.0.8.tar.gz` & `tmp/my_functions_beatzaplenty-1.0.9.tar.gz`

## Comparing `my_functions_beatzaplenty-1.0.8.tar` & `my_functions_beatzaplenty-1.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/__init__.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/.vscode/launch.json
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/.vscode/settings.json
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/.gitignore
--rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/__init__.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/check_command_exists.py
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/check_outgoing_ports.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/config.ini
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/create_config_file.py
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/create_ssh_connection.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/execute_ssh_command.py
--rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/install_required_modules.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/is_repo_up_to_date.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/parse_tuple.py
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/remote_update.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/requirements.txt
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/resize_linode_instance.py
--rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/run_command.py
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/run_updates.py
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/update-firewall.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/update_containers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/__init__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_check_command_exists.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_check_outgoing_ports.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_create_config_file.py
--rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_create_ssh_connection.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_execute_ssh_command.py
--rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_install_required_modules.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_is_repo_up_to_date.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_parse_tuple.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_remote_update.py
--rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_resize_linode_instance.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_run_command.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_run_updates.py
--rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/tests/test_update_containers.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/LICENSE
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/README.md
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/__init__.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/.vscode/launch.json
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/.gitignore
+-rw-r--r--   0        0        0     5051 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/__init__.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/check_command_exists.py
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/check_outgoing_ports.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/config.ini
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/create_config_file.py
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/create_ssh_connection.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/execute_ssh_command.py
+-rw-r--r--   0        0        0     1023 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/install_required_modules.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/is_repo_up_to_date.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/parse_tuple.py
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/remote_update.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/requirements.txt
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/resize_linode_instance.py
+-rw-r--r--   0        0        0     1245 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/run_command.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/run_updates.py
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/update-firewall.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/update_containers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/__init__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_check_command_exists.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_check_outgoing_ports.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_create_config_file.py
+-rw-r--r--   0        0        0     1563 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_create_ssh_connection.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_execute_ssh_command.py
+-rw-r--r--   0        0        0     2443 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_install_required_modules.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_is_repo_up_to_date.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_parse_tuple.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_remote_update.py
+-rw-r--r--   0        0        0     2761 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_resize_linode_instance.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_run_command.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_run_updates.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/tests/test_update_containers.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/LICENSE
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/README.md
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 my_functions_beatzaplenty-1.0.9/PKG-INFO
```

### Comparing `my_functions_beatzaplenty-1.0.8/.vscode/launch.json` & `my_functions_beatzaplenty-1.0.9/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/.gitignore` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/.gitignore`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/README.md` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/README.md`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/check_command_exists.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/check_command_exists.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/check_outgoing_ports.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/check_outgoing_ports.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/config.ini` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/config.ini`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/create_config_file.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/create_config_file.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/create_ssh_connection.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/create_ssh_connection.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/execute_ssh_command.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/execute_ssh_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/install_required_modules.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/install_required_modules.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/is_repo_up_to_date.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/is_repo_up_to_date.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/remote_update.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/remote_update.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/resize_linode_instance.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/resize_linode_instance.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/run_command.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/run_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/run_updates.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/run_updates.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/update-firewall.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/update-firewall.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
             add_cmd = f"sudo ufw {cmd_part_1} {current_ip} {cmd_part_2}"
             log_file.write("Last IP address: " + str(last_ip) + "\n")
             log_file.write("Current IP address: " + str(current_ip) + "\n")
             subprocess.run(del_cmd, shell = True, executable="/bin/bash",stdout=log_file)
             subprocess.run(add_cmd, shell = True, executable="/bin/bash",stdout=log_file)
             update_config(f'{parent_dir}/config.ini', current_ip, tzinfo)
         else:
-            log_file.write("IP address is correct. No firewall changes needed\n")
+            log_file.write(f"IP address {current_ip} is correct. No firewall changes needed\n")
         log_file.flush()
 
 def main():
     current_ip = get_current_ip()
     last_ip = get_last_ip()
 
     update_firewall_rules(current_ip, last_ip)
```

### Comparing `my_functions_beatzaplenty-1.0.8/src/my_functions_beatzaplenty/update_containers.py` & `my_functions_beatzaplenty-1.0.9/src/my_functions_beatzaplenty/update_containers.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_check_command_exists.py` & `my_functions_beatzaplenty-1.0.9/tests/test_check_command_exists.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_check_outgoing_ports.py` & `my_functions_beatzaplenty-1.0.9/tests/test_check_outgoing_ports.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_create_config_file.py` & `my_functions_beatzaplenty-1.0.9/tests/test_create_config_file.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_create_ssh_connection.py` & `my_functions_beatzaplenty-1.0.9/tests/test_create_ssh_connection.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_execute_ssh_command.py` & `my_functions_beatzaplenty-1.0.9/tests/test_execute_ssh_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_install_required_modules.py` & `my_functions_beatzaplenty-1.0.9/tests/test_install_required_modules.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_is_repo_up_to_date.py` & `my_functions_beatzaplenty-1.0.9/tests/test_is_repo_up_to_date.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_parse_tuple.py` & `my_functions_beatzaplenty-1.0.9/tests/test_parse_tuple.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_remote_update.py` & `my_functions_beatzaplenty-1.0.9/tests/test_remote_update.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_resize_linode_instance.py` & `my_functions_beatzaplenty-1.0.9/tests/test_resize_linode_instance.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_run_command.py` & `my_functions_beatzaplenty-1.0.9/tests/test_run_command.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_run_updates.py` & `my_functions_beatzaplenty-1.0.9/tests/test_run_updates.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/tests/test_update_containers.py` & `my_functions_beatzaplenty-1.0.9/tests/test_update_containers.py`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/.gitignore` & `my_functions_beatzaplenty-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/LICENSE` & `my_functions_beatzaplenty-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `my_functions_beatzaplenty-1.0.8/pyproject.toml` & `my_functions_beatzaplenty-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "my_functions_beatzaplenty"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Wayne Bennett", email="wayne.bennett@live.com" },
 ]
 description = "My Custom functions that I use all the time"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `my_functions_beatzaplenty-1.0.8/PKG-INFO` & `my_functions_beatzaplenty-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: my_functions_beatzaplenty
-Version: 1.0.8
+Version: 1.0.9
 Summary: My Custom functions that I use all the time
 Project-URL: Homepage, https://github.com/WayneBennett666/common
 Project-URL: Issues, https://github.com/WayneBennett666/common/issues
 Author-email: Wayne Bennett <wayne.bennett@live.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

