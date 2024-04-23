# Comparing `tmp/nestipy_ioc-0.1.0.tar.gz` & `tmp/nestipy_ioc-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nestipy_ioc-0.1.0.tar", max compression
+gzip compressed data, was "nestipy_ioc-0.1.10.tar", max compression
```

## Comparing `nestipy_ioc-0.1.0.tar` & `nestipy_ioc-0.1.10.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.0/README.md
--rw-r--r--   0        0        0      373 2024-04-22 14:27:29.796578 nestipy_ioc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      284 2024-04-22 14:29:42.080993 nestipy_ioc-0.1.0/src/nestipy_ioc/__init__.py
--rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.0/src/nestipy_ioc/annotation.py
--rw-r--r--   0        0        0    12296 2024-04-22 14:25:54.304207 nestipy_ioc-0.1.0/src/nestipy_ioc/container.py
--rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.0/src/nestipy_ioc/context_container.py
--rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.0/src/nestipy_ioc/meta.py
--rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.0/src/nestipy_ioc/provider.py
--rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.0/src/nestipy_ioc/utils.py
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-22 13:24:07.751008 nestipy_ioc-0.1.10/README.md
+-rw-r--r--   0        0        0      374 2024-04-23 14:25:15.014849 nestipy_ioc-0.1.10/pyproject.toml
+-rw-r--r--   0        0        0      284 2024-04-22 14:29:42.080993 nestipy_ioc-0.1.10/src/nestipy_ioc/__init__.py
+-rw-r--r--   0        0        0      122 2024-04-22 14:21:10.410610 nestipy_ioc-0.1.10/src/nestipy_ioc/annotation.py
+-rw-r--r--   0        0        0    12449 2024-04-23 11:57:44.650683 nestipy_ioc-0.1.10/src/nestipy_ioc/container.py
+-rw-r--r--   0        0        0     1440 2024-04-22 13:59:48.684851 nestipy_ioc-0.1.10/src/nestipy_ioc/context_container.py
+-rw-r--r--   0        0        0      885 2024-04-22 14:30:34.353131 nestipy_ioc-0.1.10/src/nestipy_ioc/meta.py
+-rw-r--r--   0        0        0      877 2024-04-22 14:22:54.695299 nestipy_ioc-0.1.10/src/nestipy_ioc/provider.py
+-rw-r--r--   0        0        0       56 2024-04-22 13:59:03.116828 nestipy_ioc-0.1.10/src/nestipy_ioc/utils.py
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 nestipy_ioc-0.1.10/PKG-INFO
```

### Comparing `nestipy_ioc-0.1.0/src/nestipy_ioc/container.py` & `nestipy_ioc-0.1.10/src/nestipy_ioc/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,21 @@
         from .provider import ModuleProviderDict
         # extract global data from _service, not from module because all provider is already saved in _services of
         # container
         metadata: ClassMetadata = Reflect.get_metadata(service, ClassMetadata.Metadata, None)
         if metadata is not None:
             global_providers = cls.get_global_providers()
             providers, import_providers = metadata.get_service_providers()
-            return uniq([m.token if isinstance(m, ModuleProviderDict)
-                         else m for m in uniq(providers + global_providers + import_providers)])
+            uniq_providers = []
+            for m in uniq(providers + global_providers + import_providers):
+                if isinstance(m, ModuleProviderDict):
+                    uniq_providers.append(m.token)
+                else:
+                    uniq_providers.append(m)
+            return uniq(uniq_providers)
         # raise ValueError(f"Dependency Metadata not found  for {service.__name__} service ")
         return []
 
     def _resolve_context_service(self, name: str, dep_key: CtxDepKey, annotation: Union[Type, Any]):
         context_container = NestipyContextContainer.get_instance()
         match dep_key:
             case CtxDepKey.Request:
```

### Comparing `nestipy_ioc-0.1.0/src/nestipy_ioc/context_container.py` & `nestipy_ioc-0.1.10/src/nestipy_ioc/context_container.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.0/src/nestipy_ioc/meta.py` & `nestipy_ioc-0.1.10/src/nestipy_ioc/meta.py`

 * *Files identical despite different names*

### Comparing `nestipy_ioc-0.1.0/src/nestipy_ioc/provider.py` & `nestipy_ioc-0.1.10/src/nestipy_ioc/provider.py`

 * *Files identical despite different names*

