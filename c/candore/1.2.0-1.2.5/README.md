# Comparing `tmp/candore-1.2.0.tar.gz` & `tmp/candore-1.2.5.tar.gz`

## Comparing `candore-1.2.0.tar` & `candore-1.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.0/apix/__init__.py
--rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 candore-1.2.0/apix/diff.py
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 candore-1.2.0/apix/explore.py
--rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 candore-1.2.0/apix/helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.0/apix/parsers/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 candore-1.2.0/apix/parsers/apipie.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 candore-1.2.0/apix/parsers/test.py
--rw-r--r--   0        0        0     2261 2020-02-02 00:00:00.000000 candore-1.2.0/candore/__init__.py
--rw-r--r--   0        0        0     3306 2020-02-02 00:00:00.000000 candore-1.2.0/candore/cli.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 candore-1.2.0/candore/config.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 candore-1.2.0/candore/errors.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 candore-1.2.0/candore/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/__init__.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/api_lister.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/comparator.py
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/extractor.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/finder.py
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/report.py
--rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/variatons.py
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/webapp.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 candore-1.2.0/candore/modules/templates/table.html
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 candore-1.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 candore-1.2.0/LICENSE
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 candore-1.2.0/README.md
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 candore-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 candore-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/apix/__init__.py
+-rw-r--r--   0        0        0     6639 2020-02-02 00:00:00.000000 candore-1.2.5/apix/diff.py
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 candore-1.2.5/apix/explore.py
+-rw-r--r--   0        0        0     3836 2020-02-02 00:00:00.000000 candore-1.2.5/apix/helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/apipie.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 candore-1.2.5/apix/parsers/test.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 candore-1.2.5/candore/__init__.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 candore-1.2.5/candore/cli.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 candore-1.2.5/candore/config.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 candore-1.2.5/candore/errors.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 candore-1.2.5/candore/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/__init__.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/api_lister.py
+-rw-r--r--   0        0        0     6153 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/comparator.py
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/extractor.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/finder.py
+-rw-r--r--   0        0        0     3289 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/report.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/variations.py
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/webapp.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 candore-1.2.5/candore/modules/templates/table.html
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 candore-1.2.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 candore-1.2.5/LICENSE
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 candore-1.2.5/README.md
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 candore-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 candore-1.2.5/PKG-INFO
```

### Comparing `candore-1.2.0/apix/diff.py` & `candore-1.2.5/apix/diff.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/apix/explore.py` & `candore-1.2.5/apix/explore.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/apix/helpers.py` & `candore-1.2.5/apix/helpers.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/apix/parsers/apipie.py` & `candore-1.2.5/apix/parsers/apipie.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/apix/parsers/test.py` & `candore-1.2.5/apix/parsers/test.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/candore/__init__.py` & `candore-1.2.5/candore/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -46,23 +46,24 @@
             json.dump(data, entfile)
         click.echo(f"Entities data saved to {file_path}")
 
     def compare_entities(
         self,
         pre_file=None,
         post_file=None,
+        inverse=None,
         output=None,
         report_type=None,
         record_evs=None,
     ):
         comp = Comparator(settings=self.settings)
         if record_evs:
             comp.record_evs = True
-        results = comp.compare_json(pre_file=pre_file, post_file=post_file)
+        results = comp.compare_json(pre_file=pre_file, post_file=post_file, inverse=inverse)
         reporter = Reporting(results=results)
-        reporter.generate_report(output_file=output, output_type=report_type)
+        reporter.generate_report(output_file=output, output_type=report_type, inverse=inverse)
 
     def find_path(self, path, json_file, delimiter):
         finder = Finder()
         data = finder.find(path=path, json_file=json_file, delimiter=delimiter)
         if data:
             pprint(data)
```

### Comparing `candore-1.2.0/candore/cli.py` & `candore-1.2.5/candore/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,29 +50,31 @@
     candore_obj = ctx.parent.candore
     loop.run_until_complete(candore_obj.save_all_entities(mode=mode, output_file=output, full=full))
 
 
 @candore.command(help="Compare pre and post upgrade data")
 @click.option("--pre", type=str, help="The pre upgrade json file")
 @click.option("--post", type=str, help="The post upgrade json file")
+@click.option("-i", "--inverse", is_flag=True, help="Inverse comparison, shows whats not changed")
 @click.option("-o", "--output", type=str, help="The output file name")
 @click.option(
     "-t",
     "--report-type",
     type=str,
     default="json",
     help="The type of report GSheet, JSON, or webpage",
 )
 @click.option("--record-evs", is_flag=True, help="Record Expected Variations in reporting")
 @click.pass_context
-def compare(ctx, pre, post, output, report_type, record_evs):
+def compare(ctx, pre, post, inverse, output, report_type, record_evs):
     candore_obj = ctx.parent.candore
     candore_obj.compare_entities(
         pre_file=pre,
         post_file=post,
+        inverse=inverse,
         output=output,
         report_type=report_type,
         record_evs=record_evs,
     )
 
 
 @candore.command(help="JSON Reader for reading the specific path data from entities data file")
```

### Comparing `candore-1.2.0/candore/config.py` & `candore-1.2.5/candore/config.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/candore/modules/api_lister.py` & `candore-1.2.5/candore/modules/api_lister.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/candore/modules/comparator.py` & `candore-1.2.5/candore/modules/comparator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 import json
 
-from candore.modules.variatons import Variations
-from candore.utils import last_index_of_element
+from candore.modules.variations import Variations, Constants
+from candore.utils import last_index_of_element, is_list_contains_dict
 
 
 class Comparator:
     def __init__(self, settings):
         self.big_key = []
-        self.big_compare = {}
+        self.big_diff = {}
+        self.big_constant = {}
         self.record_evs = False
         self.variations = Variations(settings)
+        self.constants = Constants(settings)
         self.expected_variations = self.variations.expected_variations
         self.skipped_variations = self.variations.skipped_variations
+        self.expected_constants = self.constants.expected_constants
+        self.skipped_constants = self.constants.skipped_constants
 
-    def remove_non_variant_key(self, key):
+
+
+    def remove_verifed_key(self, key):
         reversed_bk = self.big_key[::-1]
         if key in reversed_bk:
             reversed_bk.remove(key)
         self.big_key = reversed_bk[::-1]
 
     def remove_path(self, identy):
         id_index = last_index_of_element(self.big_key, identy)
@@ -32,21 +38,40 @@
         if var_full_path in self.expected_variations or var_full_path in self.skipped_variations:
             if self.record_evs:
                 variation = {
                     "pre": pre,
                     "post": post,
                     "variation": var_details or "Expected(A)",
                 }
-                self.big_compare.update({full_path: variation})
+                self.big_diff.update({full_path: variation})
         elif (
             var_full_path not in self.expected_variations
             and var_full_path not in self.skipped_variations
         ):
             variation = {"pre": pre, "post": post, "variation": var_details or ""}
-            self.big_compare.update({full_path: variation})
+            self.big_diff.update({full_path: variation})
+
+    def record_constants(self, pre, post, var_details=None):
+        big_key = [str(itm) for itm in self.big_key]
+        full_path = "/".join(big_key)
+        var_full_path = "/".join([itm for itm in self.big_key if not isinstance(itm, int)])
+        if var_full_path in self.expected_constants or var_full_path in self.skipped_constants:
+            if self.record_evs:
+                variation = {
+                    "pre": pre,
+                    "post": post,
+                    "constant": var_details or "Expected(A)",
+                }
+                self.big_constant.update({full_path: variation})
+        elif (
+            var_full_path not in self.expected_constants
+            and var_full_path not in self.skipped_constants
+        ):
+            variation = {"pre": pre, "post": post, "constant": var_details or ""}
+            self.big_constant.update({full_path: variation})
 
     def _is_data_type_dict(self, pre, post, unique_key=""):
         if (pre and 'id' in pre) and (post and 'id' in post):
             # Dont compare the entities if the ids are not the same
             if pre['id'] != post['id']:
                 return
         for pre_key in pre:
@@ -58,58 +83,72 @@
                     pre[pre_key],
                     None,
                     unique_key=pre_key,
                     var_details="Post lookup key missing",
                 )
         self.remove_path(unique_key)
 
-    def _is_data_type_list(self, pre, post, unique_key=""):
+    def _is_data_type_list_contains_dict(self, pre, post):
         for pre_entity in pre:
             if not pre_entity:
                 continue
-            if type(pre_entity) is dict:
-                for post_entity in post:
-                    if not post_entity:
-                        continue
-                    if "id" in pre_entity:
-                        if pre_entity["id"] == post_entity["id"]:
-                            self.compare_all_pres_with_posts(
-                                pre_entity, post_entity, unique_key=pre_entity["id"]
-                            )
-                    else:
-                        key = list(pre_entity.keys())[0]
-                        if pre_entity[key] == post_entity[key]:
-                            self.compare_all_pres_with_posts(
-                                pre_entity[key], post_entity[key], unique_key=key
-                            )
+            for post_entity in post:
+                if not post_entity:
+                    continue
                 if "id" in pre_entity:
-                    self.remove_path(pre_entity["id"])
+                    if pre_entity["id"] == post_entity["id"]:
+                        self.compare_all_pres_with_posts(
+                            pre_entity, post_entity, unique_key=pre_entity["id"]
+                        )
                 else:
-                    self.remove_path(pre_entity[list(pre_entity.keys())[0]])
+                    key = list(pre_entity.keys())[0]
+                    if pre_entity[key] == post_entity[key]:
+                        self.compare_all_pres_with_posts(
+                            pre_entity[key], post_entity[key], unique_key=key
+                        )
+            if "id" in pre_entity:
+                self.remove_path(pre_entity["id"])
             else:
-                if pre_entity not in post:
-                    self.record_variation(pre, post)
+                self.remove_path(pre_entity[list(pre_entity.keys())[0]])
+
+    def _is_data_type_list(self, pre, post, unique_key=""):
+
+        def custom_key(elem):
+            return 'None' if elem is None else str(elem)
+
+        if not is_list_contains_dict(pre):
+            if sorted(pre, key=custom_key) != sorted(post, key=custom_key):
+                self.record_variation(pre, post)
+            else:
+                self.record_constants(pre, post)
+        else:
+            self._is_data_type_list_contains_dict(pre, post)
         self.remove_path(unique_key)
 
     def compare_all_pres_with_posts(self, pre_data, post_data, unique_key="", var_details=None):
         if unique_key:
             self.big_key.append(unique_key)
         if type(pre_data) is dict:
             self._is_data_type_dict(pre_data, post_data, unique_key=unique_key)
         elif type(pre_data) is list:
             self._is_data_type_list(pre_data, post_data, unique_key=unique_key)
         else:
             if pre_data != post_data:
                 self.record_variation(pre_data, post_data, var_details)
-            self.remove_non_variant_key(unique_key)
+            else:
+                self.record_constants(pre_data, post_data, var_details)
+            self.remove_verifed_key(unique_key)
 
-    def compare_json(self, pre_file, post_file):
+    def compare_json(self, pre_file, post_file, inverse):
         pre_data = post_data = None
 
         with open(pre_file, "r") as fpre:
             pre_data = json.load(fpre)
 
         with open(post_file, "r") as fpost:
             post_data = json.load(fpost)
 
         self.compare_all_pres_with_posts(pre_data, post_data)
-        return self.big_compare
+        if not inverse:
+            return self.big_diff
+        else:
+            return self.big_constant
```

### Comparing `candore-1.2.0/candore/modules/extractor.py` & `candore-1.2.5/candore/modules/extractor.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/candore/modules/finder.py` & `candore-1.2.5/candore/modules/finder.py`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/candore/modules/report.py` & `candore-1.2.5/candore/modules/report.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,31 +13,32 @@
         """Initialize the Reporting class
 
         Args:
             comparator (Comparator): The comparator object to use for reporting
         """
         self.results = results
 
-    def generate_report(self, output_file, output_type):
+    def generate_report(self, output_file, output_type, inverse):
         """Generate a report of the compared results
 
         Args:
             output_file (str): The file to write the report to
             output_type (str): The type of report to generate json / CSV
+            inverse (bool): Shows what not changed in comparison results
         Returns:
             None
         Raises:
             ValueError: If the output_type is not supported
         """
         if output_type == "json":
             self._generate_json_report(output_file)
         elif output_type == "html":
-            self._generate_html_report()
+            print('The HTML reporting is not implemented yet! Try next time!')
         elif output_type == "csv":
-            self._generate_csv_report(output_file)
+            self._generate_csv_report(output_file, inverse=inverse)
         else:
             raise ValueError("Output type {} not supported".format(output_type))
 
     def _generate_json_report(self, output_file):
         """Generate a JSON report of the compared results
 
         Args:
@@ -61,25 +62,30 @@
         Returns:
             None
         """
         # display_json_table(results_json=self.results)
         # render_webpage()
         print("HTML report is ready to view at: http://localhost:5000")
 
-    def _generate_csv_report(self, output_file):
+    def _generate_csv_report(self, output_file, inverse):
         """Generate a CSV report of the compared results
 
         Args:
             output_file (str): The file to write the report to
         Returns:
             None
         """
         if not output_file:
             output_file = "results.csv"
         output_file = Path(output_file)
         # Convert json to csv and write to output file
         csv_writer = csv.writer(output_file.open("w"))
-        csv_writer.writerow(["Variation Path", "Pre-Upgrade", "Post-Upgrade", "Variation"])
+        # Table Column Names
+        columns = ["Path", "Pre-Upgrade", "Post-Upgrade", "Variation?" if not inverse else 'Constant?']
+        csv_writer.writerow(columns)
+        # Writing Rows
         for var_path, vals in self.results.items():
-            csv_writer.writerow([var_path, vals["pre"], vals["post"], vals["variation"]])
+            csv_writer.writerow([
+                var_path, vals["pre"], vals["post"],
+                vals["variation" if not inverse else "constant"]])
         print("Wrote CSV report to {}".format(output_file))
         print("CSV report contains {} results".format(len(self.results)))
```

### Comparing `candore-1.2.0/candore/modules/templates/table.html` & `candore-1.2.5/candore/modules/templates/table.html`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/LICENSE` & `candore-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `candore-1.2.0/pyproject.toml` & `candore-1.2.5/pyproject.toml`

 * *Files identical despite different names*

