# Comparing `tmp/energyml_utils-1.0.0.tar.gz` & `tmp/energyml_utils-1.0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyml_utils-1.0.0.tar", max compression
+gzip compressed data, was "energyml_utils-1.0.1.dev4.tar", max compression
```

## Comparing `energyml_utils-1.0.0.tar` & `energyml_utils-1.0.1.dev4.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0    11338 2024-04-04 14:33:10.568410 energyml_utils-1.0.0/LICENSE
--rw-r--r--   0        0        0      855 2024-04-04 14:33:10.568410 energyml_utils-1.0.0/README.md
--rw-r--r--   0        0        0     3073 2024-04-04 14:33:41.101194 energyml_utils-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       74 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/__init__.py
--rw-r--r--   0        0        0      514 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/__init__.py
--rw-r--r--   0        0        0      281 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/__init__.py
--rw-r--r--   0        0        0     5895 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/hdf.py
--rw-r--r--   0        0        0    17632 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/helper.py
--rw-r--r--   0        0        0    19741 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/data/mesh.py
--rw-r--r--   0        0        0    22114 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/epc.py
--rw-r--r--   0        0        0    30269 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/introspection.py
--rw-r--r--   0        0        0     7655 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/manager.py
--rw-r--r--   0        0        0     2998 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/serialization.py
--rw-r--r--   0        0        0    13604 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/validation.py
--rw-r--r--   0        0        0     6411 2024-04-04 14:33:10.636412 energyml_utils-1.0.0/src/energyml/utils/xml.py
--rw-r--r--   0        0        0     2481 1970-01-01 00:00:00.000000 energyml_utils-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2024-04-23 08:18:57.182201 energyml_utils-1.0.1.dev4/LICENSE
+-rw-r--r--   0        0        0      855 2024-04-23 08:18:57.182201 energyml_utils-1.0.1.dev4/README.md
+-rw-r--r--   0        0        0     3075 2024-04-23 08:18:57.186201 energyml_utils-1.0.1.dev4/pyproject.toml
+-rw-r--r--   0        0        0       74 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/__init__.py
+-rw-r--r--   0        0        0      281 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/data/__init__.py
+-rw-r--r--   0        0        0     6750 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/data/hdf.py
+-rw-r--r--   0        0        0    22188 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/data/helper.py
+-rw-r--r--   0        0        0    20637 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/data/mesh.py
+-rw-r--r--   0        0        0    23244 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/epc.py
+-rw-r--r--   0        0        0      385 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/exception.py
+-rw-r--r--   0        0        0    31977 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/introspection.py
+-rw-r--r--   0        0        0     7801 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/manager.py
+-rw-r--r--   0        0        0     3443 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/serialization.py
+-rw-r--r--   0        0        0    13679 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/validation.py
+-rw-r--r--   0        0        0     6545 2024-04-23 08:18:57.194201 energyml_utils-1.0.1.dev4/src/energyml/utils/xml.py
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 energyml_utils-1.0.1.dev4/PKG-INFO
```

### Comparing `energyml_utils-1.0.0/LICENSE` & `energyml_utils-1.0.1.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `energyml_utils-1.0.0/README.md` & `energyml_utils-1.0.1.dev4/README.md`

 * *Files identical despite different names*

### Comparing `energyml_utils-1.0.0/pyproject.toml` & `energyml_utils-1.0.1.dev4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 # requires = ["setuptools"]
 # build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "energyml-utils"
-version = "1.0.0" # Set at build time
+version = "1.0.1.dev4" # Set at build time
 description = "Energyml helper"
 authors = [
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
 maintainers = [
     "Valentin Gauthier <valentin.gauthier@geosiris.com>"
 ]
@@ -45,36 +45,36 @@
 #[tool.pytest.ini_options]
 #pythonpath = [ "src" ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 xsdata = {version = "^24.0", extras = ["cli", "lxml"]}
 energyml-opc = "^1.12.0"
-energyml-common2-0 = "1.12.0"
-#energyml-common2-1 = "1.12.0"
-#energyml-common2-2 = "1.12.0"
-energyml-common2-3 = "1.12.0"
-energyml-resqml2-0-1 = "^1.12.0"
-#energyml-resqml2-2-dev3 = "^1.12.0"
-energyml-resqml2-2 = "^1.12.0"
-#energyml-witsml2-0 = "^1.12.0"
-#energyml-witsml2-1 = "^1.12.0"
-#energyml-prodml2-0 = "^1.12.0"
-#energyml-prodml2-2 = "^1.12.0"
 h5py = "^3.7.0"
 
 [tool.poetry.dev-dependencies]
 coverage = {extras = ["toml"], version = "^6.2"}
 pytest = "^8.1.1"
 pytest-cov = "^4.1.0"
 flake8 = "^4.0.0"
 black = "^22.3.0"
 pylint = "^2.7.2"
 click = ">=8.1.3, <=8.1.3" # upper version than 8.0.2 fail with black
 pdoc3 = "^0.10.0"
+energyml-common2-0 = "^1.12.0"
+energyml-common2-1 = "^1.12.0"
+energyml-common2-2 = "^1.12.0"
+energyml-common2-3 = "^1.12.0"
+energyml-resqml2-0-1 = "^1.12.0"
+energyml-resqml2-2-dev3 = "^1.12.0"
+energyml-resqml2-2 = "^1.12.0"
+energyml-witsml2-0 = "^1.12.0"
+energyml-witsml2-1 = "^1.12.0"
+energyml-prodml2-0 = "^1.12.0"
+energyml-prodml2-2 = "^1.12.0"
 
 [tool.coverage.run]
 branch = true
 source = ["src/energyml"]
 
 [tool.black]
 line-length = 79
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/__init__.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `energyml_utils-1.0.0/src/energyml/utils/data/hdf.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/data/hdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Copyright (c) 2023-2024 Geosiris.
 # SPDX-License-Identifier: Apache-2.0
+import os
 from dataclasses import dataclass
 from io import BytesIO
 from typing import Optional, List, Tuple, Any, Union
 
 import h5py
 
-from ..epc import Epc, get_obj_identifier, ObjectNotFoundNotException, \
-    EPCRelsRelationshipType
+from ..epc import Epc, get_obj_identifier, EPCRelsRelationshipType
 from ..introspection import search_attribute_matching_name_with_path, search_attribute_matching_name, \
-    get_obj_uuid, get_object_attribute
+    get_object_attribute, get_object_attribute_no_verif
 
 
 @dataclass
 class DatasetReader:
     def read_array(self, source: str, path_in_external_file: str) -> Optional[List[Any]]:
         return None
 
@@ -80,57 +80,41 @@
     """
     return search_attribute_matching_name_with_path(
         obj,
         "(PathInHdfFile|PathInExternalFile)"
     )
 
 
-def get_crs_obj(
-        context_obj: Any,
-        path_in_root: Optional[str] = None,
-        root_obj: Optional[Any] = None,
-        epc: Optional[Epc] = None
-) -> Optional[Any]:
-    """
-    Search for the CRS object related to :param:`context_obj` into the :param:`epc`
-    :param context_obj:
-    :param path_in_root:
-    :param root_obj:
-    :param epc:
-    :return:
+def get_h5_path_possibilities(value_in_xml: str, epc: Epc) -> List[str]:
     """
-    crs_list = search_attribute_matching_name(context_obj, r"\.*Crs", search_in_sub_obj=True, deep_search=False)
-    if crs_list is not None and len(crs_list) > 0:
-        crs = epc.get_object_by_identifier(get_obj_identifier(crs_list[0]))
-        if crs is None:
-            crs = epc.get_object_by_uuid(get_obj_uuid(crs_list[0]))
-        if crs is None:
-            raise ObjectNotFoundNotException(get_obj_identifier(crs_list[0]))
-        if crs is not None:
-            return crs
+    Maybe the path in the epc file objet was given as an absolute one : 'C:/my_file.h5'
+    but if the epc has been moved (e.g. in 'D:/a_folder/') it will not work. Thus, the function
+    energyml.utils.data.hdf.get_hdf5_path_from_external_path return the value from epc objet concatenate to the
+    real epc folder path.
+    With our example we will have : 'D:/a_folder/C:/my_file.h5'
+    this function returns (following our example):
+        [ 'C:/my_file.h5', 'D:/a_folder/my_file.h5', 'my_file.h5']
+    :param value_in_xml: 
+    :param epc: 
+    :return: 
+    """
+    epc_folder = epc.get_epc_file_folder()
+    hdf5_path_respect = value_in_xml
+    hdf5_path_rematch = f"{epc_folder+'/' if epc_folder is not None and len(epc_folder) else ''}{os.path.basename(value_in_xml)}"
+    hdf5_path_no_folder = f"{os.path.basename(value_in_xml)}"
 
-    if context_obj != root_obj:
-        upper_path = path_in_root[:path_in_root.rindex(".")]
-        if len(upper_path) > 0:
-            return get_crs_obj(
-                context_obj=get_object_attribute(root_obj, upper_path),
-                path_in_root=upper_path,
-                root_obj=root_obj,
-                epc=epc,
-            )
-
-    return None
+    return [hdf5_path_respect, hdf5_path_rematch, hdf5_path_no_folder]
 
 
 def get_hdf5_path_from_external_path(
         external_path_obj: Any,
         path_in_root: Optional[str] = None,
         root_obj: Optional[Any] = None,
         epc: Optional[Epc] = None
-) -> Optional[str]:
+) -> Optional[List[str]]:
     """
     Return the hdf5 file path (Searches for "uri" attribute or in :param:`epc` rels files).
     :param external_path_obj: can be an attribute of an ExternalDataArrayPart
     :param path_in_root:
     :param root_obj:
     :param epc:
     :return:
@@ -144,19 +128,41 @@
             root_obj=root_obj,
             epc=epc,
         )
     elif type(external_path_obj).__name__ == "ExternalDataArrayPart":
         epc_folder = epc.get_epc_file_folder()
         h5_uri = search_attribute_matching_name(external_path_obj, "uri")
         if h5_uri is not None and len(h5_uri) > 0:
-            return f"{epc_folder}/{h5_uri[0]}"
+            return get_h5_path_possibilities(value_in_xml=h5_uri[0], epc=epc)
+            # return f"{epc_folder}/{h5_uri[0]}"
     else:
         epc_folder = epc.get_epc_file_folder()
-        hdf_proxy = search_attribute_matching_name(external_path_obj, "HdfProxy")[0]
-        if hdf_proxy is not None:
+        hdf_proxy_lst = search_attribute_matching_name(external_path_obj, "HdfProxy")
+        ext_file_proxy_lst = search_attribute_matching_name(external_path_obj, "ExternalFileProxy")
+
+        # resqml 2.0.1
+        if hdf_proxy_lst is not None and len(hdf_proxy_lst) > 0:
+            hdf_proxy = hdf_proxy_lst
+            # print("h5Proxy", hdf_proxy)
+            while isinstance(hdf_proxy, list):
+                hdf_proxy = hdf_proxy[0]
             hdf_proxy_obj = epc.get_object_by_identifier(get_obj_identifier(hdf_proxy))
             if hdf_proxy_obj is not None:
                 for rel in epc.additional_rels.get(get_obj_identifier(hdf_proxy_obj), []):
-                    # print(f"\trel : {rel}")
                     if rel.type_value == EPCRelsRelationshipType.EXTERNAL_RESOURCE.get_type():
-                        return f"{epc_folder}/{rel.target}"
+                        return get_h5_path_possibilities(value_in_xml=rel.target, epc=epc)
+                        # return f"{epc_folder}/{rel.target}"
+
+        # resqml 2.2dev3
+        if ext_file_proxy_lst is not None and len(ext_file_proxy_lst) > 0:
+            ext_file_proxy = ext_file_proxy_lst
+            while isinstance(ext_file_proxy, list):
+                ext_file_proxy = ext_file_proxy[0]
+            ext_part_ref_obj = epc.get_object_by_identifier(
+                get_obj_identifier(
+                    get_object_attribute_no_verif(ext_file_proxy, "epc_external_part_reference")
+                )
+            )
+            return get_h5_path_possibilities(value_in_xml=ext_part_ref_obj.filename, epc=epc)
+            # return f"{epc_folder}/{ext_part_ref_obj.filename}"
+
     return None
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/data/helper.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/data/helper.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (c) 2023-2024 Geosiris.
 # SPDX-License-Identifier: Apache-2.0
 import inspect
 import sys
-from typing import Any, Optional, Callable, Literal, List, Union, Tuple
+from typing import Any, Optional, Callable, List, Union
 
-from .hdf import get_hdf5_path_from_external_path, HDF5FileReader, get_hdf_reference, get_crs_obj
+from .hdf import get_hdf5_path_from_external_path, HDF5FileReader, get_hdf_reference
 from ..epc import Epc, get_obj_identifier
+from ..exception import ObjectNotFoundNotError
 from ..introspection import snake_case, get_object_attribute_no_verif, \
     search_attribute_matching_name_with_path, search_attribute_matching_name, flatten_concatenation, \
-    search_attribute_in_upper_matching_name
+    search_attribute_in_upper_matching_name, get_obj_uuid, get_object_attribute
 
 _ARRAY_NAMES_ = [
     "BooleanArrayFromDiscretePropertyArray",
     "BooleanArrayFromIndexArray",
     "BooleanConstantArray",
     "BooleanExternalArray",
     "BooleanHdf5Array",
@@ -47,26 +48,198 @@
     "StringConstantArray",
     "StringExternalArray",
     "StringHdf5Array",
     "StringXmlArray"
 ]
 
 
-def get_array_reader_function(array_type_name: str) -> Optional[Callable]:
+def _point_as_array(point: Any) -> List:
     """
-    Returns the name of the potential appropriate function to read an object with type is named :param array_type_name
-    :param array_type_name: the initial type name
+    Transform a point that has "coordinate1", "coordinate2", "coordinate3" as attributes into a list.
+    :param point:
     :return:
     """
-    for name, obj in inspect.getmembers(sys.modules[__name__]):
-        if name == f"read_{snake_case(array_type_name)}":
-            return obj
+    return [
+        get_object_attribute_no_verif(point, "coordinate1"),
+        get_object_attribute_no_verif(point, "coordinate2"),
+        get_object_attribute_no_verif(point, "coordinate3"),
+    ]
+
+
+def is_z_reversed(crs: Optional[Any]) -> bool:
+    """
+    Returns True if the Z axe is reverse (ZIncreasingDownward=='True' or VerticalAxis.Direction=='down')
+    :param crs:
+    :return: By default, False is returned (if 'crs' is None)
+    """
+    reverse_z_values = False
+    if crs is not None:
+        # resqml 201
+        zincreasing_downward = search_attribute_matching_name(crs, "ZIncreasingDownward")
+        if len(zincreasing_downward) > 0:
+            reverse_z_values = zincreasing_downward[0]
+
+        # resqml >= 22
+        vert_axis = search_attribute_matching_name(crs, "VerticalAxis.Direction")
+        if len(vert_axis) > 0:
+            reverse_z_values = vert_axis[0].lower() == "down"
+
+    return reverse_z_values
+
+
+def prod_n_tab(val: Union[float, int, str], tab: List[Union[float, int, str]]):
+    """
+    Multiply every value of the list 'tab' by the constant 'val'
+    :param val:
+    :param tab:
+    :return:
+    """
+    return list(map(lambda x: x*val, tab))
+
+
+def sum_lists(l1: List, l2: List):
+    """
+    Sums 2 lists values.
+
+    Example:
+        [1,1,1] and [2,2,3,6] gives : [3,3,4,6]
+
+    :param l1:
+    :param l2:
+    :return:
+    """
+    return [l1[i] + l2[i] for i in range(min(len(l1), len(l2)))]+max(l1, l2, key=len)[min(len(l1), len(l2)):]
+
+
+#  _       __           __
+# | |     / /___  _____/ /___________  ____ _________
+# | | /| / / __ \/ ___/ //_/ ___/ __ \/ __ `/ ___/ _ \
+# | |/ |/ / /_/ / /  / ,< (__  ) /_/ / /_/ / /__/  __/
+# |__/|__/\____/_/  /_/|_/____/ .___/\__,_/\___/\___/
+#                            /_/
+
+class EnergymlWorkspace:
+    def get_object(self, uuid: str, object_version: Optional[str]) -> Optional[Any]:
+        raise NotImplementedError("EnergymlWorkspace.get_object")
+
+    def get_object_by_identifier(self, identifier: str) -> Optional[Any]:
+        _tmp = identifier.split(".")
+        return self.get_object(_tmp[0], _tmp[1] if len(_tmp) > 1 else None)
+
+    def get_object_by_uuid(self, uuid: str) -> Optional[Any]:
+        return self.get_object(uuid, None)
+
+    def read_external_array(
+            self,
+            energyml_array: Any,
+            root_obj: Optional[Any] = None,
+            path_in_root: Optional[str] = None,
+    ) -> List[Any]:
+        raise NotImplementedError("EnergymlWorkspace.get_object")
+
+
+class EPCWorkspace(EnergymlWorkspace):
+    def __init__(self, epc: Epc):
+        self.epc = epc
+
+    def get_object(self, uuid: str, object_version: Optional[str]) -> Optional[Any]:
+        return self.epc.get_object_by_identifier(f"{uuid}.{object_version}")
+
+    def read_external_array(
+            self,
+            energyml_array: Any,
+            root_obj: Optional[Any] = None,
+            path_in_root: Optional[str] = None,
+    ) -> List[Any]:
+        hdf5_paths = get_hdf5_path_from_external_path(
+            external_path_obj=energyml_array,
+            path_in_root=path_in_root,
+            root_obj=root_obj,
+            epc=self.epc,
+        )
+        h5_reader = HDF5FileReader()
+        path_in_external = get_hdf_reference(energyml_array)[0]
+
+        result_array = None
+        for hdf5_path in hdf5_paths:
+            try:
+                result_array = h5_reader.read_array(hdf5_path, path_in_external)
+                break  # if succeed, not try with other paths
+            except OSError as e:
+                pass
+
+        if result_array is None:
+            raise Exception(f"Failed to read h5 file. Paths tried : {hdf5_paths}")
+
+        # print(f"\tpath_in_root : {path_in_root}")
+        if path_in_root.lower().endswith("points") and len(result_array) > 0 and len(result_array[0]) == 3:
+            crs = get_crs_obj(
+                context_obj=energyml_array,
+                path_in_root=path_in_root,
+                root_obj=root_obj,
+                workspace=self,
+            )
+            zincreasing_downward = is_z_reversed(crs)
+            # print(f"\tzincreasing_downward : {zincreasing_downward}")
+
+            if zincreasing_downward:
+                result_array = list(map(lambda p: [p[0], p[1], -p[2]], result_array))
+
+        return result_array
+
+
+def get_crs_obj(
+        context_obj: Any,
+        path_in_root: Optional[str] = None,
+        root_obj: Optional[Any] = None,
+        workspace: Optional[EnergymlWorkspace] = None
+) -> Optional[Any]:
+    """
+    Search for the CRS object related to :param:`context_obj` into the :param:`workspace`
+    :param context_obj:
+    :param path_in_root:
+    :param root_obj:
+    :param workspace:
+    :return:
+    """
+    if workspace is None:
+        print("@get_crs_obj no Epc file given")
+    else:
+        crs_list = search_attribute_matching_name(context_obj, r"\.*Crs", search_in_sub_obj=True, deep_search=False)
+        if crs_list is not None and len(crs_list) > 0:
+            # print(crs_list[0])
+            crs = workspace.get_object_by_identifier(get_obj_identifier(crs_list[0]))
+            if crs is None:
+                crs = workspace.get_object_by_uuid(get_obj_uuid(crs_list[0]))
+            if crs is None:
+                raise ObjectNotFoundNotError(get_obj_identifier(crs_list[0]))
+            if crs is not None:
+                return crs
+
+        if context_obj != root_obj:
+            upper_path = path_in_root[:path_in_root.rindex(".")]
+            if len(upper_path) > 0:
+                return get_crs_obj(
+                    context_obj=get_object_attribute(root_obj, upper_path),
+                    path_in_root=upper_path,
+                    root_obj=root_obj,
+                    workspace=workspace,
+                )
+
     return None
 
 
+#     ___
+#    /   |  ______________ ___  _______
+#   / /| | / ___/ ___/ __ `/ / / / ___/
+#  / ___ |/ /  / /  / /_/ / /_/ (__  )
+# /_/  |_/_/  /_/   \__,_/\__, /____/
+#                        /____/
+
+
 def _array_name_mapping(array_type_name: str) -> str:
     """
     Transform the type name to match existing reader function
     :param array_type_name:
     :return:
     """
     array_type_name = array_type_name.replace("3D", "3d").replace("2D", "2d")
@@ -80,73 +253,106 @@
         return "JaggedArray"
     elif "Lattice" in array_type_name:
         if "Integer" in array_type_name or "Double" in array_type_name:
             return "int_double_lattice_array"
     return array_type_name
 
 
+def get_supported_array() -> List[str]:
+    """
+    Return a list of the supported arrays for the use of :py:func:`energyml.utils.data.helper.read_array` function.
+    :return:
+    """
+    return [x for x in _ARRAY_NAMES_ if get_array_reader_function(_array_name_mapping(x)) is not None]
+
+
+def get_not_supported_array():
+    """
+    Return a list of the NOT supported arrays for the use of :py:func:`energyml.utils.data.helper.read_array` function.
+    :return:
+    """
+    return [x for x in _ARRAY_NAMES_ if get_array_reader_function(_array_name_mapping(x)) is None]
+
+
+def read_external_array(
+        energyml_array: Any,
+        root_obj: Optional[Any] = None,
+        path_in_root: Optional[str] = None,
+        workspace: Optional[EnergymlWorkspace] = None
+) -> List[Any]:
+    """
+    Read an external array (BooleanExternalArray, BooleanHdf5Array, DoubleHdf5Array, IntegerHdf5Array, StringExternalArray ...)
+    :param energyml_array:
+    :param root_obj:
+    :param path_in_root:
+    :param workspace:
+    :return:
+    """
+    return workspace.read_external_array(
+        energyml_array=energyml_array,
+        root_obj=root_obj,
+        path_in_root=path_in_root,
+    )
+
+
+def get_array_reader_function(array_type_name: str) -> Optional[Callable]:
+    """
+    Returns the name of the potential appropriate function to read an object with type is named :param array_type_name
+    :param array_type_name: the initial type name
+    :return:
+    """
+    for name, obj in inspect.getmembers(sys.modules[__name__]):
+        if name == f"read_{snake_case(array_type_name)}":
+            return obj
+    return None
+
+
 def read_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List[Any]:
     """
     Read an array and return a list. The array is read depending on its type. see. :py:func:`energyml.utils.data.helper.get_supported_array`
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     if isinstance(energyml_array, list):
         return energyml_array
     array_type_name = _array_name_mapping(type(energyml_array).__name__)
 
     reader_func = get_array_reader_function(array_type_name)
     if reader_func is not None:
         return reader_func(
             energyml_array=energyml_array,
             root_obj=root_obj,
             path_in_root=path_in_root,
-            epc=epc,
+            workspace=workspace,
         )
     else:
         print(f"Type {array_type_name} is not supported: function read_{snake_case(array_type_name)} not found")
         raise Exception(f"Type {array_type_name} is not supported\n\t{energyml_array}: \n\tfunction read_{snake_case(array_type_name)} not found")
 
 
-def get_supported_array() -> List[str]:
-    """
-    Return a list of the supported arrays for the use of :py:func:`energyml.utils.data.helper.read_array` function.
-    :return:
-    """
-    return [x for x in _ARRAY_NAMES_ if get_array_reader_function(_array_name_mapping(x)) is not None]
-
-
-def get_not_supported_array():
-    """
-    Return a list of the NOT supported arrays for the use of :py:func:`energyml.utils.data.helper.read_array` function.
-    :return:
-    """
-    return [x for x in _ARRAY_NAMES_ if get_array_reader_function(_array_name_mapping(x)) is None]
-
-
 def read_constant_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List[Any]:
     """
     Read a constant array ( BooleanConstantArray, DoubleConstantArray, FloatingPointConstantArray, IntegerConstantArray ...)
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     # print(f"Reading constant array\n\t{energyml_array}")
 
     value = get_object_attribute_no_verif(energyml_array, "value")
     count = get_object_attribute_no_verif(energyml_array, "count")
 
@@ -155,116 +361,76 @@
     return [value for i in range(0, count)]
 
 
 def read_xml_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List[Any]:
     """
     Read a xml array ( BooleanXmlArray, FloatingPointXmlArray, IntegerXmlArray, StringXmlArray ...)
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     values = get_object_attribute_no_verif(energyml_array, "values")
     # count = get_object_attribute_no_verif(energyml_array, "count_per_value")
     return values
 
 
 def read_jagged_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List[Any]:
     """
     Read a jagged array
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     elements = read_array(
         energyml_array=get_object_attribute_no_verif(energyml_array, "elements"),
         root_obj=root_obj,
         path_in_root=path_in_root + ".elements",
-        epc=epc,
+        workspace=workspace,
     )
     cumulative_length = read_array(
         energyml_array=read_array(get_object_attribute_no_verif(energyml_array, "cumulative_length")),
         root_obj=root_obj,
         path_in_root=path_in_root + ".cumulative_length",
-        epc=epc,
+        workspace=workspace,
     )
 
     res = []
     previous = 0
     for cl in cumulative_length:
         res.append(elements[previous: cl])
         previous = cl
     return res
 
 
-def read_external_array(
-        energyml_array: Any,
-        root_obj: Optional[Any] = None,
-        path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
-) -> List[Any]:
-    """
-    Read an external array (BooleanExternalArray, BooleanHdf5Array, DoubleHdf5Array, IntegerHdf5Array, StringExternalArray ...)
-    :param energyml_array:
-    :param root_obj:
-    :param path_in_root:
-    :param epc:
-    :return:
-    """
-    hdf5_path = get_hdf5_path_from_external_path(
-                external_path_obj=energyml_array,
-                path_in_root=path_in_root,
-                root_obj=root_obj,
-                epc=epc,
-    )
-    h5_reader = HDF5FileReader()
-    path_in_external = get_hdf_reference(energyml_array)[0]
-
-    result_array = h5_reader.read_array(hdf5_path, path_in_external)
-
-    if path_in_root.lower().endswith("points") and len(result_array) > 0 and len(result_array[0]) == 3:
-        crs = get_crs_obj(
-            context_obj=energyml_array,
-            path_in_root=path_in_root,
-            root_obj=root_obj,
-            epc=epc,
-        )
-        zincreasing_downward = is_z_reversed(crs)
-
-        if zincreasing_downward:
-            result_array = list(map(lambda p: [p[0], p[1], -p[2]], result_array))
-
-    return result_array
-
-
 def read_int_double_lattice_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ):
     """
     Read DoubleLatticeArray or IntegerLatticeArray.
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     start_value = get_object_attribute_no_verif(energyml_array, "start_value")
     offset = get_object_attribute_no_verif(energyml_array, "offset")
 
     result = []
 
@@ -274,167 +440,127 @@
     #     pass
     # else:
     raise Exception(f"{type(energyml_array)} read with an offset of length {len(offset)} is not supported")
 
     # return result
 
 
-def _point_as_array(point: Any) -> List:
-    """
-    Transform a point that has "coordinate1", "coordinate2", "coordinate3" as attributes into a list.
-    :param point:
-    :return:
-    """
-    return [
-        get_object_attribute_no_verif(point, "coordinate1"),
-        get_object_attribute_no_verif(point, "coordinate2"),
-        get_object_attribute_no_verif(point, "coordinate3"),
-    ]
-
-
-def prod_n_tab(val: Union[float, int, str], tab: List[Union[float, int, str]]):
-    """
-    Multiply every value of the list 'tab' by the constant 'val'
-    :param val:
-    :param tab:
-    :return:
-    """
-    return list(map(lambda x: x*val, tab))
-
-
-def sum_lists(l1: List, l2: List):
-    """
-    Sums 2 lists values.
-
-    Example:
-        [1,1,1] and [2,2,3,6] gives : [3,3,4,6]
-
-    :param l1:
-    :param l2:
-    :return:
-    """
-    return [l1[i] + l2[i] for i in range(min(len(l1), len(l2)))]+max(l1, l2, key=len)[min(len(l1), len(l2)):]
-
-
 def read_point3d_zvalue_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ):
     """
     Read a Point3D2ValueArray
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     supporting_geometry = get_object_attribute_no_verif(energyml_array, "supporting_geometry")
     sup_geom_array = read_array(
         energyml_array=supporting_geometry,
         root_obj=root_obj,
         path_in_root=path_in_root + ".SupportingGeometry",
-        epc=epc,
+        workspace=workspace,
     )
 
     zvalues = get_object_attribute_no_verif(energyml_array, "zvalues")
     zvalues_array = flatten_concatenation(read_array(
         energyml_array=zvalues,
         root_obj=root_obj,
         path_in_root=path_in_root + ".ZValues",
-        epc=epc,
+        workspace=workspace,
     ))
 
     count = 0
 
     for i in range(len(sup_geom_array)):
         try:
             sup_geom_array[i][2] = zvalues_array[i]
         except Exception as e:
             if count == 0:
                 print(e, f": {i} is out of bound of {len(zvalues_array)}")
                 count = count + 1
 
     return sup_geom_array
 
-
 def read_point3d_from_representation_lattice_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ):
     """
     Read a Point3DFromRepresentationLatticeArray.
 
     Note: Only works for Grid2DRepresentation.
 
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     supporting_rep_identifier = get_obj_identifier(get_object_attribute_no_verif(energyml_array, "supporting_representation"))
-    print(f"energyml_array : {energyml_array}\n\t{supporting_rep_identifier}")
-    supporting_rep = epc.get_object_by_identifier(supporting_rep_identifier)
+    # print(f"energyml_array : {energyml_array}\n\t{supporting_rep_identifier}")
+    supporting_rep = workspace.get_object_by_identifier(supporting_rep_identifier)
 
     # TODO chercher un pattern \.*patch\.*.[d]+ pour trouver le numero du patch dans le path_in_root puis lire le patch
     # print(f"path_in_root {path_in_root}")
 
     result = []
     if "grid2d" in str(type(supporting_rep)).lower():
         patch_path, patch = search_attribute_matching_name_with_path(supporting_rep, "Grid2dPatch")[0]
         points = read_grid2d_patch(
             patch=patch,
             grid2d=supporting_rep,
             path_in_root=patch_path,
-            epc=epc,
+            workspace=workspace,
         )
         # TODO: take the points by there indices from the NodeIndicesOnSupportingRepresentation
         result = points
 
     else:
         raise Exception(f"Not supported type {type(energyml_array)} for object {type(root_obj)}")
     # pour trouver les infos qu'il faut
     return result
 
-
 def read_grid2d_patch(
         patch: Any,
         grid2d: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List:
     points_path, points_obj = search_attribute_matching_name_with_path(patch, "Geometry.Points")[0]
 
     return read_array(
         energyml_array=points_obj,
         root_obj=grid2d,
         path_in_root=path_in_root + points_path,
-        epc=epc,
+        workspace=workspace,
     )
 
-
 def read_point3d_lattice_array(
         energyml_array: Any,
         root_obj: Optional[Any] = None,
         path_in_root: Optional[str] = None,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List:
     """
     Read a Point3DLatticeArray.
 
     Note: If a CRS is found and its 'ZIncreasingDownward' is set to true or its
 
     :param energyml_array:
     :param root_obj:
     :param path_in_root:
-    :param epc:
+    :param workspace:
     :return:
     """
     result = []
     origin = _point_as_array(get_object_attribute_no_verif(energyml_array, "origin"))
     offset = get_object_attribute_no_verif(energyml_array, "offset")
 
     if len(offset) == 2:
@@ -455,39 +581,46 @@
             current_path=path_in_root,
         )
 
         crs = get_crs_obj(
             context_obj=energyml_array,
             path_in_root=path_in_root,
             root_obj=root_obj,
-            epc=epc,
+            workspace=workspace,
         )
         zincreasing_downward = is_z_reversed(crs)
 
         slowest_vec = _point_as_array(get_object_attribute_no_verif(slowest, "offset"))
         slowest_spacing = read_array(get_object_attribute_no_verif(slowest, "spacing"))
         slowest_table = list(map(lambda x: prod_n_tab(x, slowest_vec), slowest_spacing))
 
         fastest_vec = _point_as_array(get_object_attribute_no_verif(fastest, "offset"))
         fastest_spacing = read_array(get_object_attribute_no_verif(fastest, "spacing"))
         fastest_table = list(map(lambda x: prod_n_tab(x, fastest_vec), fastest_spacing))
 
         slowest_size = len(slowest_table)
         fastest_size = len(fastest_table)
 
-        if len(crs_sa_count) > 0 and len(crs_fa_count) and crs_sa_count[0] == fastest_size:
-            print("reversing order")
-            # if offset were given in the wrong order
-            tmp_table = slowest_table
-            slowest_table = fastest_table
-            fastest_table = tmp_table
-
-            tmp_size = slowest_size
-            slowest_size = fastest_size
-            fastest_size = tmp_size
+        if len(crs_sa_count) > 0 and len(crs_fa_count) > 0:
+            if (
+                    (crs_sa_count[0] == fastest_size and crs_fa_count[0] == slowest_size)
+                    or (crs_sa_count[0] == fastest_size - 1 and crs_fa_count[0] == slowest_size - 1)
+            ):
+                print("reversing order")
+                # if offset were given in the wrong order
+                tmp_table = slowest_table
+                slowest_table = fastest_table
+                fastest_table = tmp_table
+
+                tmp_size = slowest_size
+                slowest_size = fastest_size
+                fastest_size = tmp_size
+            else:
+                slowest_size = crs_sa_count[0]
+                fastest_size = crs_fa_count[0]
 
         for i in range(slowest_size):
             for j in range(fastest_size):
                 previous_value = origin
                 # to avoid a sum of the parts of the array at each iteration, I take the previous value in the same line
                 # number i and add the fastest_table[j] value
 
@@ -513,35 +646,14 @@
                         result.append(previous_value)
     else:
         raise Exception(f"{type(energyml_array)} read with an offset of length {len(offset)} is not supported")
 
     return result
 
 
-def is_z_reversed(crs: Optional[Any]) -> bool:
-    """
-    Returns True if the Z axe is reverse (ZIncreasingDownward=='True' or VerticalAxis.Direction=='down')
-    :param crs:
-    :return: By default, False is returned (if 'crs' is None)
-    """
-    reverse_z_values = False
-    if crs is not None:
-        # resqml 201
-        zincreasing_downward = search_attribute_matching_name(crs, "ZIncreasingDownward")
-        if len(zincreasing_downward) > 0:
-            reverse_z_values = zincreasing_downward[0]
-
-        # resqml >= 22
-        vert_axis = search_attribute_matching_name(crs, "VerticalAxis.Direction")
-        if len(vert_axis) > 0:
-            reverse_z_values = vert_axis[0].lower() == "down"
-
-    return reverse_z_values
-
-
 # def read_boolean_constant_array(
 #         energyml_array: Any,
 #         root_obj: Optional[Any] = None,
 #         path_in_root: Optional[str] = None,
-#         epc: Optional[Epc] = None
+#         workspace: Optional[EnergymlWorkspace] = None
 # ):
 #     print(energyml_array)
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/data/mesh.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/data/mesh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 # Copyright (c) 2023-2024 Geosiris.
 # SPDX-License-Identifier: Apache-2.0
 import inspect
+import os
 import re
 import sys
 from dataclasses import dataclass, field
+from enum import Enum
 from io import BytesIO
 from typing import List, Optional, Any, Callable
 
-from .hdf import get_hdf_reference_with_path, \
-    get_hdf5_path_from_external_path, HDF5FileReader, get_crs_obj
-from .helper import read_array, read_grid2d_patch, is_z_reversed
-from ..epc import Epc, get_obj_identifier
+from .hdf import HDF5FileReader
+from .helper import read_array, read_grid2d_patch, is_z_reversed, EnergymlWorkspace, get_crs_obj, EPCWorkspace
+from ..epc import Epc, get_obj_identifier, gen_energyml_object_path
 from ..introspection import search_attribute_matching_name, \
-    search_attribute_matching_type_with_path, \
-    search_attribute_matching_name_with_path, snake_case
+    search_attribute_matching_name_with_path, snake_case, get_object_attribute
 
 _FILE_HEADER: bytes = b"# file exported by energyml-utils python module (Geosiris)\n"
 
 Point = list[float]
 
 
+class MeshFileFormat(Enum):
+    OFF = "off"
+    OBJ = "obj"
+
+
 @dataclass
 class AbstractMesh:
     energyml_object: Any = field(
         default=None
     )
 
     crs_object: Any = field(
@@ -104,197 +109,218 @@
     """
     Transform the type name to match existing reader function
     :param array_type_name:
     :return:
     """
     array_type_name = array_type_name.replace("3D", "3d").replace("2D", "2d")
     array_type_name = re.sub("^[Oo]bj([A-Z])", r"\1", array_type_name)
+    array_type_name = re.sub("(Polyline|Point)Set", r"\1", array_type_name)
     return array_type_name
 
 
 def read_mesh_object(
         energyml_object: Any,
-        epc: Optional[Epc] = None
+        workspace: Optional[EnergymlWorkspace] = None
 ) -> List[AbstractMesh]:
     """
     Read and "meshable" object. If :param:`energyml_object` is not supported, an exception will be raised.
     :param energyml_object:
-    :param epc:
+    :param workspace:
     :return:
     """
     if isinstance(energyml_object, list):
         return energyml_object
     array_type_name = _mesh_name_mapping(type(energyml_object).__name__)
 
     reader_func = get_mesh_reader_function(array_type_name)
     if reader_func is not None:
         return reader_func(
             energyml_object=energyml_object,
-            epc=epc,
+            workspace=workspace,
         )
     else:
         print(f"Type {array_type_name} is not supported: function read_{snake_case(array_type_name)} not found")
-        raise Exception(f"Type {array_type_name} is not supported\n\t{energyml_object}: \n\tfunction read_{snake_case(array_type_name)} not found")
+        raise Exception(
+            f"Type {array_type_name} is not supported\n\t{energyml_object}: \n\tfunction read_{snake_case(array_type_name)} not found")
 
 
-def read_point_set_representation(energyml_object: Any, epc: Epc) -> List[PointSetMesh]:
+def read_point_representation(energyml_object: Any, workspace: EnergymlWorkspace) -> List[PointSetMesh]:
     # pt_geoms = search_attribute_matching_type(point_set, "AbstractGeometry")
     h5_reader = HDF5FileReader()
 
     meshes = []
-    for refer_path, refer_value in get_hdf_reference_with_path(energyml_object):
-        try:
-            hdf5_path = get_hdf5_path_from_external_path(
-                external_path_obj=refer_value,
-                path_in_root=refer_path,
-                root_obj=energyml_object,
-                epc=epc,
-            )
-            crs = get_crs_obj(
-                context_obj=refer_value,
-                path_in_root=refer_path,
-                root_obj=energyml_object,
-                epc=epc,
-            )
-            if hdf5_path is not None:
-                print(f"Reading h5 file : {hdf5_path}")
-                meshes.append(PointSetMesh(
-                    identifier=refer_value,
-                    energyml_object=energyml_object,
-                    crs_object=crs,
-                    point_list=h5_reader.read_array(hdf5_path, refer_value)
-                ))
-        except Exception as e:
-            print(f"Error with path {refer_path} -- {energyml_object}")
-            raise e
+
+    patch_idx = 0
+    # resqml 2.0.1
+    for points_path_in_obj, points_obj in search_attribute_matching_name_with_path(energyml_object,
+                                                                                   "NodePatch.[\d]+.Geometry.Points"):
+        points = read_array(
+            energyml_array=points_obj,
+            root_obj=energyml_object,
+            path_in_root=points_path_in_obj,
+            workspace=workspace,
+        )
+
+        crs = get_crs_obj(
+            context_obj=points_obj,
+            path_in_root=points_path_in_obj,
+            root_obj=energyml_object,
+            workspace=workspace,
+        )
+        if points is not None:
+            meshes.append(PointSetMesh(
+                identifier=f"NodePatch num {patch_idx}",
+                energyml_object=energyml_object,
+                crs_object=crs,
+                point_list=points
+            ))
+
+        patch_idx = patch_idx + 1
+
+    # resqml 2.2
+    for points_path_in_obj, points_obj in search_attribute_matching_name_with_path(energyml_object,
+                                                                                   "NodePatchGeometry.[\d]+.Points"):
+        points = read_array(
+            energyml_array=points_obj,
+            root_obj=energyml_object,
+            path_in_root=points_path_in_obj,
+            workspace=workspace,
+        )
+
+        crs = get_crs_obj(
+            context_obj=points_obj,
+            path_in_root=points_path_in_obj,
+            root_obj=energyml_object,
+            workspace=workspace,
+        )
+        if points is not None:
+            meshes.append(PointSetMesh(
+                identifier=f"NodePatchGeometry num {patch_idx}",
+                energyml_object=energyml_object,
+                crs_object=crs,
+                point_list=points
+            ))
+
+        patch_idx = patch_idx + 1
+
     return meshes
 
 
-def read_polyline_set_representation(energyml_object: Any, epc: Epc) -> List[PointSetMesh]:
+def read_polyline_representation(energyml_object: Any, workspace: EnergymlWorkspace) -> List[PolylineSetMesh]:
     # pt_geoms = search_attribute_matching_type(point_set, "AbstractGeometry")
     h5_reader = HDF5FileReader()
 
     meshes = []
 
     patch_idx = 0
-    for path_path_in_obj, patch in search_attribute_matching_name_with_path(energyml_object, "LinePatch"):
-        print(f"patch {patch}")
-        geometry_path_in_obj, geometry = search_attribute_matching_name_with_path(patch, "geometry")[0]
-        node_count_per_poly_path_in_obj, node_count_per_poly = \
-        search_attribute_matching_name_with_path(patch, "NodeCountPerPolyline")[0]
-        points_ext_array = search_attribute_matching_type_with_path(geometry, "ExternalDataArrayPart|Hdf5Dataset")
-        node_count_ext_array = search_attribute_matching_type_with_path(node_count_per_poly,
-                                                                        "ExternalDataArrayPart|Hdf5Dataset")
-
-        if len(points_ext_array) > 0:
-            point_per_elt = []
-            point_indices = []
-            crs = None
-
-            # Reading points
-            for patch_part_path, patchPart_value in points_ext_array:
-                patch_part_full_path_in_obj = path_path_in_obj + geometry_path_in_obj + patch_part_path
-                for refer_path, refer_value in get_hdf_reference_with_path(patchPart_value):
-                    print(f"refer_path {patch_part_full_path_in_obj}{refer_path} refer_value{refer_value} ")
-                    hdf5_path = get_hdf5_path_from_external_path(
-                        external_path_obj=refer_value,
-                        path_in_root=patch_part_full_path_in_obj + refer_path,
-                        root_obj=energyml_object,
-                        epc=epc,
-                    )
-                    crs = get_crs_obj(
-                        context_obj=refer_value,
-                        path_in_root=patch_part_full_path_in_obj + refer_path,
-                        root_obj=energyml_object,
-                        epc=epc,
-                    )
-                    if hdf5_path is not None:
-                        print(f"Reading h5 file : {hdf5_path}")
-                        point_per_elt = point_per_elt + h5_reader.read_array(hdf5_path, refer_value)
-
-            # Reading polyline indices
-            # for patch_part_path, patchPart_value in node_count_ext_array:
-            #     patch_part_full_path_in_obj = path_path_in_obj + node_count_per_poly_path_in_obj + patch_part_path
-            #     for refer_path, refer_value in get_hdf_reference_with_path(patchPart_value):
-            #         print(f"refer_path: {patch_part_full_path_in_obj}{refer_path} refer_value: {refer_value} ")
-            #         hdf5_path = get_hdf5_path_from_external_path(
-            #                     external_path_obj=refer_value,
-            #                     path_in_root=patch_part_full_path_in_obj + refer_path,
-            #                     root_obj=energyml_object,
-            #                     epc=epc,
-            #         )
-            #         if hdf5_path is not None:
-            #             node_counts_list = h5_reader.read_array(hdf5_path, refer_value)
-            #             idx = 0
-            #             for nb_node in node_counts_list:
-            #                 point_indices.append([x for x in range(idx, idx + nb_node)])
-            #                 idx = idx + nb_node
+    for patch_path_in_obj, patch in (
+            search_attribute_matching_name_with_path(energyml_object, "NodePatch")
+            + search_attribute_matching_name_with_path(energyml_object, "LinePatch.[\\d]+")
+    ):
+        points_path, points_obj = search_attribute_matching_name_with_path(patch, "Geometry.Points")[0]
+        points = read_array(
+            energyml_array=points_obj,
+            root_obj=energyml_object,
+            path_in_root=patch_path_in_obj + points_path,
+            workspace=workspace,
+        )
+
+        crs = get_crs_obj(
+            context_obj=points_obj,
+            path_in_root=patch_path_in_obj + points_path,
+            root_obj=energyml_object,
+            workspace=workspace,
+        )
 
+        close_poly = None
+        try:
+            close_poly_path, close_poly_obj = search_attribute_matching_name_with_path(patch, "ClosedPolylines")[0]
+            close_poly = read_array(
+                energyml_array=close_poly_obj,
+                root_obj=energyml_object,
+                path_in_root=patch_path_in_obj + close_poly_path,
+                workspace=workspace,
+            )
+        except IndexError:
+            pass
+
+        point_indices = []
+        try:
+            node_count_per_poly_path_in_obj, node_count_per_poly = \
+                search_attribute_matching_name_with_path(patch, "NodeCountPerPolyline")[0]
             node_counts_list = read_array(
                 energyml_array=node_count_per_poly,
                 root_obj=energyml_object,
-                path_in_root=path_path_in_obj + node_count_per_poly_path_in_obj,
-                epc=epc,
+                path_in_root=patch_path_in_obj + node_count_per_poly_path_in_obj,
+                workspace=workspace,
             )
             idx = 0
+            poly_idx = 0
             for nb_node in node_counts_list:
                 point_indices.append([x for x in range(idx, idx + nb_node)])
+                if close_poly is not None and len(close_poly) > poly_idx and close_poly[poly_idx]:
+                    point_indices[len(point_indices) - 1].append(idx)
                 idx = idx + nb_node
+                poly_idx = poly_idx + 1
+        except IndexError:
+            # No NodeCountPerPolyline for Polyline but only in PolylineSet
+            pass
+
+        if point_indices is None or len(point_indices) == 0:
+            # No indices ==> all point in the polyline
+            point_indices = [list(range(len(points)))]
+
+        if len(points) > 0:
+            meshes.append(PolylineSetMesh(
+                identifier=f"{get_obj_identifier(energyml_object)}_patch{patch_idx}",
+                energyml_object=energyml_object,
+                crs_object=crs,
+                point_list=points,
+                line_indices=point_indices
+            ))
 
-            if len(point_per_elt) > 0:
-                # poly_idx = 0
-                # for single_poly_indices in point_indices:
-                meshes.append(PolylineSetMesh(
-                    # identifier=f"{get_obj_identifier(energyml_object)}_patch{patch_idx}_poly{poly_idx}",
-                    identifier=f"{get_obj_identifier(energyml_object)}_patch{patch_idx}",
-                    energyml_object=energyml_object,
-                    crs_object=crs,
-                    point_list=point_per_elt,
-                    line_indices=point_indices
-                ))
-                # poly_idx = poly_idx + 1
         patch_idx = patch_idx + 1
 
     return meshes
 
 
-def read_grid2d_representation(energyml_object: Any, epc: Epc, keep_holes=False) -> List[SurfaceMesh]:
+def read_grid2d_representation(energyml_object: Any, workspace: Optional[EnergymlWorkspace] = None, keep_holes=False) -> List[SurfaceMesh]:
     # h5_reader = HDF5FileReader()
     meshes = []
 
     patch_idx = 0
     for patch_path, patch in search_attribute_matching_name_with_path(energyml_object, "Grid2dPatch"):
         crs = get_crs_obj(
             context_obj=patch,
             path_in_root=patch_path,
             root_obj=energyml_object,
-            epc=epc,
+            workspace=workspace,
         )
 
         reverse_z_values = is_z_reversed(crs)
 
         points = read_grid2d_patch(
             patch=patch,
             grid2d=energyml_object,
             path_in_root=patch_path,
-            epc=epc,
+            workspace=workspace,
         )
 
         fa_count = search_attribute_matching_name(patch, "FastestAxisCount")
         if fa_count is None:
             fa_count = search_attribute_matching_name(energyml_object, "FastestAxisCount")
 
         sa_count = search_attribute_matching_name(patch, "SlowestAxisCount")
         if sa_count is None:
             sa_count = search_attribute_matching_name(energyml_object, "SlowestAxisCount")
 
         fa_count = fa_count[0]
         sa_count = sa_count[0]
 
-        print(f"sa_count {sa_count} fa_count {fa_count}")
+        # print(f"sa_count {sa_count} fa_count {fa_count}")
 
         points_no_nan = []
 
         indice_to_final_indice = {}
         if keep_holes:
             for i in range(len(points)):
                 p = points[i]
@@ -309,48 +335,48 @@
                     if reverse_z_values:
                         points[i][2] = - points[i][2]
                     indice_to_final_indice[i] = len(points_no_nan)
                     points_no_nan.append(p)
 
         indices = []
 
-        while sa_count*fa_count > len(points):
+        while sa_count * fa_count > len(points):
             sa_count = sa_count - 1
             fa_count = fa_count - 1
 
-        while sa_count*fa_count < len(points):
+        while sa_count * fa_count < len(points):
             sa_count = sa_count + 1
             fa_count = fa_count + 1
 
-        print(f"sa_count {sa_count} fa_count {fa_count} : {sa_count*fa_count} - {len(points)} ")
+        # print(f"sa_count {sa_count} fa_count {fa_count} : {sa_count*fa_count} - {len(points)} ")
 
-        for sa in range(sa_count-1):
-            for fa in range(fa_count-1):
+        for sa in range(sa_count - 1):
+            for fa in range(fa_count - 1):
                 line = sa * fa_count
-                if sa+1 == int(sa_count / 2) and fa == int(fa_count / 2):
-                    print(
-                        "\n\t", (line + fa), " : ", (line + fa) in indice_to_final_indice,
-                        "\n\t", (line + fa + 1), " : ", (line + fa + 1) in indice_to_final_indice,
-                        "\n\t", (line + fa_count + fa + 1), " : ", (line + fa_count + fa + 1) in indice_to_final_indice,
-                        "\n\t", (line + fa_count + fa), " : ", (line + fa_count + fa) in indice_to_final_indice,
-                    )
+                # if sa+1 == int(sa_count / 2) and fa == int(fa_count / 2):
+                #     print(
+                #         "\n\t", (line + fa), " : ", (line + fa) in indice_to_final_indice,
+                #         "\n\t", (line + fa + 1), " : ", (line + fa + 1) in indice_to_final_indice,
+                #         "\n\t", (line + fa_count + fa + 1), " : ", (line + fa_count + fa + 1) in indice_to_final_indice,
+                #         "\n\t", (line + fa_count + fa), " : ", (line + fa_count + fa) in indice_to_final_indice,
+                #     )
                 if keep_holes:
                     indices.append(
                         [
                             line + fa,
                             line + fa + 1,
                             line + fa_count + fa + 1,
                             line + fa_count + fa,
                         ]
                     )
                 elif (
-                    (line + fa) in indice_to_final_indice
-                    and (line + fa + 1) in indice_to_final_indice
-                    and (line + fa_count + fa + 1) in indice_to_final_indice
-                    and (line + fa_count + fa) in indice_to_final_indice
+                        (line + fa) in indice_to_final_indice
+                        and (line + fa + 1) in indice_to_final_indice
+                        and (line + fa_count + fa + 1) in indice_to_final_indice
+                        and (line + fa_count + fa) in indice_to_final_indice
                 ):
                     indices.append(
                         [
                             indice_to_final_indice[line + fa],
                             indice_to_final_indice[line + fa + 1],
                             indice_to_final_indice[line + fa_count + fa + 1],
                             indice_to_final_indice[line + fa_count + fa],
@@ -365,43 +391,43 @@
             faces_indices=indices
         ))
         patch_idx = patch_idx + 1
 
     return meshes
 
 
-def read_triangulated_set_representation(energyml_object: Any, epc: Epc) -> List[SurfaceMesh]:
+def read_triangulated_set_representation(energyml_object: Any, workspace: EnergymlWorkspace) -> List[SurfaceMesh]:
     meshes = []
 
     point_offset = 0
     patch_idx = 0
     for patch_path, patch in search_attribute_matching_name_with_path(energyml_object, "\\.*Patch"):
         crs = get_crs_obj(
             context_obj=patch,
             path_in_root=patch_path,
             root_obj=energyml_object,
-            epc=epc,
+            workspace=workspace,
         )
 
         point_list: List[Point] = []
         for point_path, point_obj in search_attribute_matching_name_with_path(patch, "Geometry.Points"):
             point_list = point_list + read_array(
                 energyml_array=point_obj,
                 root_obj=energyml_object,
                 path_in_root=patch_path + point_path,
-                epc=epc,
+                workspace=workspace,
             )
 
         triangles_list: List[List[int]] = []
         for triangles_path, triangles_obj in search_attribute_matching_name_with_path(patch, "Triangles"):
             triangles_list = triangles_list + read_array(
                 energyml_array=triangles_obj,
                 root_obj=energyml_object,
                 path_in_root=patch_path + triangles_path,
-                epc=epc,
+                workspace=workspace,
             )
         triangles_list = list(map(lambda tr: [ti - point_offset for ti in tr], triangles_list))
         meshes.append(SurfaceMesh(
             identifier=f"{get_obj_identifier(energyml_object)}_patch{patch_idx}",
             energyml_object=energyml_object,
             crs_object=crs,
             point_list=point_list,
@@ -532,19 +558,58 @@
     for p in points:
         if len(p) > 0:
             off_point_part.write(f"v {' '.join(list(map(lambda xyz: str(xyz), p)))}\n".encode('utf-8'))
 
     # cpt = 0
     for face in indices:
         if len(face) > 1:
-            # off_face_part.write(f"{elt_letter} ".encode('utf-8'))
-            # for pi in face:
-            #     off_face_part.write(f"{pi + point_offset} ".encode('utf-8'))
             off_point_part.write(
                 f"{elt_letter} {' '.join(list(map(lambda x: str(x + point_offset + offset_obj), face)))}\n".encode(
                     'utf-8'))
 
             # if colors is not None and len(colors) > cpt and colors[cpt] is not None and len(colors[cpt]) > 0:
             #     for col in colors[cpt]:
             #         off_face_part.write(f"{col} ".encode('utf-8'))
 
             # off_face_part.write(b"\n")
+
+
+def export_multiple_data(
+        epc_path: str,
+        uuid_list: List[str],
+        output_folder_path: str,
+        output_file_path_suffix: str = "",
+        file_format: MeshFileFormat = MeshFileFormat.OBJ
+):
+    epc = Epc.read_file(epc_path)
+
+    try:
+        os.makedirs(output_folder_path, exist_ok=True)
+    except OSError:
+        pass
+
+    for uuid in uuid_list:
+        energyml_obj = epc.get_object_by_uuid(uuid)[0]
+        file_name = (f"{gen_energyml_object_path(energyml_obj)}_"
+                     f"[{get_object_attribute(energyml_obj, 'citation.title')}]"
+                     f"{output_file_path_suffix}"
+                     f".{file_format.value}")
+        file_path = f"{output_folder_path}/{file_name}"
+        print(f"Exporting : {file_path}")
+        mesh_list = read_mesh_object(
+            energyml_object=energyml_obj,
+            workspace=EPCWorkspace(epc=epc),
+        )
+        if file_format == MeshFileFormat.OBJ:
+            with open(file_path, "wb") as f:
+                export_obj(
+                    mesh_list=mesh_list,
+                    out=f,
+                )
+        elif file_format == MeshFileFormat.OFF:
+            with open(file_path, "wb") as f:
+                export_off(
+                    mesh_list=mesh_list,
+                    out=f,
+                )
+        else:
+            print(f"Code is not written for format {file_format}")
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/epc.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/epc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,56 +1,41 @@
 # Copyright (c) 2023-2024 Geosiris.
 # SPDX-License-Identifier: Apache-2.0
 """
-This example module shows various types of documentation available for use
-with pydoc.  To generate HTML documentation for this module issue the
-command:
-
-    pydoc -w foo
-
+This module contains utilities to read/write EPC files.
 """
 
 import datetime
 import re
 import zipfile
 from dataclasses import dataclass, field
 from enum import Enum
 from io import BytesIO
 from typing import List, Any, Union, Dict, Callable, Optional, Tuple
 
-from energyml.opc.opc import CoreProperties, Relationships, Types, Default, Relationship, Override
-from xsdata.exceptions import ParserError
+from energyml.opc.opc import CoreProperties, Relationships, Types, Default, Relationship, Override, Created, Creator, \
+    Identifier, Keywords1
 from xsdata.formats.dataclass.models.generics import DerivedElement
 
 from .introspection import (
     get_class_from_content_type,
     get_obj_type, search_attribute_matching_type, get_obj_version, get_obj_uuid,
-    get_object_type_for_file_path_from_class, get_content_type_from_class, get_direct_dor_list
+    get_object_type_for_file_path_from_class, get_content_type_from_class, get_direct_dor_list, epoch_to_date, epoch,
+    gen_uuid
 )
 from .manager import get_class_pkg, get_class_pkg_version
 from .serialization import (
-    serialize_xml, read_energyml_xml_str, read_energyml_xml_bytes, read_energyml_xml_bytes_as_class
+    serialize_xml, read_energyml_xml_str, read_energyml_xml_bytes
 )
 from .xml import is_energyml_content_type
 
 RELS_CONTENT_TYPE = "application/vnd.openxmlformats-package.core-properties+xml"
 RELS_FOLDER_NAME = "_rels"
 
 
-class NoCrsException(Exception):
-    pass
-
-
-@dataclass
-class ObjectNotFoundNotException(Exception):
-    obj_id: str = field(
-        default=None
-    )
-
-
 class EpcExportVersion(Enum):
     """EPC export version."""
     #: Classical export
     CLASSIC = 1
     #: Export with objet path sorted by package (eml/resqml/witsml/prodml)
     EXPANDED = 2
 
@@ -70,31 +55,35 @@
     #: The object in Target is a media representation for the current object. As a guideline, media files
     #: should be stored in a "media" folder in the ROOT of the package.
     DestinationMedia = "destinationMedia"
     #: The current object is a media representation for the object in Target.
     SOURCE_MEDIA = "sourceMedia"
     #: The target is part of a larger data object that has been chunked into several smaller files
     CHUNKED_PART = "chunkedPart"
+    #: The core properties
+    CORE_PROPERTIES = "core-properties"
     #: /!\ not in the norm
     EXTENDED_CORE_PROPERTIES = "extended-core-properties"
 
     def get_type(self) -> str:
         match self:
             case EPCRelsRelationshipType.EXTENDED_CORE_PROPERTIES:
                 return "http://schemas.f2i-consulting.com/package/2014/relationships/" + str(self.value)
+            case EPCRelsRelationshipType.CORE_PROPERTIES:
+                return "http://schemas.openxmlformats.org/package/2006/relationships/metadata/" + str(self.value)
             case (
-            EPCRelsRelationshipType.CHUNKED_PART
-            | EPCRelsRelationshipType.DESTINATION_OBJECT
-            | EPCRelsRelationshipType.SOURCE_OBJECT
-            | EPCRelsRelationshipType.ML_TO_EXTERNAL_PART_PROXY
-            | EPCRelsRelationshipType.EXTERNAL_PART_PROXY_TO_ML
-            | EPCRelsRelationshipType.EXTERNAL_RESOURCE
-            | EPCRelsRelationshipType.DestinationMedia
-            | EPCRelsRelationshipType.SOURCE_MEDIA
-            | _
+                EPCRelsRelationshipType.CHUNKED_PART
+                | EPCRelsRelationshipType.DESTINATION_OBJECT
+                | EPCRelsRelationshipType.SOURCE_OBJECT
+                | EPCRelsRelationshipType.ML_TO_EXTERNAL_PART_PROXY
+                | EPCRelsRelationshipType.EXTERNAL_PART_PROXY_TO_ML
+                | EPCRelsRelationshipType.EXTERNAL_RESOURCE
+                | EPCRelsRelationshipType.DestinationMedia
+                | EPCRelsRelationshipType.SOURCE_MEDIA
+                | _
             ):
                 return "http://schemas.energistics.org/package/2012/relationships/" + str(self.value)
 
 
 @dataclass
 class RawFile:
     path: str = field(default="_")
@@ -147,15 +136,15 @@
         default=None
     )
 
     def __str__(self):
         return (
                 "EPC file (" + str(self.export_version) + ") "
                 + f"{len(self.energyml_objects)} energyml objects and {len(self.raw_files)} other files {[f.path for f in self.raw_files]}"
-                # + f"\n{[serialize_json(ar) for ar in self.additional_rels]}"
+            # + f"\n{[serialize_json(ar) for ar in self.additional_rels]}"
         )
 
     # EXPORT functions
 
     def gen_opc_content_type(self) -> Types:
         """
         Generates a :class:`Types` instance and fill it with energyml objects :class:`Override` values
@@ -199,39 +188,50 @@
         """
         Export the epc file into a :class:`BytesIO` instance. The result is an 'in-memory' zip file.
         :return:
         """
         zip_buffer = BytesIO()
 
         with zipfile.ZipFile(zip_buffer, "a", zipfile.ZIP_DEFLATED, False) as zip_file:
+            # CoreProps
+            if self.core_props is None:
+                self.core_props = CoreProperties(
+                    created=Created(any_element=epoch_to_date(epoch())),
+                    creator=Creator(any_element="energyml-utils python module (Geosiris)"),
+                    identifier=Identifier(any_element=f"urn:uuid:{gen_uuid()}"),
+                    keywords=Keywords1(
+                        lang="en",
+                        content=["generated;Geosiris;python;energyml-utils"]
+                    ),
+                    version="1.0"
+                )
+
+            zip_info_core = zipfile.ZipInfo(filename=gen_core_props_path(self.export_version),
+                                       date_time=datetime.datetime.now().timetuple()[:6])
+            data = serialize_xml(self.core_props)
+            zip_file.writestr(zip_info_core, data)
+
             #  Energyml objects
             for e_obj in self.energyml_objects:
                 e_path = gen_energyml_object_path(e_obj, self.export_version)
                 zip_info = zipfile.ZipInfo(filename=e_path, date_time=datetime.datetime.now().timetuple()[:6])
                 data = serialize_xml(e_obj)
                 zip_file.writestr(zip_info, data)
 
             # Rels
             for rels_path, rels in self.compute_rels().items():
                 zip_info = zipfile.ZipInfo(filename=rels_path, date_time=datetime.datetime.now().timetuple()[:6])
                 data = serialize_xml(rels)
                 zip_file.writestr(zip_info, data)
 
-            # CoreProps
-            if self.core_props is not None:
-                zip_info = zipfile.ZipInfo(filename=gen_core_props_path(self.export_version),
-                                           date_time=datetime.datetime.now().timetuple()[:6])
-                data = serialize_xml(self.core_props)
-                zip_file.writestr(zip_info, data)
-
             # ContentType
-            zip_info = zipfile.ZipInfo(filename=get_epc_content_type_path(),
+            zip_info_ct = zipfile.ZipInfo(filename=get_epc_content_type_path(),
                                        date_time=datetime.datetime.now().timetuple()[:6])
             data = serialize_xml(self.gen_opc_content_type())
-            zip_file.writestr(zip_info, data)
+            zip_file.writestr(zip_info_ct, data)
 
         return zip_buffer
 
     def compute_rels(self) -> Dict[str, Relationships]:
         """
         Returns a dict containing for each objet, the rels xml file path as key and the RelationShips object as value
         :return:
@@ -263,28 +263,29 @@
 
         map_obj_id_to_obj = {
             get_obj_identifier(obj): obj
             for obj in self.energyml_objects
         }
 
         obj_rels = {
-            gen_rels_path(energyml_object=map_obj_id_to_obj.get(obj_id), export_version=self.export_version): Relationships(
+            gen_rels_path(energyml_object=map_obj_id_to_obj.get(obj_id),
+                          export_version=self.export_version): Relationships(
                 relationship=obj_rels + (self.additional_rels[obj_id] if obj_id in self.additional_rels else []),
 
             )
             for obj_id, obj_rels in rels.items()
         }
 
         # CoreProps
         if self.core_props is not None:
             obj_rels[gen_rels_path(self.core_props)] = Relationships(
                 relationship=[
                     Relationship(
                         target=gen_core_props_path(),
-                        type_value=EPCRelsRelationshipType.EXTENDED_CORE_PROPERTIES.get_type(),
+                        type_value=EPCRelsRelationshipType.CORE_PROPERTIES.get_type(),
                         id="CoreProperties"
                     )
                 ]
             )
 
         return obj_rels
 
@@ -362,50 +363,55 @@
                         ov_path = ov.part_name
                         # print(ov_ct)
                         while ov_path.startswith("/") or ov_path.startswith("\\"):
                             ov_path = ov_path[1:]
                         if is_energyml_content_type(ov_ct):
                             _read_files.append(ov_path)
                             try:
-                                ov_obj = read_energyml_xml_bytes_as_class(
+                                ov_obj = read_energyml_xml_bytes(
                                     epc_file.read(ov_path),
                                     get_class_from_content_type(ov_ct)
                                 )
                                 if isinstance(ov_obj, DerivedElement):
                                     ov_obj = ov_obj.value
                                 path_to_obj[ov_path] = ov_obj
                                 obj_list.append(ov_obj)
-                            except ParserError as e:
-                                print(f"Epc.@read_stream failed to parse file {ov_path} for content-type: {ov_ct} => {get_class_from_content_type(ov_ct)}")
-                                raise e
+                            except Exception as e:
+                                print(
+                                    f"Epc.@read_stream failed to parse file {ov_path} for content-type: {ov_ct} => {get_class_from_content_type(ov_ct)}")
+                                print(e)
+                                # raise e
                         elif get_class_from_content_type(ov_ct) == CoreProperties:
                             _read_files.append(ov_path)
-                            core_props = read_energyml_xml_bytes_as_class(epc_file.read(ov_path), CoreProperties)
+                            core_props = read_energyml_xml_bytes(epc_file.read(ov_path), CoreProperties)
+                            path_to_obj[ov_path] = core_props
 
                     for f_info in epc_file.infolist():
                         if f_info.filename not in _read_files:
                             _read_files.append(f_info.filename)
                             if not f_info.filename.lower().endswith(".rels"):
                                 try:
                                     raw_file_list.append(
                                         RawFile(
                                             path=f_info.filename,
                                             content=BytesIO(epc_file.read(f_info.filename)),
                                         )
                                     )
                                 except IOError as e:
                                     print(e)
-                            else:  # rels
+                            elif f_info.filename != '_rels/.rels':  # CoreProperties rels file
+                                # RELS FILES READING START
+
                                 # print(f"reading rels {f_info.filename}")
                                 rels_folder, rels_file_name = get_file_folder_and_name_from_path(f_info.filename)
                                 while rels_folder.endswith("/"):
                                     rels_folder = rels_folder[:-1]
                                 obj_folder = rels_folder[:rels_folder.rindex("/") + 1] if "/" in rels_folder else ""
                                 obj_file_name = rels_file_name[:-5]  # removing the ".rels"
-                                rels_file: Relationships = read_energyml_xml_bytes_as_class(
+                                rels_file: Relationships = read_energyml_xml_bytes(
                                     epc_file.read(f_info.filename),
                                     Relationships
                                 )
                                 obj_path = obj_folder + obj_file_name
                                 if obj_path in path_to_obj:
                                     try:
                                         additional_rels_key = get_obj_identifier(path_to_obj[obj_path])
@@ -414,19 +420,23 @@
                                             if (rel.type_value != EPCRelsRelationshipType.DESTINATION_OBJECT.get_type()
                                                     and rel.type_value != EPCRelsRelationshipType.SOURCE_OBJECT.get_type()
                                                     and rel.type_value != EPCRelsRelationshipType.EXTENDED_CORE_PROPERTIES.get_type()
                                             ):  # not a computable relation
                                                 if additional_rels_key not in additional_rels:
                                                     additional_rels[additional_rels_key] = []
                                                 additional_rels[additional_rels_key].append(rel)
+                                    except AttributeError as e:
+                                        pass  # 'CoreProperties' object has no attribute 'object_version'
                                     except Exception as e:
                                         print(f"Error with obj path {obj_path} {path_to_obj[obj_path]}")
                                         raise e
                                 else:
-                                    print(f"xml file {obj_path} not found in EPC (rels is not associate to any object)")
+                                    print(f"xml file '{f_info.filename}' is not associate to any readable object "
+                                          f"(or the object type is not supported because"
+                                          f" of a lack of a dependency module) ")
 
             return Epc(energyml_objects=obj_list,
                        raw_files=raw_file_list,
                        core_props=core_props,
                        additional_rels=additional_rels
                        )
         except zipfile.BadZipFile as error:
@@ -526,18 +536,18 @@
     """
     Generate a path to store the :param:`energyml_object` rels file into an epc file
     (depending on the :param:`export_version`)
     :param energyml_object:
     :param export_version:
     :return:
     """
-    if isinstance(obj, CoreProperties):
+    if isinstance(energyml_object, CoreProperties):
         return f"{RELS_FOLDER_NAME}/.rels"
     else:
-        obj_path = gen_energyml_object_path(obj, export_version)
+        obj_path = gen_energyml_object_path(energyml_object, export_version)
         obj_folder, obj_file_name = get_file_folder_and_name_from_path(obj_path, )
         return f"{obj_folder}{RELS_FOLDER_NAME}/{obj_file_name}.rels"
 
 
 def get_epc_content_type_path(export_version: EpcExportVersion = EpcExportVersion.CLASSIC) -> str:
     """
     Generate a path to store the "[Content_Types].xml" file into an epc file
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/introspection.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/introspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 import uuid as uuid_mod
 from dataclasses import Field
 from enum import Enum
 from importlib import import_module
 from typing import Any, List, Optional, Union, Dict, Tuple
 
 from .manager import get_class_pkg, get_class_pkg_version, RELATED_MODULES, \
-    get_related_energyml_modules_name, get_sub_classes, get_classes_matching_name
+    get_related_energyml_modules_name, get_sub_classes, get_classes_matching_name, dict_energyml_modules
 from .xml import parse_content_type, ENERGYML_NAMESPACES
 
-
 primitives = (bool, str, int, float, type(None))
 
 
 def is_enum(cls: Union[type, Any]):
     """
     Returns True if :param:`cls` is an Enum
     :param cls:
@@ -87,57 +86,100 @@
             )
         elif last_ns_part[0].islower():
             return get_class_from_name(
                 module_name + "." + last_ns_part[0].upper() + last_ns_part[1:]
             )
         else:
             print(e)
+    except KeyError:
+        print(f"[ERR] module not found : '{module_name}'")
     return None
 
 
+def get_energyml_module_dev_version(pkg: str, current_version: str):
+    accessible_modules = dict_energyml_modules()
+    if not current_version.startswith("v"):
+        current_version = "v" + current_version
+
+    current_version = current_version.replace("-", "_").replace(".", "_")
+    res = []
+    if pkg in accessible_modules:
+        # print("\t", pkg, current_version)
+        for am_pkg_version in accessible_modules[pkg]:
+            if am_pkg_version != current_version and am_pkg_version.startswith(current_version):
+                # print("\t\t", am_pkg_version)
+                res.append(get_module_name(pkg, am_pkg_version))
+
+    return res
+
+
+def get_energyml_class_in_related_dev_pkg(cls: type):
+    class_name = cls.__name__
+    class_pkg = get_class_pkg(cls)
+    class_pkg_version = get_class_pkg_version(cls)
+
+    res = []
+
+    for dev_module_name in get_energyml_module_dev_version(class_pkg, class_pkg_version):
+        try:
+            res.append(get_class_from_name(f"{dev_module_name}.{class_name}"))
+        except Exception as e:
+            print(f"FAILED {dev_module_name}.{class_name}")
+            print(e)
+            pass
+
+    return res
+
+
 def get_class_from_content_type(content_type: str) -> Optional[type]:
     """
     Return a :class:`type` object matching with the content-type :param:`content_type`.
     :param content_type:
     :return:
     """
     ct = parse_content_type(content_type)
     domain = ct.group("domain")
     if domain is None:
+        # print(f"\tdomain {domain} xmlDomain {ct.group('xmlDomain')} ")
         domain = "opc"
     if domain == "opc":
         xml_domain = ct.group("xmlDomain")
         if "." in xml_domain:
             xml_domain = xml_domain[xml_domain.rindex(".") + 1:]
-        if "extended" in xml_domain:
-            xml_domain = xml_domain.replace("extended", "")
-        opc_type = pascal_case(xml_domain)
-        # print("energyml.opc.opc." + opc_type)
+        # Don't know what to do with http://schemas.f2i-consulting.com/package/2014/metadata/extended-core-properties
+        # if "extended" in xml_domain:
+        #     xml_domain = xml_domain.replace("extended", "")
+        #     if xml_domain.startswith("-"):
+        #         xml_domain = xml_domain[1:]
+        #
+        opc_type = pascal_case(xml_domain).replace("-", "")
+        # print("\tenergyml.opc.opc." + opc_type)
         return get_class_from_name("energyml.opc.opc." + opc_type)
     else:
-        ns = ENERGYML_NAMESPACES[domain]
         domain = ct.group("domain")
         obj_type = ct.group("type")
         if obj_type.lower().startswith("obj_"):  # for resqml201
             obj_type = "Obj" + obj_type[4:]
         version_num = str(ct.group("domainVersion")).replace(".", "_")
         if domain.lower() == "resqml" and version_num.startswith("2_0"):
             version_num = "2_0_1"
         return get_class_from_name(
-            "energyml."
-            + domain
-            + ".v"
-            + version_num
-            + "."
-            + ns[ns.rindex("/") + 1:]
+            get_module_name(domain, version_num)
             + "."
             + obj_type
         )
 
 
+def get_module_name(domain: str, domain_version: str):
+    ns = ENERGYML_NAMESPACES[domain]
+    if not domain_version.startswith("v"):
+        domain_version = "v" + domain_version
+    return f"energyml.{domain}.{domain_version}.{ns[ns.rindex('/') + 1:]}"
+
+
 def snake_case(s: str) -> str:
     """ Transform a str into snake case. """
     s = re.sub('(.)([A-Z][a-z]+)', r'\1_\2', s)
     s = re.sub('__([A-Z])', r'_\1', s)
     s = re.sub('([a-z0-9])([A-Z])', r'\1_\2', s)
     return s.lower()
 
@@ -525,15 +567,14 @@
         name_rgx = name_rgx[1:]
     current_match = name_rgx
     next_match = current_match
     if '.' in current_match:
         attrib_list = re.split(r"(?<!\\)\.+", name_rgx)
         current_match = attrib_list[0]
         next_match = '.'.join(attrib_list[1:])
-
     res = []
 
     match_value = None
     match_path_and_obj = []
     not_match_path_and_obj = []
     if isinstance(obj, list):
         cpt = 0
@@ -654,15 +695,15 @@
     try:
         return get_object_attribute_no_verif(obj, "object_version")
     except AttributeError as e:
         try:
             return get_object_attribute_no_verif(obj, "version_string")
         except Exception:
             print(f"Error with {type(obj)}")
-            raise e
+            # raise e
 
 
 def get_direct_dor_list(obj: Any) -> List[Any]:
     """
     Search all sub attribute of type "DataObjectreference".
     :param obj:
     :return:
@@ -707,17 +748,17 @@
     try:
         return cls.Meta.name  # to work with 3d transformed in 3D and Obj[A-Z] in obj_[A-Z]
     except AttributeError:
         pkg = get_class_pkg(cls)
         return get_obj_type(cls)
 
 
-def now(time_zone=datetime.timezone(datetime.timedelta(hours=1), "UTC")) -> int:
+def now(time_zone=datetime.timezone(datetime.timedelta(hours=1), "UTC")) -> float:
     """ Return an epoch value """
-    return int(datetime.datetime.timestamp(datetime.datetime.now(time_zone)))
+    return datetime.datetime.timestamp(datetime.datetime.now(time_zone))
 
 
 def epoch(time_zone=datetime.timezone(datetime.timedelta(hours=1), "UTC")) -> int:
     return int(now(time_zone))
 
 
 def date_to_epoch(date: str) -> int:
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/manager.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,19 +202,25 @@
     return version
 
 
 def get_class_pkg_version(
     cls, print_dev_version: bool = True, nb_max_version_digits: int = 2
 ):
     p = re.compile(REGEX_ENERGYML_MODULE_NAME)
-    m = p.search(
-        cls.__module__ if isinstance(cls, type) else type(cls).__module__
-    )
+    class_module = None
+    if isinstance(cls, type):
+        class_module = cls.__module__
+    elif isinstance(cls, str):
+        class_module = cls
+    else:
+        class_module = type(cls).__module__
+
+    m = p.search(class_module)
     return reshape_version(m.group("versionNumber"), nb_max_version_digits) + (
-        m.group("versionDev")
+        "dev" + m.group("versionDev")
         if m.group("versionDev") is not None and print_dev_version
         else ""
     )
 
 
 # ProtocolDict = DefaultDict[str, MessageDict]
 # def get_all__classes() -> ProtocolDict:
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/serialization.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/serialization.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,84 @@
 # Copyright (c) 2023-2024 Geosiris.
 # SPDX-License-Identifier: Apache-2.0
 from io import BytesIO
 from typing import Optional, Any
 
 import energyml
+import xsdata
 from xsdata.exceptions import ParserError
 from xsdata.formats.dataclass.context import XmlContext
 from xsdata.formats.dataclass.parsers import XmlParser
 from xsdata.formats.dataclass.serializers import JsonSerializer
 from xsdata.formats.dataclass.serializers import XmlSerializer
 from xsdata.formats.dataclass.serializers.config import SerializerConfig
 
-from .introspection import get_class_from_name
-from .xml import get_class_name_from_xml, get_tree
+from .introspection import get_class_from_name, get_energyml_class_in_related_dev_pkg
+from .manager import dict_energyml_modules, get_class_pkg_version, get_class_pkg
+from .xml import get_class_name_from_xml, get_tree, get_xml_encoding
 
 
-def read_energyml_xml_bytes_as_class(file: bytes, obj_class: type) -> Any:
+def _read_energyml_xml_bytes_as_class(file: bytes, obj_class: type) -> Any:
     """
     Read an xml file into the instance of type :param:`obj_class`.
     :param file:
     :param obj_class:
     :return:
     """
     parser = XmlParser()
     try:
         return parser.from_bytes(file, obj_class)
     except ParserError as e:
         print(f"Failed to parse file {file} as class {obj_class}")
         raise e
 
 
-def read_energyml_xml_bytes(file: bytes) -> Any:
+def read_energyml_xml_bytes(file: bytes, obj_type: Optional[type] = None) -> Any:
     """
-    Read an xml file. The type of object is searched from the xml root name.
+    Read an xml file. The type of object is searched from the xml root name if not given.
+    :param obj_type:
     :param file:
     :return:
     """
-    return read_energyml_xml_bytes_as_class(
-        file, get_class_from_name(get_class_name_from_xml(get_tree(file)))
-    )
+    if obj_type is None:
+        obj_type = get_class_from_name(get_class_name_from_xml(get_tree(file)))
+    try:
+        return _read_energyml_xml_bytes_as_class(file, obj_type)
+    except xsdata.exceptions.ParserError as e:
+        print(f"Failed to read file with type {obj_type}: {get_energyml_class_in_related_dev_pkg(obj_type)}")
+        for obj_type_dev in get_energyml_class_in_related_dev_pkg(obj_type):
+            try:
+                print(f"Trying with class : {obj_type_dev}")
+                obj = _read_energyml_xml_bytes_as_class(
+                    file, obj_type_dev
+                )
+                print(f" ==> succeed read with {obj_type_dev}")
+                return obj
+            except Exception:
+                pass
+        raise e
 
 
 def read_energyml_xml_io(file: BytesIO, obj_class: Optional[type] = None) -> Any:
     if obj_class is not None:
         return read_energyml_xml_bytes_as_class(file.getbuffer(), obj_class)
     else:
         return read_energyml_xml_bytes(file.getbuffer())
 
 
 def read_energyml_xml_str(file_content: str) -> Any:
-    parser = XmlParser()
-    # from energyml.resqml.v2_2.resqmlv2 import TriangulatedSetRepresentation
-    return parser.from_string(
-        file_content,
-        get_class_from_name(get_class_name_from_xml(get_tree(file_content))),
-    )  # , TriangulatedSetRepresentation)
+    encoding = get_xml_encoding(file_content)
+    return read_energyml_xml_bytes(file_content.encode(encoding))
 
 
 def read_energyml_xml_file(file_path: str) -> Any:
-    xml_content = ""
-    with open(file_path, "r") as f:
-        xml_content = f.read()
-    parser = XmlParser()
-    # from energyml.resqml.v2_2.resqmlv2 import TriangulatedSetRepresentation
-    # return parser.parse(file_path)  # , TriangulatedSetRepresentation)
-    return parser.parse(
-        file_path,
-        get_class_from_name(get_class_name_from_xml(get_tree(xml_content))),
-    )
+    xml_content_b = ""
+    with open(file_path, "rb") as f:
+        xml_content_b = f.read()
+    return read_energyml_xml_bytes(xml_content_b)
 
 
 def serialize_xml(obj) -> str:
     context = XmlContext(
         # element_name_generator=text.camel_case,
         # attribute_name_generator=text.kebab_case
     )
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/validation.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .introspection import (
     get_class_fields,
     get_object_attribute,
     search_attribute_matching_type_with_path,
     get_object_attribute_no_verif,
     get_object_attribute_rgx,
     get_matching_class_attribute_name, get_obj_uuid, get_obj_version, get_content_type_from_class,
-    get_qualified_type_from_class,
+    get_qualified_type_from_class, is_enum,
 )
 
 
 class ErrorType(Enum):
     CRITICAL = "critical"
     DEBUG = "debug"
     INFO = "info"
@@ -236,15 +236,15 @@
             errs.append(
                 MandatoryError(
                     error_type=ErrorType.CRITICAL,
                     target_obj=root_obj,
                     attribute_dot_path=path,
                 )
             )
-    else:
+    elif not is_enum(value):  # sometimes enums values fails the validation
         min_length = att_field.metadata.get("min_length", None)
         max_length = att_field.metadata.get("max_length", None)
         pattern = att_field.metadata.get("pattern", None)
         min_occurs = att_field.metadata.get("pattern", None)
         min_inclusive = att_field.metadata.get("pattern", None)
         # white_space
```

### Comparing `energyml_utils-1.0.0/src/energyml/utils/xml.py` & `energyml_utils-1.0.1.dev4/src/energyml/utils/xml.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,16 +94,18 @@
     if pkg is None:
         print(f"No pkg found for elt {tree}")
     else:
         if pkg == "opc":
             return "energyml.opc.opc." + get_root_type(tree)
         else:
             schema_version = find_schema_version_in_element(tree).replace(".", "_").replace("-", "_")
+            # print(schema_version)
             if pkg == "resqml" and schema_version == "2_0":
                 schema_version = "2_0_1"
+
             return ("energyml." + pkg
                     + ".v" + schema_version
                     + "."
                     + root_namespace[root_namespace.rindex("/") + 1:]
                     + "." + get_root_type(tree)
                     )
 
@@ -115,15 +117,16 @@
     except AttributeError:
         return "utf-8"
 
 
 def get_tree(xml_content: Union[bytes, str]) -> ETREE.Element:
     xml_bytes = xml_content
     if isinstance(xml_bytes, str):
-        xml_bytes = xml_content.encode(encoding=get_xml_encoding(xml_content).strip().lower())
+        encoding = get_xml_encoding(xml_content)
+        xml_bytes = xml_content.encode(encoding=encoding.strip().lower() if encoding is not None else "utf-8")
 
     return ETREE.parse(BytesIO(xml_bytes)).getroot()
 
 
 def energyml_xpath(tree: ETREE.Element, xpath: str) -> Optional[list]:
     """A xpath research that knows energyml namespaces"""
     try:
@@ -168,15 +171,15 @@
     :rtype: str
     """
     _schema_version = tree.xpath("@schemaVersion")
     if _schema_version is None:
         _schema_version = tree.xpath("@SchemaVersion")
 
     if _schema_version is not None:
-        match_version = re.search(r"\d+(\.\d+)*", _schema_version[0])
+        match_version = re.search(r"\d+(\.\d+)*(dev\d+)?", _schema_version[0])
         if match_version is not None:
-            return match_version.group(0)
+            return match_version.group(0).replace("dev", "-dev")
     return ""
 
 
 def parse_content_type(ct: str):
     return re.search(REGEX_CONTENT_TYPE, ct)
```

### Comparing `energyml_utils-1.0.0/PKG-INFO` & `energyml_utils-1.0.1.dev4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyml-utils
-Version: 1.0.0
+Version: 1.0.1.dev4
 Summary: Energyml helper
 Home-page: http://www.geosiris.com
 License: Apache-2.0
 Keywords: energyml,resqml,witsml,prodml
 Author: Valentin Gauthier
 Author-email: valentin.gauthier@geosiris.com
 Maintainer: Valentin Gauthier
@@ -22,19 +22,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: energyml-common2-0 (==1.12.0)
-Requires-Dist: energyml-common2-3 (==1.12.0)
 Requires-Dist: energyml-opc (>=1.12.0,<2.0.0)
-Requires-Dist: energyml-resqml2-0-1 (>=1.12.0,<2.0.0)
-Requires-Dist: energyml-resqml2-2 (>=1.12.0,<2.0.0)
 Requires-Dist: h5py (>=3.7.0,<4.0.0)
 Requires-Dist: xsdata[cli,lxml] (>=24.0,<25.0)
 Project-URL: Repository, https://github.com/geosiris-technologies/energyml-python
 Description-Content-Type: text/markdown
 
 <!--
 Copyright (c) 2022-2023 Geosiris.
```

