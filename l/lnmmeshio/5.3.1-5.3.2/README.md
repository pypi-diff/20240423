# Comparing `tmp/lnmmeshio-5.3.1.tar.gz` & `tmp/lnmmeshio-5.3.2.tar.gz`

## Comparing `lnmmeshio-5.3.1.tar` & `lnmmeshio-5.3.2.tar`

### file list

```diff
@@ -1,65 +1,64 @@
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.isort.cfg
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/pytest.ini
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/requirements-dev.txt
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/requirements.txt
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.github/workflows/build_and_test.yml
--rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/__init__.py
--rw-r--r--   0        0        0    11170 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/discretization.py
--rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/ensightio.py
--rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/fiber.py
--rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/ioutils.py
--rw-r--r--   0        0        0    11395 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/meshio_to_discretization.py
--rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/mimics_stlio.py
--rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/node.py
--rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/nodeset.py
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/progress.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/__init__.py
--rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/element.py
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/element_container.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex20.py
--rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex27.py
--rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/hex8.py
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/line2.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/line3.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/parse_element.py
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/pyramid5.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad4.py
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad8.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/quad9.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tet10.py
--rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tet4.py
--rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tri3.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/tri6.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/vertex.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/element/wedge6.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/__init__.py
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/component.py
--rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/function.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/linear_interpolation_variable.py
--rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/variable.py
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/src/lnmmeshio/functions/variablereader.py
--rw-r--r--   0        0        0    13793 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_disc.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_discretization.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_ele_container.py
--rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_element_factory.py
--rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_eles.py
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_ensight.py
--rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_fibers.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_integration.py
--rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_meshio2discretization.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_mimics_stlio.py
--rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_override.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/test_write_data.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/cube.mesh
--rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/cube.stl
--rw-r--r--   0        0        0    17237 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.dat
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.mesh
--rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.stl
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/dummy2.dat
--rw-r--r--   0        0        0     4332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/test_lnmmeshio/data/full.dat
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/LICENSE
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/README.md
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/pyproject.toml
--rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.3.1/PKG-INFO
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/.isort.cfg
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/pytest.ini
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/requirements-dev.txt
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/requirements.txt
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/.github/workflows/build_and_test.yml
+-rw-r--r--   0        0        0     7254 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/__init__.py
+-rw-r--r--   0        0        0    11170 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/discretization.py
+-rw-r--r--   0        0        0    13496 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/ensightio.py
+-rw-r--r--   0        0        0     7541 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/fiber.py
+-rw-r--r--   0        0        0     8244 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/ioutils.py
+-rw-r--r--   0        0        0    11379 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/meshio_to_discretization.py
+-rw-r--r--   0        0        0     4033 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/mimics_stlio.py
+-rw-r--r--   0        0        0     2290 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/node.py
+-rw-r--r--   0        0        0     5728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/nodeset.py
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/progress.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/__init__.py
+-rw-r--r--   0        0        0    16512 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/element.py
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/element_container.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/hex20.py
+-rw-r--r--   0        0        0     5792 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/hex27.py
+-rw-r--r--   0        0        0     5672 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/hex8.py
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/line2.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/line3.py
+-rw-r--r--   0        0        0     3674 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/parse_element.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/pyramid5.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/quad4.py
+-rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/quad8.py
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/quad9.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/tet10.py
+-rw-r--r--   0        0        0     3324 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/tet4.py
+-rw-r--r--   0        0        0     3884 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/tri3.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/tri6.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/vertex.py
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/element/wedge6.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/__init__.py
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/component.py
+-rw-r--r--   0        0        0     3161 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/function.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/linear_interpolation_variable.py
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/variable.py
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/src/lnmmeshio/functions/variablereader.py
+-rw-r--r--   0        0        0    13789 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_disc.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_discretization.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_ele_container.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_element_factory.py
+-rw-r--r--   0        0        0    20936 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_eles.py
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_ensight.py
+-rw-r--r--   0        0        0     3445 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_fibers.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_integration.py
+-rw-r--r--   0        0        0     5565 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_meshio2discretization.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_mimics_stlio.py
+-rw-r--r--   0        0        0     1370 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_override.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/test_write_data.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/cube.mesh
+-rw-r--r--   0        0        0      684 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/cube.stl
+-rw-r--r--   0        0        0    17047 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/dummy.dat
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/dummy.mesh
+-rw-r--r--   0        0        0   928184 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/dummy.stl
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/test_lnmmeshio/data/dummy2.dat
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/LICENSE
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/README.md
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2643 2020-02-02 00:00:00.000000 lnmmeshio-5.3.2/PKG-INFO
```

### Comparing `lnmmeshio-5.3.1/.github/workflows/build_and_test.yml` & `lnmmeshio-5.3.2/.github/workflows/build_and_test.yml`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/__init__.py` & `lnmmeshio-5.3.2/src/lnmmeshio/__init__.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/discretization.py` & `lnmmeshio-5.3.2/src/lnmmeshio/discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/ensightio.py` & `lnmmeshio-5.3.2/src/lnmmeshio/ensightio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/fiber.py` & `lnmmeshio-5.3.2/src/lnmmeshio/fiber.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/ioutils.py` & `lnmmeshio-5.3.2/src/lnmmeshio/ioutils.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/meshio_to_discretization.py` & `lnmmeshio-5.3.2/src/lnmmeshio/meshio_to_discretization.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,20 +48,20 @@
 
 cell_disc_eles = {
     "vertex": "UNKNOWN",
     "line": "UNKNOWN",
     "line3": "UNKNOWN",
     "triangle": "UNKNOWN",
     "triangle6": "UNKNOWN",
-    "tetra": "SOLIDT4",
-    "tetra10": "SOLIDT10",
-    "pyramid": "PYRAMID5",
-    "hexahedron": "SOLIDH8",
-    "hexahedron20": "SOLIDH20",
-    "hexahedron27": "SOLIDH27",
+    "tetra": "SOLID",
+    "tetra10": "SOLID",
+    "pyramid": "SOLID",
+    "hexahedron": "SOLID",
+    "hexahedron20": "SOLID",
+    "hexahedron27": "SOLID",
     "wedge": "UNKNOWN",
     "quad": "UNKNOWN",
     "quad9": "UNKNOWN",
 }
 
 cell_disc_shape = {
     "vertex": "VERTEX1",
```

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/mimics_stlio.py` & `lnmmeshio-5.3.2/src/lnmmeshio/mimics_stlio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/node.py` & `lnmmeshio-5.3.2/src/lnmmeshio/node.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/nodeset.py` & `lnmmeshio-5.3.2/src/lnmmeshio/nodeset.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/progress.py` & `lnmmeshio-5.3.2/src/lnmmeshio/progress.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/element.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/element.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/element_container.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/element_container.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/hex20.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/hex20.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/hex27.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/hex27.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/hex8.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/hex8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/line2.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/line2.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/line3.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/line3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/parse_element.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/parse_element.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def create_element(
     ele_type: str, ele_shape: str, ele_nodes: List[Node], throw_if_unknown=False
 ) -> Element:
     """
     Creates an element from a given element shape
 
     Args:
-        elename: name of the element (e.g. SOLIDH8)
+        elename: name of the element (e.g. SOLID)
         shape: str shape of the element (e.g. HEX8)
         nodes: nodes of the element
         throw_if_unknown: bool Throw an exception, if element type is not known
 
     Return:
         Element of the specific type
     """
```

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/pyramid5.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/pyramid5.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/quad4.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/quad4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/quad8.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/quad8.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/quad9.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/quad9.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/tet10.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/tet10.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/tet4.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/tet4.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/tri3.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/tri3.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/tri6.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/tri6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/vertex.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/vertex.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/element/wedge6.py` & `lnmmeshio-5.3.2/src/lnmmeshio/element/wedge6.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/functions/component.py` & `lnmmeshio-5.3.2/src/lnmmeshio/functions/component.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/functions/function.py` & `lnmmeshio-5.3.2/src/lnmmeshio/functions/function.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/functions/linear_interpolation_variable.py` & `lnmmeshio-5.3.2/src/lnmmeshio/functions/linear_interpolation_variable.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/src/lnmmeshio/functions/variablereader.py` & `lnmmeshio-5.3.2/src/lnmmeshio/functions/variablereader.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_disc.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_disc.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         for i in range(0, 3):
             d.surfacenodesets[0].add_node(d.nodes[i])
 
         # dvol
         for i in range(0, 4):
             d.volumenodesets[0].add_node(d.nodes[i])
 
-        d.elements.structure = [lnmmeshio.Element("SOLIDT4SCATRA", "TET4", d.nodes)]
+        d.elements.structure = [lnmmeshio.Element("SOLIDSCATRA", "TET4", d.nodes)]
         d.elements.structure[0].options = {
             "MAT": 1,
             "KINEM": "nonlinear",
             "TYPE": "Std",
         }
 
         dummy_file = io.StringIO()
@@ -163,15 +163,15 @@
             [sorted([n.id for n in nds]) for nds in d_new.surfacenodesets], [[0, 1, 2]]
         )
         self.assertListEqual(
             [sorted([n.id for n in nds]) for nds in d_new.volumenodesets],
             [[0, 1, 2, 3]],
         )
 
-        self.assertEqual(d_new.elements.structure[0].type, "SOLIDT4SCATRA")
+        self.assertEqual(d_new.elements.structure[0].type, "SOLIDSCATRA")
         self.assertEqual(d_new.elements.structure[0].shape, "TET4")
         self.assertListEqual(d_new.elements.structure[0].nodes, d_new.nodes)
         self.assertEqual(d_new.elements.structure[0].options["MAT"], "1")
         self.assertEqual(d_new.elements.structure[0].options["KINEM"], "nonlinear")
         self.assertEqual(d_new.elements.structure[0].options["TYPE"], "Std")
 
     def test_io_utils_text_fill(self):
```

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_discretization.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_ele_container.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_ele_container.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_element_factory.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_element_factory.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_eles.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_eles.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_ensight.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_ensight.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_fibers.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_fibers.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_integration.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_integration.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_meshio2discretization.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_meshio2discretization.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_mimics_stlio.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_mimics_stlio.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_override.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_override.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/test_write_data.py` & `lnmmeshio-5.3.2/test_lnmmeshio/test_write_data.py`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/data/cube.stl` & `lnmmeshio-5.3.2/test_lnmmeshio/data/cube.stl`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.dat` & `lnmmeshio-5.3.2/test_lnmmeshio/data/dummy.dat`

 * *Files 3% similar despite different names*

```diff
@@ -403,96 +403,96 @@
 NODE 219 COORD 1.0 0.5 14.0
 NODE 220 COORD 1.0 1.0 15.5
 NODE 221 COORD 1.0 1.0 16.0
 NODE 222 COORD 1.0 1.0 15.0
 NODE 223 COORD 1.0 1.0 14.5
 NODE 224 COORD 1.0 1.0 14.0
 -------------------------------------------------------STRUCTURE ELEMENTS
-1 SOLIDH8 HEX8 1 2 3 4 5 6 7 8 MAT 1 KINEM nonlinear EAS none
-2 SOLIDT4 TET4 56 57 58 59 MAT 4 KINEM nonlinear
-3 SOLIDT4 TET4 60 59 61 58 MAT 4 KINEM nonlinear
-4 SOLIDT4 TET4 56 62 57 59 MAT 4 KINEM nonlinear
-5 SOLIDT4 TET4 59 62 57 60 MAT 4 KINEM nonlinear
-6 SOLIDT4 TET4 59 63 64 62 MAT 4 KINEM nonlinear
-7 SOLIDT4 TET4 56 62 59 64 MAT 4 KINEM nonlinear
-8 SOLIDT4 TET4 56 64 59 61 MAT 4 KINEM nonlinear
-9 SOLIDT4 TET4 59 64 63 61 MAT 4 KINEM nonlinear
-10 SOLIDT4 TET4 61 58 59 56 MAT 4 KINEM nonlinear
-11 SOLIDT4 TET4 59 57 58 60 MAT 4 KINEM nonlinear
-12 SOLIDT4 TET4 61 63 59 60 MAT 4 KINEM nonlinear
-13 SOLIDT4 TET4 62 59 63 60 MAT 4 KINEM nonlinear
-14 SOLIDT10 TET10 65 66 67 68 69 70 71 72 73 74 MAT 5 KINEM nonlinear
-15 SOLIDT10 TET10 75 66 65 76 77 69 78 79 80 81 MAT 5 KINEM nonlinear
-16 SOLIDT10 TET10 82 83 65 84 85 86 87 88 89 90 MAT 5 KINEM nonlinear
-17 SOLIDT10 TET10 84 66 65 75 91 69 90 92 77 78 MAT 5 KINEM nonlinear
-18 SOLIDT10 TET10 76 83 65 82 93 86 81 94 85 87 MAT 5 KINEM nonlinear
-19 SOLIDT10 TET10 65 68 67 83 72 74 71 86 95 96 MAT 5 KINEM nonlinear
-20 SOLIDT10 TET10 67 66 65 84 70 69 71 97 91 90 MAT 5 KINEM nonlinear
-21 SOLIDT10 TET10 67 65 83 84 71 86 96 97 90 89 MAT 5 KINEM nonlinear
-22 SOLIDT10 TET10 84 82 75 65 88 98 92 90 87 78 MAT 5 KINEM nonlinear
-23 SOLIDT10 TET10 65 82 75 76 87 98 78 81 94 79 MAT 5 KINEM nonlinear
-24 SOLIDT10 TET10 76 65 83 68 81 86 93 99 72 95 MAT 5 KINEM nonlinear
-25 SOLIDT10 TET10 76 66 65 68 80 69 81 99 73 72 MAT 5 KINEM nonlinear
-26 SOLIDH8 HEX8 100 101 102 103 104 105 106 107 MAT 6 KINEM nonlinear EAS none
-27 SOLIDH8 HEX8 101 108 109 102 105 110 111 106 MAT 6 KINEM nonlinear EAS none
-28 SOLIDH8 HEX8 108 112 113 109 110 114 115 111 MAT 6 KINEM nonlinear EAS none
-29 SOLIDH8 HEX8 112 116 117 113 114 118 119 115 MAT 6 KINEM nonlinear EAS none
-30 SOLIDH8 HEX8 103 102 120 121 107 106 122 123 MAT 6 KINEM nonlinear EAS none
-31 SOLIDH8 HEX8 102 109 124 120 106 111 125 122 MAT 6 KINEM nonlinear EAS none
-32 SOLIDH8 HEX8 109 113 126 124 111 115 127 125 MAT 6 KINEM nonlinear EAS none
-33 SOLIDH8 HEX8 113 117 128 126 115 119 129 127 MAT 6 KINEM nonlinear EAS none
-34 SOLIDH8 HEX8 121 120 130 131 123 122 132 133 MAT 6 KINEM nonlinear EAS none
-35 SOLIDH8 HEX8 120 124 134 130 122 125 135 132 MAT 6 KINEM nonlinear EAS none
-36 SOLIDH8 HEX8 124 126 136 134 125 127 137 135 MAT 6 KINEM nonlinear EAS none
-37 SOLIDH8 HEX8 126 128 138 136 127 129 139 137 MAT 6 KINEM nonlinear EAS none
-38 SOLIDH8 HEX8 131 130 140 141 133 132 142 143 MAT 6 KINEM nonlinear EAS none
-39 SOLIDH8 HEX8 130 134 144 140 132 135 145 142 MAT 6 KINEM nonlinear EAS none
-40 SOLIDH8 HEX8 134 136 146 144 135 137 147 145 MAT 6 KINEM nonlinear EAS none
-41 SOLIDH8 HEX8 136 138 148 146 137 139 149 147 MAT 6 KINEM nonlinear EAS none
-42 SOLIDH8 HEX8 104 105 106 107 150 151 152 153 MAT 6 KINEM nonlinear EAS none
-43 SOLIDH8 HEX8 105 110 111 106 151 154 155 152 MAT 6 KINEM nonlinear EAS none
-44 SOLIDH8 HEX8 110 114 115 111 154 156 157 155 MAT 6 KINEM nonlinear EAS none
-45 SOLIDH8 HEX8 114 118 119 115 156 158 159 157 MAT 6 KINEM nonlinear EAS none
-46 SOLIDH8 HEX8 107 106 122 123 153 152 160 161 MAT 6 KINEM nonlinear EAS none
-47 SOLIDH8 HEX8 106 111 125 122 152 155 162 160 MAT 6 KINEM nonlinear EAS none
-48 SOLIDH8 HEX8 111 115 127 125 155 157 163 162 MAT 6 KINEM nonlinear EAS none
-49 SOLIDH8 HEX8 115 119 129 127 157 159 164 163 MAT 6 KINEM nonlinear EAS none
-50 SOLIDH8 HEX8 123 122 132 133 161 160 165 166 MAT 6 KINEM nonlinear EAS none
-51 SOLIDH8 HEX8 122 125 135 132 160 162 167 165 MAT 6 KINEM nonlinear EAS none
-52 SOLIDH8 HEX8 125 127 137 135 162 163 168 167 MAT 6 KINEM nonlinear EAS none
-53 SOLIDH8 HEX8 127 129 139 137 163 164 169 168 MAT 6 KINEM nonlinear EAS none
-54 SOLIDH8 HEX8 133 132 142 143 166 165 170 171 MAT 6 KINEM nonlinear EAS none
-55 SOLIDH8 HEX8 132 135 145 142 165 167 172 170 MAT 6 KINEM nonlinear EAS none
-56 SOLIDH8 HEX8 135 137 147 145 167 168 173 172 MAT 6 KINEM nonlinear EAS none
-57 SOLIDH8 HEX8 137 139 149 147 168 169 174 173 MAT 6 KINEM nonlinear EAS none
-58 SOLIDH8 HEX8 150 151 152 153 175 176 177 178 MAT 6 KINEM nonlinear EAS none
-59 SOLIDH8 HEX8 151 154 155 152 176 179 180 177 MAT 6 KINEM nonlinear EAS none
-60 SOLIDH8 HEX8 154 156 157 155 179 181 182 180 MAT 6 KINEM nonlinear EAS none
-61 SOLIDH8 HEX8 156 158 159 157 181 183 184 182 MAT 6 KINEM nonlinear EAS none
-62 SOLIDH8 HEX8 153 152 160 161 178 177 185 186 MAT 6 KINEM nonlinear EAS none
-63 SOLIDH8 HEX8 152 155 162 160 177 180 187 185 MAT 6 KINEM nonlinear EAS none
-64 SOLIDH8 HEX8 155 157 163 162 180 182 188 187 MAT 6 KINEM nonlinear EAS none
-65 SOLIDH8 HEX8 157 159 164 163 182 184 189 188 MAT 6 KINEM nonlinear EAS none
-66 SOLIDH8 HEX8 161 160 165 166 186 185 190 191 MAT 6 KINEM nonlinear EAS none
-67 SOLIDH8 HEX8 160 162 167 165 185 187 192 190 MAT 6 KINEM nonlinear EAS none
-68 SOLIDH8 HEX8 162 163 168 167 187 188 193 192 MAT 6 KINEM nonlinear EAS none
-69 SOLIDH8 HEX8 163 164 169 168 188 189 194 193 MAT 6 KINEM nonlinear EAS none
-70 SOLIDH8 HEX8 166 165 170 171 191 190 195 196 MAT 6 KINEM nonlinear EAS none
-71 SOLIDH8 HEX8 165 167 172 170 190 192 197 195 MAT 6 KINEM nonlinear EAS none
-72 SOLIDH8 HEX8 167 168 173 172 192 193 198 197 MAT 6 KINEM nonlinear EAS none
-73 SOLIDH8 HEX8 168 169 174 173 193 194 199 198 MAT 6 KINEM nonlinear EAS none
-74 SOLIDH8 HEX8 175 176 177 178 200 201 202 203 MAT 6 KINEM nonlinear EAS none
-75 SOLIDH8 HEX8 176 179 180 177 201 204 205 202 MAT 6 KINEM nonlinear EAS none
-76 SOLIDH8 HEX8 179 181 182 180 204 206 207 205 MAT 6 KINEM nonlinear EAS none
-77 SOLIDH8 HEX8 181 183 184 182 206 208 209 207 MAT 6 KINEM nonlinear EAS none
-78 SOLIDH8 HEX8 178 177 185 186 203 202 210 211 MAT 6 KINEM nonlinear EAS none
-79 SOLIDH8 HEX8 177 180 187 185 202 205 212 210 MAT 6 KINEM nonlinear EAS none
-80 SOLIDH8 HEX8 180 182 188 187 205 207 213 212 MAT 6 KINEM nonlinear EAS none
-81 SOLIDH8 HEX8 182 184 189 188 207 209 214 213 MAT 6 KINEM nonlinear EAS none
-82 SOLIDH8 HEX8 186 185 190 191 211 210 215 216 MAT 6 KINEM nonlinear EAS none
-83 SOLIDH8 HEX8 185 187 192 190 210 212 217 215 MAT 6 KINEM nonlinear EAS none
-84 SOLIDH8 HEX8 187 188 193 192 212 213 218 217 MAT 6 KINEM nonlinear EAS none
-85 SOLIDH8 HEX8 188 189 194 193 213 214 219 218 MAT 6 KINEM nonlinear EAS none
-86 SOLIDH8 HEX8 191 190 195 196 216 215 220 221 MAT 6 KINEM nonlinear EAS none
-87 SOLIDH8 HEX8 190 192 197 195 215 217 222 220 MAT 6 KINEM nonlinear EAS none
-88 SOLIDH8 HEX8 192 193 198 197 217 218 223 222 MAT 6 KINEM nonlinear EAS none
-89 SOLIDH8 HEX8 193 194 199 198 218 219 224 223 MAT 6 KINEM nonlinear EAS none
+1 SOLID HEX8 1 2 3 4 5 6 7 8 MAT 1 KINEM nonlinear EAS none
+2 SOLID TET4 56 57 58 59 MAT 4 KINEM nonlinear
+3 SOLID TET4 60 59 61 58 MAT 4 KINEM nonlinear
+4 SOLID TET4 56 62 57 59 MAT 4 KINEM nonlinear
+5 SOLID TET4 59 62 57 60 MAT 4 KINEM nonlinear
+6 SOLID TET4 59 63 64 62 MAT 4 KINEM nonlinear
+7 SOLID TET4 56 62 59 64 MAT 4 KINEM nonlinear
+8 SOLID TET4 56 64 59 61 MAT 4 KINEM nonlinear
+9 SOLID TET4 59 64 63 61 MAT 4 KINEM nonlinear
+10 SOLID TET4 61 58 59 56 MAT 4 KINEM nonlinear
+11 SOLID TET4 59 57 58 60 MAT 4 KINEM nonlinear
+12 SOLID TET4 61 63 59 60 MAT 4 KINEM nonlinear
+13 SOLID TET4 62 59 63 60 MAT 4 KINEM nonlinear
+14 SOLID TET10 65 66 67 68 69 70 71 72 73 74 MAT 5 KINEM nonlinear
+15 SOLID TET10 75 66 65 76 77 69 78 79 80 81 MAT 5 KINEM nonlinear
+16 SOLID TET10 82 83 65 84 85 86 87 88 89 90 MAT 5 KINEM nonlinear
+17 SOLID TET10 84 66 65 75 91 69 90 92 77 78 MAT 5 KINEM nonlinear
+18 SOLID TET10 76 83 65 82 93 86 81 94 85 87 MAT 5 KINEM nonlinear
+19 SOLID TET10 65 68 67 83 72 74 71 86 95 96 MAT 5 KINEM nonlinear
+20 SOLID TET10 67 66 65 84 70 69 71 97 91 90 MAT 5 KINEM nonlinear
+21 SOLID TET10 67 65 83 84 71 86 96 97 90 89 MAT 5 KINEM nonlinear
+22 SOLID TET10 84 82 75 65 88 98 92 90 87 78 MAT 5 KINEM nonlinear
+23 SOLID TET10 65 82 75 76 87 98 78 81 94 79 MAT 5 KINEM nonlinear
+24 SOLID TET10 76 65 83 68 81 86 93 99 72 95 MAT 5 KINEM nonlinear
+25 SOLID TET10 76 66 65 68 80 69 81 99 73 72 MAT 5 KINEM nonlinear
+26 SOLID HEX8 100 101 102 103 104 105 106 107 MAT 6 KINEM nonlinear EAS none
+27 SOLID HEX8 101 108 109 102 105 110 111 106 MAT 6 KINEM nonlinear EAS none
+28 SOLID HEX8 108 112 113 109 110 114 115 111 MAT 6 KINEM nonlinear EAS none
+29 SOLID HEX8 112 116 117 113 114 118 119 115 MAT 6 KINEM nonlinear EAS none
+30 SOLID HEX8 103 102 120 121 107 106 122 123 MAT 6 KINEM nonlinear EAS none
+31 SOLID HEX8 102 109 124 120 106 111 125 122 MAT 6 KINEM nonlinear EAS none
+32 SOLID HEX8 109 113 126 124 111 115 127 125 MAT 6 KINEM nonlinear EAS none
+33 SOLID HEX8 113 117 128 126 115 119 129 127 MAT 6 KINEM nonlinear EAS none
+34 SOLID HEX8 121 120 130 131 123 122 132 133 MAT 6 KINEM nonlinear EAS none
+35 SOLID HEX8 120 124 134 130 122 125 135 132 MAT 6 KINEM nonlinear EAS none
+36 SOLID HEX8 124 126 136 134 125 127 137 135 MAT 6 KINEM nonlinear EAS none
+37 SOLID HEX8 126 128 138 136 127 129 139 137 MAT 6 KINEM nonlinear EAS none
+38 SOLID HEX8 131 130 140 141 133 132 142 143 MAT 6 KINEM nonlinear EAS none
+39 SOLID HEX8 130 134 144 140 132 135 145 142 MAT 6 KINEM nonlinear EAS none
+40 SOLID HEX8 134 136 146 144 135 137 147 145 MAT 6 KINEM nonlinear EAS none
+41 SOLID HEX8 136 138 148 146 137 139 149 147 MAT 6 KINEM nonlinear EAS none
+42 SOLID HEX8 104 105 106 107 150 151 152 153 MAT 6 KINEM nonlinear EAS none
+43 SOLID HEX8 105 110 111 106 151 154 155 152 MAT 6 KINEM nonlinear EAS none
+44 SOLID HEX8 110 114 115 111 154 156 157 155 MAT 6 KINEM nonlinear EAS none
+45 SOLID HEX8 114 118 119 115 156 158 159 157 MAT 6 KINEM nonlinear EAS none
+46 SOLID HEX8 107 106 122 123 153 152 160 161 MAT 6 KINEM nonlinear EAS none
+47 SOLID HEX8 106 111 125 122 152 155 162 160 MAT 6 KINEM nonlinear EAS none
+48 SOLID HEX8 111 115 127 125 155 157 163 162 MAT 6 KINEM nonlinear EAS none
+49 SOLID HEX8 115 119 129 127 157 159 164 163 MAT 6 KINEM nonlinear EAS none
+50 SOLID HEX8 123 122 132 133 161 160 165 166 MAT 6 KINEM nonlinear EAS none
+51 SOLID HEX8 122 125 135 132 160 162 167 165 MAT 6 KINEM nonlinear EAS none
+52 SOLID HEX8 125 127 137 135 162 163 168 167 MAT 6 KINEM nonlinear EAS none
+53 SOLID HEX8 127 129 139 137 163 164 169 168 MAT 6 KINEM nonlinear EAS none
+54 SOLID HEX8 133 132 142 143 166 165 170 171 MAT 6 KINEM nonlinear EAS none
+55 SOLID HEX8 132 135 145 142 165 167 172 170 MAT 6 KINEM nonlinear EAS none
+56 SOLID HEX8 135 137 147 145 167 168 173 172 MAT 6 KINEM nonlinear EAS none
+57 SOLID HEX8 137 139 149 147 168 169 174 173 MAT 6 KINEM nonlinear EAS none
+58 SOLID HEX8 150 151 152 153 175 176 177 178 MAT 6 KINEM nonlinear EAS none
+59 SOLID HEX8 151 154 155 152 176 179 180 177 MAT 6 KINEM nonlinear EAS none
+60 SOLID HEX8 154 156 157 155 179 181 182 180 MAT 6 KINEM nonlinear EAS none
+61 SOLID HEX8 156 158 159 157 181 183 184 182 MAT 6 KINEM nonlinear EAS none
+62 SOLID HEX8 153 152 160 161 178 177 185 186 MAT 6 KINEM nonlinear EAS none
+63 SOLID HEX8 152 155 162 160 177 180 187 185 MAT 6 KINEM nonlinear EAS none
+64 SOLID HEX8 155 157 163 162 180 182 188 187 MAT 6 KINEM nonlinear EAS none
+65 SOLID HEX8 157 159 164 163 182 184 189 188 MAT 6 KINEM nonlinear EAS none
+66 SOLID HEX8 161 160 165 166 186 185 190 191 MAT 6 KINEM nonlinear EAS none
+67 SOLID HEX8 160 162 167 165 185 187 192 190 MAT 6 KINEM nonlinear EAS none
+68 SOLID HEX8 162 163 168 167 187 188 193 192 MAT 6 KINEM nonlinear EAS none
+69 SOLID HEX8 163 164 169 168 188 189 194 193 MAT 6 KINEM nonlinear EAS none
+70 SOLID HEX8 166 165 170 171 191 190 195 196 MAT 6 KINEM nonlinear EAS none
+71 SOLID HEX8 165 167 172 170 190 192 197 195 MAT 6 KINEM nonlinear EAS none
+72 SOLID HEX8 167 168 173 172 192 193 198 197 MAT 6 KINEM nonlinear EAS none
+73 SOLID HEX8 168 169 174 173 193 194 199 198 MAT 6 KINEM nonlinear EAS none
+74 SOLID HEX8 175 176 177 178 200 201 202 203 MAT 6 KINEM nonlinear EAS none
+75 SOLID HEX8 176 179 180 177 201 204 205 202 MAT 6 KINEM nonlinear EAS none
+76 SOLID HEX8 179 181 182 180 204 206 207 205 MAT 6 KINEM nonlinear EAS none
+77 SOLID HEX8 181 183 184 182 206 208 209 207 MAT 6 KINEM nonlinear EAS none
+78 SOLID HEX8 178 177 185 186 203 202 210 211 MAT 6 KINEM nonlinear EAS none
+79 SOLID HEX8 177 180 187 185 202 205 212 210 MAT 6 KINEM nonlinear EAS none
+80 SOLID HEX8 180 182 188 187 205 207 213 212 MAT 6 KINEM nonlinear EAS none
+81 SOLID HEX8 182 184 189 188 207 209 214 213 MAT 6 KINEM nonlinear EAS none
+82 SOLID HEX8 186 185 190 191 211 210 215 216 MAT 6 KINEM nonlinear EAS none
+83 SOLID HEX8 185 187 192 190 210 212 217 215 MAT 6 KINEM nonlinear EAS none
+84 SOLID HEX8 187 188 193 192 212 213 218 217 MAT 6 KINEM nonlinear EAS none
+85 SOLID HEX8 188 189 194 193 213 214 219 218 MAT 6 KINEM nonlinear EAS none
+86 SOLID HEX8 191 190 195 196 216 215 220 221 MAT 6 KINEM nonlinear EAS none
+87 SOLID HEX8 190 192 197 195 215 217 222 220 MAT 6 KINEM nonlinear EAS none
+88 SOLID HEX8 192 193 198 197 217 218 223 222 MAT 6 KINEM nonlinear EAS none
+89 SOLID HEX8 193 194 199 198 218 219 224 223 MAT 6 KINEM nonlinear EAS none
```

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy.stl` & `lnmmeshio-5.3.2/test_lnmmeshio/data/dummy.stl`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/test_lnmmeshio/data/dummy2.dat` & `lnmmeshio-5.3.2/test_lnmmeshio/data/dummy2.dat`

 * *Files 1% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 NODE 4 DVOL 1
 --------------------------------------------------------------NODE COORDS
 FNODE 1 COORD 0.0 0.0 0.0 FIBER1 1.0 0.0 0.0 FIBER2 0.0 1.0 0.0
 FNODE 2 COORD 1.0 0.0 0.0 FIBER1 1.0 0.0 0.0 FIBER2 0.0 1.0 0.0
 FNODE 3 COORD 0.0 1.0 0.0 FIBER1 1.0 0.0 0.0 FIBER2 0.0 1.0 0.0
 FNODE 4 COORD 0.0 0.0 1.0 FIBER1 1.0 0.0 0.0 FIBER2 0.0 1.0 0.0
 -------------------------------------------------------STRUCTURE ELEMENTS
-1 SOLIDT4SCATRA TET4 1 2 3 4 MAT 1 KINEM nonlinear TYPE Std
+1 SOLIDSCATRA TET4 1 2 3 4 MAT 1 KINEM nonlinear TYPE Std
```

### Comparing `lnmmeshio-5.3.1/LICENSE` & `lnmmeshio-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/README.md` & `lnmmeshio-5.3.2/README.md`

 * *Files identical despite different names*

### Comparing `lnmmeshio-5.3.1/pyproject.toml` & `lnmmeshio-5.3.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lnmmeshio"
-version = "5.3.1"
+version = "5.3.2"
 authors = [
   { name="Amadeus Gebauer", email="amadeus.gebauer@tum.de" },
 ]
 description = "Import and export from and to various mesh formats including dat files"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `lnmmeshio-5.3.1/PKG-INFO` & `lnmmeshio-5.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: lnmmeshio
-Version: 5.3.1
+Version: 5.3.2
 Summary: Import and export from and to various mesh formats including dat files
 Project-URL: Homepage, https://github.com/amgebauer/lnmmeshio
 Project-URL: Bug Tracker, https://github.com/amgebauer/lnmmeshio/issues
 Author-email: Amadeus Gebauer <amadeus.gebauer@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

