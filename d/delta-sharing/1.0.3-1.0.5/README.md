# Comparing `tmp/delta-sharing-1.0.3.tar.gz` & `tmp/delta-sharing-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "delta-sharing-1.0.3.tar", last modified: Sat Dec  2 01:06:39 2023, max compression
+gzip compressed data, was "delta-sharing-1.0.5.tar", last modified: Tue Apr 23 16:44:55 2024, max compression
```

## Comparing `delta-sharing-1.0.3.tar` & `delta-sharing-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-12-02 01:06:39.347390 delta-sharing-1.0.3/
--rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/NOTICE.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2671 2023-12-02 01:06:39.347076 delta-sharing-1.0.3/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/README.md
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-12-02 01:06:39.344341 delta-sharing-1.0.3/delta_sharing/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/__init__.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/_yarl_patch.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/converter.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    12923 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/delta_sharing.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/protocol.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)     8854 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/reader.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)    16797 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/delta_sharing/rest_client.py
--rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2023-12-02 01:05:32.000000 delta-sharing-1.0.3/delta_sharing/version.py
-drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2023-12-02 01:06:39.346277 delta-sharing-1.0.3/delta_sharing.egg-info/
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2671 2023-12-02 01:06:39.000000 delta-sharing-1.0.3/delta_sharing.egg-info/PKG-INFO
--rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2023-12-02 01:06:39.000000 delta-sharing-1.0.3/delta_sharing.egg-info/SOURCES.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2023-12-02 01:06:39.000000 delta-sharing-1.0.3/delta_sharing.egg-info/dependency_links.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2023-12-02 01:06:39.000000 delta-sharing-1.0.3/delta_sharing.egg-info/requires.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2023-12-02 01:06:39.000000 delta-sharing-1.0.3/delta_sharing.egg-info/top_level.txt
--rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2023-12-02 01:06:39.347437 delta-sharing-1.0.3/setup.cfg
--rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-10-04 05:59:28.000000 delta-sharing-1.0.3/setup.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2024-04-23 16:44:55.467235 delta-sharing-1.0.5/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      534 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/NOTICE.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2671 2024-04-23 16:44:55.466569 delta-sharing-1.0.5/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1201 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/README.md
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2024-04-23 16:44:55.461050 delta-sharing-1.0.5/delta_sharing/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     1274 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/__init__.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      855 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/_yarl_patch.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     5066 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/converter.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    13214 2024-04-23 16:37:15.000000 delta-sharing-1.0.5/delta_sharing/delta_sharing.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    10304 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/protocol.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     8854 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/reader.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)    16797 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/delta_sharing/rest_client.py
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      626 2024-04-23 16:43:28.000000 delta-sharing-1.0.5/delta_sharing/version.py
+drwxr-xr-x   0 lin.zhou   (502) staff       (20)        0 2024-04-23 16:44:55.465867 delta-sharing-1.0.5/delta_sharing.egg-info/
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2671 2024-04-23 16:44:55.000000 delta-sharing-1.0.5/delta_sharing.egg-info/PKG-INFO
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      430 2024-04-23 16:44:55.000000 delta-sharing-1.0.5/delta_sharing.egg-info/SOURCES.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)        1 2024-04-23 16:44:55.000000 delta-sharing-1.0.5/delta_sharing.egg-info/dependency_links.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)      167 2024-04-23 16:44:55.000000 delta-sharing-1.0.5/delta_sharing.egg-info/requires.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       14 2024-04-23 16:44:55.000000 delta-sharing-1.0.5/delta_sharing.egg-info/top_level.txt
+-rw-r--r--   0 lin.zhou   (502) staff       (20)       38 2024-04-23 16:44:55.467323 delta-sharing-1.0.5/setup.cfg
+-rw-r--r--   0 lin.zhou   (502) staff       (20)     2600 2023-10-04 05:59:28.000000 delta-sharing-1.0.5/setup.py
```

### Comparing `delta-sharing-1.0.3/NOTICE.txt` & `delta-sharing-1.0.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/PKG-INFO` & `delta-sharing-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-1.0.3/README.md` & `delta-sharing-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/__init__.py` & `delta-sharing-1.0.5/delta_sharing/__init__.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/_yarl_patch.py` & `delta-sharing-1.0.5/delta_sharing/_yarl_patch.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/converter.py` & `delta-sharing-1.0.5/delta_sharing/converter.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/delta_sharing.py` & `delta-sharing-1.0.5/delta_sharing/delta_sharing.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,31 +98,35 @@
     return response.metadata
 
 
 def load_as_pandas(
     url: str,
     limit: Optional[int] = None,
     version: Optional[int] = None,
-    timestamp: Optional[str] = None
+    timestamp: Optional[str] = None,
+    jsonPredicateHints: Optional[str] = None,
 ) -> pd.DataFrame:
     """
     Load the shared table using the given url as a pandas DataFrame.
 
     :param url: a url under the format "<profile>#<share>.<schema>.<table>"
     :param limit: a non-negative int. Load only the ``limit`` rows if the parameter is specified.
       Use this optional parameter to explore the shared table without loading the entire table to
       the memory.
     :param version: an optional non-negative int. Load the snapshot of table at version
+    :param jsonPredicateHints: Predicate hints to be applied to the table. For more details see:
+      https://github.com/delta-io/delta-sharing/blob/main/PROTOCOL.md#json-predicates-for-filtering
     :return: A pandas DataFrame representing the shared table.
     """
     profile_json, share, schema, table = _parse_url(url)
     profile = DeltaSharingProfile.read_from_file(profile_json)
     return DeltaSharingReader(
         table=Table(name=table, share=share, schema=schema),
         rest_client=DataSharingRestClient(profile),
+        jsonPredicateHints=jsonPredicateHints,
         limit=limit,
         version=version,
         timestamp=timestamp
     ).to_pandas()
 
 
 def load_as_spark(
```

### Comparing `delta-sharing-1.0.3/delta_sharing/protocol.py` & `delta-sharing-1.0.5/delta_sharing/protocol.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/reader.py` & `delta-sharing-1.0.5/delta_sharing/reader.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/rest_client.py` & `delta-sharing-1.0.5/delta_sharing/rest_client.py`

 * *Files identical despite different names*

### Comparing `delta-sharing-1.0.3/delta_sharing/version.py` & `delta-sharing-1.0.5/delta_sharing/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "1.0.3"
+__version__ = "1.0.5"
```

### Comparing `delta-sharing-1.0.3/delta_sharing.egg-info/PKG-INFO` & `delta-sharing-1.0.5/delta_sharing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: delta-sharing
-Version: 1.0.3
+Version: 1.0.5
 Summary: Python Connector for Delta Sharing
 Home-page: https://github.com/delta-io/delta-sharing/
 Author: The Delta Lake Project Authors
 Author-email: delta-users@googlegroups.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/delta-io/delta-sharing
 Project-URL: Documentation, https://github.com/delta-io/delta-sharing
```

### Comparing `delta-sharing-1.0.3/setup.py` & `delta-sharing-1.0.5/setup.py`

 * *Files identical despite different names*

