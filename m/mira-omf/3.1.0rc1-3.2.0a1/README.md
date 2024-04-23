# Comparing `tmp/mira_omf-3.1.0rc1.tar.gz` & `tmp/mira_omf-3.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mira_omf-3.1.0rc1.tar", max compression
+gzip compressed data, was "mira_omf-3.2.0a1.tar", max compression
```

## Comparing `mira_omf-3.1.0rc1.tar` & `mira_omf-3.2.0a1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1122 2023-10-10 18:38:14.946657 mira_omf-3.1.0rc1/LICENSE
--rw-r--r--   0        0        0     1684 2023-11-23 18:52:02.199192 mira_omf-3.1.0rc1/omf/__init__.py
--rw-r--r--   0        0        0     6754 2023-10-10 18:38:16.651487 mira_omf-3.1.0rc1/omf/base.py
--rw-r--r--   0        0        0     8561 2023-10-10 18:38:16.652017 mira_omf-3.1.0rc1/omf/data.py
--rw-r--r--   0        0        0      111 2023-10-10 18:38:16.652566 mira_omf-3.1.0rc1/omf/fileio/__init__.py
--rw-r--r--   0        0        0     6049 2023-10-10 18:38:16.652566 mira_omf-3.1.0rc1/omf/fileio/fileio.py
--rw-r--r--   0        0        0    43690 2023-11-23 18:51:16.819644 mira_omf-3.1.0rc1/omf/fileio/geoh5.py
--rw-r--r--   0        0        0     1123 2023-10-10 18:38:16.653603 mira_omf-3.1.0rc1/omf/fileio/utils.py
--rw-r--r--   0        0        0     1760 2023-10-10 18:38:16.653603 mira_omf-3.1.0rc1/omf/lineset.py
--rw-r--r--   0        0        0     1411 2023-10-10 18:38:16.654144 mira_omf-3.1.0rc1/omf/pointset.py
--rw-r--r--   0        0        0        0 2023-10-10 18:38:16.654677 mira_omf-3.1.0rc1/omf/scripts/__init__.py
--rw-r--r--   0        0        0     1171 2023-11-23 18:51:16.819644 mira_omf-3.1.0rc1/omf/scripts/geoh5_to_omf.py
--rw-r--r--   0        0        0     1679 2023-11-23 18:51:16.819644 mira_omf-3.1.0rc1/omf/scripts/omf_to_geoh5.py
--rw-r--r--   0        0        0     3682 2023-10-10 18:38:16.655224 mira_omf-3.1.0rc1/omf/serializers.py
--rw-r--r--   0        0        0     3736 2023-10-10 18:38:16.655732 mira_omf-3.1.0rc1/omf/surface.py
--rw-r--r--   0        0        0      675 2023-10-10 18:38:16.656264 mira_omf-3.1.0rc1/omf/texture.py
--rw-r--r--   0        0        0     2409 2023-10-10 18:38:16.656814 mira_omf-3.1.0rc1/omf/volume.py
--rw-r--r--   0        0        0     1845 2023-11-23 18:51:47.062538 mira_omf-3.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2786 2023-11-23 18:58:31.166270 mira_omf-3.1.0rc1/README.rst
--rw-r--r--   0        0        0     3983 1970-01-01 00:00:00.000000 mira_omf-3.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1122 2023-10-10 18:38:14.946657 mira_omf-3.2.0a1/LICENSE
+-rw-r--r--   0        0        0     1687 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/__init__.py
+-rw-r--r--   0        0        0     6754 2023-10-10 18:38:16.651487 mira_omf-3.2.0a1/omf/base.py
+-rw-r--r--   0        0        0     8561 2023-10-10 18:38:16.652017 mira_omf-3.2.0a1/omf/data.py
+-rw-r--r--   0        0        0      111 2023-10-10 18:38:16.652566 mira_omf-3.2.0a1/omf/fileio/__init__.py
+-rw-r--r--   0        0        0     6049 2024-01-10 23:48:56.546364 mira_omf-3.2.0a1/omf/fileio/fileio.py
+-rw-r--r--   0        0        0    43690 2024-01-10 23:48:56.547396 mira_omf-3.2.0a1/omf/fileio/geoh5.py
+-rw-r--r--   0        0        0     1123 2023-10-10 18:38:16.653603 mira_omf-3.2.0a1/omf/fileio/utils.py
+-rw-r--r--   0        0        0     1760 2023-10-10 18:38:16.653603 mira_omf-3.2.0a1/omf/lineset.py
+-rw-r--r--   0        0        0     1411 2023-10-10 18:38:16.654144 mira_omf-3.2.0a1/omf/pointset.py
+-rw-r--r--   0        0        0        0 2023-10-10 18:38:16.654677 mira_omf-3.2.0a1/omf/scripts/__init__.py
+-rw-r--r--   0        0        0     1221 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/scripts/geoh5_to_omf.py
+-rw-r--r--   0        0        0     1729 2024-04-23 17:10:17.046332 mira_omf-3.2.0a1/omf/scripts/omf_to_geoh5.py
+-rw-r--r--   0        0        0     3682 2023-10-10 18:38:16.655224 mira_omf-3.2.0a1/omf/serializers.py
+-rw-r--r--   0        0        0     3736 2023-10-10 18:38:16.655732 mira_omf-3.2.0a1/omf/surface.py
+-rw-r--r--   0        0        0      675 2023-10-10 18:38:16.656264 mira_omf-3.2.0a1/omf/texture.py
+-rw-r--r--   0        0        0     2409 2023-10-10 18:38:16.656814 mira_omf-3.2.0a1/omf/volume.py
+-rw-r--r--   0        0        0     1854 2024-04-23 17:11:09.514140 mira_omf-3.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0     2789 2024-04-23 17:11:09.514140 mira_omf-3.2.0a1/README.rst
+-rw-r--r--   0        0        0     3991 1970-01-01 00:00:00.000000 mira_omf-3.2.0a1/PKG-INFO
```

### Comparing `mira_omf-3.1.0rc1/LICENSE` & `mira_omf-3.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/__init__.py` & `mira_omf-3.2.0a1/omf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from .fileio import GeoH5Writer, OMFReader, OMFWriter
 from .lineset import LineSetElement, LineSetGeometry
 from .pointset import PointSetElement, PointSetGeometry
 from .surface import SurfaceElement, SurfaceGeometry, SurfaceGridGeometry
 from .texture import ImageTexture
 from .volume import VolumeElement, VolumeGridGeometry
 
-__version__ = "3.1.0-rc.1"
+__version__ = "3.2.0-alpha.1"
 __author__ = "Global Mining Standards and Guidelines Group"
 __license__ = "MIT License"
 __copyright__ = "Copyright 2017 Global Mining Standards and Guidelines Group"
 
 
 def _create_logger():
     error_handler = logging.StreamHandler(sys.stderr)
```

### Comparing `mira_omf-3.1.0rc1/omf/base.py` & `mira_omf-3.2.0a1/omf/base.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/data.py` & `mira_omf-3.2.0a1/omf/data.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/fileio/fileio.py` & `mira_omf-3.2.0a1/omf/fileio/fileio.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/fileio/geoh5.py` & `mira_omf-3.2.0a1/omf/fileio/geoh5.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/fileio/utils.py` & `mira_omf-3.2.0a1/omf/fileio/utils.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/lineset.py` & `mira_omf-3.2.0a1/omf/lineset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/pointset.py` & `mira_omf-3.2.0a1/omf/pointset.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/scripts/geoh5_to_omf.py` & `mira_omf-3.2.0a1/omf/scripts/geoh5_to_omf.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import sys
 from pathlib import Path
 
 from omf.fileio import OMFWriter
 from omf.fileio.geoh5 import GeoH5Reader
 
-_logger = logging.getLogger(__package__)
+_logger = logging.getLogger(__package__ + "." + Path(__file__).stem)
 
 
-def run():
+def main():
     parser = argparse.ArgumentParser(
         prog="geoh5_to_omf",
         description="Converts a geoh5 file to a new OMF file.",
     )
     parser.add_argument("geoh5_file", type=Path)
     parser.add_argument("-o", "--out", type=Path, required=False, default=None)
     args = parser.parse_args()
@@ -33,8 +33,8 @@
 
     reader = GeoH5Reader(geoh5_filepath)
     OMFWriter(reader(), str(output_filepath.absolute()))
     _logger.info("OMF file created: %s", output_filepath)
 
 
 if __name__ == "__main__":
-    run()
+    main()  # pragma: no cover
```

### Comparing `mira_omf-3.1.0rc1/omf/scripts/omf_to_geoh5.py` & `mira_omf-3.2.0a1/omf/scripts/omf_to_geoh5.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 import logging
 import sys
 from pathlib import Path
 
 from omf.fileio import OMFReader
 from omf.fileio.geoh5 import GeoH5Writer
 
-_logger = logging.getLogger(__package__)
+_logger = logging.getLogger(__package__ + "." + Path(__file__).stem)
 
 
-def run():
+def main():
     parser = argparse.ArgumentParser(
         prog="omf_to_geoh5",
         description="Converts an OMF file to a new geoh5 file.",
     )
     parser.add_argument("omf_file", type=Path, help="Path to the OMF file to convert.")
     parser.add_argument(
         "-o",
@@ -50,8 +50,8 @@
 
     reader = OMFReader(str(omf_filepath.absolute()))
     GeoH5Writer(reader.get_project(), output_filepath, compression=args.gzip)
     _logger.info("geoh5 file created: %s", output_filepath)
 
 
 if __name__ == "__main__":
-    run()
+    main()  # pragma: no cover
```

### Comparing `mira_omf-3.1.0rc1/omf/serializers.py` & `mira_omf-3.2.0a1/omf/serializers.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/surface.py` & `mira_omf-3.2.0a1/omf/surface.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/texture.py` & `mira_omf-3.2.0a1/omf/texture.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/omf/volume.py` & `mira_omf-3.2.0a1/omf/volume.py`

 * *Files identical despite different names*

### Comparing `mira_omf-3.1.0rc1/pyproject.toml` & `mira_omf-3.2.0a1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mira-omf"
-version = "3.1.0-rc.1"
+version = "3.2.0-alpha.1"
 description = "API Library for Open Mining Format"
 authors = [
     "Mira Geoscience <dominiquef@mirageoscience.com>",
     "Global Mining Standards and Guidelines Group <it@seequent.com>",
 ]
 repository = "https://github.com/MiraGeoscience/omf"
 homepage = "http://www.globalminingstandards.org/"
@@ -24,21 +24,21 @@
 ]
 
 packages = [
     { include = "omf" },
 ]
 
 [tool.poetry.scripts]
-geoh5_to_omf = 'omf.scripts.geoh5_to_omf:run'
-omf_to_geoh5 = 'omf.scripts.omf_to_geoh5:run'
+geoh5_to_omf = 'omf.scripts.geoh5_to_omf:main'
+omf_to_geoh5 = 'omf.scripts.omf_to_geoh5:main'
 
 [tool.poetry.dependencies]
 python = "^3.8,<3.11"
-geoh5py = {version = "~0.8.0rc2", allow-prereleases = true}
-# geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.8.0.zip#sha256="}
+geoh5py = {version = "~0.9.0-alpha.4", allow-prereleases = true}
+#geoh5py = {url = "https://github.com/MiraGeoscience/geoh5py/archive/refs/heads/release/0.9.0.zip#sha256="}
 numpy = "~1.23.5"
 properties = "~0.6.0"
 pypng = "^0.20220715"
 six = "^1.16"
 vectormath = "~0.2.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `mira_omf-3.1.0rc1/README.rst` & `mira_omf-3.2.0a1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.1.0-rc.1
+Version: 3.2.0-alpha.1
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <https://gmggroup.org/>`_.
 
 .. warning::
     **Pre-Release Notice**
```

### Comparing `mira_omf-3.1.0rc1/PKG-INFO` & `mira_omf-3.2.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mira-omf
-Version: 3.1.0rc1
+Version: 3.2.0a1
 Summary: API Library for Open Mining Format
 Home-page: http://www.globalminingstandards.org/
 Keywords: geology,geophysics,earth sciences
 Author: Mira Geoscience
 Author-email: dominiquef@mirageoscience.com
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: geoh5py (>=0.8.0rc2,<0.9.0)
+Requires-Dist: geoh5py (>=0.9.0-alpha.4,<0.10.0)
 Requires-Dist: numpy (>=1.23.5,<1.24.0)
 Requires-Dist: properties (>=0.6.0,<0.7.0)
 Requires-Dist: pypng (>=0.20220715,<0.20220716)
 Requires-Dist: six (>=1.16,<2.0)
 Requires-Dist: vectormath (>=0.2.0,<0.3.0)
 Project-URL: Repository, https://github.com/MiraGeoscience/omf
 Description-Content-Type: text/x-rst
@@ -46,15 +46,15 @@
     :alt: MIT license
 
 .. image:: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml/badge.svg
     :target: https://github.com/MiraGeoscience/omf/actions/workflows/pytest-windows.yml
     :alt: pytest
 
 
-Version: 3.1.0-rc.1
+Version: 3.2.0-alpha.1
 
 API library for Open Mining Format, a new standard for mining data backed by
 the `Global Mining Standards & Guidelines Group <https://gmggroup.org/>`_.
 
 .. warning::
     **Pre-Release Notice**
```

