# Comparing `tmp/hera_sim-4.2.1.tar.gz` & `tmp/hera_sim-4.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hera_sim-4.2.1.tar", last modified: Mon Jan 22 15:32:04 2024, max compression
+gzip compressed data, was "hera_sim-4.2.2.tar", last modified: Tue Apr 23 20:50:44 2024, max compression
```

## Comparing `hera_sim-4.2.1.tar` & `hera_sim-4.2.2.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.738436 hera_sim-4.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.702436 hera_sim-4.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.702436 hera_sim-4.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.github/workflows/test_suite.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-01-22 15:31:55.000000 hera_sim-4.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-22 15:31:55.000000 hera_sim-4.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20417 2024-01-22 15:31:55.000000 hera_sim-4.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-01-22 15:31:55.000000 hera_sim-4.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-22 15:31:55.000000 hera_sim-4.2.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-01-22 15:31:55.000000 hera_sim-4.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-01-22 15:32:04.738436 hera_sim-4.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-01-22 15:31:55.000000 hera_sim-4.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.702436 hera_sim-4.2.1/config_examples/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-01-22 15:31:55.000000 hera_sim-4.2.1/config_examples/simulator.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-01-22 15:31:55.000000 hera_sim-4.2.1/config_examples/template_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.706436 hera_sim-4.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.706436 hera_sim-4.2.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/_templates/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/_templates/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/environment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/notes_for_developers.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.706436 hera_sim-4.2.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.714436 hera_sim-4.2.1/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)   344696 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/end_to_end_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/hera_sim_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)   145439 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/hera_sim_defaults.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  2406697 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/hera_sim_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)  2634846 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/hera_sim_tour.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/hera_sim_vis_cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)   469268 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/mutual_coupling_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)    95849 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/polybeam_simulation.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   165797 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials/visibility_simulator.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-22 15:31:55.000000 hera_sim-4.2.1/docs/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.718436 hera_sim-4.2.1/hera_sim/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/__yaml_constructors.py
--rw-r--r--   0 runner    (1001) docker     (127)    42733 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/antpos.py
--rw-r--r--   0 runner    (1001) docker     (127)    48320 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     9112 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.722436 hera_sim-4.2.1/hera_sim/config/
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/config/H1C.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/config/H2C.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/config/debug.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.726436 hera_sim-4.2.1/hera_sim/data/
--rw-r--r--   0 runner    (1001) docker     (127)   815652 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/H37_FR_Filters_small.npz
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H1C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H1C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H1C_REFLECTIONS.npz
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H2C_BANDPASS.npy
--rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H2C_BEAM_POLY.npy
--rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H4C_BANDPASS.npz
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
--rw-r--r--   0 runner    (1001) docker     (127)    49740 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_H4C_REFLECTIONS.npz
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_LAT_LON_ALT.npy
--rw-r--r--   0 runner    (1001) docker     (127)    51246 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_Tsky_Reformatted.npz
--rw-r--r--   0 runner    (1001) docker     (127)    50598 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/HERA_Tsky_vs_LST.npz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.698436 hera_sim-4.2.1/hera_sim/data/tutorials_data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.726436 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   229229 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.726436 hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13419 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/eor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14162 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/interpolators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8105 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)    16249 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    61882 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/sigchain.py
--rw-r--r--   0 runner    (1001) docker     (127)    63166 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/simulate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.730436 hera_sim-4.2.1/hera_sim/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    40580 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_adjustment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_antpos.py
--rw-r--r--   0 runner    (1001) docker     (127)    16636 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_beams.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7016 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_compare_pyuvsim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_eor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_foregrounds.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_interpolators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_rfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_sigchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_sim_red_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_simulate_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    22073 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_simulator.py
--rw-r--r--   0 runner    (1001) docker     (127)    16007 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17810 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_vis_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/test_yaml_constructors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.730436 hera_sim-4.2.1/hera_sim/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/healvis_catalog.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.734436 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/
--rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2635200 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
--rw-r--r--   0 runner    (1001) docker     (127)    59077 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
--rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/matvis_cpu.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/matvis_gpu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1798 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/vis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.738436 hera_sim-4.2.1/hera_sim/visibilities/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    20431 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/matvis.py
--rw-r--r--   0 runner    (1001) docker     (127)     2181 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/pyuvsim_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    18643 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/simulators.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-22 15:31:55.000000 hera_sim-4.2.1/hera_sim/visibilities/vis_cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.738436 hera_sim-4.2.1/hera_sim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-22 15:32:04.000000 hera_sim-4.2.1/hera_sim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-01-22 15:31:55.000000 hera_sim-4.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-22 15:32:04.738436 hera_sim-4.2.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     7038 2024-01-22 15:31:55.000000 hera_sim-4.2.1/scripts/hera-sim-simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-01-22 15:31:55.000000 hera_sim-4.2.1/scripts/hera-sim-vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-22 15:32:04.742436 hera_sim-4.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-22 15:31:55.000000 hera_sim-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.766716 hera_sim-4.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.730717 hera_sim-4.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.730717 hera_sim-4.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.github/workflows/test_suite.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-23 20:50:40.000000 hera_sim-4.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-23 20:50:40.000000 hera_sim-4.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-23 20:50:40.000000 hera_sim-4.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2427 2024-04-23 20:50:40.000000 hera_sim-4.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-23 20:50:40.000000 hera_sim-4.2.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-23 20:50:40.000000 hera_sim-4.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-23 20:50:44.762716 hera_sim-4.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3631 2024-04-23 20:50:40.000000 hera_sim-4.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.730717 hera_sim-4.2.2/config_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-23 20:50:40.000000 hera_sim-4.2.2/config_examples/simulator.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4973 2024-04-23 20:50:40.000000 hera_sim-4.2.2/config_examples/template_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.734717 hera_sim-4.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5586 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.734717 hera_sim-4.2.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/_templates/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/_templates/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6391 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/environment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/notes_for_developers.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.734717 hera_sim-4.2.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.742716 hera_sim-4.2.2/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   344696 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/end_to_end_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/hera_sim_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   145439 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/hera_sim_defaults.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2406697 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/hera_sim_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)  2634846 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/hera_sim_tour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/hera_sim_vis_cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)   469268 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/mutual_coupling_example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    95849 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/polybeam_simulation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   165797 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials/visibility_simulator.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 20:50:40.000000 hera_sim-4.2.2/docs/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.746717 hera_sim-4.2.2/hera_sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/__yaml_constructors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42735 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6375 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/antpos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48321 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9111 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11969 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.746717 hera_sim-4.2.2/hera_sim/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/config/H1C.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/config/H2C.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/config/debug.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.750717 hera_sim-4.2.2/hera_sim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   815652 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/H37_FR_Filters_small.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H1C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     2446 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H1C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    25092 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H1C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H1C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H2C_BANDPASS.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     3680 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H2C_BEAM_MODEL.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H2C_BEAM_POLY.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     4488 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H2C_RFI_STATIONS.npy
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H4C_BANDPASS.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    49740 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_H4C_REFLECTIONS.npz
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_LAT_LON_ALT.npy
+-rw-r--r--   0 runner    (1001) docker     (127)    51246 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_Tsky_Reformatted.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    50598 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/HERA_Tsky_vs_LST.npz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.730717 hera_sim-4.2.2/hera_sim/data/tutorials_data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.750717 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/array_layout.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3243 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/obsparams.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   229229 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/telescope.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.754716 hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20400 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/obsparam_hera_phase1_gleam_top50.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/telescope_config_hera_airy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13379 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/eor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11305 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14154 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8106 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61891 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64238 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/simulate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.754716 hera_sim-4.2.2/hera_sim/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40580 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_adjustment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_antpos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16636 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_beams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_compare_pyuvsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_eor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_foregrounds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_interpolators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5505 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_rfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34942 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_sigchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_sim_red_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_simulate_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23764 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16015 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18330 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_vis_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/test_yaml_constructors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.754716 hera_sim-4.2.2/hera_sim/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/healvis_catalog.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.758716 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      929 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2635200 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    59077 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot
+-rwxr-xr-x   0 runner    (1001) docker     (127)      130 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/h4c_idr2.1_teleconfig.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      110 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/matvis_cpu.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      124 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/matvis_gpu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    27061 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/vis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.762716 hera_sim-4.2.2/hera_sim/visibilities/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9615 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20434 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/matvis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/pyuvsim_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:40.000000 hera_sim-4.2.2/hera_sim/visibilities/vis_cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.762716 hera_sim-4.2.2/hera_sim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6129 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 20:50:44.000000 hera_sim-4.2.2/hera_sim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-23 20:50:40.000000 hera_sim-4.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 20:50:44.762716 hera_sim-4.2.2/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-23 20:50:40.000000 hera_sim-4.2.2/scripts/hera-sim-simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-23 20:50:40.000000 hera_sim-4.2.2/scripts/hera-sim-vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-23 20:50:44.766716 hera_sim-4.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 20:50:40.000000 hera_sim-4.2.2/setup.py
```

### Comparing `hera_sim-4.2.1/.coveragerc` & `hera_sim-4.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/.flake8` & `hera_sim-4.2.2/.flake8`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     A003,
     # inline strong start-string without end-string. This is OK in the case of **kwargs in parameters.
     RST210,
     # Logging statement uses f-string.
     G004,
     # Logging statement uses + (this makes no sense...)
     G003,
+    # Allow builtin module names
+    A005,
 max-line-length = 88
 # Should be 18.
 max-complexity = 35
 exclude =
     development/*
 per-file-ignores =
     # print statements allowed in tests
```

### Comparing `hera_sim-4.2.1/.github/workflows/publish.yaml` & `hera_sim-4.2.2/.github/workflows/publish.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -27,11 +27,11 @@
 
       - name: Build a binary wheel and a source tarball
         run: |
           python -m build
 
       - name: Publish to PyPI
         if: startsWith(github.event.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.12
         with:
           user: __token__
           password: ${{ secrets.pypi_password }}
```

### Comparing `hera_sim-4.2.1/.github/workflows/test_suite.yaml` & `hera_sim-4.2.2/.github/workflows/test_suite.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       OS: ${{ matrix.os }}
     name: Testing
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest]
-        python-version: [3.9, "3.10", "3.11"]
+        python-version: ["3.10", "3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@main
         with:
           fetch-depth: 1
 
       - uses: mpi4py/setup-mpi@v1
@@ -40,14 +40,15 @@
           pip install .[tests]
 
       - name: Run Tests
         run: |
           python -m pytest --log-cli-level INFO
 
       - name: Upload coverage report
-        uses: codecov/codecov-action@v3.1.4
+        uses: codecov/codecov-action@v4.1.1
         with:
-          token: ${{ secrets.CODECOV_TOKEN }}
           file: ./coverage.xml
           flags: unittests
           name: codecov-umbrella
           fail_ci_if_error: true
+        env:
+          CODECOV_TOKEN: ${{ secrets.CODECOV_TOKEN }}
```

### Comparing `hera_sim-4.2.1/.pre-commit-config.yaml` & `hera_sim-4.2.2/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: 'config.yaml|config_examples/.*.yaml|hera_sim/config/H1C.yaml|hera_sim/config/H2C.yaml|setup.py|hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   # - id: check-merge-conflict
   - id: check-xml
@@ -21,40 +21,47 @@
     rev: 7.0.0  # pick a git hash / tag to point to
     hooks:
     -   id: flake8
         additional_dependencies:
           - flake8-rst-docstrings
           #- flake8-docstrings  # not available for flake8>5
           - flake8-builtins
-          - flake8-logging-format
           - flake8-rst-docstrings
           - flake8-rst
 #          - flake8-markdown    # not available for flake8>5 (check later...)
           - flake8-bugbear
           - flake8-comprehensions
           - flake8-print
 
 - repo: https://github.com/psf/black-pre-commit-mirror
-  rev: 23.12.1
+  rev: 24.4.0
   hooks:
     - id: black
 
 - repo: https://github.com/pre-commit/pygrep-hooks
   rev: v1.10.0
   hooks:
     - id: rst-backticks
 
 - repo: https://github.com/PyCQA/isort
   rev: 5.13.2
   hooks:
   - id: isort
 
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.15.0
+  rev: v3.15.2
   hooks:
   - id: pyupgrade
     args: [--py39-plus]
 
 - repo: https://github.com/asottile/setup-cfg-fmt
   rev: v2.5.0
   hooks:
-  - id: setup-cfg-fmt
+  - id: setup-cfg-fmt
+
+- repo: https://github.com/astral-sh/ruff-pre-commit
+  # Ruff version.
+  rev: v0.4.1
+  hooks:
+    # Run the linter.
+    - id: ruff
+      args: [--fix]
```

### Comparing `hera_sim-4.2.1/CHANGELOG.rst` & `hera_sim-4.2.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 dev
 ===
 
+Deprecated
+----------
+
+- Support for Python 3.9 has been dropped.
+
 Fixed
 -----
 - API calls for pyuvdata v2.4.0.
 
 v4.1.0 [2023.06.26]
 ===================
 This release heavily focuses on performance of the visibility simulators, and in
```

### Comparing `hera_sim-4.2.1/CONTRIBUTING.rst` & `hera_sim-4.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/LICENSE.rst` & `hera_sim-4.2.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/PKG-INFO` & `hera_sim-4.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera_sim
-Version: 4.2.1
+Version: 4.2.2
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.2.1/README.rst` & `hera_sim-4.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/config_examples/template_config.yaml` & `hera_sim-4.2.2/config_examples/template_config.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/Makefile` & `hera_sim-4.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/_templates/class.rst` & `hera_sim-4.2.2/docs/_templates/class.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/_templates/module.rst` & `hera_sim-4.2.2/docs/_templates/module.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/conf.py` & `hera_sim-4.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/reference/index.rst` & `hera_sim-4.2.2/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/end_to_end_example.ipynb` & `hera_sim-4.2.2/docs/tutorials/end_to_end_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/hera_sim_cli.rst` & `hera_sim-4.2.2/docs/tutorials/hera_sim_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/hera_sim_defaults.ipynb` & `hera_sim-4.2.2/docs/tutorials/hera_sim_defaults.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/hera_sim_simulator.ipynb` & `hera_sim-4.2.2/docs/tutorials/hera_sim_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/hera_sim_tour.ipynb` & `hera_sim-4.2.2/docs/tutorials/hera_sim_tour.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/hera_sim_vis_cli.rst` & `hera_sim-4.2.2/docs/tutorials/hera_sim_vis_cli.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/mutual_coupling_example.ipynb` & `hera_sim-4.2.2/docs/tutorials/mutual_coupling_example.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/polybeam_simulation.ipynb` & `hera_sim-4.2.2/docs/tutorials/polybeam_simulation.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials/visibility_simulator.ipynb` & `hera_sim-4.2.2/docs/tutorials/visibility_simulator.ipynb`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/docs/tutorials.rst` & `hera_sim-4.2.2/docs/tutorials.rst`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/__init__.py` & `hera_sim-4.2.2/hera_sim/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """A package for running instrument and systematic simulations for HERA."""
+
 from pathlib import Path
 
 try:
     from importlib.metadata import PackageNotFoundError, version
 except ImportError:
     from importlib_metadata import PackageNotFoundError, version
```

### Comparing `hera_sim-4.2.1/hera_sim/__yaml_constructors.py` & `hera_sim-4.2.2/hera_sim/__yaml_constructors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 A module for generating new YAML tags for the various ``hera_sim`` interpolator objects.
 
 This may need to be updated if the :mod:`.interpolators` module is updated.
 """
+
 import astropy.units as u
 import inspect
 import warnings
 import yaml
 
 from . import antpos, interpolators
```

### Comparing `hera_sim-4.2.1/hera_sim/adjustment.py` & `hera_sim-4.2.2/hera_sim/adjustment.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,17 +399,17 @@
         target_copy.data_array[this_slice] = vis
         target_copy.flag_array[this_slice] = target.get_flags(antpairpol)
         target_copy.nsample_array[this_slice] = target.get_nsamples(antpairpol)
 
         # Update the baseline array in case the antenna numbers got jumbled.
         old_bl_int = target.antnums_to_baseline(ant1, ant2)
         new_bl_int = target.antnums_to_baseline(*new_antpairpol[:2])
-        target_copy.baseline_array[
-            target_copy.baseline_array == old_bl_int
-        ] = new_bl_int
+        target_copy.baseline_array[target_copy.baseline_array == old_bl_int] = (
+            new_bl_int
+        )
 
     # Update the uvw array just to be safe.
     target_copy.set_uvws_from_antenna_positions()
 
     # Make sure to return a Simulator object if one was passed.
     if target_is_simulator:
         target_copy = Simulator(data=target_copy)
```

### Comparing `hera_sim-4.2.1/hera_sim/antpos.py` & `hera_sim-4.2.2/hera_sim/antpos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """A module for creating antenna array configurations.
 
 Input parameters vary between functions, but all functions return a
 dictionary whose keys refer to antenna numbers and whose values refer
 to the ENU position of the antennas.
 """
+
 import numpy as np
 
 from .components import component
 
 # FIXME: old docstrings state that the positions are returned in topocentric
 # coordinates, but this is contradictory to the claim that a linear array
 # is constructed as purely east-west. Let's resolve this before publishing v1
```

### Comparing `hera_sim-4.2.1/hera_sim/beams.py` & `hera_sim-4.2.2/hera_sim/beams.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module defining analytic polynomial beams."""
+
 import numpy as np
 from numpy.polynomial.chebyshev import chebval
 from pyuvsim import AnalyticBeam
 
 from . import utils
```

### Comparing `hera_sim-4.2.1/hera_sim/cli_utils.py` & `hera_sim-4.2.2/hera_sim/cli_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Useful helper functions and argparsers for running simulations via CLI."""
+
 from __future__ import annotations
 
 import itertools
 import numpy as np
 import os
 import warnings
 from pyuvdata import UVData
@@ -56,15 +57,15 @@
     Raises
     ------
     ValueError
         If either insufficient information is provided, or the info
         is not valid.
     """
     if config.get("defaults") is not None:
-        if type(config["defaults"]) is not str:
+        if not isinstance(config["defaults"], str):
             raise ValueError(
                 "Defaults in the CLI may only be specified using a string. "
                 "The string used may specify either a path to a configuration "
                 "yaml or one of the named default configurations."
             )
 
         if config["defaults"] in SEASON_CONFIGS.keys():
@@ -150,15 +151,15 @@
                 "If a simulation is not provided, then both frequencies and "
                 "times must be specified."
             )
 
     # Update gain keys to conform to write_cal assumptions.
     # New Simulator gains have keys (ant, pol), so shouldn't need
     # special pre-processing.
-    if all(np.issctype(type(ant)) for ant in gains.keys()):
+    if all(np.isscalar(ant) for ant in gains.keys()):
         # Old-style, single polarization assumption.
         gains = {(ant, "Jee"): gain for ant, gain in gains.items()}
 
     # At the time of writing, the write_cal function *fails silently* if the
     # keys for the gain dictionary are not tuples specifying the antenna and
     # Jones polarization string. Using linear polarizations, as in (1, 'x'),
     # will cause the function to think that the gains do not exist, and so
```

### Comparing `hera_sim-4.2.1/hera_sim/components.py` & `hera_sim-4.2.2/hera_sim/components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/config/H1C.yaml` & `hera_sim-4.2.2/hera_sim/config/H1C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/config/H2C.yaml` & `hera_sim-4.2.2/hera_sim/config/H2C.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/config/debug.yaml` & `hera_sim-4.2.2/hera_sim/config/debug.yaml`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/H37_FR_Filters_small.npz` & `hera_sim-4.2.2/hera_sim/data/H37_FR_Filters_small.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H1C_BEAM_INTEGRALS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H1C_REFLECTIONS.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H1C_REFLECTIONS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H1C_RFI_STATIONS.npy` & `hera_sim-4.2.2/hera_sim/data/HERA_H1C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H2C_BEAM_MODEL.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H2C_BEAM_MODEL.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H2C_RFI_STATIONS.npy` & `hera_sim-4.2.2/hera_sim/data/HERA_H2C_RFI_STATIONS.npy`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H4C_BANDPASS.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H4C_BANDPASS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H4C_BEAM_INTEGRALS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_H4C_REFLECTIONS.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_H4C_REFLECTIONS.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_Tsky_Reformatted.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_Tsky_Reformatted.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/HERA_Tsky_vs_LST.npz` & `hera_sim-4.2.2/hera_sim/data/HERA_Tsky_vs_LST.npz`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py` & `hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/make_mock_catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Script for making a mock point source catalog."""
+
 import argparse
 import numpy as np
 from astropy import units
 from astropy.coordinates import EarthLocation, Latitude, Longitude
 from pyradiosky import SkyModel
 from pyuvsim import create_mock_catalog
 from pyuvsim.simsetup import initialize_uvdata_from_params
@@ -13,17 +14,20 @@
     obsparam_file,
     Nsrcs=200,
     src_prefix="mock",
     flux_cut=20,
     sigma=5,
     index_low=-3,
     index_high=-1,
+    seed=None,
 ):
     """Generate and svae a mock point source catalog."""
     # Easiset to load the metadata this way.
+    rng = np.random.default_rng(seed)
+
     temp_uvdata = initialize_uvdata_from_params(str(obsparam_file))[0]
     center_time = np.mean(np.unique(temp_uvdata.time_array))
     ref_freq = np.mean(np.unique(temp_uvdata.freq_array))
     array_location = EarthLocation(*temp_uvdata.telescope_location_lat_lon_alt_degrees)
     sky_model = create_mock_catalog(
         center_time,
         arrangement="random",
@@ -33,19 +37,19 @@
     sky_model_recarray = sky_model.to_recarray()
 
     # Get the source positions.
     ras = np.array([row[1] for row in sky_model_recarray])
     decs = np.array([row[2] for row in sky_model_recarray])
 
     # Randomly assign fluxes (whether this is realistic or not).
-    ref_fluxes = np.random.lognormal(mean=1, sigma=sigma, size=len(ras))
+    ref_fluxes = rng.lognormal(mean=1, sigma=sigma, size=len(ras))
     # Don't include super bright sources.
     ref_fluxes[ref_fluxes > flux_cut] = 1 / ref_fluxes[ref_fluxes > flux_cut]
     # Assign spectral indices.
-    indices = np.random.uniform(low=index_low, high=index_high, size=len(ras))
+    indices = rng.uniform(low=index_low, high=index_high, size=len(ras))
 
     # Actually add in the spectral structure.
     freqs = np.unique(temp_uvdata.freq_array)
     ref_freq = np.mean(freqs)
     scales = np.exp(np.outer(np.log(freqs / ref_freq), indices))
     fluxes = ref_fluxes.reshape(1, -1) * scales
     stokes = np.zeros((4,) + fluxes.shape, dtype=float)
```

### Comparing `hera_sim-4.2.1/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt` & `hera_sim-4.2.2/hera_sim/data/tutorials_data/end_to_end/sample_catalog.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv` & `hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/antenna_layout_hera_phase1.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5` & `hera_sim-4.2.2/hera_sim/data/tutorials_data/visibility_simulator/gleam_top50.skyh5`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/defaults.py` & `hera_sim-4.2.2/hera_sim/defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -341,17 +341,15 @@
                 keys = set(list(old_kwargs.keys()) + list(passed_args.keys()))
 
             # make a final dictionary to pass to func
             final_args = {
                 arg: (
                     passed_args[arg]
                     if arg in passed_args
-                    else new_args[arg]
-                    if self._override_defaults
-                    else old_kwargs[arg]
+                    else new_args[arg] if self._override_defaults else old_kwargs[arg]
                 )
                 for arg in keys
             }
 
             # use the final set of arguments/kwargs
             return func(**final_args)
```

### Comparing `hera_sim-4.2.1/hera_sim/eor.py` & `hera_sim-4.2.2/hera_sim/eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/foregrounds.py` & `hera_sim-4.2.2/hera_sim/foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/interpolators.py` & `hera_sim-4.2.2/hera_sim/interpolators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module provides interfaces to different interpolation classes."""
+
 import numpy as np
 import warnings
 from cached_property import cached_property
 from os import path
 from scipy.interpolate import RectBivariateSpline, interp1d
 
 from hera_sim import DATA_PATH
@@ -311,16 +312,16 @@
         if self._interp_type == "interp1d":
             assert path.splitext(self._datafile)[1] == ".npz", (
                 "In order to use an 'interp1d' object, the reference file "
                 "must be a '.npz' file."
             )
             assert self._obj in self._data.keys() and "freqs" in self._data.keys(), (
                 "You've chosen to use an interp1d object for modeling the "
-                "{}. Please ensure that the `.npz` archive has the following "
-                "keys: 'freqs', '{}'".format(self._obj, self._obj)
+                f"{self._obj}. Please ensure that the `.npz` archive has the following "
+                f"keys: 'freqs', '{self._obj}'"
             )
         else:
             # we can relax this a bit and allow for users to also pass a npz
             # with the same keys as in the above case, but it seems silly to
             # use a polynomial interpolator instead of a spline interpolator in
             # this case
             assert path.splitext(self._datafile)[1] == ".npy", (
```

### Comparing `hera_sim-4.2.1/hera_sim/io.py` & `hera_sim-4.2.2/hera_sim/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods for input/output of data."""
+
 import numpy as np
 import os
 import pyuvdata
 import re
 import warnings
 from collections.abc import Sequence
 from pyuvdata import UVData
```

### Comparing `hera_sim-4.2.1/hera_sim/noise.py` & `hera_sim-4.2.2/hera_sim/noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/rfi.py` & `hera_sim-4.2.2/hera_sim/rfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Models of radio frequency interference."""
+
 import astropy.units as u
 import numpy as np
 import warnings
 from pathlib import Path
 
 from .components import component
 from .utils import _listify
@@ -479,16 +480,16 @@
                     "dtv_chance, dtv_strength, or dtv_std is not "
                     "formatted properly. These parameters must satisfy "
                     "*one* of the following conditions: \n"
                     "Only a single value is specified *OR* a list of "
                     "values with the same length as the number of DTV "
                     "bands specified. For reference, the DTV bands you "
                     "specified have the following characteristics: \n"
-                    "f_min : {fmin} \nf_max : {fmax}\n N_bands : "
-                    "{Nchan}".format(fmin=bands[0], fmax=bands[-1], Nchan=Nchan)
+                    f"f_min : {bands[0]} \nf_max : {bands[-1]}\n N_bands : "
+                    f"{Nchan}"
                 )
 
             # everything should be in order now, so
             listified_params.append(np.asarray(arg))
 
         return listified_params
```

### Comparing `hera_sim-4.2.1/hera_sim/sigchain.py` & `hera_sim-4.2.2/hera_sim/sigchain.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """Models of signal-chain systematics.
 
 This module defines several models of systematics that arise in the signal chain, for
 example bandpass gains, reflections and cross-talk.
 """
+
 from __future__ import annotations
 
 import astropy_healpix as aph
 import copy
 import numpy as np
 import warnings
 from astropy import constants, units
 from collections.abc import Sequence
 from pathlib import Path
 from pyuvdata import UVBeam
 from pyuvsim import AnalyticBeam
 from scipy import stats
-from scipy.signal import blackmanharris
+from scipy.signal.windows import blackmanharris
 from typing import Callable
 
 from . import DATA_PATH, interpolators, utils
 from .components import component
 from .defaults import _defaults
 
 try:
```

### Comparing `hera_sim-4.2.1/hera_sim/simulate.py` & `hera_sim-4.2.2/hera_sim/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 
 This module defines the :class:`Simulator` class, which provides the user
 with a high-level interface to all of the features provided by :mod:`hera_sim`.
 For detailed instructions on how to manage a simulation using the
 :class:`Simulator`, please refer to the tutorials.
 """
 
+import contextlib
 import functools
 import inspect
 import numpy as np
 import time
 import warnings
 import yaml
 from astropy import constants as const
 from cached_property import cached_property
 from collections.abc import Sequence
 from deprecation import deprecated
 from pathlib import Path
 from pyuvdata import UVData
+from pyuvdata import utils as uvutils
 from typing import Optional, Union
 
 from . import __version__, io, utils
 from .components import SimulationComponent, get_model, list_all_components
 from .defaults import defaults
 
 _add_depr = deprecated(
@@ -723,15 +725,15 @@
             return False
         elif len(vis_filter) == 1:
             # For now, assume a string specifies a polarization.
             if isinstance(vis_filter[0], str):
                 return not pol == vis_filter[0]
             # Otherwise, assume that this specifies an antenna.
             else:
-                return not vis_filter[0] in (ant1, ant2)
+                return vis_filter[0] not in (ant1, ant2)
         elif len(vis_filter) == 2:
             # TODO: This will need to be updated when we support ant strings.
             # Three cases: two pols; an ant+pol; a baseline.
             # If it's two polarizations, then make sure this pol is one of them.
             if all(isinstance(key, str) for key in vis_filter):
                 return pol not in vis_filter
             # If it's an ant+pol, make sure both the antenna and pol are present.
@@ -752,15 +754,15 @@
         else:
             # Assume it's some list of antennas/polarizations.
             pols = []
             ants = []
             for key in vis_filter:
                 if isinstance(key, str):
                     pols.append(key)
-                elif type(key) is int:
+                elif isinstance(key, int):
                     ants.append(key)
             # We want polarization and ant1 or ant2 in the filter.
             # This would be used in simulating e.g. a few feeds that have an
             # abnormally high system temperature.
             return not (pol in pols and (ant1 in ants or ant2 in ants))
 
     def _calculate_reds(self, tol=1.0):
@@ -1224,15 +1226,15 @@
         ValueError
             Two cases: one, the ``"redundant"`` seeding mode is being used
             and a baseline isn't provided; two, the seed is a string, but
             is not one of the supported seeding modes.
         """
         if seed is None:
             return
-        if type(seed) is int:
+        if isinstance(seed, int):
             np.random.seed(seed)
             return seed
         if not isinstance(seed, str):
             raise TypeError(
                 "The seeding mode must be specified as a string or integer. "
                 "If an integer is provided, then it will be used as the seed."
             )
@@ -1386,27 +1388,28 @@
         return model_params
 
     @staticmethod
     def _get_component(
         component: Union[str, type[SimulationComponent], SimulationComponent]
     ) -> Union[SimulationComponent, type[SimulationComponent]]:
         """Normalize a component to be either a class or instance."""
-        if np.issubclass_(component, SimulationComponent):
-            return component
-        elif isinstance(component, str):
+        if isinstance(component, str):
             try:
                 return get_model(component)
             except KeyError:
                 raise ValueError(
                     f"The model {component!r} does not exist. The following models are "
                     f"available: \n{list_all_components()}."
                 )
         elif isinstance(component, SimulationComponent):
             return component
         else:
+            with contextlib.suppress(TypeError):
+                if issubclass(component, SimulationComponent):
+                    return component
             raise TypeError(
                 "The input type for the component was not understood. "
                 "Must be a string, or a class/instance of type 'SimulationComponent'. "
                 f"Available component models are:\n{list_all_components()}"
             )
 
     def _generate_seed(self, model, key):
@@ -1431,59 +1434,90 @@
         return self._seeds[model][key]
 
     @staticmethod
     def _get_model_name(model):
         """Find out the (lowercase) name of a provided model."""
         if isinstance(model, str):
             return model.lower()
-        elif np.issubclass_(model, SimulationComponent):
-            return model.__name__.lower()
         elif isinstance(model, SimulationComponent):
             return model.__class__.__name__.lower()
         else:
+            with contextlib.suppress(TypeError):
+                if issubclass(model, SimulationComponent):
+                    return model.__name__.lower()
+
             raise TypeError(
                 "You are trying to simulate an effect using a custom function. "
                 "Please refer to the tutorial for instructions regarding how "
                 "to define new simulation components compatible with the Simulator."
             )
 
     def _parse_key(self, key: Union[int, str, AntPair, AntPairPol]) -> AntPairPol:
         """Convert a key of at-most length-3 to an (ant1, ant2, pol) tuple."""
+        valid_pols = {
+            k.lower()
+            for k in {
+                **uvutils.POL_STR2NUM_DICT,
+                **uvutils.JONES_STR2NUM_DICT,
+                **uvutils.CONJ_POL_DICT,
+            }
+        }
+        valid_pols.update({"jee", "jen", "jne", "jnn"})
+
+        def checkpol(pol):
+            if pol is None:
+                return None
+
+            if not isinstance(pol, str):
+                raise TypeError(f"Invalid polarization type: {type(pol)}.")
+
+            if pol.lower() not in valid_pols:
+                raise ValueError(f"Invalid polarization string: {pol}.")
+
+            return pol
+
         if key is None:
             ant1, ant2, pol = None, None, None
         elif np.issubdtype(type(key), int):
             # Figure out if it's an antenna or baseline integer
             if key in self.antpos:
                 ant1, ant2, pol = key, None, None
             else:
                 ant1, ant2 = self.data.baseline_to_antnums(key)
                 pol = None
         elif isinstance(key, str):
             if key.lower() in ("auto", "cross"):
                 raise NotImplementedError("Functionality not yet supported.")
+            key = checkpol(key)
             ant1, ant2, pol = None, None, key
         else:
+
+            def intify(x):
+                return x if x is None else int(x)
+
             try:
-                iter(key)
+                iter(key)  # ensure it's iterable
                 if len(key) not in (2, 3):
                     raise TypeError
+
+                if len(key) == 2:
+                    if all(isinstance(val, int) for val in key):
+                        ant1, ant2 = key
+                        pol = None
+                    else:
+                        ant1, pol = intify(key[0]), checkpol(key[1])
+                        ant2 = None
+                else:
+                    ant1, ant2, pol = intify(key[0]), intify(key[1]), checkpol(key[2])
+
             except TypeError:
                 raise ValueError(
                     "Key must be an integer, string, antenna pair, or antenna "
-                    "pair with a polarization string."
+                    f"pair with a polarization string. Got {key}."
                 )
-            if len(key) == 2:
-                if all(type(val) is int for val in key):
-                    ant1, ant2 = key
-                    pol = None
-                else:
-                    ant1, pol = key
-                    ant2 = None
-            else:
-                ant1, ant2, pol = key
         return ant1, ant2, pol
 
     def _sanity_check(self, model):
         """Check that simulation components are applied sensibly."""
         has_data = not np.all(self.data.data_array == 0)
         is_multiplicative = getattr(model, "is_multiplicative", False)
         contains_multiplicative_effect = any(
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/conftest.py` & `hera_sim-4.2.2/hera_sim/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_adjustment.py` & `hera_sim-4.2.2/hera_sim/tests/test_adjustment.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_antpos.py` & `hera_sim-4.2.2/hera_sim/tests/test_antpos.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_beams.py` & `hera_sim-4.2.2/hera_sim/tests/test_beams.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_cli_utils.py` & `hera_sim-4.2.2/hera_sim/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_compare_pyuvsim.py` & `hera_sim-4.2.2/hera_sim/tests/test_compare_pyuvsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Compare vis_cpu with pyuvsim visibilities."""
+
 import pytest
 
 import copy
 import numpy as np
 from astropy import units
 from astropy.coordinates import Latitude, Longitude
 from astropy.time import Time
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_components.py` & `hera_sim-4.2.2/hera_sim/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_defaults.py` & `hera_sim-4.2.2/hera_sim/tests/test_defaults.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_eor.py` & `hera_sim-4.2.2/hera_sim/tests/test_eor.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_foregrounds.py` & `hera_sim-4.2.2/hera_sim/tests/test_foregrounds.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_interpolators.py` & `hera_sim-4.2.2/hera_sim/tests/test_interpolators.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_io.py` & `hera_sim-4.2.2/hera_sim/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_noise.py` & `hera_sim-4.2.2/hera_sim/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_rfi.py` & `hera_sim-4.2.2/hera_sim/tests/test_rfi.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_sigchain.py` & `hera_sim-4.2.2/hera_sim/tests/test_sigchain.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_sim_red_data.py` & `hera_sim-4.2.2/hera_sim/tests/test_sim_red_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     assert len(gains) == 2 * (5)
     assert len(data) == 4 * (10)
     for bls in reds:
         bl0 = bls[0]
         for pol in ["xx", "xy", "yx", "yy"]:
             ai, aj, pol = bl0
             ans0 = data[ai, aj, pol] / (
-                gains[(ai, f"J{pol[0]*2}")] * gains[(aj, f"J{pol[1]*2}")].conj()
+                gains[(ai, f"J{pol[0] * 2}")] * gains[(aj, f"J{pol[1] * 2}")].conj()
             )
 
             for bl in bls[1:]:
                 ai, aj, pol = bl
                 ans = data[ai, aj, pol] / (
-                    gains[(ai, f"J{pol[0]*2}")] * gains[(aj, f"J{pol[1]*2}")].conj()
+                    gains[(ai, f"J{pol[0] * 2}")] * gains[(aj, f"J{pol[1] * 2}")].conj()
                 )
 
                 # compare calibrated visibilities knowing the input gains
                 np.testing.assert_almost_equal(ans0, ans, decimal=7)
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_simulate_cli.py` & `hera_sim-4.2.2/hera_sim/tests/test_simulate_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_simulator.py` & `hera_sim-4.2.2/hera_sim/tests/test_simulator.py`

 * *Files 6% similar despite different names*

```diff
@@ -281,26 +281,27 @@
 
 @pytest.mark.parametrize("pol", [None, "x"])
 @pytest.mark.parametrize("ant1", [None, 1])
 def test_get_multiplicative_effect(base_sim, pol, ant1):
     gains = base_sim.add("gains", seed="once", ret_vis=True)
     _gains = base_sim.get("gains", key=(ant1, pol))
     if pol is not None and ant1 is not None:
-        assert np.all(gains[(ant1, pol)] == _gains)
+        assert np.allclose(gains[(ant1, pol)], _gains)
     elif pol is None and ant1 is not None:
         assert all(
-            np.all(gains[(ant1, _pol)] == _gains[(ant1, _pol)])
+            np.allclose(gains[(ant1, _pol)], _gains[(ant1, _pol)])
             for _pol in base_sim.data.get_feedpols()
         )
     elif pol is not None and ant1 is None:
         assert all(
-            np.all(gains[(ant, pol)] == _gains[(ant, pol)]) for ant in base_sim.antpos
+            np.allclose(gains[(ant, pol)], _gains[(ant, pol)])
+            for ant in base_sim.antpos
         )
     else:
-        assert all(np.all(gains[antpol] == _gains[antpol]) for antpol in gains)
+        assert all(np.allclose(gains[antpol], _gains[antpol]) for antpol in gains)
 
 
 def test_not_add_vis(base_sim):
     vis = base_sim.add("noiselike_eor", add_vis=False, ret_vis=True)
 
     assert np.all(base_sim.data.data_array == 0)
 
@@ -414,42 +415,40 @@
     assert not np.all(np.isclose(sim.data.data_array, 0))
 
     # instantiate a mock simulation file
     tmp_sim_file = tempfile.mkstemp()[1]
     # write something to it
     with open(tmp_sim_file, "w") as sim_file:
         sim_file.write(
-            """
+            f"""
             diffuse_foreground:
                 Tsky_mdl: !Tsky
-                    datafile: {}/HERA_Tsky_Reformatted.npz
+                    datafile: {DATA_PATH}/HERA_Tsky_Reformatted.npz
                     pol: yy
             pntsrc_foreground:
                 nsrcs: 500
                 Smin: 0.1
             noiselike_eor:
                 eor_amp: 0.03
             gains:
                 gain_spread: 0.05
             cross_coupling_xtalk:
                 amp: 0.225
                 dly: 13.2
                 phs: 2.1123
             thermal_noise:
                 Tsky_mdl: !Tsky
-                    datafile: {}/HERA_Tsky_Reformatted.npz
+                    datafile: {DATA_PATH}/HERA_Tsky_Reformatted.npz
                     pol: xx
                 integration_time: 9.72
             rfi_scatter:
                 scatter_chance: 0.99
                 scatter_strength: 5.7
                 scatter_std: 2.2
-                """.format(
-                DATA_PATH, DATA_PATH
-            )
+                """
         )
     sim = create_sim(autos=True)
     sim.run_sim(tmp_sim_file)
     assert not np.all(np.isclose(sim.data.data_array, 0))
 
     # deactivate season defaults for good measure
     defaults.deactivate()
@@ -700,7 +699,53 @@
     )
     seed = 1420
     sim2.calculate_filters(**kwargs)
     sim1.add("diffuse_foreground", seed=seed, **kwargs)
     sim2.add("diffuse_foreground", seed=seed)
     defaults.deactivate()
     assert np.allclose(sim1.data.data_array, sim2.data.data_array)
+
+
+def test_get_model_name():
+    assert Simulator._get_model_name("noiselike_eor") == "noiselike_eor"
+    assert Simulator._get_model_name("NOISELIKE_EOR") == "noiselike_eor"
+
+    assert Simulator._get_model_name(DiffuseForeground) == "diffuseforeground"
+    assert Simulator._get_model_name(diffuse_foreground) == "diffuseforeground"
+
+    with pytest.raises(
+        TypeError, match="You are trying to simulate an effect using a custom function"
+    ):
+        Simulator._get_model_name(lambda x: x)
+
+    with pytest.raises(
+        TypeError, match="You are trying to simulate an effect using a custom function"
+    ):
+        Simulator._get_model_name(3)
+
+
+def test_parse_key(base_sim: Simulator):
+    assert base_sim._parse_key(None) == (None, None, None)
+    assert base_sim._parse_key(1) == (1, None, None)
+    assert base_sim._parse_key(
+        base_sim.data.baseline_array[-1]
+    ) == base_sim.data.baseline_to_antnums(base_sim.data.baseline_array[-1]) + (None,)
+
+    with pytest.raises(NotImplementedError, match="Functionality not yet supported"):
+        base_sim._parse_key("auto")
+
+    assert base_sim._parse_key("ee") == (None, None, "ee")
+
+    for badkey in [3.14, [1, 2, 3], (1,)]:
+        print(badkey)
+        with pytest.raises(
+            ValueError,
+            match="Key must be an integer, string, antenna pair, or antenna pair with",
+        ):
+            base_sim._parse_key(badkey)
+
+    with pytest.raises(ValueError, match="Invalid polarization string"):
+        base_sim._parse_key("bad_pol")
+
+    assert base_sim._parse_key((1, 2)) == (1, 2, None)
+    assert base_sim._parse_key((1, "Jee")) == (1, None, "Jee")
+    assert base_sim._parse_key((1, 2, "ee")) == (1, 2, "ee")
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_utils.py` & `hera_sim-4.2.2/hera_sim/tests/test_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,15 @@
     filt_data = getattr(utils, f"rough_{filter_type}_filter")(data, **kwargs)
     assert np.allclose(data, filt_data)
 
 
 @pytest.mark.parametrize("shape", [100, (100, 200)])
 def test_gen_white_noise_shape(shape):
     noise = utils.gen_white_noise(shape)
-    if type(shape) is int:
+    if isinstance(shape, int):
         shape = (shape,)
     assert noise.shape == shape
 
 
 @pytest.mark.parametrize("shape", [100, (100, 200)])
 def test_gen_white_noise_mean(shape):
     noise = utils.gen_white_noise(shape)
@@ -380,15 +380,15 @@
 
     conversion_factors = utils.jansky_to_kelvin(freqs, omega_p)
     assert conversion_factors.shape == freqs.shape
 
 
 @pytest.mark.parametrize("obj", [1, (1, 2), "abc", np.array([13])])
 def test_listify(obj):
-    assert type(utils._listify(obj)) is list
+    assert isinstance(utils._listify(obj), list)
 
 
 @pytest.mark.parametrize("jit", [True, False])
 @pytest.mark.parametrize(
     "pols",
     [
         sorted(pols)[::-1]
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_vis.py` & `hera_sim-4.2.2/hera_sim/tests/test_vis.py`

 * *Files 2% similar despite different names*

```diff
@@ -626,7 +626,19 @@
 
 def test_bad_load(tmpdir):
     with open(tmpdir / "bad_sim.yaml", "w") as fl:
         fl.write("""simulator: nonexistent\n""")
 
     with pytest.raises(AttributeError, match="The given simulator"):
         load_simulator_from_yaml(tmpdir / "bad_sim.yaml")
+
+    with open(tmpdir / "bad_sim.yaml", "w") as fl:
+        fl.write("""simulator: hera_sim.foregrounds.DiffuseForeground\n""")
+
+    with pytest.raises(ValueError, match="is not a subclass of VisibilitySimulator"):
+        load_simulator_from_yaml(tmpdir / "bad_sim.yaml")
+
+    with open(tmpdir / "bad_sim.yaml", "w") as fl:
+        fl.write("""simulator: hera_sim.foregrounds.diffuse_foreground\n""")
+
+    with pytest.raises(TypeError, match="is not a class"):
+        load_simulator_from_yaml(tmpdir / "bad_sim.yaml")
```

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_vis_cli.py` & `hera_sim-4.2.2/hera_sim/tests/test_vis_cli.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/test_yaml_constructors.py` & `hera_sim-4.2.2/hera_sim/tests/test_yaml_constructors.py`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv` & `hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/H4C-antennas-slim.csv`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits` & `hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/NF_HERA_Dipole_small.fits`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot` & `hera_sim-4.2.2/hera_sim/tests/testdata/hera-sim-vis-config/gleam_50srcs.vot`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim/utils.py` & `hera_sim-4.2.2/hera_sim/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utility module."""
+
 from __future__ import annotations
 
 import numpy as np
 import pyuvdata.utils as uvutils
 import warnings
 from astropy import constants, units
 from astropy.coordinates import Longitude
```

### Comparing `hera_sim-4.2.1/hera_sim/vis.py` & `hera_sim-4.2.2/hera_sim/vis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions for producing white-noise redundant visibilities."""
+
 import numpy as np
 from copy import deepcopy
 
 from . import noise
 
 DEFAULT_LSTS = np.linspace(0, 2 * np.pi, 10000, endpoint=False)
 DEFAULT_FQS = np.linspace(0.1, 0.2, 1024, endpoint=False)
```

### Comparing `hera_sim-4.2.1/hera_sim/visibilities/__init__.py` & `hera_sim-4.2.2/hera_sim/visibilities/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 The focus is on simulating visibilities from a known sky-locked signal. These
 include simulators of varying levels of accuracy and performance capabilities,
 as well as varying expected input types -- eg. floating point sources,
 temperature fields, rectilinear co-ordinates, spherical co-ordinates, healpix
 maps etc. This package intends to unify the interfaces of these various kinds
 of simulators.
 """
+
 from .pyuvsim_wrapper import UVSim
 from .simulators import (
     ModelData,
     VisibilitySimulation,
     VisibilitySimulator,
     load_simulator_from_yaml,
 )
```

### Comparing `hera_sim-4.2.1/hera_sim/visibilities/cli.py` & `hera_sim-4.2.2/hera_sim/visibilities/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,16 +135,16 @@
         cns.print(f"Largest Beam Array: {max(beam_array_sizes) / 1024**2:.2f} MB")
         cns.print(f"Total Beam Arrays : {sum(beam_array_sizes) / 1024**2:.2f} MB")
 
     ram = simulator.estimate_memory(data_model)
     ram_avail = psutil.virtual_memory().available / 1024**3
 
     cprint(
-        f"[bold {'red' if ram < 1.5*ram_avail else 'green'}] This simulation will use "
-        f"at least {ram:.2f}GB of RAM (Available: {ram_avail:.2f}GB).[/]"
+        f"[bold {'red' if ram < 1.5 * ram_avail else 'green'}] This simulation will use"
+        f" at least {ram:.2f}GB of RAM (Available: {ram_avail:.2f}GB).[/]"
     )
 
     if args.object_name is None:
         data_model.uvdata.object_name = simulator.__class__.__name__
     else:
         data_model.uvdata.object_name = args.object_name
```

### Comparing `hera_sim-4.2.1/hera_sim/visibilities/matvis.py` & `hera_sim-4.2.2/hera_sim/visibilities/matvis.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper for matvis visibility simulator."""
+
 from __future__ import annotations
 
 import astropy.units as u
 import itertools
 import logging
 import numpy as np
 from astropy.coordinates import EarthLocation
@@ -373,15 +374,15 @@
             )
 
         for i, freq in enumerate(data_model.freqs):
             # Divide tasks between MPI workers if needed
             if self.mpi_comm is not None and i % nproc != myid:
                 continue
 
-            logger.info(f"Simulating Frequency {i+1}/{len(data_model.freqs)}")
+            logger.info(f"Simulating Frequency {i + 1}/{len(data_model.freqs)}")
 
             # Call matvis function to simulate visibilities
             vis = self._matvis(
                 antpos=active_antpos,
                 freq=freq,
                 eq2tops=eq2tops,
                 crd_eq=crd_eq,
```

### Comparing `hera_sim-4.2.1/hera_sim/visibilities/pyuvsim_wrapper.py` & `hera_sim-4.2.2/hera_sim/visibilities/pyuvsim_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Wrapper for the pyuvsim simulator."""
+
 import numpy as np
 import pyuvsim
 import warnings
 
 from .simulators import ModelData, VisibilitySimulator
```

### Comparing `hera_sim-4.2.1/hera_sim/visibilities/simulators.py` & `hera_sim-4.2.2/hera_sim/visibilities/simulators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Module defining a high-level visibility simulator wrapper."""
+
 from __future__ import annotations
 
 import astropy_healpix as aph
 import importlib
 import logging
 import numpy as np
 import yaml
@@ -489,15 +490,17 @@
                 f"The given simulator {simulator_cls!r} is not available in hera_sim."
             )
     else:  # pragma: nocover
         module = ".".join(simulator_cls.split(".")[:-1])
         module = importlib.import_module(module)
         simulator_cls = getattr(module, simulator_cls.split(".")[-1])
 
-    if not issubclass(simulator_cls, VisibilitySimulator):
-        raise TypeError(
-            f"Specified simulator {simulator_cls} is not a subclass of"
-            "VisibilitySimulator!"
-        )
+    try:
+        if not issubclass(simulator_cls, VisibilitySimulator):
+            raise ValueError(
+                f"Specified simulator {simulator_cls} is not a subclass of "
+                "VisibilitySimulator!"
+            )
+    except TypeError as e:
+        raise TypeError(f"Specified simulator {simulator_cls} is not a class!") from e
 
-    assert issubclass(simulator_cls, VisibilitySimulator)
     return simulator_cls.from_yaml(cfg)
```

### Comparing `hera_sim-4.2.1/hera_sim.egg-info/PKG-INFO` & `hera_sim-4.2.2/hera_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hera_sim
-Version: 4.2.1
+Version: 4.2.2
 Summary: A collection of simulation routines describing the HERA instrument.
 Home-page: https://github.com/HERA-Team/hera_sim
 Author: HERA Team
 Author-email: steven.g.murray@asu.edu
 License: MIT
 Project-URL: Documentation, https://hera_sim.readthedocs.org
 Platform: any
```

### Comparing `hera_sim-4.2.1/hera_sim.egg-info/SOURCES.txt` & `hera_sim-4.2.2/hera_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/hera_sim.egg-info/requires.txt` & `hera_sim-4.2.2/hera_sim.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hera_sim-4.2.1/scripts/hera-sim-simulate.py` & `hera_sim-4.2.2/scripts/hera-sim-simulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             # BDA will modify the time structure of the data, so we'll need to
             # apply it to each component prior to saving.
             this_sim = copy.deepcopy(sim)
             if type(data) is np.ndarray:
                 this_sim.data.data_array = data
             if bda_params:
                 this_sim.data = bda_tools.apply_bda(this_sim.data, **bda_params)
-            if type(data) is dict:
+            if isinstance(data, dict):
                 # The component is a gain-like term, so save as a calfits file.
                 ext = os.path.splitext(filename)[1]
                 if ext == "":
                     filename += ".calfits"
                 else:
                     filename = filename.replace(ext, ".calfits")
                 # XXX when time-varying gains are supported, we'll need special
```

### Comparing `hera_sim-4.2.1/setup.cfg` & `hera_sim-4.2.2/setup.cfg`

 * *Files identical despite different names*

