# Comparing `tmp/excel_graph_parser-0.1.8.tar.gz` & `tmp/excel_graph_parser-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excel_graph_parser-0.1.8.tar", last modified: Mon Apr 15 14:20:45 2024, max compression
+gzip compressed data, was "excel_graph_parser-0.1.9.tar", last modified: Tue Apr 23 08:59:40 2024, max compression
```

## Comparing `excel_graph_parser-0.1.8.tar` & `excel_graph_parser-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.8/LICENSE
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-02-14 06:51:33.000000 excel_graph_parser-0.1.8/README.md
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/excel_graph_parser/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.8/excel_graph_parser/__init__.py
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13475 2024-04-15 14:17:41.000000 excel_graph_parser-0.1.8/excel_graph_parser/graph_parser.py
-drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/PKG-INFO
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/SOURCES.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/dependency_links.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/requires.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-04-15 14:20:45.000000 excel_graph_parser-0.1.8/excel_graph_parser.egg-info/top_level.txt
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-04-15 14:18:44.000000 excel_graph_parser-0.1.8/pyproject.toml
--rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-04-15 14:20:45.431510 excel_graph_parser-0.1.8/setup.cfg
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-23 08:59:40.607172 excel_graph_parser-0.1.9/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1063 2024-02-13 13:30:58.000000 excel_graph_parser-0.1.9/LICENSE
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-23 08:59:40.607172 excel_graph_parser-0.1.9/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      759 2024-04-23 08:56:31.000000 excel_graph_parser-0.1.9/README.md
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-23 08:59:40.607172 excel_graph_parser-0.1.9/excel_graph_parser/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      140 2024-02-13 14:42:52.000000 excel_graph_parser-0.1.9/excel_graph_parser/__init__.py
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)    13475 2024-04-15 14:17:41.000000 excel_graph_parser-0.1.9/excel_graph_parser/graph_parser.py
+drwxr-xr-x   0 dsommers  (1000) dsommers  (1000)        0 2024-04-23 08:59:40.607172 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     2655 2024-04-23 08:59:40.000000 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/PKG-INFO
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)      307 2024-04-23 08:59:40.000000 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)        1 2024-04-23 08:59:40.000000 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       49 2024-04-23 08:59:40.000000 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/requires.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       19 2024-04-23 08:59:40.000000 excel_graph_parser-0.1.9/excel_graph_parser.egg-info/top_level.txt
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)     1209 2024-04-23 08:56:48.000000 excel_graph_parser-0.1.9/pyproject.toml
+-rw-r--r--   0 dsommers  (1000) dsommers  (1000)       38 2024-04-23 08:59:40.607172 excel_graph_parser-0.1.9/setup.cfg
```

### Comparing `excel_graph_parser-0.1.8/LICENSE` & `excel_graph_parser-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.8/PKG-INFO` & `excel_graph_parser-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
         
@@ -24,15 +24,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/viktor-platform/excel_graph_parser
 Project-URL: Bug Reports, https://github.com/viktor-platform/excel_graph_parser/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: viktor
 Requires-Dist: openpyxl
 Requires-Dist: plotly
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
@@ -42,15 +42,15 @@
 # Excel graph parser (open-source parser for translation of excel graphs to Plotly figures)
 This repository can be installed to show nicely formatted graphs generated by excel documents.
 Currently only useful for [VIKTOR](https://www.viktor.ai) applications.
 
 # Installation
 Paste the link of this repository in your `requirements.txt`:
 ```text
-viktor==14.7.0
+viktor==14.9.0
 excel-graph-parser
 ```
 
 # Contributing
 Improvements to the view are very welcome. Please ensure your improvements adhere to the code standards by running 
 black, isort and pylint (with the versions specified in `dev-requirements.txt`):
 ```shell
```

### Comparing `excel_graph_parser-0.1.8/README.md` & `excel_graph_parser-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Excel graph parser (open-source parser for translation of excel graphs to Plotly figures)
 This repository can be installed to show nicely formatted graphs generated by excel documents.
 Currently only useful for [VIKTOR](https://www.viktor.ai) applications.
 
 # Installation
 Paste the link of this repository in your `requirements.txt`:
 ```text
-viktor==14.7.0
+viktor==14.9.0
 excel-graph-parser
 ```
 
 # Contributing
 Improvements to the view are very welcome. Please ensure your improvements adhere to the code standards by running 
 black, isort and pylint (with the versions specified in `dev-requirements.txt`):
 ```shell
```

### Comparing `excel_graph_parser-0.1.8/excel_graph_parser/graph_parser.py` & `excel_graph_parser-0.1.9/excel_graph_parser/graph_parser.py`

 * *Files identical despite different names*

### Comparing `excel_graph_parser-0.1.8/excel_graph_parser.egg-info/PKG-INFO` & `excel_graph_parser-0.1.9/excel_graph_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excel_graph_parser
-Version: 0.1.8
+Version: 0.1.9
 Summary: Parser to translate excel graphs to Plotly figures
 Author-email: "D. Sommers" <dsommers@viktor.ai>
 Maintainer-email: "D. Sommers" <dsommers@viktor.ai>
 License: MIT License
         
         Copyright (c) 2024 VIKTOR
         
@@ -24,15 +24,15 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/viktor-platform/excel_graph_parser
 Project-URL: Bug Reports, https://github.com/viktor-platform/excel_graph_parser/issues
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: viktor
 Requires-Dist: openpyxl
 Requires-Dist: plotly
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
@@ -42,15 +42,15 @@
 # Excel graph parser (open-source parser for translation of excel graphs to Plotly figures)
 This repository can be installed to show nicely formatted graphs generated by excel documents.
 Currently only useful for [VIKTOR](https://www.viktor.ai) applications.
 
 # Installation
 Paste the link of this repository in your `requirements.txt`:
 ```text
-viktor==14.7.0
+viktor==14.9.0
 excel-graph-parser
 ```
 
 # Contributing
 Improvements to the view are very welcome. Please ensure your improvements adhere to the code standards by running 
 black, isort and pylint (with the versions specified in `dev-requirements.txt`):
 ```shell
```

### Comparing `excel_graph_parser-0.1.8/pyproject.toml` & `excel_graph_parser-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "excel_graph_parser"
-version = "0.1.8"
+version = "0.1.9"
 description = "Parser to translate excel graphs to Plotly figures"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "D. Sommers", email = "dsommers@viktor.ai" }
 ]
 maintainers = [
     {name = "D. Sommers", email = "dsommers@viktor.ai" }
 ]
```

