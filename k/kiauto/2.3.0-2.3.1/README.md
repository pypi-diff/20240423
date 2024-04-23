# Comparing `tmp/kiauto-2.3.0.tar.gz` & `tmp/kiauto-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiauto-2.3.0.tar", last modified: Thu Mar 21 10:18:11 2024, max compression
+gzip compressed data, was "kiauto-2.3.1.tar", last modified: Tue Apr 23 11:15:06 2024, max compression
```

## Comparing `kiauto-2.3.0.tar` & `kiauto-2.3.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.376182 kiauto-2.3.0/
--rw-rw-r--   0 root         (0) root         (0)    11358 2024-03-21 10:16:45.000000 kiauto-2.3.0/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       67 2024-03-21 10:16:45.000000 kiauto-2.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    17079 2024-03-21 10:18:11.376182 kiauto-2.3.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)    13874 2024-03-21 10:16:45.000000 kiauto-2.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.372182 kiauto-2.3.0/kiauto/
--rw-rw-r--   0 root         (0) root         (0)        0 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    15558 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/file_util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.372182 kiauto-2.3.0/kiauto/interposer/
--rwxrwxr-x   0 root         (0) root         (0)    27512 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/interposer/libinterposer.so
--rw-rw-r--   0 root         (0) root         (0)    30265 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/interposer.py
--rw-rw-r--   0 root         (0) root         (0)     3755 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/log.py
--rw-rw-r--   0 root         (0) root         (0)    14466 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/misc.py
--rw-rw-r--   0 root         (0) root         (0)    19007 2024-03-21 10:16:45.000000 kiauto-2.3.0/kiauto/ui_automation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.372182 kiauto-2.3.0/kiauto.egg-info/
--rw-r--r--   0 root         (0) root         (0)    17079 2024-03-21 10:18:11.000000 kiauto-2.3.0/kiauto.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      786 2024-03-21 10:18:11.000000 kiauto-2.3.0/kiauto.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-21 10:18:11.000000 kiauto-2.3.0/kiauto.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       19 2024-03-21 10:18:11.000000 kiauto-2.3.0/kiauto.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-03-21 10:18:11.000000 kiauto-2.3.0/kiauto.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-21 10:18:11.376182 kiauto-2.3.0/setup.cfg
--rwxrwxr-x   0 root         (0) root         (0)     1430 2024-03-21 10:16:45.000000 kiauto-2.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.372182 kiauto-2.3.0/src/
--rwxrwxr-x   0 root         (0) root         (0)    47614 2024-03-21 10:16:45.000000 kiauto-2.3.0/src/eeschema_do
--rwxrwxr-x   0 root         (0) root         (0)     7074 2024-03-21 10:16:45.000000 kiauto-2.3.0/src/kicad2step_do
--rwxrwxr-x   0 root         (0) root         (0)    80765 2024-03-21 10:16:45.000000 kiauto-2.3.0/src/pcbnew_do
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.372182 kiauto-2.3.0/tests/
--rw-rw-r--   0 root         (0) root         (0)      390 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.376182 kiauto-2.3.0/tests/eeschema/
--rw-rw-r--   0 root         (0) root         (0)      947 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/eeschema/test_bom_xml.py
--rw-rw-r--   0 root         (0) root         (0)     6310 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/eeschema/test_erc.py
--rw-rw-r--   0 root         (0) root         (0)     5308 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/eeschema/test_export.py
--rw-rw-r--   0 root         (0) root         (0)     1501 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/eeschema/test_netlist.py
--rw-rw-r--   0 root         (0) root         (0)     5291 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/eeschema/test_sch_misc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.376182 kiauto-2.3.0/tests/kicad2step/
--rw-rw-r--   0 root         (0) root         (0)     1120 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/kicad2step/test_step.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.376182 kiauto-2.3.0/tests/pcbnew/
--rw-rw-r--   0 root         (0) root         (0)     1557 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_3d.py
--rw-rw-r--   0 root         (0) root         (0)     4988 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_drc.py
--rw-rw-r--   0 root         (0) root         (0)     1141 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_export_gencad.py
--rw-rw-r--   0 root         (0) root         (0)     1974 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_export_vrml.py
--rw-rw-r--   0 root         (0) root         (0)     3917 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_pcb_misc.py
--rw-rw-r--   0 root         (0) root         (0)     7080 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/pcbnew/test_print_layers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 10:18:11.376182 kiauto-2.3.0/tests/utils/
--rw-rw-r--   0 root         (0) root         (0)    15980 2024-03-21 10:16:45.000000 kiauto-2.3.0/tests/utils/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/
+-rw-rw-r--   0 root         (0) root         (0)    11358 2024-04-23 11:05:55.000000 kiauto-2.3.1/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       67 2024-04-23 11:05:55.000000 kiauto-2.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    17079 2024-04-23 11:15:06.487620 kiauto-2.3.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)    13874 2024-04-23 11:05:55.000000 kiauto-2.3.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.483621 kiauto-2.3.1/kiauto/
+-rw-rw-r--   0 root         (0) root         (0)        0 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    15566 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.483621 kiauto-2.3.1/kiauto/interposer/
+-rwxrwxr-x   0 root         (0) root         (0)    27512 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/interposer/libinterposer.so
+-rw-rw-r--   0 root         (0) root         (0)    30265 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/interposer.py
+-rw-rw-r--   0 root         (0) root         (0)     3755 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/log.py
+-rw-rw-r--   0 root         (0) root         (0)    14736 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/misc.py
+-rw-rw-r--   0 root         (0) root         (0)    19007 2024-04-23 11:05:55.000000 kiauto-2.3.1/kiauto/ui_automation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.483621 kiauto-2.3.1/kiauto.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    17079 2024-04-23 11:15:06.000000 kiauto-2.3.1/kiauto.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      786 2024-04-23 11:15:06.000000 kiauto-2.3.1/kiauto.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 11:15:06.000000 kiauto-2.3.1/kiauto.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2024-04-23 11:15:06.000000 kiauto-2.3.1/kiauto.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-04-23 11:15:06.000000 kiauto-2.3.1/kiauto.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 11:15:06.487620 kiauto-2.3.1/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     1430 2024-04-23 11:05:55.000000 kiauto-2.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/src/
+-rwxrwxr-x   0 root         (0) root         (0)    47677 2024-04-23 11:05:55.000000 kiauto-2.3.1/src/eeschema_do
+-rwxrwxr-x   0 root         (0) root         (0)     7074 2024-04-23 11:05:55.000000 kiauto-2.3.1/src/kicad2step_do
+-rwxrwxr-x   0 root         (0) root         (0)    83490 2024-04-23 11:05:55.000000 kiauto-2.3.1/src/pcbnew_do
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)      390 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/tests/eeschema/
+-rw-rw-r--   0 root         (0) root         (0)      947 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/eeschema/test_bom_xml.py
+-rw-rw-r--   0 root         (0) root         (0)     6310 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/eeschema/test_erc.py
+-rw-rw-r--   0 root         (0) root         (0)     5308 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/eeschema/test_export.py
+-rw-rw-r--   0 root         (0) root         (0)     1501 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/eeschema/test_netlist.py
+-rw-rw-r--   0 root         (0) root         (0)     5411 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/eeschema/test_sch_misc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/tests/kicad2step/
+-rw-rw-r--   0 root         (0) root         (0)     1120 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/kicad2step/test_step.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/tests/pcbnew/
+-rw-rw-r--   0 root         (0) root         (0)     2861 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_3d.py
+-rw-rw-r--   0 root         (0) root         (0)     4988 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_drc.py
+-rw-rw-r--   0 root         (0) root         (0)     1141 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_export_gencad.py
+-rw-rw-r--   0 root         (0) root         (0)     1974 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_export_vrml.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_pcb_misc.py
+-rw-rw-r--   0 root         (0) root         (0)     7080 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/pcbnew/test_print_layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 11:15:06.487620 kiauto-2.3.1/tests/utils/
+-rw-rw-r--   0 root         (0) root         (0)    15980 2024-04-23 11:05:55.000000 kiauto-2.3.1/tests/utils/context.py
```

### Comparing `kiauto-2.3.0/LICENSE` & `kiauto-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/PKG-INFO` & `kiauto-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.3.0
+Version: 2.3.1
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.3.0/README.md` & `kiauto-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/kiauto/file_util.py` & `kiauto-2.3.1/kiauto/file_util.py`

 * *Files identical despite different names*

```diff
@@ -243,15 +243,15 @@
     with open(cfg.conf_kicad, "wt") as text_file:
         if cfg.conf_kicad_json:
             kiconf = {"environment": {"show_warning_dialog": False}}
             kiconf['graphics'] = {"cairo_antialiasing_mode": 0, "opengl_antialiasing_mode": 0}
             kiconf['system'] = {"editor_name": "/bin/cat"}
             # Copy the environment vars if available
             if cfg.conf_kicad_bkp:
-                vars = Config.get_config_vars_json(cfg.conf_kicad_bkp)
+                vars = Config.get_config_vars_json(cfg.conf_kicad_bkp, logger)
                 if vars:
                     kiconf['environment']['vars'] = vars
             text_file.write(json.dumps(kiconf))
             logger.debug(json.dumps(kiconf))
         else:
             text_file.write('ShowEnvVarWarningDialog=0\n')
             text_file.write('Editor=/bin/cat\n')
```

### Comparing `kiauto-2.3.0/kiauto/interposer/libinterposer.so` & `kiauto-2.3.1/kiauto/interposer/libinterposer.so`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/kiauto/interposer.py` & `kiauto-2.3.1/kiauto/interposer.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/kiauto/log.py` & `kiauto-2.3.1/kiauto/log.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/kiauto/misc.py` & `kiauto-2.3.1/kiauto/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 CORRUPTED_PCB = 13
 NO_EN_LOCALE = 14
 MISSING_TOOL = 15
 KICAD_DIED = 16
 READ_ONLY_PROBLEM = 17
 WONT_OVERWRITE = 18
 KICAD_CLI_ERROR = 19
+CORRUPTED_CONFIG = 20
 # Wait 60 s to pcbnew/eeschema window to be present
 WAIT_START = 60
 # Name for testing versions
 NIGHTLY = 'nightly'
 # Scale factor for the timeouts
 TIME_OUT_MULT = 1.0
 
@@ -287,28 +288,33 @@
         self.wrns = []
         # Error filters
         self.err_filters = []
 
     def load_kicad_environment(self, logger):
         self.env = {}
         if self.conf_kicad_json:
-            env = self.get_config_vars_json(self.conf_kicad)
+            env = self.get_config_vars_json(self.conf_kicad, logger)
             if env:
                 self.env = env
         else:
             env = self.get_config_vars_ini(self.conf_kicad)
             if env:
                 for k, v in env.items():
                     self.env[k.upper()] = v
         logger.debug('KiCad environment: '+str(self.env))
 
     @staticmethod
-    def get_config_vars_json(file):
+    def get_config_vars_json(file, logger):
         with open(file, "rt") as f:
-            data = json.load(f)
+            raw_data = f.read()
+            try:
+                data = json.loads(raw_data)
+            except json.decoder.JSONDecodeError:
+                logger.error(f"Corrupted KiCad config file `{file}`:\n{raw_data}")
+                exit(CORRUPTED_CONFIG)
         if 'environment' in data and 'vars' in data['environment']:
             return data['environment']['vars']
         return None
 
     @staticmethod
     def get_config_vars_ini(file):
         config = configparser.ConfigParser()
@@ -344,8 +350,8 @@
 __author__ = 'Salvador E. Tropea'
 __copyright__ = 'Copyright 2018-2024, INTI/Productize SPRL'
 __credits__ = ['Salvador E. Tropea', 'Seppe Stas', 'Jesse Vincent', 'Scott Bezek']
 __license__ = 'Apache 2.0'
 __email__ = 'stropea@inti.gob.ar'
 __status__ = 'stable'
 __url__ = 'https://github.com/INTI-CMNB/KiAuto/'
-__version__ = '2.3.0'
+__version__ = '2.3.1'
```

### Comparing `kiauto-2.3.0/kiauto/ui_automation.py` & `kiauto-2.3.1/kiauto/ui_automation.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/kiauto.egg-info/PKG-INFO` & `kiauto-2.3.1/kiauto.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiauto
-Version: 2.3.0
+Version: 2.3.1
 Summary: KiCad Automation Scripts
 Home-page: https://github.com/INTI-CMNB/KiAuto/
 Author: Salvador E. Tropea
 Author-email: stropea@inti.gob.ar
 License: Apache License 2.0
 Description: 
         KiAuto
```

### Comparing `kiauto-2.3.0/kiauto.egg-info/SOURCES.txt` & `kiauto-2.3.1/kiauto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/setup.py` & `kiauto-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/src/eeschema_do` & `kiauto-2.3.1/src/eeschema_do`

 * *Files 0% similar despite different names*

```diff
@@ -862,14 +862,31 @@
             return True
         # The kicad-cli for v8 can do all, try the command
         res = run_command(['kicad-cli', 'sch', 'export', cfg.export_format], check=False)
         return 'Usage: '+cfg.export_format in res
     return False
 
 
+def setup_config_files(cfg):
+    # Back-up the current eeschema configuration
+    cfg.conf_eeschema_bkp = backup_config('Eeschema', cfg.conf_eeschema, EESCHEMA_CFG_PRESENT, cfg)
+    # Create a suitable configuration
+    create_eeschema_config(cfg)
+    # Back-up the current kicad_common configuration
+    cfg.conf_kicad_bkp = backup_config('KiCad common', cfg.conf_kicad, KICAD_CFG_PRESENT, cfg)
+    # Create a suitable configuration
+    create_kicad_config(cfg)
+    if cfg.kicad_version >= KICAD_VERSION_5_99:
+        # KiCad 6 breaks menu short-cuts, but we can configure user hotkeys
+        # Back-up the current user.hotkeys configuration
+        cfg.conf_hotkeys_bkp = backup_config('User hotkeys', cfg.conf_hotkeys, USER_HOTKEYS_PRESENT, cfg)
+        # Create a suitable configuration
+        create_user_hotkeys(cfg)
+
+
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='KiCad schematic automation')
     subparsers = parser.add_subparsers(help='Command:', dest='command')
 
     parser.add_argument('schematic', help='KiCad schematic file')
     parser.add_argument('output_dir', help='Output directory (ignored for bom_xml)')
 
@@ -959,28 +976,14 @@
     #
     # Configure KiCad in a deterministic way
     #
     # Force english + UTF-8
     os.environ['LANG'] = get_en_locale(logger)
     # Ensure we have a config dir
     check_kicad_config_dir(cfg)
-    # Back-up the current eeschema configuration
-    cfg.conf_eeschema_bkp = backup_config('Eeschema', cfg.conf_eeschema, EESCHEMA_CFG_PRESENT, cfg)
-    # Create a suitable configuration
-    create_eeschema_config(cfg)
-    # Back-up the current kicad_common configuration
-    cfg.conf_kicad_bkp = backup_config('KiCad common', cfg.conf_kicad, KICAD_CFG_PRESENT, cfg)
-    # Create a suitable configuration
-    create_kicad_config(cfg)
-    if cfg.kicad_version >= KICAD_VERSION_5_99:
-        # KiCad 6 breaks menu short-cuts, but we can configure user hotkeys
-        # Back-up the current user.hotkeys configuration
-        cfg.conf_hotkeys_bkp = backup_config('User hotkeys', cfg.conf_hotkeys, USER_HOTKEYS_PRESENT, cfg)
-        # Create a suitable configuration
-        create_user_hotkeys(cfg)
     # Make sure the user has sym-lib-table
     check_lib_table(cfg.user_sym_lib_table, cfg.sys_sym_lib_table)
     #
     # Setup filenames
     #
     input_file_no_ext = os.path.splitext(os.path.basename(cfg.input_file))[0]
     cfg.input_file = os.path.abspath(cfg.input_file)
@@ -1022,14 +1025,15 @@
         elif args.command == 'run_erc':
             error_level = eeschema_run_erc_schematic_cli(cfg)
         else:  # export
             eeschema_plot_schematic_cli(cfg)
         do_retry = False
         cfg.use_interposer = cfg.enable_interposer = False
     else:
+        setup_config_files(cfg)
         # Interposer settings
         check_interposer(args, logger, cfg)
         flog_out, flog_err, cfg.flog_int = get_log_files(output_dir, 'eeschema', also_interposer=cfg.enable_interposer)
         if cfg.enable_interposer:
             flog_out = subprocess.PIPE
             atexit.register(dump_interposer_dialog, cfg)
         os.environ['KIAUTO_INTERPOSER_LOWLEVEL_IO'] = '1' if use_low_level_io else ''
```

### Comparing `kiauto-2.3.0/src/kicad2step_do` & `kiauto-2.3.1/src/kicad2step_do`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/src/pcbnew_do` & `kiauto-2.3.1/src/pcbnew_do`

 * *Files 3% similar despite different names*

```diff
@@ -1261,24 +1261,39 @@
                                    "use_relative_paths": cfg.use_relative_paths}
             json_text = json.dumps(conf)
             text_file.write(json_text)
             logger.debug(json_text)
             # Colors for the 3D Viewer
             if cfg.bg_color_1 is not None:
                 conf = {}
+                if cfg.ki8 and cfg.use_layer_colors:
+                    # KiCad 8 doesn't have a mode for this, we must emulate
+                    copper = "rgb(77, 127, 196)"  # Top
+                    silk_bottom = "rgb(232, 178, 167)"
+                    silk_top = "rgb(242, 237, 161)"
+                    solder_bottom = "rgba(2, 255, 238, 0.400)"
+                    solder_top = "rgba(216, 100, 255, 0.400)"
+                    solder_paste = "rgba(180, 160, 154, 0.902)"  # Top
+                else:
+                    copper = to_rgb(cfg.copper_color)
+                    silk_bottom = to_rgb(cfg.silk_color, bottom=True)
+                    silk_top = to_rgb(cfg.silk_color)
+                    solder_bottom = to_rgb(cfg.sm_color, bottom=True)
+                    solder_top = to_rgb(cfg.sm_color)
+                    solder_paste = to_rgb(cfg.sp_color)
                 conf["3d_viewer"] = {"background_bottom": to_rgb(cfg.bg_color_1),
                                      "background_top": to_rgb(cfg.bg_color_2),
                                      "board": to_rgb(cfg.board_color),
-                                     "copper": to_rgb(cfg.copper_color),
-                                     "silkscreen_bottom": to_rgb(cfg.silk_color, bottom=True),
-                                     "silkscreen_top": to_rgb(cfg.silk_color),
-                                     "soldermask_bottom": to_rgb(cfg.sm_color, bottom=True),
-                                     "soldermask_top": to_rgb(cfg.sm_color),
-                                     "solderpaste": to_rgb(cfg.sp_color),
-                                     "use_board_stackup_colors": False}
+                                     "copper": copper,
+                                     "silkscreen_bottom": silk_bottom,
+                                     "silkscreen_top": silk_top,
+                                     "soldermask_bottom": solder_bottom,
+                                     "soldermask_top": solder_top,
+                                     "solderpaste": solder_paste,
+                                     "use_board_stackup_colors": cfg.use_stackup_colors}
                 json_text = json.dumps(conf)
                 os.makedirs(os.path.dirname(cfg.conf_colors), exist_ok=True)
                 with open(cfg.conf_colors, "wt") as color_file:
                     color_file.write(json_text)
                 logger.debug("Colors:")
                 logger.debug(json_text)
                 # 3D Viewer window
@@ -1293,20 +1308,31 @@
                                   "opengl_AA_mode": 0,
                                   "show_silkscreen": not cfg.hide_silkscreen,
                                   "show_soldermask": not cfg.hide_soldermask,
                                   "show_solderpaste": not cfg.hide_solderpaste,
                                   "show_zones": not cfg.hide_zones,
                                   "clip_silk_on_via_annulus": not cfg.dont_clip_silk_on_via_annulus,
                                   "subtract_mask_from_silk": not cfg.dont_substrack_mask_from_silk,
-                                  "realistic": not cfg.use_layer_colors,
                                   "show_board_body": not cfg.hide_board_body,
                                   "show_comments": cfg.show_comments,
-                                  "show_eco": cfg.show_eco,
                                   "show_adhesive": cfg.show_adhesive}
-                json_text = json.dumps(conf)
+                render = conf["render"]
+                if cfg.ki8:
+                    render["show_drawings"] = cfg.show_drawings
+                    if cfg.show_eco and not (cfg.show_eco1 or cfg.show_eco2):
+                        # Some compatibility
+                        cfg.show_eco1 = cfg.show_eco2 = True
+                    render["show_eco1"] = cfg.show_eco1
+                    render["show_eco2"] = cfg.show_eco2
+                    conf["use_stackup_colors"] = cfg.use_stackup_colors
+                    conf["current_layer_preset"] = ""
+                elif cfg.ki6:
+                    render["show_eco"] = cfg.show_eco
+                    render["realistic"] = not cfg.use_layer_colors
+                json_text = json.dumps(conf, sort_keys=True)
                 with open(cfg.conf_3dview, "wt") as viewer_file:
                     viewer_file.write(json_text)
                 logger.debug("3D Viewer:")
                 logger.debug(json_text)
         else:
             text_file.write('canvas_type=2\n')
             text_file.write('RefillZonesBeforeDrc=1\n')
@@ -1337,14 +1363,17 @@
             text_file.write('PcbFrameSize_x=%d\n' % (cfg.rec_width))
             text_file.write('PcbFrameSize_y=%d\n' % (cfg.rec_height))
             text_file.write('ShowAxis=0\n')
             text_file.write('ShowFootprints_Normal=%d\n' % (not cfg.no_tht))  # Normal?!
             # Insert????!!!! please a cup of coffee for this guy ...
             text_file.write('ShowFootprints_Insert=%d\n' % (not cfg.no_smd))
             text_file.write('ShowFootprints_Virtual=%d\n' % (not cfg.no_virtual))
+            text_file.write('ShowRealisticMode=%d\n' % (not cfg.use_layer_colors))
+            text_file.write('ShowEcoLayers=%d\n' % (cfg.show_eco))
+            text_file.write('ShowCommentsLayers=%d\n' % (cfg.show_comments))
             # We enable the raytracer after applying all moves
             # text_file.write('RenderEngine=%d\n' % (cfg.ray_tracing))
             write_color(text_file, 'Bg', cfg.bg_color_1)
             write_color(text_file, 'Bg', cfg.bg_color_2, 'Top')
             write_color(text_file, 'SMask', cfg.sm_color)
             write_color(text_file, 'SPaste', cfg.sp_color)
             write_color(text_file, 'Silk', cfg.silk_color)
@@ -1418,14 +1447,36 @@
 
 def wait_pcbnew_start_by_msg(cfg):
     wait_start_by_msg(cfg)
     # Make sure pcbnew has the focus, I saw problems with WM pop-ups getting the focus
     return wait_pcbnew()
 
 
+def setup_config_files(cfg):
+    # Back-up the current pcbnew configuration
+    cfg.conf_pcbnew_bkp = backup_config('PCBnew', cfg.conf_pcbnew, PCBNEW_CFG_PRESENT, cfg)
+    if cfg.conf_colors:
+        cfg.conf_colors_bkp = backup_config('Colors', cfg.conf_colors, PCBNEW_CFG_PRESENT, cfg)
+    if cfg.conf_3dview:
+        cfg.conf_3dview_bkp = backup_config('3D Viewer', cfg.conf_3dview, PCBNEW_CFG_PRESENT, cfg)
+    # Create a suitable configuration
+    create_pcbnew_config(cfg)
+    # Hotkeys
+    if not cfg.ki5:
+        # KiCad 6 breaks menu short-cuts, but we can configure user hotkeys
+        # Back-up the current user.hotkeys configuration
+        cfg.conf_hotkeys_bkp = backup_config('User hotkeys', cfg.conf_hotkeys, USER_HOTKEYS_PRESENT, cfg)
+        # Create a suitable configuration
+        create_user_hotkeys(cfg)
+    # Back-up the current kicad_common configuration
+    cfg.conf_kicad_bkp = backup_config('KiCad common', cfg.conf_kicad, KICAD_CFG_PRESENT, cfg)
+    # Create a suitable configuration
+    create_kicad_config(cfg)
+
+
 if __name__ == '__main__':  # noqa: C901
     parser = argparse.ArgumentParser(description='KiCad PCB automation')
     subparsers = parser.add_subparsers(help='Command:', dest='command')
 
     # short commands: iIrmnsSvVw
     parser.add_argument('--disable_interposer', '-I', help='Avoid using the interposer lib', action='store_true')
     parser.add_argument('--info', '-n', help='Show information about the installation', action=ShowInfoAction, nargs=0)
@@ -1466,16 +1517,18 @@
     drc_parser = subparsers.add_parser('run_drc', help='Run Design Rules Checker on a PCB')
     drc_parser.add_argument('--errors_filter', '-f', nargs=1, help='File with filters to exclude errors')
     drc_parser.add_argument('--force_gui', '-F', help='Force the use of the GUI (KiCad 6/7 not 8+)', action='store_true')
     drc_parser.add_argument('--ignore_unconnected', '-i', help='Ignore unconnected paths', action='store_true')
     drc_parser.add_argument('--output_name', '-o', nargs=1, help='Name of the output file', default=['drc_result.rpt'])
     drc_parser.add_argument('--save', '-s', help='Save after DRC (updating filled zones)', action='store_true')
     drc_parser.add_argument('--schematic-parity', '-p', help='Check PCB vs SCH parity (KiCad 8+)', action='store_true')
-    drc_parser.add_argument('--all-track-errors', '-t', help='Report all errors for each track (KiCad 8+)', action='store_true')
-    drc_parser.add_argument('--units', '-u', help='Report units (KiCad 8+)', default='mm', choices=['in', 'mm', 'mils'], type=str)
+    drc_parser.add_argument('--all-track-errors', '-t', help='Report all errors for each track (KiCad 8+)',
+                            action='store_true')
+    drc_parser.add_argument('--units', '-u', help='Report units (KiCad 8+)', default='mm', choices=['in', 'mm', 'mils'],
+                            type=str)
     drc_parser.add_argument('kicad_pcb_file', help='KiCad PCB file')
     drc_parser.add_argument('output_dir', help='Output directory')
 
     # short commands: bcdBoOrSTuvVwWxXyYzZ
     v3d_parser = subparsers.add_parser('3d_view', help='Capture the 3D view')
     v3d_parser.add_argument('--bg_color_1', '-b', nargs=1, help='Background color 1', default=['#66667F'])
     v3d_parser.add_argument('--bg_color_2', '-B', nargs=1, help='Background color 2', default=['#CCCCE5'])
@@ -1505,23 +1558,30 @@
     v3d_parser.add_argument('--no_smd', '-S', help='Do not include surface mount components', action='store_true')
     v3d_parser.add_argument('--no_tht', '-T', help='Do not include through-hole components', action='store_true')
     v3d_parser.add_argument('--virtual', '-V', help='Include virtual components', action='store_true')
     v3d_parser.add_argument('--orthographic', '-O', help='Enable the orthographic projection', action='store_true')
     v3d_parser.add_argument('--output_name', '-o', nargs=1, help='Name of the output file (PNG)', default=['capture.png'])
     v3d_parser.add_argument('--ray_tracing', '-r', help='Enable the realistic render', action='store_true')
     v3d_parser.add_argument('--show_adhesive', help='Show the adhesive layer', action='store_true')
-    v3d_parser.add_argument('--show_comments', help='Show the user comments layer', action='store_true')
-    v3d_parser.add_argument('--show_eco', help='Show the user eco layers', action='store_true')
+    v3d_parser.add_argument('--show_comments', help='Show the user comments layer (KiCad 7: also drawings)',
+                            action='store_true')
+    v3d_parser.add_argument('--show_drawings', help='Show the user comments layer (KiCad 8)', action='store_true')
+    v3d_parser.add_argument('--show_eco', help='Show both user eco layers (KiCad 7)', action='store_true')
+    v3d_parser.add_argument('--show_eco1', help='Show the user eco layer 1 (KiCad 8)', action='store_true')
+    v3d_parser.add_argument('--show_eco2', help='Show the user eco layer 2 (KiCad 8)', action='store_true')
     v3d_parser.add_argument('--silk_color', nargs=1,
                             help='Silk color (KiCad 6 supports color1,color2 for top/bottom)', default=['#E5E5E5'])
     v3d_parser.add_argument('--sm_color', nargs=1, help='Solder mask color (KiCad 6 supports color1,color2 for top/bottom)',
                             default=['#143324D4'])
     v3d_parser.add_argument('--sp_color', nargs=1, help='Solder paste color', default=['#808080'])
-    v3d_parser.add_argument('--use_layer_colors', help='Use the colors of the layers, not realistic colors (KiCad 6)',
-                            action='store_true')
+    group = v3d_parser.add_mutually_exclusive_group()
+    group.add_argument('--use_layer_colors', help='Use the colors of the layers, not realistic colors (KiCad 6+)',
+                       action='store_true')
+    group.add_argument('--use_stackup_colors', help='Use the colors defined in the stackup (KiCad 6+)',
+                       action='store_true')
     v3d_parser.add_argument('--use_rt_wait', '-u', help='Use the ray tracing end detection even on normal renders',
                             action='store_true')
     v3d_parser.add_argument('--view', '-v', nargs=1, help='Axis view, uppercase is reversed (i.e. Z is bottom)',
                             default=['z'], choices=['x', 'y', 'z', 'X', 'Y', 'Z'],)
     v3d_parser.add_argument('--wait_after_move', '-W', help='Wait after moving (KiCad 6 and interposer option)',
                             action='store_true')
     v3d_parser.add_argument('--wait_rt', '-w', nargs=1, help='Seconds to wait for the ray tracing render [5]', default=[5],
@@ -1683,26 +1743,33 @@
         cfg.hide_silkscreen = args.hide_silkscreen
         cfg.hide_soldermask = args.hide_soldermask
         cfg.hide_solderpaste = args.hide_solderpaste
         cfg.hide_zones = args.hide_zones
         cfg.dont_substrack_mask_from_silk = args.dont_substrack_mask_from_silk
         cfg.dont_clip_silk_on_via_annulus = args.dont_clip_silk_on_via_annulus
         cfg.use_layer_colors = args.use_layer_colors
+        cfg.use_stackup_colors = args.use_stackup_colors
         cfg.hide_board_body = args.hide_board_body
         cfg.show_comments = args.show_comments
+        cfg.show_drawings = args.show_drawings
         cfg.show_eco = args.show_eco
+        cfg.show_eco1 = args.show_eco1
+        cfg.show_eco2 = args.show_eco2
         cfg.show_adhesive = args.show_adhesive
     else:
         cfg.no_tht = False
         cfg.no_smd = False
         cfg.no_virtual = True
         cfg.ray_tracing = False
         cfg.bg_color_1 = cfg.bg_color_2 = cfg.board_color = None
         cfg.copper_color = cfg.silk_color = cfg.sm_color = cfg.sp_color = None
         cfg.wait_after_move = False
+        cfg.show_adhesive = cfg.show_eco2 = cfg.show_eco1 = cfg.show_eco = cfg.show_drawings = cfg.show_comments = False
+        cfg.use_layer_colors = False
+        cfg.use_stackup_colors = True
 
     if args.command == 'export_vrml':
         cfg.copy_3d_models = args.dir_models is not None
         cfg.origin_mode = 1 if args.ref_x is None and args.ref_y is None else 0
         cfg.ref_units = 1 if args.ref_units == 'inches' else 0
         cfg.ref_x = 0.0 if args.ref_x is None else args.ref_x
         cfg.ref_y = 0.0 if args.ref_y is None else args.ref_y
@@ -1715,34 +1782,16 @@
         cfg.ref_x = cfg.ref_y = 0.0
         cfg.dir_models = ''
 
     if args.command == 'run_drc' and args.errors_filter:
         load_filters(cfg, args.errors_filter[0])
 
     memorize_project(cfg)
-    # Back-up the current pcbnew configuration
+    # Ensure we have a config dir
     check_kicad_config_dir(cfg)
-    cfg.conf_pcbnew_bkp = backup_config('PCBnew', cfg.conf_pcbnew, PCBNEW_CFG_PRESENT, cfg)
-    if cfg.conf_colors:
-        cfg.conf_colors_bkp = backup_config('Colors', cfg.conf_colors, PCBNEW_CFG_PRESENT, cfg)
-    if cfg.conf_3dview:
-        cfg.conf_3dview_bkp = backup_config('3D Viewer', cfg.conf_3dview, PCBNEW_CFG_PRESENT, cfg)
-    # Create a suitable configuration
-    create_pcbnew_config(cfg)
-    # Hotkeys
-    if not cfg.ki5:
-        # KiCad 6 breaks menu short-cuts, but we can configure user hotkeys
-        # Back-up the current user.hotkeys configuration
-        cfg.conf_hotkeys_bkp = backup_config('User hotkeys', cfg.conf_hotkeys, USER_HOTKEYS_PRESENT, cfg)
-        # Create a suitable configuration
-        create_user_hotkeys(cfg)
-    # Back-up the current kicad_common configuration
-    cfg.conf_kicad_bkp = backup_config('KiCad common', cfg.conf_kicad, KICAD_CFG_PRESENT, cfg)
-    # Create a suitable configuration
-    create_kicad_config(cfg)
     # Make sure the user has fp-lib-table
     check_lib_table(cfg.user_fp_lib_table, cfg.sys_fp_lib_table)
     # Create output dir, compute full name for output file and remove it
     output_dir = os.path.abspath(args.output_dir)
     cfg.video_dir = cfg.output_dir = output_dir
     os.makedirs(output_dir, exist_ok=True)
     # Remove the output file
@@ -1763,14 +1812,15 @@
         else:
             # First command to migrate to Python!
             run_drc_python(cfg)
         error_level = process_drc_out(cfg)
         do_retry = False
         cfg.use_interposer = cfg.enable_interposer = False
     else:
+        setup_config_files(cfg)
         # Interposer settings
         check_interposer(args, logger, cfg)
         # When using the interposer inform the output file name using the environment
         setup_interposer_filename(cfg)
         flog_out, flog_err, cfg.flog_int = get_log_files(output_dir, 'pcbnew', also_interposer=cfg.enable_interposer)
         if cfg.enable_interposer:
             flog_out = subprocess.PIPE
```

### Comparing `kiauto-2.3.0/tests/eeschema/test_bom_xml.py` & `kiauto-2.3.1/tests/eeschema/test_bom_xml.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/eeschema/test_erc.py` & `kiauto-2.3.1/tests/eeschema/test_erc.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/eeschema/test_export.py` & `kiauto-2.3.1/tests/eeschema/test_export.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/eeschema/test_netlist.py` & `kiauto-2.3.1/tests/eeschema/test_netlist.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/eeschema/test_sch_misc.py` & `kiauto-2.3.1/tests/eeschema/test_sch_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 from kiauto.misc import (EESCHEMA_CFG_PRESENT, KICAD_CFG_PRESENT, NO_SCHEMATIC, WRONG_SCH_NAME, EESCHEMA_ERROR,
                          WRONG_ARGUMENTS, KICAD_CLI_ERROR)
 
 PROG = 'eeschema_do'
 BOGUS_SCH = 'bogus'
 
 
+@pytest.mark.skipif(context.ki8, reason="KiCad 8 uses cli")
 def test_eeschema_config_backup(test_dir):
     """ Here we test the extreme situation that a previous run left a config
         back-up and the user must take action. """
     prj = 'good-project'
     ctx = context.TestContextSCH(test_dir, 'Eeschema_config_bkp', prj)
     # Create a fake back-up
     if not os.path.isdir(ctx.kicad_cfg_dir):
@@ -47,14 +48,15 @@
     ctx.run(cmd, EESCHEMA_CFG_PRESENT)
     os.remove(old_config_file)
     m = ctx.search_err('Eeschema config back-up found')
     assert m is not None
     ctx.clean_up()
 
 
+@pytest.mark.skipif(context.ki8, reason="KiCad 8 uses cli")
 def test_kicad_common_config_backup(test_dir):
     """ Here we test the extreme situation that a previous run left a config
         back-up and the user must take action. """
     prj = 'good-project'
     ctx = context.TestContextSCH(test_dir, 'Eeschema_common_config_bkp', prj)
     # Create a fake back-up
     if not os.path.isdir(ctx.kicad_cfg_dir):
```

### Comparing `kiauto-2.3.0/tests/kicad2step/test_step.py` & `kiauto-2.3.1/tests/kicad2step/test_step.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/pcbnew/test_3d.py` & `kiauto-2.3.1/tests/pcbnew/test_export_gencad.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 # -*- coding: utf-8 -*-
-# Copyright (c) 2021 Salvador E. Tropea
-# Copyright (c) 2021 Instituto Nacional de Tecnologïa Industrial
+# Copyright (c) 2022 Theo Hussey
 # License: Apache 2.0
 # Project: KiAuto (formerly kicad-automation-scripts)
 """
-Tests for 'pcbnew_do 3d_view'
+Tests for 'pcbnew_do export_gencad'
 
 For debug information use:
 pytest-3 --log-cli-level debug
 
 """
-
 import os
 import sys
+import re
 # Look for the 'utils' module from where the script is running
 script_dir = os.path.dirname(os.path.abspath(__file__))
 prev_dir = os.path.dirname(script_dir)
 sys.path.insert(0, prev_dir)
 # Utils import
 from utils import context
 sys.path.insert(0, os.path.dirname(prev_dir))
 
 PROG = 'pcbnew_do'
 
 
-def test_3d_view_1(test_dir):
-    """ Simple 3D Viewer test """
-    ctx = context.TestContext(test_dir, '3DView_1', 'good-project')
-    cmd = [PROG, '-r', '-vvv', '3d_view', '-x', '1', '--output_name', 'good_3d_rt_1.png', '-r', '-d', '-w', '20',
-           '-X', '3', '-Z', '3']
-    if not context.ki8:
-        # KiCad 8 does a zoom to fit
-        cmd.extend(['--zoom', '3'])
-    ctx.run(cmd)
-    ctx.compare_image('good_3d_rt_1.png', fuzz='50%', tol=2000)
-    ctx.clean_up()
-
-
-def test_3d_view_2(test_dir):
-    """ Simple 3D Viewer test """
-    ctx = context.TestContext(test_dir, '3DView_2', 'good-project')
-    cmd = [PROG, '-vvv', '3d_view', '-x', '-1', '--output_name', 'good_3d_rt_2.png', '--no_smd', '-r', '-O',
-           '-d', '-w', '20', '--zoom']
-    # KiCad 8 does a zoom to fit
-    cmd.append('1' if context.ki8 else '6')
+def test_export_gencad_1(test_dir):
+    """ Generate a GenCAD file with no special options test """
+    ctx = context.TestContext(test_dir, 'export_gencad_1', 'good-project')
+    cmd = [PROG, '-vv', 'export_gencad', '-f', '-n', '-O', '--output_name', 'good.cad']
     ctx.run(cmd)
-    ctx.compare_image('good_3d_rt_2.png', fuzz='50%', tol=2000)
+    ctx.expect_out_file('good.cad')
+    file = ctx.get_out_path('good.cad')
+    with open(file, 'rt') as f:
+        text = f.read()
+    text = re.sub(r'(USER|DRAWING) "(.*)"', r'\1 ""', text)
+    with open(file, 'wt') as f:
+        f.write(text)
+    ctx.compare_txt('good.cad')
     ctx.clean_up()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kiauto-2.3.0/tests/pcbnew/test_drc.py` & `kiauto-2.3.1/tests/pcbnew/test_drc.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/pcbnew/test_export_vrml.py` & `kiauto-2.3.1/tests/pcbnew/test_export_vrml.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/pcbnew/test_pcb_misc.py` & `kiauto-2.3.1/tests/pcbnew/test_pcb_misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         os.makedirs(ctx.kicad_cfg_dir, exist_ok=True)
     old_config_file = ctx.pcbnew_conf + '.pre_script'
     logging.debug('PCBnew old config: '+old_config_file)
     with open(old_config_file, 'wt') as f:
         f.write('Dummy back-up\n')
     # Run the command
     try:
-        cmd = [PROG, 'run_drc']
+        cmd = [PROG, 'ipc_netlist']
         ctx.run(cmd, PCBNEW_CFG_PRESENT)
     finally:
         os.remove(old_config_file)
     m = ctx.search_err('PCBnew config back-up found')
     assert m is not None
     ctx.clean_up()
```

### Comparing `kiauto-2.3.0/tests/pcbnew/test_print_layers.py` & `kiauto-2.3.1/tests/pcbnew/test_print_layers.py`

 * *Files identical despite different names*

### Comparing `kiauto-2.3.0/tests/utils/context.py` & `kiauto-2.3.1/tests/utils/context.py`

 * *Files identical despite different names*

