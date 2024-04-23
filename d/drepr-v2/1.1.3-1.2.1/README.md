# Comparing `tmp/drepr_v2-1.1.3.tar.gz` & `tmp/drepr_v2-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drepr_v2-1.1.3.tar", max compression
+gzip compressed data, was "drepr_v2-1.2.1.tar", max compression
```

## Comparing `drepr_v2-1.1.3.tar` & `drepr_v2-1.2.1.tar`

### file list

```diff
@@ -1,51 +1,53 @@
--rw-r--r--   0        0        0     1064 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/LICENSE
--rw-r--r--   0        0        0       53 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/README.md
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/__init__.py
--rw-r--r--   0        0        0     3448 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/__main__.py
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/__init__.py
--rw-r--r--   0        0        0     4565 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/align.py
--rw-r--r--   0        0        0     1263 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/attr.py
--rw-r--r--   0        0        0    17593 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/drepr.py
--rw-r--r--   0        0        0     3416 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/drepr_builder.py
--rw-r--r--   0        0        0       71 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/format.py
--rw-r--r--   0        0        0     8805 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/__init__.py
--rw-r--r--   0        0        0     5815 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/align_parser.py
--rw-r--r--   0        0        0     4494 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/attr_parser.py
--rw-r--r--   0        0        0     5940 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/path_parser.py
--rw-r--r--   0        0        0     5430 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/preprocessing_parser.py
--rw-r--r--   0        0        0     3255 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/resource_parser.py
--rw-r--r--   0        0        0     7107 2024-03-26 23:13:27.937340 drepr_v2-1.1.3/drepr/models/parse_v1/sm_parser.py
--rw-r--r--   0        0        0     9430 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/parse_v2/__init__.py
--rw-r--r--   0        0        0    11157 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/parse_v2/path_parser.py
--rw-r--r--   0        0        0     8608 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/parse_v2/sm_parser.py
--rw-r--r--   0        0        0     6706 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/path.py
--rw-r--r--   0        0        0      326 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/prelude.py
--rw-r--r--   0        0        0     1951 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/preprocessing.py
--rw-r--r--   0        0        0     1339 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/resource.py
--rw-r--r--   0        0        0     9102 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/models/sm.py
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/planning/__init__.py
--rw-r--r--   0        0        0    16295 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/planning/class_map_plan.py
--rw-r--r--   0        0        0    16754 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/planning/drepr_model_alignments.py
--rw-r--r--   0        0        0     4610 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/planning/topological_sorting.py
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/__init__.py
--rw-r--r--   0        0        0    15366 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/alignment_fn.py
--rw-r--r--   0        0        0    18497 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/main.py
--rw-r--r--   0        0        0     1569 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/predefined_fn.py
--rw-r--r--   0        0        0    11605 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/preprocessing.py
--rw-r--r--   0        0        0     1277 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/program_space.py
--rw-r--r--   0        0        0     4966 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/program_generation/writers.py
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/readers/__init__.py
--rw-r--r--   0        0        0      157 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/readers/csv.py
--rw-r--r--   0        0        0      160 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/readers/json.py
--rw-r--r--   0        0        0      145 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/readers/prelude.py
--rw-r--r--   0        0        0       61 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/__init__.py
--rw-r--r--   0        0        0     2664 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/misc.py
--rw-r--r--   0        0        0      998 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/namespace_mixin.py
--rw-r--r--   0        0        0      443 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/safe.py
--rw-r--r--   0        0        0     3829 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/udf.py
--rw-r--r--   0        0        0     7798 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/utils/validator.py
--rw-r--r--   0        0        0        0 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/writers/__init__.py
--rw-r--r--   0        0        0     3850 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/writers/base.py
--rw-r--r--   0        0        0     2995 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/drepr/writers/rdfgraph_writer.py
--rw-r--r--   0        0        0      584 2024-03-26 23:13:27.941340 drepr_v2-1.1.3/pyproject.toml
--rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 drepr_v2-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/LICENSE
+-rw-r--r--   0        0        0       53 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/__init__.py
+-rw-r--r--   0        0        0     3754 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/__init__.py
+-rw-r--r--   0        0        0     4710 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/align.py
+-rw-r--r--   0        0        0     1263 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/attr.py
+-rw-r--r--   0        0        0    18068 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/drepr.py
+-rw-r--r--   0        0        0     3416 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/drepr_builder.py
+-rw-r--r--   0        0        0       71 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/format.py
+-rw-r--r--   0        0        0     8805 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/__init__.py
+-rw-r--r--   0        0        0     5815 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/align_parser.py
+-rw-r--r--   0        0        0     4494 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/attr_parser.py
+-rw-r--r--   0        0        0     5940 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/path_parser.py
+-rw-r--r--   0        0        0     5430 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/preprocessing_parser.py
+-rw-r--r--   0        0        0     3255 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/resource_parser.py
+-rw-r--r--   0        0        0     7107 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v1/sm_parser.py
+-rw-r--r--   0        0        0     9430 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/__init__.py
+-rw-r--r--   0        0        0    11569 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/path_parser.py
+-rw-r--r--   0        0        0     9359 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/parse_v2/sm_parser.py
+-rw-r--r--   0        0        0     6706 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/path.py
+-rw-r--r--   0        0        0      326 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/prelude.py
+-rw-r--r--   0        0        0     3917 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/preprocessing.py
+-rw-r--r--   0        0        0     2005 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/resource.py
+-rw-r--r--   0        0        0     9252 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/models/sm.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/__init__.py
+-rw-r--r--   0        0        0    19789 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/class_map_plan.py
+-rw-r--r--   0        0        0    17577 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/drepr_model_alignments.py
+-rw-r--r--   0        0        0     4783 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/planning/topological_sorting.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/__init__.py
+-rw-r--r--   0        0        0    17908 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/alignment_fn.py
+-rw-r--r--   0        0        0    23969 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/main.py
+-rw-r--r--   0        0        0     1569 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/predefined_fn.py
+-rw-r--r--   0        0        0    16794 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/preprocessing.py
+-rw-r--r--   0        0        0     1458 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/program_space.py
+-rw-r--r--   0        0        0     4966 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/program_generation/writers.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/__init__.py
+-rw-r--r--   0        0        0      157 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/csv.py
+-rw-r--r--   0        0        0      160 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/json.py
+-rw-r--r--   0        0        0      145 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/prelude.py
+-rw-r--r--   0        0        0      382 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/readers/spreadsheet.py
+-rw-r--r--   0        0        0       61 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/__init__.py
+-rw-r--r--   0        0        0     6400 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/attr_data.py
+-rw-r--r--   0        0        0     2960 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/misc.py
+-rw-r--r--   0        0        0      828 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/namespace_mixin.py
+-rw-r--r--   0        0        0      443 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/safe.py
+-rw-r--r--   0        0        0     4341 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/udf.py
+-rw-r--r--   0        0        0     7798 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/utils/validator.py
+-rw-r--r--   0        0        0        0 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/__init__.py
+-rw-r--r--   0        0        0     3850 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/base.py
+-rw-r--r--   0        0        0     3627 2024-04-23 19:55:32.414102 drepr_v2-1.2.1/drepr/writers/rdfgraph_writer.py
+-rw-r--r--   0        0        0      604 2024-04-23 19:55:32.418102 drepr_v2-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      719 1970-01-01 00:00:00.000000 drepr_v2-1.2.1/PKG-INFO
```

### Comparing `drepr_v2-1.1.3/LICENSE` & `drepr_v2-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/__main__.py` & `drepr_v2-1.2.1/drepr/__main__.py`

 * *Files 17% similar despite different names*

```diff
@@ -87,15 +87,15 @@
     exec_plan = ClassesMapExecutionPlan.create(parsed_repr)
 
     if outfile is not None:
         output = FileOutput(outfile, format)
     else:
         output = MemoryOutput(format)
 
-    prog = gen_program(parsed_repr, exec_plan, output, debuginfo).to_python()
+    prog = gen_program(exec_plan.desc, exec_plan, output, debuginfo).to_python()
     cleanup = progfile is None
     if progfile is not None:
         with open(progfile, "w") as f:
             f.write(prog)
     else:
         tmpdir.mkdir(parents=True, exist_ok=True)
         unique_id = str(uuid4()).replace("-", "_")
@@ -103,17 +103,32 @@
         progfile.write_text(prog)
 
     spec = importlib.util.spec_from_file_location("drepr_prog", progfile)
     assert spec is not None and spec.loader is not None
     module = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(module)
     if outfile is not None:
-        module.main(*[parsed_resources[r.id] for r in parsed_repr.resources], outfile)
+        module.main(
+            *[
+                parsed_resources[r.id]
+                for r in exec_plan.desc.resources
+                if not r.is_preprocessing_output()
+            ],
+            outfile,
+        )
     else:
-        print(module.main(*[parsed_resources[r.id] for r in parsed_repr.resources]))
+        print(
+            module.main(
+                *[
+                    parsed_resources[r.id]
+                    for r in exec_plan.desc.resources
+                    if not r.is_preprocessing_output()
+                ]
+            )
+        )
 
     if cleanup:
         progfile.unlink()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `drepr_v2-1.1.3/drepr/models/align.py` & `drepr_v2-1.2.1/drepr/models/align.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,18 +98,25 @@
         else:
             if target.unique:
                 return Cardinality.ManyToOne
             else:
                 return Cardinality.ManyToMany
 
 
+@dataclass
 class IdenticalAlign:
+    source: AttrId
+    target: AttrId
+
     def compute_cardinality(self, desc: DRepr) -> Cardinality:
         return Cardinality.OneToOne
 
+    def swap(self) -> IdenticalAlign:
+        return IdenticalAlign(self.target, self.source)
+
 
 @dataclass
 class AutoAlignment:
     attrs: Optional[list[str]] = None
 
     def compute_cardinality(self, desc: DRepr) -> Cardinality:
         raise NotImplementedError(
```

### Comparing `drepr_v2-1.1.3/drepr/models/attr.py` & `drepr_v2-1.2.1/drepr/models/attr.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/drepr.py` & `drepr_v2-1.2.1/drepr/models/drepr.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,27 +152,35 @@
 
     def is_valid(self):
         """
         Perform a check to see if this D-REPR is valid. Raise AssertionError if this is not valid
         """
         # CHECK 1: all references (resource id, attribute ids) are valid
         resource_ids = {r.id for r in self.resources}
-        for pref in self.preprocessing:
-            if pref.value.output is not None:
-                # preprocessing create new resource
-                assert (
-                    pref.value.output not in resource_ids
-                ), "Cannot overwrite existing resources"
-                resource_ids.add(pref.value.output)
-        attr_ids = {attr.id for attr in self.attrs}
+        for r in self.resources:
+            assert not r.is_preprocessing_output(), (
+                f"Resource {r.id} is detected as output of a preprocessing step. "
+                f"Please choose a different name"
+            )
 
+        attr_ids = {attr.id for attr in self.attrs}
+        assert len(attr_ids) == len(self.attrs), "Duplicate attribute ids"
         for attr in self.attrs:
             assert (
                 attr.resource_id in resource_ids
             ), f"Attribute {attr.resource_id} does not belong to any resources"
+
+        for pref in self.preprocessing:
+            if pref.value.output is not None:
+                # preprocessing create new attribute
+                assert (
+                    pref.value.output not in attr_ids
+                ), f"Cannot overwrite existing attribute: {pref.value.output}"
+                attr_ids.add(pref.value.output)
+
         for align in self.aligns:
             if isinstance(align, AutoAlignment):
                 if align.attrs is not None:
                     assert all(
                         attr_id in attr_ids for attr_id in align.attrs
                     ), f"The alignment {align} links to non-existence attributes"
             else:
@@ -418,14 +426,18 @@
 
     def get_resource_by_id(self, resource_id: str) -> Optional[Resource]:
         for r in self.resources:
             if r.id == resource_id:
                 return r
         return None
 
+    def add_resource(self, resource: Resource):
+        assert self.get_resource_by_id(resource.id) is None
+        self.resources.append(resource)
+
     def has_attr(self, attr_id: str) -> bool:
         return any(a.id == attr_id for a in self.attrs)
 
     def get_attr_index_by_id(self, attr_id: str) -> int:
         for i, a in enumerate(self.attrs):
             if a.id == attr_id:
                 return i
```

### Comparing `drepr_v2-1.1.3/drepr/models/drepr_builder.py` & `drepr_v2-1.2.1/drepr/models/drepr_builder.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/__init__.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/align_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/align_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/attr_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/attr_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/path_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/path_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/preprocessing_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/preprocessing_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/resource_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/resource_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v1/sm_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v1/sm_parser.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v2/__init__.py` & `drepr_v2-1.2.1/drepr/models/parse_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v2/path_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v2/path_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 from abc import ABC, abstractmethod
 from copy import copy
-from typing import List, Union
+from typing import List, Optional, Union
 
 from drepr.models.parse_v1.path_parser import PathParser
 from drepr.utils.validator import InputError
 
 from ..path import Expr, IndexExpr, Path, RangeExpr, WildcardExpr
 from ..resource import Resource, ResourceType
 
@@ -25,15 +25,15 @@
 
     REG_JPATH_BRACKET = re.compile(
         r"(?:\[(-?\d+)?\:(-?\d+)?(?:\:(-?\d+))?\])|(?:\[(-?\d+)\])|(?:\['([^']+)'\])"
     )
     REG_JPATH_DOT = re.compile(r"\.((?:(?!\.|\[).)+)")
 
     def parse(
-        self, resource: Resource, path: Union[str, list], parse_trace: str
+        self, resource: Optional[Resource], path: Union[str, list], parse_trace: str
     ) -> Path:
         if isinstance(path, str):
             return self.parse_jsonpath(resource, path, parse_trace)
 
         if isinstance(path, list):
             return self.parse_custom_path(resource, path, parse_trace)
 
@@ -55,71 +55,74 @@
         return index - 1
 
     def isdigit(self, s: str) -> bool:
         if s.startswith("-"):
             return s[1:].isdigit()
         return s.isdigit()
 
-    def parse_jsonpath(self, resource: Resource, jpath: str, parse_trace: str) -> Path:
+    def parse_jsonpath(
+        self, resource: Optional[Resource], jpath: str, parse_trace: str
+    ) -> Path:
         if not jpath.startswith("$"):
             raise InputError(
                 f"{parse_trace}\nERROR: invalid json path. The path must start with `$`. "
                 f"Get: {jpath}"
             )
 
         jpath = jpath[1:]
         steps = []
         parsing_pos = 1
 
         # pre-processing the spreadsheet resource to allow letter column
-        if resource.type == ResourceType.Spreadsheet:
-            last_step_index = max(jpath.rfind("["), jpath.rfind("."))
-            if jpath[last_step_index] == "[":
-                last_step = jpath[last_step_index + 1 : -1]
-                result = last_step.split(":")
-                if len(result) == 1:
-                    index = result[0]
-                    if not self.isdigit(index):
-                        new_last_step = self.letter2index(index)
-                    else:
-                        new_last_step = index
-                else:
-                    if len(result) == 3:
-                        start, end, step = result
-                    elif len(result) == 2:
-                        start, end = result
-                        step = 1
+        if resource is not None:
+            if resource.type == ResourceType.Spreadsheet:
+                last_step_index = max(jpath.rfind("["), jpath.rfind("."))
+                if jpath[last_step_index] == "[":
+                    last_step = jpath[last_step_index + 1 : -1]
+                    result = last_step.split(":")
+                    if len(result) == 1:
+                        index = result[0]
+                        if not self.isdigit(index):
+                            new_last_step = self.letter2index(index)
+                        else:
+                            new_last_step = index
                     else:
-                        raise InputError(f"{parse_trace}\nERROR: invalid path")
+                        if len(result) == 3:
+                            start, end, step = result
+                        elif len(result) == 2:
+                            start, end = result
+                            step = 1
+                        else:
+                            raise InputError(f"{parse_trace}\nERROR: invalid path")
 
-                    if (len(start) > 0 and not self.isdigit(start)) or (
-                        len(end) > 0 and not self.isdigit(end)
-                    ):
-                        # they use letter system, otherwise, do nothing
-                        if (len(start) > 0 and self.isdigit(start)) or (
-                            len(end) > 0 and self.isdigit(end)
+                        if (len(start) > 0 and not self.isdigit(start)) or (
+                            len(end) > 0 and not self.isdigit(end)
                         ):
-                            raise InputError(
-                                f"{parse_trace}\nERROR: Cannot mixed between number and letter index"
-                            )
-                        start = self.letter2index(start)
-                        if len(end) > 0:
-                            end = self.letter2index(end)
-                        new_last_step = f"{start}:{end}:{step}"
+                            # they use letter system, otherwise, do nothing
+                            if (len(start) > 0 and self.isdigit(start)) or (
+                                len(end) > 0 and self.isdigit(end)
+                            ):
+                                raise InputError(
+                                    f"{parse_trace}\nERROR: Cannot mixed between number and letter index"
+                                )
+                            start = self.letter2index(start)
+                            if len(end) > 0:
+                                end = self.letter2index(end)
+                            new_last_step = f"{start}:{end}:{step}"
+                        else:
+                            new_last_step = f"{start}:{end}:{step}"
+
+                    jpath = jpath[:last_step_index] + f"[{new_last_step}]"
+                elif jpath[last_step_index] == ".":
+                    last_step = jpath[last_step_index + 1 :]
+                    if not self.isdigit(last_step):
+                        new_last_step = self.letter2index(last_step)
                     else:
-                        new_last_step = f"{start}:{end}:{step}"
-
-                jpath = jpath[:last_step_index] + f"[{new_last_step}]"
-            elif jpath[last_step_index] == ".":
-                last_step = jpath[last_step_index + 1 :]
-                if not self.isdigit(last_step):
-                    new_last_step = self.letter2index(last_step)
-                else:
-                    new_last_step = last_step
-                jpath = jpath[:last_step_index] + f".{new_last_step}"
+                        new_last_step = last_step
+                    jpath = jpath[:last_step_index] + f".{new_last_step}"
 
         while len(jpath) > 0:
             if jpath.startswith("["):
                 m = self.REG_JPATH_BRACKET.match(jpath)
                 if m is None:
                     raise InputError(
                         f"{parse_trace}\nERROR: invalid json path, error while parsing bracket at position {parsing_pos}"
@@ -166,47 +169,48 @@
                     steps.append(IndexExpr(int(m.group(1))))
                 else:
                     steps.append(IndexExpr(m.group(1)))
 
         return Path(steps)
 
     def parse_custom_path(
-        self, resource: Resource, path: List[str], parse_trace: str
+        self, resource: Optional[Resource], path: List[str], parse_trace: str
     ) -> Path:
-        if resource.type == ResourceType.Spreadsheet:
-            path = copy(path)
-            last_step = path[-1]
-            if isinstance(last_step, str):
-                if last_step.find("..") != -1:
-                    tmp = last_step.split(":")
-                    start, end = tmp[0].split("..")
-                    if len(tmp) == 2:
-                        step = f":{tmp[1]}"
-                    else:
-                        step = ""
+        if resource is not None:
+            if resource.type == ResourceType.Spreadsheet:
+                path = copy(path)
+                last_step = path[-1]
+                if isinstance(last_step, str):
+                    if last_step.find("..") != -1:
+                        tmp = last_step.split(":")
+                        start, end = tmp[0].split("..")
+                        if len(tmp) == 2:
+                            step = f":{tmp[1]}"
+                        else:
+                            step = ""
 
-                    if (len(start) > 0 and not self.isdigit(start)) or (
-                        len(end) > 0 and not self.isdigit(end)
-                    ):
-                        # they use letter system, otherwise, do nothing
-                        if (len(start) > 0 and self.isdigit(start)) or (
-                            len(end) > 0 and self.isdigit(end)
+                        if (len(start) > 0 and not self.isdigit(start)) or (
+                            len(end) > 0 and not self.isdigit(end)
                         ):
-                            raise InputError(
-                                f"{parse_trace}\nERROR: Cannot mixed between number and letter index"
-                            )
-                        start = self.letter2index(start)
-                        if len(end) > 0:
-                            end = self.letter2index(end)
-                        new_last_step = f"{start}..{end}{step}"
-                    else:
-                        new_last_step = f"{start}..{end}{step}"
-                    path[-1] = new_last_step
-                elif not self.isdigit(last_step):
-                    path[-1] = self.letter2index(last_step)
+                            # they use letter system, otherwise, do nothing
+                            if (len(start) > 0 and self.isdigit(start)) or (
+                                len(end) > 0 and self.isdigit(end)
+                            ):
+                                raise InputError(
+                                    f"{parse_trace}\nERROR: Cannot mixed between number and letter index"
+                                )
+                            start = self.letter2index(start)
+                            if len(end) > 0:
+                                end = self.letter2index(end)
+                            new_last_step = f"{start}..{end}{step}"
+                        else:
+                            new_last_step = f"{start}..{end}{step}"
+                        path[-1] = new_last_step
+                    elif not self.isdigit(last_step):
+                        path[-1] = self.letter2index(last_step)
 
         steps = []
         for i, step in enumerate(path):
             trace = f"Parsing step {i} ({step})"
             if isinstance(step, str):
                 m = self.REG_SRANGE.match(step)
                 if m is not None:
```

### Comparing `drepr_v2-1.1.3/drepr/models/parse_v2/sm_parser.py` & `drepr_v2-1.2.1/drepr/models/parse_v2/sm_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import copy
 import re
 
-from drepr.utils.misc import F
+from drepr.utils.misc import F, get_abs_iri
+from drepr.utils.namespace_mixin import NamespaceMixin
 from drepr.utils.validator import InputError, Validator
 
 from ..sm import (
+    DREPR_URI,
     ClassNode,
     DataNode,
     DataType,
     Edge,
     LiteralNode,
     PredefinedDataType,
     SemanticModel,
@@ -21,15 +23,15 @@
 
     ```
     semantic_model:
       <class_id>:
         properties:
             - [<predicate>, <attr_id>, (<data_type>, (<is_required=false>)?)?]
         links:
-            - [<predicate>, <class_id>]
+            - [<predicate>, <class_id>, (<is_required=false>)?]
         static_properties:
             - [<predicate>, <value>, (<data_type>)?]
         inverse_static_properties:
             - [<predicate>, <uri>]
       prefixes:
         <prefix>: <uri>
     ```
@@ -39,15 +41,15 @@
         "properties",
         "subject",
         "links",
         "static_properties",
         "inverse_static_properties",
     }
 
-    REG_SM_CLASS = re.compile(r"^((.+):\d+)$")
+    REG_SM_CLASS = re.compile(r"^((.+):[a-zA-Z0-9]+)$")
     REG_SM_DNODE = re.compile(r"^((?:(?!--).)+:\d+)--((?:(?!\^\^).)+)(?:\^\^(.+))?$")
     REG_SM_LNODE = re.compile(
         r"^((?:(?!--).)+:\d+)--((?:(?!--).)+)--((?:(?!\^\^).)+)(?:\^\^(.+))?$"
     )
     REG_SM_REL = re.compile(r"^((?:(?!--).)+:\d+)--((?:(?!--).)+)--((?:(?!--).)+:\d+)$")
 
     @classmethod
@@ -80,15 +82,15 @@
 
             try:
                 m = cls.REG_SM_CLASS.match(class_id)
                 assert m is not None
                 class_name = m.group(2)
             except Exception as e:
                 raise InputError(
-                    f"{trace0}\nERROR: invalid class_id `{class_id}`. Expect to be <string>:<number>"
+                    f"{trace0}\nERROR: invalid class_id `{class_id}`. Expect to be <string>:<alphanumeric>"
                 )
 
             nodes[class_id] = ClassNode(class_id, class_name)
 
         for class_id, class_conf in sm.items():
             trace0 = f"Parsing class `{class_id}` of the semantic model"
 
@@ -136,22 +138,32 @@
                     node.node_id,
                     predicate,
                     is_required=is_required,
                 )
 
             for i, link_conf in enumerate(class_conf.get("links", [])):
                 trace1 = f"{trace0}\nParsing link {i}: {link_conf}"
-                if len(link_conf) != 2:
+                if not (2 <= len(link_conf) <= 3):
                     raise InputError(
-                        f"{trace1}\nERROR: Expect value of the link to be an array of two "
-                        f"items (<predicate>, <class_id>)"
+                        f"{trace1}\nERROR: Expect value of the link to be an array of two or three"
+                        f"items (<predicate>, <class_id>, <is_required=false>)"
                     )
-                predicate, object_class_id = link_conf
+
+                if len(link_conf) == 2:
+                    predicate, object_class_id = link_conf
+                    is_required = False
+                else:
+                    predicate, object_class_id, is_required = link_conf
+
                 edges[len(edges)] = Edge(
-                    len(edges), class_id, object_class_id, predicate
+                    len(edges),
+                    class_id,
+                    object_class_id,
+                    predicate,
+                    is_required=is_required,
                 )
 
             for i, prop in enumerate(class_conf.get("static_properties", [])):
                 trace1 = f"{trace0}\nParsing static properties {i}: {prop}"
                 if len(prop) == 2:
                     predicate, value = prop
                     data_type = None
@@ -173,14 +185,20 @@
                 if isinstance(value, str):
                     value = str(value)
                 elif isinstance(value, int):
                     value = int(value)
                 elif isinstance(value, float):
                     value = float(value)
 
+                if data_type == DREPR_URI:
+                    assert isinstance(value, str)
+                    # test if the value is relative uri, if so, convert it to absolute uri
+                    if NamespaceMixin.is_rel_iri(value):
+                        value = get_abs_iri(prefixes, value)
+
                 node = LiteralNode(
                     node_id=f"lnode:{len(nodes)}", value=value, data_type=data_type
                 )
                 nodes[node.node_id] = node
                 edges[len(edges)] = Edge(len(edges), class_id, node.node_id, predicate)
 
             for i, prop in enumerate(class_conf.get("inverse_static_properties", [])):
```

### Comparing `drepr_v2-1.1.3/drepr/models/path.py` & `drepr_v2-1.2.1/drepr/models/path.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/models/resource.py` & `drepr_v2-1.2.1/drepr/models/resource.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
 from typing import Optional, TypeAlias, Union
 
 ResourceId: TypeAlias = str
 
@@ -20,28 +22,49 @@
 
 
 @dataclass
 class CSVProp:
     delimiter: str = ","
 
 
+# @dataclass
+# class SpreadsheetProp:
+#     worksheet: Optional[str] = None
+
+
 @dataclass
 class Resource:
     id: ResourceId
     type: ResourceType
     prop: Optional[CSVProp] = None
 
     @staticmethod
     def deserialize(raw: dict):
         if raw["type"] == ResourceType.CSV.value and raw["prop"] is not None:
             prop = CSVProp(raw["prop"]["delimiter"])
         else:
             prop = None
         return Resource(raw["id"], ResourceType(raw["type"]), prop)
 
+    def is_preprocessing_output(self):
+        """Return true if this resource holds output of preprocessing functions"""
+        return (
+            self.id.startswith(f"__preproc__") and self.type == ResourceType.Container
+        )
+
+    @staticmethod
+    def create_preprocessing_output(attr_id: str) -> Resource:
+        return Resource(
+            Resource.get_preprocessing_output_id(attr_id), ResourceType.Container
+        )
+
+    @staticmethod
+    def get_preprocessing_output_id(attr_id: str) -> str:
+        return f"__preproc__{attr_id}"
+
 
 class ResourceData(ABC):
 
     @abstractmethod
     def to_dict(self):
         pass
```

### Comparing `drepr_v2-1.1.3/drepr/models/sm.py` & `drepr_v2-1.2.1/drepr/models/sm.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from rdflib import OWL, RDF, RDFS, XSD
 
 from drepr.utils.namespace_mixin import NamespaceMixin
 
 from .attr import Attr, AttrId
 
 DREPR_URI = "https://purl.org/drepr/1.0/uri"
+DREPR_BLANK = "https://purl.org/drepr/1.0/blank"
 NodeId: TypeAlias = str
 EdgeId: TypeAlias = int
 
 
 class PredefinedNamespace(Enum):
     drepr = "https://purl.org/drepr/1.0/"
     rdf = str(RDF)
@@ -37,14 +38,17 @@
             obj = str.__new__(cls, f"{prefixes[prefix]}{ns}")
         else:
             obj = str.__new__(cls, value)
 
         obj.prefixes = prefixes
         return obj
 
+    def __getnewargs__(self) -> tuple[str, dict[str, str]]:
+        return str(self), self.prefixes
+
     def get_rel_uri(self):
         for prefix, uri in self.prefixes.items():
             if self.startswith(uri):
                 return f"{prefix}:{self.replace(uri, '')}"
         raise ValueError(
             "Cannot create relative URI because there is no suitable prefix"
         )
```

### Comparing `drepr_v2-1.1.3/drepr/planning/class_map_plan.py` & `drepr_v2-1.2.1/drepr/planning/class_map_plan.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from copy import deepcopy
 from dataclasses import dataclass
 from typing import Any, Optional, TypeAlias, cast
 
 from drepr.models.prelude import (
     DREPR_URI,
     MISSING_VALUE_TYPE,
     Alignment,
@@ -12,27 +13,32 @@
     Cardinality,
     ClassNode,
     DataNode,
     DRepr,
     EdgeId,
     LiteralNode,
     NodeId,
+    Resource,
 )
+from drepr.models.sm import DREPR_BLANK
 from drepr.planning.drepr_model_alignments import DReprModelAlignments
 from drepr.planning.topological_sorting import topological_sorting
 
 
 @dataclass
 class ClassesMapExecutionPlan:
+    desc: DRepr
     # read_plans: list[ReadPlan]
     # write_plan: WritePlan
     class_map_plans: list[ClassMapPlan]
 
-    @staticmethod
-    def create(desc: DRepr):
+    @classmethod
+    def create(cls, desc: DRepr):
+        desc = cls.rewrite_desc_for_preprocessing_output(desc)
+
         reversed_topo_orders = topological_sorting(desc.sm)
         alignments = DReprModelAlignments.create(desc)
         edges_optional = {e.edge_id: not e.is_required for e in desc.sm.edges.values()}
         edges_has_missing_values: dict[EdgeId, bool] = {}
         class_map_plans = []
         class2plan = {}
 
@@ -130,24 +136,48 @@
         ), f"{len(edges_has_missing_values)} == {len(desc.sm.edges)} - {sum(reversed_topo_orders.removed_outgoing_edges.values())}"
 
         # generate plans
         for class_id in reversed_topo_orders.topo_order:
             classplan = ClassMapPlan.create(
                 desc,
                 class_id,
+                class2plan,
                 class2subj,
                 alignments,
                 edges_optional,
                 edges_has_missing_values,
                 reversed_topo_orders.removed_outgoing_edges,
             )
             class2plan[class_id] = classplan
             class_map_plans.append(classplan)
 
-        return ClassesMapExecutionPlan(class_map_plans)
+        return ClassesMapExecutionPlan(desc, class_map_plans)
+
+    @classmethod
+    def rewrite_desc_for_preprocessing_output(cls, desc: DRepr):
+        if all(not pre.is_output_new_data() for pre in desc.preprocessing):
+            return desc
+
+        desc = deepcopy(desc)
+        assert all(not r.is_preprocessing_output() for r in desc.resources)
+        for pre in desc.preprocessing:
+            if not pre.is_output_new_data():
+                continue
+
+            attr = pre.get_new_data_attribute("")
+            newresource = Resource.create_preprocessing_output(attr.id)
+            attr.resource_id = newresource.id
+
+            assert not desc.has_attr(
+                attr.id
+            ), f"Preprocessing attempts to write to an existing attribute: {attr.id}. Please change the output attribute id"
+            desc.attrs.append(attr)
+            desc.add_resource(newresource)
+
+        return desc
 
 
 @dataclass
 class ClassMapPlan:
     class_id: str
     subject: Subject
     data_props: list[DataProp]
@@ -155,41 +185,51 @@
     object_props: list[ObjectProp]
     buffered_object_props: list[ObjectProp]
 
     @staticmethod
     def create(
         desc: DRepr,
         class_id: NodeId,
+        class2plan: dict[NodeId, ClassMapPlan],
         class2subj: dict[NodeId, AttrId],
         inference: DReprModelAlignments,
         edges_optional: dict[EdgeId, bool],
         edges_missing_values: dict[EdgeId, bool],
         removed_edges: dict[EdgeId, bool],
     ):
         subj = class2subj[class_id]
         uri_dnode: Optional[DataNode] = None
+        blank_dnode: Optional[DataNode] = None
         for e in desc.sm.iter_outgoing_edges(class_id):
-            if e.get_abs_iri(desc.sm) == DREPR_URI:
+            e_abs_uri = e.get_abs_iri(desc.sm)
+            if e_abs_uri == DREPR_URI:
+                assert uri_dnode is None
                 tmp = desc.sm.nodes[e.target_id]
                 assert isinstance(tmp, DataNode)
                 uri_dnode = tmp
-                break
+            elif e_abs_uri == DREPR_BLANK:
+                assert blank_dnode is None
+                tmp = desc.sm.nodes[e.target_id]
+                assert isinstance(tmp, DataNode)
+                blank_dnode = tmp
+
+        assert not (uri_dnode is not None and blank_dnode is not None)
 
         # generate other properties
         literal_props = []
         data_props: list[DataProp] = []
         object_props = []
         buffered_object_props = []
 
         for e in desc.sm.iter_outgoing_edges(class_id):
             target = desc.sm.nodes[e.target_id]
             if isinstance(target, DataNode):
                 attribute = desc.get_attr_by_id(target.attr_id)
-
-                if e.get_abs_iri(desc.sm) != DREPR_URI:
+                e_abs_iri = e.get_abs_iri(desc.sm)
+                if e_abs_iri != DREPR_URI and e_abs_iri != DREPR_BLANK:
                     alignments = inference.get_alignments(subj, target.attr_id)
                     alignments_cardinality = inference.estimate_cardinality(alignments)
 
                     if attribute.value_type.is_list():
                         if alignments_cardinality.is_one_to_star():
                             alignments_cardinality = Cardinality.OneToMany
                         else:
@@ -205,41 +245,62 @@
                                 alignments
                             ),
                             predicate=e.get_abs_iri(desc.sm),
                             attr=attribute,
                             is_optional=edges_optional[e.edge_id],
                             missing_values=set(attribute.missing_values),
                             missing_path=attribute.path.has_optional_steps(),
-                            datatype=(
-                                target.data_type
-                                if target.data_type is not None
-                                else None
-                            ),
+                            datatype=(target.data_type),
                         )
                     )
             elif isinstance(target, LiteralNode):
                 literal_props.append(
-                    LiteralProp(predicate=e.get_abs_iri(desc.sm), value=target.value)
+                    LiteralProp(
+                        predicate=e.get_abs_iri(desc.sm),
+                        value=target.value,
+                        datatype=target.data_type,
+                    )
                 )
             elif isinstance(target, ClassNode):
                 attribute = desc.get_attr_by_id(class2subj[e.target_id])
 
                 alignments = inference.get_alignments(subj, attribute.id)
 
                 if target.is_blank_node(desc.sm):
+                    if any(
+                        etmp.get_abs_iri(desc.sm) == DREPR_BLANK
+                        for etmp in desc.sm.iter_outgoing_edges(target.node_id)
+                    ):
+                        # ensure that it is consistent
+                        assert (
+                            target.node_id in class2plan
+                            and isinstance(
+                                (
+                                    targetclsplansubj := class2plan[
+                                        target.node_id
+                                    ].subject
+                                ),
+                                BlankSubject,
+                            )
+                            and targetclsplansubj.use_attr_value
+                        )
+                        use_attr_value = True
+                    else:
+                        use_attr_value = False
                     prop = BlankObject(
                         attr=attribute,
                         alignments_cardinality=inference.estimate_cardinality(
                             alignments
                         ),
                         alignments=alignments,
                         predicate=e.get_abs_iri(desc.sm),
                         class_id=class_id,
                         is_optional=edges_optional[e.edge_id],
                         can_target_missing=edges_missing_values[e.edge_id],
+                        use_attr_value=use_attr_value,
                     )
                 else:
                     prop = IDObject(
                         attr=attribute,
                         alignments_cardinality=inference.estimate_cardinality(
                             alignments
                         ),
@@ -255,16 +316,20 @@
                     buffered_object_props.append(prop)
                 else:
                     object_props.append(prop)
 
         subj_attr = desc.get_attr_by_id(subj)
 
         if uri_dnode is None:
+            if blank_dnode is not None:
+                assert blank_dnode.attr_id == subj
             subject = BlankSubject(
                 attr=subj_attr,
+                use_attr_value=blank_dnode is not None,
+                missing_values=set(subj_attr.missing_values),
             )
         else:
             # get missing values from the real subjects
             missing_values = set(subj_attr.missing_values)
             (uri_dnode_inedge,) = [
                 e
                 for e in desc.sm.get_edges_between_nodes(class_id, uri_dnode.node_id)
@@ -305,24 +370,32 @@
 
         The subject has *-to-one relationship with other attributes.
         """
         # get data nodes, attributes, and the attribute that contains URIs of the class
         data_nodes: list[DataNode] = []
         attrs: list[AttrId] = []
         uri_attr: Optional[AttrId] = None
+        blank_attr: Optional[AttrId] = None
 
         for e in desc.sm.iter_outgoing_edges(class_id):
             target = desc.sm.nodes[e.target_id]
 
             if isinstance(target, DataNode):
                 data_nodes.append(target)
                 attrs.append(target.attr_id)
 
-                if e.get_abs_iri(desc.sm) == DREPR_URI:
+                e_abs_iri = e.get_abs_iri(desc.sm)
+                if e_abs_iri == DREPR_URI:
+                    assert uri_attr is None
                     uri_attr = target.attr_id
+                elif e_abs_iri == DREPR_BLANK:
+                    assert blank_attr is None
+                    blank_attr = target.attr_id
+
+        assert not (uri_attr is not None and blank_attr is not None)
 
         # if the subject attribute is provided, then, we will use it.
         subjs = []
         for u in data_nodes:
             if any(
                 e.is_subject
                 for e in desc.sm.get_edges_between_nodes(class_id, u.node_id)
@@ -349,32 +422,41 @@
         if len(subjs) == 0:
             raise Exception(
                 "There is no subject attribute of class: {} ({}). Users need to specify it explicitly".format(
                     cast(ClassNode, desc.sm.nodes[class_id]).label, class_id
                 )
             )
 
-        return ClassMapPlan.select_subject(desc, class_id, subjs, attrs, uri_attr)
+        return ClassMapPlan.select_subject(
+            desc, class_id, subjs, attrs, uri_attr, blank_attr
+        )
 
     @staticmethod
     def select_subject(
         desc: DRepr,
         class_id: NodeId,
         subjs: list[AttrId],
         attrs: list[AttrId],
         uri_attr: Optional[AttrId],
+        blank_attr: Optional[AttrId],
     ) -> AttrId:
         if uri_attr is not None and uri_attr in subjs:
             return uri_attr
+        if blank_attr is not None and blank_attr in subjs:
+            return blank_attr
         return subjs[0]
 
 
 @dataclass
 class BlankSubject:
     attr: Attr
+    # whether to use the attribute value as the value of the subject
+    use_attr_value: bool
+    # only works when use_attr_value is True
+    missing_values: set[MISSING_VALUE_TYPE]
 
 
 @dataclass
 class InternalIDSubject:
     attr: Attr
     is_optional: bool
     missing_values: set[MISSING_VALUE_TYPE]
@@ -406,26 +488,29 @@
         return len(self.missing_values) > 0 or self.missing_path
 
 
 @dataclass
 class LiteralProp:
     predicate: str
     value: Any
+    datatype: Optional[str]
 
 
 @dataclass
 class BlankObject:
     attr: Attr
     alignments: list[Alignment]
     alignments_cardinality: Cardinality
     predicate: str
     class_id: NodeId
     is_optional: bool
     # whether an instance of the target class can be missing
     can_target_missing: bool
+    # whether to use the attribute value as the value of the blank object
+    use_attr_value: bool
 
 
 @dataclass
 class IDObject:
     attr: Attr
     alignments: list[Alignment]
     alignments_cardinality: Cardinality
```

### Comparing `drepr_v2-1.1.3/drepr/planning/drepr_model_alignments.py` & `drepr_v2-1.2.1/drepr/planning/drepr_model_alignments.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,32 +58,32 @@
                             aligns[(target.id, source.id)] = [new_align.swap()]
             elif isinstance(a, IdenticalAlign):
                 raise Exception(
                     "Unreachable! Users should not provide identical alignment in the model"
                 )
 
         for a in desc.attrs:
-            aligns[(a.id, a.id)] = [IdenticalAlign()]
+            aligns[(a.id, a.id)] = [IdenticalAlign(a.id, a.id)]
 
         inf = DReprModelAlignments(desc, aligns)
         inf.inference()
         return inf
 
     def get_alignments(self, source: AttrId, target: AttrId) -> list[Alignment]:
         return self.aligns[(source, target)]
 
     def inference(self):
         ig: dict[str, dict[str, int]] = {
             attr.id: {attr.id: 0} for attr in self.desc.attrs
         }
         for (source, target), aligns in self.aligns.items():
             assert len(aligns) <= 1, aligns
-            if len(aligns) == 0:
+            if source == target or len(aligns) == 0:
                 continue
-            if isinstance(aligns[0], (RangeAlignment, ValueAlignment)):
+            if isinstance(aligns[0], (RangeAlignment, ValueAlignment, IdenticalAlign)):
                 ig[source][target] = sum(
                     self.score_alignment(align) for align in aligns
                 )
             elif not isinstance(aligns[0], IdenticalAlign):
                 print(aligns)
                 raise Exception("Unreachable")
 
@@ -304,26 +304,42 @@
                 )
             else:
                 joins.append(align)
 
         return joins
 
     @staticmethod
-    def auto_align(source: Attr, target: Attr) -> Optional[RangeAlignment]:
+    def auto_align(
+        source: Attr, target: Attr
+    ) -> Optional[RangeAlignment | IdenticalAlign]:
+        # TODO: fix auto-alignment
         source_range_steps = [
             i for i, step in enumerate(source.path.steps) if isinstance(step, RangeExpr)
         ]
         target_range_steps = [
             i for i, step in enumerate(target.path.steps) if isinstance(step, RangeExpr)
         ]
 
         if len(source_range_steps) == 0 or len(target_range_steps) == 0:
+            # mapping between two single values is identical mapping
+            is_source_single_val = all(
+                isinstance(step, IndexExpr) for step in source.path.steps
+            )
+            is_target_single_val = all(
+                isinstance(step, IndexExpr) for step in target.path.steps
+            )
+            if is_source_single_val and is_target_single_val:
+                return IdenticalAlign(source.id, target.id)
+
+            if is_source_single_val or is_target_single_val:
+                return RangeAlignment(source.id, target.id, [])
             return None
 
-        end = min(source_range_steps[-1], target_range_steps[-1])
+        end = min(source_range_steps[-1], target_range_steps[-1]) + 1
+        assert end > 0
 
         if source.path.steps[:end] == target.path.steps[:end]:
             # we can align all of them as long as all the steps are index
             if all(
                 isinstance(step, (RangeExpr, IndexExpr, SetIndexExpr))
                 for step in source.path.steps
             ) and all(
@@ -331,15 +347,17 @@
                 for step in target.path.steps
             ):
                 return RangeAlignment(
                     source=source.id,
                     target=target.id,
                     aligned_steps=[
                         AlignedStep(source_idx=dim, target_idx=dim)
-                        for dim in source_range_steps
+                        for dim in source_range_steps[
+                            : min(len(target_range_steps), len(source_range_steps))
+                        ]
                     ],
                 )
 
         return None
 
     def score_alignment(self, align: Alignment) -> int:
         """Score an alignment function so we can justify if an alignment is new/better or not. Lower score is better."""
```

### Comparing `drepr_v2-1.1.3/drepr/planning/topological_sorting.py` & `drepr_v2-1.2.1/drepr/planning/topological_sorting.py`

 * *Files 16% similar despite different names*

```diff
@@ -34,30 +34,20 @@
                 has_unvisited_node = True
                 break
 
         if not has_unvisited_node:
             # we don't have any unvisited node left, so we finish!
             break
 
-        # preparing the data
-        for k in tmp_visited_nodes:
-            tmp_visited_nodes[k] = False
-
         # loop until it breaks all cycles
-        while dfs_breaking_cycle(
-            sm, random_start_node, tmp_visited_nodes, removed_outgoing_edges
-        ):
-            # reset the tmp visited nodes
-            for k in tmp_visited_nodes:
-                tmp_visited_nodes[k] = False
-
-        # mark visited nodes
-        for uid, is_visited in tmp_visited_nodes.items():
-            if is_visited:
-                visited_nodes[uid] = True
+        while dfs_breaking_cycle(sm, random_start_node, [], removed_outgoing_edges):
+            pass
+
+        # mark visited nodes so that we can just skip them
+        reverse_dfs(sm, random_start_node, visited_nodes, removed_outgoing_edges)
 
     # now we get acyclic graph, determine the topo-order
     reversed_topo_order = []
     for uid in sm.nodes:
         visited_nodes[uid] = False
         tmp_visited_nodes[uid] = False
 
@@ -116,29 +106,43 @@
     visited_nodes[node] = True
     topo_order.append(node)
 
 
 def dfs_breaking_cycle(
     sm: SemanticModel,
     node: str,
-    visited_nodes: dict[str, bool],
+    visited_path: list[str],
     removed_outgoing_edges: dict[int, bool],
 ) -> bool:
     """
     Try to break cycles using invert DFS. It returns true when break one cycle, and it terminates
     immediately. Thus, requires you to run this function many times until it return false
     """
-    visited_nodes[node] = True
+    visited_path.append(node)
 
     for e in sm.iter_incoming_edges(node):
         if not removed_outgoing_edges[e.edge_id]:
-            if visited_nodes[e.source_id]:
-                # this node is visited, and it is visited by traveling through `e`, we can drop `e` and move on
+            if e.source_id in visited_path:
+                # this node is visited before in the path, and it is visited by traveling through `e`, we can drop `e` and move on
                 removed_outgoing_edges[e.edge_id] = True
                 return True
 
             if dfs_breaking_cycle(
-                sm, e.source_id, visited_nodes, removed_outgoing_edges
+                sm, e.source_id, visited_path, removed_outgoing_edges
             ):
                 return True
 
+    visited_path.pop()
     return False
+
+
+def reverse_dfs(
+    sm: SemanticModel,
+    node: str,
+    visited_nodes: dict[str, bool],
+    removed_outgoing_edges: dict[int, bool],
+) -> bool:
+    """Reverse DFS to visit all ancestors of a node"""
+    visited_nodes[node] = True
+    for e in sm.iter_incoming_edges(node):
+        if not removed_outgoing_edges[e.edge_id]:
+            reverse_dfs(sm, e.source_id, visited_nodes, removed_outgoing_edges)
```

### Comparing `drepr_v2-1.1.3/drepr/program_generation/alignment_fn.py` & `drepr_v2-1.2.1/drepr/program_generation/alignment_fn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
 
-from typing import Any, Callable, Literal, Optional
-
-from codegen.models import AST, DeferredVar, PredefinedFn, Program, Var, expr, stmt
+from typing import Any, Callable, Literal, Optional, Protocol
 
 import drepr.models.path as path
+from codegen.models import AST, DeferredVar, PredefinedFn, Program, Var, expr, stmt
 from drepr.models.align import IdenticalAlign
 from drepr.models.prelude import Alignment, Attr, DRepr, RangeAlignment
 from drepr.program_generation.predefined_fn import DReprPredefinedFn
 from drepr.program_generation.program_space import VarSpace
 
 
 class AlignmentFn:
@@ -27,16 +26,33 @@
     ):
         for align in aligns:
             if isinstance(align, RangeAlignment):
                 ast = self.align_by_range(
                     ast, align, validate_path, on_missing_key, iter_final_list
                 )
             elif isinstance(align, IdenticalAlign):
-                # this is the alignment between the same attribute
-                continue
+                # if this is the alignment between the same attribute -- do nothing
+                if align.source == align.target:
+                    continue
+
+                # the two attributes are different, but they have identical align, it means that they are single-value attributes
+                # we just need to access the value of the target attribute
+                target = self.desc.get_attr_by_id(align.target)
+                assert all(
+                    isinstance(step, path.IndexExpr) for step in target.path.steps
+                )
+                ast = PathAccessor(self.program).iterate_elements(
+                    ast,
+                    target,
+                    aligned_attr=None,
+                    to_aligned_dim=None,
+                    validate_path=validate_path,
+                    on_missing_key=on_missing_key,
+                    iter_final_list=iter_final_list,
+                )
             else:
                 raise NotImplementedError(type(align))
         return ast
 
     def align_by_range(
         self,
         ast: AST,
@@ -78,25 +94,27 @@
         ast: AST,
         attr: Attr,
         aligned_attr: Optional[Attr] = None,
         to_aligned_dim: Optional[dict[int, int]] = None,
         validate_path: bool = False,
         on_missing_key: Optional[Callable[[AST], Any]] = None,
         iter_final_list: bool = False,
+        on_step_callback: Optional[OnStepCallback] = None,
     ):
         ast = ast.update_recursively(
             fn=lambda ast, dim: self.next_dimensions(
                 ast,
                 attr,
                 dim,
                 aligned_attr,
                 to_aligned_dim,
                 validate_path,
                 on_missing_key,
                 iter_final_list,
+                on_step_callback,
             ),
             context=0,
         )
         return ast
 
     def next_dimensions(
         self,
@@ -104,14 +122,15 @@
         attr: Attr,
         dim: int,
         aligned_attr: Optional[Attr],
         to_aligned_dim: Optional[dict[int, int]],
         validate_path: bool,
         on_missing_key: Optional[Callable[[AST], Any]] = None,
         iter_final_list: bool = False,
+        on_step_callback: Optional[OnStepCallback] = None,
     ):
         """Generate code to access elements of dimensions of attr started at dim.
         Return the next ast, remaining dimension index, and whether it has stopped.
 
         Args:
             mem: memory to store variables
             ast: current ast
@@ -119,14 +138,15 @@
             dim: starting dimension
             aligned_attr:
             to_aligned_dim:
             validate_path: whether to generate code to check if values of each dimension is correct. If the attribute
                 is annotated with `missing_path = True`, then setting this does not have any effect.
             on_missing_key: a function that will be called when the key does not exist. If it is None, then we will raise an exception.
             iter_final_list: if value type of attribute is a list, and this flag is true, we will iterate over the list to yield each item
+            on_step_callback: a function that can be called to generate code at each time we step into a new dimension (except dimension 0, which is the resource data)
         """
         n_dim = len(attr.path.steps)
         if attr.value_type.is_list() and iter_final_list:
             n_dim += 1
 
         if dim >= n_dim:
             return ast, dim, True
@@ -145,24 +165,25 @@
             # we are iterating over the value list
             step = path.RangeExpr(0, None, 1)
         else:
             step = attr.path.steps[dim]
 
         # index expr does not need nested ast.
         while isinstance(step, path.IndexExpr) and dim < len(attr.path.steps):
+            if isinstance(step.val, path.Expr):
+                # I don't know about recursive path expression yet -- what usecase and how to use them -- so I can't implement.
+                raise Exception(
+                    f"Recursive path expression is not supported yet. Please raise a ticket to notify us for future support! Found: {step.val}"
+                )
+
             # we do not need nested loop for index expression as we can just directly access the value
             c1 = DeferredVar(
                 name=f"{attr.id}_value_{dim}",
                 key=VarSpace.attr_value_dim(attr.resource_id, attr.id, dim),
             )
-            if isinstance(step.val, path.Expr):
-                # I don't know about recursive path expression yet.
-                raise Exception(
-                    f"Recursive path expression is not supported yet. Please raise a ticket to notify us for future support! Found: {step.val}"
-                )
 
             if validate_path and not attr.path.is_step_optional(dim):
                 handle_missing_key = "safe"
             elif attr.path.is_step_optional(dim):
                 assert on_missing_key is not None
                 handle_missing_key = on_missing_key
             else:
@@ -172,14 +193,15 @@
                 ast,
                 attr,
                 expr.ExprVar(collection),
                 expr.ExprConstant(step.val),
                 c1,
                 dim,
                 handle_missing_key,
+                on_step_callback,
             )
 
             collection = c1.get_var()
             dim += 1
             if dim == len(attr.path.steps):
                 # we have reached the end of the path
                 # however, if the value type is a list, and we enable iter_final_list,
@@ -236,14 +258,22 @@
                 else:
                     invok_item_getter = PredefinedFn.item_getter(
                         expr.ExprVar(collection), expr.ExprVar(itemindex)
                     )
 
                 ast.assign(itemvalue, invok_item_getter)
                 itemvalue = itemvalue.get_var()
+                if on_step_callback is not None:
+                    on_step_callback(
+                        ast,
+                        dim,
+                        expr.ExprVar(collection),
+                        expr.ExprVar(itemindex),
+                        itemvalue,
+                    )
             else:
                 # the dimension is not bound, we are going to generate multiple values
                 # using a for loop
                 start_var = DeferredVar(
                     name=f"start",
                     key=("local-var", "start", f"attr={attr.id}", f"ast={ast.id}"),
                 )
@@ -328,14 +358,22 @@
                 ast.assign(
                     itemvalue,
                     PredefinedFn.item_getter(
                         expr.ExprVar(collection), expr.ExprVar(itemindex)
                     ),
                 )
                 itemvalue = itemvalue.get_var()
+                if on_step_callback is not None:
+                    on_step_callback(
+                        ast,
+                        dim,
+                        expr.ExprVar(collection),
+                        expr.ExprVar(itemindex),
+                        itemvalue,
+                    )
             return (
                 ast,
                 dim + 1,
                 False,
             )
 
         raise NotImplementedError(step)
@@ -345,17 +383,20 @@
         ast: AST,
         attr: Attr,
         collection: expr.Expr,
         key: expr.ExprConstant,
         result: DeferredVar | Var,
         dim: int,
         handle_missing_key: Literal["safe", "no_missing_key"] | Callable[[AST], None],
+        on_step_callback: Optional[OnStepCallback] = None,
     ):
         if handle_missing_key == "no_missing_key":
             ast.assign(result, PredefinedFn.item_getter(collection, key))
+            if on_step_callback is not None:
+                on_step_callback(ast, dim, collection, key, result)
             return ast
 
         if handle_missing_key == "safe":
             ast.assign(
                 result,
                 DReprPredefinedFn.safe_item_getter(
                     self.program,
@@ -363,16 +404,32 @@
                     key,
                     expr.ExprConstant(
                         f"While traveling elements of attribute {attr.id}, encounter key error: "
                         + f"key {key.constant} does not exist (key position = {dim} - full path = {attr.path.to_lang_format()})"
                     ),
                 ),
             )
+            if on_step_callback is not None:
+                on_step_callback(ast, dim, collection, key, result)
             return ast
 
         ast.if_(expr.ExprNegation(PredefinedFn.has_item(collection, key)))(
             # if the key does not exist, we call the function to handle it
+            # because we do not step in -- we don't invoke the callback here
             handle_missing_key
         )
         inner_ast = ast.else_()
         inner_ast.assign(result, PredefinedFn.item_getter(collection, key))
+        if on_step_callback is not None:
+            on_step_callback(inner_ast, dim, collection, key, result)
         return inner_ast
+
+
+class OnStepCallback(Protocol):
+    def __call__(
+        self,
+        ast: AST,
+        dim: int,
+        collection: expr.Expr,
+        key: expr.Expr,
+        result: DeferredVar | Var,
+    ): ...
```

### Comparing `drepr_v2-1.1.3/drepr/program_generation/main.py` & `drepr_v2-1.2.1/drepr/program_generation/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     BlankSubject,
     ClassesMapExecutionPlan,
     ClassMapPlan,
     DataProp,
     ExternalIDSubject,
     IDObject,
     InternalIDSubject,
+    LiteralProp,
     ObjectProp,
 )
 from drepr.program_generation.alignment_fn import AlignmentFn, PathAccessor
 from drepr.program_generation.predefined_fn import DReprPredefinedFn
 from drepr.program_generation.preprocessing import GenPreprocessing
 from drepr.program_generation.program_space import VarSpace
 from drepr.program_generation.writers import Writer
@@ -47,29 +48,39 @@
     desc: DRepr, exec_plan: ClassesMapExecutionPlan, output: Output, debuginfo: bool
 ) -> AST:
     """Generate a program to convert the given D-REPR to a target format"""
     program = Program()
     writer = Writer(desc, output.format, program)
 
     func_args = [
-        DeferredVar(name="resource", key=VarSpace.resource(res.id))
+        DeferredVar(
+            name="resource" if len(desc.resources) == 1 else f"resource_{res.id}",
+            key=VarSpace.resource(res.id),
+        )
         for res in desc.resources
+        if not res.is_preprocessing_output()
     ]
     if isinstance(output, FileOutput):
         output_file = DeferredVar(name="output_file", key=VarSpace.output_file())
         func_args.append(output_file)
     else:
         output_file = None
 
     program.root.linebreak()
     main_fn = program.root.func("main", func_args)
 
     for resource in desc.resources:
+        if resource.is_preprocessing_output():
+            continue
         var = DeferredVar(
-            name="resource_data",
+            name=(
+                "resource_data"
+                if len(desc.resources) == 1
+                else f"resource_data_{resource.id}"
+            ),
             key=VarSpace.resource_data(resource.id),
         )
         main_fn.assign(
             var,
             DReprPredefinedFn.read_source(
                 program,
                 resource.type,
@@ -84,15 +95,15 @@
     for attr in desc.attrs:
         if len(attr.missing_values) > 0:
             main_fn.assign(
                 DeferredVar(
                     name=f"{attr.id}_missing_values",
                     key=VarSpace.attr_missing_values(attr.id),
                 ),
-                expr.ExprConstant(attr.missing_values),
+                expr.ExprConstant(set(attr.missing_values)),
             )
 
     # create transformation
     GenPreprocessing(program, desc, main_fn).generate()
 
     # create a writer
     writer.create_writer(main_fn)
@@ -198,19 +209,19 @@
     is_subj_blank = isinstance(classplan.subject, BlankSubject)
     can_class_missing = (
         any(
             not dprop.is_optional and dprop.can_target_missing
             for dprop in classplan.data_props
         )
         or any(
-            not oprop.is_optional and not oprop.can_target_missing
+            not oprop.is_optional and oprop.can_target_missing
             for oprop in classplan.object_props
         )
         or any(
-            not oprop.is_optional and not oprop.can_target_missing
+            not oprop.is_optional and oprop.can_target_missing
             for oprop in classplan.buffered_object_props
         )
     )
     is_buffered = can_class_missing
 
     get_subj_val: Callable[[AST], expr.Expr]
     if isinstance(classplan.subject, (InternalIDSubject, ExternalIDSubject)):
@@ -221,44 +232,68 @@
                     classplan.subject.attr.id,
                     len(classplan.subject.attr.path.steps) - 1,
                 ),
                 at=ast.next_child_id(),
             )
         )
     else:
-        # if this is a blank node, the subj_val is the entire index that leads to the last value
-        get_subj_val = lambda ast: (
-            PredefinedFn.tuple(
+        assert isinstance(classplan.subject, BlankSubject)
+        if classplan.subject.use_attr_value:
+            get_subj_val = lambda ast: PredefinedFn.tuple(
                 [
                     expr.ExprConstant(
                         desc.get_attr_index_by_id(classplan.subject.attr.id)
-                    )
-                ]
-                + [
+                    ),
                     expr.ExprVar(
                         program.get_var(
-                            key=VarSpace.attr_index_dim(
+                            key=VarSpace.attr_value_dim(
                                 classplan.subject.attr.resource_id,
                                 classplan.subject.attr.id,
-                                dim,
+                                len(classplan.subject.attr.path.steps) - 1,
                             ),
                             at=ast.next_child_id(),
                         )
-                    )
-                    for dim, step in enumerate(classplan.subject.attr.path.steps)
-                    if not isinstance(step, IndexExpr)
+                    ),
                 ]
             )
-        )
+        else:
+            # if we don't use attr value, the subj_val is the entire index that leads to the last value
+            get_subj_val = lambda ast: (
+                PredefinedFn.tuple(
+                    [
+                        expr.ExprConstant(
+                            desc.get_attr_index_by_id(classplan.subject.attr.id)
+                        )
+                    ]
+                    + [
+                        expr.ExprVar(
+                            program.get_var(
+                                key=VarSpace.attr_index_dim(
+                                    classplan.subject.attr.resource_id,
+                                    classplan.subject.attr.id,
+                                    dim,
+                                ),
+                                at=ast.next_child_id(),
+                            )
+                        )
+                        for dim, step in enumerate(classplan.subject.attr.path.steps)
+                        if not isinstance(step, IndexExpr)
+                    ]
+                )
+            )
 
     if (
         isinstance(classplan.subject, (InternalIDSubject, ExternalIDSubject))
         and len(classplan.subject.attr.missing_values) > 0
+    ) or (
+        isinstance(classplan.subject, BlankSubject)
+        and classplan.subject.use_attr_value
+        and len(classplan.subject.attr.missing_values) > 0
     ):
-        # we know immediately that it's missing if the URI is missing
+        # we know immediately that it's missing if the subject value is missing
 
         if ast.id == parent_ast.id:
             # same ast because of a single value, we can't use continue
             # so we wrap it with if -- if not missing, continue to generate the instance
             ast = ast.if_(
                 expr.ExprNegation(
                     PredefinedFn.set_contains(
@@ -298,64 +333,89 @@
     for dataprop in classplan.data_props:
         ast.linebreak()
         ast.comment(f"Retrieve value of data property: {dataprop.attr.id}")
 
         gen_classprop_body(
             program,
             desc,
-            ast,
+            parent_ast,
+            ast.block(),
             writer,
             is_buffered,
             is_subj_blank,
             dataprop,
             debuginfo,
         )
 
     for objprop in classplan.object_props:
         ast.linebreak()
         ast.comment(f"Retrieve value of object property: {objprop.attr.id}")
 
         gen_classprop_body(
             program,
             desc,
-            ast,
+            parent_ast,
+            ast.block(),
             writer,
             is_buffered,
             is_subj_blank,
             objprop,
             debuginfo,
         )
 
+    if len(classplan.literal_props) > 0:
+        ast.linebreak()
+        ast.comment("Set static properties")
+
+        for litprop in classplan.literal_props:
+            gen_classprop_body(
+                program,
+                desc,
+                parent_ast,
+                ast.block(),
+                writer,
+                is_buffered,
+                is_subj_blank,
+                litprop,
+                debuginfo,
+            )
+
     assert len(classplan.buffered_object_props) == 0, "Not implemented yet"
 
     # we can end the record even if we abort it before. the end record code should handle this.
     ast.linebreak()
 
     if isinstance(classplan.subject, BlankSubject) and can_class_missing:
         ast.if_(writer.is_record_empty(ast))(lambda ast00: writer.abort_record(ast00))
+        ast.else_()(lambda ast00: writer.end_record(ast00))
     else:
         writer.end_record(ast)
 
     return ast
 
 
 def gen_classprop_body(
     program: Program,
     desc: DRepr,
+    parent_ast: AST,
     ast: AST,
     writer: Writer,
     is_buffered: bool,
     is_subj_blank: bool,
-    classprop: DataProp | ObjectProp,
+    classprop: DataProp | ObjectProp | LiteralProp,
     debuginfo: bool,
 ):
-    attr = classprop.attr
+    """
+    Args:
+        parent_ast: the parent AST that above iterating subject values -- this is good to detect continue statement is okay to skip to the next subject/record
+    """
     iter_final_list = False
     get_prop_val: Callable[[AST], expr.Expr]
     if isinstance(classprop, (DataProp, IDObject)):
+        attr = classprop.attr
         if isinstance(classprop, DataProp) and classprop.attr.value_type.is_list():
             # for a list, we need to iterate over the list.
             get_prop_val = lambda ast: expr.ExprVar(
                 program.get_var(
                     key=VarSpace.attr_value_dim(
                         attr.resource_id,
                         attr.id,
@@ -374,159 +434,219 @@
                         attr.resource_id,
                         attr.id,
                         len(attr.path.steps) - 1,
                     ),
                     at=ast.next_child_id(),
                 )
             )
-    else:
-        assert isinstance(classprop, BlankObject)
-        get_prop_val = lambda ast: (
-            PredefinedFn.tuple(
-                [expr.ExprConstant(desc.get_attr_index_by_id(classprop.attr.id))]
-                + [
+    elif isinstance(classprop, BlankObject):
+        attr = classprop.attr
+        if classprop.use_attr_value:
+            get_prop_val = lambda ast: PredefinedFn.tuple(
+                [
+                    expr.ExprConstant(desc.get_attr_index_by_id(attr.id)),
                     expr.ExprVar(
                         program.get_var(
-                            key=VarSpace.attr_index_dim(
-                                classprop.attr.resource_id,
-                                classprop.attr.id,
-                                dim,
+                            key=VarSpace.attr_value_dim(
+                                attr.resource_id,
+                                attr.id,
+                                len(attr.path.steps) - 1,
                             ),
                             at=ast.next_child_id(),
                         )
-                    )
-                    for dim, step in enumerate(classprop.attr.path.steps)
-                    if not isinstance(step, IndexExpr)
+                    ),
                 ]
             )
-        )
+        else:
+            get_prop_val = lambda ast: (
+                PredefinedFn.tuple(
+                    [expr.ExprConstant(desc.get_attr_index_by_id(classprop.attr.id))]
+                    + [
+                        expr.ExprVar(
+                            program.get_var(
+                                key=VarSpace.attr_index_dim(
+                                    classprop.attr.resource_id,
+                                    classprop.attr.id,
+                                    dim,
+                                ),
+                                at=ast.next_child_id(),
+                            )
+                        )
+                        for dim, step in enumerate(classprop.attr.path.steps)
+                        if not isinstance(step, IndexExpr)
+                    ]
+                )
+            )
+    else:
+        assert isinstance(classprop, LiteralProp)
+        get_prop_val = lambda ast: expr.ExprConstant(classprop.value)
 
     is_prop_val_not_missing: Callable[[AST], expr.Expr]
     if isinstance(classprop, DataProp):
         if len(attr.missing_values) == 0:
             # leverage the fact that if True will be optimized away
             is_prop_val_not_missing = lambda ast: expr.ExprConstant(True)
         else:
-            is_prop_val_not_missing = lambda ast: PredefinedFn.set_contains(
-                expr.ExprNegation(
+            is_prop_val_not_missing = lambda ast: expr.ExprNegation(
+                PredefinedFn.set_contains(
                     expr.ExprVar(
                         program.get_var(
                             key=VarSpace.attr_missing_values(attr.id),
                             at=ast.next_child_id(),
                         )
-                    )
+                    ),
+                    get_prop_val(ast),
                 ),
-                get_prop_val(ast),
             )
         write_fn = partial(
             writer.write_data_property, dtype=expr.ExprConstant(classprop.datatype)
         )
-    else:
-        assert isinstance(classprop, ObjectProp)
+    elif isinstance(classprop, ObjectProp):
         is_prop_val_not_missing = lambda ast: writer.has_written_record(
             ast,
             get_prop_val(ast),
         )
         write_fn = partial(
             writer.write_object_property,
             is_subject_blank=expr.ExprConstant(is_subj_blank),
             is_object_blank=expr.ExprConstant(isinstance(classprop, BlankObject)),
             is_new_subj=expr.ExprConstant(False),
         )
-
-    if not classprop.can_target_missing:
-        AlignmentFn(desc, program).align(
-            ast, classprop.alignments, debuginfo, None, iter_final_list
-        )(
-            lambda ast_l0: write_fn(
-                ast_l0,
-                expr.ExprConstant(classprop.predicate),
-                get_prop_val(ast_l0),
-            )
+    else:
+        assert isinstance(classprop, LiteralProp)
+        is_prop_val_not_missing = lambda ast: expr.ExprConstant(True)
+        write_fn = partial(
+            writer.write_data_property, dtype=expr.ExprConstant(classprop.datatype)
         )
+
+    if isinstance(classprop, LiteralProp):
+        write_fn(ast, expr.ExprConstant(classprop.predicate), get_prop_val(ast))
     else:
-        if classprop.is_optional:
+        if not classprop.can_target_missing:
             AlignmentFn(desc, program).align(
-                ast,
-                classprop.alignments,
-                debuginfo,
-                # if the value is missing, we just ignore it.
-                on_missing_key=lambda astxx: astxx(stmt.NoStatement()),
-                iter_final_list=iter_final_list,
+                ast, classprop.alignments, debuginfo, None, iter_final_list
             )(
-                lambda ast00: ast00.if_(is_prop_val_not_missing(ast00))(
-                    lambda ast01: write_fn(
-                        ast01,
-                        expr.ExprConstant(classprop.predicate),
-                        get_prop_val(ast01),
-                    )
+                lambda ast_l0: write_fn(
+                    ast_l0,
+                    expr.ExprConstant(classprop.predicate),
+                    get_prop_val(ast_l0),
                 )
             )
         else:
-            if classprop.alignments_cardinality.is_star_to_many():
-                has_dataprop_val = DeferredVar(
-                    name=f"{attr.id}_has_value_d{len(attr.path.steps) - 1}",
-                    key=VarSpace.has_attr_value_dim(
-                        attr.resource_id,
-                        attr.id,
-                        len(attr.path.steps) - 1,
-                    ),
-                )
-                ast.assign(has_dataprop_val, expr.ExprConstant(False))
-                has_dataprop_val = has_dataprop_val.get_var()
-
-                AlignmentFn(desc, program).align(
-                    ast,
-                    classprop.alignments,
-                    debuginfo,
-                    lambda astxx: astxx(stmt.NoStatement()),
-                    iter_final_list,
-                )(
-                    lambda ast00: ast00.if_(is_prop_val_not_missing(ast00))(
-                        lambda ast01: ast01.assign(
-                            has_dataprop_val, expr.ExprConstant(True)
-                        ),
-                        lambda ast02: write_fn(
-                            ast02,
-                            expr.ExprConstant(classprop.predicate),
-                            get_prop_val(ast02),
-                        ),
-                    )
-                )
-                ast.if_(expr.ExprNegation(expr.ExprVar(has_dataprop_val)))(
-                    lambda ast00: (
-                        assert_true(
-                            is_buffered,
-                            "We should only abort record if we are buffering",
-                        )
-                        and writer.abort_record(ast00)
-                    )
-                )
-            else:
+            if classprop.is_optional:
                 AlignmentFn(desc, program).align(
                     ast,
                     classprop.alignments,
                     debuginfo,
-                    on_missing_key=lambda astxx: assert_true(
-                        is_buffered,
-                        "We should only abort record if we are buffering",
-                    )
-                    and writer.abort_record(astxx),
+                    # if the value is missing, we just ignore it.
+                    on_missing_key=lambda astxx: astxx(stmt.NoStatement()),
                     iter_final_list=iter_final_list,
                 )(
                     lambda ast00: ast00.if_(is_prop_val_not_missing(ast00))(
                         lambda ast01: write_fn(
                             ast01,
                             expr.ExprConstant(classprop.predicate),
                             get_prop_val(ast01),
+                        )
+                    )
+                )
+            else:
+                if classprop.alignments_cardinality.is_star_to_many():
+                    has_dataprop_val = DeferredVar(
+                        name=f"{attr.id}_has_value_d{len(attr.path.steps) - 1}",
+                        key=VarSpace.has_attr_value_dim(
+                            attr.resource_id,
+                            attr.id,
+                            len(attr.path.steps) - 1,
                         ),
-                    ),
-                    lambda ast10: ast10.else_()(
-                        lambda ast11: (
+                    )
+                    ast.assign(has_dataprop_val, expr.ExprConstant(False))
+                    has_dataprop_val = has_dataprop_val.get_var()
+
+                    AlignmentFn(desc, program).align(
+                        ast,
+                        classprop.alignments,
+                        debuginfo,
+                        lambda astxx: astxx(stmt.NoStatement()),
+                        iter_final_list,
+                    )(
+                        lambda ast00: ast00.if_(is_prop_val_not_missing(ast00))(
+                            lambda ast01: ast01.assign(
+                                has_dataprop_val, expr.ExprConstant(True)
+                            ),
+                            lambda ast02: write_fn(
+                                ast02,
+                                expr.ExprConstant(classprop.predicate),
+                                get_prop_val(ast02),
+                            ),
+                        )
+                    )
+                    ast.if_(expr.ExprNegation(expr.ExprVar(has_dataprop_val)))(
+                        lambda ast00: (
                             assert_true(
                                 is_buffered,
                                 "We should only abort record if we are buffering",
                             )
-                            and writer.abort_record(ast11)
+                            and writer.abort_record(ast00)
                         ),
-                    ),
-                )
+                        (
+                            stmt.ContinueStatement()
+                            if parent_ast.has_statement_between_ast(
+                                stmt.ForLoopStatement, ast.id
+                            )
+                            else stmt.NoStatement()
+                        ),
+                    )
+                else:
+
+                    def on_missing_key(tree: AST):
+                        assert_true(
+                            is_buffered,
+                            "We should only abort record if we are buffering",
+                        )
+                        writer.abort_record(tree)
+                        if parent_ast.has_statement_between_ast(
+                            stmt.ForLoopStatement, tree.id
+                        ):
+                            tree(stmt.ContinueStatement())
+                        else:
+                            # same ast because of a single value, we can't use continue
+                            # however, we use pass as it's a single-level if/else -- the else part
+                            # will handle the instance generation if there is no missing value.
+                            tree(stmt.NoStatement())
+
+                    AlignmentFn(desc, program).align(
+                        ast,
+                        classprop.alignments,
+                        debuginfo,
+                        # on_missing_key=lambda astxx: assert_true(
+                        #     is_buffered,
+                        #     "We should only abort record if we are buffering",
+                        # )
+                        # and writer.abort_record(astxx),
+                        on_missing_key=on_missing_key,
+                        iter_final_list=iter_final_list,
+                    )(
+                        lambda ast00: ast00.if_(is_prop_val_not_missing(ast00))(
+                            lambda ast01: write_fn(
+                                ast01,
+                                expr.ExprConstant(classprop.predicate),
+                                get_prop_val(ast01),
+                            ),
+                        ),
+                        lambda ast10: ast10.else_()(
+                            lambda ast11: (
+                                assert_true(
+                                    is_buffered,
+                                    "We should only abort record if we are buffering",
+                                )
+                                and writer.abort_record(ast11)
+                            ),
+                            (
+                                stmt.ContinueStatement()
+                                if parent_ast.has_statement_between_ast(
+                                    stmt.ForLoopStatement, ast10.id
+                                )
+                                else stmt.NoStatement()
+                            ),
+                        ),
+                    )
```

### Comparing `drepr_v2-1.1.3/drepr/program_generation/predefined_fn.py` & `drepr_v2-1.2.1/drepr/program_generation/predefined_fn.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/program_generation/preprocessing.py` & `drepr_v2-1.2.1/drepr/program_generation/preprocessing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from typing import Optional
 
+import drepr.models.path as dpath
 from codegen.models import AST, Program, Var, expr
 from codegen.models.var import DeferredVar
-
-from drepr.models.attr import Attr, Sorted, ValueType
-from drepr.models.drepr import DRepr
-from drepr.models.path import IndexExpr, RangeExpr
-from drepr.models.preprocessing import Context, PMap, PreprocessingType
+from drepr.models.prelude import (
+    Attr,
+    Context,
+    DRepr,
+    PMap,
+    PreprocessingType,
+    Resource,
+    Sorted,
+    ValueType,
+)
 from drepr.program_generation.alignment_fn import PathAccessor
 from drepr.program_generation.predefined_fn import DReprPredefinedFn
 from drepr.program_generation.program_space import VarSpace
 from drepr.utils.udf import SourceTree, UDFParsedResult, UDFParser
 
 PreprocessingId = int
 
@@ -60,136 +66,244 @@
             value = preprocessing.value
             assert isinstance(value, PMap)
 
             # generate the necessary function (user defined fn & our preprocessing fn)
             self._init_user_defined_fn(prepro_id, value.code)
             self._generate_preprocessing_pmap(prepro_id, prepro_fn, value)
 
-            # call preprocessing fn in the main program
-            self.call_preproc_ast.expr(
-                expr.ExprFuncCall(
-                    expr.ExprIdent(genfn_name),
-                    [
-                        expr.ExprVar(
-                            self.program.get_var(
-                                key=VarSpace.resource_data(
-                                    preprocessing.value.resource_id
-                                ),
-                                at=self.call_preproc_ast.next_child_id(),
-                            )
-                        ),
-                    ],
-                )
+            prepro_invoke_expr = expr.ExprFuncCall(
+                expr.ExprIdent(genfn_name),
+                [
+                    expr.ExprVar(
+                        self.program.get_var(
+                            key=VarSpace.resource_data(preprocessing.value.resource_id),
+                            at=self.call_preproc_ast.next_child_id(),
+                        )
+                    ),
+                ],
             )
+            # call preprocessing fn in the main program and assign if needed
+            if value.output is not None:
+                prepro_resource_id = Resource.get_preprocessing_output_id(value.output)
+                self.call_preproc_ast.assign(
+                    DeferredVar(
+                        name=f"resource_data_{prepro_resource_id}",
+                        key=VarSpace.resource_data(prepro_resource_id),
+                    ),
+                    prepro_invoke_expr,
+                )
+            else:
+                self.call_preproc_ast.expr(prepro_invoke_expr)
             return None
 
         raise NotImplementedError(preprocessing.type)
 
     def _generate_preprocessing_pmap(self, prepro_id: int, prepro_fn: AST, value: PMap):
-        if not value.change_structure and value.output is None:
-            # if we don't change the structure and don't have output, we directly mutate the resource data
-            # the idea is to loop through the path without the last index, get the value, apply the function, and set the value
-            # of the last index to the new value.
+        if not value.change_structure:
+            if value.output is not None:
+                prepro_resource_id = Resource.get_preprocessing_output_id(value.output)
+                # create a variable to store the preprocess results
+                output_attr_id = value.output
+                output_attr = DeferredVar(
+                    name=output_attr_id, key=VarSpace.preprocessing_output(prepro_id)
+                )
+
+                # we use a special class called AttributeData that can store data as if it is in the resource data (same index, etc -- but the
+                # real location in memory is different)
+                self.program.import_("drepr.utils.attr_data.AttributeData", True)
+                prepro_fn.assign(
+                    output_attr,
+                    expr.ExprFuncCall(
+                        expr.ExprIdent("AttributeData.from_raw_path"),
+                        [
+                            expr.ExprConstant(value.path.to_lang_format()),
+                        ],
+                    ),
+                )
+
+                def on_step(
+                    ast: AST,
+                    dim: int,
+                    collection: expr.Expr,
+                    key: expr.Expr,
+                    result: DeferredVar | Var,
+                ):
+                    # everytime we step into a new dimension, we step into the output variable as well.
+                    if dim == 0:
+                        # this is better than `output_attr.get_var()` as we can ensure the scope is correct
+                        output_collection = expr.ExprVar(
+                            self.program.get_var(
+                                key=output_attr.key, at=ast.next_child_id()
+                            )
+                        )
+                    else:
+                        output_collection = expr.ExprVar(
+                            self.program.get_var(
+                                key=VarSpace.attr_value_dim(
+                                    prepro_resource_id, output_attr_id, dim - 1
+                                ),
+                                at=ast.next_child_id(),
+                            )
+                        )
+
+                    itemvalue = DeferredVar(
+                        name=f"{output_attr_id}_value_{dim}",
+                        key=VarSpace.attr_value_dim(
+                            prepro_resource_id, output_attr_id, dim
+                        ),
+                    )
+                    ast.assign(
+                        itemvalue, DReprPredefinedFn.item_getter(output_collection, key)
+                    )
+
+                on_step_callback = on_step
+            else:
+                on_step_callback = None
+
+            # the idea is to loop through the path without the last index, get the value, apply the function, and set
+            # the value of the last index to the new value
             pseudo_attr = Attr(
                 id=f"preproc_{prepro_id}_path",
                 resource_id=value.resource_id,
                 path=value.path,
                 missing_values=[],
                 unique=False,
                 sorted=Sorted.Null,
                 value_type=ValueType.UnspecifiedSingle,
             )
             ast = PathAccessor(self.program).iterate_elements(
-                ast=prepro_fn,
-                attr=pseudo_attr,
+                ast=prepro_fn, attr=pseudo_attr, on_step_callback=on_step_callback
             )
 
             # get item value & item context
             item_value = self.program.get_var(
                 key=VarSpace.attr_value_dim(
                     pseudo_attr.resource_id,
                     pseudo_attr.id,
                     len(pseudo_attr.path.steps) - 1,
                 ),
                 at=ast.next_child_id(),
             )
-            if len(pseudo_attr.path.steps) > 1:
-                parent_item_value = self.program.get_var(
-                    key=VarSpace.attr_value_dim(
-                        pseudo_attr.resource_id,
-                        pseudo_attr.id,
-                        len(pseudo_attr.path.steps) - 2,
-                    ),
-                    at=ast.next_child_id(),
+            if self.user_defined_fn[prepro_id].use_context:
+                context_index: list[expr.Expr] = []
+                for dim in range(len(pseudo_attr.path.steps)):
+                    step = pseudo_attr.path.steps[dim]
+                    if isinstance(step, dpath.IndexExpr):
+                        if isinstance(step.val, dpath.Expr):
+                            # I don't know about recursive path expression yet -- what usecase and how to use them -- so I can't implement.
+                            raise Exception(
+                                f"Recursive path expression is not supported yet. Please raise a ticket to notify us for future support! Found: {step.vals}"
+                            )
+                        context_index.append(expr.ExprConstant(step.val))
+                    else:
+                        context_index.append(
+                            expr.ExprVar(
+                                self.program.get_var(
+                                    key=VarSpace.attr_index_dim(
+                                        pseudo_attr.resource_id, pseudo_attr.id, dim
+                                    ),
+                                    at=ast.next_child_id(),
+                                )
+                            )
+                        )
+
+                self.program.import_(
+                    "drepr.program_generation.preprocessing.ContextImpl", True
                 )
-            else:
-                parent_item_value = self.program.get_var(
-                    key=VarSpace.resource_data(pseudo_attr.resource_id),
-                    at=ast.next_child_id(),
+                item_context = expr.ExprFuncCall(
+                    expr.ExprIdent("ContextImpl"),
+                    [
+                        expr.ExprVar(
+                            self.program.get_var(
+                                key=VarSpace.resource_data(value.resource_id),
+                                at=prepro_fn.next_child_id(),
+                            )
+                        ),
+                        DReprPredefinedFn.tuple(context_index),
+                    ],
                 )
+            else:
+                item_context = None
 
-            if isinstance(pseudo_attr.path.steps[-1], IndexExpr):
+            # then we call the user defined fn to get the new item value
+            new_item_value = self._call_user_defined_fn(
+                prepro_id,
+                ast,
+                expr.ExprVar(item_value),
+                item_context,
+            )
+
+            # get the parent item value & index to assign the new value
+            # if output new data, we need to retrieve the parent item value from correct location
+            if value.output is not None:
+                if len(pseudo_attr.path.steps) > 1:
+                    parent_item_value = self.program.get_var(
+                        key=VarSpace.attr_value_dim(
+                            prepro_resource_id,
+                            output_attr_id,
+                            len(pseudo_attr.path.steps) - 2,
+                        ),
+                        at=ast.next_child_id(),
+                    )
+                else:
+                    # this is better than `output_attr.get_var()` as we can ensure the scope is correct
+                    parent_item_value = self.program.get_var(
+                        key=output_attr.key,
+                        at=ast.next_child_id(),
+                    )
+            else:
+                if len(pseudo_attr.path.steps) > 1:
+                    parent_item_value = self.program.get_var(
+                        key=VarSpace.attr_value_dim(
+                            pseudo_attr.resource_id,
+                            pseudo_attr.id,
+                            len(pseudo_attr.path.steps) - 2,
+                        ),
+                        at=ast.next_child_id(),
+                    )
+                else:
+                    parent_item_value = self.program.get_var(
+                        key=VarSpace.resource_data(pseudo_attr.resource_id),
+                        at=ast.next_child_id(),
+                    )
+
+            if isinstance(pseudo_attr.path.steps[-1], dpath.IndexExpr):
                 parent_item_index = expr.ExprConstant(pseudo_attr.path.steps[-1].val)
             else:
                 parent_item_index = expr.ExprVar(
                     self.program.get_var(
                         key=VarSpace.attr_index_dim(
                             pseudo_attr.resource_id,
                             pseudo_attr.id,
                             len(pseudo_attr.path.steps) - 1,
                         ),
                         at=ast.next_child_id(),
                     )
                 )
 
-            if self.user_defined_fn[prepro_id].use_context:
-                # TODO: implement this
-                # item_context = expr.ExprFuncCall(
-                #     expr.ExprIdent("ContextImpl"),
-                #     [
-                #         expr.ExprVar(
-                #             Var.deref(
-                #                 self.memory,
-                #                 key=VarSpace.resource_data(pseudo_attr.resource_id),
-                #             )
-                #         ),
-                #         expr.ExprVar(
-                #             Var.deref(
-                #                 self.memory,
-                #                 key=VarSpace.attr_index_dim(
-                #                     pseudo_attr.resource_id,
-                #                     pseudo_attr.id,
-                #                     len(pseudo_attr.path.steps) - 1,
-                #                 ),
-                #             )
-                #         ),
-                #     ],
-                # )
-                raise NotImplementedError()
-            else:
-                item_context = None
-
-            # then we call the user defined fn to get the new item value
-            new_item_value = self._call_user_defined_fn(
-                prepro_id,
-                ast,
-                expr.ExprVar(item_value),
-                item_context,
-            )
-
             # then, we set the new item value to the parent item value
             ast.expr(
                 DReprPredefinedFn.item_setter(
                     expr.ExprVar(parent_item_value),
                     parent_item_index,
                     new_item_value,
                 )
             )
+
+            if value.output is not None:
+                prepro_fn.return_(
+                    expr.ExprVar(
+                        self.program.get_var(
+                            key=output_attr.key,
+                            at=prepro_fn.next_child_id(),
+                        )
+                    )
+                )
         else:
-            # we have to create a temporary variable to store preprocessed results
+            # haven't considered the case of changing structure yet
             raise NotImplementedError()
 
     def _init_user_defined_fn(self, prepro_id: PreprocessingId, code: str):
         """First, import statements are moved to the top of the file. The rest of the code can be either
         wrapped in a function (as expected in DRepr design), or directly embedded whenever it is used.
 
         The later option (embedding code) yields more performance, but it is harder because of potential variable name conflicts.
@@ -243,15 +357,15 @@
 
             assert parsed_udf.source_tree.node == ""
             assert len(parsed_udf.source_tree.children) > 0
             for child in parsed_udf.source_tree.children:
                 insert_source_tree(inner_udf, child)
 
             # now we create the user-defined function
-            fnvar = DeferredVar(fnname)
+            fnvar = DeferredVar(fnname, key=VarSpace.preprocessing_udf(fnname))
             self.program.root.assign(
                 fnvar,
                 expr.ExprFuncCall(expr.ExprIdent("get_" + fnname), []),
             )
             fnvar = expr.ExprVar(fnvar.get_var())
         else:
             inner_udf = self.program.root.func(fnname, fnargs)
@@ -293,12 +407,16 @@
     def __init__(self, resource_data, index: tuple):
         self.resource_data = resource_data
         self.index = index
 
     def get_index(self) -> tuple:
         return self.index
 
-    def get_value(self, resource_data, index: tuple):
+    def get_value(self, index: tuple):
         ptr = self.resource_data
         for i in index:
             ptr = ptr[i]
         return ptr
+
+
+class GenerateDataStorage:
+    pass
```

### Comparing `drepr_v2-1.1.3/drepr/program_generation/program_space.py` & `drepr_v2-1.2.1/drepr/program_generation/program_space.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,22 +7,27 @@
 
 class VarSpace:
     output_file = lambda: ("output_file",)
     resource = lambda resource: ResourceKey(
         f"resource={resource}",
     )
     resource_data = lambda resource: (f"resource-data={resource}",)
+    preprocessing_udf = lambda func_name: (func_name,)
     preprocessing_udf_value = lambda preprocessing_id: (
         f"preprocessing-id={preprocessing_id}",
         "udf-value",
     )
     preprocessing_udf_context = lambda preprocessing_id: (
         f"preprocessing-id={preprocessing_id}",
         "udf-context",
     )
+    preprocessing_output = lambda preprocessing_id: (
+        f"preprocessing-id={preprocessing_id}",
+        "output",
+    )
     writer = lambda: ("writer",)
     attr_index_dim = lambda resource, attr, di: (
         f"resource={resource}",
         f"attr={attr}",
         f"index-dim={di}",
     )
     attr_value_dim = lambda resource, attr, di: (
```

### Comparing `drepr_v2-1.1.3/drepr/program_generation/writers.py` & `drepr_v2-1.2.1/drepr/program_generation/writers.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/utils/misc.py` & `drepr_v2-1.2.1/drepr/utils/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -91,7 +91,16 @@
                 if k not in cache:
                     cache[k] = func(self, *args, **kwargs)
                 return cache[k]
 
             return fn
 
         return wrapper_fn  # type: ignore
+
+
+def get_abs_iri(prefixes: dict[str, str], rel_iri: str) -> str:
+    prefix, val = rel_iri.split(":", 1)
+    if prefix not in prefixes:
+        raise ValueError(
+            f"Cannot create absolute IRI because the prefix {prefix} does not exist"
+        )
+    return f"{prefixes[prefix]}{val}"
```

### Comparing `drepr_v2-1.1.3/drepr/utils/namespace_mixin.py` & `drepr_v2-1.2.1/drepr/utils/namespace_mixin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from drepr.utils.misc import get_abs_iri
+
+
 class NamespaceMixin:
     prefixes: dict[str, str]
 
     @classmethod
     def is_rel_iri(cls, iri: str) -> bool:
         return iri.find("://") == -1 and iri.find(":") != -1
 
@@ -14,13 +17,8 @@
         raise ValueError(
             "Cannot create relative IRI because there is no suitable prefix"
         )
 
     def get_abs_iri(self, rel_iri: str) -> str:
         """Convert a relative IRI to an absolute IRI."""
         assert self.is_rel_iri(rel_iri)
-        prefix, val = rel_iri.split(":", 1)
-        if prefix not in self.prefixes:
-            raise ValueError(
-                f"Cannot create absolute IRI because the prefix {prefix} does not exist"
-            )
-        return f"{self.prefixes[prefix]}{val}"
+        return get_abs_iri(self.prefixes, rel_iri)
```

### Comparing `drepr_v2-1.1.3/drepr/utils/udf.py` & `drepr_v2-1.2.1/drepr/utils/udf.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,24 @@
                 out[0].children.extend(self._parse_ast(stmt, imports))
             if len(tree.orelse) > 0:
                 out.append(SourceTree("else:", []))
                 for stmt in tree.orelse:
                     out[1].children.extend(self._parse_ast(stmt, imports))
             return out
 
+        if isinstance(tree, ast.For):
+            content = f"for {self._get_node_code(tree.target)}{self._get_node_code(tree.iter)}"
+            out = [SourceTree(content, [])]
+            for stmt in tree.body:
+                out[0].children.extend(self._parse_ast(stmt, imports))
+            if len(tree.orelse) > 0:
+                out.append(SourceTree("else:", []))
+                for stmt in tree.orelse:
+                    out[1].children.extend(self._parse_ast(stmt, imports))
+            return out
         raise NotImplementedError()
 
     def _get_node_code(self, node: ast.AST) -> str:
         lines = self.source_code_lines[node.lineno - 1 : node.end_lineno]
         lines[0] = lines[0][node.col_offset :]
         lines[-1] = lines[-1][: node.end_col_offset]
         return "\n".join(lines)
```

### Comparing `drepr_v2-1.1.3/drepr/utils/validator.py` & `drepr_v2-1.2.1/drepr/utils/validator.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/drepr/writers/base.py` & `drepr_v2-1.2.1/drepr/writers/base.py`

 * *Files identical despite different names*

### Comparing `drepr_v2-1.1.3/pyproject.toml` & `drepr_v2-1.2.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "drepr-v2"
-version = "1.1.3"
+version = "1.2.1"
 description = ""
 authors = ["Binh Vu <binh@toan2.com>"]
 readme = "README.md"
 packages = [{ include = "drepr" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 orjson = "^3.9.13"
 ruamel-yaml = "^0.17.21"
 graph-wrapper = "^1.7.1"
 serde2 = "^1.7.3"
 typer = { extras = ["all"], version = "^0.9.0" }
-codegen-2 = "^2.1.0"
+codegen-2 = "^2.1.3"
 rdflib = "^7.0.0"
+openpyxl = "^3.1.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.1.1"
 autoflake = "^2.2.1"
 pytest = "^8.0.0"
 pytest-cov = "^4.1.0"
```

### Comparing `drepr_v2-1.1.3/PKG-INFO` & `drepr_v2-1.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: drepr-v2
-Version: 1.1.3
+Version: 1.2.1
 Summary: 
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: codegen-2 (>=2.1.0,<3.0.0)
+Requires-Dist: codegen-2 (>=2.1.3,<3.0.0)
 Requires-Dist: graph-wrapper (>=1.7.1,<2.0.0)
+Requires-Dist: openpyxl (>=3.1.2,<4.0.0)
 Requires-Dist: orjson (>=3.9.13,<4.0.0)
 Requires-Dist: rdflib (>=7.0.0,<8.0.0)
 Requires-Dist: ruamel-yaml (>=0.17.21,<0.18.0)
 Requires-Dist: serde2 (>=1.7.3,<2.0.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

