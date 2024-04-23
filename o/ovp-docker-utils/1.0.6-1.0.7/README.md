# Comparing `tmp/ovp_docker_utils-1.0.6.tar.gz` & `tmp/ovp_docker_utils-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovp_docker_utils-1.0.6.tar", last modified: Wed Apr 17 00:16:55 2024, max compression
+gzip compressed data, was "ovp_docker_utils-1.0.7.tar", last modified: Tue Apr 23 06:23:58 2024, max compression
```

## Comparing `ovp_docker_utils-1.0.6.tar` & `ovp_docker_utils-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.653143 ovp_docker_utils-1.0.6/
--rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.6/LICENSE
--rw-rw-rw-   0        0        0      380 2024-04-17 00:16:55.652145 ovp_docker_utils-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.613147 ovp_docker_utils-1.0.6/ovp_docker_utils/
--rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-15 20:43:27.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/__version__.py
--rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/defaults.py
--rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/docker_compose_instance.py
--rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/oem_logging.py
--rw-rw-rw-   0        0        0    33397 2024-04-17 00:10:52.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ovp_docker_utils.py
--rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_file_utils.py
--rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_key_gen.py
-drwxrwxrwx   0        0        0        0 2024-04-17 00:16:55.650143 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/
--rw-rw-rw-   0        0        0      380 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      553 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-17 00:16:55.000000 ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-17 00:16:55.653143 ovp_docker_utils-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.501605 ovp_docker_utils-1.0.7/
+-rw-rw-rw-   0        0        0    11527 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.7/LICENSE
+-rw-rw-rw-   0        0        0      380 2024-04-23 06:23:58.500604 ovp_docker_utils-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1409 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.471052 ovp_docker_utils-1.0.7/ovp_docker_utils/
+-rw-rw-rw-   0        0        0      354 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-23 03:55:20.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/__version__.py
+-rw-rw-rw-   0        0        0       27 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/defaults.py
+-rw-rw-rw-   0        0        0     2441 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/docker_compose_instance.py
+-rw-rw-rw-   0        0        0     5084 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/oem_logging.py
+-rw-rw-rw-   0        0        0    33907 2024-04-23 05:12:46.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ovp_docker_utils.py
+-rw-rw-rw-   0        0        0     6556 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_file_utils.py
+-rw-rw-rw-   0        0        0     3948 2024-04-03 15:53:12.000000 ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_key_gen.py
+drwxrwxrwx   0        0        0        0 2024-04-23 06:23:58.499605 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/
+-rw-rw-rw-   0        0        0      380 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      553 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-04-23 06:23:58.000000 ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2024-02-19 17:41:17.000000 ovp_docker_utils-1.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 06:23:58.501605 ovp_docker_utils-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      878 2024-04-01 23:55:26.000000 ovp_docker_utils-1.0.7/setup.py
```

### Comparing `ovp_docker_utils-1.0.6/LICENSE` & `ovp_docker_utils-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/README.md` & `ovp_docker_utils-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils/docker_compose_instance.py` & `ovp_docker_utils-1.0.7/ovp_docker_utils/docker_compose_instance.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils/oem_logging.py` & `ovp_docker_utils-1.0.7/ovp_docker_utils/oem_logging.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils/ovp_docker_utils.py` & `ovp_docker_utils-1.0.7/ovp_docker_utils/ovp_docker_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,14 +508,15 @@
     def get_logs(self, vpu_log_dir: str = "/home/oem/share/logs", local_log_cache: str = "~/ovp_logs/From_VPUs") -> None:
         get_logs(
             vpu_log_dir=vpu_log_dir,
             local_log_cache=local_log_cache,
             vpu_sn=self.vpu_sn,
             scp=self._scp,
             ssh=self._ssh,
+            vpu_name = self.vpu_name
         )
 
     def set_vpu_name(self, set_vpu_name: str) -> None:
         logger.info(f"Setting device name to {set_vpu_name}")
         self._o3r.set({"device": {"info": {"name": set_vpu_name}}})
 
     def mount_usb(self) -> list:
@@ -678,22 +679,25 @@
         logger.info(
             f">>> {_stderr.read().decode().strip()} {_stdout.read().decode().strip()}")
         if type(dst_dir) == str:
             dst_dir = Path(dst_dir).expanduser().absolute()
         logger.info(dst_dir/dst_name)
         self.transfer_from_vpu("/home/oem/"+fname, dst_dir/dst_name)
 
-    def initialize_container(self, service: DockerComposeServiceInstance, pipe_duration: float = 0, stop_upon_exit: bool = False, trigger_to_close_container: str = "") -> None:
+    def initialize_container(self, service: DockerComposeServiceInstance, pipe_duration: float = 0, stop_upon_exit: bool = False, autostart_enabled = True, trigger_to_close_container: str = "") -> None:
         initialized = False
 
         non_standard_docker_logger_used = service.log_driver is not None
 
         if non_standard_docker_logger_used or not pipe_duration:
             # detach from the container immediately
-            cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up --d --remove-orphan {service.service_name} "
+            if autostart_enabled:
+                cmd = f"cd /usr/share/oem/docker/compose/{service.service_name}/ && docker-compose up --d --remove-orphans {service.service_name}"
+            else:
+                cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up --d --remove-orphans {service.service_name}"
             _stdin, _stdout, _stderr = self._ssh.exec_command(cmd)
             logger.info(cmd)
             output_lines_from_container = _stdout.read().decode().strip().split("\n")
             logger.info(
                 f">>> {_stderr.read().decode().strip()} {' '.join(output_lines_from_container)}")
             logger.info(
                 f"{service.service_name} initialized from {service.docker_compose_dst_on_vpu}")
@@ -705,15 +709,19 @@
 
         if pipe_duration:
             if initialized:
                 cmd = f"docker attach {service.container_name}"
                 logger.info(
                     f"Now Attempting to show output from {service.container_name}: {cmd}")
             else:
-                cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up {service.service_name}"
+                if autostart_enabled:
+                    cmd = f"cd /usr/share/oem/docker/compose/{service.service_name}/ && docker-compose up --remove-orphans {service.service_name}"                
+                else:
+                    cmd = f"docker-compose -f {service.docker_compose_dst_on_vpu} up {service.service_name}"
+                
                 logger.info(
                     f"Initializing service and showing output of container as it appears to be using the standard logger... {cmd}")
 
             output_lines_from_container += self.attach_to_container(
                 cmd=cmd,
                 container_name=service.container_name,
                 pipe_duration=pipe_duration,
```

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_file_utils.py` & `ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_file_utils.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils/ssh_key_gen.py` & `ovp_docker_utils-1.0.7/ovp_docker_utils/ssh_key_gen.py`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/ovp_docker_utils.egg-info/SOURCES.txt` & `ovp_docker_utils-1.0.7/ovp_docker_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovp_docker_utils-1.0.6/setup.py` & `ovp_docker_utils-1.0.7/setup.py`

 * *Files identical despite different names*

