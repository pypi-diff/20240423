# Comparing `tmp/pypaq-1.7.5.tar.gz` & `tmp/pypaq-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypaq-1.7.5.tar", last modified: Sat Apr  6 18:28:17 2024, max compression
+gzip compressed data, was "pypaq-1.7.6.tar", last modified: Tue Apr 23 11:27:37 2024, max compression
```

## Comparing `pypaq-1.7.5.tar` & `pypaq-1.7.6.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-06 18:28:17.451240 pypaq-1.7.5/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      470 2024-04-06 17:44:30.000000 pypaq-1.7.5/README.md
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       41 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/exception.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/lipytools/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4111 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/decorators.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      826 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/double_hinge.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3934 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/files.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     1297 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/moving_average.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4908 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/plots.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     5783 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/printout.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     2361 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/pylogger.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       73 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/softmax.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)      977 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/stats.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     1941 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/lipytools/time_reporter.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/mpython/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1570 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/mpdecor.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     5528 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/mpython/mptools.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.447240 pypaq-1.7.5/pypaq/pms/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/__init__.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     4582 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/base.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     3651 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/config_manager.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     8354 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/para.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)    13853 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/parasave.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)    18707 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/paspa.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)     6863 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pms/points_cloud.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      211 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/pytypes.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/pypaq/textools/
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/__init__.py
--rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1210 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/text_metrics.py
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      668 2024-04-06 17:44:30.000000 pypaq-1.7.5/pypaq/textools/text_processing.py
-drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-06 18:28:17.451240 pypaq-1.7.5/pypaq.egg-info/
--rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/PKG-INFO
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      852 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/SOURCES.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/dependency_links.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       63 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/requires.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)        6 2024-04-06 18:28:17.000000 pypaq-1.7.5/pypaq.egg-info/top_level.txt
--rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-06 18:28:17.451240 pypaq-1.7.5/setup.cfg
--rw-rw-r--   0 ppp       (1000) ppp       (1000)      491 2024-04-06 18:22:30.000000 pypaq-1.7.5/setup.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.587747 pypaq-1.7.6/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-23 11:27:37.587747 pypaq-1.7.6/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      470 2024-04-06 17:44:30.000000 pypaq-1.7.6/README.md
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.579747 pypaq-1.7.6/pypaq/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       41 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/exception.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/lipytools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4111 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/decorators.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      826 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/double_hinge.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3930 2024-04-06 21:52:22.000000 pypaq-1.7.6/pypaq/lipytools/files.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1531 2024-04-07 18:56:30.000000 pypaq-1.7.6/pypaq/lipytools/moving_average.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     4908 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/plots.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     6044 2024-04-22 18:29:22.000000 pypaq-1.7.6/pypaq/lipytools/printout.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     2361 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/pylogger.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       73 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/softmax.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)      977 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/stats.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     1941 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/lipytools/time_reporter.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/mpython/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1570 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/mpdecor.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     5528 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/mpython/mptools.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/pms/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/__init__.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     4582 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/base.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     3651 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/config_manager.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     8354 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/para.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    13853 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/parasave.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)    18707 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/paspa.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)     6863 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pms/points_cloud.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      211 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/pytypes.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq/textools/
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        0 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/__init__.py
+-rwxrwxr-x   0 ppp       (1000) ppp       (1000)     1210 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/text_metrics.py
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      668 2024-04-06 17:44:30.000000 pypaq-1.7.6/pypaq/textools/text_processing.py
+drwxrwxr-x   0 ppp       (1000) ppp       (1000)        0 2024-04-23 11:27:37.583747 pypaq-1.7.6/pypaq.egg-info/
+-rw-r--r--   0 ppp       (1000) ppp       (1000)      383 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/PKG-INFO
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      852 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        1 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       63 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/requires.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)        6 2024-04-23 11:27:37.000000 pypaq-1.7.6/pypaq.egg-info/top_level.txt
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)       38 2024-04-23 11:27:37.587747 pypaq-1.7.6/setup.cfg
+-rw-rw-r--   0 ppp       (1000) ppp       (1000)      491 2024-04-23 11:27:35.000000 pypaq-1.7.6/setup.py
```

### Comparing `pypaq-1.7.5/pypaq/lipytools/decorators.py` & `pypaq-1.7.6/pypaq/lipytools/decorators.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/lipytools/double_hinge.py` & `pypaq-1.7.6/pypaq/lipytools/double_hinge.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/lipytools/files.py` & `pypaq-1.7.6/pypaq/lipytools/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     if not os.path.isfile(file_path):
         if raise_exception:
             raise FileNotFoundError(f'file {file_path} not exists!')
         return None
     csv.field_size_limit(sys.maxsize)
     with open(file_path, newline='') as f:
         reader = csv.reader(f)
-        return [row for row in reader][1:]
+        return [row for row in reader]
 
 
 def r_yaml(file_path, raise_exception=False):
     if not os.path.isfile(file_path):
         if raise_exception:
             raise FileNotFoundError(f'file {file_path} not exists!')
         return None
```

### Comparing `pypaq-1.7.5/pypaq/lipytools/moving_average.py` & `pypaq-1.7.6/pypaq/lipytools/moving_average.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,45 +6,46 @@
 
 class MovAvg:
     """ moving average
     updates self.value with factor (given while init) """
 
     def __init__(
             self,
-            factor: NUM=        0.1,    # (0.0;1.0>
-            first_avg: bool=    True,   # first 1/factor values will be averaged
+            factor: NUM=                0.1,    # (0.0;1.0>
+            first_avg: bool=            True,   # first 1/factor values will be averaged
+            init_value: Optional[NUM]=  None,
+            init_weight: int=           10,
     ):
-        self.value: Optional[NUM] = None
+        self.value: Optional[NUM] = init_value
 
         if not 0 < factor <= 1:
             raise PyPaqException('factor should: 0 < factor <= 1')
 
         self.factor = factor
-        self.upd_ix = 0
+        self.upd_ix = 0 if self.value is None else init_weight
         self.first_avg = first_avg
-        self.firstL = []
-
+        self.firstL = [] if self.value is None else [self.value] * self.upd_ix
 
     def upd(self, val:NUM):
 
         if self.first_avg and self.upd_ix < 1/self.factor:
             self.firstL.append(val)
             self.value = sum(self.firstL) / len(self.firstL)
         else:
-            if self.value is None: self.value = val
-            else: self.value = (1-self.factor)*self.value + self.factor*val
+            if self.value is None:
+                self.value = val
+            else:
+                self.value = (1-self.factor)*self.value + self.factor*val
 
         self.upd_ix += 1
 
         return self.value
 
-
     def reset(self, val:Optional[NUM]=None):
         self.value = val
         self.upd_ix = 0
         self.firstL = []
 
-
     def __call__(self) -> NUM:
         if self.value is None:
             raise PyPaqException('MovAvg not updated yet, value unknown')
         return self.value
```

### Comparing `pypaq-1.7.5/pypaq/lipytools/plots.py` & `pypaq-1.7.6/pypaq/lipytools/plots.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/lipytools/printout.py` & `pypaq-1.7.6/pypaq/lipytools/printout.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,58 +155,63 @@
 
         self._prev = 0
         self._ptime = time.time()
         self._stime = self._ptime
         self.speed = MovAvg()
 
     def __call__(self, current:NUM, prefix:str='', suffix:str=''):
-        prog = current / self.total
-        if prog > 1:
-            prog = 1
-
-        diff_n = current - self._prev
-        ctime = time.time()
-        diff_time = ctime - self._ptime
-        self._prev = current
-        self._ptime = ctime
-
-        filled_length = int(self.length * prog)
-        bar = self.fill * filled_length + '-' * (self.length - filled_length)
-
-        fract = f'{current}/{self.total}' if self.show_fract else ''
-
-        speed_str = ''
-        self.speed.upd(diff_n / diff_time)
-        speed = self.speed()
-        if self.show_speed:
-            if speed > 1:
-                if speed > 100: speed_str = f'{int(speed)}/s'
-                else:           speed_str = f'{speed:.1f}/s'
-            else:               speed_str = f'{speed:.3f}/s'
-
-        eta_str = ''
-        if self.show_eta:
-            if speed > 0:
-                eta = (self.total - current) / speed
-                if eta > 4000:    eta_str = f'{eta/60/60:.1f}h'
+
+        if current > self._prev:
+
+            prog = current / self.total
+            if prog > 1:
+                prog = 1
+
+            diff_n = current - self._prev
+            ctime = time.time()
+            diff_time = ctime - self._ptime
+            self._prev = current
+            self._ptime = ctime
+
+            filled_length = int(self.length * prog)
+            bar = self.fill * filled_length + '-' * (self.length - filled_length)
+
+            fract = f'{current}/{self.total}' if self.show_fract else ''
+
+            speed_str = ''
+            self.speed.upd(diff_n / diff_time)
+            speed = self.speed()
+            if self.show_speed:
+                if speed > 1:
+                    if speed > 100: speed_str = f'{int(speed)}/s'
+                    else:           speed_str = f'{speed:.1f}/s'
+                else:               speed_str = f'{speed:.3f}/s'
+
+            eta_str = ''
+            if self.show_eta:
+                if speed > 0:
+                    eta = (self.total - current) / speed
+                    if eta < 0:
+                        eta = 0
+                    if eta > 4000:    eta_str = f'{eta/60/60:.1f}h'
+                    else:
+                        if eta > 100: eta_str = f'{eta/60:.1f}m'
+                        else:         eta_str = f'{eta:.1f}s'
+                else:                 eta_str = '---'
+                eta_str = f'ETA:{eta_str}'
+
+            detailsL = [fract,speed_str,eta_str]
+            detailsL = [e for e in detailsL if e]
+            details = f'{" ".join(detailsL)} ' if detailsL else ''
+
+            elapsed = ''
+            if prog == 1 and self.show_eta:
+                el = self._ptime-self._stime
+                if el > 4000:    elapsed = f'TOT:{el/60/60:.1f}h '
                 else:
-                    if eta > 100: eta_str = f'{eta/60:.1f}m'
-                    else:         eta_str = f'{eta:.1f}s'
-            else:                 eta_str = '---'
-            eta_str = f'ETA:{eta_str}'
-
-        detailsL = [fract,speed_str,eta_str]
-        detailsL = [e for e in detailsL if e]
-        details = f'{" ".join(detailsL)} ' if detailsL else ''
-
-        elapsed = ''
-        if prog == 1 and self.show_eta:
-            el = self._ptime-self._stime
-            if el > 4000:    elapsed = f'TOT:{el / 60 / 60:.1f}h '
-            else:
-                if el > 100: elapsed = f'TOT:{el / 60:.1f}m '
-                else:        elapsed = f'TOT:{el:.1f}s '
+                    if el > 100: elapsed = f'TOT:{el/60:.1f}m '
+                    else:        elapsed = f'TOT:{el:.1f}s '
 
-        printover(f'{prefix} |{bar}| {prog * 100:.1f}% {details}{elapsed}{suffix}')
+            printover(f'{prefix} |{bar}| {prog * 100:.1f}% {details}{elapsed}{suffix}')
 
-        if prog == 1:
-            print()
+            if prog == 1:
+                print()
```

### Comparing `pypaq-1.7.5/pypaq/lipytools/pylogger.py` & `pypaq-1.7.6/pypaq/lipytools/pylogger.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/lipytools/stats.py` & `pypaq-1.7.6/pypaq/lipytools/stats.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/lipytools/time_reporter.py` & `pypaq-1.7.6/pypaq/lipytools/time_reporter.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/mpython/mpdecor.py` & `pypaq-1.7.6/pypaq/mpython/mpdecor.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/mpython/mptools.py` & `pypaq-1.7.6/pypaq/mpython/mptools.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/base.py` & `pypaq-1.7.6/pypaq/pms/base.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/config_manager.py` & `pypaq-1.7.6/pypaq/pms/config_manager.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/para.py` & `pypaq-1.7.6/pypaq/pms/para.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/parasave.py` & `pypaq-1.7.6/pypaq/pms/parasave.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/paspa.py` & `pypaq-1.7.6/pypaq/pms/paspa.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/pms/points_cloud.py` & `pypaq-1.7.6/pypaq/pms/points_cloud.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/textools/text_metrics.py` & `pypaq-1.7.6/pypaq/textools/text_metrics.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq/textools/text_processing.py` & `pypaq-1.7.6/pypaq/textools/text_processing.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.7.5/pypaq.egg-info/SOURCES.txt` & `pypaq-1.7.6/pypaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

