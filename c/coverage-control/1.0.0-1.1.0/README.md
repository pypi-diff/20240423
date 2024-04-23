# Comparing `tmp/coverage_control-1.0.0.tar.gz` & `tmp/coverage_control-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coverage_control-1.0.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "coverage_control-1.1.0.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `coverage_control-1.0.0.tar` & `coverage_control-1.1.0.tar`

### file list

```diff
@@ -1,225 +1,230 @@
--rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.git_archival.txt
--rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.gitattributes
--rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/CONTRIBUTING.md
--rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/dependabot.yml
--rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/docker-base-action/action.yml
--rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/matchers/pylint.json
--rw-r--r--   0        0        0     1209 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0      536 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.github/workflows/ghaction-doxygen-ghpages.yml
--rw-r--r--   0        0        0     2379 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.gitignore
--rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 coverage_control-1.0.0/.prettierignore
--rw-r--r--   0        0        0     1692 2022-11-09 12:37:21.000000 coverage_control-1.0.0/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 coverage_control-1.0.0/LICENSE
--rw-r--r--   0        0        0     3031 2022-11-09 12:37:21.000000 coverage_control-1.0.0/README.md
--rw-r--r--   0        0        0     6423 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/CMakeLists.txt
--rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in
--rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/cmake/CoverageControlConfig.h.in
--rw-r--r--   0        0        0     2140 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h
--rw-r--r--   0        0        0     4644 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h
--rw-r--r--   0        0        0     4444 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h
--rw-r--r--   0        0        0     6907 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h
--rw-r--r--   0        0        0     4216 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h
--rw-r--r--   0        0        0     6247 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h
--rw-r--r--   0        0        0    14125 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h
--rw-r--r--   0        0        0     6826 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h
--rw-r--r--   0        0        0    15316 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h
--rw-r--r--   0        0        0     6530 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h
--rw-r--r--   0        0        0     2210 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/config.h
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h
--rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/utilities.h
--rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/constants.h
--rw-r--r--   0        0        0    21941 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/coverage_system.h
--rw-r--r--   0        0        0     3257 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh
--rw-r--r--   0        0        0     5159 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cuda_utils.h
--rw-r--r--   0        0        0    27792 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h
--rw-r--r--   0        0        0    14875 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h
--rw-r--r--   0        0        0    90630 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h
--rw-r--r--   0        0        0   914638 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp
--rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h
--rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE
--rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt
--rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp
--rw-r--r--   0        0        0     2769 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/generate_world_map.h
--rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h
--rw-r--r--   0        0        0     5141 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/map_utils.h
--rw-r--r--   0        0        0     5085 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/parameters.h
--rw-r--r--   0        0        0     5085 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/plotter.h
--rw-r--r--   0        0        0    15301 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/robot_model.h
--rw-r--r--   0        0        0     2859 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/typedefs.h
--rw-r--r--   0        0        0     3999 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/vec2d.h
--rw-r--r--   0        0        0     6529 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/voronoi.h
--rw-r--r--   0        0        0    13632 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/include/CoverageControl/world_idf.h
--rw-r--r--   0        0        0    24774 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/coverage_system.cpp
--rw-r--r--   0        0        0     7990 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/cuda/cuda_utils.cu
--rw-r--r--   0        0        0    11363 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/cuda/generate_world_map.cu
--rw-r--r--   0        0        0     1349 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/cuda_utils.cpp
--rw-r--r--   0        0        0    12642 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/extern/Hungarian.cpp
--rw-r--r--   0        0        0    10134 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/parameters.cpp
--rw-r--r--   0        0        0    10722 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/plotter.cpp
--rw-r--r--   0        0        0     2474 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/polygon_utils.cpp
--rw-r--r--   0        0        0     9358 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/core/src/voronoi.cpp
--rw-r--r--   0        0        0     1700 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/CMakeLists.txt
--rw-r--r--   0        0        0     4301 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/coverage_algorithm.cpp
--rw-r--r--   0        0        0     2079 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/data_generation.cpp
--rw-r--r--   0        0        0     4464 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/eval_dist_gnn.cpp
--rw-r--r--   0        0        0     3885 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/eval_gnn.cpp
--rw-r--r--   0        0        0     3764 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/test_cnn.cpp
--rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/train_cnn.cpp
--rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/main/torch/train_gnn.cpp
--rw-r--r--   0        0        0    18609 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/python_bindings/core_binds.h
--rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/python_bindings/python_binds.cpp
--rwxr-xr-x   0        0        0     4319 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/setup.sh
--rw-r--r--   0        0        0     3261 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/CMakeLists.txt
--rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/geo_transforms.cpp
--rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/map_generation.cpp
--rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/simultaneous_explore_exploit.cpp
--rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/torch/torch_data_loader.cpp
--rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/torch/torch_map_conversion.cpp
--rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/torch/torch_normalization.cpp
--rw-r--r--   0        0        0     6003 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/torch/torch_scripting.cpp
--rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/tests/torch/torch_test.cpp
--rw-r--r--   0        0        0     3585 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/CMakeLists.txt
--rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in
--rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/cmake/CoverageControlTorchConfig.h.in
--rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/base.h
--rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h
--rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h
--rw-r--r--   0        0        0    23777 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h
--rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h
--rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp
--rw-r--r--   0        0        0    16536 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h
--rw-r--r--   0        0        0     3380 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h
--rw-r--r--   0        0        0     5512 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/mlp.h
--rw-r--r--   0        0        0     7754 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h
--rw-r--r--   0        0        0     2925 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h
--rw-r--r--   0        0        0     1214 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/python_bindings/CMakeLists.txt
--rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/python_bindings/pyproject.toml
--rw-r--r--   0        0        0     6075 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp
--rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/src/base.cpp
--rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 coverage_control-1.0.0/cppsrc/torch/src/coverage_system.cpp
--rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/Doxyfile
--rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/bash-filter.py
--rw-r--r--   0        0        0   127483 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/BaseDoxyfile
--rw-r--r--   0        0        0     6808 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/DoxygenLayout.xml
--rw-r--r--   0        0        0     2921 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/custom.css
--rw-r--r--   0        0        0     8469 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-darkmode-toggle.js
--rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-fragment-copy-button.js
--rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-interactive-toc.js
--rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-paragraph-link.js
--rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-r--r--   0        0        0     3287 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-sidebar-only.css
--rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome-tabs.js
--rw-r--r--   0        0        0    67128 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/doxygen-awesome.css
--rw-r--r--   0        0        0     5455 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/header.html
--rw-r--r--   0        0        0    15889 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/config/navtree-hacks.js
--rw-r--r--   0        0        0  6603024 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/graphics/LPAC.gif
--rw-r--r--   0        0        0  1443985 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/graphics/SearchRescue.png
--rw-r--r--   0        0        0   831774 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/graphics/coveragecontrol_global.png
--rw-r--r--   0        0        0  1111552 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/graphics/learnable_pac.png
--rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/CUDA-installation-troubleshooting.md
--rw-r--r--   0        0        0     3240 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/README.md
--rw-r--r--   0        0        0     6274 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/algorithms.md
--rw-r--r--   0        0        0     7513 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/coverage-control.md
--rw-r--r--   0        0        0     2671 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/docker.md
--rw-r--r--   0        0        0     5644 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/installation.md
--rw-r--r--   0        0        0     3077 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/lpac.md
--rw-r--r--   0        0        0     4793 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/quick_start.md
--rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/manual/ref_manual.txt
--rwxr-xr-x   0        0        0       34 2022-11-09 12:37:21.000000 coverage_control-1.0.0/doc/py-filter.sh
--rw-r--r--   0        0        0     2525 2022-11-09 12:37:21.000000 coverage_control-1.0.0/params/coverage_control_params.toml
--rw-r--r--   0        0        0     1155 2022-11-09 12:37:21.000000 coverage_control-1.0.0/params/data_params.toml
--rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 coverage_control-1.0.0/params/eval.toml
--rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 coverage_control-1.0.0/params/eval_single.toml
--rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 coverage_control-1.0.0/params/learning_params.toml
--rw-r--r--   0        0        0     3416 2022-11-09 12:37:21.000000 coverage_control-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      348 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/__init__.py
--rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/_version.py
--rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/_version.pyi
--rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/algorithms/__init__.py
--rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/core/__init__.py
--rw-r--r--   0        0        0     3572 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/io_utils.py
--rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/__init__.py
--rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/data_loaders/__init__.py
--rw-r--r--   0        0        0    14354 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py
--rw-r--r--   0        0        0     7690 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/data_loaders/data_loader_utils.py
--rw-r--r--   0        0        0     8753 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/data_loaders/loaders.py
--rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/__init__.py
--rw-r--r--   0        0        0     2610 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/cnn.py
--rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/cnn_backbone.py
--rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/config_parser.py
--rw-r--r--   0        0        0     2282 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/gnn_backbone.py
--rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/models/lpac.py
--rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/trainers/__init__.py
--rw-r--r--   0        0        0     8195 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/nn/trainers/trainer.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/coverage_control/py.typed
--rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/coverage_env/coverage_class.py
--rw-r--r--   0        0        0     2018 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/coverage_env/coverage_simple.py
--rw-r--r--   0        0        0    16013 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/data_generation/data_generation.py
--rwxr-xr-x   0        0        0      150 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/data_generation/gen.sh
--rw-r--r--   0        0        0    11910 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/data_generation/simple_data_generation.py
--rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/controller.py
--rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_multi.py
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_rf_exp.py
--rw-r--r--   0        0        0     7617 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_semantic_video.py
--rw-r--r--   0        0        0     9535 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_video.py
--rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/deprecated/semantic_eval.py
--rw-r--r--   0        0        0     6547 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/eval.py
--rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/evaluators/eval_single_env.py
--rw-r--r--   0        0        0     3468 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/training/train_cnn.py
--rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/scripts/training/train_lpac.py
--rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/cnn_data_generation.py
--rw-r--r--   0        0        0     6652 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py
--rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py
--rw-r--r--   0        0        0     6804 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py
--rw-r--r--   0        0        0     6111 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py
--rw-r--r--   0        0        0     7892 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py
--rw-r--r--   0        0        0     7140 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py
--rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/gnn.py
--rw-r--r--   0        0        0     4851 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/gnn_dist.py
--rw-r--r--   0        0        0     2948 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/mlp_test.py
--rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/plot_edge_weights.py
--rw-r--r--   0        0        0     3574 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/test_cnn.py
--rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/test_jit_tensor.py
--rw-r--r--   0        0        0     6115 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/test_library_objects.py
--rw-r--r--   0        0        0     3977 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/test_lpac_coverage.py
--rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/testplot.py
--rw-r--r--   0        0        0     2861 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/deprecated/torch_compat.py
--rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_coverage.py
--rw-r--r--   0        0        0     9921 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_coverage_env_utils.py
--rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_env_io.py
--rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_map_generation.py
--rw-r--r--   0        0        0     3583 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_models.py
--rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_package.py
--rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_parameters.py
--rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/tests/test_parity.py
--rw-r--r--   0        0        0    27669 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/ts_jit/TorchVisionResize_32.pt
--rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/ts_jit/gnn_backbone.py
--rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/ts_jit/torchvision_resize.py
--rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/utils/dataset_utils.py
--rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/utils/generate_video.py
--rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/utils/process_data.sh
--rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/utils/save_gnn_params.py
--rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 coverage_control-1.0.0/python/utils/save_state_dict.py
--rwxr-xr-x   0        0        0     2987 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup.sh
--rwxr-xr-x   0        0        0     1163 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/check_headers.sh
--rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/Dockerfile
--rwxr-xr-x   0        0        0     4196 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/.bashrc
--rwxr-xr-x   0        0        0     4514 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/.ros.bashrc
--rw-r--r--   0        0        0     1470 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/build_all_images.sh
--rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/requirements.txt
--rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/requirements_cpu.txt
--rw-r--r--   0        0        0     3410 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile
--rw-r--r--   0        0        0     3382 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile
--rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile
--rwxr-xr-x   0        0        0     1436 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/create_container.sh
--rwxr-xr-x   0        0        0       68 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/docker/entrypoint.sh
--rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/helpers.sh
--rwxr-xr-x   0        0        0     9060 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/install_dependencies.sh
--rwxr-xr-x   0        0        0      911 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/install_libtorch.sh
--rwxr-xr-x   0        0        0      633 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/manylinux_2_28_before-all.sh
--rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/noxfile.py
--rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/requirements.txt
--rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 coverage_control-1.0.0/setup_utils/requirements_cpu.txt
--rw-r--r--   0        0        0    45197 2022-11-09 12:37:21.000000 coverage_control-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      125 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.git_archival.txt
+-rw-r--r--   0        0        0       61 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.gitattributes
+-rw-r--r--   0        0        0     1333 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/CONTRIBUTING.md
+-rw-r--r--   0        0        0      224 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1635 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/docker-base-action/action.yml
+-rw-r--r--   0        0        0      668 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/matchers/pylint.json
+-rw-r--r--   0        0        0     1253 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     1714 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/cd_wheels.yml
+-rw-r--r--   0        0        0      561 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.github/workflows/ghaction-doxygen-ghpages.yml
+-rw-r--r--   0        0        0     2379 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.gitignore
+-rw-r--r--   0        0        0     2870 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        4 2022-11-09 12:37:21.000000 coverage_control-1.1.0/.prettierignore
+-rw-r--r--   0        0        0     1757 2022-11-09 12:37:21.000000 coverage_control-1.1.0/CMakeLists.txt
+-rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 coverage_control-1.1.0/LICENSE
+-rw-r--r--   0        0        0     3418 2022-11-09 12:37:21.000000 coverage_control-1.1.0/README.md
+-rw-r--r--   0        0        0     6438 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/CMakeLists.txt
+-rw-r--r--   0        0        0      642 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in
+-rw-r--r--   0        0        0      443 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.h.in
+-rw-r--r--   0        0        0     2140 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h
+-rw-r--r--   0        0        0     4644 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h
+-rw-r--r--   0        0        0     4444 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h
+-rw-r--r--   0        0        0     6907 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h
+-rw-r--r--   0        0        0     4216 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h
+-rw-r--r--   0        0        0     6247 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h
+-rw-r--r--   0        0        0    14125 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h
+-rw-r--r--   0        0        0     6826 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h
+-rw-r--r--   0        0        0    15316 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h
+-rw-r--r--   0        0        0     6530 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h
+-rw-r--r--   0        0        0     2477 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/config.h
+-rw-r--r--   0        0        0     2220 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h
+-rw-r--r--   0        0        0     3752 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/utilities.h
+-rw-r--r--   0        0        0     2219 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/constants.h
+-rw-r--r--   0        0        0    22208 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/coverage_system.h
+-rw-r--r--   0        0        0     3320 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh
+-rw-r--r--   0        0        0     5159 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda_utils.h
+-rw-r--r--   0        0        0    27792 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h
+-rw-r--r--   0        0        0    14875 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h
+-rw-r--r--   0        0        0    90448 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h
+-rw-r--r--   0        0        0   914638 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp
+-rw-r--r--   0        0        0     2157 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h
+-rw-r--r--   0        0        0     1291 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE
+-rw-r--r--   0        0        0      555 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt
+-rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp
+-rw-r--r--   0        0        0     2769 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/generate_world_map.h
+-rw-r--r--   0        0        0     2321 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h
+-rw-r--r--   0        0        0     5141 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/map_utils.h
+-rw-r--r--   0        0        0     5246 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/parameters.h
+-rw-r--r--   0        0        0     5085 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/plotter.h
+-rw-r--r--   0        0        0    15301 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/robot_model.h
+-rw-r--r--   0        0        0     2859 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/typedefs.h
+-rw-r--r--   0        0        0     3999 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/vec2d.h
+-rw-r--r--   0        0        0     6529 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/voronoi.h
+-rw-r--r--   0        0        0    11924 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/include/CoverageControl/world_idf.h
+-rw-r--r--   0        0        0    25544 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/coverage_system.cpp
+-rw-r--r--   0        0        0     8168 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda/cuda_utils.cu
+-rw-r--r--   0        0        0    11364 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda/generate_world_map.cu
+-rw-r--r--   0        0        0     1349 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/cuda_utils.cpp
+-rw-r--r--   0        0        0    12642 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/extern/Hungarian.cpp
+-rw-r--r--   0        0        0    10949 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/parameters.cpp
+-rw-r--r--   0        0        0    10722 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/plotter.cpp
+-rw-r--r--   0        0        0     3994 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/polygon_utils.cpp
+-rw-r--r--   0        0        0     9358 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/voronoi.cpp
+-rw-r--r--   0        0        0     4659 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/core/src/world_idf.cpp
+-rw-r--r--   0        0        0     1878 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/CMakeLists.txt
+-rw-r--r--   0        0        0     4301 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/coverage_algorithm.cpp
+-rw-r--r--   0        0        0     2079 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/data_generation.cpp
+-rw-r--r--   0        0        0     4464 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/eval_dist_gnn.cpp
+-rw-r--r--   0        0        0     3885 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/eval_gnn.cpp
+-rw-r--r--   0        0        0     3764 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/test_cnn.cpp
+-rw-r--r--   0        0        0     1217 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/train_cnn.cpp
+-rw-r--r--   0        0        0     1210 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/torch/train_gnn.cpp
+-rw-r--r--   0        0        0     2100 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/main/world_idf.cpp
+-rw-r--r--   0        0        0    19463 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/python_bindings/core_binds.h
+-rw-r--r--   0        0        0     1513 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/python_bindings/python_binds.cpp
+-rwxr-xr-x   0        0        0     4319 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/setup.sh
+-rw-r--r--   0        0        0     3261 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/CMakeLists.txt
+-rw-r--r--   0        0        0     2056 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/geo_transforms.cpp
+-rw-r--r--   0        0        0     2658 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/map_generation.cpp
+-rw-r--r--   0        0        0     3234 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/simultaneous_explore_exploit.cpp
+-rw-r--r--   0        0        0     2597 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_data_loader.cpp
+-rw-r--r--   0        0        0     2749 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_map_conversion.cpp
+-rw-r--r--   0        0        0     1288 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_normalization.cpp
+-rw-r--r--   0        0        0     6003 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_scripting.cpp
+-rw-r--r--   0        0        0     1011 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/tests/torch/torch_test.cpp
+-rw-r--r--   0        0        0     3585 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/CMakeLists.txt
+-rw-r--r--   0        0        0      764 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in
+-rw-r--r--   0        0        0      242 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.h.in
+-rw-r--r--   0        0        0     1057 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/base.h
+-rw-r--r--   0        0        0     3104 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h
+-rw-r--r--   0        0        0     2961 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h
+-rw-r--r--   0        0        0    23777 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h
+-rw-r--r--   0        0        0     4278 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h
+-rw-r--r--   0        0        0   485931 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp
+-rw-r--r--   0        0        0    16536 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h
+-rw-r--r--   0        0        0     3380 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h
+-rw-r--r--   0        0        0     5512 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/mlp.h
+-rw-r--r--   0        0        0     7754 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h
+-rw-r--r--   0        0        0     2925 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h
+-rw-r--r--   0        0        0     1214 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/CMakeLists.txt
+-rw-r--r--   0        0        0      405 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/pyproject.toml
+-rw-r--r--   0        0        0     6075 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp
+-rw-r--r--   0        0        0     1379 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/src/base.cpp
+-rw-r--r--   0        0        0     5111 2022-11-09 12:37:21.000000 coverage_control-1.1.0/cppsrc/torch/src/coverage_system.cpp
+-rw-r--r--   0        0        0     1228 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/Doxyfile
+-rw-r--r--   0        0        0     4824 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/bash-filter.py
+-rw-r--r--   0        0        0   127483 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/BaseDoxyfile
+-rw-r--r--   0        0        0     6808 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/DoxygenLayout.xml
+-rw-r--r--   0        0        0     2957 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/custom.css
+-rw-r--r--   0        0        0     8469 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-darkmode-toggle.js
+-rw-r--r--   0        0        0     4042 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-fragment-copy-button.js
+-rw-r--r--   0        0        0     3177 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-interactive-toc.js
+-rw-r--r--   0        0        0     2447 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-paragraph-link.js
+-rw-r--r--   0        0        0     1474 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-r--r--   0        0        0     3287 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only.css
+-rw-r--r--   0        0        0     3797 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome-tabs.js
+-rw-r--r--   0        0        0    67222 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/doxygen-awesome.css
+-rw-r--r--   0        0        0     5455 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/header.html
+-rw-r--r--   0        0        0    15889 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/config/navtree-hacks.js
+-rw-r--r--   0        0        0  6603024 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/LPAC.gif
+-rw-r--r--   0        0        0  1443985 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/SearchRescue.png
+-rw-r--r--   0        0        0   831774 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/coveragecontrol_global.png
+-rw-r--r--   0        0        0  1111552 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/graphics/learnable_pac.png
+-rw-r--r--   0        0        0       12 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/CUDA-installation-troubleshooting.md
+-rw-r--r--   0        0        0     3629 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/README.md
+-rw-r--r--   0        0        0     6274 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/algorithms.md
+-rw-r--r--   0        0        0     7513 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/coverage-control.md
+-rw-r--r--   0        0        0     2671 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/docker.md
+-rw-r--r--   0        0        0     5747 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/installation.md
+-rw-r--r--   0        0        0     3082 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/lpac.md
+-rw-r--r--   0        0        0     5038 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/quick_start.md
+-rw-r--r--   0        0        0      721 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/manual/ref_manual.txt
+-rwxr-xr-x   0        0        0       34 2022-11-09 12:37:21.000000 coverage_control-1.1.0/doc/py-filter.sh
+-rw-r--r--   0        0        0     2578 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/coverage_control_params.toml
+-rw-r--r--   0        0        0     1155 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/data_params.toml
+-rw-r--r--   0        0        0      900 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/eval.toml
+-rw-r--r--   0        0        0     1074 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/eval_single.toml
+-rw-r--r--   0        0        0      837 2022-11-09 12:37:21.000000 coverage_control-1.1.0/params/learning_params.toml
+-rw-r--r--   0        0        0     3876 2022-11-09 12:37:21.000000 coverage_control-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      457 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/__init__.py
+-rw-r--r--   0        0        0      411 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/_version.py
+-rw-r--r--   0        0        0      118 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/_version.pyi
+-rw-r--r--   0        0        0      268 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/algorithms/__init__.py
+-rw-r--r--   0        0        0      656 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/core/__init__.py
+-rw-r--r--   0        0        0     3572 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/io_utils.py
+-rw-r--r--   0        0        0      446 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/__init__.py
+-rw-r--r--   0        0        0      493 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/__init__.py
+-rw-r--r--   0        0        0    14354 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py
+-rw-r--r--   0        0        0     7690 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/data_loader_utils.py
+-rw-r--r--   0        0        0     8753 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/data_loaders/loaders.py
+-rw-r--r--   0        0        0      182 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/__init__.py
+-rw-r--r--   0        0        0     2610 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/cnn.py
+-rw-r--r--   0        0        0     3374 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/cnn_backbone.py
+-rw-r--r--   0        0        0     2560 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/config_parser.py
+-rw-r--r--   0        0        0     2282 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/gnn_backbone.py
+-rw-r--r--   0        0        0     3922 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/models/lpac.py
+-rw-r--r--   0        0        0      129 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/trainers/__init__.py
+-rw-r--r--   0        0        0     8195 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/nn/trainers/trainer.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/coverage_control/py.typed
+-rw-r--r--   0        0        0     2808 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/coverage_class.py
+-rw-r--r--   0        0        0     2018 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/coverage_simple.py
+-rw-r--r--   0        0        0     1283 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/world_idf.py
+-rw-r--r--   0        0        0     2480 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/coverage_env/world_map_numpy.py
+-rw-r--r--   0        0        0    16013 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/data_generation.py
+-rwxr-xr-x   0        0        0      150 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/gen.sh
+-rw-r--r--   0        0        0    11910 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/data_generation/simple_data_generation.py
+-rw-r--r--   0        0        0     5359 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/controller.py
+-rw-r--r--   0        0        0     1284 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_multi.py
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_rf_exp.py
+-rw-r--r--   0        0        0     7617 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_semantic_video.py
+-rw-r--r--   0        0        0     9535 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_video.py
+-rw-r--r--   0        0        0    10152 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/deprecated/semantic_eval.py
+-rw-r--r--   0        0        0     6547 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/eval.py
+-rw-r--r--   0        0        0     5705 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/evaluators/eval_single_env.py
+-rw-r--r--   0        0        0     3468 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/training/train_cnn.py
+-rw-r--r--   0        0        0     4049 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/scripts/training/train_lpac.py
+-rw-r--r--   0        0        0     5830 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation.py
+-rw-r--r--   0        0        0     6652 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py
+-rw-r--r--   0        0        0     7866 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py
+-rw-r--r--   0        0        0     6804 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py
+-rw-r--r--   0        0        0     6111 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py
+-rw-r--r--   0        0        0     7892 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py
+-rw-r--r--   0        0        0     7140 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py
+-rw-r--r--   0        0        0     3562 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/gnn.py
+-rw-r--r--   0        0        0     4851 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/gnn_dist.py
+-rw-r--r--   0        0        0     2948 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/mlp_test.py
+-rw-r--r--   0        0        0      361 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/plot_edge_weights.py
+-rw-r--r--   0        0        0     3574 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_cnn.py
+-rw-r--r--   0        0        0      350 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_jit_tensor.py
+-rw-r--r--   0        0        0     6115 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_library_objects.py
+-rw-r--r--   0        0        0     3977 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/test_lpac_coverage.py
+-rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/testplot.py
+-rw-r--r--   0        0        0     2861 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/deprecated/torch_compat.py
+-rw-r--r--   0        0        0     3870 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_coverage.py
+-rw-r--r--   0        0        0     9921 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_coverage_env_utils.py
+-rw-r--r--   0        0        0     1859 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_env_io.py
+-rw-r--r--   0        0        0     2042 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_map_generation.py
+-rw-r--r--   0        0        0     3583 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_models.py
+-rw-r--r--   0        0        0     1083 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_package.py
+-rw-r--r--   0        0        0     2242 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_parameters.py
+-rw-r--r--   0        0        0     2200 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/tests/test_parity.py
+-rw-r--r--   0        0        0    27669 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/TorchVisionResize_32.pt
+-rw-r--r--   0        0        0     1552 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/gnn_backbone.py
+-rw-r--r--   0        0        0      581 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/ts_jit/torchvision_resize.py
+-rw-r--r--   0        0        0     5928 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/dataset_utils.py
+-rw-r--r--   0        0        0     1146 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/generate_video.py
+-rw-r--r--   0        0        0      304 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/process_data.sh
+-rw-r--r--   0        0        0     2941 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/save_gnn_params.py
+-rw-r--r--   0        0        0      217 2022-11-09 12:37:21.000000 coverage_control-1.1.0/python/utils/save_state_dict.py
+-rwxr-xr-x   0        0        0     2993 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup.sh
+-rwxr-xr-x   0        0        0     1163 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/check_headers.sh
+-rw-r--r--   0        0        0      468 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/Dockerfile
+-rwxr-xr-x   0        0        0     4196 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/.bashrc
+-rwxr-xr-x   0        0        0     4514 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/.ros.bashrc
+-rw-r--r--   0        0        0     1070 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/build_all_images.sh
+-rw-r--r--   0        0        0      297 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/requirements.txt
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/requirements_cpu.txt
+-rw-r--r--   0        0        0     3410 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile
+-rw-r--r--   0        0        0     3382 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile
+-rw-r--r--   0        0        0     2576 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile
+-rwxr-xr-x   0        0        0     1436 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/create_container.sh
+-rwxr-xr-x   0        0        0       68 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/docker/entrypoint.sh
+-rw-r--r--   0        0        0      198 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/helpers.sh
+-rwxr-xr-x   0        0        0    10447 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/install_dependencies.sh
+-rwxr-xr-x   0        0        0      911 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/install_libtorch.sh
+-rwxr-xr-x   0        0        0      633 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/manylinux_2_28_before-all.sh
+-rw-r--r--   0        0        0     1659 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/noxfile.py
+-rw-r--r--   0        0        0      312 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/requirements.txt
+-rw-r--r--   0        0        0      360 2022-11-09 12:37:21.000000 coverage_control-1.1.0/setup_utils/requirements_cpu.txt
+-rw-r--r--   0        0        0    45505 2022-11-09 12:37:21.000000 coverage_control-1.1.0/PKG-INFO
```

### Comparing `coverage_control-1.0.0/.github/CONTRIBUTING.md` & `coverage_control-1.1.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/.github/docker-base-action/action.yml` & `coverage_control-1.1.0/.github/docker-base-action/action.yml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/.github/matchers/pylint.json` & `coverage_control-1.1.0/.github/matchers/pylint.json`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/.github/workflows/cd.yml` & `coverage_control-1.1.0/.github/workflows/cd.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 name: docker-deploy
 on:
+  workflow_dispatch:
   release:
     types: [published]
 
+env:
+  FORCE_COLOR: 3
+
 jobs:
   docker-deploy:
     permissions: write-all
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
       - name: Free Disk Space (Ubuntu)
         uses: jlumbroso/free-disk-space@v1.3.1
       - name: 'CI docker base'
         uses: ./.github/docker-base-action
         with:
-          base_tag: pytorch2.2.1-cuda12.3.1-ros2humble
+          base_tag: pytorch2.2.2-cuda12.2.2-ros2humble
           github_token: ${{ secrets.GITHUB_TOKEN }}
       - name: cleanup
         run: docker system prune -a -f
       - name: 'CI docker base'
         uses: ./.github/docker-base-action
         with:
-          base_tag: pytorch2.2.1-ros2humble
+          base_tag: pytorch2.2.2-ros2humble
           github_token: ${{ secrets.GITHUB_TOKEN }}
       - name: cleanup
         run: docker system prune -a -f
       - name: 'CI docker base'
         uses: ./.github/docker-base-action
         with:
-          base_tag: pytorch2.2.1-cuda12.3.1
+          base_tag: pytorch2.2.2-cuda12.2.2
           github_token: ${{ secrets.GITHUB_TOKEN }}
       - name: cleanup
         run: docker system prune -a -f
       - name: 'CI docker base'
         uses: ./.github/docker-base-action
         with:
-          base_tag: pytorch2.2.1
+          base_tag: pytorch2.2.2
           github_token: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `coverage_control-1.0.0/.github/workflows/ghaction-doxygen-ghpages.yml` & `coverage_control-1.1.0/.github/workflows/ghaction-doxygen-ghpages.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 name: doxygen-ghpages
 on:
+  workflow_dispatch:
   release:
     types: [published]
   push:
     paths:
       - 'doc/**'
 permissions:
   contents: write
@@ -12,13 +13,13 @@
   deploy:
     runs-on: ubuntu-latest
     steps:
       - name: Checkout
         uses: actions/checkout@v4
       - name: Action Doxygen and GitHub Pages
         id: ghaction
-        uses: AgarwalSaurav/ghaction-doxygen-ghpages@v2.0.1
+        uses: AgarwalSaurav/ghaction-doxygen-ghpages@release/v2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           doxyfile-path: doc/Doxyfile
           html-output-folder: doc/html
           branch: gh-pages
```

### Comparing `coverage_control-1.0.0/.gitignore` & `coverage_control-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/.pre-commit-config.yaml` & `coverage_control-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/CMakeLists.txt` & `coverage_control-1.1.0/CMakeLists.txt`

 * *Files 3% similar despite different names*

```diff
@@ -6,27 +6,31 @@
 endif()
 project(${PROJECT_NAME} LANGUAGES CXX)
 
 set(CMAKE_CXX_STANDARD 17)
 set(CMAKE_CXX_STANDARD_REQUIRED True)
 set(CMAKE_COLOR_DIAGNOSTICS True)
 
+if(NOT CMAKE_BUILD_TYPE)
+	set(CMAKE_BUILD_TYPE Release)
+endif()
+
 include(FetchContent)
 
 find_package(Python COMPONENTS Interpreter Development)
 if(NOT ${SKBUILD_STATE} STREQUAL "sdist"
 		AND EXISTS "${CMAKE_CURRENT_SOURCE_DIR}/third_party/pybind11/CMakeLists.txt")
 	message(STATUS "Using integrated pybind11")
 	add_subdirectory(third_party/pybind11)
 else()
 	message(STATUS "Using pybind11 via FetchContent")
 	FetchContent_Declare(
 		pybind11
 		GIT_REPOSITORY https://github.com/pybind/pybind11.git
-		GIT_TAG v2.11.1
+		GIT_TAG v2.12.0
 	)
 	FetchContent_MakeAvailable(pybind11)
 endif()
 
 set(PYBIND11_NEWPYTHON True)
 # find_package(pybind11 CONFIG REQUIRED)
 find_package(Python COMPONENTS Interpreter Development.Module REQUIRED)
```

### Comparing `coverage_control-1.0.0/LICENSE` & `coverage_control-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/README.md` & `coverage_control-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,34 @@
 See full documentation at [https://KumarRobotics.github.io/CoverageControl/](https://KumarRobotics.github.io/CoverageControl/)
 
 ## Introduction
 
 Coverage control is the problem of navigating a robot swarm to collaboratively monitor features or a phenomenon of interest not known _a priori_.
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
-<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/blob/main/doc/graphics/LPAC.gif">
+<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/raw/main/doc/graphics/LPAC.gif">
 
 **Key features:**  
-- The core library `CoverageControlCore` is written in `C++` and `CUDA` to handle large-scale simulations
+- The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
 - GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
+## Quick Start
+The library is available as a `pip` package. To install the package, run the following command:
+```bash
+pip install coverage_control
+```
+
+See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
+
+See [Quick Start](https://kumarrobotics.github.io/CoverageControl/quick_start.html) guide for a quick introduction to the library.
+
+---
 
 ## Citation
 ```
 @article{agarwal2024lpac,
       title         =   {LPAC: Learnable Perception-Action-Communication Loops with
                             Applications to Coverage Control}, 
       author        =   {Saurav Agarwal and Ramya Muthukrishnan and
```

### Comparing `coverage_control-1.0.0/cppsrc/core/CMakeLists.txt` & `coverage_control-1.1.0/cppsrc/core/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 include(DynamicVersion)
 dynamic_version(PROJECT_PREFIX "CoverageControl_" GIT_ARCHIVAL_FILE "${CMAKE_CURRENT_SOURCE_DIR}/../../.git_archival.txt"
   FALLBACK_VERSION 0.0.1)
 
 project(CoverageControl VERSION ${PROJECT_VERSION} LANGUAGES CXX)
 
-if (NOT CMAKE_BUILD_TYPE)
+if(NOT CMAKE_BUILD_TYPE)
 	set(CMAKE_BUILD_TYPE Release)
 endif()
 
 option(COVERAGECONTROL_WITH_CUDA "Enable CUDA support" ON)
 
 if (COVERAGECONTROL_WITH_CUDA)
 	cmake_minimum_required(VERSION 3.24)
@@ -114,14 +114,15 @@
 ## CoverageControl library ##
 #################################
 
 set(sources_list
 	polygon_utils.cpp
 	parameters.cpp
 	voronoi.cpp
+  world_idf.cpp
 	coverage_system.cpp
 	plotter.cpp
 	cuda_utils.cpp
 	extern/Hungarian.cpp)
 
 if (COVERAGECONTROL_WITH_CUDA)
 	list(APPEND sources_list
```

### Comparing `coverage_control-1.0.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in` & `coverage_control-1.1.0/cppsrc/core/cmake/CoverageControlConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/abstract_controller.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/centralized_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/clairvoyant_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/decentralized_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/near_optimal_cvt_algorithm.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_bang_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/oracle_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/algorithms/simul_explore_exploit.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/bivariate_normal_distribution.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/config.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/config.h`

 * *Files 10% similar despite different names*

```diff
@@ -32,16 +32,20 @@
 #include <CGAL/Arr_linear_traits_2.h>
 #include <CGAL/Arr_walk_along_line_point_location.h>
 #include <CGAL/Arrangement_2.h>
 #include <CGAL/Delaunay_triangulation_2.h>
 #include <CGAL/Exact_predicates_exact_constructions_kernel.h>
 #include <CGAL/Partition_traits_2.h>
 #include <CGAL/Polygon_with_holes_2.h>
+#include <CGAL/Random.h>
+#include <CGAL/algorithm.h>
 #include <CGAL/centroid.h>
 #include <CGAL/partition_2.h>
+#include <CGAL/point_generators_2.h>
+#include <CGAL/random_polygon_2.h>
 
 #include <iterator>
 
 typedef CGAL::Exact_predicates_exact_constructions_kernel K;
 typedef K::Point_2 CGAL_Point2;
 typedef K::Iso_rectangle_2 Iso_rectangle_2;
 typedef K::Segment_2 Segment_2;
@@ -54,8 +58,11 @@
 
 typedef CGAL::Arr_linear_traits_2<K> Traits_2;
 typedef CGAL::Arrangement_2<Traits_2> Arrangement_2;
 typedef CGAL::Arr_walk_along_line_point_location<Arrangement_2> CGAL_pl;
 
 typedef CGAL::Partition_traits_2<K> Partition_traits_2;
 
+typedef CGAL::Creator_uniform_2<double, CGAL_Point2> Creator;
+typedef CGAL::Random_points_in_square_2<CGAL_Point2, Creator> Point_generator;
+
 #endif  // CPPSRC_CORE_INCLUDE_COVERAGECONTROL_CGAL_CONFIG_H_
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/polygon_utils.h`

 * *Files 18% similar despite different names*

```diff
@@ -39,10 +39,23 @@
  *
  * @param[in] polygon The input polygon
  * @param[out] y_monotone_polygons The output y-monotone polygons
  */
 void PolygonYMonotonePartition(PointVector const &polygon,
                                std::vector<PointVector> &y_monotone_polygons);
 
+/*! \brief Generate random polygons
+ *
+ * @param[in] num_polygons The number of polygons to generate
+ * @param[in] max_vertices The maximum number of vertices in each polygon
+ * @param[in] half_width The half-width of the polygon
+ * @param[in] world_size The size of the world
+ * @param[out] polygons The output polygons
+ */
+
+void GenerateRandomPolygons(int const num_polygons, int const max_vertices,
+                            double const half_width, double const world_size,
+                            std::vector<PointVector> &polygons);
+
 } /* namespace CoverageControl */
 
 #endif  // CPPSRC_CORE_INCLUDE_COVERAGECONTROL_CGAL_POLYGON_UTILS_H_
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cgal/utilities.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cgal/utilities.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/constants.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/constants.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/coverage_system.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/coverage_system.h`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,17 @@
    * \param params Parameters for the coverage system
    * \param num_gaussians Number of gaussian distributions for the world IDF
    * \param num_robots Number of robots
    */
   CoverageSystem(Parameters const &params, int const num_gaussians,
                  int const num_robots);
 
+  CoverageSystem(Parameters const &params, int const num_gaussians,
+                 int const num_polygons, int const num_robots);
+
   /*! \brief Create with given world IDF and robot positions from file
    *
    *
    * \param params Parameters for the coverage system
    * \param world_idf World IDF
    * \param pos_file_name File name for initial positions
    */
@@ -437,18 +440,21 @@
   }
   //! @}
 
   //! \name Getters
   //
   //! @{
   const auto &GetWorldIDFObject() const { return world_idf_; }
-  const MapType &GetWorldMap() const { return world_idf_.GetWorldMap(); }
   const MapType &GetSystemMap() const { return system_map_; }
   const MapType &GetSystemExplorationMap() const { return exploration_map_; }
   const MapType &GetSystemExploredIDFMap() const { return explored_idf_map_; }
+  //! Get the world map
+  const MapType &GetWorldMap() const { return world_idf_.GetWorldMap(); }
+  //! Get the world map (mutable)
+  MapType &GetWorldMapMutable() { return world_idf_.GetWorldMapMutable(); }
 
   inline auto GetNumRobots() const { return num_robots_; }
   inline auto GetNumFeatures() const { return num_robots_; }
 
   inline double GetExplorationRatio() const {
     double exploration_ratio =
         1.0 - static_cast<double>(exploration_map_.sum()) /
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda/geometry_utils.cuh`

 * *Files 2% similar despite different names*

```diff
@@ -37,30 +37,31 @@
 namespace CoverageControl {
 /*!
  * Get the orientation of the point r with respect to the directional vector
  * from p to q \return 1 if point r is in counter clockwise direction, i.e.,
  * left of the vector \return -1 if point r is in clockwise direction, i.e.,
  * right of the vector \return  0 otherwise
  */
-__device__ int Orientation(float2 const &p, float2 const &q, float2 const &r) {
+__host__ __device__ int Orientation(float2 const &p, float2 const &q,
+                                    float2 const &r) {
   float2 qp{q.x - p.x, q.y - p.y};
   float2 rp{r.x - p.x, r.y - p.y};
   float cross_prod1 = qp.x * rp.y;
   float cross_prod2 = qp.y * rp.x;
   if (cross_prod1 > cross_prod2) return 1;
   if (cross_prod1 < cross_prod2) return -1;
   return 0;
 }
 
 /*!
  * Check if the point r is inside the monotone polygon defined by the vertices x
  * and y \return true if the point is inside the polygon \return false otherwise
  */
-__device__ bool IsPointInMonotonePolygon(float *x, float *y, int sz,
-                                         float2 const &r) {
+__host__ __device__ bool IsPointInMonotonePolygon(float *x, float *y, int sz,
+                                                  float2 const &r) {
   bool left = false;
   bool right = false;
   for (int ct = 0; ct < sz; ++ct) {
     int ctp1 = ct + 1;
     if (ctp1 == sz) {
       ctp1 = 0;
     }
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/cuda_utils.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/cuda_utils.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_cuda.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/cuda_helpers/helper_string.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/gnuplot/gnuplot-iostream.h`

 * *Files 2% similar despite different names*

```diff
@@ -99,32 +99,23 @@
 #    endif
 #else
 #    define GNUPLOT_DEPRECATE(msg)
 #endif
 
 // Patch for Windows by Damien Loison
 #ifdef _WIN32
-#    include <windows.h>
 #    define GNUPLOT_PCLOSE _pclose
 #    define GNUPLOT_POPEN  _popen
 #    define GNUPLOT_FILENO _fileno
 #else
 #    define GNUPLOT_PCLOSE pclose
 #    define GNUPLOT_POPEN  popen
 #    define GNUPLOT_FILENO fileno
 #endif
 
-#ifdef _WIN32
-#    define GNUPLOT_ISNAN _isnan
-#else
-// cppreference.com says std::isnan is only for C++11.  However, this seems to work on Linux
-// and I am assuming that if isnan exists in math.h then std::isnan exists in cmath.
-#    define GNUPLOT_ISNAN std::isnan
-#endif
-
 // MSVC gives a warning saying that fopen and getenv are not secure.  But they are secure.
 // Unfortunately their replacement functions are not simple drop-in replacements.  The best
 // solution is to just temporarily disable this warning whenever fopen or getenv is used.
 // http://stackoverflow.com/a/4805353/1048959
 #if defined(_MSC_VER) && _MSC_VER >= 1400
 #    define GNUPLOT_MSVC_WARNING_4996_PUSH \
         __pragma(warning(push)) \
@@ -137,17 +128,17 @@
 #endif
 
 #ifndef GNUPLOT_DEFAULT_COMMAND
 #ifdef _WIN32
 // "pgnuplot" is considered deprecated according to the Internet.  It may be faster.  It
 // doesn't seem to handle binary data though.
 //#    define GNUPLOT_DEFAULT_COMMAND "pgnuplot -persist"
-// On Windows, gnuplot echos commands to stderr.  So we forward its stderr to the bit bucket.
-// Unfortunately, this means you will miss out on legitimate error messages.
-#    define GNUPLOT_DEFAULT_COMMAND "gnuplot -persist 2> NUL"
+// The default install path for gnuplot is written here.  This way the user doesn't have to add
+// anything to their %PATH% environment variable.
+#    define GNUPLOT_DEFAULT_COMMAND "\"C:\\Program Files\\gnuplot\\bin\\gnuplot.exe\" -persist"
 #else
 #    define GNUPLOT_DEFAULT_COMMAND "gnuplot -persist"
 #endif
 #endif
 
 // }}}1
 
@@ -506,15 +497,15 @@
 template<> struct TextSender<   signed char> : public CastIntTextSender<   signed char> { };
 template<> struct TextSender< unsigned char> : public CastIntTextSender< unsigned char> { };
 
 // Make sure that the same not-a-number string is printed on all platforms.
 template <typename T>
 struct FloatTextSender {
     static void send(std::ostream &stream, const T &v) {
-        if(GNUPLOT_ISNAN(v)) { stream << "nan"; } else { stream << v; }
+        if(std::isnan(v)) { stream << "nan"; } else { stream << v; }
     }
 };
 template<> struct TextSender<      float> : FloatTextSender<      float> { };
 template<> struct TextSender<     double> : FloatTextSender<     double> { };
 template<> struct TextSender<long double> : FloatTextSender<long double> { };
 
 // }}}2
@@ -1638,15 +1629,18 @@
 struct FileHandleWrapper {
     FileHandleWrapper(std::FILE *_fh, bool _should_use_pclose) :
         wrapped_fh(_fh), should_use_pclose(_should_use_pclose) { }
 
     void fh_close() {
         if(should_use_pclose) {
             if(GNUPLOT_PCLOSE(wrapped_fh)) {
-                std::cerr << "pclose returned error: " << strerror(errno) << std::endl;
+                perror("pclose");
+                //char msg[1000];
+                //strerror_s(msg, sizeof(msg), errno);
+                //std::cerr << "pclose returned error: " << msg << std::endl;
             }
         } else {
             if(fclose(wrapped_fh)) {
                 std::cerr << "fclose returned error" << std::endl;
             }
         }
     }
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/json/json.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/Hungarian.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/LICENSE`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/lsap/README.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/extern/tomlplusplus/toml.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/generate_world_map.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/generate_world_map.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/geographiclib_wrapper.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/map_utils.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/map_utils.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/parameters.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/parameters.h`

 * *Files 4% similar despite different names*

```diff
@@ -53,14 +53,17 @@
 
   /*!
    * \name Environment Parameters
    * @{
    */
   int pNumRobots = 32;    //!< Number of robots
   int pNumFeatures = 32;  //!< Number of features
+  int pNumPolygons = 0;   //!< Number of polygonal features
+  int pMaxVertices = 10;  //!< Maximum number of vertices in a polygon
+  double pPolygonRadius = 64;
 
   /*! \name Map Parameters
    * @{
    */
   //! Assuming same resolution in both the directions in meters. Pixel area =
   //! pResolution^2
   double pResolution = 1.0;
```

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/plotter.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/plotter.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/robot_model.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/robot_model.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/typedefs.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/typedefs.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/vec2d.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/vec2d.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/voronoi.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/voronoi.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/include/CoverageControl/world_idf.h` & `coverage_control-1.1.0/cppsrc/core/include/CoverageControl/world_idf.h`

 * *Files 22% similar despite different names*

```diff
@@ -172,14 +172,28 @@
     }
   }
 
   explicit WorldIDF(Parameters const &params) : WorldIDF(params.pWorldMapSize) {
     params_ = params;
   }
 
+  WorldIDF(Parameters const &params, MapType const &world_map)
+      : WorldIDF(params.pWorldMapSize) {
+    params_ = params;
+    if (world_map.rows() != params.pWorldMapSize ||
+        world_map.cols() != params.pWorldMapSize) {
+      std::cout << "Error: World map size does not match the specified size"
+                << std::endl;
+      throw std::invalid_argument(
+          "World map size does not match the specified size");
+      exit(1);
+    }
+    world_map_ = world_map;
+  }
+
   WorldIDF(Parameters const &params, std::string const &file_name)
       : WorldIDF(params.pWorldMapSize) {
     params_ = params;
     // Load Bivariate Normal Distribution from file
     params_ = params;
     std::ifstream file(file_name);
     if (!file.is_open()) {
@@ -197,22 +211,23 @@
         double x, y, sigma, scale;
         file >> x >> y >> sigma >> scale;
         AddNormalDistribution(
             BivariateNormalDistribution(Point2(x, y), sigma, scale));
       } else if (type == "Uniform") {
         int num_vertices;
         file >> num_vertices;
+        double importance;
+        file >>
+            importance;  // importance moved here. Be careful with semantic file
         std::vector<Point2> vertices;
         for (int i = 0; i < num_vertices; ++i) {
           double x, y;
           file >> x >> y;
           vertices.push_back(Point2(x, y));
         }
-        double importance;
-        file >> importance;
         AddUniformDistributionPolygon(PolygonFeature(vertices, importance));
       } else {
         std::cout << "Error: Unknown feature type " << type << std::endl;
         exit(1);
       }
     }
     GenerateMap();
@@ -301,82 +316,23 @@
               << world_map_.cols() << std::endl;
   }
 
   auto GetNormalizationFactor() const { return normalization_factor_; }
 
   const MapType &GetWorldMap() const { return world_map_; }
 
-  inline int WriteDistributions(std::string const &file_name) const {
-    std::ofstream file(file_name);
-    if (!file.is_open()) {
-      std::cerr << "Could not open file: " << file_name << std::endl;
-      return -1;
-    }
-    file << std::setprecision(kMaxPrecision);
-    for (auto const &dist : normal_distributions_) {
-      Point2 sigma = dist.GetSigma();
-      if (sigma.x() == sigma.y()) {
-        file << "CircularBND" << std::endl;
-        file << dist.GetMean().x() << " " << dist.GetMean().y() << " "
-             << sigma.x() << " " << dist.GetScale() << std::endl;
-      } else {
-        file << "BND" << std::endl;
-        file << dist.GetMean().x() << " " << dist.GetMean().y() << " "
-             << dist.GetSigma().x() << " " << dist.GetSigma().y() << " "
-             << dist.GetRho() << " " << dist.GetScale() << std::endl;
-      }
-    }
-    file.close();
-    return 0;
-  }
+  MapType &GetWorldMapMutable() { return world_map_; }
+
+  int WriteDistributions(std::string const &file_name) const;
 
   auto GetNumFeatures() const {
     return normal_distributions_.size() + polygon_features_.size();
   }
 
-  /*! Fills in values of the world_map_ with the total importance for each cell
-   */
-  void GenerateMapCPU() {
-    /* std::cout << "Generating map using CPU" << std::endl; */
-    float max_importance = 0;
-    float res = static_cast<float>(params_.pResolution);
-    for (int i = 0; i < params_.pWorldMapSize; ++i) {  // Row (x index)
-      float x1 = res * i;   // Left x-coordinate of pixel
-      float x2 = x1 + res;  // Right x-coordinate of pixel
-      for (int j = 0; j < params_.pWorldMapSize; ++j) {  // Column (y index)
-        float y1 = res * j;   // Lower y-coordinate of pixel
-        float y2 = y1 + res;  // Upper y-coordinate of pixel
-        float importance = ComputeImportanceBND<Point2f, float>(
-            Point2f(x1, y1), Point2f(x2, y2));
-        /* auto importance = ComputeImportanceBND(pt1, pt2); */
-        /* if (std::abs(importance) < kEps) { */
-        /*   importance = 0; */
-        /* } */
-        world_map_(i, j) = importance;
-        if (importance > max_importance) {
-          max_importance = importance;
-        }
-      }
-    }
-
-    if (max_importance < kEps) {
-      normalization_factor_ = static_cast<float>(params_.pNorm);
-    } else {
-      normalization_factor_ =
-          static_cast<float>(params_.pNorm) / max_importance;
-    }
-
-    // Normalize the world map
-#pragma omp parallel for
-    for (int i = 0; i < params_.pWorldMapSize; ++i) {
-      for (int j = 0; j < params_.pWorldMapSize; ++j) {
-        world_map_(i, j) *= normalization_factor_;
-      }
-    }
-  }
+  void GenerateMapCPU();
 
 #ifdef COVERAGECONTROL_WITH_CUDA
   void GenerateMapCuda() {
     /* std::cout << "Generating map using CUDA" << std::endl; */
     GenerateMapCuda(static_cast<float>(params_.pResolution),
                     static_cast<float>(params_.pTruncationBND),
                     static_cast<int>(params_.pWorldMapSize));
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/coverage_system.cpp` & `coverage_control-1.1.0/cppsrc/core/src/coverage_system.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -28,46 +28,64 @@
 
 #include "CoverageControl/coverage_system.h"
 #include "CoverageControl/plotter.h"
 
 namespace CoverageControl {
 
 CoverageSystem::CoverageSystem(Parameters const &params)
-    : CoverageSystem(params, params.pNumFeatures, params.pNumRobots) {}
+    : CoverageSystem(params, params.pNumFeatures, params.pNumPolygons,
+                     params.pNumRobots) {}
 
-CoverageSystem::CoverageSystem(Parameters const &params, int const num_features,
+CoverageSystem::CoverageSystem(Parameters const &params,
+                               int const num_gaussians, int const num_robots)
+    : CoverageSystem(params, num_gaussians, 0, num_robots) {}
+
+CoverageSystem::CoverageSystem(Parameters const &params,
+                               int const num_gaussians, int const num_polygons,
                                int const num_robots)
     : params_{params}, world_idf_{WorldIDF(params_)} {
   // Generate Bivariate Normal Distribution from random numbers
   std::srand(
       std::time(nullptr));  // use current time as seed for random generator
   gen_ = std::mt19937(
       rd_());  // Standard mersenne_twister_engine seeded with rd_()
   distrib_pts_ = std::uniform_real_distribution<>(
       kLargeEps, params_.pWorldMapSize * params_.pResolution - kLargeEps);
   std::uniform_real_distribution<> distrib_var(params_.pMinSigma,
                                                params_.pMaxSigma);
   std::uniform_real_distribution<> distrib_peak(params_.pMinPeak,
                                                 params_.pMaxPeak);
-  for (int i = 0; i < num_features; ++i) {
+  for (int i = 0; i < num_gaussians; ++i) {
     Point2 mean(distrib_pts_(gen_), distrib_pts_(gen_));
     double sigma(distrib_var(gen_));
     double scale(distrib_peak(gen_));
+    scale = 2 * M_PI * sigma * sigma * scale;
     BivariateNormalDistribution dist(mean, sigma, scale);
     world_idf_.AddNormalDistribution(dist);
   }
 
+  std::vector<PointVector> polygons;
+  GenerateRandomPolygons(num_polygons, params_.pMaxVertices,
+                         params_.pPolygonRadius,
+                         params_.pWorldMapSize * params_.pResolution, polygons);
+
+  for (auto &poly : polygons) {
+    double importance = distrib_peak(gen_) * 0.5;
+    PolygonFeature poly_feature(poly, importance);
+    world_idf_.AddUniformDistributionPolygon(poly_feature);
+  }
+
   world_idf_.GenerateMap();
   normalization_factor_ = world_idf_.GetNormalizationFactor();
 
-  std::uniform_real_distribution<> robot_pos_dist(
+  std::uniform_real_distribution<> env_point_dist(
       kLargeEps, params_.pRobotInitDist - kLargeEps);
   robots_.reserve(num_robots);
   for (int i = 0; i < num_robots; ++i) {
-    Point2 start_pos(robot_pos_dist(gen_), robot_pos_dist(gen_));
+    Point2 start_pos(env_point_dist(gen_), env_point_dist(gen_));
     robots_.push_back(RobotModel(params_, start_pos, world_idf_));
   }
   InitSetup();
 }
 
 CoverageSystem::CoverageSystem(Parameters const &params,
                                WorldIDF const &world_idf,
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/cuda/cuda_utils.cu` & `coverage_control-1.1.0/cppsrc/core/src/cuda/cuda_utils.cu`

 * *Files 7% similar despite different names*

```diff
@@ -33,211 +33,211 @@
 
 #include "CoverageControl/cuda_utils.h"
 #include "CoverageControl/extern/cuda_helpers/helper_cuda.h"
 #include "CoverageControl/extern/cuda_helpers/helper_string.h"
 
 namespace CoverageControl {
 
-bool CheckCudaErrors(cudaError_t result) {
-  if (result != cudaSuccess) {
-    std::cerr << "CUDA error: [" << static_cast<unsigned int>(result) << "] "
-              << cudaGetErrorString(result) << std::endl;
-    return false;
-  }
-  return true;
-}
-
-bool CudaUtils::GetDeviceCount(int &device_count) {
-  CheckCudaErrors(cudaGetDeviceCount(&device_count));
-  if (device_count == 0) {
-    /* std::cerr << "No CUDA devices found" << std::endl; */
-    return false;
-  }
-  return true;
-}
-
-int CudaUtils::GPUDeviceInit(int dev_id) {
-  int device_count;
-  bool device_count_success = GetDeviceCount(device_count);
-  if (!device_count_success) {
-    return -1;
-  }
-
-  if (dev_id < 0) {
-    dev_id = 0;
+  bool CheckCudaErrors(cudaError_t result) {
+    if (result != cudaSuccess) {
+      std::cerr << "CUDA error: [" << static_cast<unsigned int>(result) << "] "
+        << cudaGetErrorString(result) << std::endl;
+      return false;
+    }
+    return true;
   }
 
-  if (dev_id > device_count - 1) {
-    std::cerr << "Invalid GPU device ID" << std::endl;
-    std::cerr << "Device ID: " << dev_id << " Device Count: " << device_count
-              << std::endl;
-    return -1;
+  bool CudaUtils::GetDeviceCount(int &device_count) {
+    CheckCudaErrors(cudaGetDeviceCount(&device_count));
+    if (device_count == 0) {
+      /* std::cerr << "No CUDA devices found" << std::endl; */
+      return false;
+    }
+    return true;
   }
 
-  int compute_mode = -1, major = 0, minor = 0;
-  CheckCudaErrors(
-      cudaDeviceGetAttribute(&compute_mode, cudaDevAttrComputeMode, dev_id));
-  CheckCudaErrors(cudaDeviceGetAttribute(
-      &major, cudaDevAttrComputeCapabilityMajor, dev_id));
-  CheckCudaErrors(cudaDeviceGetAttribute(
-      &minor, cudaDevAttrComputeCapabilityMinor, dev_id));
-  if (compute_mode == cudaComputeModeProhibited) {
-    std::cerr << "Error: device is running in <Compute Mode Prohibited>, no "
-                 "threads can use cudaSetDevice()."
-              << std::endl;
-    return -1;
-  }
+  int CudaUtils::GPUDeviceInit(int dev_id) {
+    int device_count;
+    bool device_count_success = GetDeviceCount(device_count);
+    if (!device_count_success) {
+      return -1;
+    }
 
-  if (major < 1) {
-    std::cerr << "GPUDeviceInit(): GPU device does not support CUDA."
-              << std::endl;
-    return -1;
-  }
+    if (dev_id < 0) {
+      dev_id = 0;
+    }
 
-  CheckCudaErrors(cudaSetDevice(dev_id));
-  std::cout << "GPU Device " << dev_id << " has been set" << std::endl;
-  std::cout << "CUDA Device [" << dev_id << "]: \""
-            << _ConvertSMVer2ArchName(major, minor) << "\"" << std::endl;
-  is_cuda_initialized_ = true;
-  device_id_ = dev_id;
-  return dev_id;
-}
-
-int CudaUtils::FindDevice() { return GPUGetMaxGflopsDeviceId(); }
-
-int CudaUtils::FindIntegratedGPU() {
-  int current_device = 0;
-  int device_count = 0;
-  int devices_prohibited = 0;
+    if (dev_id > device_count - 1) {
+      std::cerr << "Invalid GPU device ID" << std::endl;
+      std::cerr << "Device ID: " << dev_id << " Device Count: " << device_count
+        << std::endl;
+      return -1;
+    }
 
-  CheckCudaErrors(cudaGetDeviceCount(&device_count));
+    int compute_mode = -1, major = 0, minor = 0;
+    CheckCudaErrors(
+        cudaDeviceGetAttribute(&compute_mode, cudaDevAttrComputeMode, dev_id));
+    CheckCudaErrors(cudaDeviceGetAttribute(
+          &major, cudaDevAttrComputeCapabilityMajor, dev_id));
+    CheckCudaErrors(cudaDeviceGetAttribute(
+          &minor, cudaDevAttrComputeCapabilityMinor, dev_id));
+    if (compute_mode == cudaComputeModeProhibited) {
+      std::cerr << "Error: device is running in <Compute Mode Prohibited>, no "
+        "threads can use cudaSetDevice()."
+        << std::endl;
+      return -1;
+    }
 
-  if (device_count == 0) {
-    /* std::cerr << "No CUDA devices found" << std::endl; */
-    return -1;
-  }
+    if (major < 1) {
+      std::cerr << "GPUDeviceInit(): GPU device does not support CUDA."
+        << std::endl;
+      return -1;
+    }
 
-  // Find the integrated GPU which is compute capable
-  while (current_device < device_count) {
-    int compute_mode = -1, integrated = -1;
-    CheckCudaErrors(cudaDeviceGetAttribute(
-        &compute_mode, cudaDevAttrComputeMode, current_device));
-    CheckCudaErrors(cudaDeviceGetAttribute(&integrated, cudaDevAttrIntegrated,
-                                           current_device));
-    // If GPU is integrated and is not running on Compute Mode prohibited,
-    // then cuda can map to GLES resource
-    if (integrated && (compute_mode != cudaComputeModeProhibited)) {
-      CheckCudaErrors(cudaSetDevice(current_device));
+    CheckCudaErrors(cudaSetDevice(dev_id));
+    std::cout << "GPU Device " << dev_id << " has been set" << std::endl;
+    std::cout << "CUDA Device [" << dev_id << "]: \""
+      << _ConvertSMVer2ArchName(major, minor) << "\"" << std::endl;
+    is_cuda_initialized_ = true;
+    device_id_ = dev_id;
+    return dev_id;
+  }
+
+  int CudaUtils::FindDevice() { return GPUGetMaxGflopsDeviceId(); }
+
+  int CudaUtils::FindIntegratedGPU() {
+    int current_device = 0;
+    int device_count = 0;
+    int devices_prohibited = 0;
+
+    CheckCudaErrors(cudaGetDeviceCount(&device_count));
+
+    if (device_count == 0) {
+      /* std::cerr << "No CUDA devices found" << std::endl; */
+      return -1;
+    }
 
-      int major = 0, minor = 0;
-      CheckCudaErrors(cudaDeviceGetAttribute(
-          &major, cudaDevAttrComputeCapabilityMajor, current_device));
+    // Find the integrated GPU which is compute capable
+    while (current_device < device_count) {
+      int compute_mode = -1, integrated = -1;
       CheckCudaErrors(cudaDeviceGetAttribute(
-          &minor, cudaDevAttrComputeCapabilityMinor, current_device));
-      std::cout << "GPU Device " << current_device << " has been set"
-                << std::endl;
-      std::cout << "CUDA Device [" << current_device << "]: \""
-                << _ConvertSMVer2ArchName(major, minor) << "\"" << std::endl;
-      return current_device;
-    } else {
-      devices_prohibited++;
+            &compute_mode, cudaDevAttrComputeMode, current_device));
+      CheckCudaErrors(cudaDeviceGetAttribute(&integrated, cudaDevAttrIntegrated,
+            current_device));
+      // If GPU is integrated and is not running on Compute Mode prohibited,
+      // then cuda can map to GLES resource
+      if (integrated && (compute_mode != cudaComputeModeProhibited)) {
+        CheckCudaErrors(cudaSetDevice(current_device));
+
+        int major = 0, minor = 0;
+        CheckCudaErrors(cudaDeviceGetAttribute(
+              &major, cudaDevAttrComputeCapabilityMajor, current_device));
+        CheckCudaErrors(cudaDeviceGetAttribute(
+              &minor, cudaDevAttrComputeCapabilityMinor, current_device));
+        std::cout << "GPU Device " << current_device << " has been set"
+          << std::endl;
+        std::cout << "CUDA Device [" << current_device << "]: \""
+          << _ConvertSMVer2ArchName(major, minor) << "\"" << std::endl;
+        return current_device;
+      } else {
+        devices_prohibited++;
+      }
+
+      current_device++;
     }
 
-    current_device++;
-  }
+    if (devices_prohibited == device_count) {
+      std::cerr << "CUDA error: No Integrated GPU found that supports CUDA."
+        << std::endl;
+      return -1;
+    }
 
-  if (devices_prohibited == device_count) {
-    std::cerr << "CUDA error: No Integrated GPU found that supports CUDA."
-              << std::endl;
     return -1;
   }
 
-  return -1;
-}
+  /*!
+   * \brief Provides a way to select the best GPU based on maximum GFLOPS
+   * \return The device ID of the GPU with the maximum GFLOPS
+   * \return -1 if no device is found
+   * See: extern/cuda_helpers/helper_cuda.h
+   */
+  int CudaUtils::GPUGetMaxGflopsDeviceId(std::vector<int> device_list) {
+    int sm_per_multiproc = 0;
+    int max_perf_device = 0;
+    int device_count = 0;
+    int devices_prohibited = 0;
 
-/*!
- * \brief Provides a way to select the best GPU based on maximum GFLOPS
- * \return The device ID of the GPU with the maximum GFLOPS
- * \return -1 if no device is found
- * See: extern/cuda_helpers/helper_cuda.h
- */
-int CudaUtils::GPUGetMaxGflopsDeviceId(std::vector<int> device_list) {
-  int sm_per_multiproc = 0;
-  int max_perf_device = 0;
-  int device_count = 0;
-  int devices_prohibited = 0;
+    uint64_t max_compute_perf = 0;
 
-  uint64_t max_compute_perf = 0;
-
-  if (GetDeviceCount(device_count) == false) {
-    return -1;
-  }
+    if (GetDeviceCount(device_count) == false) {
+      return -1;
+    }
 
-  if (device_count == 0) {
-    /* std::cerr << "No CUDA devices found" << std::endl; */
-    return -1;
-  }
+    if (device_count == 0) {
+      /* std::cerr << "No CUDA devices found" << std::endl; */
+      return -1;
+    }
 
-  if (device_list.size() == 0) {
-    for (int i = 0; i < device_count; i++) {
-      device_list.push_back(i);
+    if (device_list.size() == 0) {
+      for (int i = 0; i < device_count; i++) {
+        device_list.push_back(i);
+      }
     }
-  }
 
-  while (device_list.size() > 0) {
-    int current_device = device_list.back();
-    device_list.pop_back();
-    int compute_mode = -1, major = 0, minor = 0;
-    CheckCudaErrors(cudaDeviceGetAttribute(
-        &compute_mode, cudaDevAttrComputeMode, current_device));
-    CheckCudaErrors(cudaDeviceGetAttribute(
-        &major, cudaDevAttrComputeCapabilityMajor, current_device));
-    CheckCudaErrors(cudaDeviceGetAttribute(
-        &minor, cudaDevAttrComputeCapabilityMinor, current_device));
+    while (device_list.size() > 0) {
+      int current_device = device_list.back();
+      device_list.pop_back();
+      int compute_mode = -1, major = 0, minor = 0;
+      CheckCudaErrors(cudaDeviceGetAttribute(
+            &compute_mode, cudaDevAttrComputeMode, current_device));
+      CheckCudaErrors(cudaDeviceGetAttribute(
+            &major, cudaDevAttrComputeCapabilityMajor, current_device));
+      CheckCudaErrors(cudaDeviceGetAttribute(
+            &minor, cudaDevAttrComputeCapabilityMinor, current_device));
 
-    // If this GPU is not running on Compute Mode prohibited,
-    // then we can add it to the list
-    if (compute_mode != cudaComputeModeProhibited) {
-      if (major == 9999 && minor == 9999) {
-        sm_per_multiproc = 1;
-      } else {
-        sm_per_multiproc = _ConvertSMVer2Cores(major, minor);
-      }
-      int multiProcessorCount = 0, clockRate = 0;
-      CheckCudaErrors(cudaDeviceGetAttribute(&multiProcessorCount,
-                                             cudaDevAttrMultiProcessorCount,
-                                             current_device));
-      cudaError_t result = cudaDeviceGetAttribute(
-          &clockRate, cudaDevAttrClockRate, current_device);
-      if (result != cudaSuccess) {
-        // If cudaDevAttrClockRate attribute is not supported we
-        // set clockRate as 1, to consider GPU with most SMs and CUDA Cores.
-        if (result == cudaErrorInvalidValue) {
-          clockRate = 1;
+      // If this GPU is not running on Compute Mode prohibited,
+      // then we can add it to the list
+      if (compute_mode != cudaComputeModeProhibited) {
+        if (major == 9999 && minor == 9999) {
+          sm_per_multiproc = 1;
         } else {
-          fprintf(stderr, "CUDA error at %s:%d code=%d(%s) \n", __FILE__,
-                  __LINE__, static_cast<unsigned int>(result),
-                  _cudaGetErrorEnum(result));
-          return -1;
+          sm_per_multiproc = _ConvertSMVer2Cores(major, minor);
         }
-      }
-      uint64_t compute_perf =
+        int multiProcessorCount = 0, clockRate = 0;
+        CheckCudaErrors(cudaDeviceGetAttribute(&multiProcessorCount,
+              cudaDevAttrMultiProcessorCount,
+              current_device));
+        cudaError_t result = cudaDeviceGetAttribute(
+            &clockRate, cudaDevAttrClockRate, current_device);
+        if (result != cudaSuccess) {
+          // If cudaDevAttrClockRate attribute is not supported we
+          // set clockRate as 1, to consider GPU with most SMs and CUDA Cores.
+          if (result == cudaErrorInvalidValue) {
+            clockRate = 1;
+          } else {
+            fprintf(stderr, "CUDA error at %s:%d code=%d(%s) \n", __FILE__,
+                __LINE__, static_cast<unsigned int>(result),
+                _cudaGetErrorEnum(result));
+            return -1;
+          }
+        }
+        uint64_t compute_perf =
           (uint64_t)multiProcessorCount * sm_per_multiproc * clockRate;
 
-      if (compute_perf > max_compute_perf) {
-        max_compute_perf = compute_perf;
-        max_perf_device = current_device;
+        if (compute_perf > max_compute_perf) {
+          max_compute_perf = compute_perf;
+          max_perf_device = current_device;
+        }
+      } else {
+        devices_prohibited++;
       }
-    } else {
-      devices_prohibited++;
     }
-  }
 
-  if (devices_prohibited == device_count) {
-    std::cerr << "GPUGetMaxGflopsDeviceId() CUDA error:"
-              << " all devices have compute mode prohibited." << std::endl;
-    return -1;
-  }
+    if (devices_prohibited == device_count) {
+      std::cerr << "GPUGetMaxGflopsDeviceId() CUDA error:"
+        << " all devices have compute mode prohibited." << std::endl;
+      return -1;
+    }
 
-  return max_perf_device;
-}
+    return max_perf_device;
+  }
 } /* namespace CoverageControl */
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/cuda/generate_world_map.cu` & `coverage_control-1.1.0/cppsrc/core/src/cuda/generate_world_map.cu`

 * *Files 0% similar despite different names*

```diff
@@ -38,17 +38,17 @@
 #include <cuda_runtime.h>
 #include <thrust/device_ptr.h>
 #include <thrust/extrema.h>
 
 #include <cmath>
 
 #include "CoverageControl/constants.h"
+#include "CoverageControl/cuda/geometry_utils.cuh"
 #include "CoverageControl/extern/cuda_helpers/helper_cuda.h"
 #include "CoverageControl/generate_world_map.h"
-#include "CoverageControl/cuda/geometry_utils.cuh"
 
 namespace CoverageControl {
 __device__ __constant__ int cu_num_dists;
 __device__ __constant__ int cu_map_size;
 __device__ __constant__ float cu_resolution;
 __device__ __constant__ float cu_truncation;
 __device__ __constant__ float cu_trun_sq;
@@ -274,7 +274,8 @@
   if (error != cudaSuccess) {
     std::stringstream strstr;
     strstr << "run_kernel launch failed" << std::endl;
     throw strstr.str();
   }
 }
 } /* namespace CoverageControl */
+
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/cuda_utils.cpp` & `coverage_control-1.1.0/cppsrc/core/src/cuda_utils.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/src/extern/Hungarian.cpp` & `coverage_control-1.1.0/cppsrc/core/src/extern/Hungarian.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/src/parameters.cpp` & `coverage_control-1.1.0/cppsrc/core/src/parameters.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -55,19 +55,37 @@
     }
     pNumRobots = toml_config["NumRobots"].value<int>().value();
   } else {
     std::cout << "NumRobots (default): " << pNumRobots << std::endl;
   }
 
   if (toml_config["NumFeatures"].value<int>()) {
-    pNumFrontiers = toml_config["NumFeatures"].value<int>().value();
+    pNumFeatures = toml_config["NumFeatures"].value<int>().value();
   } else {
     std::cout << "NumFeatures (default): " << pNumFeatures << std::endl;
   }
 
+  if (toml_config["NumPolygons"].value<int>()) {
+    pNumPolygons = toml_config["NumPolygons"].value<int>().value();
+  } else {
+    std::cout << "NumPolygons (default): " << pNumPolygons << std::endl;
+  }
+
+  if (toml_config["MaxVertices"].value<int>()) {
+    pMaxVertices = toml_config["MaxVertices"].value<int>().value();
+  } else {
+    std::cout << "MaxVertices (default): " << pMaxVertices << std::endl;
+  }
+
+  if (toml_config["PolygonRadius"].value<double>()) {
+    pPolygonRadius = toml_config["PolygonRadius"].value<double>().value();
+  } else {
+    std::cout << "PolygonRadius (default): " << pPolygonRadius << std::endl;
+  }
+
   auto toml_EnvironmentMaps = toml_config["Environment.Maps"];
 
   if (toml_EnvironmentMaps) {
     auto toml_Resolution = toml_EnvironmentMaps["Resolution"].value<double>();
     auto toml_WorldMapSize = toml_EnvironmentMaps["WorldMapSize"].value<int>();
     auto toml_RobotMapSize = toml_EnvironmentMaps["RobotMapSize"].value<int>();
     auto toml_LocalMapSize = toml_EnvironmentMaps["LocalMapSize"].value<int>();
@@ -219,22 +237,25 @@
     if (toml_LloydNumTries) {
       pLloydNumTries = toml_LloydNumTries.value();
     }
 
     auto toml_NumFrontiers =
         toml_Algorithm["Exploration.NumFrontiers"].value<int>();
     if (toml_NumFrontiers) {
-      pNumFrontiers = toml_NumFrontiers.value();
+      pNumFeatures = toml_NumFrontiers.value();
     }
   }
 }
 
 void Parameters::PrintParameters() {
   std::cout << "NumRobots: " << pNumRobots << std::endl;
-  std::cout << "NumFrontiers: " << pNumFrontiers << std::endl;
+  std::cout << "NumFeatures: " << pNumFeatures << std::endl;
+  std::cout << "NumPolygons: " << pNumPolygons << std::endl;
+  std::cout << "MaxVertices: " << pMaxVertices << std::endl;
+  std::cout << "PolygonRadius" << pPolygonRadius << std::endl;
 
   std::cout << "Resolution: " << pResolution << std::endl;
   std::cout << "WorldMapSize: " << pWorldMapSize << std::endl;
   std::cout << "RobotMapSize: " << pRobotMapSize << std::endl;
   std::cout << "LocalMapSize: " << pLocalMapSize << std::endl;
 
   std::cout << "UpdateRobotMap: " << pUpdateRobotMap << std::endl;
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/plotter.cpp` & `coverage_control-1.1.0/cppsrc/core/src/plotter.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/core/src/polygon_utils.cpp` & `coverage_control-1.1.0/cppsrc/tests/simultaneous_explore_exploit.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -17,51 +17,82 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU General
  * Public License for more details.
  *
  * You should have received a copy of the GNU General Public License along with
  * CoverageControl library. If not, see <https://www.gnu.org/licenses/>.
  */
 
-/*!
- * \file polygon_utils.cpp
- * \brief Helper functions for polygon operations using CGAL
- */
-
-#include <list>
-#include <vector>
-
-#include "CoverageControl/cgal/config.h"
-#include "CoverageControl/cgal/polygon_utils.h"
-#include "CoverageControl/cgal/utilities.h"
-
-namespace CoverageControl {
-void PolygonYMonotonePartition(PointVector const &poly,
-                               std::vector<PointVector> &new_polys) {
-  // Transform general polygon to CGAL //
-  Partition_traits_2::Polygon_2 cgal_poly;
-  for (auto const &pt : poly) {
-    cgal_poly.push_back(Partition_traits_2::Point_2(pt.x(), pt.y()));
+#include <CoverageControl/algorithms/oracle_bang_explore_exploit.h>
+#include <CoverageControl/algorithms/oracle_explore_exploit.h>
+#include <CoverageControl/algorithms/simul_explore_exploit.h>
+#include <CoverageControl/bivariate_normal_distribution.h>
+#include <CoverageControl/constants.h>
+#include <CoverageControl/coverage_system.h>
+#include <CoverageControl/generate_world_map.h>
+#include <CoverageControl/parameters.h>
+#include <CoverageControl/robot_model.h>
+#include <CoverageControl/typedefs.h>
+#include <CoverageControl/world_idf.h>
+
+#include <chrono>
+#include <cstdlib>
+#include <fstream>
+#include <iomanip>
+#include <iostream>
+#include <random>
+#include <string>
+
+using namespace CoverageControl;
+
+int main(int argc, char** argv) {
+  Parameters params;
+  /* params.pSensorSize = 16; */
+  /* params.pMaxRobotSpeed = 10; */
+  if (argc == 2) {
+    std::string parameter_file = argv[1];
+    params = Parameters(parameter_file);
   }
 
-  /* std::cout << "Is simple: " << cgal_poly.is_simple() << std::endl; */
-  /* std::cout << "Is orientation: " << cgal_poly.orientation() << std::endl; */
-  if (cgal_poly.orientation() == CGAL::CLOCKWISE) {
-    cgal_poly.reverse_orientation();
+  PointVector frontiers;
+  int num_robots = 15;
+  int num_dists = 10;
+  CoverageSystem env(params, num_dists, num_robots);
+  OracleSimulExploreExploit oracle(params, num_robots, env);
+
+  std::string dir = "data/oracle/";
+  env.PlotWorldMap(dir, "world_map");
+  env.RecordPlotData();
+  for (int ii = 1; ii < params.pEpisodeSteps; ++ii) {
+    std::cout << "Step: " << ii << std::endl;
+    bool cont_flag = oracle.Step();
+    auto actions = oracle.GetActions();
+    if (env.StepActions(actions)) {
+      std::cerr << "Error: StepActions" << std::endl;
+      break;
+    }
+    auto robot_status = oracle.GetRobotStatus();
+    if (ii % 1 == 0) {
+      frontiers = oracle.GetFrontiers();
+      env.RecordPlotData(robot_status);
+    }
+    if (cont_flag == false) {
+      break;
+    }
   }
-  // Obtain partition //
-  std::list<Partition_traits_2::Polygon_2> partition_polys;
-  CGAL::y_monotone_partition_2(cgal_poly.begin(), cgal_poly.end(),
-                               std::back_inserter(partition_polys));
-
-  // Transform to coveragecontrol data type
-
-  new_polys.reserve(new_polys.size() + partition_polys.size());
-  for (auto const &p : partition_polys) {
-    PointVector new_p;
-    new_p.reserve(p.size());
-    std::transform(p.vertices_begin(), p.vertices_end(),
-                   std::back_inserter(new_p),
-                   [](CGAL_Point2 const &pt) { return CGALtoCC(pt); });
-    new_polys.push_back(new_p);
+  std::cout << "Converged" << std::endl;
+  std::cout << "Exploration ratio: " << env.GetExplorationRatio()
+            << " Weighted: " << env.GetWeightedExplorationRatio() << std::endl;
+
+  auto robot_status = oracle.GetRobotStatus();
+  auto zero_actions = PointVector(num_robots, Point2(0, 0));
+
+  for (int ii = 0; ii < 90; ++ii) {
+    if (env.StepActions(zero_actions)) {
+      std::cerr << "Error: StepActions" << std::endl;
+      break;
+    }
+    env.RecordPlotData(robot_status);
   }
+  env.RenderRecordedMap(dir, "CoverageControl_ExploreExploit.mp4");
+
+  return 0;
 }
-} /* namespace CoverageControl */
```

### Comparing `coverage_control-1.0.0/cppsrc/core/src/voronoi.cpp` & `coverage_control-1.1.0/cppsrc/core/src/voronoi.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/CMakeLists.txt` & `coverage_control-1.1.0/cppsrc/main/CMakeLists.txt`

 * *Files 9% similar despite different names*

```diff
@@ -42,12 +42,16 @@
 ## Executables ##
 #################
 
 add_executable(coverage_algorithm coverage_algorithm.cpp)
 target_link_libraries(coverage_algorithm PRIVATE CoverageControl::CoverageControl)
 install(TARGETS coverage_algorithm DESTINATION ${CMAKE_INSTALL_BINDIR})
 
+add_executable(world_idf world_idf.cpp)
+target_link_libraries(world_idf PRIVATE CoverageControl::CoverageControl)
+install(TARGETS world_idf DESTINATION ${CMAKE_INSTALL_BINDIR})
+
 # if(WITH_TORCH)
 # 	add_executable(eval_dist_gnn torch/eval_dist_gnn.cpp)
 # 	target_link_libraries(eval_dist_gnn PRIVATE compiler_flags CoverageControl CoverageControlTorch ${CUDA_cusparse_LIBRARY})
 # 	install(TARGETS eval_dist_gnn DESTINATION ${CMAKE_INSTALL_BINDIR})
 # endif()
```

### Comparing `coverage_control-1.0.0/cppsrc/main/coverage_algorithm.cpp` & `coverage_control-1.1.0/cppsrc/main/coverage_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/data_generation.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/data_generation.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/eval_dist_gnn.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/eval_dist_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/eval_gnn.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/eval_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/test_cnn.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/test_cnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/train_cnn.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/train_cnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/main/torch/train_gnn.cpp` & `coverage_control-1.1.0/cppsrc/main/torch/train_gnn.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/python_bindings/core_binds.h` & `coverage_control-1.1.0/cppsrc/python_bindings/core_binds.h`

 * *Files 3% similar despite different names*

```diff
@@ -64,14 +64,17 @@
 
   m.def(
       "Point2", []() { return Point2(0, 0); },
       "Create a Point2 object with both values 0");
   m.def(
       "Point2", [](double const &a, double const &b) { return Point2(a, b); },
       "Create a Point2 object with values a and b");
+  m.def(
+      "Point2", [](Point2 const &p) { return Point2(p); },
+      "Create a Point2 object with values from another Point2 object");
 
   m.def(
       "Point2f", []() { return Point2f(0, 0); },
       "Create a Point2f object with both values 0");
   m.def(
       "Point2f", [](float const &a, float const &b) { return Point2f(a, b); },
       "Create a Point2f object with values a and b");
@@ -108,28 +111,31 @@
       .def("GetScale", &BivariateNormalDistribution::GetScale);
 
   py::bind_vector<BNDVector>(m, "BNDVector");
 
   py::class_<WorldIDF>(m, "WorldIDF")
       .def(py::init<Parameters const &>())
       .def(py::init<Parameters const &, std::string const &>())
+      .def(py::init<Parameters const &, MapType const &>())
       .def("AddUniformDistributionPolygon",
            &WorldIDF::AddUniformDistributionPolygon)
       .def("AddNormalDistribution",
            py::overload_cast<BivariateNormalDistribution const &>(
                &WorldIDF::AddNormalDistribution))
       .def("AddNormalDistribution", py::overload_cast<BNDVector const &>(
                                         &WorldIDF::AddNormalDistribution))
       .def("GenerateMap", &WorldIDF::GenerateMap)
       .def("GenerateMapCPU", &WorldIDF::GenerateMapCPU)
 #ifdef COVERAGECONTROL_WITH_CUDA
       .def("GenerateMapCuda", py::overload_cast<>(&WorldIDF::GenerateMapCuda))
 #endif
       .def("GetWorldMap", &WorldIDF::GetWorldMap,
            py::return_value_policy::reference_internal)
+      .def("GetWorldMapMutable", &WorldIDF::GetWorldMapMutable,
+           py::return_value_policy::reference_internal)
       .def("WriteWorldMap", &WorldIDF::WriteWorldMap)
       .def("GetNormalizationFactor", &WorldIDF::GetNormalizationFactor)
       .def("PrintMapSize", &WorldIDF::PrintMapSize)
       .def("LoadMap", &WorldIDF::LoadMap)
       .def("WriteDistributions", &WorldIDF::WriteDistributions)
       .def("GetNumFeatures", &WorldIDF::GetNumFeatures);
 
@@ -222,14 +228,17 @@
 
   py::class_<Parameters>(m, "Parameters")
       .def(py::init<>())
       .def(py::init<std::string const &>())
       .def("SetConfig", &Parameters::SetConfig)
       .def_readwrite("pNumRobots", &Parameters::pNumRobots)
       .def_readwrite("pNumFeatures", &Parameters::pNumFeatures)
+      .def_readwrite("pNumPolygons", &Parameters::pNumPolygons)
+      .def_readwrite("pMaxVertices", &Parameters::pMaxVertices)
+      .def_readwrite("pPolygonRadius", &Parameters::pPolygonRadius)
       .def_readwrite("pResolution", &Parameters::pResolution)
       .def_readwrite("pWorldMapSize", &Parameters::pWorldMapSize)
       .def_readwrite("pRobotMapSize", &Parameters::pRobotMapSize)
       .def_readwrite("pUnknownImportance", &Parameters::pUnknownImportance)
       .def_readwrite("pLocalMapSize", &Parameters::pLocalMapSize)
       .def_readwrite("pCommunicationRange", &Parameters::pCommunicationRange)
       .def_readwrite("pRobotInitDist", &Parameters::pRobotInitDist)
@@ -256,22 +265,25 @@
   /*     .def("Reverse", &GeoLocalTransform::Reverse); */
 }
 
 void pyCoverageControl_core_coverage_system(py::module &m) {
   py::class_<CoverageSystem>(m, "CoverageSystem")
       .def(py::init<Parameters const &>())
       .def(py::init<Parameters const &, int const, int const>())
+      .def(py::init<Parameters const &, int const, int const, int const>())
       .def(
           py::init<Parameters const &, WorldIDF const &, PointVector const &>())
       .def(
           py::init<Parameters const &, WorldIDF const &, std::string const &>())
       .def(py::init<Parameters const &, BNDVector const &,
                     PointVector const &>())
       .def("GetWorldMap", &CoverageSystem::GetWorldMap,
            py::return_value_policy::reference_internal)
+      .def("GetWorldMapMutable", &CoverageSystem::GetWorldMapMutable,
+           py::return_value_policy::reference_internal)
       .def("GetWorldIDFObject", &CoverageSystem::GetWorldIDFObject,
            py::return_value_policy::reference_internal)
       .def("StepControl", &CoverageSystem::StepControl)
       .def("StepAction", &CoverageSystem::StepAction)
       .def("StepActions", &CoverageSystem::StepActions)
       .def("SetLocalRobotPositions", &CoverageSystem::SetLocalRobotPositions)
       .def("SetLocalRobotPosition", &CoverageSystem::SetLocalRobotPosition)
@@ -312,14 +324,16 @@
            py::overload_cast<>(&CoverageSystem::GetRobotVoronoiFeatures),
            py::return_value_policy::copy)
       .def("GetRobotExplorationFeatures",
            py::overload_cast<>(&CoverageSystem::GetRobotExplorationFeatures),
            py::return_value_policy::copy)
       .def("GetRobotExplorationMap", &CoverageSystem::GetRobotExplorationMap,
            py::return_value_policy::reference_internal)
+      .def("GetSystemExplorationMap", &CoverageSystem::GetSystemExplorationMap,
+           py::return_value_policy::reference_internal)
       .def("GetSystemMap", &CoverageSystem::GetSystemMap,
            py::return_value_policy::reference_internal)
       .def("GetObjectiveValue", &CoverageSystem::GetObjectiveValue)
       .def("PlotSystemMap", py::overload_cast<std::string const &>(
                                 &CoverageSystem::PlotSystemMap, py::const_))
       .def("PlotSystemMap", py::overload_cast<std::string const &, int const &>(
                                 &CoverageSystem::PlotSystemMap, py::const_))
```

### Comparing `coverage_control-1.0.0/cppsrc/python_bindings/python_binds.cpp` & `coverage_control-1.1.0/cppsrc/python_bindings/python_binds.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/setup.sh` & `coverage_control-1.1.0/cppsrc/setup.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/CMakeLists.txt` & `coverage_control-1.1.0/cppsrc/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/geo_transforms.cpp` & `coverage_control-1.1.0/cppsrc/tests/geo_transforms.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/map_generation.cpp` & `coverage_control-1.1.0/cppsrc/tests/map_generation.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/torch/torch_data_loader.cpp` & `coverage_control-1.1.0/cppsrc/tests/torch/torch_data_loader.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/torch/torch_map_conversion.cpp` & `coverage_control-1.1.0/cppsrc/tests/torch/torch_map_conversion.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/torch/torch_normalization.cpp` & `coverage_control-1.1.0/cppsrc/tests/torch/torch_normalization.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/torch/torch_scripting.cpp` & `coverage_control-1.1.0/cppsrc/tests/torch/torch_scripting.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/tests/torch/torch_test.cpp` & `coverage_control-1.1.0/cppsrc/tests/torch/torch_test.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/CMakeLists.txt` & `coverage_control-1.1.0/cppsrc/torch/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in` & `coverage_control-1.1.0/cppsrc/torch/cmake/CoverageControlTorchConfig.cmake.in`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/base.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/base.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_backbone.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/cnn_module.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/coverage_system.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/edge_wts_comm_map_generator.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/extern/tomlplusplus/toml.hpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/generate_dataset.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/gnn_backbone.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/mlp.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/mlp.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/train_cnn.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h` & `coverage_control-1.1.0/cppsrc/torch/include/CoverageControlTorch/type_conversions.h`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/python_bindings/CMakeLists.txt` & `coverage_control-1.1.0/cppsrc/torch/python_bindings/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp` & `coverage_control-1.1.0/cppsrc/torch/python_bindings/src/coverage_control_torch_extension.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/src/base.cpp` & `coverage_control-1.1.0/cppsrc/torch/src/base.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/cppsrc/torch/src/coverage_system.cpp` & `coverage_control-1.1.0/cppsrc/torch/src/coverage_system.cpp`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/Doxyfile` & `coverage_control-1.1.0/doc/Doxyfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/bash-filter.py` & `coverage_control-1.1.0/doc/bash-filter.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/BaseDoxyfile` & `coverage_control-1.1.0/doc/config/BaseDoxyfile`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/DoxygenLayout.xml` & `coverage_control-1.1.0/doc/config/DoxygenLayout.xml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/custom.css` & `coverage_control-1.1.0/doc/config/custom.css`

 * *Files 4% similar despite different names*

```diff
@@ -63,21 +63,21 @@
     vertical-align: middle;
     margin-right: 2px;
     font-family: serif;
     height: auto;
     text-align: right;
 }
 
-#nav-tree a:focus {
-    outline-style: none;
-}
+/* #nav-tree a:focus { */
+/*     outline-style: none; */
+/* } */
 
-#nav-tree .selected .arrow {
-		opacity: var(--side-nav-arrow-hover-opacity)
-}
+/* #nav-tree .selected .arrow { */
+/* 		opacity: var(--side-nav-arrow-hover-opacity) */
+/* } */
 
 #nav-tree a:focus .arrow {
     font-size: 60%;
 }
 
 html {
     /* --page-font-size: 15px; */
```

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-darkmode-toggle.js` & `coverage_control-1.1.0/doc/config/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-fragment-copy-button.js` & `coverage_control-1.1.0/doc/config/doxygen-awesome-fragment-copy-button.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-interactive-toc.js` & `coverage_control-1.1.0/doc/config/doxygen-awesome-interactive-toc.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-paragraph-link.js` & `coverage_control-1.1.0/doc/config/doxygen-awesome-paragraph-link.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-sidebar-only.css` & `coverage_control-1.1.0/doc/config/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome-tabs.js` & `coverage_control-1.1.0/doc/config/doxygen-awesome-tabs.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/doxygen-awesome.css` & `coverage_control-1.1.0/doc/config/doxygen-awesome.css`

 * *Files 1% similar despite different names*

```diff
@@ -330,14 +330,15 @@
 p.reference, p.definition {
     color: var(--page-secondary-foreground-color);
 }
 
 a:link, a:visited, a:hover, a:focus, a:active {
     color: var(--primary-color) !important;
     font-weight: 500;
+    background: none;
 }
 
 a.anchor {
     scroll-margin-top: var(--spacing-large);
     display: block;
 }
 
@@ -802,14 +803,18 @@
 }
 
 #nav-tree .item {
     height: var(--tree-item-height);
     line-height: var(--tree-item-height);
 }
 
+#nav-tree .item > a:focus {
+    outline: none;
+}
+
 #nav-sync {
     bottom: 12px;
     right: 12px;
     top: auto !important;
     user-select: none;
 }
 
@@ -839,14 +844,15 @@
 
 #nav-tree a:focus {
     outline-style: auto;
 }
 
 #nav-tree .arrow {
     opacity: var(--side-nav-arrow-opacity);
+    background: none;
 }
 
 .arrow {
     color: inherit;
     cursor: pointer;
     font-size: 45%;
     vertical-align: middle;
```

### Comparing `coverage_control-1.0.0/doc/config/header.html` & `coverage_control-1.1.0/doc/config/header.html`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/config/navtree-hacks.js` & `coverage_control-1.1.0/doc/config/navtree-hacks.js`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/graphics/LPAC.gif` & `coverage_control-1.1.0/doc/graphics/LPAC.gif`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/graphics/SearchRescue.png` & `coverage_control-1.1.0/doc/graphics/SearchRescue.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/graphics/coveragecontrol_global.png` & `coverage_control-1.1.0/doc/graphics/coveragecontrol_global.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/graphics/learnable_pac.png` & `coverage_control-1.1.0/doc/graphics/learnable_pac.png`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/manual/README.md` & `coverage_control-1.1.0/doc/manual/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,34 @@
 Coverage control is the problem of navigating a robot swarm to collaboratively monitor features or a phenomenon of interest not known _a priori_.
 The relative importance of the features is modeled as an underlying scalar field known as the importance density field (IDF).
 Coverage control with unknown features of interest has applications in various domains, including search and rescue, surveillance, and target tracking.
 
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
 
 **Key features:**  
-- The core library `CoverageControlCore` is written in `C++` and `CUDA` to handle large-scale simulations
+- The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
 - GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
 
+## Quick Start
+The library is available as a `pip` package. To install the package, run the following command:
+```bash
+pip install coverage_control
+```
+
+See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
+
+See [Quick Start](https://kumarrobotics.github.io/CoverageControl/quick_start.html) guide for a quick introduction to the library.
+
+---
+
 ## Citation
 ```
 @article{agarwal2024lpac,
       title         =   {LPAC: Learnable Perception-Action-Communication Loops with
                             Applications to Coverage Control}, 
       author        =   {Saurav Agarwal and Ramya Muthukrishnan and 
                             Walker Gosrich and Vijay Kumar and Alejandro Ribeiro},
```

### Comparing `coverage_control-1.0.0/doc/manual/algorithms.md` & `coverage_control-1.1.0/doc/manual/algorithms.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/manual/coverage-control.md` & `coverage_control-1.1.0/doc/manual/coverage-control.md`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/doc/manual/docker.md` & `coverage_control-1.1.0/doc/manual/docker.md`

 * *Files 2% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 - `--with-cuda` : With CUDA support
 - `--with-ros` : With ROS support
 
 The base image is `ghcr.io/\repo_owner_lower/coveragecontrol` with different tags for different versions and configurations.
 
 |Tags Suffix | Flags|
 |--- | ---|
-|`python2.2.1-cuda12.3.1-ros2humble` | `--with-ros --with-cuda`|
-|`python2.2.1-cuda12.3.1` | `--with-cuda`|
-|`python2.2.1-ros2humble` | `--with-ros`|
-|`python2.2.1` | None|
+|`python2.2.2-cuda12.2.2-ros2humble` | `--with-ros --with-cuda`|
+|`python2.2.2-cuda12.2.2` | `--with-cuda`|
+|`python2.2.2-ros2humble` | `--with-ros`|
+|`python2.2.2` | None|
 
 --------
 
 ## Building and Executing
 
 The library is already built and installed in the container.
 However, if you want to build it again, you can do so using the following commands.
```

### Comparing `coverage_control-1.0.0/doc/manual/installation.md` & `coverage_control-1.1.0/doc/manual/installation.md`

 * *Files 6% similar despite different names*

```diff
@@ -4,19 +4,22 @@
 # PyPI Installation
 The library is available on PyPI and can be installed using `pip`.
 It is recommended to install the library inside a virtual environment.
 ```bash
 pip install coverage_control
 ```
 
-The package depends on the following packages, which are installed as dependencies:
+The package depends on the following packages
 - [PyTorch](https://pytorch.org/)
 - [PyTorch Geometric](https://pytorch-geometric.readthedocs.io/en/latest/)
+```bash
+pip install torch torchvision torch-geometric
+```
 
-\note PyTorch and PyTorch Geometric have CPU and CUDA-specific versions. The package installs the default version (latest CUDA).
+\note PyTorch and PyTorch Geometric have CPU and CUDA-specific versions. The command installs the default version (latest CUDA).
 
 We need the following optional packages for visualization and video generation:
 - `gnuplot` or `gnuplot-nox` (for visualizing environment)
 - `ffmpeg` (for generating videos)
 
 On Ubuntu, these can be installed using the following command:
 ```bash
@@ -47,15 +50,15 @@
 ```
 
 --------
 
 ## Docker Container
 Container can be created using the script in `setup_utils/create_container.sh`.
 ```bash
-cd ${CoverageControl_ws}/src/CoverageControl/setup_utils
+cd ${CoverageControl_ws}/src/CoverageControl/setup_utils/docker
 bash create_container.sh --with-cuda -d ${CoverageControl_ws} # See flags below
 ```
 
 This will land you in a shell inside the container in the directory `/workspace`.
 If the workspace directory was specified, it will be mounted to the container at the same location.
 
 One can exit the container by typing `exit` or pressing `Ctrl+D`.
@@ -72,18 +75,18 @@
 - `--with-cuda` : With CUDA support
 - `--with-ros` : With ROS support
 
 The base image is `ghcr.io/\repo_owner_lower/coveragecontrol` with different tags for different versions and configurations.
 
 |Tags Suffix | Flags|
 |--- | ---|
-|`python2.2.1-cuda12.3.1-ros2humble` | `--with-ros --with-cuda`|
-|`python2.2.1-cuda12.3.1` | `--with-cuda`|
+|`python2.2.2-cuda12.2.2-ros2humble` | `--with-ros --with-cuda`|
+|`python2.2.2-cuda12.2.2` | `--with-cuda`|
 |`python2.2.1-ros2humble` | `--with-ros`|
-|`python2.2.1` | None|
+|`python2.2.2` | None|
 
 The library is already built and installed in the container.
 However, if you want to build it again, you can do so following the [Installation from Source](#installation-from-source) instructions (except for the prerequisites).
 
 --------
 
 # Installation From Source {#installation-from-source}
@@ -127,14 +130,17 @@
 pip install pytest
 pytest
 ```
 
 
 ## Building the Core C++ Library
 
+
+\note This is only necessary if you want to use the C++ library directly.
+
 We will organize files in a **workspace** directory: `${CoverageControl_ws}` (e.g., ~/CoverageControl\_ws).
 
 Add the following lines to your `~/.bashrc` file.
 ```bash
 export CoverageControl_ws=~/CoverageControl_ws # Change to your workspace directory
 export PATH=${CoverageControl_ws}/install/bin:$PATH
 export LD_LIBRARY_PATH=${CoverageControl_ws}/install/lib:$LD_LIBRARY_PATH
```

### Comparing `coverage_control-1.0.0/doc/manual/lpac.md` & `coverage_control-1.1.0/doc/manual/lpac.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \page lpac LPAC Neural Network
 \tableofcontents
 
-# Prelminaries
+# Preliminaries
 We will organize files in a **workspace** directory: `${CoverageControl_ws}` (e.g., ~/CoverageControl\_ws).
 
 Download and extract the file `lpac_CoverageControl.tar.gz` to the workspace directory.
 The file can be downloaded from the repository's release page.
 ```bash
 tar -xvzf lpac_CoverageControl.tar.gz -C ${CoverageControl_ws}
 ```
@@ -66,11 +66,11 @@
 ```bash
 python python/scripts/evaluators/eval.py \
        ${CoverageControl_ws}/lpac/params/eval.toml
 ```
 or
 ```bash
 python python/scripts/evaluators/eval_single_dataset.py \
-       ${CoverageControl_ws}/lpac/params/eval_single.toml
+       ${CoverageControl_ws}/lpac/params/eval_single_env.toml
 ```
 
 The `eval.toml` and `eval_single.toml` files are also provided in the `params` directory of the repository.
```

### Comparing `coverage_control-1.0.0/doc/manual/quick_start.md` & `coverage_control-1.1.0/doc/manual/quick_start.md`

 * *Files 6% similar despite different names*

```diff
@@ -83,14 +83,17 @@
 
 See \ref python/scripts/coverage_env/coverage_simple.py and \ref python/scripts/coverage_env/coverage_class.py for complete examples.
 
 ---
 
 # C++ Interface
 
+\note The C++ interface is not available in the pip package. You need to build the library from source. See the [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html#installation-from-source) guide for instructions.
+
+
 Include the `CoverageControl` library, algorithms, and other necessary headers:
 ```cpp
 #include <CoverageControl/parameters.h>
 #include <CoverageControl/typedefs.h>
 #include <CoverageControl/world_idf.h>
 #include <CoverageControl/coverage_system.h>
```

### Comparing `coverage_control-1.0.0/doc/manual/ref_manual.txt` & `coverage_control-1.1.0/doc/manual/ref_manual.txt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/params/coverage_control_params.toml` & `coverage_control-1.1.0/params/coverage_control_params.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Specify parameters for coverage control in toml format
 
 NumRobots = 32
 NumFeatures = 32
 
+NumPolygons = 0
+MaxVertices = 10
+PolygonRadius = 64
+
 # Parameters for the environment
 [Environment]
 
 [Environment.Maps]
 # Assuming same resolution in both the directions. Pixel area = Resolution^2
 Resolution = 1
```

### Comparing `coverage_control-1.0.0/params/data_params.toml` & `coverage_control-1.1.0/params/data_params.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/params/eval.toml` & `coverage_control-1.1.0/params/eval.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/params/eval_single.toml` & `coverage_control-1.1.0/params/eval_single.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/params/learning_params.toml` & `coverage_control-1.1.0/params/learning_params.toml`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/pyproject.toml` & `coverage_control-1.1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 	"Framework :: Robot Framework",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 	"Environment :: GPU :: NVIDIA CUDA",
 ]
 dynamic = ["version"]
 dependencies = ["numpy", "pyyaml",
   'toml; python_version < "3.11"',
-  "torch", "torchvision", "torch_geometric",
 ]
 
 [project.optional-dependencies]
 nn = ["torch >=2.1", "torchvision >=2.1", "torch_geometric >=2.1"]
 core_test = ["pytest >=6"]
 test = ["pytest >=6", "torch >=2.1", "torchvision"]
 
@@ -58,27 +57,29 @@
 
 [tool.cibuildwheel]
 build = "*"
 skip = ["pp*", "*musllinux*"]
 test-skip = ""
 
 # archs = ["x86_64", "aarch64"]
+# archs = ["aarch64"]
 archs = ["x86_64"]
 build-frontend = "default"
 config-settings = {}
 dependency-versions = "pinned"
 environment-pass = []
 build-verbosity = 1
 
 repair-wheel-command = ""
 
-test-command=""
-before-test=""
-# test-command = "pytest -ra --showlocals --ignore={project}/python/tests/deprecated {project}/python/tests"
-# before-test = "pip install pytest torch torchvision torch_geometric"
+# test-command=""
+# before-test=""
+test-command = "pytest -ra --showlocals --ignore={project}/python/tests/deprecated {project}/python/tests/test_coverage_env_utils.py {project}/python/tests/test_coverage.py {project}/python/tests/test_env_io.py {project}/python/tests/test_map_generation.py {project}/python/tests/test_models.py {project}/python/tests/test_package.py {project}/python/tests/test_parameters.py {project}/python/tests/test_parity.py"
+
+before-test = "pip install pytest torch torchvision torch_geometric && wget https://github.com/KumarRobotics/CoverageControl/releases/download/v1.1.0/pytest_data.tar.gz && tar -xvf pytest_data.tar.gz -C python/tests/ && rm pytest_data.tar.gz"
 test-requires = []
 test-extras = []
 
 container-engine = "docker"
 
 manylinux-x86_64-image = "manylinux_2_28"
 manylinux-aarch64-image = "manylinux_2_28"
```

### Comparing `coverage_control-1.0.0/python/coverage_control/core/__init__.py` & `coverage_control-1.1.0/python/coverage_control/core/__init__.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/io_utils.py` & `coverage_control-1.1.0/python/coverage_control/io_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py` & `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/coverage_env_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/data_loaders/data_loader_utils.py` & `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/data_loader_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/data_loaders/loaders.py` & `coverage_control-1.1.0/python/coverage_control/nn/data_loaders/loaders.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/models/cnn.py` & `coverage_control-1.1.0/python/coverage_control/nn/models/cnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/models/cnn_backbone.py` & `coverage_control-1.1.0/python/coverage_control/nn/models/cnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/models/config_parser.py` & `coverage_control-1.1.0/python/coverage_control/nn/models/config_parser.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/models/gnn_backbone.py` & `coverage_control-1.1.0/python/coverage_control/nn/models/gnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/models/lpac.py` & `coverage_control-1.1.0/python/coverage_control/nn/models/lpac.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/coverage_control/nn/trainers/trainer.py` & `coverage_control-1.1.0/python/coverage_control/nn/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/coverage_env/coverage_class.py` & `coverage_control-1.1.0/python/scripts/coverage_env/coverage_class.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/coverage_env/coverage_simple.py` & `coverage_control-1.1.0/python/scripts/coverage_env/coverage_simple.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/data_generation/data_generation.py` & `coverage_control-1.1.0/python/scripts/data_generation/data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/data_generation/simple_data_generation.py` & `coverage_control-1.1.0/python/scripts/data_generation/simple_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/controller.py` & `coverage_control-1.1.0/python/scripts/evaluators/controller.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_multi.py` & `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_multi.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_rf_exp.py` & `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_rf_exp.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_semantic_video.py` & `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_semantic_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/deprecated/eval_video.py` & `coverage_control-1.1.0/python/scripts/evaluators/deprecated/eval_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/deprecated/semantic_eval.py` & `coverage_control-1.1.0/python/scripts/evaluators/deprecated/semantic_eval.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/eval.py` & `coverage_control-1.1.0/python/scripts/evaluators/eval.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/evaluators/eval_single_env.py` & `coverage_control-1.1.0/python/scripts/evaluators/eval_single_env.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/training/train_cnn.py` & `coverage_control-1.1.0/python/scripts/training/train_cnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/scripts/training/train_lpac.py` & `coverage_control-1.1.0/python/scripts/training/train_lpac.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/cnn_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/cnn_data_generation_NoCommsMap.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_NoCommMaps_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/dense_gnn_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/gnn_NoCNNmaps_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_NoCommsMap_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py` & `coverage_control-1.1.0/python/tests/deprecated/data_generators/sparse_gnn_data_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/gnn.py` & `coverage_control-1.1.0/python/tests/deprecated/gnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/gnn_dist.py` & `coverage_control-1.1.0/python/tests/deprecated/gnn_dist.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/mlp_test.py` & `coverage_control-1.1.0/python/tests/deprecated/mlp_test.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/test_cnn.py` & `coverage_control-1.1.0/python/tests/deprecated/test_cnn.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/test_library_objects.py` & `coverage_control-1.1.0/python/tests/deprecated/test_library_objects.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/test_lpac_coverage.py` & `coverage_control-1.1.0/python/tests/deprecated/test_lpac_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/testplot.py` & `coverage_control-1.1.0/python/tests/deprecated/testplot.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/deprecated/torch_compat.py` & `coverage_control-1.1.0/python/tests/deprecated/torch_compat.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_coverage.py` & `coverage_control-1.1.0/python/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_coverage_env_utils.py` & `coverage_control-1.1.0/python/tests/test_coverage_env_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_env_io.py` & `coverage_control-1.1.0/python/tests/test_env_io.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_map_generation.py` & `coverage_control-1.1.0/python/tests/test_map_generation.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_models.py` & `coverage_control-1.1.0/python/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_package.py` & `coverage_control-1.1.0/python/tests/test_package.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_parameters.py` & `coverage_control-1.1.0/python/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/tests/test_parity.py` & `coverage_control-1.1.0/python/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/ts_jit/TorchVisionResize_32.pt` & `coverage_control-1.1.0/python/ts_jit/TorchVisionResize_32.pt`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/ts_jit/gnn_backbone.py` & `coverage_control-1.1.0/python/ts_jit/gnn_backbone.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/ts_jit/torchvision_resize.py` & `coverage_control-1.1.0/python/ts_jit/torchvision_resize.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/utils/dataset_utils.py` & `coverage_control-1.1.0/python/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/utils/generate_video.py` & `coverage_control-1.1.0/python/utils/generate_video.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/python/utils/save_gnn_params.py` & `coverage_control-1.1.0/python/utils/save_gnn_params.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup.sh` & `coverage_control-1.1.0/setup.sh`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 #!/usr/bin/env bash
-ORIG_INPUT_PARAMS="$@"
-params="$(getopt -o d:hctpg -l directory:,help,clean,torch,python,global,with-cuda,with-deps,pip-path: --name "$(basename "$0")" -- "$@")"
-
-if [ $? -ne 0 ]
-then
-	print_usage
-fi
-
 print_usage() {
-	printf "bash $0 [-h|--help] [-d|--directory <workspace directory>] [-p|--python] [--with-cuda] [--with-deps] [-g|--global] [-c|--clean] [-t|--torch]\n"
+	printf "bash %s [-h|--help] [-d|--directory <workspace directory>] [-p|--python] [--with-cuda] [--with-deps] [-g|--global] [-c|--clean] [-t|--torch]\n" "$0"
 	printf "Options:\n"
 	printf "  -h, --help                             : Prints this help message\n"
 	printf "  -d, --directory <workspace directory>  : Builds and installs the package in the specified directory\n"
 	printf "  -p, --python                           : Installs the python bindings\n"
 	printf "  --with-cuda                            : Builds the package with CUDA support\n"
 	printf "  --with-deps                            : Installs the dependencies\n"
 	printf "  -g, --global                           : Installs the package globally. Needs sudo permissions\n"
 }
 
+ORIG_INPUT_PARAMS="$@"
+
+params="$(getopt -o d:hctpg -l directory:,help,clean,torch,python,global,with-cuda,with-deps,pip-path: --name "$(basename "$0")" -- "$@")"
+
+if [ $? -ne 0 ]
+then
+	print_usage
+fi
+
 eval set -- "$params"
 echo "Params: $params"
 unset params
 
 WITH_TORCH=0
 INSTALL=true
 WITH_DEPS=false
```

### Comparing `coverage_control-1.0.0/setup_utils/check_headers.sh` & `coverage_control-1.1.0/setup_utils/check_headers.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/.bashrc` & `coverage_control-1.1.0/setup_utils/docker/base_images/.bashrc`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/.ros.bashrc` & `coverage_control-1.1.0/setup_utils/docker/base_images/.ros.bashrc`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile` & `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda-ros2.Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Start with cuda image
-FROM nvidia/cuda:12.3.1-devel-ubuntu22.04
+FROM nvidia/cuda:12.2.2-devel-ubuntu22.04
 
 SHELL ["/bin/bash", "-c"]
 
 ENV DEBIAN_FRONTEND noninteractive
 
 # Post actions after apt installs cause errors. This has been fixed in more recent versions of docker
 RUN sed -i -e 's/^APT/# APT/' -e 's/^DPkg/# DPkg/' \
@@ -65,15 +65,15 @@
 # Remove cache to reduce image size
 RUN rm -rf /var/lib/apt/lists/*; \
 		rm -f /var/cache/apt/archives/*.deb; \
 		rm -f /var/cache/apt/archives/parital/*.deb; \
 		rm -f /var/cache/apt/*.bin
 
 RUN mkdir download; \
-		wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcu121.zip -O download/libtorch.zip; \
+		wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcu121.zip -O download/libtorch.zip; \
 		unzip download/libtorch.zip -d /opt/; \
 		rm -r download
 
 ENV LD_LIBRARY_PATH /usr/local/lib:/opt/libtorch/lib:${LD_LIBRARY_PATH}
 ENV Torch_DIR /opt/libtorch/share/cmake/
 
 COPY requirements.txt /opt/requirements.txt
```

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile` & `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-cuda.Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Start with cuda image
-FROM nvidia/cuda:12.3.1-devel-ubuntu22.04
+FROM nvidia/cuda:12.2.2-devel-ubuntu22.04
 
 SHELL ["/bin/bash", "-c"]
 
 ENV DEBIAN_FRONTEND noninteractive
 
 # Post actions after apt installs cause errors. This has been fixed in more recent versions of docker
 RUN sed -i -e 's/^APT/# APT/' -e 's/^DPkg/# DPkg/' \
@@ -55,15 +55,15 @@
 # Remove cache to reduce image size
 RUN rm -rf /var/lib/apt/lists/*; \
 		rm -f /var/cache/apt/archives/*.deb; \
 		rm -f /var/cache/apt/archives/parital/*.deb; \
 		rm -f /var/cache/apt/*.bin
 
 RUN mkdir download; \
-		wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcu121.zip -O download/libtorch.zip; \
+		wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcu121.zip -O download/libtorch.zip; \
 		unzip download/libtorch.zip -d /opt/; \
 		rm -r download
 
 ENV LD_LIBRARY_PATH /usr/local/lib:/opt/libtorch/lib:${LD_LIBRARY_PATH}
 ENV Torch_DIR /opt/libtorch/share/cmake/
 
 COPY requirements.txt /opt/requirements.txt
```

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile` & `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04-ros2.Dockerfile`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 # Remove cache to reduce image size
 RUN rm -rf /var/lib/apt/lists/*; \
 		rm -f /var/cache/apt/archives/*.deb; \
 		rm -f /var/cache/apt/archives/parital/*.deb; \
 		rm -f /var/cache/apt/*.bin
 
 RUN mkdir download; \
-		wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcpu.zip -O download/libtorch.zip; \
+		wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcpu.zip -O download/libtorch.zip; \
 		unzip download/libtorch.zip -d /opt/; \
 		rm -r download
 
 ENV LD_LIBRARY_PATH /usr/local/lib:/opt/libtorch/lib:${LD_LIBRARY_PATH}
 ENV Torch_DIR /opt/libtorch/share/cmake/
 
 COPY requirements_cpu.txt /opt/requirements.txt
```

### Comparing `coverage_control-1.0.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile` & `coverage_control-1.1.0/setup_utils/docker/base_images/ubuntu22.04.Dockerfile`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 # Remove cache to reduce image size
 RUN rm -rf /var/lib/apt/lists/*; \
 		rm -f /var/cache/apt/archives/*.deb; \
 		rm -f /var/cache/apt/archives/parital/*.deb; \
 		rm -f /var/cache/apt/*.bin
 
 RUN mkdir download; \
-		wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcpu.zip -O download/libtorch.zip; \
+		wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcpu.zip -O download/libtorch.zip; \
 		unzip download/libtorch.zip -d /opt/; \
 		rm -r download
 
 ENV LD_LIBRARY_PATH /usr/local/lib:/opt/libtorch/lib:${LD_LIBRARY_PATH}
 ENV Torch_DIR /opt/libtorch/share/cmake/
 
 COPY requirements_cpu.txt /opt/requirements.txt
```

### Comparing `coverage_control-1.0.0/setup_utils/docker/create_container.sh` & `coverage_control-1.1.0/setup_utils/docker/create_container.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup_utils/install_dependencies.sh` & `coverage_control-1.1.0/setup_utils/install_dependencies.sh`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env bash
 
-TMP_DIR=`mktemp -d`
+TMP_DIR=$(mktemp -d)
 
 params="$(getopt -o d: -l directory:,no-cuda,boost,gmp,mpfr,eigen,cgal,pybind11,yaml-cpp,geographiclib,opencv --name "$(basename "$0")" -- "$@")"
 
 print_usage() {
-	printf "bash $0 [-d|--directory <specify install directory>]\n"
+  printf "bash %s [-d|--directory <specify install directory>] [--no-cuda] [--boost] [--gmp] [--mpfr] [--eigen] [--cgal] [--pybind11] [--yaml-cpp] [--geographiclib] [--opencv]\n" "$(basename "$0")"
 }
 eval set -- "$params"
 unset params
 
 while true; do
 	case ${1} in
 		-d|--directory) INSTALL_DIR+=("${2}");shift 2;;
@@ -38,59 +38,75 @@
 	CMAKE_END_FLAGS="-DCMAKE_BUILD_TYPE=Release -DCMAKE_INSTALL_PREFIX=$INSTALL_DIR"
 	CONFIGURE_END_FLAGS="--prefix=$INSTALL_DIR"
 	echo "Installing to $INSTALL_DIR"
 fi
 
 InstallCGAL () {
 	echo "Setting up CGAL"
-	wget https://github.com/CGAL/cgal/releases/download/v${CGAL_VERSION}/CGAL-${CGAL_VERSION}-library.tar.xz -P ${MAIN_DIR}/src > /dev/null
+	wget --tries=4 https://github.com/CGAL/cgal/releases/download/v${CGAL_VERSION}/CGAL-${CGAL_VERSION}-library.tar.xz -P ${MAIN_DIR}/src > /dev/null
+  if [ $? -ne 0 ]; then
+    echo "Failed to download CGAL"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/CGAL-${CGAL_VERSION}-library.tar.xz -C ${MAIN_DIR}/src/ > /dev/null
 	cmake -S ${MAIN_DIR}/src/CGAL-${CGAL_VERSION} -B ${BUILD_DIR}/cgal ${CMAKE_END_FLAGS} > /dev/null
 	cmake --install ${BUILD_DIR}/cgal > /dev/null
 	if [ $? -eq 0 ]; then
 		echo "cgal install succeeded"
 	else
 		echo "cgal install failed"
 		exit 1
 	fi
 }
 
 InstallGeoGraphicLib () {
 	echo "Setting up geographiclib"
-	wget https://github.com/geographiclib/geographiclib/archive/refs/tags/v2.3.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://github.com/geographiclib/geographiclib/archive/refs/tags/v2.3.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download geographiclib"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/v2.3.tar.gz -C ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/geographiclib-2.3 -B ${BUILD_DIR}/geographiclib ${CMAKE_END_FLAGS} -DBUILD_SHARED_LIBS=OFF -DCMAKE_POSITION_INDEPENDENT_CODE=ON
 	cmake --build ${BUILD_DIR}/geographiclib -j$(nproc)
 	cmake --install ${BUILD_DIR}/geographiclib
 	if [ $? -eq 0 ]; then
 		echo "geographiclib install succeeded"
 	else
 		echo "geographiclib install failed"
 		exit 1
 	fi
 }
 
 InstallPybind11 () {
 	echo "Setting up pybind11"
-	wget https://github.com/pybind/pybind11/archive/refs/tags/v2.11.1.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://github.com/pybind/pybind11/archive/refs/tags/v2.11.1.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download pybind11"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/v2.11.1.tar.gz -C ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/pybind11-2.11.1 -B ${BUILD_DIR}/pybind11 -DPYBIND11_TEST=OFF ${CMAKE_END_FLAGS}
 	cmake --build ${BUILD_DIR}/pybind11 -j$(nproc)
 	cmake --install ${BUILD_DIR}/pybind11
 	if [ $? -eq 0 ]; then
 		echo "pybind11 install succeeded"
 	else
 		echo "pybind11 install failed"
 		exit 1
 	fi
 }
 
 InstallYamlCPP () {
 	echo "Setting up yaml-cpp"
-	wget https://github.com/jbeder/yaml-cpp/archive/refs/tags/0.8.0.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://github.com/jbeder/yaml-cpp/archive/refs/tags/0.8.0.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download yaml-cpp"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/0.8.0.tar.gz -C ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/yaml-cpp-0.8.0 -B ${BUILD_DIR}/yaml-cpp -DYAML_BUILD_SHARED_LIBS=ON  ${CMAKE_END_FLAGS} -DCMAKE_POSITION_INDEPENDENT_CODE=ON
 	cmake --build ${BUILD_DIR}/yaml-cpp -j$(nproc)
 	if [ $? -ne 0 ]; then
 		echo "YAML build failed"
 	fi
 	cmake --install ${BUILD_DIR}/yaml-cpp
@@ -100,30 +116,38 @@
 		echo "yaml-cpp install failed"
 		exit 1
 	fi
 }
 
 InstallEigen3 () {
 	echo "Setting up eigen3"
-	wget https://gitlab.com/libeigen/eigen/-/archive/${EIGEN_VERSION}/${EIGEN_TAR_NAME}.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://gitlab.com/libeigen/eigen/-/archive/${EIGEN_VERSION}/${EIGEN_TAR_NAME}.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download eigen3"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/${EIGEN_TAR_NAME}.tar.gz -C ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/${EIGEN_TAR_NAME} -B ${BUILD_DIR}/eigen3 ${CMAKE_END_FLAGS} > /dev/null
 	cmake --build ${BUILD_DIR}/eigen3 -j$(nproc) > /dev/null
 	cmake --install ${BUILD_DIR}/eigen3 > /dev/null
 	if [ $? -eq 0 ]; then
 		echo "eigen3 install succeeded"
 	else
 		echo "eigen3 install failed"
 		exit 1
 	fi
 }
 
 InstallTorchVision () {
 	echo "Setting up torchvision"
-	wget https://github.com/pytorch/vision/archive/refs/tags/v0.15.2.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://github.com/pytorch/vision/archive/refs/tags/v0.15.2.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download torchvision"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/v0.15.2.tar.gz -C ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/vision-0.15.2 -B ${BUILD_DIR}/torchvision -DWITH_CUDA=ON -DUSE_PYTHON=ON -DCMAKE_INSTALL_PREFIX=${Torch_ROOT} ${CMAKE_END_FLAGS}
 	cmake --build ${BUILD_DIR}/torchvision -j$(nproc)
 	cmake --install ${BUILD_DIR}/torchvision
 	if [ $? -eq 0 ]; then
 		echo "torchvision install succeeded"
 	else
@@ -158,15 +182,19 @@
 		echo "torchsparse install failed"
 		exit 1
 	fi
 }
 
 InstallOpenCV () {
 	echo "Setting up opencv"
-	wget -O ${MAIN_DIR}/src/opencv.tar.gz https://github.com/opencv/opencv/archive/refs/tags/4.8.0.tar.gz
+	wget --tries=4 -O ${MAIN_DIR}/src/opencv.tar.gz https://github.com/opencv/opencv/archive/refs/tags/4.8.0.tar.gz
+  if [ $? -ne 0 ]; then
+    echo "Failed to download opencv"
+    exit 1
+  fi
 	wget -O ${MAIN_DIR}/src/opencv_contrib.zip https://github.com/opencv/opencv_contrib/archive/4.8.0.zip
 	tar -xf ${MAIN_DIR}/src/opencv.tar.gz -C ${MAIN_DIR}/src/
 	unzip ${MAIN_DIR}/src/opencv_contrib.zip -d ${MAIN_DIR}/src/
 	cmake -S ${MAIN_DIR}/src/opencv-4.8.0 -B ${BUILD_DIR}/opencv -DWITH_CUDA=ON -DWITH_CUBLAS=ON -DWITH_CUDNN=ON -DWITH_FFMPEG=ON -DWITH_EIGEN=ON -DWITH_OPENMP=ON -DWITH_JPEG=ON -DWITH_PNG=ON -DWITH_TIFF=ON -DWITH_OPENJPEG=ON -DOPENCV_EXTRA_MODULES_PATH=${MAIN_DIR}/src/opencv_contrib-4.8.0/modules ${CMAKE_END_FLAGS}
 	cmake --build ${BUILD_DIR}/opencv -j$(nproc)
 	cmake --install ${BUILD_DIR}/opencv
 	if [ $? -eq 0 ]; then
@@ -175,30 +203,44 @@
 		echo "opencv install failed"
 		exit 1
 	fi
 }
 
 InstallGMP () {
 	echo "Setting up gmp"
-	wget https://gmplib.org/download/gmp/${GMP_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src > /dev/null
+	wget --tries=1 https://gmplib.org/download/gmp/${GMP_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src > /dev/null
+  if [ $? -ne 0 ]; then
+    wget --tries=4 https://github.com/AgarwalSaurav/gmp-mpfr/releases/download/${GMP_TAR_NAME}/${GMP_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src > /dev/null
+  fi
+  if [ $? -ne 0 ]; then
+    echo "Failed to download gmp"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/${GMP_TAR_NAME}.tar.xz -C ${MAIN_DIR}/src/ > /dev/null
 	cd ${MAIN_DIR}/src/${GMP_TAR_NAME}
 	./configure --enable-cxx --disable-shared --with-pic ${CONFIGURE_END_FLAGS}  > /dev/null
 	make -C ${MAIN_DIR}/src/${GMP_TAR_NAME} install -j$(nproc) > /dev/null
 	if [ $? -eq 0 ]; then
 		echo "gmp install succeeded"
 	else
 		echo "gmp install failed"
 		exit 1
 	fi
 }
 
 InstallMPFR() {
 	echo "Setting up mpfr"
-	wget https://www.mpfr.org/mpfr-current/${MPFR_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src
+	wget --tries=1 https://www.mpfr.org/mpfr-current/${MPFR_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src > /dev/null
+  if [ $? -ne 0 ]; then
+    wget --tries=4 https://github.com/AgarwalSaurav/gmp-mpfr/releases/download/${MPFR_TAR_NAME}/${MPFR_TAR_NAME}.tar.xz -P ${MAIN_DIR}/src > /dev/null
+  fi
+  if [ $? -ne 0 ]; then
+    echo "Failed to download mpfr"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/${MPFR_TAR_NAME}.tar.xz -C ${MAIN_DIR}/src/
 	cd ${MAIN_DIR}/src/${MPFR_TAR_NAME}
 	# if ${INSTALL_DIR} is set, then we need to tell where gmp is installed
 	if [ -z "$INSTALL_DIR" ]; then
 		./configure --disable-shared --with-pic ${CONFIGURE_END_FLAGS}
 	else
 		./configure --disable-shared --with-pic --with-gmp=${INSTALL_DIR} ${CONFIGURE_END_FLAGS}
@@ -210,15 +252,19 @@
 		echo "mpfr install failed"
 		exit 1
 	fi
 }
 
 InstallBoost () {
 	echo "Setting up boost"
-	wget https://boostorg.jfrog.io/artifactory/main/release/${BOOST_VERSION}/source/${BOOST_TAR_NAME}.tar.gz -P ${MAIN_DIR}/src
+	wget --tries=4 https://boostorg.jfrog.io/artifactory/main/release/${BOOST_VERSION}/source/${BOOST_TAR_NAME}.tar.gz -P ${MAIN_DIR}/src
+  if [ $? -ne 0 ]; then
+    echo "Failed to download boost"
+    exit 1
+  fi
 	tar -xf ${MAIN_DIR}/src/${BOOST_TAR_NAME}.tar.gz -C ${MAIN_DIR}/src/
 	cd ${MAIN_DIR}/src/${BOOST_TAR_NAME}
 	if [ -z "$INSTALL_DIR" ]; then
 		./bootstrap.sh
 	else
 		./bootstrap.sh --prefix=${INSTALL_DIR}
 	fi
@@ -227,24 +273,24 @@
 		echo "boost install succeeded"
 	else
 		echo "boost install failed"
 		exit 1
 	fi
 }
 
-BOOST_VERSION=1.82.0
-BOOST_TAR_NAME=`echo boost_${BOOST_VERSION} | tr . _`
+BOOST_VERSION=1.85.0
+BOOST_TAR_NAME=$(echo boost_${BOOST_VERSION} | tr . _)
 GMP_VERSION=6.3.0
-GMP_TAR_NAME=`echo gmp-${GMP_VERSION}`
+GMP_TAR_NAME=$(echo gmp-${GMP_VERSION})
 MPFR_VERSION=4.2.1
-MPFR_TAR_NAME=`echo mpfr-${MPFR_VERSION}`
+MPFR_TAR_NAME=$(echo mpfr-${MPFR_VERSION})
 EIGEN_VERSION=3.4.0
-EIGEN_TAR_NAME=`echo eigen-${EIGEN_VERSION}`
+EIGEN_TAR_NAME=$(echo eigen-${EIGEN_VERSION})
 CGAL_VERSION=5.6.1
-CGAL_TAR_NAME=`echo CGAL-${CGAL_VERSION}`
+CGAL_TAR_NAME=$(echo CGAL-${CGAL_VERSION})
 
 if [ -n "$BOOST" ]; then
 	InstallBoost
 fi
 
 if [ -n "$GMP" ]; then
 	InstallGMP
```

### Comparing `coverage_control-1.0.0/setup_utils/install_libtorch.sh` & `coverage_control-1.1.0/setup_utils/install_libtorch.sh`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 			exit 1 ;;
 	esac
 done
 
 mkdir -p ${INSTALL_DIR}
 if [[ ${NOCUDA} ]]
 then
-	wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcpu.zip -O ${TMP_DIR}/libtorch.zip
+	wget https://download.pytorch.org/libtorch/cpu/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcpu.zip -O ${TMP_DIR}/libtorch.zip
 
 else
-	wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.1%2Bcu121.zip -O ${TMP_DIR}/libtorch.zip
+	wget https://download.pytorch.org/libtorch/cu121/libtorch-cxx11-abi-shared-with-deps-2.2.2%2Bcu121.zip -O ${TMP_DIR}/libtorch.zip
 fi
 unzip ${TMP_DIR}/libtorch.zip -d ${INSTALL_DIR}/
 # cp -r ${TMP_DIR}/libtorch/* ${1}/.
 rm -r ${TMP_DIR}
```

### Comparing `coverage_control-1.0.0/setup_utils/manylinux_2_28_before-all.sh` & `coverage_control-1.1.0/setup_utils/manylinux_2_28_before-all.sh`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/setup_utils/noxfile.py` & `coverage_control-1.1.0/setup_utils/noxfile.py`

 * *Files identical despite different names*

### Comparing `coverage_control-1.0.0/PKG-INFO` & `coverage_control-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coverage_control
-Version: 1.0.0
+Version: 1.1.0
 Summary: Library for large-scale coverage control using robot swarms
 Author-Email: Saurav Agarwal <agr.saurav1@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -691,45 +691,53 @@
 Project-URL: Bug tracker, https://github.com/KumarRobotics/CoverageControl/issues
 Project-URL: Discussions, https://github.com/KumarRobotics/CoverageControl/discussions
 Project-URL: Changelog, https://github.com/KumarRobotics/CoverageControl/releases
 Requires-Python: >=3.10
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Requires-Dist: toml; python_version < "3.11"
-Requires-Dist: torch
-Requires-Dist: torchvision
-Requires-Dist: torch_geometric
 Requires-Dist: torch>=2.1; extra == "nn"
 Requires-Dist: torchvision>=2.1; extra == "nn"
 Requires-Dist: torch_geometric>=2.1; extra == "nn"
 Requires-Dist: pytest>=6; extra == "core-test"
 Requires-Dist: pytest>=6; extra == "test"
 Requires-Dist: torch>=2.1; extra == "test"
 Requires-Dist: torchvision; extra == "test"
 Provides-Extra: nn
-Provides-Extra: core_test
+Provides-Extra: core-test
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 See full documentation at [https://KumarRobotics.github.io/CoverageControl/](https://KumarRobotics.github.io/CoverageControl/)
 
 ## Introduction
 
 Coverage control is the problem of navigating a robot swarm to collaboratively monitor features or a phenomenon of interest not known _a priori_.
 The library provides a simulation environment, algorithms, and GNN-based architectures for the coverage control problem.  
-<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/blob/main/doc/graphics/LPAC.gif">
+<img align="right" width="300" src="https://github.com/KumarRobotics/CoverageControl/raw/main/doc/graphics/LPAC.gif">
 
 **Key features:**  
-- The core library `CoverageControlCore` is written in `C++` and `CUDA` to handle large-scale simulations
+- The core library is written in `C++` and `CUDA` to handle large-scale simulations
 - There are `python` bindings that interface with the core library
 - Several Centroidal Voronoi Tessellation (CVT)-based algorithms (aka Lloyd's algorithms)
 - Learnable Perception-Action-Communication (LPAC) architecture for the coverage control problem is implemented in `PyTorch` and `PyTorch Geometric`
 - GPU and CPU parallelization using `CUDA` and `OpenMP`
 
 ---
+## Quick Start
+The library is available as a `pip` package. To install the package, run the following command:
+```bash
+pip install coverage_control
+```
+
+See [Installation](https://kumarrobotics.github.io/CoverageControl/installation.html) for more details on installation.
+
+See [Quick Start](https://kumarrobotics.github.io/CoverageControl/quick_start.html) guide for a quick introduction to the library.
+
+---
 
 ## Citation
 ```
 @article{agarwal2024lpac,
       title         =   {LPAC: Learnable Perception-Action-Communication Loops with
                             Applications to Coverage Control}, 
       author        =   {Saurav Agarwal and Ramya Muthukrishnan and
```

