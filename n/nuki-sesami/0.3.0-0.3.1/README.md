# Comparing `tmp/nuki_sesami-0.3.0.tar.gz` & `tmp/nuki_sesami-0.3.1.tar.gz`

## Comparing `nuki_sesami-0.3.0.tar` & `nuki_sesami-0.3.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/build.sh
--rw-r--r--   0        0        0    64862 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/nuki-raspi-door-erreka.png
--rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/publish.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/src/nuki_sesami/__init__.py
--rw-r--r--   0        0        0    13077 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/src/nuki_sesami/door_controller.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/src/nuki_sesami/door_state.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/src/nuki_sesami/sesami_systemd.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/LICENSE
--rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 nuki_sesami-0.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0       75 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/build.sh
+-rw-r--r--   0        0        0    64862 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/nuki-raspi-door-erreka.png
+-rwxr-xr-x   0        0        0      107 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/publish.sh
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/src/nuki_sesami/__init__.py
+-rw-r--r--   0        0        0    13729 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/src/nuki_sesami/door_controller.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/src/nuki_sesami/door_state.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/src/nuki_sesami/sesami_systemd.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3584 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 nuki_sesami-0.3.1/PKG-INFO
```

### Comparing `nuki_sesami-0.3.0/nuki-raspi-door-erreka.png` & `nuki_sesami-0.3.1/nuki-raspi-door-erreka.png`

 * *Files identical despite different names*

### Comparing `nuki_sesami-0.3.0/src/nuki_sesami/door_controller.py` & `nuki_sesami-0.3.1/src/nuki_sesami/door_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -230,27 +230,43 @@
         elif self.state == DoorState.openclose2:
             self.open()
         elif self.state == DoorState.openhold:
             pass # no action here
 
 
 def getlogger(name: str, path: str, level: int = logging.INFO) -> Logger:
+    '''Returns a logger instance for the given name and path.
+    
+    The logger for will rotating log files with a maximum size of 1MB and 
+    a maximum of 10 log files.
+
+    Parameters:
+    * name: name of the logger, e.g. 'nuki-sesami'
+    * path: complete path for storing the log files, e.g. '/var/log/nuki-sesami'
+    * level: logging level, e.g; logging.DEBUG
+
+    '''
     logger = logging.getLogger(name)
     logger.setLevel(level)
     handler = logging.StreamHandler(sys.stdout)
     handler.setLevel(level)
     handler.setFormatter(logging.Formatter('[%(levelname)s] %(message)s'))
     logger.addHandler(handler)
     handler = RotatingFileHandler(f'{os.path.join(path,name)}.log', maxBytes=1048576, backupCount=10)
     handler.setLevel(level)
     handler.setFormatter(logging.Formatter('%(asctime)s [%(levelname)s] %(message)s'))
     logger.addHandler(handler)
     return logger
 
 
+def is_virtual_env():
+    '''Returns true when running in a virtual environment.'''
+    return sys.prefix != sys.base_prefix
+
+
 def main():
     parser = argparse.ArgumentParser(
         prog='nuki-sesami',
         description='Open and close an electric door equipped with a Nuki 3.0 pro smart lock',
         epilog='Belrog: you shall not pass!',
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
@@ -264,16 +280,21 @@
     parser.add_argument('-3', '--openhold_mode', help="door open and hold mode relay (gpio)pin", default=20, type=int)
     parser.add_argument('-4', '--openclose_mode', help="door open/close mode relay (gpio)pin", default=21, type=int)
     parser.add_argument('-B', '--buttonlogic', help="pushbutton logic when pressed; 0=openhold,1=open,2=toggle", default=0, type=int)
     parser.add_argument('-V', '--verbose', help="be verbose", action='store_true')
 
     args = parser.parse_args()
 
-    logpath = '/var/log/nuki-sesami'
+    if is_virtual_env():    
+        logpath = os.path.join(sys.prefix, 'var/log/nuki-sesami')
+    else:
+        logpath = '/var/log/nuki-sesami'
+
     if not os.path.exists(logpath):
+        print(f"mkdir -p {logpath}")
         os.makedirs(logpath)
 
     logger = getlogger('nuki-sesami', logpath, level=logging.DEBUG if args.verbose else logging.INFO)
     logger.debug(f"args.device={args.device}")
     logger.debug(f"args.host={args.host}")
     logger.debug(f"args.port={args.port}")
     logger.debug(f"args.username={args.username}")
```

### Comparing `nuki_sesami-0.3.0/src/nuki_sesami/door_state.py` & `nuki_sesami-0.3.1/src/nuki_sesami/door_state.py`

 * *Files identical despite different names*

### Comparing `nuki_sesami-0.3.0/src/nuki_sesami/sesami_systemd.py` & `nuki_sesami-0.3.1/src/nuki_sesami/sesami_systemd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #!/bin/env python3
 
+import os
 import sys
 import argparse
 import subprocess
 import shutil
 
 
 SYSTEMD_TEMPLATE = f'''[Unit]
@@ -11,43 +12,47 @@
 After=network.target
 Wants=Network.target
 
 [Service]
 Type=simple
 Restart=always
 RestartSec=1
-Environment=PYTHONPATH=%s:$PYTHONPATH
+Environment=%s
 ExecStart=%s %s -H %s -U %s -P %s
 StandardError=journal
 StandardOutput=journal
 StandardInput=null
 
 [Install]
 WantedBy=multi-user.target
 '''
 
 
 def nuki_sesami_systemd(device: str, host: str, username: str, password: str, remove: bool = False)  -> None:
+    systemd_fname = f'/lib/systemd/system/nuki-sesami.service'
+
     if remove:
         subprocess.run(["systemctl", "stop", "nuki-sesami"])
         subprocess.run(["systemctl", "disable", "nuki-sesami"])
-        subprocess.run(["rm", "-vrf", "/lib/systemd/system/nuki-sesami.service"])
+        subprocess.run(["rm", "-vrf", systemd_fname])
         return
 
     bin = shutil.which('nuki-sesami')
     if not bin:
         print(f"Failed to detect 'nuki-sesami' binary")
         sys.exit(1)
 
-    pythonpath = [x for x in sys.path if x.startswith('/home/')][0]
-
-    fname = f'/lib/systemd/system/nuki-sesami.service'
-    with open(fname, 'w+') as f:
-        f.write(SYSTEMD_TEMPLATE % (pythonpath, bin, device, host, username, password))
-        print(f"Created systemd file; '{fname}'")
+    try:
+        env = 'PYTHONPATH=%s:$PYTHONPATH' % [x for x in sys.path if x.startswith('/home/')][0]
+    except:
+        env = ''
+
+    with open(systemd_fname, 'w+') as f:
+        f.write(SYSTEMD_TEMPLATE % (env, bin, device, host, username, password))
+        print(f"Created systemd file; '{systemd_fname}'")
 
     try:
         subprocess.run(["systemctl", "daemon-reload"], check=True)
         subprocess.run(["systemctl", "enable", "nuki-sesami"], check=True)
         subprocess.run(["systemctl", "start", "nuki-sesami"], check=True)
     except subprocess.CalledProcessError as e:
         print(f"Something went wrong: {e}")
@@ -74,14 +79,18 @@
     if args.verbose:
         print(f"device      : {args.device}")
         print(f"host        : {args.host}")
         print(f"username    : {args.username}")
         print(f"password    : ***")
         print(f"remove      : {args.remove}")
 
+    if 'VIRTUAL_ENV' in os.environ:
+        print("Virtual environment detected, systemd is not supported")
+        sys.exit(1)
+
     try:
         nuki_sesami_systemd(args.device, args.host, args.username, args.password, args.remove)
     except KeyboardInterrupt:
         print("Program terminated")
     except Exception as e:
         print(f"Something went wrong: {e}")
```

### Comparing `nuki_sesami-0.3.0/.gitignore` & `nuki_sesami-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nuki_sesami-0.3.0/LICENSE` & `nuki_sesami-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nuki_sesami-0.3.0/README.md` & `nuki_sesami-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nuki_sesami-0.3.0/pyproject.toml` & `nuki_sesami-0.3.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "nuki-sesami"
-version = "0.3.0"
+version = "0.3.1"
 authors = [
     { name = "Michel Mooij", email = "michel.mooij7@gmail.com" }
 ]
 description = "Open an electric door using Nuki smartlock status"
 readme = "README.md"
 dependencies = [
     "paho-mqtt>=1.6.1",
```

### Comparing `nuki_sesami-0.3.0/PKG-INFO` & `nuki_sesami-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: nuki-sesami
-Version: 0.3.0
+Version: 0.3.1
 Summary: Open an electric door using Nuki smartlock status
 Project-URL: Homepage, https://github.com/michelm/nuki-sesami
 Author-email: Michel Mooij <michel.mooij7@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

