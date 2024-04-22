# Comparing `tmp/es_wait-0.1.4.tar.gz` & `tmp/es_wait-0.2.0.tar.gz`

## Comparing `es_wait-0.1.4.tar` & `es_wait-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.1.4/pytest.ini
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/__init__.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/args.py
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/base.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/exists.py
--rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/health.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/relocate.py
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/restore.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/snapshot.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.1.4/src/es_wait/task.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.1.4/.gitignore
--rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.1.4/LICENSE
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.1.4/README.md
--rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 es_wait-0.2.0/pytest.ini
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/__init__.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/args.py
+-rw-r--r--   0        0        0     3226 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/base.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/exists.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/health.py
+-rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/relocate.py
+-rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/restore.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/snapshot.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 es_wait-0.2.0/src/es_wait/task.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 es_wait-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11347 2020-02-02 00:00:00.000000 es_wait-0.2.0/LICENSE
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 es_wait-0.2.0/README.md
+-rw-r--r--   0        0        0     3922 2020-02-02 00:00:00.000000 es_wait-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 es_wait-0.2.0/PKG-INFO
```

### Comparing `es_wait-0.1.4/src/es_wait/args.py` & `es_wait-0.2.0/src/es_wait/args.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/base.py` & `es_wait-0.2.0/src/es_wait/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,40 +43,45 @@
             msg = f'Keyword arg {name} cannot be None'
             self.logger.critical(msg)
             raise ValueError(msg)
 
     def setup(self) -> None:
         """Setup the waiter"""
 
-    def wait_for_it(self) -> None:
+    def wait_for_it(self, frequency: int = 5) -> None:
         """Do the actual waiting"""
         # Now with this mapped, we can perform the wait as indicated.
         start_time = self.now
-        result = False
+        success = False
+        self.logger.debug('Only logging every %s seconds', frequency)
         while True:
             elapsed = int((self.now - start_time).total_seconds())
-            self.logger.debug('Elapsed time: %s seconds', elapsed)
+            loggit = elapsed % frequency == 0 # Only log every frequency seconds
             response = self.check
+            # Successfully completed task.
             if response:
                 self.logger.debug('%s finished executing', self.checkid)
-                result = True
+                total = f'{(self.now - start_time).tota_seconds():.2f}'
+                self.logger.debug('Elapsed time: %s seconds', total)
+                success = True
                 break
             # Not success, and reached timeout (if defined)
             if (self.timeout != -1) and (elapsed >= self.timeout):
                 msg = f'The {self.checkid} did not complete within {self.timeout} seconds.'
                 self.logger.error(msg)
                 break
             # Not timed out and not yet success, so we wait.
-            msg = (
-                f'The {self.checkid} is not yet complete. {elapsed} total seconds have elapsed. '
-                f'Waiting {self.pause} seconds before checking again.'
-            )
-            self.logger.debug(msg)
-            sleep(self.pause)
+            if loggit:
+                msg = (
+                    f'The {self.checkid} is not yet complete. {elapsed} total seconds have '
+                    f'elapsed. Waiting {self.pause} seconds before checking again.'
+                )
+                self.logger.debug(msg)
+            sleep(self.pause) # Actual wait here
 
-        if not result:
+        if not success:
             msg = (
                 f'The {self.checkid} failed to complete in the '
                 f'timeout period of {self.timeout} seconds'
             )
             self.logger.error(msg)
             raise TimeoutError(msg)
```

### Comparing `es_wait-0.1.4/src/es_wait/exists.py` & `es_wait-0.2.0/src/es_wait/exists.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/health.py` & `es_wait-0.2.0/src/es_wait/health.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/relocate.py` & `es_wait-0.2.0/src/es_wait/relocate.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/restore.py` & `es_wait-0.2.0/src/es_wait/restore.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/snapshot.py` & `es_wait-0.2.0/src/es_wait/snapshot.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/src/es_wait/task.py` & `es_wait-0.2.0/src/es_wait/task.py`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/.gitignore` & `es_wait-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/LICENSE` & `es_wait-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/pyproject.toml` & `es_wait-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `es_wait-0.1.4/PKG-INFO` & `es_wait-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: es-wait
-Version: 0.1.4
+Version: 0.2.0
 Summary: Helping you wait for certain Elasticsearch tasks and API calls to finish
 Project-URL: Documentation, https://github.com/untergeek/es-wait#readme
 Project-URL: Issues, https://github.com/untergeek/es-wait/issues
 Project-URL: Source, https://github.com/untergeek/es-wait
 Author-email: Aaron Mildenstein <untergeek@elastic.co>
 License: Apache-2.0
 License-File: LICENSE
```

