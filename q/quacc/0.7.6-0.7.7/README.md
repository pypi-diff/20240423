# Comparing `tmp/quacc-0.7.6.tar.gz` & `tmp/quacc-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quacc-0.7.6.tar", last modified: Sat Apr 20 17:25:13 2024, max compression
+gzip compressed data, was "quacc-0.7.7.tar", last modified: Tue Apr 23 21:38:43 2024, max compression
```

## Comparing `quacc-0.7.6.tar` & `quacc-0.7.7.tar`

### file list

```diff
@@ -1,177 +1,177 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.230923 quacc-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-20 17:23:17.000000 quacc-0.7.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-20 17:23:17.000000 quacc-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-20 17:25:13.230923 quacc-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-20 17:23:17.000000 quacc-0.7.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-20 17:23:17.000000 quacc-0.7.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-20 17:25:13.230923 quacc-0.7.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.202923 quacc-0.7.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/_cli/quacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/atoms/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6421 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5323 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/deformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/atoms/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/calculators/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.206923 quacc-0.7.6/src/quacc/calculators/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17623 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/espresso.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/espresso/presets/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/metal_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    10584 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/espresso/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12398 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/qchem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/qchem/qchem_custodian.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.210923 quacc-0.7.6/src/quacc/calculators/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/params.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/calculators/vasp/presets/
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/BulkSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/QMOFSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/SlabSet.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_base.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_qmof.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/calculators/vasp/vasp_custodian.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/common/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/common/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/dftb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/dftb/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/emt/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/defects.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/elastic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/emt/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.214923 quacc-0.7.6/src/quacc/recipes/espresso/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/bands.py
--rw-r--r--   0 runner    (1001) docker     (127)    15327 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/dos.py
--rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/espresso/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/gaussian/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gaussian/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/gulp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/gulp/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/lj/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/lj/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/lj/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/mlp/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/mlp/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/newtonnet/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/newtonnet/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/onetep/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/onetep/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/orca/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6872 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/orca/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.218923 quacc-0.7.6/src/quacc/recipes/psi4/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/psi4/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/qchem/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7008 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/qchem/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/tblite/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/tblite/phonons.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/recipes/vasp/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/mp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9076 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/qmof.py
--rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/recipes/vasp/slabs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/runners/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11347 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/runners/thermo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.222923 quacc-0.7.6/src/quacc/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/schemas/_aliases/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/emmet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/_aliases/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/ase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    18073 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/cclib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2752 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/phonons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/prep.py
--rw-r--r--   0 runner    (1001) docker     (127)    12882 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/schemas/vasp.py
--rw-r--r--   0 runner    (1001) docker     (127)    16783 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5091 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/dicts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/kpts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/utils/lists.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc/wflow_tools/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/customizers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-20 17:23:17.000000 quacc-0.7.6/src/quacc/wflow_tools/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-20 17:25:13.226923 quacc-0.7.6/src/quacc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-20 17:25:13.000000 quacc-0.7.6/src/quacc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.560052 quacc-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-23 21:36:44.000000 quacc-0.7.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 21:36:44.000000 quacc-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-23 21:38:43.560052 quacc-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-23 21:36:44.000000 quacc-0.7.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5973 2024-04-23 21:36:44.000000 quacc-0.7.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:38:43.560052 quacc-0.7.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.524052 quacc-0.7.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.528052 quacc-0.7.7/src/quacc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.528052 quacc-0.7.7/src/quacc/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/_cli/quacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/atoms/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7246 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/deformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/atoms/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17619 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/espresso.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.532052 quacc-0.7.7/src/quacc/calculators/espresso/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_metal_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_metal_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/esm_semiconductors_slab_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/metal_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/metal_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/molecule_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/semiconductors_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/semiconductors_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17071 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/espresso/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12373 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/qchem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/qchem/qchem_custodian.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/params.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/calculators/vasp/presets/
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/BulkSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/QMOFSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/SlabSet.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_base.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_pbe54.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_qmof.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12127 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7751 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/calculators/vasp/vasp_custodian.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.536052 quacc-0.7.7/src/quacc/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/common/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/dftb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/dftb/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/emt/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/defects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/elastic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/emt/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/espresso/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8331 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13160 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/bands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15322 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10393 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/dos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24396 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/espresso/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.540052 quacc-0.7.7/src/quacc/recipes/gaussian/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3973 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gaussian/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/gulp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3632 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/gulp/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/lj/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/lj/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/lj/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/mlp/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2905 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/mlp/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/newtonnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/newtonnet/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/onetep/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/onetep/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/orca/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6236 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12436 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/orca/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.544052 quacc-0.7.7/src/quacc/recipes/psi4/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/psi4/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/qchem/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5618 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10013 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/qchem/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/tblite/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4816 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3588 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/tblite/phonons.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/recipes/vasp/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9432 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14585 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/mp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8922 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/qmof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6768 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/recipes/vasp/slabs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.548052 quacc-0.7.7/src/quacc/runners/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11353 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4646 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/runners/thermo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/schemas/_aliases/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/emmet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/_aliases/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13456 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/ase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17451 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/cclib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/phonons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5485 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/prep.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/schemas/vasp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16656 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/dicts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9240 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/kpts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/utils/lists.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc/wflow_tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/customizers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-04-23 21:36:44.000000 quacc-0.7.7/src/quacc/wflow_tools/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:38:43.552052 quacc-0.7.7/src/quacc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6536 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-23 21:38:43.000000 quacc-0.7.7/src/quacc.egg-info/top_level.txt
```

### Comparing `quacc-0.7.6/LICENSE.md` & `quacc-0.7.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/PKG-INFO` & `quacc-0.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.6
+Version: 0.7.7
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
```

### Comparing `quacc-0.7.6/README.md` & `quacc-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/pyproject.toml` & `quacc-0.7.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "quacc"
 description="A platform to enable high-throughput, database-driven quantum chemistry and computational materials science"
-version = "0.7.6"
+version = "0.7.7"
 readme = "README.md"
 license = { text = "BSD-3" }
 authors = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 maintainers = [{ name = "Andrew S. Rosen", email = "asrosen@princeton.edu" }]
 keywords = ["high-throughput", "automated", "workflow", "dft"]
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -168,16 +168,21 @@
   "PT012",  # pytest.raises
   "RET505", # Unnecessary `elif` after `return`
 ]
 src = ["src"]
 lint.pydocstyle.convention = "numpy"
 lint.isort.known-first-party = ["quacc"]
 lint.isort.required-imports = ["from __future__ import annotations"]
+lint.isort.split-on-trailing-comma=false
 extend-include = ["*.ipynb"]
 
+[tool.ruff.format]
+docstring-code-format = true
+skip-magic-trailing-comma = true
+
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/**" = ["ANN", "ARG", "D", "E402", "PTH", "S101"]
 "src/quacc/settings.py" = ["FBT003", "TCH002", "UP007"]
 
 [tool.docformatter]
 pre-summary-newline = true
```

### Comparing `quacc-0.7.6/src/quacc/__init__.py` & `quacc-0.7.7/src/quacc/__init__.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/_cli/quacc.py` & `quacc-0.7.7/src/quacc/_cli/quacc.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/atoms/core.py` & `quacc-0.7.7/src/quacc/atoms/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from ase.filters import Filter
 from ase.io.jsonio import encode
 from pymatgen.io.ase import AseAtomsAdaptor
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
     from ase.optimize.optimize import Dynamics
+    from numpy.typing import NDArray
 
 logger = logging.getLogger(__name__)
 
 
 def get_atoms_id(atoms: Atoms) -> str:
     """
     Returns a unique ID for the Atoms object. Note: The .info dict and calculator is
@@ -250,7 +251,38 @@
     -------
     Atoms
         Atoms object
     """
     return (
         dynamics.atoms.atoms if isinstance(dynamics.atoms, Filter) else dynamics.atoms
     )
+
+
+def perturb(mol: Atoms, matrix: list[list[float]] | NDArray, scale: float) -> Atoms:
+    """
+    Perturb each atom in a molecule by a (scaled) 1x3 vector, reflecting e.g. a vibrational normal mode.
+
+    Parameters
+    ----------
+    mol
+        ASE Atoms object representing a molecule
+    matrix
+        Nx3 matrix, where N is the numebr of atoms. This means that there is potentially a different translation
+        vector for each atom in the molecule.
+    scale
+        Scaling factor for perturbation
+
+    Returns
+    -------
+    Atoms
+        The input molecule after perturbation
+    """
+
+    mol_copy = copy_atoms(mol)
+    mode = np.asarray(matrix)
+
+    orig_pos = mol_copy.get_positions()
+
+    pos = orig_pos + mode * scale
+    mol_copy.set_positions(pos)
+
+    return mol_copy
```

### Comparing `quacc-0.7.6/src/quacc/atoms/defects.py` & `quacc-0.7.7/src/quacc/atoms/defects.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
             min_atoms=min_atoms,
             max_atoms=max_atoms,
             min_length=min_length,
             force_diagonal=force_diagonal,
         )
 
         # Generate DefectEntry object from Defect object
-        defect_entry = _get_defect_entry_from_defect(
+        defect_entry = get_defect_entry_from_defect(
             defect=defect,
             defect_supercell=defect_supercell,
             defect_charge=defect_charge,
         )
 
         # Instantiate class to apply rattle and bond distortion to all defects
         dist = Distortions([defect_entry])
@@ -132,15 +132,15 @@
                 "defect": defect,
             }
             final_defect.info["defect_stats"] = defect_stats
             final_defects.append(final_defect)
     return final_defects
 
 
-def _get_defect_entry_from_defect(
+def get_defect_entry_from_defect(
     defect: Defect, defect_supercell: Structure, defect_charge: int
 ) -> DefectEntry:
     """
     Function to generate DefectEntry object from Defect object.
 
     Parameters
     ----------
```

### Comparing `quacc-0.7.6/src/quacc/atoms/deformation.py` & `quacc-0.7.7/src/quacc/atoms/deformation.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/atoms/phonons.py` & `quacc-0.7.7/src/quacc/atoms/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/atoms/slabs.py` & `quacc-0.7.7/src/quacc/atoms/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/espresso/espresso.py` & `quacc-0.7.7/src/quacc/calculators/espresso/espresso.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,18 +137,18 @@
                 atoms,
                 format="espresso-in",
                 pseudo_dir=str(profile.pseudo_dir),
                 properties=properties,
                 **parameters,
             )
         elif self.binary in ["ph", "phcg"]:
-            with Path.open(directory / self.inputname, "w") as fd:
+            with Path(directory, self.inputname).open(mode="w") as fd:
                 write_espresso_ph(fd=fd, properties=properties, **parameters)
         else:
-            with Path.open(directory / self.inputname, "w") as fd:
+            with Path(directory, self.inputname).open(mode="w") as fd:
                 write_fortran_namelist(
                     fd,
                     binary=self.binary if self._ase_known_binary else None,
                     properties=properties,
                     **parameters,
                 )
 
@@ -218,24 +218,24 @@
             The results dictionnary
         """
         results = {}
         if self.binary == "pw":
             atoms = read(directory / self.outputname, format="espresso-out")
             results = dict(atoms.calc.properties())
         elif self.binary in ["ph", "phcg"]:
-            with Path.open(directory / self.outputname, "r") as fd:
+            with Path(directory, self.outputname).open() as fd:
                 results = read_espresso_ph(fd)
         elif self.binary == "dos":
-            with Path.open(directory / "pwscf.dos", "r") as fd:
+            with Path(directory, "pwscf.dos").open() as fd:
                 lines = fd.readlines()
                 fermi = float(re.search(r"-?\d+\.?\d*", lines[0])[0])
                 dos = np.loadtxt(lines[1:])
             results = {"dos_results": {"dos": dos, "fermi": fermi}}
         elif self.binary == "projwfc":
-            with Path.open(directory / "pwscf.pdos_tot", "r") as fd:
+            with Path(directory, "pwscf.pdos_tot").open() as fd:
                 lines = np.loadtxt(fd.readlines())
                 energy = lines[1:, 0]
                 dos = lines[1:, 1]
                 pdos = lines[1:, 2]
             results = {"projwfc_results": {"energy": energy, "dos": dos, "pdos": pdos}}
         elif self.binary == "matdyn":
             fldos = Path(directory, "matdyn.dos")
```

### Comparing `quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml` & `quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml` & `quacc-0.7.7/src/quacc/calculators/espresso/presets/sssp_1.3.0_pbe_precision.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml` & `quacc-0.7.7/src/quacc/calculators/espresso/presets/tough_metal_clusters_efficiency.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/espresso/utils.py` & `quacc-0.7.7/src/quacc/calculators/espresso/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,18 +280,15 @@
         if lqdir:
             to_copy.extend(
                 [Path("_ph*", "pwscf.q_*", "pwscf.save", "data-file-schema.*")]
             )
 
             if recover:
                 to_copy.extend(
-                    [
-                        Path("_ph*", "pwscf.q_*", "pwscf.save", "charge-density.*"),
-                        # Path("_ph*", "pwscf.q_*", "pwscf.wfc*.gz"),
-                    ]
+                    [Path("_ph*", "pwscf.q_*", "pwscf.save", "charge-density.*")]
                 )
 
         if recover:
             to_copy.append(Path("_ph*", "pwscf.phsave"))
 
         if ldvscf_interpolate:
             to_copy.extend((Path("_ph*", "pwscf.dvscf*"), Path("w_pot")))
```

### Comparing `quacc-0.7.6/src/quacc/calculators/qchem/io.py` & `quacc-0.7.7/src/quacc/calculators/qchem/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/qchem/params.py` & `quacc-0.7.7/src/quacc/calculators/qchem/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/qchem/qchem.py` & `quacc-0.7.7/src/quacc/calculators/qchem/qchem.py`

 * *Files 0% similar despite different names*

```diff
@@ -258,17 +258,15 @@
         None
         """
         FileIOCalculator.write_input(self, atoms, properties, system_changes)
 
         qc_input = make_qc_input(self, atoms)
 
         write_qchem(
-            qc_input,
-            self.directory,
-            prev_orbital_coeffs=self.prev_orbital_coeffs,
+            qc_input, self.directory, prev_orbital_coeffs=self.prev_orbital_coeffs
         )
 
     def execute(self) -> int:
         """
         Execute Q-Chem.
 
         Returns
```

### Comparing `quacc-0.7.6/src/quacc/calculators/qchem/qchem_custodian.py` & `quacc-0.7.7/src/quacc/calculators/qchem/qchem_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/io.py` & `quacc-0.7.7/src/quacc/calculators/vasp/io.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/params.py` & `quacc-0.7.7/src/quacc/calculators/vasp/params.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml` & `quacc-0.7.7/src/quacc/calculators/vasp/presets/magmoms_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_pbe54.yaml` & `quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_pbe54.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/presets/setups_qmof.yaml` & `quacc-0.7.7/src/quacc/calculators/vasp/presets/setups_qmof.yaml`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/vasp.py` & `quacc-0.7.7/src/quacc/calculators/vasp/vasp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/calculators/vasp/vasp_custodian.py` & `quacc-0.7.7/src/quacc/calculators/vasp/vasp_custodian.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/common/defects.py` & `quacc-0.7.7/src/quacc/recipes/common/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/common/elastic.py` & `quacc-0.7.7/src/quacc/recipes/common/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/common/phonons.py` & `quacc-0.7.7/src/quacc/recipes/common/phonons.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
-from quacc import flow, job, subflow
+from quacc import job, subflow
 from quacc.atoms.phonons import get_phonopy, phonopy_atoms_to_ase_atoms
 from quacc.runners.phonons import run_phonopy
 from quacc.schemas.phonons import summarize_phonopy
 
 has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
 
 if TYPE_CHECKING:
@@ -19,19 +19,19 @@
 
     from ase.atoms import Atoms
 
     from quacc import Job
     from quacc.schemas._aliases.phonons import PhononSchema
 
 
-@flow
+@subflow
 @requires(
     has_deps, "Phonopy and seekpath must be installed. Run `pip install quacc[phonons]`"
 )
-def phonon_flow(
+def phonon_subflow(
     atoms: Atoms,
     force_job: Job,
     relax_job: Job | None = None,
     symprec: float = 1e-4,
     min_lengths: float | tuple[float, float, float] | None = 20.0,
     supercell_matrix: (
         tuple[tuple[int, int, int], tuple[int, int, int], tuple[int, int, int]] | None
@@ -76,27 +76,28 @@
 
     Returns
     -------
     PhononSchema
         Dictionary of results from [quacc.schemas.phonons.summarize_phonopy][]
     """
 
+    phonon = get_phonopy(
+        atoms,
+        min_lengths=min_lengths,
+        supercell_matrix=supercell_matrix,
+        symprec=symprec,
+        displacement=displacement,
+        phonopy_kwargs=phonopy_kwargs,
+    )
+    supercells = [
+        phonopy_atoms_to_ase_atoms(s) for s in phonon.supercells_with_displacements
+    ]
+
     @subflow
-    def _get_forces_subflow(atoms: Atoms) -> list[dict]:
-        phonon = get_phonopy(
-            atoms,
-            min_lengths=min_lengths,
-            supercell_matrix=supercell_matrix,
-            symprec=symprec,
-            displacement=displacement,
-            phonopy_kwargs=phonopy_kwargs,
-        )
-        supercells = [
-            phonopy_atoms_to_ase_atoms(s) for s in phonon.supercells_with_displacements
-        ]
+    def _get_forces_subflow(supercells: list[Atoms]) -> list[dict]:
         return [
             force_job(supercell) for supercell in supercells if supercell is not None
         ]
 
     @job
     def _thermo_job(atoms: Atoms, force_job_results: list[dict]) -> PhononSchema:
         phonon = get_phonopy(
@@ -105,22 +106,24 @@
             supercell_matrix=supercell_matrix,
             symprec=symprec,
             displacement=displacement,
             phonopy_kwargs=phonopy_kwargs,
         )
         parameters = force_job_results[-1].get("parameters")
         forces = [output["results"]["forces"] for output in force_job_results]
-        phonon = run_phonopy(phonon, forces, t_step=t_step, t_min=t_min, t_max=t_max)
+        phonon_results = run_phonopy(
+            phonon, forces, t_step=t_step, t_min=t_min, t_max=t_max
+        )
 
         return summarize_phonopy(
             phonon,
             atoms,
-            phonon.directory,
+            phonon_results.directory,
             parameters=parameters,
             additional_fields=additional_fields,
         )
 
     if relax_job is not None:
         atoms = relax_job(atoms)["atoms"]
 
-    force_job_results = _get_forces_subflow(atoms)
+    force_job_results = _get_forces_subflow(supercells)
     return _thermo_job(atoms, force_job_results)
```

### Comparing `quacc-0.7.6/src/quacc/recipes/common/slabs.py` & `quacc-0.7.7/src/quacc/recipes/common/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/dftb/_base.py` & `quacc-0.7.7/src/quacc/recipes/dftb/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/dftb/core.py` & `quacc-0.7.7/src/quacc/recipes/dftb/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/emt/core.py` & `quacc-0.7.7/src/quacc/recipes/emt/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/emt/defects.py` & `quacc-0.7.7/src/quacc/recipes/emt/defects.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/emt/elastic.py` & `quacc-0.7.7/src/quacc/recipes/emt/elastic.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/emt/phonons.py` & `quacc-0.7.7/src/quacc/recipes/emt/phonons.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Phonon recipes for EMT."""
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from quacc import flow
-from quacc.recipes.common.phonons import phonon_flow as common_phonon_flow
+from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.emt.core import relax_job, static_job
 from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 if TYPE_CHECKING:
     from typing import Any, Callable
 
@@ -89,15 +89,15 @@
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
-    return common_phonon_flow(
+    return phonon_subflow(
         atoms,
         static_job_,
         relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
```

### Comparing `quacc-0.7.6/src/quacc/recipes/emt/slabs.py` & `quacc-0.7.7/src/quacc/recipes/emt/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/espresso/_base.py` & `quacc-0.7.7/src/quacc/recipes/espresso/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,25 +72,25 @@
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][]
     """
-    atoms = _prepare_atoms(
+    atoms = prepare_atoms(
         atoms=atoms,
         preset=preset,
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
-    updated_copy_files = _prepare_copy(
+    updated_copy_files = prepare_copy(
         copy_files=copy_files,
         calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
 
     geom_file = template.outputname if template.binary == "pw" else None
 
@@ -100,15 +100,14 @@
         final_atoms, atoms, move_magmoms=True, additional_fields=additional_fields
     )
 
 
 def run_and_summarize_opt(
     atoms: Atoms | None = None,
     preset: str | None = None,
-    relax_cell: bool = False,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
     opt_params: dict[str, Any] | None = None,
     parallel_info: dict[str, Any] | None = None,
@@ -125,16 +124,14 @@
 
     Parameters
     ----------
     atoms
         Atoms object
     preset
         Name of the preset to use
-    relax_cell
-        Whether to relax the cell or not.
     template
         EspressoTemplate to use
     profile
         EspressoProfile to use
     calc_defaults
         The default calculator parameters.
     calc_swaps
@@ -155,42 +152,40 @@
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
     RunSchema
         Dictionary of results from [quacc.schemas.ase.summarize_run][]
     """
-    atoms = _prepare_atoms(
+    atoms = prepare_atoms(
         atoms=atoms,
         preset=preset,
         template=template,
         profile=profile,
         calc_defaults=calc_defaults,
         calc_swaps=calc_swaps,
         parallel_info=parallel_info,
     )
 
-    updated_copy_files = _prepare_copy(
+    updated_copy_files = prepare_copy(
         copy_files=copy_files,
         calc_params=atoms.calc.user_calc_params,
         binary=atoms.calc.template.binary,
     )
 
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
-    dyn = run_opt(
-        atoms, relax_cell=relax_cell, copy_files=updated_copy_files, **opt_flags
-    )
+    dyn = run_opt(atoms, copy_files=updated_copy_files, **opt_flags)
 
     return summarize_opt_run(
         dyn, move_magmoms=True, additional_fields=additional_fields
     )
 
 
-def _prepare_atoms(
+def prepare_atoms(
     atoms: Atoms | None = None,
     preset: str | None = None,
     template: EspressoTemplate | None = None,
     profile: EspressoProfile | None = None,
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     parallel_info: dict[str, Any] | None = None,
@@ -248,15 +243,15 @@
         profile=profile,
         **calc_flags,
     )
 
     return atoms
 
 
-def _prepare_copy(
+def prepare_copy(
     copy_files: (
         SourceDirectory
         | list[SourceDirectory]
         | dict[SourceDirectory, Filenames]
         | None
     ) = None,
     calc_params: dict[str, Any] | None = None,
```

### Comparing `quacc-0.7.6/src/quacc/recipes/espresso/bands.py` & `quacc-0.7.7/src/quacc/recipes/espresso/bands.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/espresso/core.py` & `quacc-0.7.7/src/quacc/recipes/espresso/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,20 +248,19 @@
     calc_defaults = BASE_SET_METAL if is_metal else BASE_SET_NON_METAL
     calc_defaults["input_data"]["control"] = {
         "calculation": "scf",
         "tstress": relax_cell,
         "tprnfor": True,
     }
 
-    opt_defaults = {"optimizer": BFGSLineSearch}
+    opt_defaults = {"optimizer": BFGSLineSearch, "relax_cell": relax_cell}
 
     return run_and_summarize_opt(
         atoms,
         preset=preset,
-        relax_cell=relax_cell,
         template=EspressoTemplate("pw", autorestart=autorestart, outdir=prev_outdir),
         calc_defaults=calc_defaults,
         calc_swaps=calc_kwargs,
         opt_defaults=opt_defaults,
         opt_params=opt_params,
         parallel_info=parallel_info,
         additional_fields={"name": "pw.x ExternalRelax"},
```

### Comparing `quacc-0.7.6/src/quacc/recipes/espresso/dos.py` & `quacc-0.7.7/src/quacc/recipes/espresso/dos.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/espresso/phonons.py` & `quacc-0.7.7/src/quacc/recipes/espresso/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/gaussian/_base.py` & `quacc-0.7.7/src/quacc/recipes/gaussian/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/gaussian/core.py` & `quacc-0.7.7/src/quacc/recipes/gaussian/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/gulp/_base.py` & `quacc-0.7.7/src/quacc/recipes/gulp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/gulp/core.py` & `quacc-0.7.7/src/quacc/recipes/gulp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/lj/core.py` & `quacc-0.7.7/src/quacc/recipes/lj/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/mlp/_base.py` & `quacc-0.7.7/src/quacc/recipes/mlp/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/mlp/core.py` & `quacc-0.7.7/src/quacc/recipes/mlp/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/mlp/phonons.py` & `quacc-0.7.7/src/quacc/recipes/mlp/phonons.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import flow
-from quacc.recipes.common.phonons import phonon_flow as common_phonon_flow
+from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.mlp.core import relax_job, static_job
 from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 has_deps = find_spec("phonopy") is not None and find_spec("seekpath") is not None
 
 if TYPE_CHECKING:
@@ -102,15 +102,15 @@
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
-    return common_phonon_flow(
+    return phonon_subflow(
         atoms,
         static_job_,
         relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
```

### Comparing `quacc-0.7.6/src/quacc/recipes/newtonnet/core.py` & `quacc-0.7.7/src/quacc/recipes/newtonnet/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/newtonnet/ts.py` & `quacc-0.7.7/src/quacc/recipes/newtonnet/ts.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/onetep/_base.py` & `quacc-0.7.7/src/quacc/recipes/onetep/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,13 +125,10 @@
         The Onetep calculator.
     """
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
 
     return Onetep(
         pseudo_path=str(SETTINGS.ONETEP_PP_PATH) if SETTINGS.ONETEP_PP_PATH else ".",
         parallel_info=SETTINGS.ONETEP_PARALLEL_CMD,
-        profile=OnetepProfile(
-            SETTINGS.ONETEP_CMD
-        ),  # TODO: If the ASE merge is successful, we need to change ONETEP_PARALLEL_CMD to a list[str] and remove parallel info.
-        # If we also have access to post_args we can point not to the binary but to the launcher which takes -t nthreads as a post_args
+        profile=OnetepProfile(SETTINGS.ONETEP_CMD),
         **calc_flags,
     )
```

### Comparing `quacc-0.7.6/src/quacc/recipes/onetep/core.py` & `quacc-0.7.7/src/quacc/recipes/onetep/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/orca/_base.py` & `quacc-0.7.7/src/quacc/recipes/orca/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/psi4/_base.py` & `quacc-0.7.7/src/quacc/recipes/psi4/_base.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/psi4/core.py` & `quacc-0.7.7/src/quacc/recipes/psi4/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/qchem/_base.py` & `quacc-0.7.7/src/quacc/recipes/qchem/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,17 +105,14 @@
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
     OptSchema
         Dictionary of results from [quacc.schemas.ase.summarize_opt_run][]
     """
-    # TODO:
-    #   - passing initial Hessian?
-
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
     atoms.calc = QChem(
         atoms, charge=charge, spin_multiplicity=spin_multiplicity, **calc_flags
     )
     dyn = run_opt(atoms, copy_files=copy_files, **opt_flags)
```

### Comparing `quacc-0.7.6/src/quacc/recipes/qchem/core.py` & `quacc-0.7.7/src/quacc/recipes/qchem/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/qchem/ts.py` & `quacc-0.7.7/src/quacc/recipes/qchem/ts.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,39 +3,43 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import SETTINGS, job, strip_decorator
+from quacc.atoms.core import perturb
 from quacc.recipes.qchem._base import run_and_summarize_opt
 from quacc.recipes.qchem.core import _BASE_SET, relax_job
 from quacc.utils.dicts import recursive_dict_merge
 
 try:
     from sella import IRC, Sella
 
+    has_sella = True
+
 except ImportError:
-    Sella = False
+    has_sella = False
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.atoms import Atoms
+    from numpy.typing import NDArray
 
     from quacc.schemas._aliases.ase import OptSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def ts_job(
     atoms: Atoms,
-    charge: int,
-    spin_multiplicity: int,
+    charge: int = 0,
+    spin_multiplicity: int = 1,
     method: str = "wb97mv",
     basis: str = "def2-svpd",
     opt_params: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
     """
@@ -88,19 +92,19 @@
         opt_params=opt_params,
         additional_fields={"name": "Q-Chem TS"},
         copy_files=copy_files,
     )
 
 
 @job
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def irc_job(
     atoms: Atoms,
-    charge: int,
-    spin_multiplicity: int,
+    charge: int = 0,
+    spin_multiplicity: int = 1,
     direction: Literal["forward", "reverse"] = "forward",
     method: str = "wb97mv",
     basis: str = "def2-svpd",
     opt_params: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
 ) -> OptSchema:
@@ -158,19 +162,19 @@
         opt_params=opt_params,
         additional_fields={"name": "Q-Chem IRC"},
         copy_files=copy_files,
     )
 
 
 @job
-@requires(Sella, "Sella must be installed. Refer to the quacc documentation.")
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
 def quasi_irc_job(
     atoms: Atoms,
-    charge: int,
-    spin_multiplicity: int,
+    charge: int = 0,
+    spin_multiplicity: int = 1,
     direction: Literal["forward", "reverse"] = "forward",
     method: str = "wb97mv",
     basis: str = "def2-svpd",
     irc_job_kwargs: dict[str, Any] | None = None,
     relax_job_kwargs: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
 ) -> OptSchema:
@@ -225,7 +229,85 @@
 
     SETTINGS.CHECK_CONVERGENCE = default_settings.CHECK_CONVERGENCE
     relax_summary = strip_decorator(relax_job)(irc_summary["atoms"], **relax_job_kwargs)
 
     relax_summary["initial_irc"] = irc_summary
 
     return relax_summary
+
+
+@job
+@requires(has_sella, "Sella must be installed. Refer to the quacc documentation.")
+def quasi_irc_perturb_job(
+    atoms: Atoms,
+    mode: list[list[float]] | NDArray,
+    charge: int = 0,
+    spin_multiplicity: int = 1,
+    perturb_magnitude: float = 0.6,
+    direction: Literal["forward", "reverse"] = "forward",
+    method: str = "wb97mv",
+    basis: str = "def2-svpd",
+    opt_params: dict[str, Any] | None = None,
+    copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
+    **calc_kwargs,
+) -> OptSchema:
+    """
+    Quasi-IRC to optimize a reaction endpoint from a transition-state with known vibrational frequency modes.
+    Perturbs the structure of `atoms` by a finite amount (0.6 * the normalized mode magnitude) along the specified
+    vibrational frequency mode (assumed to be the transition mode), and then performs a `relax_job` on the perturbed
+    structure.
+
+    Parameters
+    ----------
+    atoms
+        Atoms object.
+    mode
+        Transition mode. This should be an Nx3 matrix, where N is the number of atoms in `atoms`.
+    charge
+        Charge of the system.
+    spin_multiplicity
+        Multiplicity of the system.
+    perturb_magnitude
+        Factor to multiply the transition mode. Default is 0.6. In some cases, it may be advisable to increase this
+        factor, perhaps to 1.0 or 1.1. Lowering it is not generally found to be helpful.
+    direction
+        Direction of the (Quasi)IRC. Should be "forward" or "reverse".
+    method
+        DFT exchange-correlation functional or other electronic structure
+        method.
+    basis
+        Basis set.
+    opt_params
+        Dictionary of custom kwargs for the optimization process. For a list
+        of available keys, refer to [quacc.runners.ase.run_opt][].
+    copy_files
+        Files to copy (and decompress) from source to the runtime directory.
+    **calc_kwargs
+        Custom kwargs for the calculator. Set a value to `quacc.Remove` to remove
+        a pre-existing key entirely. See [quacc.calculators.qchem.qchem.QChem][] for more
+        details.
+
+
+    Returns
+    -------
+    OptSchema
+        Dictionary of results from [quacc.schemas.ase.summarize_opt_run][]
+    """
+
+    calc_defaults = recursive_dict_merge(
+        _BASE_SET, {"rem": {"job_type": "force", "method": method, "basis": basis}}
+    )
+    opt_defaults = {"optimizer": Sella} if has_sella else {}
+
+    scale = perturb_magnitude if direction == "forward" else perturb_magnitude * -1
+
+    return run_and_summarize_opt(
+        perturb(atoms, mode, scale),
+        charge=charge,
+        spin_multiplicity=spin_multiplicity,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        opt_defaults=opt_defaults,
+        opt_params=opt_params,
+        additional_fields={"name": "Q-Chem Quasi-IRC perturbed optimization"},
+        copy_files=copy_files,
+    )
```

### Comparing `quacc-0.7.6/src/quacc/recipes/tblite/core.py` & `quacc-0.7.7/src/quacc/recipes/tblite/core.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/tblite/phonons.py` & `quacc-0.7.7/src/quacc/recipes/tblite/phonons.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from importlib.util import find_spec
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import flow
-from quacc.recipes.common.phonons import phonon_flow as common_phonon_flow
+from quacc.recipes.common.phonons import phonon_subflow
 from quacc.recipes.tblite.core import relax_job, static_job
 from quacc.utils.dicts import recursive_dict_merge
 from quacc.wflow_tools.customizers import customize_funcs
 
 has_deps_tblite = find_spec("tblite") is not None
 has_deps_phonons = (
     find_spec("phonopy") is not None and find_spec("seekpath") is not None
@@ -102,15 +102,15 @@
     relax_job_, static_job_ = customize_funcs(
         ["relax_job", "static_job"],
         [relax_job, static_job],
         parameters=job_params,
         decorators=job_decorators,
     )
 
-    return common_phonon_flow(
+    return phonon_subflow(
         atoms,
         static_job_,
         relax_job=relax_job_ if run_relax else None,
         symprec=symprec,
         min_lengths=min_lengths,
         supercell_matrix=supercell_matrix,
         displacement=displacement,
```

### Comparing `quacc-0.7.6/src/quacc/recipes/vasp/_base.py` & `quacc-0.7.7/src/quacc/recipes/vasp/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from quacc.utils.dicts import recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
-    from quacc.schemas._aliases.vasp import VaspASESchema, VaspSchema
+    from quacc.schemas._aliases.vasp import VaspASEOptSchema, VaspSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 def run_and_summarize(
     atoms: Atoms,
     preset: str | None = None,
     calc_defaults: dict[str, Any] | None = None,
@@ -72,15 +72,15 @@
     calc_defaults: dict[str, Any] | None = None,
     calc_swaps: dict[str, Any] | None = None,
     opt_defaults: dict[str, Any] | None = None,
     opt_params: dict[str, Any] | None = None,
     report_mp_corrections: bool = False,
     additional_fields: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
-) -> VaspASESchema:
+) -> VaspASEOptSchema:
     """
     Base job function for VASP recipes with ASE optimizers.
 
     Parameters
     ----------
     atoms
         Atoms object
@@ -101,15 +101,15 @@
     additional_fields
         Additional fields to supply to the summarizer.
     copy_files
         Files to copy (and decompress) from source to the runtime directory.
 
     Returns
     -------
-    VaspASESchema
+    VaspASEOptSchema
         Dictionary of results
     """
     calc_flags = recursive_dict_merge(calc_defaults, calc_swaps)
     opt_flags = recursive_dict_merge(opt_defaults, opt_params)
 
     atoms.calc = Vasp(atoms, preset=preset, **calc_flags)
     dyn = run_opt(atoms, copy_files=copy_files, **opt_flags)
```

### Comparing `quacc-0.7.6/src/quacc/recipes/vasp/core.py` & `quacc-0.7.7/src/quacc/recipes/vasp/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from quacc.recipes.vasp._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
-    from quacc.schemas._aliases.vasp import DoubleRelaxSchema, VaspASESchema, VaspSchema
+    from quacc.schemas._aliases.vasp import VaspASEOptSchema, VaspSchema
     from quacc.utils.files import Filenames, SourceDirectory
 
 
 @job
 def static_job(
     atoms: Atoms,
     preset: str | None = "BulkSet",
@@ -125,15 +125,15 @@
 @flow
 def double_relax_flow(
     atoms: Atoms,
     preset: str | None = "BulkSet",
     relax_cell: bool = True,
     relax1_kwargs: dict[str, Any] | None = None,
     relax2_kwargs: dict[str, Any] | None = None,
-) -> DoubleRelaxSchema:
+) -> dict[Literal["relax1"], VaspSchema, Literal["relax2"], VaspSchema]:
     """
     Double-relax a structure. This is particularly useful for a few reasons:
 
     1. To carry out a cheaper pre-relaxation before the high-quality run.
 
     2. To carry out a GGA calculation before a meta-GGA or hybrid calculation
     that requires the GGA wavefunction.
@@ -153,16 +153,16 @@
     relax1_kwargs
         Dictionary of custom kwargs for the first relaxation.
     relax2_kwargs
         Dictionary of custom kwargs for the second relaxation.
 
     Returns
     -------
-    DoubleRelaxSchema
-        Dictionary of results. See the type-hint for the data structure.
+    dict[Literal["relax1"], VaspSchema, Literal["relax2"], VaspSchema]
+        Dictionary of results from each step.
     """
     relax1_kwargs = relax1_kwargs or {}
     relax2_kwargs = relax2_kwargs or {}
 
     # Run first relaxation
     summary1 = relax_job(atoms, preset=preset, relax_cell=relax_cell, **relax1_kwargs)
 
@@ -182,15 +182,15 @@
 def ase_relax_job(
     atoms: Atoms,
     preset: str | None = "BulkSet",
     relax_cell: bool = True,
     opt_params: dict[str, Any] | None = None,
     copy_files: SourceDirectory | dict[SourceDirectory, Filenames] | None = None,
     **calc_kwargs,
-) -> VaspASESchema:
+) -> VaspASEOptSchema:
     """
     Relax a structure.
 
     Parameters
     ----------
     atoms
         Atoms object
@@ -207,15 +207,15 @@
     **calc_kwargs
         Custom kwargs for the Vasp calculator. Set a value to
         `None` to remove a pre-existing key entirely. For a list of available
         keys, refer to the [quacc.calculators.vasp.vasp.Vasp][] calculator.
 
     Returns
     -------
-    VaspASESchema
+    VaspASEOptSchema
         Dictionary of results. See the type-hint for the data structure.
     """
     calc_defaults = {"lcharg": False, "lwave": False, "nsw": 0}
     opt_defaults = {"relax_cell": relax_cell}
     return run_and_summarize_opt(
         atoms,
         preset=preset,
```

### Comparing `quacc-0.7.6/src/quacc/recipes/vasp/mp.py` & `quacc-0.7.7/src/quacc/recipes/vasp/mp.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/recipes/vasp/qmof.py` & `quacc-0.7.7/src/quacc/recipes/vasp/qmof.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,15 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 from ase.optimize import BFGSLineSearch
 
 from quacc import job
-from quacc.calculators.vasp import Vasp
-from quacc.recipes.vasp._base import run_and_summarize
-from quacc.runners.ase import run_opt
-from quacc.schemas.ase import summarize_opt_run
-from quacc.utils.dicts import recursive_dict_merge
+from quacc.recipes.vasp._base import run_and_summarize, run_and_summarize_opt
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.ase import OptSchema
     from quacc.schemas._aliases.vasp import QMOFRelaxSchema, VaspSchema
 
@@ -130,19 +126,22 @@
         "encut": None,
         "lcharg": False,
         "lreal": "auto",
         "lwave": True,
         "nelm": 225,
         "nsw": 0,
     }
-    calc_flags = recursive_dict_merge(calc_defaults, calc_kwargs)
-    atoms.calc = Vasp(atoms, preset=preset, **calc_flags)
-    dyn = run_opt(atoms, fmax=fmax, optimizer=BFGSLineSearch)
-
-    return summarize_opt_run(dyn, additional_fields={"name": "QMOF Prerelax"})
+    return run_and_summarize_opt(
+        atoms,
+        preset=preset,
+        calc_defaults=calc_defaults,
+        calc_swaps=calc_kwargs,
+        opt_defaults={"fmax": fmax, "optimizer": BFGSLineSearch},
+        additional_fields={"name": "QMOF Prerelax"},
+    )
 
 
 def _loose_relax_positions(
     atoms: Atoms, preset: str | None = "QMOFSet", **calc_kwargs
 ) -> VaspSchema:
     """
     Position relaxation with default ENCUT and coarse k-point grid.
```

### Comparing `quacc-0.7.6/src/quacc/recipes/vasp/slabs.py` & `quacc-0.7.7/src/quacc/recipes/vasp/slabs.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/runners/ase.py` & `quacc-0.7.7/src/quacc/runners/ase.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,15 +195,15 @@
     # Check if trajectory kwarg is specified
     if "trajectory" in optimizer_kwargs:
         msg = "Quacc does not support setting the `trajectory` kwarg."
         raise ValueError(msg)
 
     # Handle optimizer kwargs
     if optimizer.__name__.startswith("SciPy"):
-        optimizer_kwargs.pop("restart")
+        optimizer_kwargs.pop("restart", None)
     elif optimizer.__name__ == "Sella":
         _set_sella_kwargs(atoms, optimizer_kwargs)
     elif optimizer.__name__ == "IRC":
         optimizer_kwargs.pop("restart", None)
 
     # Define the Trajectory object
     traj_file = tmpdir / "opt.traj"
```

### Comparing `quacc-0.7.6/src/quacc/runners/phonons.py` & `quacc-0.7.7/src/quacc/runners/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/runners/prep.py` & `quacc-0.7.7/src/quacc/runners/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/runners/thermo.py` & `quacc-0.7.7/src/quacc/runners/thermo.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
 from ase import units
 from ase.thermochemistry import IdealGasThermo
-
-from quacc.schemas.atoms import atoms_to_metadata
+from emmet.core.symmetry import PointGroupData
+from pymatgen.io.ase import AseAtomsAdaptor
 
 if TYPE_CHECKING:
     from ase.atoms import Atoms
 
 
 def run_ideal_gas(
     atoms: Atoms,
@@ -40,17 +40,14 @@
         The spin multiplicity (2S+1). If None, this will be determined
         automatically from the attached magnetic moments.
 
     Returns
     -------
     IdealGasThermo object
     """
-    # Switch off PBC since this is only for molecules
-    atoms.set_pbc(False)
-
     # Ensure all negative modes are made complex
     for i, f in enumerate(vib_freqs):
         if not isinstance(f, complex) and f < 0:
             vib_freqs[i] = complex(0 - f * 1j)
 
     # Convert vibrational frequencies to energies
     vib_energies = [f * units.invcm for f in vib_freqs]
@@ -73,26 +70,27 @@
     elif atoms.has("initial_magmoms"):
         spin = round(np.sum(atoms.get_initial_magnetic_moments())) / 2
     else:
         spin = 0
 
     # Get symmetry for later use
     natoms = len(atoms)
-    metadata = atoms_to_metadata(atoms)
+    mol = AseAtomsAdaptor().get_molecule(atoms, charge_spin_check=False)
+    point_group_data = PointGroupData().from_molecule(mol)
 
     # Get the geometry
     if natoms == 1:
         geometry = "monatomic"
-    elif metadata["symmetry"]["linear"]:
+    elif point_group_data.linear:
         geometry = "linear"
     else:
         geometry = "nonlinear"
 
     return IdealGasThermo(
         vib_energies,
         geometry,
         potentialenergy=energy,
         atoms=atoms,
-        symmetrynumber=metadata["symmetry"]["rotation_number"],
+        symmetrynumber=point_group_data.rotation_number,
         spin=spin,
         ignore_imag_modes=True,
     )
```

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/ase.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/ase.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/atoms.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/atoms.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/cclib.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/cclib.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/emmet.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/emmet.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/phonons.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/phonons.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/_aliases/vasp.py` & `quacc-0.7.7/src/quacc/schemas/_aliases/vasp.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,9 +71,9 @@
 
     prerelax_lowacc: VaspSchema | None
     position_relax_lowacc: VaspSchema
     volume_relax_lowacc: VaspSchema | None
     double_relax: VaspSchema
 
 
-class VaspASESchema(VaspSchema, OptSchema):
+class VaspASEOptSchema(VaspSchema, OptSchema):
     """Type hint associated with VASP relaxations run via ASE"""
```

### Comparing `quacc-0.7.6/src/quacc/schemas/ase.py` & `quacc-0.7.7/src/quacc/schemas/ase.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 """Schemas for storing ASE-based data."""
 
 from __future__ import annotations
 
-import gzip
-import pickle
-from pathlib import Path
 from typing import TYPE_CHECKING
 
 import numpy as np
 from ase import units
 from ase.io import read
 from ase.vibrations import Vibrations
 from ase.vibrations.data import VibrationsData
 
 from quacc import SETTINGS, __version__
 from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.atoms import atoms_to_metadata
 from quacc.schemas.prep import prep_next_run
-from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
+from quacc.utils.dicts import finalize_dict, recursive_dict_merge
 from quacc.utils.files import get_uri
-from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
     from ase.io import Trajectory
     from ase.optimize.optimize import Optimizer
@@ -83,57 +79,47 @@
         raise ValueError(msg)
     if not final_atoms.calc.results:
         msg = "ASE Atoms object's calculator has no results."
         raise ValueError(msg)
 
     directory = final_atoms.calc.directory
     uri = get_uri(directory)
-    input_atoms_metadata = (
-        atoms_to_metadata(
+
+    if input_atoms:
+        input_atoms_metadata = atoms_to_metadata(
             input_atoms,
             charge_and_multiplicity=charge_and_multiplicity,
             store_pmg=False,
         )
-        if input_atoms
-        else None
-    )
+    else:
+        input_atoms_metadata = {}
+
     inputs = {
         "parameters": final_atoms.calc.parameters,
         "nid": uri.split(":")[0],
         "dir_name": directory,
         "input_atoms": input_atoms_metadata,
         "quacc_version": __version__,
     }
-
     results = {"results": final_atoms.calc.results}
 
     atoms_to_store = prep_next_run(final_atoms, move_magmoms=move_magmoms)
 
     if final_atoms:
         final_atoms_metadata = atoms_to_metadata(
             atoms_to_store, charge_and_multiplicity=charge_and_multiplicity
         )
     else:
         final_atoms_metadata = {}
 
     unsorted_task_doc = final_atoms_metadata | inputs | results | additional_fields
-    task_doc = clean_task_doc(unsorted_task_doc)
 
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def summarize_opt_run(
     dyn: Optimizer,
     trajectory: Trajectory | list[Atoms] | None = None,
     check_convergence: bool = _DEFAULT_SETTING,
     charge_and_multiplicity: tuple[int, int] | None = None,
@@ -218,28 +204,18 @@
         "nsteps": dyn.get_number_of_steps(),
         "trajectory": trajectory,
         "trajectory_results": [atoms.calc.results for atoms in trajectory],
     }
 
     # Create a dictionary of the inputs/outputs
     unsorted_task_doc = base_task_doc | opt_fields | additional_fields
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
 
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def summarize_vib_and_thermo(
     vib: Vibrations,
     igt: IdealGasThermo,
     temperature: float = 298.15,
     pressure: float = 1.0,
@@ -273,76 +249,56 @@
     -------
     VibThermoSchema
         A dictionary that merges the `VibSchema` and `ThermoSchema`.
     """
     store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
 
     vib_task_doc = _summarize_vib_run(
-        vib,
-        charge_and_multiplicity=charge_and_multiplicity,
-        store=None,
-        additional_fields=additional_fields,
+        vib, charge_and_multiplicity=charge_and_multiplicity
     )
     thermo_task_doc = _summarize_ideal_gas_thermo(
         igt,
         temperature=temperature,
         pressure=pressure,
         charge_and_multiplicity=charge_and_multiplicity,
-        store=None,
-        additional_fields=additional_fields,
     )
 
-    unsorted_task_doc = recursive_dict_merge(vib_task_doc, thermo_task_doc)
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if isinstance(vib, Vibrations):
-        directory = vib.atoms.calc.directory
-        if SETTINGS.WRITE_PICKLE:
-            with (
-                gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-                if SETTINGS.GZIP_FILES
-                else Path(directory, "quacc_results.pkl").open("wb")
-            ) as f:
-                pickle.dump(task_doc, f)
-    if store:
-        results_to_db(store, task_doc)
+    unsorted_task_doc = recursive_dict_merge(
+        vib_task_doc, thermo_task_doc, additional_fields
+    )
 
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc,
+        vib.atoms.calc.directory if isinstance(vib, Vibrations) else None,
+        gzip_file=SETTINGS.GZIP_FILES,
+        store=store,
+    )
 
 
 def _summarize_vib_run(
     vib: Vibrations | VibrationsData,
     charge_and_multiplicity: tuple[int, int] | None = None,
-    additional_fields: dict[str, Any] | None = None,
-    store: Store | None = None,
 ) -> VibSchema:
     """
     Get tabulated results from an ASE Vibrations object and store them in a database-
     friendly format.
 
     Parameters
     ----------
     vib
         ASE Vibrations object.
     charge_and_multiplicity
         Charge and spin multiplicity of the Atoms object, only used for Molecule
         metadata.
-    additional_fields
-        Additional fields to add to the task document.
-    store
-        Maggma Store object to store the results in. Defaults to `SETTINGS.STORE`.
 
     Returns
     -------
     VibSchema
         Dictionary representation of the task document
     """
-    additional_fields = additional_fields or {}
-    store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
-
     vib_freqs_raw = vib.get_frequencies().tolist()
     vib_energies_raw = vib.get_energies().tolist()
 
     # Convert imaginary modes to negative values for DB storage
     for i, f in enumerate(vib_freqs_raw):
         if np.imag(f) > 0:
             vib_freqs_raw[i] = -np.abs(f)
@@ -407,30 +363,22 @@
             "vib_energies": vib_energies,
             "vib_freqs": vib_freqs,
             "vib_energies_raw": vib_energies_raw,
             "vib_freqs_raw": vib_freqs_raw,
         }
     }
 
-    unsorted_task_doc = atoms_metadata | inputs | results | additional_fields
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return atoms_metadata | inputs | results
 
 
 def _summarize_ideal_gas_thermo(
     igt: IdealGasThermo,
     temperature: float = 298.15,
     pressure: float = 1.0,
     charge_and_multiplicity: tuple[int, int] | None = None,
-    additional_fields: dict[str, Any] | None = None,
-    store: Store | None = _DEFAULT_SETTING,
 ) -> ThermoSchema:
     """
     Get tabulated results from an ASE IdealGasThermo object and store them in a
     database-friendly format.
 
     Parameters
     ----------
@@ -441,25 +389,20 @@
     pressure
         Pressure in bar.
     charge_and_multiplicity
         Charge and spin multiplicity of the Atoms object, only used for Molecule
         metadata.
     additional_fields
         Additional fields to add to the task document.
-    store
-        Maggma Store object to store the results in. Defaults to `SETTINGS.STORE`
 
     Returns
     -------
     ThermoSchema
         Dictionary representation of the task document
     """
-    additional_fields = additional_fields or {}
-    store = SETTINGS.STORE if store == _DEFAULT_SETTING else store
-
     spin_multiplicity = round(2 * igt.spin + 1)
 
     inputs = {
         "parameters_thermo": {
             "temperature": temperature,
             "pressure": pressure,
             "sigma": igt.sigma,
@@ -490,14 +433,8 @@
         )
         raise ValueError(msg)
 
     atoms_metadata = atoms_to_metadata(
         igt.atoms, charge_and_multiplicity=charge_and_multiplicity
     )
 
-    unsorted_task_doc = atoms_metadata | inputs | results | additional_fields
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return atoms_metadata | inputs | results
```

### Comparing `quacc-0.7.6/src/quacc/schemas/atoms.py` & `quacc-0.7.7/src/quacc/schemas/atoms.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from pymatgen.io.ase import AseAtomsAdaptor
 
 from quacc.atoms.core import (
     copy_atoms,
     get_charge_attribute,
     get_spin_multiplicity_attribute,
 )
-from quacc.utils.dicts import clean_task_doc
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
 
     from quacc.schemas._aliases.atoms import AtomsSchema
@@ -80,18 +79,15 @@
                 results["molecule"] = mol
     else:
         metadata = {}
 
     # Store Atoms object
     results["atoms"] = atoms
 
-    # Combine the metadata and results dictionaries
-    atoms_doc_unsorted = metadata | results | additional_fields
-
-    return clean_task_doc(atoms_doc_unsorted)
+    return metadata | results | additional_fields
 
 
 def _set_charge_and_spin(
     atoms: Atoms, charge_and_multiplicity: tuple[int, int] | None = None
 ) -> None:
     """
     Set the charge and spin multiplicity of an Atoms object.
```

### Comparing `quacc-0.7.6/src/quacc/schemas/cclib.py` & `quacc-0.7.7/src/quacc/schemas/cclib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,26 @@
 """Schemas for molecular DFT codes parsed by cclib."""
 
 from __future__ import annotations
 
-import gzip
 import logging
 import os
-import pickle
 from inspect import getmembers, isclass
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 import cclib
 from ase.atoms import Atoms
 from cclib.io import ccread
 
 from quacc import SETTINGS
 from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.ase import summarize_opt_run, summarize_run
-from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
+from quacc.utils.dicts import finalize_dict, recursive_dict_merge
 from quacc.utils.files import find_recent_logfile
-from quacc.wflow_tools.db import results_to_db
 
 if TYPE_CHECKING:
     from typing import Any, Literal
 
     from ase.io import Trajectory
     from ase.optimize.optimize import Optimizer
     from maggma.core import Store
@@ -31,15 +28,15 @@
     from quacc.schemas._aliases.cclib import (
         PopAnalysisAttributes,
         cclibASEOptSchema,
         cclibBaseSchema,
         cclibSchema,
     )
 
-logger = logging.getLogger(__name__)
+LOGGER = logging.getLogger(__name__)
 
 _DEFAULT_SETTING = ()
 
 
 def cclib_summarize_run(
     final_atoms: Atoms,
     logfile_extensions: str | list[str],
@@ -150,29 +147,17 @@
         store=None,
     )
 
     # Create a dictionary of the inputs/outputs
     unsorted_task_doc = (
         run_task_doc | intermediate_cclib_task_docs | cclib_task_doc | additional_fields
     )
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    # Store the results
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def summarize_cclib_opt_run(
     optimizer: Optimizer,
     logfile_extensions: str | list[str],
     trajectory: Trajectory | list[Atoms] | None = None,
     directory: Path | str | None = None,
@@ -253,29 +238,18 @@
         charge_and_multiplicity=(
             cclib_summary["charge"],
             cclib_summary["spin_multiplicity"],
         ),
         additional_fields=additional_fields,
         store=None,
     )
-    task_doc = recursive_dict_merge(cclib_summary, opt_run_summary)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    # Store the results
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    unsorted_task_doc = recursive_dict_merge(cclib_summary, opt_run_summary)
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def _make_cclib_schema(
     directory: str | Path,
     logfile_extensions: str | list[str],
     analysis: str | list[str] | None = None,
     proatom_dir: Path | str | None = None,
@@ -459,15 +433,15 @@
             m = method_class(cclib_obj, vol)
     else:
         m = method_class(cclib_obj)
 
     try:
         m.calculate()
     except Exception as e:
-        logger.warning(f"Could not calculate {method}: {e}")
+        LOGGER.warning(f"Could not calculate {method}: {e}")
         return None
 
     # The list of available attributes after a calculation. This is hardcoded
     # for now until https://github.com/cclib/cclib/issues/1097 is resolved. Once
     # it is, we can delete this and just do `return
     # calc_attributes.getattributes()`.
     avail_attributes = [
```

### Comparing `quacc-0.7.6/src/quacc/schemas/phonons.py` & `quacc-0.7.7/src/quacc/schemas/phonons.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Summarizer for phonopy."""
 
 from __future__ import annotations
 
-import gzip
-import pickle
-from pathlib import Path
 from typing import TYPE_CHECKING
 
 from monty.dev import requires
 
 from quacc import SETTINGS, __version__
 from quacc.schemas.atoms import atoms_to_metadata
-from quacc.utils.dicts import clean_task_doc
+from quacc.utils.dicts import finalize_dict
 from quacc.utils.files import get_uri
-from quacc.wflow_tools.db import results_to_db
 
 try:
     import phonopy
 except ImportError:
     phonopy = None
 
 if TYPE_CHECKING:
+    from pathlib import Path
     from typing import Any
 
     from ase.atoms import Atoms
     from maggma.core import Store
 
     from quacc.schemas._aliases.phonons import PhononSchema
 
@@ -87,21 +84,10 @@
             "total_dos": phonon.get_total_dos_dict(),
             "force_constants": phonon.force_constants,
         }
     }
 
     atoms_metadata = atoms_to_metadata(input_atoms)
     unsorted_task_doc = atoms_metadata | inputs | results | additional_fields
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
```

### Comparing `quacc-0.7.6/src/quacc/schemas/prep.py` & `quacc-0.7.7/src/quacc/schemas/prep.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/schemas/vasp.py` & `quacc-0.7.7/src/quacc/schemas/vasp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 """Schemas for VASP."""
 
 from __future__ import annotations
 
-import gzip
 import logging
 import os
-import pickle
 from pathlib import Path
 from typing import TYPE_CHECKING
 
 from ase.io import read
 from emmet.core.tasks import TaskDoc
 from monty.os.path import zpath
 from pymatgen.command_line.bader_caller import bader_analysis_from_path
@@ -18,29 +16,28 @@
     CompatibilityError,
     MaterialsProject2020Compatibility,
 )
 
 from quacc import SETTINGS
 from quacc.atoms.core import get_final_atoms_from_dynamics
 from quacc.schemas.ase import summarize_opt_run, summarize_run
-from quacc.utils.dicts import clean_task_doc, recursive_dict_merge
-from quacc.wflow_tools.db import results_to_db
+from quacc.utils.dicts import finalize_dict, recursive_dict_merge
 
 if TYPE_CHECKING:
     from typing import Any
 
     from ase.atoms import Atoms
     from ase.io import Trajectory
     from ase.optimize.optimize import Optimizer
     from maggma.core import Store
 
     from quacc.schemas._aliases.vasp import (
         BaderSchema,
         ChargemolSchema,
-        VaspASESchema,
+        VaspASEOptSchema,
         VaspSchema,
     )
 
 logger = logging.getLogger(__name__)
 
 _DEFAULT_SETTING = ()
 
@@ -165,43 +162,31 @@
         if chargemol_results:
             vasp_task_doc["chargemol"] = chargemol_results
 
     # Make task document
     unsorted_task_doc = (
         intermediate_vasp_task_docs | vasp_task_doc | base_task_doc | additional_fields
     )
-    task_doc = clean_task_doc(unsorted_task_doc)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    # Store the results
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def summarize_vasp_opt_run(
     optimizer: Optimizer,
     trajectory: Trajectory | list[Atoms] | None = None,
     directory: str | Path | None = None,
     move_magmoms: bool = True,
     run_bader: bool = _DEFAULT_SETTING,
     run_chargemol: bool = _DEFAULT_SETTING,
     check_convergence: bool = _DEFAULT_SETTING,
     report_mp_corrections: bool = False,
     additional_fields: dict[str, Any] | None = None,
     store: Store | None = _DEFAULT_SETTING,
-) -> VaspASESchema:
+) -> VaspASEOptSchema:
     """
     Merges the `vasp_summarize_run` with an `summarize_opt_run`, meant to
     be used for an ASE-based VASP relaxation.
 
     Parameters
     ----------
     optimizer
@@ -251,29 +236,18 @@
         run_bader=run_bader,
         run_chargemol=run_chargemol,
         check_convergence=check_convergence,
         report_mp_corrections=report_mp_corrections,
         additional_fields=additional_fields,
         store=None,
     )
-    task_doc = recursive_dict_merge(vasp_summary, opt_run_summary)
-
-    if SETTINGS.WRITE_PICKLE:
-        with (
-            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
-            if SETTINGS.GZIP_FILES
-            else Path(directory, "quacc_results.pkl").open("wb")
-        ) as f:
-            pickle.dump(task_doc, f)
-
-    # Store the results
-    if store:
-        results_to_db(store, task_doc)
-
-    return task_doc
+    unsorted_task_doc = recursive_dict_merge(vasp_summary, opt_run_summary)
+    return finalize_dict(
+        unsorted_task_doc, directory, gzip_file=SETTINGS.GZIP_FILES, store=store
+    )
 
 
 def _bader_runner(path: Path | str) -> BaderSchema:
     """
     Runs a Bader partial charge and spin moment analysis using the VASP output
     files in the given path. This function requires that `bader` is located in
     your PATH environment variable. See
```

### Comparing `quacc-0.7.6/src/quacc/settings.py` & `quacc-0.7.7/src/quacc/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,17 +103,14 @@
             in which case you should set this to False.
             """
         ),
     )
     GZIP_FILES: bool = Field(
         True, description="Whether generated files should be gzip'd."
     )
-    WRITE_PICKLE: bool = Field(
-        True, description="Whether the results schema should be written to a .pkl file."
-    )
     CHECK_CONVERGENCE: bool = Field(
         True,
         description="Whether to check for convergence, when implemented by a given recipe.",
     )
 
     # ---------------------------
     # Data Store Settings
```

### Comparing `quacc-0.7.6/src/quacc/utils/dicts.py` & `quacc-0.7.7/src/quacc/utils/dicts.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 """Utility functions for dealing with dictionaries."""
 
 from __future__ import annotations
 
+import gzip
 import logging
+import pickle
 from collections.abc import MutableMapping
 from copy import deepcopy
+from pathlib import Path
 from typing import TYPE_CHECKING
 
+from quacc.wflow_tools.db import results_to_db
+
 if TYPE_CHECKING:
     from typing import Any
 
+    from maggma.stores import Store
+
 LOGGER = logging.getLogger(__name__)
 
 
 class Remove:
     """
     A sentinel class used in quacc to mark a key in a dictionary for removal.
 
@@ -174,15 +181,15 @@
     """
     return {
         k: sort_dict(v) if isinstance(v, MutableMapping) else v
         for k, v in sorted(start_dict.items())
     }
 
 
-def clean_task_doc(start_dict: dict[str, Any]) -> dict[str, Any]:
+def clean_dict(start_dict: dict[str, Any]) -> dict[str, Any]:
     """
     Clean up a task document dictionary by removing all entries that are None and
     sorting the dictionary alphabetically by key.
 
     Parameters
     ----------
     start_dict
@@ -190,7 +197,51 @@
 
     Returns
     -------
     dict
         Cleaned dictionary
     """
     return sort_dict(remove_dict_entries(start_dict, None))
+
+
+def finalize_dict(
+    task_doc: dict,
+    directory: str | Path | None,
+    gzip_file: bool = True,
+    store: Store | None = None,
+) -> dict:
+    """
+    Finalize a schema by cleaning it and storing it in a database and/or file.
+
+    Parameters
+    ----------
+    task_doc
+        Dictionary representation of the task document.
+    directory
+        Directory where the results file is stored.
+    gzip_file
+        Whether to gzip the results file.
+    store
+        Maggma Store object to store the results in.
+
+    Returns
+    -------
+    dict
+        Cleaned task document
+    """
+
+    cleaned_task_doc = clean_dict(task_doc)
+
+    if directory:
+        if "tmp-quacc" in str(directory):
+            raise ValueError("The directory should not be a temporary directory.")
+        with (
+            gzip.open(Path(directory, "quacc_results.pkl.gz"), "wb")
+            if gzip_file
+            else Path(directory, "quacc_results.pkl").open("wb")
+        ) as f:
+            pickle.dump(task_doc, f)
+
+    if store:
+        results_to_db(store, task_doc)
+
+    return cleaned_task_doc
```

### Comparing `quacc-0.7.6/src/quacc/utils/files.py` & `quacc-0.7.7/src/quacc/utils/files.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/utils/kpts.py` & `quacc-0.7.7/src/quacc/utils/kpts.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         The generated k-points.
     gamma
         Whether the k-points are gamma-centered.
     """
     struct = AseAtomsAdaptor.get_structure(input_atoms)
 
     if pmg_kpts.get("line_density"):
-        # TODO: Support methods other than latimer-munro
         kpath = HighSymmKpath(
             struct,
             path_type="latimer_munro",
             has_magmoms=np.any(struct.site_properties.get("magmom", None)),
         )
         kpts, _ = kpath.get_kpoints(
             line_density=pmg_kpts["line_density"], coords_are_cartesian=True
```

### Comparing `quacc-0.7.6/src/quacc/utils/lists.py` & `quacc-0.7.7/src/quacc/utils/lists.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/wflow_tools/customizers.py` & `quacc-0.7.7/src/quacc/wflow_tools/customizers.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/wflow_tools/db.py` & `quacc-0.7.7/src/quacc/wflow_tools/db.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc/wflow_tools/decorators.py` & `quacc-0.7.7/src/quacc/wflow_tools/decorators.py`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc.egg-info/PKG-INFO` & `quacc-0.7.7/src/quacc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quacc
-Version: 0.7.6
+Version: 0.7.7
 Summary: A platform to enable high-throughput, database-driven quantum chemistry and computational materials science
 Author-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 Maintainer-email: "Andrew S. Rosen" <asrosen@princeton.edu>
 License: BSD-3
 Project-URL: repository, https://github.com/Quantum-Accelerators/quacc
 Project-URL: documentation, https://quantum-accelerators.github.io/quacc/
 Project-URL: changelog, https://github.com/Quantum-Accelerators/quacc/blob/main/CHANGELOG.md
```

### Comparing `quacc-0.7.6/src/quacc.egg-info/SOURCES.txt` & `quacc-0.7.7/src/quacc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quacc-0.7.6/src/quacc.egg-info/requires.txt` & `quacc-0.7.7/src/quacc.egg-info/requires.txt`

 * *Files identical despite different names*

