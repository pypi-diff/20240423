# Comparing `tmp/aiida_quantumespresso-4.5.1.tar.gz` & `tmp/aiida_quantumespresso-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida_quantumespresso-4.5.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiida_quantumespresso-4.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiida_quantumespresso-4.5.1.tar` & `aiida_quantumespresso-4.6.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0      148 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/config/code-ph.yaml
--rw-r--r--   0        0        0      148 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/config/code-pw.yaml
--rw-r--r--   0        0        0       43 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/config/localhost-config.yaml
--rw-r--r--   0        0        0      234 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/config/localhost-setup.yaml
--rw-r--r--   0        0        0      215 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/config/profile.yaml
--rw-r--r--   0        0        0     1922 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/scripts/run_documentation_scripts.py
--rw-r--r--   0        0        0     3009 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4135 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2284 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     2497 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/workflows/update_changelog.py
--rw-r--r--   0        0        0     1520 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0     1286 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.gitignore
--rw-r--r--   0        0        0     1347 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      277 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/.readthedocs.yml
--rw-r--r--   0        0        0    49491 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1273 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/LICENSE.txt
--rw-r--r--   0        0        0    33074 2024-02-13 10:43:22.446543 aiida_quantumespresso-4.5.1/README.md
--rw-r--r--   0        0        0     8635 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/pyproject.toml
--rw-r--r--   0        0        0      100 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/__init__.py
--rw-r--r--   0        0        0    38896 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/__init__.py
--rw-r--r--   0        0        0     2017 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/base.py
--rw-r--r--   0        0        0     6243 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/cp.py
--rw-r--r--   0        0        0     1245 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/dos.py
--rw-r--r--   0        0        0    14015 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/epw.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/__init__.py
--rw-r--r--   0        0        0     1595 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0     5461 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/create_magnetic_configuration.py
--rw-r--r--   0        0        0     1226 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py
--rw-r--r--   0        0        0     1436 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
--rw-r--r--   0        0        0     4593 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
--rw-r--r--   0        0        0     4251 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py
--rw-r--r--   0        0        0     5358 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py
--rw-r--r--   0        0        0     2624 2024-02-13 10:43:22.454543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
--rw-r--r--   0        0        0    84796 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
--rw-r--r--   0        0        0    87073 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
--rw-r--r--   0        0        0    87073 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
--rw-r--r--   0        0        0    83767 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
--rw-r--r--   0        0        0    96224 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
--rw-r--r--   0        0        0    96319 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
--rw-r--r--   0        0        0    93230 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
--rw-r--r--   0        0        0    96763 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
--rw-r--r--   0        0        0    97862 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
--rw-r--r--   0        0        0    97871 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
--rw-r--r--   0        0        0    98698 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
--rw-r--r--   0        0        0   109373 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
--rw-r--r--   0        0        0   110988 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
--rw-r--r--   0        0        0   112295 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
--rw-r--r--   0        0        0   116180 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
--rw-r--r--   0        0        0   118149 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
--rw-r--r--   0        0        0    26623 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/__init__.py
--rw-r--r--   0        0        0     4438 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/matdyn.py
--rw-r--r--   0        0        0    10731 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/namelists.py
--rw-r--r--   0        0        0    16773 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/neb.py
--rw-r--r--   0        0        0     1714 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/open_grid.py
--rw-r--r--   0        0        0    16652 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/ph.py
--rw-r--r--   0        0        0    11511 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pp.py
--rw-r--r--   0        0        0     3549 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/projwfc.py
--rw-r--r--   0        0        0    13586 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw.py
--rw-r--r--   0        0        0     3008 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw2gw.py
--rw-r--r--   0        0        0     2758 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw2wannier90.py
--rw-r--r--   0        0        0    23331 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pwimmigrant.py
--rw-r--r--   0        0        0     1716 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/q2r.py
--rw-r--r--   0        0        0     5746 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/xspectra.py
--rw-r--r--   0        0        0      609 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/__init__.py
--rw-r--r--   0        0        0      874 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/__init__.py
--rw-r--r--   0        0        0     2130 2024-02-13 10:43:22.458543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/cp.py
--rwxr-xr-x   0        0        0     1992 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/dos.py
--rw-r--r--   0        0        0     3530 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/epw.py
--rw-r--r--   0        0        0     1418 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/matdyn.py
--rw-r--r--   0        0        0     3622 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/neb.py
--rw-r--r--   0        0        0     2118 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/ph.py
--rw-r--r--   0        0        0     1981 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pp.py
--rwxr-xr-x   0        0        0     2012 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/projwfc.py
--rw-r--r--   0        0        0     4121 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pw.py
--rwxr-xr-x   0        0        0     3060 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
--rw-r--r--   0        0        0     1794 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/q2r.py
--rw-r--r--   0        0        0      361 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/data/__init__.py
--rw-r--r--   0        0        0     1062 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/data/structure.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/__init__.py
--rw-r--r--   0        0        0     1555 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/defaults.py
--rw-r--r--   0        0        0     1530 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/display.py
--rw-r--r--   0        0        0     1259 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/launch.py
--rw-r--r--   0        0        0     6820 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/options.py
--rw-r--r--   0        0        0     5435 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/validate.py
--rw-r--r--   0        0        0      675 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
--rwxr-xr-x   0        0        0     1666 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
--rwxr-xr-x   0        0        0     1568 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
--rwxr-xr-x   0        0        0     3526 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/bands.py
--rwxr-xr-x   0        0        0     2720 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/base.py
--rwxr-xr-x   0        0        0     3408 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
--rwxr-xr-x   0        0        0     1720 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/q2r/base.py
--rw-r--r--   0        0        0       84 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/common/__init__.py
--rw-r--r--   0        0        0     6155 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/common/hubbard.py
--rw-r--r--   0        0        0     1588 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/common/types.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/data/__init__.py
--rw-r--r--   0        0        0     9253 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/data/force_constants.py
--rw-r--r--   0        0        0     9315 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/data/hubbard_structure.py
--rw-r--r--   0        0        0      202 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/__init__.py
--rw-r--r--   0        0        0     8636 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/base.py
--rw-r--r--   0        0        0    17005 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/cp.py
--rw-r--r--   0        0        0     5089 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/dos.py
--rw-r--r--   0        0        0     4749 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/matdyn.py
--rw-r--r--   0        0        0     9541 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/neb.py
--rw-r--r--   0        0        0     2749 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/open_grid.py
--rw-r--r--   0        0        0       71 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
--rw-r--r--   0        0        0     2686 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/base.py
--rw-r--r--   0        0        0     8569 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/cp.py
--rw-r--r--   0        0        0     6773 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/neb.py
--rw-r--r--   0        0        0    18957 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/ph.py
--rw-r--r--   0        0        0    48436 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/pw.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
--rw-r--r--   0        0        0    17305 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
--rw-r--r--   0        0        0      291 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
--rw-r--r--   0        0        0    21297 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
--rw-r--r--   0        0        0    24260 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/parse.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
--rw-r--r--   0        0        0    16555 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
--rw-r--r--   0        0        0      900 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
--rw-r--r--   0        0        0    39204 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
--rw-r--r--   0        0        0    42964 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
--rw-r--r--   0        0        0    41134 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
--rw-r--r--   0        0        0    41234 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
--rw-r--r--   0        0        0    42964 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
--rw-r--r--   0        0        0    42964 2024-02-13 10:43:22.462543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
--rw-r--r--   0        0        0    49812 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
--rw-r--r--   0        0        0    57907 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
--rw-r--r--   0        0        0    58917 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd
--rw-r--r--   0        0        0     4627 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/versions.py
--rw-r--r--   0        0        0     2684 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/ph.py
--rw-r--r--   0        0        0    13750 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pp.py
--rw-r--r--   0        0        0    19897 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/projwfc.py
--rw-r--r--   0        0        0    29518 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw.py
--rw-r--r--   0        0        0     2882 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw2gw.py
--rw-r--r--   0        0        0     1067 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw2wannier90.py
--rw-r--r--   0        0        0     1369 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/q2r.py
--rw-r--r--   0        0        0    10164 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/xspectra.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/__init__.py
--rw-r--r--   0        0        0     2840 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/base.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/calculations/__init__.py
--rw-r--r--   0        0        0     4288 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/calculations/pw.py
--rw-r--r--   0        0        0     1035 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/cpinputparser.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/orbital/__init__.py
--rw-r--r--   0        0        0     2981 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
--rw-r--r--   0        0        0     5427 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
--rw-r--r--   0        0        0     6586 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/pwinputparser.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/__init__.py
--rw-r--r--   0        0        0     3972 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/bands.py
--rw-r--r--   0        0        0     8343 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/convert.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/defaults/__init__.py
--rw-r--r--   0        0        0      669 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
--rw-r--r--   0        0        0    15049 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/hubbard.py
--rw-r--r--   0        0        0     1032 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/linalg.py
--rw-r--r--   0        0        0     3672 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/mapping.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/__init__.py
--rw-r--r--   0        0        0    10193 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/pw.py
--rw-r--r--   0        0        0    14855 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
--rw-r--r--   0        0        0    15000 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
--rw-r--r--   0        0        0    14831 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
--rw-r--r--   0        0        0    15000 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
--rw-r--r--   0        0        0     3050 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/resources.py
--rw-r--r--   0        0        0     2615 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/restart.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/validation/__init__.py
--rw-r--r--   0        0        0     5337 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/validation/trajectory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/__init__.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/__init__.py
--rw-r--r--   0        0        0      671 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0     2095 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/get_marked_structures.py
--rw-r--r--   0        0        0    15977 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py
--rw-r--r--   0        0        0      665 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/matdyn/__init__.py
--rw-r--r--   0        0        0     2682 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/matdyn/base.py
--rw-r--r--   0        0        0    26217 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pdos.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/ph/__init__.py
--rw-r--r--   0        0        0    16585 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/__init__.py
--rw-r--r--   0        0        0     1125 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
--rw-r--r--   0        0        0     1469 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
--rw-r--r--   0        0        0     1983 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
--rw-r--r--   0        0        0     1045 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
--rw-r--r--   0        0        0     1826 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
--rw-r--r--   0        0        0      840 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
--rw-r--r--   0        0        0     5782 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/utils.py
--rw-r--r--   0        0        0      538 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xps.yaml
--rw-r--r--   0        0        0     1914 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
--rw-r--r--   0        0        0      657 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
--rw-r--r--   0        0        0      599 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.466543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/__init__.py
--rw-r--r--   0        0        0    16378 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/bands.py
--rw-r--r--   0        0        0    34088 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/base.py
--rw-r--r--   0        0        0    18141 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/q2r/__init__.py
--rw-r--r--   0        0        0     2649 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/q2r/base.py
--rw-r--r--   0        0        0    32724 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xps.py
--rw-r--r--   0        0        0        0 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/__init__.py
--rw-r--r--   0        0        0    12916 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/base.py
--rw-r--r--   0        0        0    34631 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/core.py
--rw-r--r--   0        0        0    30310 2024-02-13 10:43:22.470543 aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/crystal.py
--rw-r--r--   0        0        0    35115 1970-01-01 00:00:00.000000 aiida_quantumespresso-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0      148 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/config/code-ph.yaml
+-rw-r--r--   0        0        0      148 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/config/code-pw.yaml
+-rw-r--r--   0        0        0       43 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/config/localhost-config.yaml
+-rw-r--r--   0        0        0      234 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/config/localhost-setup.yaml
+-rw-r--r--   0        0        0      215 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/config/profile.yaml
+-rw-r--r--   0        0        0     1922 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/scripts/run_documentation_scripts.py
+-rw-r--r--   0        0        0     3009 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4135 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2284 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     2497 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/workflows/update_changelog.py
+-rw-r--r--   0        0        0     1520 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0     1286 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.gitignore
+-rw-r--r--   0        0        0     1347 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      277 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/.readthedocs.yml
+-rw-r--r--   0        0        0    51398 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1273 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    33074 2024-04-23 07:36:23.946673 aiida_quantumespresso-4.6.0/README.md
+-rw-r--r--   0        0        0     8635 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/__init__.py
+-rw-r--r--   0        0        0    38896 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/__init__.py
+-rw-r--r--   0        0        0     2017 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/base.py
+-rw-r--r--   0        0        0     6243 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/cp.py
+-rw-r--r--   0        0        0     1245 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/dos.py
+-rw-r--r--   0        0        0    14015 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/epw.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/__init__.py
+-rw-r--r--   0        0        0     1595 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0     5461 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/create_magnetic_configuration.py
+-rw-r--r--   0        0        0     1226 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py
+-rw-r--r--   0        0        0     2654 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
+-rw-r--r--   0        0        0     4593 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
+-rw-r--r--   0        0        0     4251 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py
+-rw-r--r--   0        0        0     5358 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py
+-rw-r--r--   0        0        0     2624 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
+-rw-r--r--   0        0        0    84796 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
+-rw-r--r--   0        0        0    87073 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
+-rw-r--r--   0        0        0    87073 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
+-rw-r--r--   0        0        0    83767 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
+-rw-r--r--   0        0        0    96224 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
+-rw-r--r--   0        0        0    96319 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
+-rw-r--r--   0        0        0    93230 2024-04-23 07:36:23.954673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
+-rw-r--r--   0        0        0    96763 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
+-rw-r--r--   0        0        0    97862 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
+-rw-r--r--   0        0        0    97871 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
+-rw-r--r--   0        0        0    98698 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
+-rw-r--r--   0        0        0   109373 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
+-rw-r--r--   0        0        0   110988 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
+-rw-r--r--   0        0        0   112295 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
+-rw-r--r--   0        0        0   116180 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
+-rw-r--r--   0        0        0   118149 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
+-rw-r--r--   0        0        0    26623 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/__init__.py
+-rw-r--r--   0        0        0     4438 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/matdyn.py
+-rw-r--r--   0        0        0    10731 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/namelists.py
+-rw-r--r--   0        0        0    16773 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/neb.py
+-rw-r--r--   0        0        0     1714 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/open_grid.py
+-rw-r--r--   0        0        0    17160 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/ph.py
+-rw-r--r--   0        0        0    11511 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pp.py
+-rw-r--r--   0        0        0     3549 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/projwfc.py
+-rw-r--r--   0        0        0    13586 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw.py
+-rw-r--r--   0        0        0     3008 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw2gw.py
+-rw-r--r--   0        0        0     2758 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0    23331 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pwimmigrant.py
+-rw-r--r--   0        0        0     1716 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/q2r.py
+-rw-r--r--   0        0        0     5746 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/xspectra.py
+-rw-r--r--   0        0        0      609 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/__init__.py
+-rw-r--r--   0        0        0      874 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/__init__.py
+-rw-r--r--   0        0        0     2130 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/cp.py
+-rwxr-xr-x   0        0        0     1992 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/dos.py
+-rw-r--r--   0        0        0     3530 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/epw.py
+-rw-r--r--   0        0        0     1418 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/matdyn.py
+-rw-r--r--   0        0        0     3622 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/neb.py
+-rw-r--r--   0        0        0     2118 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/ph.py
+-rw-r--r--   0        0        0     1981 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pp.py
+-rwxr-xr-x   0        0        0     2012 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/projwfc.py
+-rw-r--r--   0        0        0     4121 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pw.py
+-rwxr-xr-x   0        0        0     3060 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0     1794 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/q2r.py
+-rw-r--r--   0        0        0      361 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/data/__init__.py
+-rw-r--r--   0        0        0      994 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/data/structure.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1555 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/defaults.py
+-rw-r--r--   0        0        0     1530 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/display.py
+-rw-r--r--   0        0        0     1259 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/launch.py
+-rw-r--r--   0        0        0     6820 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/options.py
+-rw-r--r--   0        0        0     5435 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/validate.py
+-rw-r--r--   0        0        0      675 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
+-rwxr-xr-x   0        0        0     1666 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
+-rwxr-xr-x   0        0        0     1568 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
+-rwxr-xr-x   0        0        0     3526 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py
+-rwxr-xr-x   0        0        0     2720 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/base.py
+-rwxr-xr-x   0        0        0     3408 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.958673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
+-rwxr-xr-x   0        0        0     1720 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py
+-rw-r--r--   0        0        0       84 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/common/__init__.py
+-rw-r--r--   0        0        0     6155 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/common/hubbard.py
+-rw-r--r--   0        0        0     1588 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/common/types.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/data/__init__.py
+-rw-r--r--   0        0        0     9253 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/data/force_constants.py
+-rw-r--r--   0        0        0     9855 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/data/hubbard_structure.py
+-rw-r--r--   0        0        0      202 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/__init__.py
+-rw-r--r--   0        0        0     8636 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/base.py
+-rw-r--r--   0        0        0    17005 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/cp.py
+-rw-r--r--   0        0        0     5089 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/dos.py
+-rw-r--r--   0        0        0     4749 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/matdyn.py
+-rw-r--r--   0        0        0     9541 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/neb.py
+-rw-r--r--   0        0        0     2749 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/open_grid.py
+-rw-r--r--   0        0        0       71 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
+-rw-r--r--   0        0        0     2686 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/base.py
+-rw-r--r--   0        0        0     8569 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py
+-rw-r--r--   0        0        0     6773 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py
+-rw-r--r--   0        0        0    18957 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py
+-rw-r--r--   0        0        0    48436 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
+-rw-r--r--   0        0        0    17305 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
+-rw-r--r--   0        0        0      291 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
+-rw-r--r--   0        0        0    21297 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
+-rw-r--r--   0        0        0    24260 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
+-rw-r--r--   0        0        0    16555 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
+-rw-r--r--   0        0        0      900 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
+-rw-r--r--   0        0        0    39204 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
+-rw-r--r--   0        0        0    42964 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
+-rw-r--r--   0        0        0    41134 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
+-rw-r--r--   0        0        0    41234 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
+-rw-r--r--   0        0        0    42964 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
+-rw-r--r--   0        0        0    42964 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
+-rw-r--r--   0        0        0    49812 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
+-rw-r--r--   0        0        0    57907 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
+-rw-r--r--   0        0        0    58917 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd
+-rw-r--r--   0        0        0     4627 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py
+-rw-r--r--   0        0        0     2824 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/ph.py
+-rw-r--r--   0        0        0    13750 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pp.py
+-rw-r--r--   0        0        0    19897 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/projwfc.py
+-rw-r--r--   0        0        0    29518 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw.py
+-rw-r--r--   0        0        0     2882 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw2gw.py
+-rw-r--r--   0        0        0     1067 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw2wannier90.py
+-rw-r--r--   0        0        0     1369 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/q2r.py
+-rw-r--r--   0        0        0    10164 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/xspectra.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/__init__.py
+-rw-r--r--   0        0        0     2840 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/base.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/calculations/__init__.py
+-rw-r--r--   0        0        0     4288 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/calculations/pw.py
+-rw-r--r--   0        0        0     1035 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/cpinputparser.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.962673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/orbital/__init__.py
+-rw-r--r--   0        0        0     2981 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
+-rw-r--r--   0        0        0     5427 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
+-rw-r--r--   0        0        0     6586 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/pwinputparser.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/__init__.py
+-rw-r--r--   0        0        0     3972 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/bands.py
+-rw-r--r--   0        0        0     8343 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/convert.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/defaults/__init__.py
+-rw-r--r--   0        0        0      669 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
+-rw-r--r--   0        0        0    15049 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/hubbard.py
+-rw-r--r--   0        0        0     1032 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/linalg.py
+-rw-r--r--   0        0        0     3672 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/mapping.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/__init__.py
+-rw-r--r--   0        0        0    10193 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/pw.py
+-rw-r--r--   0        0        0    14855 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
+-rw-r--r--   0        0        0    15000 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
+-rw-r--r--   0        0        0    14831 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
+-rw-r--r--   0        0        0    15000 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
+-rw-r--r--   0        0        0     3050 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/resources.py
+-rw-r--r--   0        0        0     2615 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/restart.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/validation/__init__.py
+-rw-r--r--   0        0        0     5337 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/validation/trajectory.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0     2095 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/get_marked_structures.py
+-rw-r--r--   0        0        0    21746 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py
+-rw-r--r--   0        0        0      665 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/matdyn/__init__.py
+-rw-r--r--   0        0        0     2682 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/matdyn/base.py
+-rw-r--r--   0        0        0    26217 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pdos.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/ph/__init__.py
+-rw-r--r--   0        0        0    16585 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/__init__.py
+-rw-r--r--   0        0        0     1125 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
+-rw-r--r--   0        0        0     1469 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
+-rw-r--r--   0        0        0     1983 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
+-rw-r--r--   0        0        0     1071 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
+-rw-r--r--   0        0        0     1045 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
+-rw-r--r--   0        0        0     1826 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
+-rw-r--r--   0        0        0      840 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
+-rw-r--r--   0        0        0     5782 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/utils.py
+-rw-r--r--   0        0        0      538 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml
+-rw-r--r--   0        0        0     1914 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
+-rw-r--r--   0        0        0      657 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
+-rw-r--r--   0        0        0      599 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/__init__.py
+-rw-r--r--   0        0        0    16494 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/bands.py
+-rw-r--r--   0        0        0    34088 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/base.py
+-rw-r--r--   0        0        0    18141 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/q2r/__init__.py
+-rw-r--r--   0        0        0     2649 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/q2r/base.py
+-rw-r--r--   0        0        0    33394 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xps.py
+-rw-r--r--   0        0        0        0 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/__init__.py
+-rw-r--r--   0        0        0    12916 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/base.py
+-rw-r--r--   0        0        0    35080 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/core.py
+-rw-r--r--   0        0        0    32785 2024-04-23 07:36:23.966673 aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py
+-rw-r--r--   0        0        0    35115 1970-01-01 00:00:00.000000 aiida_quantumespresso-4.6.0/PKG-INFO
```

### Comparing `aiida_quantumespresso-4.5.1/.github/scripts/run_documentation_scripts.py` & `aiida_quantumespresso-4.6.0/.github/scripts/run_documentation_scripts.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.github/workflows/cd.yml` & `aiida_quantumespresso-4.6.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.github/workflows/ci.yml` & `aiida_quantumespresso-4.6.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.github/workflows/nightly.yml` & `aiida_quantumespresso-4.6.0/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.github/workflows/update_changelog.py` & `aiida_quantumespresso-4.6.0/.github/workflows/update_changelog.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.github/workflows/validate_release_tag.py` & `aiida_quantumespresso-4.6.0/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.gitignore` & `aiida_quantumespresso-4.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/.pre-commit-config.yaml` & `aiida_quantumespresso-4.6.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/CHANGELOG.md` & `aiida_quantumespresso-4.6.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+## v4.6.0
+
+This minor release provides several improvements and bug fixes, mostly related to the `HubbardStructureData` and XPS/XAS calculations.
+
+Since there were no changes in the schema for Quantum ESPRESSO v7.3, versions 4.3 and above of the plugin package should now also fully support the new Quantum ESPRESSO release.
+
+### 👌 Improvements
+
+* XAS: Enable Correct Parsing of Hubbard and Magnetic Data [[f439504](https://github.com/aiidateam/aiida-quantumespresso/commit/f4395048dfb9c74b97a5d38eff99029449816dc0)]
+* `PhCalculation`: add symmetry related exit codes [[5a6529f](https://github.com/aiidateam/aiida-quantumespresso/commit/5a6529f46fa3519f006527c02db3a065f6e5ebaa)]
+* `seekpath_structure_analysis`: `HubbardStructureData` compatibility [[9cb1cfa](https://github.com/aiidateam/aiida-quantumespresso/commit/9cb1cfa8a70d19af7aaa1b624cf17c8babe93f41)]
+* `HubbardStructureData`: add compatibility for <3D structures [[d645069](https://github.com/aiidateam/aiida-quantumespresso/commit/d645069d1d6ac40d6a23e4bbf49b01b51f5bb33c)]
+* `HubbardStructureData`: Add validation on site indices [[960a371](https://github.com/aiidateam/aiida-quantumespresso/commit/960a371d2e7f327a3f5bedb86e21dcb5100c03d1)]
+
+### 🐛 Bug fixes
+
+* `PwBandsWorkChain`: Respect `bands_kpoints` in overrides  [[ae7d248](https://github.com/aiidateam/aiida-quantumespresso/commit/ae7d2484a084ca55dcef4c1ca332b2fb0b478fad)]
+* CLI: Fix import of `StructureData` from QE input file  [[3440623](https://github.com/aiidateam/aiida-quantumespresso/commit/34406230023c3c3715264a7de180a576fd7def48)]
+* Fix inputs for molecules in the XPS calculation  [[b7f17cf](https://github.com/aiidateam/aiida-quantumespresso/commit/b7f17cfaf71e5b07089426a4fbe7ae2ca5317523)]
+
+### 🧪 Tests
+
+* CLI: Add test for data structure import [[5c3c301](https://github.com/aiidateam/aiida-quantumespresso/commit/5c3c3012c36577cc0ca6a4374fd97f2ce3177ebe)]
+
+
 ## v4.5.1
 
 This patch release fixes some issues with the changes introduced in [b9c7517](https://github.com/aiidateam/aiida-quantumespresso/commit/b9c7517744e645a93d4afc9b1999881fc39a0e46) and released in v4.5.0.
 The new approach for setting the q-points was unfortunately broken, which is now fixed in [c353cc2](https://github.com/aiidateam/aiida-quantumespresso/commit/c353cc2e4104352ef9b5490adb53a60da47f293d).
 Moreover, the validation that was added to the top-level inputs of the `PhBaseWorkChain` requires the user to specify either the `qpoints` or `qpoints_distance` input.
 This means that work chains which wrap the `PhBaseWorkChain` but provide the q-points on the fly will have to disable this validation by setting the corresponding validator to `None` in the input spec.
 To avoid this, we have the validator check if one of the `qpoints` or `qpoints_distance` ports are still present in the port namespace.
```

### Comparing `aiida_quantumespresso-4.5.1/LICENSE.txt` & `aiida_quantumespresso-4.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/README.md` & `aiida_quantumespresso-4.6.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 ## Compatibility matrix
 
 The matrix below assumes the user always install the latest patch release of the specified minor version, which is recommended.
 
 | Plugin | AiiDA | Python | Quantum ESPRESSO |
 |-|-|-|-|
-| `v4.3 < v5.0` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.2] |
+| `v4.3 < v5.0` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.3] |
 | `v4.0 < v4.3` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.1] |
 | `v3.5 < v4.0` | ![Compatibility for v3.5][AiiDA v3.5] |  [![PyPI pyversions][Python v3.6-v3.9]](https://pypi.org/project/aiida-quantumespresso/3.5.2/) | ![Quantum ESPRESSO compatibility][QE v6-7] |
 | `v3.4 < v3.5` | ![Compatibility for v3.4][AiiDA v3.4] |  [![PyPI pyversions][Python v3.6-v3.9]](https://pypi.org/project/aiida-quantumespresso/3.4.2/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.3 < v3.4` | ![Compatibility for v3.3][AiiDA v3.3] |  [![PyPI pyversions][Python v3.6-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.3.1/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.1 < v3.3` | ![Compatibility for v3.1][AiiDA v3.1] |  [![PyPI pyversions][Python v3.5-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.2.1/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.0 < v3.1` | ![Compatibility for v3.0][AiiDA v3.0] |  [![PyPI pyversions][Python v2.7-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.0.0/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v2.0 < v3.0` | ![Compatibility for v2.0][AiiDA v2.0] |  [![PyPI pyversions][Python v2.7-v3.8]](https://pypi.org/project/aiida-quantumespresso/2.1.0/) | ![Quantum ESPRESSO compatibility][QE v6] |
@@ -142,8 +142,8 @@
 [Python v3.6-v3.8]: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue
 [Python v3.5-v3.8]: https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue
 [Python v2.7-v3.8]: https://img.shields.io/badge/python-2.7%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue
 
 [QE v6]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.0,<=6.7-007ec6.svg?logo=data:image/png;base64,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
 [QE v6-7]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.0,<=7.0-007ec6.svg?logo=data:image/png;base64,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
 [QE v6.6-7.1]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.1-007ec6.svg?logo=data:image/png;base64,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
-[QE v6.6-7.2]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.2-007ec6.svg?logo=data:image/png;base64,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
+[QE v6.6-7.3]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.3-007ec6.svg?logo=data:image/png;base64,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
```

### Comparing `aiida_quantumespresso-4.5.1/pyproject.toml` & `aiida_quantumespresso-4.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/cp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/cp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/dos.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/dos.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/epw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/epw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/create_magnetic_configuration.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/create_magnetic_configuration.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/helpers/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/matdyn.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/namelists.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/namelists.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/neb.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/neb.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/open_grid.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/open_grid.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/ph.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/ph.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,14 +68,20 @@
             message='The stdout output file could not be read.')
         spec.exit_code(311, 'ERROR_OUTPUT_STDOUT_PARSE',
             message='The stdout output file could not be parsed.')
         spec.exit_code(312, 'ERROR_OUTPUT_STDOUT_INCOMPLETE',
             message='The stdout output file was incomplete probably because the calculation got interrupted.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
+        spec.exit_code(360, 'ERROR_INCOMPATIBLE_FFT_GRID',
+            message='The FFT grid is incompatible with the detected symmetries. Try using the lattice-specific '
+                    '`ibrav` != 0 in the parent `pw.x` calculation.')
+        spec.exit_code(361, 'ERROR_WRONG_REPRESENTATION',
+            message=('The representation found seems to be wrong according to the detected symmetries. '
+                     'Try using the lattice-specific `ibrav` != 0 in the parent `pw.x` calculation.'))
 
         # Significant errors but calculation can be used to restart
         spec.exit_code(400, 'ERROR_OUT_OF_WALLTIME',
             message='The calculation stopped prematurely because it ran out of walltime.')
         spec.exit_code(410, 'ERROR_CONVERGENCE_NOT_REACHED',
             message='The minimization cycle did not reach self-consistency.')
         spec.exit_code(462, 'ERROR_COMPUTING_CHOLESKY',
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/projwfc.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw2gw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw2gw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pw2wannier90.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/pwimmigrant.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/pwimmigrant.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/q2r.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/calculations/xspectra.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/calculations/xspectra.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/cp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/cp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/dos.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/dos.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/epw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/epw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/matdyn.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/neb.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/neb.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/ph.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/ph.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/projwfc.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/calculations/q2r.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/calculations/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/data/structure.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/data/structure.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 @click.argument('filename', type=click.File('r'))
 @options.DRY_RUN()
 @decorators.with_dbenv()
 def cmd_import(filename, dry_run):
     """Import a `StructureData` from a Quantum ESPRESSO input file."""
     from aiida_quantumespresso.tools.pwinputparser import PwInputFile
 
-    with open(filename, 'r', encoding='utf-8') as input_file:
-        parser = PwInputFile(input_file.read())
+    parser = PwInputFile(filename.read())
     structure = parser.get_structuredata()
     formula = structure.get_formula()
 
     if dry_run:
         echo.echo_success(f'parsed structure with formula {formula}')
     else:
         structure.store()
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/defaults.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/display.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/display.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/launch.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/launch.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/options.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/options.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/utils/validate.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/utils/validate.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/matdyn/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/ph/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/ph/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/bands.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/pw/relax.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/cli/workflows/q2r/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/common/hubbard.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/common/hubbard.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/common/types.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/common/types.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/data/force_constants.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/data/force_constants.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/data/hubbard_structure.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/data/hubbard_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 """Data plugin that represents a crystal structure with Hubbard parameters."""
 import json
 from typing import List, Tuple, Union
 
 from aiida.orm import StructureData
 import numpy as np
+from pymatgen.core import Lattice, PeriodicSite
 
 from aiida_quantumespresso.common.hubbard import Hubbard, HubbardParameters
 
 __all__ = ('HubbardStructureData',)
 
 
 class HubbardStructureData(StructureData):
@@ -54,14 +55,15 @@
 
     @property
     def hubbard(self) -> Hubbard:
         """Get the `Hubbard` instance.
 
         :returns: a :class:`~aiida_quantumespresso.common.hubbard.Hubbard` instance.
         """
+        # pylint: disable=not-context-manager
         with self.base.repository.open(self._hubbard_filename, mode='rb') as handle:
             return Hubbard.model_validate_json(json.load(handle))
 
     @hubbard.setter
     def hubbard(self, hubbard: Hubbard):
         """Set the full Hubbard information."""
         if not isinstance(hubbard, Hubbard):
@@ -105,16 +107,27 @@
         :param neighbour_manifold: neighbour manifold (e.g. 3d, 3d-2p)
         :param value: value of the Hubbard parameter, in eV
         :param translation: (3,) list of ints, describing the translation vector
             associated with the neighbour atom, defaults to None
         :param hubbard_type: hubbard type (U, V, J, ...), defaults to 'Ueff'
             (see :class:`~aiida_quantumespresso.common.hubbard.Hubbard` for full allowed values)
         """
-        pymat = self.get_pymatgen_structure()
-        sites = pymat.sites
+        sites = [
+            PeriodicSite(
+                species=site.species,
+                coords=site.coords,
+                lattice=Lattice(self.cell, pbc=self.pbc),
+                coords_are_cartesian=True
+            ) for site in self.get_pymatgen().sites
+        ]
+
+        if any((atom_index > len(sites) - 1, neighbour_index > len(sites) - 1)):
+            raise ValueError(
+                'atom_index and neighbour_index must be within the range of the number of sites in the structure'
+            )
 
         if translation is None:
             _, translation = sites[atom_index].distance_and_image(sites[neighbour_index])
             translation = np.array(translation, dtype=np.int64).tolist()
 
         hp_tuple = (atom_index, atom_manifold, neighbour_index, neighbour_manifold, value, translation, hubbard_type)
         parameters = HubbardParameters.from_tuple(hp_tuple)
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/cp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/cp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/dos.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/dos.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/matdyn.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/neb.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/neb.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/open_grid.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/open_grid.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/cp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/neb.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/ph.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_raw/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/legacy.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/parse.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/parse_xml/versions.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/ph.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/ph.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 
 class PhParser(BaseParser):
     """``Parser`` implementation for the ``PhCalculation`` calculation job class."""
 
     class_error_map = {
         'No convergence has been achieved': 'ERROR_CONVERGENCE_NOT_REACHED',
         'problems computing cholesky': 'ERROR_COMPUTING_CHOLESKY',
+        'FFT grid incompatible with symmetry': 'ERROR_INCOMPATIBLE_FFT_GRID',
+        'wrong representation': 'ERROR_WRONG_REPRESENTATION',
     }
 
     def parse(self, **kwargs):
         """Parse the retrieved files from a ``PhCalculation`` into output nodes."""
         logs = get_logging_container()
 
         stdout, parsed_data, logs = self.parse_stdout_from_retrieved(logs)
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pp.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pp.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/projwfc.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw2gw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw2gw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/pw2wannier90.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/q2r.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/parsers/xspectra.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/parsers/xspectra.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/calculations/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/calculations/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/cpinputparser.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/cpinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/tools/pwinputparser.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/tools/pwinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/bands.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/bands.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/convert.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/convert.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/hubbard.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/hubbard.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/linalg.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/mapping.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/pw.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/pw.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/resources.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/restart.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/restart.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/utils/validation/trajectory.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/utils/validation/trajectory.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/get_marked_structures.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/get_marked_structures.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from aiida.common.constants import elements
 from aiida.engine import calcfunction
 from aiida.orm.nodes.data.structure import Kind, Site, StructureData
 from aiida.tools import spglib_tuple_to_structure, structure_to_spglib_tuple
 import numpy as np
 import spglib
 
+from aiida_quantumespresso.utils.hubbard import HubbardStructureData, HubbardUtils
+
 
 @calcfunction
 def get_xspectra_structures(structure, **kwargs):  # pylint: disable=too-many-statements
     """Read a StructureData object using spglib for its symmetry data and return structures for XSpectra calculations.
 
     Takes an incoming StructureData node and prepares structures suitable for calculation with
     xspectra.x. The basic criteria for a suitable structure is for the cell parameters to be
@@ -41,14 +43,19 @@
         - absorbing_elements_list: a List object defining the list of elements to consider
                                    when producing structures. All elements in the structure
                                    will be considered if no input is given.
         - is_molecule_input: a Bool object to define for the function that the input structure is
                     a molecule and not a periodic solid system. Required in order to instruct
                     the CF to use Pymatgen rather than spglib to determine the symmetry. The
                     CF will assume the structure to be a periodic solid if no input is given.
+        - use_element_types: a Bool object to indicate that symmetry analysis should consider all
+                             sites of the same element to be equal and ignore any special Kind names
+                             from the parent structure. For instance, use_element_types = True would
+                             consider sites for Kinds 'Si' and 'Si1' to be equivalent if both are sites
+                             containing silicon. Defaults to True.
         - spglib_settings: an optional Dict object containing overrides for the symmetry
                             tolerance parameters used by spglib (symmprec, angle_tolerance).
         - pymatgen_settings: an optional Dict object containing overrides for the symmetry
                              tolerance parameters used by Pymatgen when processing molecular
                              systems (tolerance, eigen_tolerance, matrix_tolerance).
 
     :param structure: the StructureData object to be analysed
@@ -85,26 +92,28 @@
         scale_unit_cell = True
     if 'standardize_structure' in unwrapped_kwargs.keys():
         standardize_structure = unwrapped_kwargs['standardize_structure'].value
         unwrapped_kwargs.pop('standardize_structure')
     else:
         standardize_structure = True
     if 'absorbing_elements_list' in unwrapped_kwargs.keys():
-        elements_defined = True
         abs_elements_list = unwrapped_kwargs['absorbing_elements_list'].get_list()
         # confirm that the elements requested are actually in the input structure
         for req_element in abs_elements_list:
             if req_element not in elements_present:
                 raise ValidationError(
                     f'Requested elements {abs_elements_list} do not match those in the given structure:'
                     f' {elements_present}'
                 )
     else:
-        elements_defined = False
-        abs_elements_list = [Kind.symbol for Kind in structure.kinds]
+        abs_elements_list = []
+        for kind in structure.kinds:
+            if kind.symbol not in abs_elements_list:
+                abs_elements_list.append(kind.symbol)
+
     if 'is_molecule_input' in unwrapped_kwargs.keys():
         is_molecule_input = unwrapped_kwargs['is_molecule_input'].value
         # If we are working with a molecule, check for pymatgen_settings
         if 'pymatgen_settings' in unwrapped_kwargs.keys():
             pymatgen_settings_dict = unwrapped_kwargs.keys()['pymatgen_settings'].get_dict()
             valid_keys = ['tolerance', 'eigen_tolerance', 'matrix_tolerance']
             pymatgen_kwargs = {key: value for key, value in pymatgen_settings_dict.items() if key in valid_keys}
@@ -114,14 +123,29 @@
     if 'spglib_settings' in unwrapped_kwargs.keys():
         spglib_settings_dict = unwrapped_kwargs['spglib_settings'].get_dict()
         valid_keys = ['symprec', 'angle_tolerance']
         spglib_kwargs = {key: value for key, value in spglib_settings_dict.items() if key in valid_keys}
     else:
         spglib_kwargs = {}
 
+    if 'use_element_types' in unwrapped_kwargs.keys():
+        use_element_types = unwrapped_kwargs['use_element_types'].value
+    else:
+        use_element_types = True
+
+    if isinstance(structure, HubbardStructureData):
+        is_hubbard_structure = True
+        if standardize_structure:
+            raise ValidationError(
+                'Incoming structure set to be standardized, but hubbard data has been found. '
+                'Please set ``standardize_structure`` to false in ``**kwargs`` to preserve the hubbard data.'
+            )
+    else:
+        is_hubbard_structure = False
+
     output_params = {}
     result = {}
 
     output_params['absorbing_elements_list'] = abs_elements_list
 
     incoming_structure_size = len(structure.sites)
     incoming_structure_cell = structure.cell
@@ -199,64 +223,108 @@
         output_params['supercell_cell_lengths'] = new_supercell.cell_lengths
         output_params['supercell_num_sites'] = len(new_supercell.sites)
         result['supercell'] = new_supercell
 
     # Process a periodic system
     else:
         incoming_structure_tuple = structure_to_spglib_tuple(structure)
-
-        symmetry_dataset = spglib.get_symmetry_dataset(incoming_structure_tuple[0], **spglib_kwargs)
+        spglib_tuple = incoming_structure_tuple[0]
+        types_order = spglib_tuple[-1]
+        kinds_information = incoming_structure_tuple[1]
+        kinds_list = incoming_structure_tuple[2]
+
+        # We need a way to reliably convert type number into element, so we
+        # first create a mapping of assigned number to kind name then a mapping
+        # of assigned number to ``Kind``
+
+        type_name_mapping = {str(value): key for key, value in kinds_information.items()}
+        type_mapping_dict = {}
+
+        for key, value in type_name_mapping.items():
+            for kind in kinds_list:
+                if value == kind.name:
+                    type_mapping_dict[key] = kind
+
+        # By default, `structure_to_spglib_tuple` gives different
+        # ``Kinds`` of the same element a distinct atomic number by
+        # multiplying the normal atomic number by 1000, then adding
+        # 100 for each distinct duplicate. if we want to treat all sites
+        # of the same element as equal, then we must therefore briefly
+        # operate on a "cleaned" version of the structure tuple where this
+        # new label is reduced to its normal element number.
+        if use_element_types:
+            cleaned_structure_tuple = (spglib_tuple[0], spglib_tuple[1], [])
+            for i in spglib_tuple[2]:
+                if i >= 1000:
+                    new_i = int(np.trunc(i / 1000))
+                else:
+                    new_i = i
+                cleaned_structure_tuple[2].append(new_i)
+            symmetry_dataset = spglib.get_symmetry_dataset(cleaned_structure_tuple, **spglib_kwargs)
+        else:
+            symmetry_dataset = spglib.get_symmetry_dataset(spglib_tuple, **spglib_kwargs)
 
         # if there is no symmetry to exploit, or no standardization is desired, then we just use
         # the input structure in the following steps. This is done to account for the case where
         # the user has submitted an improper crystal for calculation work and doesn't want it to
         # be changed.
         if symmetry_dataset['number'] in [1, 2] or not standardize_structure:
-            standardized_structure_node = spglib_tuple_to_structure(incoming_structure_tuple[0])
+            standardized_structure_node = spglib_tuple_to_structure(spglib_tuple, kinds_information, kinds_list)
             structure_is_standardized = False
         else:  # otherwise, we proceed with the standardized structure.
-            standardized_structure_tuple = spglib.standardize_cell(incoming_structure_tuple[0], **spglib_kwargs)
-            standardized_structure_node = spglib_tuple_to_structure(standardized_structure_tuple)
+            standardized_structure_tuple = spglib.standardize_cell(spglib_tuple, **spglib_kwargs)
+            standardized_structure_node = spglib_tuple_to_structure(
+                standardized_structure_tuple, kinds_information, kinds_list
+            )
             # if we are standardizing the structure, then we need to update the symmetry
             # information for the standardized structure
             symmetry_dataset = spglib.get_symmetry_dataset(standardized_structure_tuple, **spglib_kwargs)
             structure_is_standardized = True
 
         equivalent_atoms_array = symmetry_dataset['equivalent_atoms']
-        element_types = symmetry_dataset['std_types']
+
+        if structure_is_standardized:
+            element_types = symmetry_dataset['std_types']
+        else:  # convert the 'std_types' from standardized to primitive cell
+            # we generate the type-specific data on-the-fly since we need to
+            # know which type (and thus kind) *should* be at each site
+            # even if we "cleaned" the structure previously
+            non_cleaned_dataset = spglib.get_symmetry_dataset(spglib_tuple, **spglib_kwargs)
+            spglib_std_types = non_cleaned_dataset['std_types']
+            spglib_map_to_prim = non_cleaned_dataset['mapping_to_primitive']
+            spglib_std_map_to_prim = non_cleaned_dataset['std_mapping_to_primitive']
+
+            map_std_pos_to_type = {}
+            for position, atom_type in zip(spglib_std_map_to_prim, spglib_std_types):
+                map_std_pos_to_type[str(position)] = atom_type
+            primitive_types = []
+            for position in spglib_map_to_prim:
+                atom_type = map_std_pos_to_type[str(position)]
+                primitive_types.append(atom_type)
+            element_types = primitive_types
 
         equivalency_dict = {}
-        index_counter = 0
-        for symmetry_value, element_type in zip(equivalent_atoms_array, element_types):
-            if elements_defined:  # only process the elements given in the list
-                if f'site_{symmetry_value}' in equivalency_dict:
-                    equivalency_dict[f'site_{symmetry_value}']['equivalent_sites_list'].append(index_counter)
-                elif elements[element_type]['symbol'] not in abs_elements_list:
-                    pass
-                else:
-                    equivalency_dict[f'site_{symmetry_value}'] = {
-                        'symbol': elements[element_type]['symbol'],
-                        'site_index': symmetry_value,
-                        'equivalent_sites_list': [symmetry_value]
-                    }
-            else:  # process everything in the system
+        for index, symmetry_types in enumerate(zip(equivalent_atoms_array, element_types)):
+            symmetry_value, element_type = symmetry_types
+            if type_mapping_dict[str(element_type)].symbol in abs_elements_list:
                 if f'site_{symmetry_value}' in equivalency_dict:
-                    equivalency_dict[f'site_{symmetry_value}']['equivalent_sites_list'].append(index_counter)
+                    equivalency_dict[f'site_{symmetry_value}']['equivalent_sites_list'].append(index)
                 else:
                     equivalency_dict[f'site_{symmetry_value}'] = {
-                        'symbol': elements[element_type]['symbol'],
+                        'kind_name': type_mapping_dict[str(element_type)].name,
+                        'symbol': type_mapping_dict[str(element_type)].symbol,
                         'site_index': symmetry_value,
                         'equivalent_sites_list': [symmetry_value]
                     }
-            index_counter += 1
 
         for value in equivalency_dict.values():
             value['multiplicity'] = len(value['equivalent_sites_list'])
 
         output_params['equivalent_sites_data'] = equivalency_dict
+
         output_params['spacegroup_number'] = symmetry_dataset['number']
         output_params['international_symbol'] = symmetry_dataset['international']
 
         output_params['structure_is_standardized'] = structure_is_standardized
         if structure_is_standardized:
             result['standardized_structure'] = standardized_structure_node
             output_params['standardized_structure_num_sites'] = len(standardized_structure_node.sites)
@@ -270,39 +338,78 @@
             multiples = []
             for length in standard_pbc:
                 multiple = np.ceil(supercell_min_parameter / length)
                 multiples.append(int(multiple))
 
         ase_structure = standardized_structure_node.get_ase()
         ase_supercell = ase_structure * multiples
-        new_supercell = StructureData(ase=ase_supercell)
 
-        result['supercell'] = new_supercell
+        # if there are hubbard data to apply, we re-construct
+        # the supercell site-by-site to keep the correct ordering
+        if is_hubbard_structure:
+            blank_supercell = StructureData(ase=ase_supercell)
+            new_supercell = StructureData()
+            new_supercell.set_cell(blank_supercell.cell)
+            num_extensions = np.product(multiples)
+            supercell_types_order = []
+            # For each supercell extension, loop over each site.
+            # This way, the original pattern-ordering of sites is
+            # preserved.
+            for i in range(0, num_extensions):  # pylint: disable=unused-variable
+                for type_number in types_order:
+                    supercell_types_order.append(type_number)
+
+            for site, type_number in zip(blank_supercell.sites, supercell_types_order):
+                kind_present = type_mapping_dict[str(type_number)]
+                if kind_present.name not in [kind.name for kind in new_supercell.kinds]:
+                    new_supercell.append_kind(kind_present)
+                new_site = Site(kind_name=kind_present.name, position=site.position)
+                new_supercell.append_site(new_site)
+        else:  # otherwise, simply re-construct the supercell with ASE
+            new_supercell = StructureData(ase=ase_supercell)
+
+        if is_hubbard_structure:  # Scale up the hubbard parameters to match and return the HubbardStructureData
+            # we can exploit the fact that `get_hubbard_for_supercell` will return a HubbardStructureData node
+            # with the same hubbard parameters in the case where the input structure and the supercell are the
+            # same (i.e. multiples == [1, 1, 1])
+            hubbard_manip = HubbardUtils(structure)
+            new_hubbard_supercell = hubbard_manip.get_hubbard_for_supercell(new_supercell)
+            new_supercell = new_hubbard_supercell
+            supercell_hubbard_params = new_supercell.hubbard
+            result['supercell'] = new_supercell
+        else:
+            result['supercell'] = new_supercell
         output_params['supercell_factors'] = multiples
         output_params['supercell_num_sites'] = len(new_supercell.sites)
         output_params['supercell_cell_matrix'] = new_supercell.cell
         output_params['supercell_cell_lengths'] = new_supercell.cell_lengths
 
     for value in equivalency_dict.values():
         target_site = value['site_index']
         marked_structure = StructureData()
-        supercell_kinds = {kind.name: kind for kind in new_supercell.kinds}
         marked_structure.set_cell(new_supercell.cell)
+        new_kind_names = [kind.name for kind in new_supercell.kinds]
 
         for index, site in enumerate(new_supercell.sites):
+            kind_at_position = new_supercell.kinds[new_kind_names.index(site.kind_name)]
             if index == target_site:
-                absorbing_kind = Kind(name=abs_atom_marker, symbols=site.kind_name)
+                absorbing_kind = Kind(name=abs_atom_marker, symbols=kind_at_position.symbol)
                 absorbing_site = Site(kind_name=absorbing_kind.name, position=site.position)
                 marked_structure.append_kind(absorbing_kind)
                 marked_structure.append_site(absorbing_site)
             else:
-                if site.kind_name not in [kind.name for kind in marked_structure.kinds]:
-                    marked_structure.append_kind(supercell_kinds[site.kind_name])
+                if kind_at_position.name not in [kind.name for kind in marked_structure.kinds]:
+                    marked_structure.append_kind(kind_at_position)
                 new_site = Site(kind_name=site.kind_name, position=site.position)
                 marked_structure.append_site(new_site)
 
-        result[f'site_{target_site}_{value["symbol"]}'] = marked_structure
+        if is_hubbard_structure:
+            marked_hubbard_structure = HubbardStructureData.from_structure(marked_structure)
+            marked_hubbard_structure.hubbard = supercell_hubbard_params
+            result[f'site_{target_site}_{value["symbol"]}'] = marked_hubbard_structure
+        else:
+            result[f'site_{target_site}_{value["symbol"]}'] = marked_structure
 
     output_params['is_molecule_input'] = is_molecule_input
     result['output_parameters'] = orm.Dict(dict=output_params)
 
     return result
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/matdyn/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pdos.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pdos.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/ph/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/ph/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pdos.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/utils.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xps.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/bands.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/bands.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,15 +159,18 @@
         builder = cls.get_builder()
         builder.structure = structure
         builder.relax = relax
         builder.scf = scf
         builder.bands = bands
         builder.clean_workdir = orm.Bool(inputs['clean_workdir'])
         builder.nbands_factor = orm.Float(inputs['nbands_factor'])
-        builder.bands_kpoints_distance = orm.Float(inputs['bands_kpoints_distance'])
+        if 'bands_kpoints' in inputs:
+            builder.bands_kpoints = inputs['bands_kpoints']
+        else:
+            builder.bands_kpoints_distance = orm.Float(inputs['bands_kpoints_distance'])
 
         return builder
 
     def setup(self):
         """Define the current structure in the context to be the input structure."""
         self.ctx.current_structure = self.inputs.structure
         self.ctx.current_number_of_bands = None
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/pw/relax.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/pw/relax.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/q2r/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xps.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xps.py`

 * *Files 2% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         return files(protocols) / 'core_hole_treatments.yaml'
 
     @classmethod
     def get_builder_from_protocol(
         cls, code, structure, pseudos, core_hole_treatments=None, protocol=None,
         overrides=None, elements_list=None, atoms_list=None, options=None,
         structure_preparation_settings=None, correction_energies=None, **kwargs
-    ):
+    ): # pylint: disable=too-many-statements
         """Return a builder prepopulated with inputs selected according to the chosen protocol.
 
         :param code: the ``Code`` instance configured for the ``quantumespresso.pw`` plugin.
         :param structure: the ``StructureData`` instance to use.
         :param pseudos: the core-hole pseudopotential pairs (ground-state and
                         excited-state) for the elements to be calculated. These must
                         use the mapping of {"element" : {"core_hole" : <upf>, "gipaw" : <upf>}}
@@ -459,14 +459,22 @@
         builder.core_hole_pseudos = core_hole_pseudos
         builder.gipaw_pseudos = gipaw_pseudos
         if core_hole_treatments:
             builder.core_hole_treatments = orm.Dict(dict=core_hole_treatments)
         # for get_xspectra_structures
         if structure_preparation_settings:
             builder.structure_preparation_settings = structure_preparation_settings
+            if structure_preparation_settings.get('is_molecule_input').value:
+                builder.ch_scf.pw.parameters.base.attributes.all['SYSTEM']['assume_isolated']='mt'
+                builder.ch_scf.pw.settings=orm.Dict(dict={'gamma_only':True})
+                # To ensure compatibility with the gamma_only setting, the k-points must be configured to [1, 1, 1].
+                kpoints_mesh = DataFactory('core.array.kpoints')()
+                kpoints_mesh.set_kpoints_mesh([1, 1, 1])
+                builder.ch_scf.kpoints = kpoints_mesh
+                builder.relax.base.pw.settings=orm.Dict(dict={'gamma_only':True})
         # pylint: enable=no-member
         return builder
 
 
     def setup(self):
         """Init required context variables."""
         elements_list = self.inputs.get('elements_list', None)
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/base.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/base.py`

 * *Files identical despite different names*

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/core.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import pathlib
 from typing import Optional, Union
 
 from aiida import orm
 from aiida.common import AttributeDict
 from aiida.engine import ToContext, WorkChain, append_, if_
 from aiida.orm.nodes.data.base import to_aiida_type
-from aiida.plugins import CalculationFactory, WorkflowFactory
+from aiida.plugins import CalculationFactory, DataFactory, WorkflowFactory
 import yaml
 
 from aiida_quantumespresso.calculations.functions.xspectra.get_powder_spectrum import get_powder_spectrum
 from aiida_quantumespresso.calculations.functions.xspectra.merge_spectra import merge_spectra
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
 from aiida_quantumespresso.workflows.protocols.utils import ProtocolMixin, recursive_merge
 
 PwCalculation = CalculationFactory('quantumespresso.pw')
 PwBaseWorkChain = WorkflowFactory('quantumespresso.pw.base')
 XspectraBaseWorkChain = WorkflowFactory('quantumespresso.xspectra.base')
+HubbardStructureData = DataFactory('quantumespresso.hubbard_structure')
 
 
 class XspectraCoreWorkChain(ProtocolMixin, WorkChain):
     """Workchain to compute X-ray absorption spectra for a given structure using Quantum ESPRESSO.
 
     The workflow follows the process required to compute the XAS of an input structure: an SCF calculation is performed
     using the provided structure, which is then followed by the calculation of the XAS itself by XSpectra. The
@@ -97,15 +98,15 @@
                 'required': False,
                 'populate_defaults': False
             }
         )
         spec.inputs.validator = cls.validate_inputs
         spec.input(
             'structure',
-            valid_type=orm.StructureData,
+            valid_type=(orm.StructureData, HubbardStructureData),
             help=(
                 'Structure to be used for calculation, with at least one site containing the `abs_atom_marker` '
                 'as the kind label.'
             )
         )
         spec.input(
             'eps_vectors',
@@ -344,16 +345,16 @@
             left=pw_params,
             right=cls.get_treatment_inputs(
                 treatment=core_hole_treatment, overrides=inputs.get('scf', {}).get('pw', {}).get('parameters', None)
             )
         )
 
         pw_inputs['pw']['parameters'] = pw_params
-
         pw_args = (pw_code, structure, protocol)
+
         scf = PwBaseWorkChain.get_builder_from_protocol(*pw_args, overrides=pw_inputs, options=options, **kwargs)
 
         scf.pop('clean_workdir', None)
         scf['pw'].pop('structure', None)
 
         # pylint: disable=no-member
         builder = cls.get_builder()
@@ -364,20 +365,24 @@
         xs_prod_metadata = xs_prod_inputs['xspectra']['metadata']
         if options:
             xs_prod_metadata['options'] = recursive_merge(xs_prod_metadata['options'], options)
 
         abs_atom_marker = inputs['abs_atom_marker']
         xs_prod_parameters['INPUT_XSPECTRA']['xiabs'] = kinds_present.index(abs_atom_marker) + 1
         if core_hole_pseudos:
+            abs_element_kinds = []
             for kind in structure.kinds:
                 if kind.name == abs_atom_marker:
                     abs_element = kind.symbol
-
+            for kind in structure.kinds:  # run a second pass to check for multiple kinds of the same absorbing element
+                if kind.symbol == abs_element and kind.name != abs_atom_marker:
+                    abs_element_kinds.append(kind.name)
             builder.scf.pw.pseudos[abs_atom_marker] = core_hole_pseudos[abs_atom_marker]
-            builder.scf.pw.pseudos[abs_element] = core_hole_pseudos[abs_element]
+            for kind_name in abs_element_kinds:
+                builder.scf.pw.pseudos[kind_name] = core_hole_pseudos[abs_element]
 
         builder.xs_prod.xspectra.code = xs_code
         builder.xs_prod.xspectra.parameters = orm.Dict(xs_prod_parameters)
         builder.xs_prod.xspectra.metadata = xs_prod_metadata
         if xs_prod_inputs['kpoints_distance']:
             builder.xs_prod.kpoints_distance = orm.Float(xs_prod_inputs['kpoints_distance'])
         elif xs_prod_inputs['kpoints']:
```

### Comparing `aiida_quantumespresso-4.5.1/src/aiida_quantumespresso/workflows/xspectra/crystal.py` & `aiida_quantumespresso-4.6.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from aiida.common import AttributeDict, ValidationError
 from aiida.engine import ToContext, WorkChain, if_
 from aiida.orm import UpfData as aiida_core_upf
 from aiida.plugins import CalculationFactory, DataFactory, WorkflowFactory
 from aiida_pseudo.data.pseudo import UpfData as aiida_pseudo_upf
 
 from aiida_quantumespresso.calculations.functions.xspectra.get_spectra_by_element import get_spectra_by_element
+from aiida_quantumespresso.utils.hubbard import HubbardStructureData
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
 from aiida_quantumespresso.workflows.protocols.utils import ProtocolMixin, recursive_merge
 
 PwCalculation = CalculationFactory('quantumespresso.pw')
 PwBaseWorkChain = WorkflowFactory('quantumespresso.pw.base')
 PwRelaxWorkChain = WorkflowFactory('quantumespresso.pw.relax')
 XspectraBaseWorkChain = WorkflowFactory('quantumespresso.xspectra.base')
@@ -477,14 +478,18 @@
             }
         }
         if 'structure_preparation_settings' in self.inputs:
             optional_cell_prep = self.inputs.structure_preparation_settings
             for key, node in optional_cell_prep.items():
                 inputs[key] = node
 
+        if isinstance(self.inputs.structure, HubbardStructureData):
+            # This must be False in the case of HubbardStructureData, otherwise get_xspectra_structures will except
+            inputs['standardize_structure'] = orm.Bool(False)
+
         if 'spglib_settings' in self.inputs:
             inputs['spglib_settings'] = self.inputs.spglib_settings
 
         if 'relax' in self.inputs:
             result = get_xspectra_structures(self.ctx.optimized_structure, **inputs)
         else:
             result = get_xspectra_structures(self.inputs.structure, **inputs)
@@ -523,16 +528,24 @@
         for element in elements_list:
             upf = self.inputs.gipaw_pseudos[f'{element}']
 
             shell_inputs = {}
 
             shell_inputs['code'] = self.inputs.upf2plotcore_code
             shell_inputs['nodes'] = {'upf': upf}
-            shell_inputs['arguments'] = ['upf']
-            shell_inputs['metadata'] = {'call_link_label': f'upf2plotcore_{element}'}
+            shell_inputs['metadata'] = {
+                'call_link_label': f'upf2plotcore_{element}',
+                'options' : {
+                    'filename_stdin' : upf.filename,
+                    'resources' : {
+                        'num_machines' : 1,
+                        'num_mpiprocs_per_machine' : 1
+                    }
+                }
+            }
 
             future_shelljob = self.submit(ShellJob, **shell_inputs)
             self.report(f'Launching upf2plotcore.sh for {element}<{future_shelljob.pk}>')
             shelljobs[f'upf2plotcore_{element}'] = future_shelljob
 
         return ToContext(**shelljobs)
 
@@ -549,27 +562,28 @@
             shelljob_node = self.ctx[f'upf2plotcore_{label}']
             core_wfc_data = shelljob_node.outputs.stdout
             header_line = core_wfc_data.get_content()[:40]
             num_core_states = int(header_line.split(' ')[5])
             if num_core_states == 0:
                 return self.exit_codes.ERROR_NO_GIPAW_INFO_FOUND
 
-    def run_all_xspectra_core(self):
+    def run_all_xspectra_core(self): # pylint: disable=too-many-statements
         """Call all XspectraCoreWorkChains required to compute all requested spectra."""
 
         structures_to_process = self.ctx.structures_to_process
         equivalent_sites_data = self.ctx.equivalent_sites_data
         abs_atom_marker = self.inputs.abs_atom_marker.value
 
         xspectra_core_workchains = {}
         for site in structures_to_process:
             inputs = AttributeDict(self.exposed_inputs(XspectraCoreWorkChain, namespace='core'))
             structure = structures_to_process[site]
             inputs.structure = structure
             abs_element = equivalent_sites_data[site]['symbol']
+            abs_atom_kind = equivalent_sites_data[site]['kind_name']
 
             if 'core_hole_treatments' in self.inputs:
                 ch_treatments = self.inputs.core_hole_treatments.get_dict()
                 ch_treatment = ch_treatments.get(abs_element, 'full')
             else:
                 ch_treatment = 'full'
 
@@ -581,50 +595,74 @@
                 inputs.core_wfc_data = self.ctx[f'upf2plotcore_{abs_element}'].outputs.stdout
 
             # Get the given settings for the SCF inputs and then overwrite them with the
             # chosen core-hole approximation, then apply the correct pseudopotential pair.
             scf_inputs = inputs.scf.pw
             scf_params = scf_inputs.parameters.get_dict()
             ch_inputs = XspectraCoreWorkChain.get_treatment_inputs(treatment=ch_treatment)
-            new_scf_params = recursive_merge(left=scf_params, right=ch_inputs)
+            new_scf_params = recursive_merge(left=ch_inputs, right=scf_params)
 
             # Set the absorbing species index (`xiabs`) for the xspectra.x input.
             new_xs_params = inputs.xs_prod.xspectra.parameters.get_dict()
             kinds_present = sorted([kind.name for kind in structure.kinds])
             abs_species_index = kinds_present.index(abs_atom_marker) + 1
             new_xs_params['INPUT_XSPECTRA']['xiabs'] = abs_species_index
 
-            # Set `starting_magnetization` if we are using an XCH approximation, using the
-            # absorbing species as a reasonable place for the unpaired electron.
-            # As a future note, we need to re-visit the core-hole treatment settings, in order
-            # to avoid the need for fudges like these.
-            if ch_treatment == 'xch_smear':
-                new_scf_params['SYSTEM'][f'starting_magnetization({abs_species_index})'] = 1
+            # Set `starting_magnetization` if we are using an XCH approximation, using
+            # the absorbing species as a reasonable place for the unpaired electron.
+            # Alternatively, ensure the starting magnetic moment is a reasonable guess
+            # given the input parameters. (e.g. it conforms to an existing magnetic
+            # structure already defined for the system)
+
+            # TODO: we need to re-visit the core-hole treatment settings,
+            # in order to avoid the need for fudges like these and set these at
+            # submission rather than inside the WorkChain itself.
+            if 'starting_magnetization' in new_scf_params['SYSTEM']:
+                inherited_mag =  new_scf_params['SYSTEM']['starting_magnetization'][abs_atom_kind]
+                if ch_treatment not in ['xch_smear', 'xch_fixed']:
+                    new_scf_params['SYSTEM']['starting_magnetization'][abs_atom_marker] = inherited_mag
+                else: # if there is meant to be an unpaired electron, give it to the absorbing atom.
+                    if inherited_mag == 0: # set it to 1, if it would be neutral in the ground-state.
+                        new_scf_params['SYSTEM']['starting_magnetization'][abs_atom_marker] =  1
+                    else: # assume that it takes the same magnetic configuration as the kind that it replaces.
+                        new_scf_params['SYSTEM']['starting_magnetization'][abs_atom_marker] =  inherited_mag
+            elif ch_treatment in ['xch_smear', 'xch_fixed']:
+                new_scf_params['SYSTEM']['starting_magnetization'] = {abs_atom_marker : 1}
+
+            # remove any duplicates created from the "core_hole_treatments.yaml" defaults
+            for key in new_scf_params['SYSTEM'].keys():
+                if 'starting_magnetization(' in key:
+                    new_scf_params['SYSTEM'].pop(key, None)
 
             core_hole_pseudo = self.inputs.core_hole_pseudos[abs_element]
+            gipaw_pseudo = self.inputs.gipaw_pseudos[abs_element]
             inputs.scf.pw.pseudos[abs_atom_marker] = core_hole_pseudo
-            # In the case where the absorbing atom is the only one of its element in the
-            # structure, we avoid setting the GIPAW pseudo for it and remove the one .
-            if abs_element in kinds_present:
-                gipaw_pseudo = self.inputs.gipaw_pseudos[abs_element]
-                inputs.scf.pw.pseudos[abs_element] = gipaw_pseudo
-            else:
+            # Check how many instances of the absorbing element are present and assign
+            # each the GIPAW pseudo if they are not the absorbing atom itself.
+            abs_element_kinds = []
+            for kind in structure.kinds:
+                if kind.symbol == abs_element and kind.name != abs_atom_marker:
+                    abs_element_kinds.append(kind.name)
+            if len(abs_element_kinds) > 0:
+                for kind_name in abs_element_kinds:
+                    scf_inputs['pseudos'][kind_name] = gipaw_pseudo
+            else: # if there is only one atom of the absorbing element, pop the GIPAW pseudo to avoid a crash
                 scf_inputs['pseudos'].pop(abs_element, None)
 
             scf_inputs.parameters = orm.Dict(new_scf_params)
             inputs.scf.pw = scf_inputs
             inputs.xs_prod.xspectra.parameters = orm.Dict(new_xs_params)
 
             inputs = prepare_process_inputs(XspectraCoreWorkChain, inputs)
 
             future = self.submit(XspectraCoreWorkChain, **inputs)
             xspectra_core_workchains[site] = future
             self.report(f'launched XspectraCoreWorkChain for {site}<{future.pk}>')
 
-        return ToContext(**xspectra_core_workchains)
+        return ToContext(**xspectra_core_workchains) # pylint: enable=too-many-statements
 
     def inspect_all_xspectra_core(self):
         """Check that all the XspectraCoreWorkChain sub-processes finished sucessfully."""
 
         labels = self.ctx.structures_to_process.keys()
         work_chain_nodes = {
             label : self.ctx[label] for label in labels
```

### Comparing `aiida_quantumespresso-4.5.1/PKG-INFO` & `aiida_quantumespresso-4.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-quantumespresso
-Version: 4.5.1
+Version: 4.6.0
 Summary: The official AiiDA plugin for Quantum ESPRESSO
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -56,15 +56,15 @@
 
 ## Compatibility matrix
 
 The matrix below assumes the user always install the latest patch release of the specified minor version, which is recommended.
 
 | Plugin | AiiDA | Python | Quantum ESPRESSO |
 |-|-|-|-|
-| `v4.3 < v5.0` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.2] |
+| `v4.3 < v5.0` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.3] |
 | `v4.0 < v4.3` | ![Compatibility for v4.0][AiiDA v4.0] |  [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.org/project/aiida-quantumespresso) | ![Quantum ESPRESSO compatibility][QE v6.6-7.1] |
 | `v3.5 < v4.0` | ![Compatibility for v3.5][AiiDA v3.5] |  [![PyPI pyversions][Python v3.6-v3.9]](https://pypi.org/project/aiida-quantumespresso/3.5.2/) | ![Quantum ESPRESSO compatibility][QE v6-7] |
 | `v3.4 < v3.5` | ![Compatibility for v3.4][AiiDA v3.4] |  [![PyPI pyversions][Python v3.6-v3.9]](https://pypi.org/project/aiida-quantumespresso/3.4.2/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.3 < v3.4` | ![Compatibility for v3.3][AiiDA v3.3] |  [![PyPI pyversions][Python v3.6-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.3.1/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.1 < v3.3` | ![Compatibility for v3.1][AiiDA v3.1] |  [![PyPI pyversions][Python v3.5-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.2.1/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v3.0 < v3.1` | ![Compatibility for v3.0][AiiDA v3.0] |  [![PyPI pyversions][Python v2.7-v3.8]](https://pypi.org/project/aiida-quantumespresso/3.0.0/) | ![Quantum ESPRESSO compatibility][QE v6] |
 | `v2.0 < v3.0` | ![Compatibility for v2.0][AiiDA v2.0] |  [![PyPI pyversions][Python v2.7-v3.8]](https://pypi.org/project/aiida-quantumespresso/2.1.0/) | ![Quantum ESPRESSO compatibility][QE v6] |
@@ -190,9 +190,9 @@
 [Python v3.6-v3.8]: https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue
 [Python v3.5-v3.8]: https://img.shields.io/badge/python-3.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue
 [Python v2.7-v3.8]: https://img.shields.io/badge/python-2.7%20%7C%203.5%20%7C%203.6%20%7C%203.7%20%7C%203.8-blue
 
 [QE v6]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.0,<=6.7-007ec6.svg?logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABgAAAAYCAIAAABvFaqvAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAABmJLR0QA/wD/AP+gvaeTAAAACXBIWXMAAC4jAAAuIwF4pT92AAAAB3RJTUUH5QkVEQ0n7crnLAAABcBJREFUOMtVld1PHOcVxs9533c+dmdnd2FtWNhdwEBY1xjWxk7bOHGJCEFJaOJ8VJUi2WqrtFetKvWm6lX/hKq9qFRVVi+qSk2jNKriSlEkKyYkNrFDbYONsYGADbPGBu/HLLs7Ozsz7+nFklQ9t+foJ53zPHoOnj17FhGllMC4ETZsu6wpAhm6btNpBkJRo5FQJKQBYrXWqNScwGuGNaGoipRERIgIAAAgEBEBfAk/e+PU+LGe3/39yvziigTs7OgYHzv09LdSnYmoJhiCdBuNrR17bmn788XNYrEQCamA+A1LAAAAaZp6mK+K1bmBWOIyht559enpUxlgys27OzM37hftuuCYTJhjAwd+NJ394XjPu7P5jz5fVFnAuZBSIqJAhHrdjR2MkWXB43vRzNRvf/rCiSF+6drWPz6583i3gCAZIgFIgve46M8kz070/2Qqnk0/98f3rwaByxgnIv7U0OHvjI385p3xyMJc3SoOPpdNHeR/upD/28c3yHeMkKapiqoITRG6JjSBxWJpZvER+crLRxvJrsG523nBCBH51NTkr38wEL3378bKlrSbunDPr0c/mltpj6iMCyklEEkiIAKiABBCOlPg2rotAv7yoO2E+2+tWLomRDalaO+/u/vhGuoh05SzT3V/fC/fZigBAZFsSYKMEZErRMR1E6WyBuD43j8vB4Oh8NsD+txS0t59zKf7U8MX7vpFzncabm/yz2aXW6lzzoioRZGMTSwsNXQtUyiO3N/SpWxWa1kjkiuVtx5UTvQ6e9H0wtoTRk4ALpHAUAhvpJP5sqsJJokAEQB8ziJu0zaN4QeWWXc+yw1/0pdpvDZt/PIXcyNDjx7Xbp//z/FoNWSaTAwe4M+YJD2Kajd5CJs+ICACEgWMxRx34vrC4MbmbjRyZThbcZyEorw+MXl95tKObd84dviCHacvVzuTEVbEA/rPXwq/Ea8Zaj5gAkACACACBIzF6vV4uVI1wkt9PUrd6Umlp187U3cbqh4SyESttpztX79divseW1h6cE2OmtOvVKVXI+T7jgcCUILgYXvbZqqrGDUdRQjEcsUOh41PZ2Ysa+uZU88amt7QFKuJ7FGJcZS//+ul2RUwEhpJIvgahMiIXM7v9qabqtpq1Ot1Aurs7Jx8ceqFyRdDoVBA5CL61TpTVMWt1W4+2o1lDIORJNiXnIgAuJQ+oub7HMD3/fb2RCqVsu3yZ7OfWtaWbdsKY3oQ+GGdSSIBVNFNLWOmVem11IJ91XgQFKKm5nlxp1GXQU86ZVnWxYsXh7KHq3al4jbMmpM2NLcjwYhAMLDswOntPhn3iAkAaC1CiAzA42y9s+Pk2oYP2NU/sJ3PC8ZS3d3r23lfKCfX1ju+27frBgwAFIU/2SnfCved7pHdMd31A8awZUiJqHr+Wldn0TReur2ckrSRt5RYLJFM7t1Z/t7VxVePcKu/194p8dHRUWTMdxs1LfH8Uc0IvMsPUUcfkH2dNchlsJVo54rQLs0aK6uHnIb25XywunnmtNHx5rPnrzlutcJzuRwAqIqwtoup7OjpTGEPEgv3y2EVERkRASIito71VVu8YkZKujLnsW+/NXJqsusDq/vK/HI4rPFcLteaZhTcsWpjY7nn+2xHdN3aKEDQVBXBGCIgMlQkcYRCIMt69O3vj7x1AueLh/7y4byuAAHyXC6HiETEhahVKzc3myPDR8aPYm8y/aAUPCntNVy36QdNz3OafgBsqC/zqzNHxo+Fr+cTf3jvKgQNzgUR4blz5/YdSMQ5azRcI9r+41eOnx4xJKp3N2oLG4Un5ToiJBPm2GBHf1/Eqzv/urLzwcV5Rk0hlFbU/g/UYjHGfN9zfRga6Jk43nNi8GBbPEKKAoDk+du79hfL2zPXNx7mt42QgoxJ+X/hv1+tv8S5iAhY+2pjeeV+JBJpi4ZNQyMCe88p2FXXqesqNyO6lPQNBQD+C1Fl4Lfj+TndAAAAJXRFWHRkYXRlOmNyZWF0ZQAyMDIxLTA5LTIxVDE1OjEzOjM5KzAyOjAwpCQipAAAACV0RVh0ZGF0ZTptb2RpZnkAMjAyMS0wOS0yMVQxNToxMzozOSswMjowMNV5mhgAAAAASUVORK5CYII=
 [QE v6-7]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.0,<=7.0-007ec6.svg?logo=data:image/png;base64,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
 [QE v6.6-7.1]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.1-007ec6.svg?logo=data:image/png;base64,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
-[QE v6.6-7.2]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.2-007ec6.svg?logo=data:image/png;base64,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
+[QE v6.6-7.3]: https://img.shields.io/badge/Quantum%20ESPRESSO->=6.6,<=7.3-007ec6.svg?logo=data:image/png;base64,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
```

