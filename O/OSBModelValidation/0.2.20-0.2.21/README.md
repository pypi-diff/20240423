# Comparing `tmp/osbmodelvalidation-0.2.20.tar.gz` & `tmp/osbmodelvalidation-0.2.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osbmodelvalidation-0.2.20.tar", last modified: Mon Apr 15 17:29:57 2024, max compression
+gzip compressed data, was "osbmodelvalidation-0.2.21.tar", last modified: Tue Apr 23 19:12:13 2024, max compression
```

## Comparing `osbmodelvalidation-0.2.20.tar` & `osbmodelvalidation-0.2.21.tar`

### file list

```diff
@@ -1,141 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.103317 osbmodelvalidation-0.2.20/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/LICENSE.lesser
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.103317 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-15 17:29:57.000000 osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10856 2024-04-15 17:29:57.103317 osbmodelvalidation-0.2.20/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.083317 osbmodelvalidation-0.2.20/omv/
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.087317 osbmodelvalidation-0.2.20/omv/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/activation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/dryrun.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/input_resistance.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/morphology.py
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/resting.py
--rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/spikes.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/temperature.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.087317 osbmodelvalidation-0.2.20/omv/analyzers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/utils/filenode.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/analyzers/utils/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/autogen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.087317 osbmodelvalidation-0.2.20/omv/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3877 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/common/inout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.095317 osbmodelvalidation-0.2.20/omv/engines/
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/arbor_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/brian1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/brian2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/eden_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/genesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getarbor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getbrian1.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/geteden.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getgenesis.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getjlems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getjnml.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getlibsbml.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getmoose.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getnetpyne.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getneuroconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getnml2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getoctave.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getpylems.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getpyneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/getpynn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jlems.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlbrian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromleden.py
--rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlmoose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne_np2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne_np4.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2734 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlpynnnrn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2016 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlvalidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/jneuromlvalidatev1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/moose_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/nestsli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/netpyne_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/netpyne__np2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/netpyne__np4.py
--rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/neuron_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/octave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pylems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pylemsnml2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pyneuroconstruct.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pyneuroml_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pyneuromlvalidatesbml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pyneuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynnbrian1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynnbrian2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynnnest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynnneuroml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/pynnneuron.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/engines/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/utils/genesis_utils.g
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/engines/utils/wdir.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/find_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/omt_mep_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    14890 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/omv_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/parse_omt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/schemata/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/mep.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/schemata/types/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/schemata/types/base/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/observable_datafile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/observable_literal.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/observables.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/schemata/types/base/test/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/test/observable_datafile.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/test/observable_literal.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/base/test/observable_literal.3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/expected.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/experiment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/observable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/protocol.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/protocol_properties.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/schemata/types/test/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/expected.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/expected.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/expected.3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/expected.4.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/experiment.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/experiment.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/observable.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/protocol.1.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/schemata/types/test/protocol.2.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/tally.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.099317 osbmodelvalidation-0.2.20/omv/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/test/test_rates.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/test/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:57.103317 osbmodelvalidation-0.2.20/omv/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/validation/rx_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/validation/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/validation/validate.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/omv/validation/validate_mep.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-15 17:29:53.000000 osbmodelvalidation-0.2.20/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-15 17:29:57.103317 osbmodelvalidation-0.2.20/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/LICENSE.lesser
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-23 19:12:13.000000 osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10907 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9783 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.303167 osbmodelvalidation-0.2.21/omv/
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.307167 osbmodelvalidation-0.2.21/omv/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/activation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2583 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/dryrun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/input_resistance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/morphology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/resting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4373 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/spikes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/temperature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.307167 osbmodelvalidation-0.2.21/omv/analyzers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/utils/filenode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/analyzers/utils/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/autogen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.307167 osbmodelvalidation-0.2.21/omv/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3915 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/common/inout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.315167 osbmodelvalidation-0.2.21/omv/engines/
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/arbor_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/brian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/brian2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/eden_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getarbor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getbrian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/geteden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getgenesis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getjlems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getjnml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getlibsbml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getmoose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getnetpyne.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getneuroconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getnml2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getoctave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getpylems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getpyneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getpynn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/getxpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jlems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2382 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlbrian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromleden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2337 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlmoose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne_np2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne_np4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlpynnnrn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2019 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlvalidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlvalidatev1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2020 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/jneuromlxpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/moose_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/nestsli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/netpyne_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/netpyne__np2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/netpyne__np4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7775 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/neuron_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1558 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/octave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pylems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pylemsnml2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3990 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pyneuroconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pyneuroml_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pyneuromlvalidatesbml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pyneuromlxpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3263 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pyneuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynnbrian1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynnbrian2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynnnest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynnneuroml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/pynnneuron.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.315167 osbmodelvalidation-0.2.21/omv/engines/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/utils/genesis_utils.g
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/utils/wdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/engines/xpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3873 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/find_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/omt_mep_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15188 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/omv_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/parse_omt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.315167 osbmodelvalidation-0.2.21/omv/schemata/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/mep.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.315167 osbmodelvalidation-0.2.21/omv/schemata/types/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/omv/schemata/types/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/observable_datafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/observable_literal.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/observables.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/omv/schemata/types/base/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/test/observable_datafile.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/test/observable_literal.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/base/test/observable_literal.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/expected.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/experiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/observable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/protocol.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/protocol_properties.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/omv/schemata/types/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/expected.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/expected.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/expected.3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/expected.4.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/experiment.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/experiment.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/observable.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/protocol.1.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/schemata/types/test/protocol.2.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3536 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/tally.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/omv/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/test/test_rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/test/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:13.319167 osbmodelvalidation-0.2.21/omv/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/validation/rx_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/validation/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/validation/validate.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      380 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/omv/validation/validate_mep.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 19:12:09.000000 osbmodelvalidation-0.2.21/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-23 19:12:13.323167 osbmodelvalidation-0.2.21/setup.cfg
```

### Comparing `osbmodelvalidation-0.2.20/LICENSE.lesser` & `osbmodelvalidation-0.2.21/LICENSE.lesser`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/PKG-INFO` & `osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: OSBModelValidation
-Version: 0.2.20
+Version: 0.2.21
 Summary: Open Source Brain Model validation
 Home-page: https://github.com/OpenSourceBrain/osb-model-validation
 Author: Boris Marin, Padraig Gleeson
 Author-email: borismarin@gmail.com
 License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.lesser
 Requires-Dist: PyYAML
 Requires-Dist: numpy
 Requires-Dist: pyrx
 Requires-Dist: pathlib; python_version < "3.4"
```

### Comparing `osbmodelvalidation-0.2.20/OSBModelValidation.egg-info/SOURCES.txt` & `osbmodelvalidation-0.2.21/OSBModelValidation.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -54,47 +54,51 @@
 omv/engines/getneuroconstruct.py
 omv/engines/getnml2.py
 omv/engines/getnrn.py
 omv/engines/getoctave.py
 omv/engines/getpylems.py
 omv/engines/getpyneuroml.py
 omv/engines/getpynn.py
+omv/engines/getxpp.py
 omv/engines/jlems.py
 omv/engines/jneuroml.py
 omv/engines/jneuromlbrian.py
 omv/engines/jneuromlbrian2.py
 omv/engines/jneuromleden.py
 omv/engines/jneuromlmoose.py
 omv/engines/jneuromlnetpyne.py
 omv/engines/jneuromlnetpyne_np2.py
 omv/engines/jneuromlnetpyne_np4.py
 omv/engines/jneuromlnrn.py
 omv/engines/jneuromlpynnnrn.py
 omv/engines/jneuromlvalidate.py
 omv/engines/jneuromlvalidatev1.py
+omv/engines/jneuromlxpp.py
 omv/engines/moose_.py
 omv/engines/nestsli.py
 omv/engines/netpyne_.py
 omv/engines/netpyne__np2.py
 omv/engines/netpyne__np4.py
 omv/engines/neuron_.py
 omv/engines/octave.py
 omv/engines/pylems.py
 omv/engines/pylemsnml2.py
 omv/engines/pynest.py
 omv/engines/pyneuroconstruct.py
 omv/engines/pyneuroml_.py
 omv/engines/pyneuromlvalidatesbml.py
+omv/engines/pyneuromlxpp.py
 omv/engines/pyneuron.py
 omv/engines/pynn.py
 omv/engines/pynnbrian1.py
 omv/engines/pynnbrian2.py
 omv/engines/pynnnest.py
 omv/engines/pynnneuroml.py
 omv/engines/pynnneuron.py
+omv/engines/xpp.py
 omv/engines/utils/__init__.py
 omv/engines/utils/genesis_utils.g
 omv/engines/utils/wdir.py
 omv/schemata/mep.yaml
 omv/schemata/types/expected.yaml
 omv/schemata/types/experiment.yaml
 omv/schemata/types/observable.yaml
```

### Comparing `osbmodelvalidation-0.2.20/PKG-INFO` & `osbmodelvalidation-0.2.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: OSBModelValidation
-Version: 0.2.20
+Version: 0.2.21
 Summary: Open Source Brain Model validation
 Home-page: https://github.com/OpenSourceBrain/osb-model-validation
 Author: Boris Marin, Padraig Gleeson
 Author-email: borismarin@gmail.com
 License: LGPL-3.0-only
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Description-Content-Type: text/markdown
 License-File: LICENSE.lesser
 Requires-Dist: PyYAML
 Requires-Dist: numpy
 Requires-Dist: pyrx
 Requires-Dist: pathlib; python_version < "3.4"
```

### Comparing `osbmodelvalidation-0.2.20/README.md` & `osbmodelvalidation-0.2.21/README.md`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/__init__.py` & `osbmodelvalidation-0.2.21/omv/analyzers/__init__.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/activation.py` & `osbmodelvalidation-0.2.21/omv/analyzers/activation.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/analyzer.py` & `osbmodelvalidation-0.2.21/omv/analyzers/analyzer.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/input_resistance.py` & `osbmodelvalidation-0.2.21/omv/analyzers/input_resistance.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/morphology.py` & `osbmodelvalidation-0.2.21/omv/analyzers/morphology.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/rates.py` & `osbmodelvalidation-0.2.21/omv/analyzers/rates.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/resting.py` & `osbmodelvalidation-0.2.21/omv/analyzers/resting.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/spikes.py` & `osbmodelvalidation-0.2.21/omv/analyzers/spikes.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/timeseries.py` & `osbmodelvalidation-0.2.21/omv/analyzers/timeseries.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/utils/filenode.py` & `osbmodelvalidation-0.2.21/omv/analyzers/utils/filenode.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/analyzers/utils/timeseries.py` & `osbmodelvalidation-0.2.21/omv/analyzers/utils/timeseries.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/autogen.py` & `osbmodelvalidation-0.2.21/omv/autogen.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/common/inout.py` & `osbmodelvalidation-0.2.21/omv/common/inout.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         )
         if isinstance(ret_string, bytes):
             ret_string = ret_string.decode("utf-8")  # For Python 3...
         return ret_string
 
     except sp.CalledProcessError as err:
         inform(
-            "Error running commands: %s in %s (return code: %s)"
-            % (cmds, cwd, err.returncode),
+            "CalledProcessError running commands: %s in %s (return code: %s), output:\n%s"
+            % (cmds, cwd, err.returncode, err.output),
             indent=2,
             verbosity=verbosity,
         )
         inform("Error: %s" % (err), indent=2, verbosity=verbosity)
         raise err
     except Exception as err:
         inform(
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/__init__.py` & `osbmodelvalidation-0.2.21/omv/engines/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,27 @@
 from omv.engines.jneuromlnetpyne import JNeuroMLNetPyNEEngine
 from omv.engines.jneuromlnetpyne_np4 import JNeuroMLNetPyNENP4Engine
 from omv.engines.jneuromlnetpyne_np2 import JNeuroMLNetPyNENP2Engine
 
 # from omv.engines.jneuromlbrian import JNeuroMLBrianEngine
 from omv.engines.jneuromleden import JNeuroMLEdenEngine
 from omv.engines.jneuromlbrian2 import JNeuroMLBrian2Engine
+from omv.engines.jneuromlxpp import JNeuroMLXppEngine
 from omv.engines.jneuromlmoose import JNeuroMLMooseEngine
 from omv.engines.jneuromlvalidate import JNeuroMLValidateEngine
 from omv.engines.jneuromlvalidatev1 import JNeuroMLValidateV1Engine
 from omv.engines.jlems import JLemsEngine
 from omv.engines.pylems import PyLemsEngine
 from omv.engines.pylemsnml2 import PyLemsNeuroML2Engine
 from omv.engines.genesis import GenesisEngine
 
 # from omv.engines.brian1 import Brian1Engine
 from omv.engines.brian2_ import Brian2Engine
 from omv.engines.arbor_ import ArborEngine
+from omv.engines.xpp import XppEngine
 from omv.engines.eden_ import EdenEngine
 from omv.engines.nestsli import NestEngine
 from omv.engines.pynest import PyNestEngine
 from omv.engines.moose_ import MooseEngine
 from omv.engines.pynn import PyNNEngine
 from omv.engines.pynnneuron import PyNNNRNEngine
 from omv.engines.pyneuron import PyNRNEngine
@@ -38,14 +40,15 @@
 from omv.engines.octave import OctaveEngine
 from omv.engines.netpyne_ import NetPyNEEngine
 from omv.engines.netpyne__np4 import NetPyNENP4Engine
 from omv.engines.netpyne__np2 import NetPyNENP2Engine
 from omv.engines.pyneuroconstruct import PyneuroConstructEngine
 from omv.engines.pyneuroml_ import PyNeuroMLEngine
 from omv.engines.pyneuromlvalidatesbml import PyNeuroMLValidateSBMLEngine
+from omv.engines.pyneuromlxpp import PyNeuroMLXppEngine
 
 
 OMVEngines = {
     be.name: be
     for be in locals().values()
     if inspect.isclass(be)
     and issubclass(be, OMVEngine)
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/arbor_.py` & `osbmodelvalidation-0.2.21/omv/engines/arbor_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/brian1.py` & `osbmodelvalidation-0.2.21/omv/engines/brian1.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/brian2_.py` & `osbmodelvalidation-0.2.21/omv/engines/brian2_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/eden_.py` & `osbmodelvalidation-0.2.21/omv/engines/eden_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/engine.py` & `osbmodelvalidation-0.2.21/omv/engines/engine.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/genesis.py` & `osbmodelvalidation-0.2.21/omv/engines/genesis.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getbrian1.py` & `osbmodelvalidation-0.2.21/omv/engines/getbrian1.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getgenesis.py` & `osbmodelvalidation-0.2.21/omv/engines/getgenesis.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getjlems.py` & `osbmodelvalidation-0.2.21/omv/engines/getjlems.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getjnml.py` & `osbmodelvalidation-0.2.21/omv/engines/getjnml.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getnest.py` & `osbmodelvalidation-0.2.21/omv/engines/getnest.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getnetpyne.py` & `osbmodelvalidation-0.2.21/omv/engines/getnetpyne.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getneuroconstruct.py` & `osbmodelvalidation-0.2.21/omv/engines/getneuroconstruct.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getnml2.py` & `osbmodelvalidation-0.2.21/omv/engines/getnml2.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getnrn.py` & `osbmodelvalidation-0.2.21/omv/engines/getnrn.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/getpynn.py` & `osbmodelvalidation-0.2.21/omv/engines/getpynn.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jlems.py` & `osbmodelvalidation-0.2.21/omv/engines/jlems.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuroml.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuroml.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlbrian.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlbrian.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         return JNeuroMLEngine.is_installed() and Brian1Engine.is_installed()
 
     @staticmethod
     def install(version):
         if not JNeuroMLEngine.is_installed():
             JNeuroMLEngine.install(None)
         if not Brian1Engine.is_installed():
-            Brian1Engine.install(None)
+            Brian1Engine.install(version)
 
         JNeuroMLBrianEngine.path = JNeuroMLEngine.path + ":" + Brian1Engine.path
         JNeuroMLBrianEngine.environment_vars = {}
         JNeuroMLBrianEngine.environment_vars.update(JNeuroMLEngine.environment_vars)
         JNeuroMLBrianEngine.environment_vars.update(Brian1Engine.environment_vars)
         inform("PATH: " + JNeuroMLBrianEngine.path)
         inform("Env vars: %s" % JNeuroMLBrianEngine.environment_vars)
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlbrian2.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlbrian2.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromleden.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromleden.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlmoose.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlmoose.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             JNeuroMLEngine.install(None)
             inform(
                 "%s installed JNeuroML..." % JNeuroMLNetPyNEEngine.name,
                 indent=2,
                 verbosity=1,
             )
         if not NetPyNEEngine.is_installed():
-            NetPyNEEngine.install(None)
+            NetPyNEEngine.install(version)
             inform(
                 "%s installed NetPyNE (& NEURON)..." % JNeuroMLNetPyNEEngine.name,
                 indent=2,
                 verbosity=1,
             )
 
         environment_vars_nrn, path_nrn = NeuronEngine.get_nrn_environment()
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne_np2.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne_np2.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlnetpyne_np4.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlnetpyne_np4.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlnrn.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlnrn.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlpynnnrn.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlpynnnrn.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             JNeuroMLEngine.install(None)
             inform(
                 "%s installed JNeuroML..." % JNeuroMLPyNNNRNEngine.name,
                 indent=2,
                 verbosity=1,
             )
         if not PyNNNRNEngine.is_installed():
-            PyNNNRNEngine.install(None)
+            PyNNNRNEngine.install(version)
             inform(
                 "%s installed PyNN & NRN..." % JNeuroMLPyNNNRNEngine.name,
                 indent=2,
                 verbosity=1,
             )
 
         environment_vars_nrn, path_nrn = NeuronEngine.get_nrn_environment()
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlvalidate.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlvalidate.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     @staticmethod
     def is_installed():
         return JNeuroMLEngine.is_installed()
 
     @staticmethod
     def install(version):
         if not JNeuroMLEngine.is_installed():
-            JNeuroMLEngine.install(None)
+            JNeuroMLEngine.install(version)
 
         JNeuroMLValidateEngine.path = JNeuroMLEngine.path
         JNeuroMLValidateEngine.environment_vars = {}
         JNeuroMLValidateEngine.environment_vars.update(JNeuroMLEngine.environment_vars)
 
     def run(self):
         try:
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/jneuromlvalidatev1.py` & `osbmodelvalidation-0.2.21/omv/engines/jneuromlvalidatev1.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     @staticmethod
     def is_installed():
         return JNeuroMLEngine.is_installed()
 
     @staticmethod
     def install(version):
         if not JNeuroMLEngine.is_installed():
-            JNeuroMLEngine.install(None)
+            JNeuroMLEngine.install(version)
 
         JNeuroMLValidateV1Engine.path = JNeuroMLEngine.path
         JNeuroMLValidateV1Engine.environment_vars = {}
         JNeuroMLValidateV1Engine.environment_vars.update(
             JNeuroMLEngine.environment_vars
         )
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/moose_.py` & `osbmodelvalidation-0.2.21/omv/engines/moose_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/nestsli.py` & `osbmodelvalidation-0.2.21/omv/engines/nestsli.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/netpyne_.py` & `osbmodelvalidation-0.2.21/omv/engines/netpyne_.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                 "%s installed PyNeuroML..." % NetPyNEEngine.name, indent=2, verbosity=1
             )
 
         from omv.engines.getnetpyne import install_netpyne
 
         home = os.environ["HOME"]
         inform("Will fetch and install the latest NetPyNE..", indent=2)
-        install_netpyne()
+        install_netpyne(version)
         inform("Done, NetPyNE is correctly installed...", indent=2)
 
         NetPyNEEngine.path = PyNRNEngine.path
         NetPyNEEngine.environment_vars = {}
         NetPyNEEngine.environment_vars.update(PyNRNEngine.environment_vars)
 
         inform("PATH: " + NetPyNEEngine.path, indent=2, verbosity=1)
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/netpyne__np2.py` & `osbmodelvalidation-0.2.21/omv/engines/netpyne__np2.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/netpyne__np4.py` & `osbmodelvalidation-0.2.21/omv/engines/netpyne__np4.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/neuron_.py` & `osbmodelvalidation-0.2.21/omv/engines/neuron_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/octave.py` & `osbmodelvalidation-0.2.21/omv/engines/octave.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pylems.py` & `osbmodelvalidation-0.2.21/omv/engines/pylems.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pylemsnml2.py` & `osbmodelvalidation-0.2.21/omv/engines/pylemsnml2.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if nml2_installed and PyLemsEngine.is_installed():
             return PyLemsEngine.is_installed()
         else:
             return False
 
     def install(self, version):
         if not PyLemsEngine.is_installed():
-            PyLemsEngine.install(None)
+            PyLemsEngine.install(version)
         if not os.path.isdir(default_nml2_dir):
             install_nml2()
 
         inform("Finished installation of %s..." % self.name, indent=2)
 
     def run(self):
         try:
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynest.py` & `osbmodelvalidation-0.2.21/omv/engines/pynest.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pyneuroconstruct.py` & `osbmodelvalidation-0.2.21/omv/engines/pyneuroconstruct.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pyneuroml_.py` & `osbmodelvalidation-0.2.21/omv/engines/pyneuroml_.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pyneuromlvalidatesbml.py` & `osbmodelvalidation-0.2.21/omv/engines/pyneuromlvalidatesbml.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pyneuron.py` & `osbmodelvalidation-0.2.21/omv/engines/pyneuron.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynn.py` & `osbmodelvalidation-0.2.21/omv/engines/pynn.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynnbrian1.py` & `osbmodelvalidation-0.2.21/omv/engines/pynnbrian1.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynnbrian2.py` & `osbmodelvalidation-0.2.21/omv/engines/pynnbrian2.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynnnest.py` & `osbmodelvalidation-0.2.21/omv/engines/pynnnest.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynnneuroml.py` & `osbmodelvalidation-0.2.21/omv/engines/pynnneuroml.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                 "Checking whether %s is installed..." % PyNNNeuroMLEngine.name, indent=1
             )
         return PyNNEngine.is_installed() and PyNeuroMLEngine.is_installed()
 
     @staticmethod
     def install(version):
         if not PyNeuroMLEngine.is_installed():
-            PyNeuroMLEngine.install(None)
+            PyNeuroMLEngine.install(version)
             inform(
                 "%s installed PyNeuroML..." % PyNNNeuroMLEngine.name,
                 indent=2,
                 verbosity=1,
             )
         if not PyNNEngine.is_installed():
             PyNNEngine.install(None)
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/pynnneuron.py` & `osbmodelvalidation-0.2.21/omv/engines/pynnneuron.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         installed = PyNNEngine.is_installed() and NeuronEngine.is_installed()
 
         return installed
 
     @staticmethod
     def install(version=None):
         if not NeuronEngine.is_installed():
-            NeuronEngine.install(None)
+            NeuronEngine.install(version)
             inform("%s installed NEURON..." % PyNNNRNEngine.name, indent=2, verbosity=1)
         if not PyNNEngine.is_installed():
             PyNNEngine.install(None)
             inform("%s installed PyNN..." % PyNNNRNEngine.name, indent=2, verbosity=1)
 
         import pyNN
```

### Comparing `osbmodelvalidation-0.2.20/omv/engines/utils/genesis_utils.g` & `osbmodelvalidation-0.2.21/omv/engines/utils/genesis_utils.g`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/experiment.py` & `osbmodelvalidation-0.2.21/omv/experiment.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/find_tests.py` & `osbmodelvalidation-0.2.21/omv/find_tests.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/omt_mep_parser.py` & `osbmodelvalidation-0.2.21/omv/omt_mep_parser.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/omv_util.py` & `osbmodelvalidation-0.2.21/omv/omv_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,24 @@
             if ee.is_installed():
                 already_installed = True
             else:
                 from omv.engines.getarbor import install_arbor
 
                 install_arbor(engine_version)
 
+        elif eng.lower() == "XPP".lower():
+            from omv.engines.xpp import XppEngine as ee
+
+            if ee.is_installed():
+                already_installed = True
+            else:
+                from omv.engines.getxpp import install_xpp
+
+                install_xpp(engine_version)
+
         elif eng.lower() == "EDEN".lower():
             from omv.engines.eden_ import EdenEngine as ee
 
             if ee.is_installed():
                 already_installed = True
             else:
                 from omv.engines.geteden import install_eden
```

### Comparing `osbmodelvalidation-0.2.20/omv/parse_omt.py` & `osbmodelvalidation-0.2.21/omv/parse_omt.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/schemata/types/test/experiment.2.yaml` & `osbmodelvalidation-0.2.21/omv/schemata/types/test/experiment.2.yaml`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/tally.py` & `osbmodelvalidation-0.2.21/omv/tally.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/test/test_rates.py` & `osbmodelvalidation-0.2.21/omv/test/test_rates.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/test/test_types.py` & `osbmodelvalidation-0.2.21/omv/test/test_types.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/validation/rx_validator.py` & `osbmodelvalidation-0.2.21/omv/validation/rx_validator.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/validation/utils.py` & `osbmodelvalidation-0.2.21/omv/validation/utils.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/omv/validation/validate.py` & `osbmodelvalidation-0.2.21/omv/validation/validate.py`

 * *Files identical despite different names*

### Comparing `osbmodelvalidation-0.2.20/setup.cfg` & `osbmodelvalidation-0.2.21/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = OSBModelValidation
-version = 0.2.20
+version = 0.2.21
 author = Boris Marin, Padraig Gleeson
 author_email = borismarin@gmail.com
 url = https://github.com/OpenSourceBrain/osb-model-validation
 license = LGPL-3.0-only
 description = Open Source Brain Model validation
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -14,14 +14,15 @@
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Topic :: Scientific/Engineering
 
 [options]
 install_requires = 
 	PyYAML
 	numpy
 	pyrx
```

