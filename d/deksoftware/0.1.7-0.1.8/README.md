# Comparing `tmp/deksoftware-0.1.7-py3-none-any.whl.zip` & `tmp/deksoftware-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,25 +1,25 @@
-Zip file size: 10344 bytes, number of entries: 23
--rw-r--r--  2.0 unx      242 b- defN 16-Jan-01 00:00 deksoftware-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 deksoftware-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       66 b- defN 16-Jan-01 00:00 deksoftware-0.1.7.dist-info/entry_points.txt
+Zip file size: 10365 bytes, number of entries: 23
+-rw-r--r--  2.0 unx      242 b- defN 16-Jan-01 00:00 deksoftware-0.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       90 b- defN 16-Jan-01 00:00 deksoftware-0.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       66 b- defN 16-Jan-01 00:00 deksoftware-0.1.8.dist-info/entry_points.txt
 -rw-r--r--  2.0 unx     1856 b- defN 16-Jan-01 00:00 deksoftware/click/__entry__.py
 -rw-r--r--  2.0 unx       54 b- defN 16-Jan-01 00:00 deksoftware/click/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 deksoftware/core/__init__.py
 -rw-r--r--  2.0 unx       85 b- defN 16-Jan-01 00:00 deksoftware/core/installer/__init__.py
--rw-r--r--  2.0 unx      626 b- defN 16-Jan-01 00:00 deksoftware/core/installer/base/__init__.py
+-rw-r--r--  2.0 unx      677 b- defN 16-Jan-01 00:00 deksoftware/core/installer/base/__init__.py
 -rw-r--r--  2.0 unx      411 b- defN 16-Jan-01 00:00 deksoftware/core/installer/helm.py
 -rw-r--r--  2.0 unx      133 b- defN 16-Jan-01 00:00 deksoftware/core/installer/libvirt.py
 -rw-r--r--  2.0 unx     1129 b- defN 16-Jan-01 00:00 deksoftware/core/installer/nerdctl.py
--rw-r--r--  2.0 unx      567 b- defN 16-Jan-01 00:00 deksoftware/core/installer/whl.py
+-rw-r--r--  2.0 unx      551 b- defN 16-Jan-01 00:00 deksoftware/core/installer/whl.py
 -rw-r--r--  2.0 unx       45 b- defN 16-Jan-01 00:00 deksoftware/core/package/__init__.py
 -rw-r--r--  2.0 unx     2313 b- defN 16-Jan-01 00:00 deksoftware/core/package/base/__init__.py
 -rw-r--r--  2.0 unx      603 b- defN 16-Jan-01 00:00 deksoftware/core/package/coding.py
 -rw-r--r--  2.0 unx      123 b- defN 16-Jan-01 00:00 deksoftware/core/package/default.py
--rw-r--r--  2.0 unx      872 b- defN 16-Jan-01 00:00 deksoftware/core/repository.py
+-rw-r--r--  2.0 unx      915 b- defN 16-Jan-01 00:00 deksoftware/core/repository.py
 -rw-r--r--  2.0 unx      693 b- defN 16-Jan-01 00:00 deksoftware/resources/index.yaml
 -rw-r--r--  2.0 unx     2598 b- defN 16-Jan-01 00:00 deksoftware/resources/lock/libvirt.txt
 -rw-r--r--  2.0 unx      173 b- defN 16-Jan-01 00:00 deksoftware/resources/shell/history.sh
 -rw-r--r--  2.0 unx      705 b- defN 16-Jan-01 00:00 deksoftware/resources/shell/libvirt.sh
 -rw-r--r--  2.0 unx     2463 b- defN 16-Jan-01 00:00 deksoftware/resources/shell/sinicization.sh
-?rw-------  2.0 unx     2054 b- defN 16-Jan-01 00:00 deksoftware-0.1.7.dist-info/RECORD
-23 files, 17901 bytes uncompressed, 6932 bytes compressed:  61.3%
+?rw-------  2.0 unx     2054 b- defN 16-Jan-01 00:00 deksoftware-0.1.8.dist-info/RECORD
+23 files, 17979 bytes uncompressed, 6953 bytes compressed:  61.3%
```

## zipnote {}

```diff
@@ -1,14 +1,14 @@
-Filename: deksoftware-0.1.7.dist-info/METADATA
+Filename: deksoftware-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: deksoftware-0.1.7.dist-info/WHEEL
+Filename: deksoftware-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: deksoftware-0.1.7.dist-info/entry_points.txt
+Filename: deksoftware-0.1.8.dist-info/entry_points.txt
 Comment: 
 
 Filename: deksoftware/click/__entry__.py
 Comment: 
 
 Filename: deksoftware/click/__init__.py
 Comment: 
@@ -60,11 +60,11 @@
 
 Filename: deksoftware/resources/shell/libvirt.sh
 Comment: 
 
 Filename: deksoftware/resources/shell/sinicization.sh
 Comment: 
 
-Filename: deksoftware-0.1.7.dist-info/RECORD
+Filename: deksoftware-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## deksoftware/core/installer/base/__init__.py

```diff
@@ -1,14 +1,15 @@
 import os
 from dektools.shell import shell_wrapper
+from dektools.file import normal_path
 
 
 class InstallerBase:
     def __init__(self, path):
-        self.path = path
+        self.path = normal_path(path)
 
     def run(self):
         raise NotImplementedError
 
     @staticmethod
     def exe(path, target=None):
         target = target or '/usr/local/bin'
```

## deksoftware/core/installer/whl.py

```diff
@@ -1,16 +1,16 @@
 import os
+from dektools.file import list_dir
 from dektools.shell import shell_wrapper
 from dektools.py import get_whl_name
 from .base import InstallerBase, register_installer
 
 
 @register_installer('whl')
 class WhlInstaller(InstallerBase):
     def run(self):
-        if os.path.isdir(self.path):
-            for whl_file in self.path:
-                if whl_file.endswith('.whl'):
-                    shell_wrapper(
-                        f'bash -c "python3 -m pip uninstall -y {get_whl_name(whl_file)} 2>&1 || true;'
-                        f'python3 -m pip install {whl_file}"'
-                    )
+        for whl_file in list_dir(self.path):
+            if whl_file.endswith('.whl'):
+                shell_wrapper(
+                    f'bash -c "python3 -m pip uninstall -y {get_whl_name(whl_file)} 2>&1 || true;'
+                    f'python3 -m pip install {whl_file}"'
+                )
```

## deksoftware/core/repository.py

```diff
@@ -16,11 +16,12 @@
             pk = package_cls(pd, *args)
             self.packages[pk.name] = pk
 
     def pull(self, name, version):
         return self.packages[name].pull(version)
 
     def install(self, name, version=None, path=None):
-        path = path or self.pull(name, version or 'latest')
+        path_final = path or self.pull(name, version or 'latest')
         installer_cls = all_installer[name]
-        installer_cls(path).run()
-        remove_path(path)
+        installer_cls(path_final).run()
+        if not path:
+            remove_path(path_final)
```

