# Comparing `tmp/sleplet-1.4.6.tar.gz` & `tmp/sleplet-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sleplet-1.4.6.tar", last modified: Tue Nov 28 09:56:05 2023, max compression
+gzip compressed data, was "sleplet-1.4.7.tar", last modified: Tue Apr 23 13:49:48 2024, max compression
```

## Comparing `sleplet-1.4.6.tar` & `sleplet-1.4.7.tar`

### file list

```diff
@@ -1,120 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.408810 sleplet-1.4.6/
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-11-28 09:55:53.000000 sleplet-1.4.6/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2023-11-28 09:55:53.000000 sleplet-1.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7270 2023-11-28 09:55:53.000000 sleplet-1.4.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-11-28 09:55:53.000000 sleplet-1.4.6/LICENCE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2023-11-28 09:56:05.408810 sleplet-1.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5776 2023-11-28 09:55:53.000000 sleplet-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2023-11-28 09:55:53.000000 sleplet-1.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-28 09:56:05.408810 sleplet-1.4.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.388810 sleplet-1.4.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.392810 sleplet-1.4.6/src/sleplet/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_array_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_bool_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4689 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_class_lists.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_convolution_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.396810 sleplet-1.4.6/src/sleplet/_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1163 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/create_earth_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/create_wmap_flm.py
--rw-r--r--   0 runner    (1001) docker     (127)    39339 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_bird.off
--rw-r--r--   0 runner    (1001) docker     (127)   111621 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_cheetah.off
--rw-r--r--   0 runner    (1001) docker     (127)   321932 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_cube.off
--rw-r--r--   0 runner    (1001) docker     (127)    65194 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_dragon.off
--rw-r--r--   0 runner    (1001) docker     (127)   329591 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_homer.off
--rw-r--r--   0 runner    (1001) docker     (127)    36961 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_polygons_teapot.off
--rw-r--r--   0 runner    (1001) docker     (127)      287 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_bird.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_cheetah.toml
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_cube.toml
--rw-r--r--   0 runner    (1001) docker     (127)      290 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_dragon.toml
--rw-r--r--   0 runner    (1001) docker     (127)      283 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_homer.toml
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/meshes_regions_teapot.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_data/setup_pooch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_integration_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_mask_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_mesh_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_parallel_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_plotly_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.396810 sleplet-1.4.6/src/sleplet/_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_scripts/plotting_on_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    11052 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_scripts/plotting_on_sphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_slepian_arbitrary_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_string_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.404810 sleplet-1.4.6/src/sleplet/functions/
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7153 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/elongated_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/flm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/fp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/harmonic_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/noise_earth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/ridgelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2462 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_dirac_delta.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_identity.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_noise_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_noise_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     4156 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/south_america.py
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/spherical_harmonic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/squashed_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/functions/wmap.py
--rw-r--r--   0 runner    (1001) docker     (127)     5637 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/harmonic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.404810 sleplet-1.4.6/src/sleplet/meshes/
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/_mesh_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3181 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2647 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_basis_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3318 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_harmonic_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian.py
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_noise_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_wavelets.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     7709 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/plot_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.404810 sleplet-1.4.6/src/sleplet/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/plotting/_create_plot_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7013 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/plotting/_create_plot_sphere.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.408810 sleplet-1.4.6/src/sleplet/slepian/
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/_slepian_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (127)     5743 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/region.py
--rw-r--r--   0 runner    (1001) docker     (127)     7665 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/slepian_arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/slepian_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/slepian_limit_lat_lon.py
--rw-r--r--   0 runner    (1001) docker     (127)    14565 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian/slepian_polar_cap.py
--rw-r--r--   0 runner    (1001) docker     (127)     6989 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/slepian_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2023-11-28 09:55:53.000000 sleplet-1.4.6/src/sleplet/wavelet_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 09:56:05.408810 sleplet-1.4.6/src/sleplet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9713 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4065 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      331 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-28 09:56:05.000000 sleplet-1.4.6/src/sleplet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.612817 sleplet-1.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-23 13:49:43.000000 sleplet-1.4.7/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-04-23 13:49:43.000000 sleplet-1.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7270 2024-04-23 13:49:43.000000 sleplet-1.4.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-04-23 13:49:43.000000 sleplet-1.4.7/LICENCE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-23 13:49:48.612817 sleplet-1.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5881 2024-04-23 13:49:43.000000 sleplet-1.4.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-23 13:49:43.000000 sleplet-1.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 13:49:48.612817 sleplet-1.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.588817 sleplet-1.4.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.596817 sleplet-1.4.7/src/sleplet/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_array_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_bool_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4689 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_class_lists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_convolution_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.600817 sleplet-1.4.7/src/sleplet/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/create_earth_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1441 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/create_wmap_flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39339 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_bird.off
+-rw-r--r--   0 runner    (1001) docker     (127)   111621 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cheetah.off
+-rw-r--r--   0 runner    (1001) docker     (127)   321932 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cube.off
+-rw-r--r--   0 runner    (1001) docker     (127)    65194 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_dragon.off
+-rw-r--r--   0 runner    (1001) docker     (127)   329591 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_homer.off
+-rw-r--r--   0 runner    (1001) docker     (127)    36961 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_polygons_teapot.off
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_bird.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_cheetah.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_cube.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_dragon.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_homer.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/meshes_regions_teapot.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_data/setup_pooch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_integration_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_mask_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4959 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_mesh_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1873 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_parallel_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_plotly_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.600817 sleplet-1.4.7/src/sleplet/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/plotting_on_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11063 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_scripts/plotting_on_sphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_slepian_arbitrary_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_string_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.604817 sleplet-1.4.7/src/sleplet/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/elongated_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/flm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3253 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/fp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/harmonic_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/noise_earth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/ridgelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_dirac_delta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_noise_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_noise_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_africa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/south_america.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/spherical_harmonic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/squashed_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/functions/wmap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5675 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/harmonic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/meshes/
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/_mesh_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_basis_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_harmonic_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6112 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_noise_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10852 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7736 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plot_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/_create_plot_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7025 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/plotting/_create_plot_sphere.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.608817 sleplet-1.4.7/src/sleplet/slepian/
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/_slepian_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7681 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8587 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_limit_lat_lon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian/slepian_polar_cap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7023 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/slepian_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-04-23 13:49:43.000000 sleplet-1.4.7/src/sleplet/wavelet_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 13:49:48.612817 sleplet-1.4.7/src/sleplet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4065 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-23 13:49:48.000000 sleplet-1.4.7/src/sleplet.egg-info/top_level.txt
```

### Comparing `sleplet-1.4.6/CITATION.cff` & `sleplet-1.4.7/CITATION.cff`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,27 @@
-cff-version: "1.2.0"
+cff-version: 1.2.0
 authors:
   - family-names: Roddy
     given-names: Patrick J.
-    orcid: "https://orcid.org/0000-0002-6271-1700"
+    orcid: https://orcid.org/0000-0002-6271-1700
 doi: 10.5281/zenodo.7268074
-message: If you use this software, please cite our article in the
+message: >-
+  If you use this software, please cite our article in the
   Journal of Open Source Software.
 preferred-citation:
   authors:
     - family-names: Roddy
       given-names: Patrick J.
-      orcid: "https://orcid.org/0000-0002-6271-1700"
+      orcid: https://orcid.org/0000-0002-6271-1700
   date-published: 2023-04-20
   doi: 10.21105/joss.05221
   issn: 2475-9066
   issue: 84
   journal: Journal of Open Source Software
   publisher:
     name: Open Journals
   start: 5221
   title: "SLEPLET: Slepian Scale-Discretised Wavelets in Python"
   type: article
-  url: "https://joss.theoj.org/papers/10.21105/joss.05221"
+  url: https://joss.theoj.org/papers/10.21105/joss.05221
   volume: 8
 title: "SLEPLET: Slepian Scale-Discretised Wavelets in Python"
```

### Comparing `sleplet-1.4.6/CODE_OF_CONDUCT.md` & `sleplet-1.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/CONTRIBUTING.md` & `sleplet-1.4.7/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/LICENCE.txt` & `sleplet-1.4.7/LICENCE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause Licence
 
-Copyright (c) 2017-2023, Patrick Roddy
+Copyright (c) 2017-2024, Patrick Roddy
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `sleplet-1.4.6/PKG-INFO` & `sleplet-1.4.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.6
+Version: 1.4.7
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
-        Copyright (c) 2017-2023, Patrick Roddy
+        Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -74,14 +74,15 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-uv; extra == "dev"
 Requires-Dist: tuna; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
@@ -89,18 +90,19 @@
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
-[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
+[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
```

### Comparing `sleplet-1.4.6/README.md` & `sleplet-1.4.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
-[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
+[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
```

### Comparing `sleplet-1.4.6/pyproject.toml` & `sleplet-1.4.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 optional-dependencies = {dev = [
     "build",
     "mypy",
     "pre-commit",
     "pytest",
     "ruff",
     "tox",
+    "tox-uv",
     "tuna",
     "twine",
 ], docs = [
     "pdoc3",
 ], readme = [
     "pytest-codeblocks",
 ]}
@@ -128,67 +129,68 @@
 testpaths = [
     "tests",
 ]
 
 [tool.ruff]
 fix = true
 force-exclude = true
-ignore = [
+lint.ignore = [
     "COM812",
     "D105",
     "D203",
     "D205",
     "D212",
     "D407",
+    "D413",
     "ISC001",
     "N803",
     "N806",
 ]
-isort = {known-first-party = [
+lint.isort = {known-first-party = [
     "sleplet",
 ], section-order = [
     "future",
     "standard-library",
     "third-party",
     "astro-info",
     "first-party",
     "local-folder",
 ], sections = {"astro-info" = [
     "pys2let",
     "pyssht",
 ]}}
-per-file-ignores = {"examples*" = [
+lint.per-file-ignores = {"examples*" = [
     "D100",
     "INP001",
     "T201",
 ], "src*" = [
     "SLF001",
 ], "tests*" = [
     "D100",
     "INP001",
     "S101",
     "SLF001",
 ]}
-select = [
+lint.select = [
     "ALL",
 ]
-mccabe.max-complexity = 18
-pep8-naming.classmethod-decorators = [
+lint.mccabe.max-complexity = 18
+lint.pep8-naming.classmethod-decorators = [
     "classmethod",
     "pydantic.field_validator",
 ]
 
 [tool.setuptools_scm]
 local_scheme = "no-local-version"
 write_to = "src/sleplet/_version.py"
 
 [tool.tomlsort]
 overrides."project.classifiers".inline_arrays = false
 overrides."tool.coverage.paths.source".inline_arrays = false
-overrides."tool.ruff.isort.section-order".inline_arrays = false
+overrides."tool.ruff.lint.isort.section-order".inline_arrays = false
 
 [tool.tox]
 legacy_tox_ini = """
     [gh-actions]
     python =
         3.10: py310
         3.11: py311
```

### Comparing `sleplet-1.4.6/src/sleplet/__init__.py` & `sleplet-1.4.7/src/sleplet/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_bool_methods.py` & `sleplet-1.4.7/src/sleplet/_bool_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_class_lists.py` & `sleplet-1.4.7/src/sleplet/_class_lists.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_convolution_methods.py` & `sleplet-1.4.7/src/sleplet/_convolution_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 import numpy.typing as npt
 
 
 def sifting_convolution(
-    f_coefficient: npt.NDArray[np.complex_ | np.float_],
-    g_coefficient: npt.NDArray[np.complex_ | np.float_],
+    f_coefficient: npt.NDArray[np.complex128 | np.float64],
+    g_coefficient: npt.NDArray[np.complex128 | np.float64],
     *,
     shannon: int | None = None,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """Compute the sifting convolution between two multipoles."""
     n = shannon if shannon is not None else np.newaxis
     # change shape if the sizes don't match
     g_reshape = (
         g_coefficient[np.newaxis]
         if len(g_coefficient.shape) < len(f_coefficient.shape)
         else g_coefficient
```

### Comparing `sleplet-1.4.6/src/sleplet/_data/create_earth_flm.py` & `sleplet-1.4.7/src/sleplet/_data/create_earth_flm.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import pyssht as ssht
 
 import sleplet._data.setup_pooch
 import sleplet._smoothing
 
 
-def create_flm(L: int, *, smoothing: int | None = None) -> npt.NDArray[np.complex_]:
+def create_flm(L: int, *, smoothing: int | None = None) -> npt.NDArray[np.complex128]:
     """Create the flm for the whole Earth."""
     # load in data
     flm = _load_flm()
 
     # fill in negative m components so as to avoid confusion with zero values
     for ell in range(1, L):
         for m in range(1, ell + 1):
@@ -25,15 +25,15 @@
     flm = flm[: L**2].conj()
 
     if isinstance(smoothing, int):
         flm = sleplet._smoothing.apply_gaussian_smoothing(flm, L, smoothing)
     return flm
 
 
-def _load_flm() -> npt.NDArray[np.complex_]:
+def _load_flm() -> npt.NDArray[np.complex128]:
     """Load coefficients from file."""
     mat_contents = sio.loadmat(
         sleplet._data.setup_pooch.find_on_pooch_then_local(
             "EGM2008_Topography_flms_L2190.mat",
         ),
     )
     return np.ascontiguousarray(mat_contents["flm"][:, 0])
```

### Comparing `sleplet-1.4.6/src/sleplet/_data/create_wmap_flm.py` & `sleplet-1.4.7/src/sleplet/_data/create_wmap_flm.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 import pyssht as ssht
 
 import sleplet._data.setup_pooch
 import sleplet._vars
 
 
-def create_flm(L: int) -> npt.NDArray[np.complex_]:
+def create_flm(L: int) -> npt.NDArray[np.complex128]:
     """Create the flm for the whole CMB."""
     # load in data
     cl = _load_cl()
 
     # same random seed
     rng = np.random.default_rng(sleplet._vars.RANDOM_SEED)
 
     # Simulate CMB in harmonic space.
-    flm = np.zeros(L**2, dtype=np.complex_)
+    flm = np.zeros(L**2, dtype=np.complex128)
     for ell in range(2, L):
         sigma = np.sqrt(2 * np.pi / (ell * (ell + 1)) * cl[ell - 2])
         ind = ssht.elm2ind(ell, 0)
         flm[ind] = sigma * rng.standard_normal()
         for m in range(1, ell + 1):
             ind_pm = ssht.elm2ind(ell, m)
             ind_nm = ssht.elm2ind(ell, -m)
@@ -33,15 +33,15 @@
             flm[ind_nm] = (-1) ** m * flm[ind_pm].conj()
     return flm
 
 
 def _load_cl(
     *,
     file_ending: str = "_lcdm_pl_model_wmap7baoh0",
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """
     Pick coefficients from file options are:
     * _lcdm_pl_model_yr1_v1.mat
     * _tt_spectrum_7yr_v4p1.mat
     * _lcdm_pl_model_wmap7baoh0.mat.
     """
     mat_contents = sio.loadmat(
```

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_bird.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_bird.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_cheetah.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cheetah.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_cube.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_cube.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_dragon.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_dragon.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_homer.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_homer.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/meshes_polygons_teapot.off` & `sleplet-1.4.7/src/sleplet/_data/meshes_polygons_teapot.off`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_data/setup_pooch.py` & `sleplet-1.4.7/src/sleplet/_data/setup_pooch.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 _POOCH = None
 _ZENODO_DATA_DOI = "10.5281/zenodo.7767698"
 
 
 def _lazy_load_registry(
-    func: typing.Callable[..., os.PathLike[str] | None]
+    func: typing.Callable[..., os.PathLike[str] | None],
 ) -> typing.Callable[..., os.PathLike[str] | None]:
     """
     Lazily loads POOCH registry before executing a function.
 
     Args:
         func: Function to be decorated
```

### Comparing `sleplet-1.4.6/src/sleplet/_integration_methods.py` & `sleplet-1.4.7/src/sleplet/_integration_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,60 +5,60 @@
 import numpy.typing as npt
 
 import pyssht as ssht
 
 import sleplet._vars
 
 
-def calc_integration_weight(L: int) -> npt.NDArray[np.float_]:
+def calc_integration_weight(L: int) -> npt.NDArray[np.float64]:
     """Compute the spherical Jacobian for the integration."""
     thetas, phis = ssht.sample_positions(
         L,
         Grid=True,
         Method=sleplet._vars.SAMPLING_SCHEME,
     )
     delta_theta = np.ediff1d(thetas[:, 0]).mean()
     delta_phi = np.ediff1d(phis[0]).mean()
     return np.sin(thetas) * delta_theta * delta_phi
 
 
 def integrate_whole_sphere(
-    weight: npt.NDArray[np.float_],
-    *functions: npt.NDArray[np.complex_],
+    weight: npt.NDArray[np.float64],
+    *functions: npt.NDArray[np.complex128],
 ) -> complex:
     """Compute the integration for the whole sphere."""
     multiplied_inputs = _multiply_args(*functions)
     return (multiplied_inputs * weight).sum()
 
 
 def integrate_region_sphere(
-    mask: npt.NDArray[np.float_],
-    weight: npt.NDArray[np.float_],
-    *functions: npt.NDArray[np.complex_ | np.float_],
+    mask: npt.NDArray[np.float64],
+    weight: npt.NDArray[np.float64],
+    *functions: npt.NDArray[np.complex128 | np.float64],
 ) -> complex:
     """Compute the integration for a region of the sphere."""
     multiplied_inputs = _multiply_args(*functions)
     return (multiplied_inputs * weight * mask).sum()
 
 
 def integrate_whole_mesh(
-    vertices: npt.NDArray[np.float_],  # noqa: ARG001
+    vertices: npt.NDArray[np.float64],  # noqa: ARG001
     faces: npt.NDArray[np.int_],  # noqa: ARG001
-    *functions: npt.NDArray[np.complex_ | np.float_],
+    *functions: npt.NDArray[np.complex128 | np.float64],
 ) -> float:
     """Compute the integral of functions on the vertices."""
     multiplied_inputs = _multiply_args(*functions)
     return multiplied_inputs.sum()
 
 
 def integrate_region_mesh(
     mask: npt.NDArray[np.bool_],
-    vertices: npt.NDArray[np.float_],  # noqa: ARG001
+    vertices: npt.NDArray[np.float64],  # noqa: ARG001
     faces: npt.NDArray[np.int_],  # noqa: ARG001
-    *functions: npt.NDArray[np.complex_ | np.float_],
+    *functions: npt.NDArray[np.complex128 | np.float64],
 ) -> float:
     """Compute the integral of a region of functions on the vertices."""
     multiplied_inputs = _multiply_args(*functions)
     return (multiplied_inputs * mask).sum()
 
 
 def _multiply_args(*args: npt.NDArray[typing.Any]) -> npt.NDArray[typing.Any]:
```

### Comparing `sleplet-1.4.6/src/sleplet/_mask_methods.py` & `sleplet-1.4.7/src/sleplet/_mask_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 _AFRICA_RANGE = np.deg2rad(41)
 _SOUTH_AMERICA_RANGE = np.deg2rad(40)
 
 
 def create_mask_region(
     L: int,
     region: "sleplet.slepian.region.Region",
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """
     Create a mask of a region of interested, the output will be based
     on the value of the provided L. The mask could be either:
     * polar cap - if theta_max provided
     * limited latitude longitude - if one of theta_min, theta_max,
                                    phi_min or phi_max is provided
     * arbitrary - just checks the shape of the input mask.
@@ -63,30 +63,30 @@
             mask = thetas <= region.theta_max
             if region.gap:
                 _logger.info("creating polar gap mask")
                 mask += thetas >= np.pi - region.theta_max
     return mask
 
 
-def _load_mask(L: int, mask_name: str) -> npt.NDArray[np.float_]:
+def _load_mask(L: int, mask_name: str) -> npt.NDArray[np.float64]:
     """Attempt to read the mask from the config file."""
     mask = sleplet._data.setup_pooch.find_on_pooch_then_local(
         f"slepian_masks_{mask_name}",
     )
     return create_mask(L, mask_name) if mask is None else np.load(mask)
 
 
 def ensure_masked_flm_bandlimited(
-    flm: npt.NDArray[np.complex_],
+    flm: npt.NDArray[np.complex128],
     L: int,
     region: "sleplet.slepian.region.Region",
     *,
     reality: bool,
     spin: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Ensure the coefficients is bandlimited for a given region."""
     field = ssht.inverse(
         flm,
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
         Reality=reality,
         Spin=spin,
@@ -112,52 +112,52 @@
         theta_max=np.deg2rad(int(os.getenv("THETA_MAX", "180"))),
         theta_min=np.deg2rad(int(os.getenv("THETA_MIN", "0"))),
     )
 
 
 def create_mesh_region(
     mesh_config: dict[str, typing.Any],
-    vertices: npt.NDArray[np.float_],
+    vertices: npt.NDArray[np.float64],
 ) -> npt.NDArray[np.bool_]:
     """Create a boolean region for the given mesh."""
     return (
         (vertices[:, 0] >= mesh_config["XMIN"])
         & (vertices[:, 0] <= mesh_config["XMAX"])
         & (vertices[:, 1] >= mesh_config["YMIN"])
         & (vertices[:, 1] <= mesh_config["YMAX"])
         & (vertices[:, 2] >= mesh_config["ZMIN"])
         & (vertices[:, 2] <= mesh_config["ZMAX"])
     )
 
 
 def ensure_masked_bandlimit_mesh_signal(
     mesh: "sleplet.meshes.mesh.Mesh",
-    u_i: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.float_]:
+    u_i: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.float64]:
     """Ensure that signal in pixel space is bandlimited."""
     field = sleplet.harmonic_methods.mesh_inverse(mesh, u_i)
     masked_field = np.where(mesh.mesh_region, field, 0)
     return sleplet.harmonic_methods.mesh_forward(mesh, masked_field)
 
 
 def convert_region_on_vertices_to_faces(
     mesh: "sleplet.meshes.mesh.Mesh",
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Convert the region on vertices to faces."""
     region_reshape = np.argwhere(mesh.mesh_region).reshape(-1)
     faces_in_region = np.isin(mesh.faces, region_reshape).all(axis=1)
     region_on_faces = np.zeros(mesh.faces.shape[0])
     region_on_faces[faces_in_region] = 1
     return region_on_faces
 
 
 def _create_africa_mask(
     L: int,
-    earth_flm: npt.NDArray[np.complex_],
-) -> npt.NDArray[np.float_]:
+    earth_flm: npt.NDArray[np.complex128],
+) -> npt.NDArray[np.float64]:
     """Create the Africa region mask."""
     rot_flm = sleplet.harmonic_methods.rotate_earth_to_africa(earth_flm, L)
     earth_f = ssht.inverse(
         rot_flm,
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
         Reality=True,
@@ -168,16 +168,16 @@
         Method=sleplet._vars.SAMPLING_SCHEME,
     )
     return (thetas <= _AFRICA_RANGE) & (earth_f >= 0)
 
 
 def _create_south_america_mask(
     L: int,
-    earth_flm: npt.NDArray[np.complex_],
-) -> npt.NDArray[np.float_]:
+    earth_flm: npt.NDArray[np.complex128],
+) -> npt.NDArray[np.float64]:
     """Create the Africa region mask."""
     rot_flm = sleplet.harmonic_methods.rotate_earth_to_south_america(earth_flm, L)
     earth_f = ssht.inverse(
         rot_flm,
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
         Reality=True,
@@ -186,15 +186,15 @@
         L,
         Grid=True,
         Method=sleplet._vars.SAMPLING_SCHEME,
     )
     return (thetas <= _SOUTH_AMERICA_RANGE) & (earth_f >= 0)
 
 
-def create_mask(L: int, mask_name: str) -> npt.NDArray[np.float_]:
+def create_mask(L: int, mask_name: str) -> npt.NDArray[np.float64]:
     """Create the South America region mask."""
     earth_flm = sleplet._data.create_earth_flm.create_flm(L)
     if mask_name == f"africa_L{L}.npy":
         mask = _create_africa_mask(L, earth_flm)
     elif mask_name == f"south_america_L{L}.npy":
         mask = _create_south_america_mask(L, earth_flm)
     else:
```

### Comparing `sleplet-1.4.6/src/sleplet/_mesh_methods.py` & `sleplet-1.4.7/src/sleplet/_mesh_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 _data_path = pathlib.Path(__file__).resolve().parent / "_data"
 _logger = logging.getLogger(__name__)
 
 
 def average_functions_on_vertices_to_faces(
     faces: npt.NDArray[np.int_],
-    functions_on_vertices: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.float_]:
+    functions_on_vertices: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.float64]:
     """
     Require all functions to be defined on faces
     this method handles an arbitrary number of functions.
     """
     _logger.info("converting function on vertices to faces")
     # handle the case of a 1D array
     array_is_1d = len(functions_on_vertices.shape) == 1
@@ -38,15 +38,15 @@
     if array_is_1d:
         functions_on_faces = functions_on_faces.reshape(-1)
     return functions_on_faces
 
 
 def create_mesh_region(
     mesh_config: dict[str, typing.Any],
-    vertices: npt.NDArray[np.float_],
+    vertices: npt.NDArray[np.float64],
 ) -> npt.NDArray[np.bool_]:
     """Create a boolean region for the given mesh."""
     return (
         (vertices[:, 0] >= mesh_config["XMIN"])
         & (vertices[:, 0] <= mesh_config["XMAX"])
         & (vertices[:, 1] >= mesh_config["YMIN"])
         & (vertices[:, 1] <= mesh_config["YMAX"])
@@ -62,19 +62,19 @@
         "rb",
     ) as f:
         return tomli.load(f)
 
 
 def mesh_eigendecomposition(
     name: str,
-    vertices: npt.NDArray[np.float_],
+    vertices: npt.NDArray[np.float64],
     faces: npt.NDArray[np.int_],
     *,
     number_basis_functions: int | None = None,
-) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_], int]:
+) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64], int]:
     """
     Compute the eigendecomposition of the mesh represented
     as a graph if already computed then it loads the data.
     """
     # determine number of basis functions
     if number_basis_functions is None:
         number_basis_functions = vertices.shape[0] // 4
@@ -108,36 +108,36 @@
         _logger.info("saving binaries...")
         np.save(platformdirs.user_data_path() / eval_loc, eigenvalues)
         np.save(platformdirs.user_data_path() / evec_loc, eigenvectors)
     return eigenvalues, eigenvectors, number_basis_functions
 
 
 def read_mesh(
-    mesh_config: dict[str, float | int | str]
-) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.int_]]:
+    mesh_config: dict[str, float | int | str],
+) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.int_]]:
     """Read in the given mesh."""
     vertices, faces = igl.read_triangle_mesh(
         str(_data_path / f"meshes_polygons_{mesh_config['FILENAME']}"),
     )
     return igl.upsample(vertices, faces, number_of_subdivs=mesh_config["UPSAMPLE"])
 
 
 def _mesh_laplacian(
-    vertices: npt.NDArray[np.float_],
+    vertices: npt.NDArray[np.float64],
     faces: npt.NDArray[np.int_],
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Compute the cotagent mesh laplacian."""
     return -igl.cotmatrix(vertices, faces)
 
 
 def _orthonormalise_basis_functions(
-    vertices: npt.NDArray[np.float_],
+    vertices: npt.NDArray[np.float64],
     faces: npt.NDArray[np.int_],
-    basis_functions: npt.NDArray[np.float_],
-) -> npt.NDArray[np.float_]:
+    basis_functions: npt.NDArray[np.float64],
+) -> npt.NDArray[np.float64]:
     """For computing the Slepian D matrix the basis functions must be orthonormal."""
     _logger.info("orthonormalising basis functions")
     factor = np.zeros(basis_functions.shape[0])
     for i, phi_i in enumerate(basis_functions):
         factor[i] = sleplet._integration_methods.integrate_whole_mesh(
             vertices,
             faces,
```

### Comparing `sleplet-1.4.6/src/sleplet/_parallel_methods.py` & `sleplet-1.4.7/src/sleplet/_parallel_methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,38 @@
     arr = np.arange(arr_max)
     size = len(arr)
     arr[size // 2 : size] = arr[size // 2 : size][::-1]
     return [np.sort(arr[i::ncpu]) for i in range(ncpu)]
 
 
 def create_shared_memory_array(
-    array: npt.NDArray[np.float_],
-) -> tuple[npt.NDArray[np.float_], multiprocess.shared_memory.SharedMemory]:
+    array: npt.NDArray[np.float64],
+) -> tuple[npt.NDArray[np.float64], multiprocess.shared_memory.SharedMemory]:
     """Create a shared memory array to be used in a parallel function."""
     ext_shared_memory = multiprocess.shared_memory.SharedMemory(
         create=True,
         size=array.nbytes,
     )
-    array_ext: npt.NDArray[np.float_] = np.ndarray(
+    array_ext: npt.NDArray[np.float64] = np.ndarray(
         array.shape,
         dtype=array.dtype,
         buffer=ext_shared_memory.buf,
     )
     return array_ext, ext_shared_memory
 
 
 def attach_to_shared_memory_block(
-    array: npt.NDArray[np.float_],
+    array: npt.NDArray[np.float64],
     ext_shared_memory: multiprocess.shared_memory.SharedMemory,
-) -> tuple[npt.NDArray[np.float_], multiprocess.shared_memory.SharedMemory]:
+) -> tuple[npt.NDArray[np.float64], multiprocess.shared_memory.SharedMemory]:
     """Attach an array to the shared memory within the parallel function."""
     int_shared_memory = multiprocess.shared_memory.SharedMemory(
         name=ext_shared_memory.name,
     )
-    array_int: npt.NDArray[np.float_] = np.ndarray(
+    array_int: npt.NDArray[np.float64] = np.ndarray(
         array.shape,
         dtype=array.dtype,
         buffer=int_shared_memory.buf,
     )
     return array_int, int_shared_memory
```

### Comparing `sleplet-1.4.6/src/sleplet/_plotly_methods.py` & `sleplet-1.4.7/src/sleplet/_plotly_methods.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_scripts/plotting_on_mesh.py` & `sleplet-1.4.7/src/sleplet/_scripts/plotting_on_mesh.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/_scripts/plotting_on_sphere.py` & `sleplet-1.4.7/src/sleplet/_scripts/plotting_on_sphere.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
 def _rotation_helper(
     f: sleplet.functions.coefficients.Coefficients,
     filename: str,
     alpha_pi_frac: float,
     beta_pi_frac: float,
     gamma_pi_frac: float,
-) -> tuple[npt.NDArray[np.complex_], str]:
+) -> tuple[npt.NDArray[np.complex128], str]:
     """Perform the rotation specific steps."""
     msg = (
         "angles: (alpha, beta, gamma) = "
         f"({alpha_pi_frac}, {beta_pi_frac}, {gamma_pi_frac})",
     )
     _logger.info(msg)
     filename += (
@@ -298,15 +298,15 @@
 
 def _translation_helper(
     f: sleplet.functions.coefficients.Coefficients,
     filename: str,
     alpha_pi_frac: float,
     beta_pi_frac: float,
     shannon: int | None,
-) -> tuple[npt.NDArray[np.complex_ | np.float_], str, dict[str, float | int]]:
+) -> tuple[npt.NDArray[np.complex128 | np.float64], str, dict[str, float | int]]:
     """Perform the translation specific steps."""
     msg = f"angles: (alpha, beta) = ({alpha_pi_frac}, {beta_pi_frac})"
     _logger.info(msg)
     # don't add gamma if translation
     filename += (
         "_translate_"
         f"{sleplet._string_methods.filename_angle(alpha_pi_frac, beta_pi_frac)}"
@@ -332,18 +332,18 @@
     } | _ARROW_STYLE
     return coefficients, filename, annotation
 
 
 def _convolution_helper(
     f: sleplet.functions.coefficients.Coefficients,
     g: sleplet.functions.coefficients.Coefficients,
-    coefficients: npt.NDArray[np.complex_ | np.float_],
+    coefficients: npt.NDArray[np.complex128 | np.float64],
     shannon: int | None,
     filename: str,
-) -> tuple[npt.NDArray[np.complex_ | np.float_], str]:
+) -> tuple[npt.NDArray[np.complex128 | np.float64], str]:
     """Perform the convolution specific steps."""
     g_coefficients = (
         sleplet.slepian_methods.slepian_forward(f.L, f.slepian, flm=g.coefficients)
         if hasattr(f, "slepian")
         else g.coefficients
     )
     coefficients = f.convolve(g_coefficients, coefficients, shannon=shannon)
```

### Comparing `sleplet-1.4.6/src/sleplet/_slepian_arbitrary_methods.py` & `sleplet-1.4.7/src/sleplet/_slepian_arbitrary_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 if typing.TYPE_CHECKING:
     import sleplet.meshes.mesh
 
 _MACHINE_EPSILON = 1e-14
 
 
 def clean_evals_and_evecs(
-    eigendecomposition: tuple[npt.NDArray[np.complex_], npt.NDArray[np.complex_]],
-) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    eigendecomposition: tuple[npt.NDArray[np.complex128], npt.NDArray[np.complex128]],
+) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
     """Need eigenvalues and eigenvectors to be in a certain format."""
     # access values
     eigenvalues_complex, eigenvectors = eigendecomposition
 
     # eigenvalues should be real
     eigenvalues = eigenvalues_complex.real
```

### Comparing `sleplet-1.4.6/src/sleplet/_smoothing.py` & `sleplet-1.4.7/src/sleplet/_smoothing.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 import pyssht as ssht
 
 _logger = logging.getLogger(__name__)
 
 
 def apply_gaussian_smoothing(
-    flm: npt.NDArray[np.complex_],
+    flm: npt.NDArray[np.complex128],
     L: int,
     smoothing_factor: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Apply Gaussian smoothing to the given signal.
 
     s_lm = exp(-ell^2 sigma^2)
     s(omega) = exp(-theta^2 / sigma^2)
     FWHM = 2 * sqrt(ln2) * sigma
     """
```

### Comparing `sleplet-1.4.6/src/sleplet/_string_methods.py` & `sleplet-1.4.7/src/sleplet/_string_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
 def multiples_of_pi(angle: float) -> str:
     """
     Print the unicode pi with a prefix of the multiple unless it's 1
     i.e. pi, 2pi, 3pi.
     """
     multiple = int(angle / np.pi)
-    return f"{multiple if multiple != 1 else ''}\u03C0"
+    return f"{multiple if multiple != 1 else ''}\u03c0"
 
 
 def angle_as_degree(radian: float) -> int:
     """Convert radian angle to integer degree."""
     return round(np.rad2deg(radian))
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/__init__.py` & `sleplet-1.4.7/src/sleplet/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/functions/africa.py` & `sleplet-1.4.7/src/sleplet/functions/south_america.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Contains the `Africa` class."""
+"""Contains the `SouthAmerica` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -13,26 +14,23 @@
 import sleplet._validation
 import sleplet._vars
 import sleplet.harmonic_methods
 from sleplet.functions.flm import Flm
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
-class Africa(Flm):
-    """
-    Create a topographic map of the Earth setting everything outide of the
-    Africa region to zero.
-    """
+class SouthAmerica(Flm):
+    """Create the South America region of the topographic map of the Earth."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         return sleplet.harmonic_methods._ensure_f_bandlimited(
             self._grid_fun,
             self.L,
             reality=self.reality,
             spin=self.spin,
         )
 
@@ -50,23 +48,26 @@
     def _setup_args(self: typing_extensions.Self) -> None:
         if isinstance(self.extra_args, list):
             msg = f"{self.__class__.__name__} does not support extra arguments"
             raise TypeError(msg)
 
     def _grid_fun(
         self: typing_extensions.Self,
-        theta: npt.NDArray[np.float_],  # noqa: ARG002
-        phi: npt.NDArray[np.float_],  # noqa: ARG002
-    ) -> npt.NDArray[np.float_]:
+        theta: npt.NDArray[np.float64],  # noqa: ARG002
+        phi: npt.NDArray[np.float64],  # noqa: ARG002
+    ) -> npt.NDArray[np.float64]:
         """Define the function on the grid."""
         earth_flm = sleplet._data.create_earth_flm.create_flm(
             self.L,
             smoothing=self.smoothing,
         )
-        rot_flm = sleplet.harmonic_methods.rotate_earth_to_africa(earth_flm, self.L)
+        rot_flm = sleplet.harmonic_methods.rotate_earth_to_south_america(
+            earth_flm,
+            self.L,
+        )
         earth_f = ssht.inverse(
             rot_flm,
             self.L,
             Method=sleplet._vars.SAMPLING_SCHEME,
             Reality=self.reality,
         )
         mask_name = f"{self.name}_L{self.L}.npy"
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py` & `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_africa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `AxisymmetricWaveletCoefficientsAfrica` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -36,15 +37,15 @@
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -67,15 +68,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.complex128], npt.NDArray[np.complex128]]:
         """Compute wavelet coefficients of Africa."""
         wavelets = sleplet.wavelet_methods._create_axisymmetric_wavelets(
             self.L,
             self.B,
             self.j_min,
         )
         self._africa = sleplet.functions.africa.Africa(
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py` & `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_earth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `AxisymmetricWaveletCoefficientsEarth` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -36,15 +37,15 @@
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -67,15 +68,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.complex128], npt.NDArray[np.complex128]]:
         """Compute wavelet coefficients of the Earth."""
         wavelets = sleplet.wavelet_methods._create_axisymmetric_wavelets(
             self.L,
             self.B,
             self.j_min,
         )
         self._earth = sleplet.functions.earth.Earth(self.L, smoothing=self.smoothing)
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py` & `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelet_coefficients_south_america.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `AxisymmetricWaveletCoefficientsSouthAmerica` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -35,15 +36,15 @@
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -66,15 +67,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.complex128], npt.NDArray[np.complex128]]:
         """Compute wavelet coefficients of South America."""
         wavelets = sleplet.wavelet_methods._create_axisymmetric_wavelets(
             self.L,
             self.B,
             self.j_min,
         )
         self._south_america = sleplet.functions.south_america.SouthAmerica(
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/axisymmetric_wavelets.py` & `sleplet-1.4.7/src/sleplet/functions/axisymmetric_wavelets.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `AxisymmetricWavelets` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -32,15 +33,15 @@
     whereas `0` would correspond to the selected `j_min`."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelets")
         self.wavelets = self._create_wavelets()
         _logger.info("finish computing wavelets")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelets[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -61,15 +62,15 @@
         if isinstance(self.extra_args, list):
             num_args = 3
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
-    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.complex_]:
+    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.complex128]:
         """Compute all wavelets."""
         return sleplet.wavelet_methods._create_axisymmetric_wavelets(
             self.L,
             self.B,
             self.j_min,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/coefficients.py` & `sleplet-1.4.7/src/sleplet/functions/coefficients.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `Coefficients` class."""
+
 import abc
 import dataclasses
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
@@ -31,36 +32,36 @@
     coefficients. Only to be set by the `sphere` CLI."""
     noise: float | None = None
     """How much to noise the data."""
     region: sleplet.slepian.region.Region | None = None
     """Whether to set a region or not, used in the Slepian case."""
     smoothing: int | None = None
     """How much to smooth the topographic map of the Earth by."""
-    _unnoised_coefficients: (
-        npt.NDArray[np.complex_ | np.float_] | None
-    ) = pydantic.Field(
-        default=None,
-        init_var=False,
-        repr=False,
+    _unnoised_coefficients: npt.NDArray[np.complex128 | np.float64] | None = (
+        pydantic.Field(
+            default=None,
+            init_var=False,
+            repr=False,
+        )
     )
-    coefficients: npt.NDArray[np.complex_ | np.float_] = pydantic.Field(
+    coefficients: npt.NDArray[np.complex128 | np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
     name: str = pydantic.Field(default="", init_var=False, repr=False)
     reality: bool = pydantic.Field(default=False, init_var=False, repr=False)
     snr: float | None = pydantic.Field(default=None, init_var=False, repr=False)
     spin: int = pydantic.Field(default=0, init_var=False, repr=False)
-    wavelet_coefficients: npt.NDArray[np.complex_ | np.float_] = pydantic.Field(
+    wavelet_coefficients: npt.NDArray[np.complex128 | np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
-    wavelets: npt.NDArray[np.complex_ | np.float_] = pydantic.Field(
+    wavelets: npt.NDArray[np.complex128 | np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._setup_args()
@@ -73,15 +74,15 @@
 
     def translate(
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
         *,
         shannon: int | None = None,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         r"""
         Perform the translation of the coefficients, used in the sifting convolution.
 
         Args:
             alpha: The point on the 2-sphere to translate to, i.e. the \(\phi\) value.
             beta: The point on the 2-sphere to translate to, i.e. the \(\theta\) value.
             shannon: The Shannon number, only used in the Slepian case.
@@ -94,19 +95,19 @@
             g_coefficients
             if "dirac_delta" in self.name
             else self.convolve(self.coefficients, g_coefficients, shannon=shannon)
         )
 
     def convolve(
         self: typing_extensions.Self,
-        f_coefficient: npt.NDArray[np.complex_ | np.float_],
-        g_coefficient: npt.NDArray[np.complex_ | np.float_],
+        f_coefficient: npt.NDArray[np.complex128 | np.float64],
+        g_coefficient: npt.NDArray[np.complex128 | np.float64],
         *,
         shannon: int | None = None,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """
         Perform the sifting convolution of the two inputs.
 
         Args:
             f_coefficient: Input harmonic/Slepian coefficients.
             g_coefficient: Input harmonic/Slepian coefficients.
             shannon: The Shannon number, only used in the Slepian case.
@@ -143,15 +144,15 @@
     @abc.abstractmethod
     def rotate(
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
         *,
         gamma: float = 0,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         r"""
         Rotates given flm on the sphere by alpha/beta/gamma.
 
         Args:
             alpha: The third Euler angle, a \(\alpha\) rotation about the z-axis.
             beta: The second Euler angle, a \(\beta\) rotation about the y-axis.
             gamma: The first Euler angle, a \(\gamma\) rotation about the z-axis.
@@ -162,29 +163,29 @@
         raise NotImplementedError
 
     @abc.abstractmethod
     def _translation_helper(
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         """Compute the basis function at omega' for translation."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise to the signal."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Create the flm on the north pole."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         """Create the name of the function."""
         raise NotImplementedError
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/dirac_delta.py` & `sleplet-1.4.7/src/sleplet/functions/dirac_delta.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `DiracDelta` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -16,16 +17,16 @@
     """Create a Dirac delta."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        flm = np.zeros(self.L**2, dtype=np.complex_)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        flm = np.zeros(self.L**2, dtype=np.complex128)
         for ell in range(self.L):
             ind = ssht.elm2ind(ell, 0)
             flm[ind] = np.sqrt((2 * ell + 1) / (4 * np.pi))
         return flm
 
     def _create_name(self: typing_extensions.Self) -> str:
         return sleplet._string_methods._convert_camel_case_to_snake_case(
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/earth.py` & `sleplet-1.4.7/src/sleplet/functions/earth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Earth` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._data.create_earth_flm
 import sleplet._string_methods
@@ -15,15 +16,15 @@
     """Create the topographic map of the Earth."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         return sleplet._data.create_earth_flm.create_flm(
             self.L,
             smoothing=self.smoothing,
         )
 
     def _create_name(self: typing_extensions.Self) -> str:
         return sleplet._string_methods._convert_camel_case_to_snake_case(
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/elongated_gaussian.py` & `sleplet-1.4.7/src/sleplet/functions/elongated_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `ElongatedGaussian` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -25,15 +26,15 @@
     r"""Sets the \(\sigma_{\theta}\) value."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         return sleplet.harmonic_methods._ensure_f_bandlimited(
             self._grid_fun,
             self.L,
             reality=self.reality,
             spin=self.spin,
         )
 
@@ -58,17 +59,17 @@
                 raise ValueError(msg)
             self.t_sigma, self.p_sigma = (
                 np.float_power(10, x) for x in self.extra_args
             )
 
     def _grid_fun(
         self: typing_extensions.Self,
-        theta: npt.NDArray[np.float_],
-        phi: npt.NDArray[np.float_],
-    ) -> npt.NDArray[np.float_]:
+        theta: npt.NDArray[np.float64],
+        phi: npt.NDArray[np.float64],
+    ) -> npt.NDArray[np.float64]:
         """Define the function on the grid."""
         return np.exp(
             -(
                 ((theta - sleplet._vars.THETA_0) / self.t_sigma) ** 2
                 + ((phi - sleplet._vars.PHI_0) / self.p_sigma) ** 2
             )
             / 2,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/flm.py` & `sleplet-1.4.7/src/sleplet/functions/flm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `Flm` class."""
+
 import abc
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -22,41 +23,41 @@
 
     def rotate(  # noqa: D102
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
         *,
         gamma: float = 0,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         return ssht.rotate_flms(self.coefficients, alpha, beta, gamma, self.L)
 
     def _translation_helper(
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         return ssht.create_ylm(beta, alpha, self.L).conj().flatten()
 
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise to the signal."""
-        self.coefficients: npt.NDArray[np.complex_ | np.float_]
+        self.coefficients: npt.NDArray[np.complex128 | np.float64]
         if self.noise is not None:
             unnoised_coefficients = self.coefficients.copy()
             nlm = sleplet.noise._create_noise(self.L, self.coefficients, self.noise)
             snr = sleplet.noise.compute_snr(self.coefficients, nlm, "Harmonic")
             self.coefficients = self.coefficients + nlm
             return unnoised_coefficients, snr
         return None, None
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/fp.py` & `sleplet-1.4.7/src/sleplet/functions/fp.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `Fp` class."""
+
 import abc
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -40,35 +41,35 @@
 
     def rotate(  # noqa: D102
         self: typing_extensions.Self,
         alpha: float,  # noqa: ARG002
         beta: float,  # noqa: ARG002
         *,
         gamma: float = 0,  # noqa: ARG002
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         msg = "Slepian rotation is not defined"
         raise NotImplementedError(msg)
 
     def _translation_helper(
         self: typing_extensions.Self,
         alpha: float,
         beta: float,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         return sleplet.slepian_methods._compute_s_p_omega_prime(
             self.L,
             alpha,
             beta,
             self.slepian,
         ).conj()
 
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise converted to Slepian space."""
-        self.coefficients: npt.NDArray[np.complex_ | np.float_]
+        self.coefficients: npt.NDArray[np.complex128 | np.float64]
         if self.noise is not None:
             unnoised_coefficients = self.coefficients.copy()
             n_p = sleplet.noise._create_slepian_noise(
                 self.L,
                 self.coefficients,
                 self.slepian,
                 self.noise,
@@ -77,15 +78,15 @@
             self.coefficients = self.coefficients + n_p
             return unnoised_coefficients, snr
         return None, None
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/gaussian.py` & `sleplet-1.4.7/src/sleplet/functions/gaussian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Gaussian` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -19,16 +20,16 @@
     r"""Sets the \(\sigma\) value."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        flm = np.zeros(self.L**2, dtype=np.complex_)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        flm = np.zeros(self.L**2, dtype=np.complex128)
         for ell in range(self.L):
             ind = ssht.elm2ind(ell, 0)
             flm[ind] = np.exp(-ell * (ell + 1) / (2 * self.sigma**2))
         return flm
 
     def _create_name(self: typing_extensions.Self) -> str:
         return (
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/harmonic_gaussian.py` & `sleplet-1.4.7/src/sleplet/functions/harmonic_gaussian.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `HarmonicGaussian` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -25,16 +26,16 @@
     r"""Sets the \(\sigma_{m}\) value."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        flm = np.zeros(self.L**2, dtype=np.complex_)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        flm = np.zeros(self.L**2, dtype=np.complex128)
         for ell in range(self.L):
             upsilon_l = np.exp(-((ell / self.l_sigma) ** 2) / 2)
             for m in range(-ell, ell + 1):
                 ind = ssht.elm2ind(ell, m)
                 flm[ind] = upsilon_l * np.exp(-((m / self.m_sigma) ** 2) / 2)
         return flm
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/identity.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_identity.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-"""Contains the `Identity` class."""
+"""Contains the `SlepianIdentity` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
-from sleplet.functions.flm import Flm
+from sleplet.functions.fp import Fp
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
-class Identity(Flm):
-    """Create an identity function."""
+class SlepianIdentity(Fp):
+    """Create an identify function in the Slepian region."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        return np.ones(self.L**2, dtype=np.complex_)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        return np.ones(self.L**2, dtype=np.complex128)
 
     def _create_name(self: typing_extensions.Self) -> str:
-        return sleplet._string_methods._convert_camel_case_to_snake_case(
-            self.__class__.__name__,
+        return (
+            f"{sleplet._string_methods._convert_camel_case_to_snake_case(self.__class__.__name__)}"
+            f"_{self.slepian.region._name_ending}"
         )
 
     def _set_reality(self: typing_extensions.Self) -> bool:
-        return True
+        return False
 
     def _set_spin(self: typing_extensions.Self) -> int:
         return 0
 
     def _setup_args(self: typing_extensions.Self) -> None:
         if isinstance(self.extra_args, list):
             msg = f"{self.__class__.__name__} does not support extra arguments"
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/noise_earth.py` & `sleplet-1.4.7/src/sleplet/functions/noise_earth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `NoiseEarth` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -20,15 +21,15 @@
     data."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         earth = sleplet.functions.earth.Earth(self.L, smoothing=self.smoothing)
         noise = sleplet.noise._create_noise(self.L, earth.coefficients, self.SNR)
         sleplet.noise.compute_snr(earth.coefficients, noise, "Harmonic")
         return noise
 
     def _create_name(self: typing_extensions.Self) -> str:
         return (
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/ridgelets.py` & `sleplet-1.4.7/src/sleplet/functions/ridgelets.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Ridgelets` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import scipy.special
 import typing_extensions
@@ -36,15 +37,15 @@
     """Spin value."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelets")
         self.wavelets = self._create_wavelets()
         _logger.info("finish computing wavelets")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelets[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -66,28 +67,28 @@
         if isinstance(self.extra_args, list):
             num_args = 4
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.spin, self.j = self.extra_args
 
-    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.complex_]:
+    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.complex128]:
         """Compute all wavelets."""
         ring_lm = self._compute_ring()
         kappas = sleplet.wavelet_methods.create_kappas(self.L, self.B, self.j_min)
-        wavelets = np.zeros((kappas.shape[0], self.L**2), dtype=np.complex_)
+        wavelets = np.zeros((kappas.shape[0], self.L**2), dtype=np.complex128)
         for ell in range(self.L):
             ind = ssht.elm2ind(ell, 0)
             wavelets[0, ind] = kappas[0, ell] * ring_lm[ind]
             wavelets[1:, ind] = kappas[1:, ell] * ring_lm[ind] / np.sqrt(2 * np.pi)
         return wavelets
 
-    def _compute_ring(self: typing_extensions.Self) -> npt.NDArray[np.complex_]:
+    def _compute_ring(self: typing_extensions.Self) -> npt.NDArray[np.complex128]:
         """Compute ring in harmonic space."""
-        ring_lm = np.zeros(self.L**2, dtype=np.complex_)
+        ring_lm = np.zeros(self.L**2, dtype=np.complex128)
         for ell in range(abs(self.spin), self.L):
             logp2 = (
                 scipy.special.gammaln(ell + self.spin + 1)
                 - ell * np.log(2)
                 - scipy.special.gammaln((ell + self.spin) / 2 + 1)
                 - scipy.special.gammaln((ell - self.spin) / 2 + 1)
             )
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian.py` & `sleplet-1.4.7/src/sleplet/functions/slepian.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Slepian` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -38,15 +39,15 @@
             )
             .replace(".", "-")
             .replace("+", "")
         )
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         msg = (
             f"Shannon number: {self.slepian.N}\n"
             f"Eigenvalue {self.rank}: {self.slepian.eigenvalues[self.rank]:e}"
         )
         _logger.info(msg)
         return sleplet.slepian_methods.slepian_forward(
             self.L,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_africa.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_africa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianAfrica` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -26,15 +27,15 @@
             and self.region._name_ending != "africa"
         ):
             msg = "Slepian region selected must be 'africa'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         a = sleplet.functions.africa.Africa(self.L, smoothing=self.smoothing)
         return sleplet.slepian_methods.slepian_forward(
             self.L,
             self.slepian,
             flm=a.coefficients,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_dirac_delta.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_dirac_delta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianDiracDelta` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -25,15 +26,15 @@
     _beta: float = pydantic.Field(default=0, init_var=False, repr=False)
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         self._compute_angles()
         return sleplet.slepian_methods._compute_s_p_omega_prime(
             self.L,
             self._alpha,
             self._beta,
             self.slepian,
         ).conj()
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_identity.py` & `sleplet-1.4.7/src/sleplet/functions/wmap.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-"""Contains the `SlepianIdentity` class."""
+"""Contains the `Wmap` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
+import sleplet._data.create_wmap_flm
 import sleplet._string_methods
 import sleplet._validation
-from sleplet.functions.fp import Fp
+from sleplet.functions.flm import Flm
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
-class SlepianIdentity(Fp):
-    """Create an identify function in the Slepian region."""
+class Wmap(Flm):
+    """Create the WMAP data."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        return np.ones(self.L**2, dtype=np.complex_)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        return sleplet._data.create_wmap_flm.create_flm(self.L)
 
     def _create_name(self: typing_extensions.Self) -> str:
-        return (
-            f"{sleplet._string_methods._convert_camel_case_to_snake_case(self.__class__.__name__)}"
-            f"_{self.slepian.region._name_ending}"
+        return sleplet._string_methods._convert_camel_case_to_snake_case(
+            self.__class__.__name__,
         )
 
     def _set_reality(self: typing_extensions.Self) -> bool:
-        return False
+        return True
 
     def _set_spin(self: typing_extensions.Self) -> int:
         return 0
 
     def _setup_args(self: typing_extensions.Self) -> None:
         if isinstance(self.extra_args, list):
             msg = f"{self.__class__.__name__} does not support extra arguments"
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_noise_africa.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_noise_africa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianNoiseAfrica` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -30,15 +31,15 @@
             and self.region._name_ending != "africa"
         ):
             msg = "Slepian region selected must be 'africa'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         sa = sleplet.functions.slepian_africa.SlepianAfrica(
             self.L,
             region=self.region,
             smoothing=self.smoothing,
         )
         noise = sleplet.noise._create_slepian_noise(
             self.L,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_noise_south_america.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_noise_south_america.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianNoiseSouthAmerica` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -30,15 +31,15 @@
             and self.region._name_ending != "south_america"
         ):
             msg = "Slepian region selected must be 'south_america'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         sa = sleplet.functions.slepian_south_america.SlepianSouthAmerica(
             self.L,
             region=self.region,
             smoothing=self.smoothing,
         )
         noise = sleplet.noise._create_slepian_noise(
             self.L,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_south_america.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_south_america.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianSouthAmerica` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -25,15 +26,15 @@
             and self.region._name_ending != "south_america"
         ):
             msg = "Slepian region selected must be 'south_america'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         sa = sleplet.functions.south_america.SouthAmerica(
             self.L,
             smoothing=self.smoothing,
         )
         return sleplet.slepian_methods.slepian_forward(
             self.L,
             self.slepian,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_wavelet_coefficients_africa.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_africa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianWaveletCoefficientsAfrica` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -38,15 +39,15 @@
             and self.region._name_ending != "africa"
         ):
             msg = "Slepian region selected must be 'africa'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -69,15 +70,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_ | np.float_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128 | np.float64]]:
         """Compute wavelet coefficients in Slepian space."""
         sw = sleplet.functions.slepian_wavelets.SlepianWavelets(
             self.L,
             B=self.B,
             j_min=self.j_min,
             region=self.region,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_wavelet_coefficients_south_america.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianWaveletCoefficientsSouthAmerica` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -38,15 +39,15 @@
             and self.region._name_ending != "south_america"
         ):
             msg = "Slepian region selected must be 'south_america'"
             raise RuntimeError(msg)
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -69,15 +70,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_ | np.float_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128 | np.float64]]:
         """Compute wavelet coefficients in Slepian space."""
         sw = sleplet.functions.slepian_wavelets.SlepianWavelets(
             self.L,
             B=self.B,
             j_min=self.j_min,
             region=self.region,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/slepian_wavelets.py` & `sleplet-1.4.7/src/sleplet/functions/slepian_wavelets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianWavelets` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -29,15 +30,15 @@
     whereas `0` would correspond to the selected `j_min`."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelets")
         self.wavelets = self._create_wavelets()
         _logger.info("finish computing wavelets")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelets[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -59,15 +60,15 @@
         if isinstance(self.extra_args, list):
             num_args = 3
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
-    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         """Compute wavelets in Slepian space."""
         return sleplet.wavelet_methods.create_kappas(self.L**2, self.B, self.j_min)
 
     @pydantic.field_validator("j")
     def _check_j(
         cls,  # noqa: ANN101
         v: int | None,
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/south_america.py` & `sleplet-1.4.7/src/sleplet/functions/africa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-"""Contains the `SouthAmerica` class."""
+"""Contains the `Africa` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -13,23 +14,26 @@
 import sleplet._validation
 import sleplet._vars
 import sleplet.harmonic_methods
 from sleplet.functions.flm import Flm
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
-class SouthAmerica(Flm):
-    """Create the South America region of the topographic map of the Earth."""
+class Africa(Flm):
+    """
+    Create a topographic map of the Earth setting everything outide of the
+    Africa region to zero.
+    """
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         return sleplet.harmonic_methods._ensure_f_bandlimited(
             self._grid_fun,
             self.L,
             reality=self.reality,
             spin=self.spin,
         )
 
@@ -47,26 +51,23 @@
     def _setup_args(self: typing_extensions.Self) -> None:
         if isinstance(self.extra_args, list):
             msg = f"{self.__class__.__name__} does not support extra arguments"
             raise TypeError(msg)
 
     def _grid_fun(
         self: typing_extensions.Self,
-        theta: npt.NDArray[np.float_],  # noqa: ARG002
-        phi: npt.NDArray[np.float_],  # noqa: ARG002
-    ) -> npt.NDArray[np.float_]:
+        theta: npt.NDArray[np.float64],  # noqa: ARG002
+        phi: npt.NDArray[np.float64],  # noqa: ARG002
+    ) -> npt.NDArray[np.float64]:
         """Define the function on the grid."""
         earth_flm = sleplet._data.create_earth_flm.create_flm(
             self.L,
             smoothing=self.smoothing,
         )
-        rot_flm = sleplet.harmonic_methods.rotate_earth_to_south_america(
-            earth_flm,
-            self.L,
-        )
+        rot_flm = sleplet.harmonic_methods.rotate_earth_to_africa(earth_flm, self.L)
         earth_f = ssht.inverse(
             rot_flm,
             self.L,
             Method=sleplet._vars.SAMPLING_SCHEME,
             Reality=self.reality,
         )
         mask_name = f"{self.name}_L{self.L}.npy"
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/spherical_harmonic.py` & `sleplet-1.4.7/src/sleplet/functions/spherical_harmonic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SphericalHarmonic` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import pyssht as ssht
 
@@ -19,15 +20,15 @@
     ell: int = 0
     r"""Degree \(\ell \geq 0\)."""
     m: int = 0
     r"""Order \(\leq |\ell|\)"""
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         ind = ssht.elm2ind(self.ell, self.m)
         return sleplet.harmonic_methods._create_spherical_harmonic(self.L, ind)
 
     def _create_name(self: typing_extensions.Self) -> str:
         return (
             f"{sleplet._string_methods._convert_camel_case_to_snake_case(self.__class__.__name__)}"
             f"{sleplet._string_methods.filename_args(self.ell, 'l')}"
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/squashed_gaussian.py` & `sleplet-1.4.7/src/sleplet/functions/squashed_gaussian.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SquashedGaussian` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -25,15 +26,15 @@
     r"""Sets the \(\sigma_{\theta}\) value."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         return sleplet.harmonic_methods._ensure_f_bandlimited(
             self._grid_fun,
             self.L,
             reality=self.reality,
             spin=self.spin,
         )
 
@@ -56,14 +57,14 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.t_sigma, self.freq = (np.float_power(10, x) for x in self.extra_args)
 
     def _grid_fun(
         self: typing_extensions.Self,
-        theta: npt.NDArray[np.float_],
-        phi: npt.NDArray[np.float_],
-    ) -> npt.NDArray[np.float_]:
+        theta: npt.NDArray[np.float64],
+        phi: npt.NDArray[np.float64],
+    ) -> npt.NDArray[np.float64]:
         """Define the function on the grid."""
         return np.exp(
             -(((theta - sleplet._vars.THETA_0) / self.t_sigma) ** 2) / 2,
         ) * np.sin(self.freq * phi)
```

### Comparing `sleplet-1.4.6/src/sleplet/functions/wmap.py` & `sleplet-1.4.7/src/sleplet/functions/identity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-"""Contains the `Wmap` class."""
+"""Contains the `Identity` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
-import sleplet._data.create_wmap_flm
 import sleplet._string_methods
 import sleplet._validation
 from sleplet.functions.flm import Flm
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
-class Wmap(Flm):
-    """Create the WMAP data."""
+class Identity(Flm):
+    """Create an identity function."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
-        return sleplet._data.create_wmap_flm.create_flm(self.L)
+    ) -> npt.NDArray[np.complex128 | np.float64]:
+        return np.ones(self.L**2, dtype=np.complex128)
 
     def _create_name(self: typing_extensions.Self) -> str:
         return sleplet._string_methods._convert_camel_case_to_snake_case(
             self.__class__.__name__,
         )
 
     def _set_reality(self: typing_extensions.Self) -> bool:
```

### Comparing `sleplet-1.4.6/src/sleplet/harmonic_methods.py` & `sleplet-1.4.7/src/sleplet/harmonic_methods.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods to perform operations in Fourier space of the sphere or mesh."""
+
 import collections
 import typing
 
 import numpy as np
 import numpy.typing as npt
 
 import pyssht as ssht
@@ -15,37 +16,37 @@
 _AFRICA_BETA = np.deg2rad(87)
 _AFRICA_GAMMA = np.deg2rad(341)
 _SOUTH_AMERICA_ALPHA = np.deg2rad(54)
 _SOUTH_AMERICA_BETA = np.deg2rad(108)
 _SOUTH_AMERICA_GAMMA = np.deg2rad(63)
 
 
-def _create_spherical_harmonic(L: int, ind: int) -> npt.NDArray[np.complex_]:
+def _create_spherical_harmonic(L: int, ind: int) -> npt.NDArray[np.complex128]:
     """Create a spherical harmonic in harmonic space for the given index."""
-    flm = np.zeros(L**2, dtype=np.complex_)
+    flm = np.zeros(L**2, dtype=np.complex128)
     flm[ind] = 1
     return flm
 
 
 def _boost_coefficient_resolution(
     flm: npt.NDArray[typing.Any],
     boost: int,
 ) -> npt.NDArray[typing.Any]:
     """Calculate a boost in resolution for given flm."""
     return np.pad(flm, (0, boost), "constant")
 
 
 def invert_flm_boosted(
-    flm: npt.NDArray[np.complex_],
+    flm: npt.NDArray[np.complex128],
     L: int,
     resolution: int,
     *,
     reality: bool = False,
     spin: int = 0,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Upsamples the signal and performs the inverse harmonic transform .
 
     Args:
         flm: The spherical harmonic coefficients.
         L: The spherical harmonic bandlimit.
         resolution: The output resolution of the field values.
@@ -64,22 +65,22 @@
         Reality=reality,
         Spin=spin,
     )
 
 
 def _ensure_f_bandlimited(
     grid_fun: collections.abc.Callable[
-        [npt.NDArray[np.float_], npt.NDArray[np.float_]],
-        npt.NDArray[np.float_],
+        [npt.NDArray[np.float64], npt.NDArray[np.float64]],
+        npt.NDArray[np.float64],
     ],
     L: int,
     *,
     reality: bool,
     spin: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     If the function created is created in pixel space rather than harmonic
     space then need to transform it into harmonic space first before using it.
     """
     thetas, phis = ssht.sample_positions(
         L,
         Grid=True,
@@ -91,15 +92,15 @@
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
         Reality=reality,
         Spin=spin,
     )
 
 
-def _create_emm_vector(L: int) -> npt.NDArray[np.float_]:
+def _create_emm_vector(L: int) -> npt.NDArray[np.float64]:
     """Create vector of m values for a given L."""
     emm = np.zeros(2 * L * 2 * L)
     k = 0
 
     for ell in range(2 * L):
         M = 2 * ell + 1
         emm[k : k + M] = np.arange(-ell, ell + 1)
@@ -108,15 +109,15 @@
 
 
 def compute_random_signal(
     L: int,
     rng: np.random.Generator,
     *,
     var_signal: float,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Generate a normally distributed random signal of a
     complex signal with mean `0` and variance `1`.
 
     Args:
         L: The spherical harmonic bandlimit.
         rng: The random number generator object.
@@ -128,16 +129,16 @@
     return np.sqrt(var_signal / 2) * (
         rng.standard_normal(L**2) + 1j * rng.standard_normal(L**2)
     )
 
 
 def mesh_forward(
     mesh: "sleplet.meshes.mesh.Mesh",
-    u: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.float_]:
+    u: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.float64]:
     """
     Compute the mesh forward transform from pixel space to Fourier space.
 
     Args:
         mesh: The given mesh object.
         u: The signal field value on the mesh.
 
@@ -153,33 +154,33 @@
             phi_i,
         )
     return u_i
 
 
 def mesh_inverse(
     mesh: "sleplet.meshes.mesh.Mesh",
-    u_i: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.complex_ | np.float_]:
+    u_i: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Compute the mesh inverse transform from Fourier space to pixel space.
 
     Args:
         mesh: The given mesh object.
         u_i: The Fourier coefficients on the mesh.
 
     Returns:
         The values on the mesh in pixel space.
     """
     return (u_i[:, np.newaxis] * mesh.basis_functions).sum(axis=0)
 
 
 def rotate_earth_to_south_america(
-    earth_flm: npt.NDArray[np.complex_ | np.float_],
+    earth_flm: npt.NDArray[np.complex128 | np.float64],
     L: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Rotates the harmonic coefficients of the Earth to a view centered on South America.
 
     Args:
         earth_flm: The spherical harmonic coefficients of the Earth.
         L: The spherical harmonic bandlimit.
 
@@ -192,17 +193,17 @@
         _SOUTH_AMERICA_BETA,
         _SOUTH_AMERICA_GAMMA,
         L,
     )
 
 
 def rotate_earth_to_africa(
-    earth_flm: npt.NDArray[np.complex_ | np.float_],
+    earth_flm: npt.NDArray[np.complex128 | np.float64],
     L: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Rotates the harmonic coefficients of the Earth to a view centered on Africa.
 
     Args:
         earth_flm: The spherical harmonic coefficients of the Earth.
         L: The spherical harmonic bandlimit.
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/__init__.py` & `sleplet-1.4.7/src/sleplet/meshes/__init__.py`

 * *Files identical despite different names*

### Comparing `sleplet-1.4.6/src/sleplet/meshes/_mesh_slepian_decomposition.py` & `sleplet-1.4.7/src/sleplet/meshes/_mesh_slepian_decomposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class MeshSlepianDecomposition:
     mesh_slepian: MeshSlepian
     _: dataclasses.KW_ONLY
     mask: bool = False
-    u_i: npt.NDArray[np.complex_ | np.float_] | None = None
-    u: npt.NDArray[np.complex_ | np.float_] | None = None
+    u_i: npt.NDArray[np.complex128 | np.float64] | None = None
+    u: npt.NDArray[np.complex128 | np.float64] | None = None
     _method: str = pydantic.Field(default="", init_var=False, repr=False)
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._detect_method()
 
     def decompose(self: typing_extensions.Self, rank: int) -> float:
         """Decompose the signal into its Slepian coefficients via the given method."""
@@ -40,15 +40,15 @@
             case _:
                 msg = f"'{self._method}' is not a valid method"
                 raise ValueError(msg)
 
     def decompose_all(
         self: typing_extensions.Self,
         n_coefficients: int,
-    ) -> npt.NDArray[np.float_]:
+    ) -> npt.NDArray[np.float64]:
         """Decompose all ranks of the Slepian coefficients."""
         coefficients = np.zeros(n_coefficients)
         for rank in range(n_coefficients):
             coefficients[rank] = self.decompose(rank)
         return coefficients
 
     def _integrate_region(self: typing_extensions.Self, rank: int) -> float:
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Mesh` class."""
+
 import dataclasses
 
 import numpy as np
 import numpy.typing as npt
 import plotly.graph_objs as go
 import pydantic
 import typing_extensions
@@ -28,35 +29,35 @@
     plots."""
     _camera_view: go.layout.scene.Camera | None = pydantic.Field(
         default=go.layout.scene.Camera(),
         init_var=False,
         repr=False,
     )
     _colourbar_pos: float = pydantic.Field(default=0, init_var=False, repr=False)
-    basis_functions: npt.NDArray[np.float_] = pydantic.Field(
+    basis_functions: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
-    faces: npt.NDArray[np.float_] = pydantic.Field(
+    faces: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
-    mesh_eigenvalues: npt.NDArray[np.float_] = pydantic.Field(
+    mesh_eigenvalues: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
     mesh_region: npt.NDArray[np.bool_] = pydantic.Field(
         default_factory=lambda: np.empty(0, dtype=np.bool_),
         init_var=False,
         repr=False,
     )
-    vertices: npt.NDArray[np.float_] = pydantic.Field(
+    vertices: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         mesh_config = sleplet._mesh_methods.extract_mesh_config(self.name)
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_basis_functions.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_basis_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshBasisFunctions` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -23,15 +24,15 @@
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._validate_rank()
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Compute field on the vertices of the mesh."""
         msg = (
             f"Mesh eigenvalue {self.rank}: "
             f"{self.mesh.mesh_eigenvalues[self.rank]:e}",
         )
         _logger.info(msg)
         basis_function = self.mesh.basis_functions[self.rank]
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_coefficients.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_coefficients.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `MeshCoefficients` class."""
+
 import abc
 import dataclasses
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
@@ -26,34 +27,34 @@
     extra_args: list[int] | None = None
     """Control the extra arguments for the given set of mesh
     coefficients. Only to be set by the `mesh` CLI."""
     noise: float | None = None
     """How much to noise the data."""
     region: bool = False
     """Whether to set a region or not, used in the Slepian case."""
-    _unnoised_coefficients: (
-        npt.NDArray[np.complex_ | np.float_] | None
-    ) = pydantic.Field(
-        default=None,
-        init_var=False,
-        repr=False,
+    _unnoised_coefficients: npt.NDArray[np.complex128 | np.float64] | None = (
+        pydantic.Field(
+            default=None,
+            init_var=False,
+            repr=False,
+        )
     )
-    coefficients: npt.NDArray[np.complex_ | np.float_] = pydantic.Field(
+    coefficients: npt.NDArray[np.complex128 | np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
     name: str = pydantic.Field(default="", init_var=False, repr=False)
     snr: float | None = pydantic.Field(default=None, init_var=False, repr=False)
-    wavelet_coefficients: npt.NDArray[np.complex_ | np.float_] = pydantic.Field(
+    wavelet_coefficients: npt.NDArray[np.complex128 | np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
-    wavelets: npt.NDArray[np.float_] = pydantic.Field(
+    wavelets: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._setup_args()
@@ -70,22 +71,22 @@
             self.name += f"{sleplet._string_methods.filename_args(self.noise, 'noise')}"
         if self.mesh.zoom:
             self.name += "_zoom"
 
     @abc.abstractmethod
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise to the signal."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Create the flm on the north pole."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         """Create the name of the function."""
         raise NotImplementedError
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_field.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshField` class."""
+
 import igl
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._validation
@@ -15,15 +16,15 @@
     """Create a per-vertex normals field on a given mesh."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Compute field on the vertices of the mesh."""
         field = igl.per_vertex_normals(self.mesh.vertices, self.mesh.faces)[:, 1]
         return sleplet.harmonic_methods.mesh_forward(self.mesh, field)
 
     def _create_name(self: typing_extensions.Self) -> str:
         return f"{self.mesh.name}_field"
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_harmonic_coefficients.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_harmonic_coefficients.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `MeshHarmonicCoefficients` class."""
+
 import abc
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -16,29 +17,29 @@
     """Abstract parent class to handle Fourier coefficients on the mesh."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise to the signal."""
-        self.coefficients: npt.NDArray[np.complex_ | np.float_]
+        self.coefficients: npt.NDArray[np.complex128 | np.float64]
         if self.noise is not None:
             unnoised_coefficients = self.coefficients.copy()
             nlm = sleplet.noise._create_mesh_noise(self.coefficients, self.noise)
             snr = sleplet.noise.compute_snr(self.coefficients, nlm, "Harmonic")
             self.coefficients = self.coefficients + nlm
             return unnoised_coefficients, snr
         return None, None
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_noise_field.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_noise_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshNoiseField` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -20,15 +21,15 @@
     data."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         mf = sleplet.meshes.mesh_slepian.MeshField(self.mesh)
         noise = sleplet.noise._create_mesh_noise(mf.coefficients, self.SNR)
         sleplet.noise.compute_snr(mf.coefficients, noise, "Harmonic")
         return noise
 
     def _create_name(self: typing_extensions.Self) -> str:
         return (
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepian` class."""
+
 import concurrent.futures
 import logging
 import os
 
 import numpy as np
 import numpy.linalg as LA  # noqa: N812
 import numpy.typing as npt
@@ -24,20 +25,20 @@
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class MeshSlepian:
     """Create Slepian object of a given mesh."""
 
     mesh: Mesh
     """A mesh object."""
     N: int = pydantic.Field(default=0, init_var=False, repr=False)
-    slepian_eigenvalues: npt.NDArray[np.float_] = pydantic.Field(
+    slepian_eigenvalues: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
-    slepian_functions: npt.NDArray[np.float_] = pydantic.Field(
+    slepian_functions: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self.N = sleplet._slepian_arbitrary_methods.compute_mesh_shannon(self.mesh)
@@ -90,15 +91,15 @@
         np.save(
             platformdirs.user_data_path() / evec_loc,
             self.slepian_functions[: self.N],
         )
 
     def _create_D_matrix(  # noqa: N802
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.float_]:
+    ) -> npt.NDArray[np.float64]:
         """Compute the D matrix for the mesh eigenfunctions."""
         D = np.zeros(
             (self.mesh.mesh_eigenvalues.shape[0], self.mesh.mesh_eigenvalues.shape[0]),
         )
 
         D_ext, shm_ext = sleplet._parallel_methods.create_shared_memory_array(D)
 
@@ -137,15 +138,15 @@
         # Free and release the shared memory block at the very end
         sleplet._parallel_methods.free_shared_memory(shm_ext)
         sleplet._parallel_methods.release_shared_memory(shm_ext)
         return D
 
     def _fill_D_elements(  # noqa: N802
         self: typing_extensions.Self,
-        D: npt.NDArray[np.float_],
+        D: npt.NDArray[np.float64],
         i: int,
     ) -> None:
         """Fill in the D matrix elements using symmetries."""
         D[i][i] = self._integral(i, i)
         for j in range(i + 1, self.mesh.mesh_eigenvalues.shape[0]):
             D[j][i] = self._integral(j, i)
 
@@ -157,16 +158,16 @@
             self.mesh.faces,
             self.mesh.basis_functions[i],
             self.mesh.basis_functions[j],
         )
 
     @staticmethod
     def _clean_evals_and_evecs(
-        eigendecomposition: tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]],
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.float_]]:
+        eigendecomposition: tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]],
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
         """Need eigenvalues and eigenvectors to be in a certain format."""
         # access values
         eigenvalues, eigenvectors = eigendecomposition
 
         # sort eigenvalues and eigenvectors in descending order of eigenvalues
         idx = eigenvalues.argsort()[::-1]
         eigenvalues = eigenvalues[idx]
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_coefficients.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_coefficients.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `MeshSlepianCoefficients` class."""
+
 import abc
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -24,17 +25,17 @@
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self.mesh_slepian = sleplet.meshes.mesh_slepian.MeshSlepian(self.mesh)
         super().__post_init__()
 
     def _add_noise_to_signal(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.complex_ | np.float_] | None, float | None]:
+    ) -> tuple[npt.NDArray[np.complex128 | np.float64] | None, float | None]:
         """Add Gaussian white noise converted to Slepian space."""
-        self.coefficients: npt.NDArray[np.complex_ | np.float_]
+        self.coefficients: npt.NDArray[np.complex128 | np.float64]
         if self.noise is not None:
             unnoised_coefficients = self.coefficients.copy()
             n_p = sleplet.noise._create_slepian_mesh_noise(
                 self.mesh_slepian,
                 self.coefficients,
                 self.noise,
             )
@@ -42,15 +43,15 @@
             self.coefficients = self.coefficients + n_p
             return unnoised_coefficients, snr
         return None, None
 
     @abc.abstractmethod
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         raise NotImplementedError
 
     @abc.abstractmethod
     def _create_name(self: typing_extensions.Self) -> str:
         raise NotImplementedError
 
     @abc.abstractmethod
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_field.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepianField` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._validation
 import sleplet.meshes.mesh_field
@@ -18,15 +19,15 @@
     """
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Compute field on the vertices of the mesh."""
         mf = sleplet.meshes.mesh_field.MeshField(
             self.mesh,
             region=True,
         )
         return sleplet.slepian_methods.slepian_mesh_forward(
             self.mesh_slepian,
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_functions.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepianFunctions` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -22,15 +23,15 @@
     selects a given Slepian function from the spectrum (p in the papers)."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         """Compute field on the vertices of the mesh."""
         msg = (
             f"Slepian eigenvalue {self.rank}: "
             f"{self.mesh_slepian.slepian_eigenvalues[self.rank]:e}",
         )
         _logger.info(msg)
         s_p_i = self.mesh_slepian.slepian_functions[self.rank]
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_noise_field.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_noise_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepianNoiseField` class."""
+
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
 import sleplet._string_methods
 import sleplet._validation
@@ -23,15 +24,15 @@
     data."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         smf = sleplet.meshes.mesh_slepian_field.MeshSlepianField(
             self.mesh,
             region=True,
         )
         noise = sleplet.noise._create_slepian_mesh_noise(
             self.mesh_slepian,
             smf.coefficients,
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelet_coefficients.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepianWaveletCoefficients` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -31,15 +32,15 @@
     whereas `0` would correspond to the selected `j_min`."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelet coefficients")
         self.wavelets, self.wavelet_coefficients = self._create_wavelet_coefficients()
         _logger.info("finish computing wavelet coefficients")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelet_coefficients[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -56,15 +57,15 @@
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
     def _create_wavelet_coefficients(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_ | np.float_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128 | np.float64]]:
         """Compute wavelet coefficients in Slepian space."""
         smw = sleplet.meshes.mesh_slepian_wavelets.MeshSlepianWavelets(
             self.mesh,
             B=self.B,
             j_min=self.j_min,
         )
         smf = sleplet.meshes.mesh_slepian_field.MeshSlepianField(
```

### Comparing `sleplet-1.4.6/src/sleplet/meshes/mesh_slepian_wavelets.py` & `sleplet-1.4.7/src/sleplet/meshes/mesh_slepian_wavelets.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `MeshSlepianWavelets` class."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
 import typing_extensions
 
@@ -29,15 +30,15 @@
     whereas `0` would correspond to the selected `j_min`."""
 
     def __post_init__(self: typing_extensions.Self) -> None:
         super().__post_init__()
 
     def _create_coefficients(
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_ | np.float_]:
+    ) -> npt.NDArray[np.complex128 | np.float64]:
         _logger.info("start computing wavelets")
         self.wavelets = self._create_wavelets()
         _logger.info("finish computing wavelets")
         jth = 0 if self.j is None else self.j + 1
         return self.wavelets[jth]
 
     def _create_name(self: typing_extensions.Self) -> str:
@@ -52,15 +53,15 @@
         if isinstance(self.extra_args, list):
             num_args = 3
             if len(self.extra_args) != num_args:
                 msg = f"The number of extra arguments should be {num_args}"
                 raise ValueError(msg)
             self.B, self.j_min, self.j = self.extra_args
 
-    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_wavelets(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         """Create Slepian wavelets of the mesh."""
         return sleplet.wavelet_methods.create_kappas(
             self.mesh.mesh_eigenvalues.shape[0],
             self.B,
             self.j_min,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/noise.py` & `sleplet-1.4.7/src/sleplet/noise.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods to handle noise in Fourier or wavelet space."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 
 import pyssht as ssht
 
@@ -11,22 +12,22 @@
 import sleplet.meshes.mesh_slepian
 import sleplet.slepian_methods
 from sleplet.slepian.slepian_functions import SlepianFunctions
 
 _logger = logging.getLogger(__name__)
 
 
-def _signal_power(signal: npt.NDArray[np.complex_ | np.float_]) -> float:
+def _signal_power(signal: npt.NDArray[np.complex128 | np.float64]) -> float:
     """Compute the power of the signal."""
     return (np.abs(signal) ** 2).sum()
 
 
 def compute_snr(
-    signal: npt.NDArray[np.complex_ | np.float_],
-    noise: npt.NDArray[np.complex_ | np.float_],
+    signal: npt.NDArray[np.complex128 | np.float64],
+    noise: npt.NDArray[np.complex128 | np.float64],
     signal_type: str,
 ) -> float:
     """
     Compute the signal to noise ratio.
 
     Args:
         signal: The unnoised signal.
@@ -39,15 +40,15 @@
     snr = 10 * np.log10(_signal_power(signal) / _signal_power(noise))
     msg = f"{signal_type} SNR: {snr:.2f}"
     _logger.info(msg)
     return snr
 
 
 def compute_sigma_noise(
-    signal: npt.NDArray[np.complex_ | np.float_],
+    signal: npt.NDArray[np.complex128 | np.float64],
     snr_in: float,
     *,
     denominator: int | None = None,
 ) -> float:
     """
     Compute the standard deviation of the noise.
 
@@ -62,23 +63,23 @@
     if denominator is None:
         denominator = signal.shape[0]
     return np.sqrt(10 ** (-snr_in / 10) * _signal_power(signal) / denominator)
 
 
 def _create_noise(
     L: int,
-    signal: npt.NDArray[np.complex_ | np.float_],
+    signal: npt.NDArray[np.complex128 | np.float64],
     snr_in: float,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Compute Gaussian white noise."""
     # set random seed
     rng = np.random.default_rng(sleplet._vars.RANDOM_SEED)
 
     # initialise
-    nlm = np.zeros(L**2, dtype=np.complex_)
+    nlm = np.zeros(L**2, dtype=np.complex128)
 
     # std dev of the noise
     sigma_noise = compute_sigma_noise(signal, snr_in)
 
     # compute noise
     for ell in range(L):
         ind = ssht.elm2ind(ell, 0)
@@ -93,44 +94,44 @@
             )
             nlm[ind_nm] = (-1) ** m * nlm[ind_pm].conj()
     return nlm
 
 
 def _create_slepian_noise(
     L: int,
-    slepian_signal: npt.NDArray[np.complex_ | np.float_],
+    slepian_signal: npt.NDArray[np.complex128 | np.float64],
     slepian: SlepianFunctions,
     snr_in: float,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Compute Gaussian white noise in Slepian space."""
     flm = ssht.forward(
         sleplet.slepian_methods.slepian_inverse(slepian_signal, L, slepian),
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
     )
     nlm = _create_noise(L, flm, snr_in)
     return sleplet.slepian_methods.slepian_forward(L, slepian, flm=nlm)
 
 
 def _perform_hard_thresholding(
-    f: npt.NDArray[np.complex_ | np.float_],
-    sigma_j: float | npt.NDArray[np.float_],
+    f: npt.NDArray[np.complex128 | np.float64],
+    sigma_j: float | npt.NDArray[np.float64],
     n_sigma: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Set pixels in pixel space to zero if the magnitude is less than the threshold."""
     threshold = n_sigma * sigma_j
     return np.where(np.abs(f) < threshold, 0, f)
 
 
 def harmonic_hard_thresholding(
     L: int,
-    wav_coeffs: npt.NDArray[np.complex_],
-    sigma_j: npt.NDArray[np.float_],
+    wav_coeffs: npt.NDArray[np.complex128],
+    sigma_j: npt.NDArray[np.float64],
     n_sigma: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     r"""
     Perform thresholding in harmonic space.
 
     Args:
         L: The spherical harmonic bandlimit.
         wav_coeffs: The harmonic wavelet coefficients.
         sigma_j: The wavelet standard deviation \(\sigma_{j}\).
@@ -151,19 +152,19 @@
             Method=sleplet._vars.SAMPLING_SCHEME,
         )
     return wav_coeffs
 
 
 def slepian_wavelet_hard_thresholding(
     L: int,
-    wav_coeffs: npt.NDArray[np.complex_ | np.float_],
-    sigma_j: npt.NDArray[np.float_],
+    wav_coeffs: npt.NDArray[np.complex128 | np.float64],
+    sigma_j: npt.NDArray[np.float64],
     n_sigma: int,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     r"""
     Perform thresholding in Slepian wavelet space.
 
     Args:
         L: The spherical harmonic bandlimit.
         wav_coeffs: The Slepian wavelet coefficients
         sigma_j: The wavelet standard deviation \(\sigma_{j}\).
@@ -185,19 +186,19 @@
             f=f_thresholded,
         )
     return wav_coeffs
 
 
 def slepian_function_hard_thresholding(
     L: int,
-    coefficients: npt.NDArray[np.complex_ | np.float_],
+    coefficients: npt.NDArray[np.complex128 | np.float64],
     sigma: float,
     n_sigma: int,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     r"""
     Perform thresholding in Slepian space.
 
     Args:
         L: The spherical harmonic bandlimit.
         coefficients: The Slepian coefficients.
         sigma: The standard deviation of the noise \(\sigma\).
@@ -210,43 +211,43 @@
     _logger.info("begin Slepian hard thresholding")
     f = sleplet.slepian_methods.slepian_inverse(coefficients, L, slepian)
     f_thresholded = _perform_hard_thresholding(f, sigma, n_sigma)
     return sleplet.slepian_methods.slepian_forward(L, slepian, f=f_thresholded)
 
 
 def _compute_sigma_j(
-    signal: npt.NDArray[np.complex_ | np.float_],
-    psi_j: npt.NDArray[np.complex_],
+    signal: npt.NDArray[np.complex128 | np.float64],
+    psi_j: npt.NDArray[np.complex128],
     snr_in: float,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Compute sigma_j for wavelets used in denoising the signal."""
     sigma_noise = compute_sigma_noise(signal, snr_in)
     wavelet_power = (np.abs(psi_j) ** 2).sum(axis=1)
     return sigma_noise * np.sqrt(wavelet_power)
 
 
 def _compute_slepian_sigma_j(
     L: int,
-    signal: npt.NDArray[np.complex_ | np.float_],
-    psi_j: npt.NDArray[np.float_],
+    signal: npt.NDArray[np.complex128 | np.float64],
+    psi_j: npt.NDArray[np.float64],
     snr_in: float,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Compute sigma_j for wavelets used in denoising the signal."""
     sigma_noise = compute_sigma_noise(signal, snr_in, denominator=L**2)
     s_p = sleplet.slepian_methods.compute_s_p_omega(L, slepian)
     psi_j_reshape = psi_j[:, : slepian.N, np.newaxis, np.newaxis]
     wavelet_power = (np.abs(psi_j_reshape) ** 2 * np.abs(s_p) ** 2).sum(axis=1)
     return sigma_noise * np.sqrt(wavelet_power)
 
 
 def _create_mesh_noise(
-    u_i: npt.NDArray[np.complex_ | np.float_],
+    u_i: npt.NDArray[np.complex128 | np.float64],
     snr_in: float,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Compute Gaussian white noise."""
     # set random seed
     rng = np.random.default_rng(sleplet._vars.RANDOM_SEED)
 
     # initialise
     n_i = np.zeros(u_i.shape[0])
 
@@ -257,17 +258,17 @@
     for i in range(u_i.shape[0]):
         n_i[i] = sigma_noise * rng.standard_normal()
     return n_i
 
 
 def _create_slepian_mesh_noise(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
-    slepian_signal: npt.NDArray[np.complex_ | np.float_],
+    slepian_signal: npt.NDArray[np.complex128 | np.float64],
     snr_in: float,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Compute Gaussian white noise in Slepian space."""
     u_i = sleplet.harmonic_methods.mesh_forward(
         mesh_slepian.mesh,
         sleplet.slepian_methods.slepian_mesh_inverse(
             mesh_slepian,
             slepian_signal,
         ),
@@ -277,18 +278,18 @@
         mesh_slepian,
         u_i=n_i,
     )
 
 
 def compute_slepian_mesh_sigma_j(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
-    signal: npt.NDArray[np.complex_ | np.float_],
-    psi_j: npt.NDArray[np.float_],
+    signal: npt.NDArray[np.complex128 | np.float64],
+    psi_j: npt.NDArray[np.float64],
     snr_in: float,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     r"""
     Compute \(\sigma_{j}\) for wavelets used in denoising the signal.
 
     Args:
         mesh_slepian: The Slepian mesh object containing the eigensolutions.
         signal: The noised signal.
         psi_j: The Slepian wavelet coefficients.
@@ -306,18 +307,18 @@
     psi_j_reshape = psi_j[:, : mesh_slepian.N, np.newaxis]
     wavelet_power = (np.abs(psi_j_reshape) ** 2 * np.abs(s_p) ** 2).sum(axis=1)
     return sigma_noise * np.sqrt(wavelet_power)
 
 
 def slepian_mesh_hard_thresholding(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
-    wav_coeffs: npt.NDArray[np.complex_ | np.float_],
-    sigma_j: npt.NDArray[np.float_],
+    wav_coeffs: npt.NDArray[np.complex128 | np.float64],
+    sigma_j: npt.NDArray[np.float64],
     n_sigma: int,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     r"""
     Perform thresholding in Slepian space of the mesh.
 
     Args:
         mesh_slepian: The Slepian mesh object containing the eigensolutions.
         wav_coeffs: The Slepian wavelet coefficients of the mesh.
         sigma_j: The wavelet standard deviation \(\sigma_{j}\).
```

### Comparing `sleplet-1.4.6/src/sleplet/plot_methods.py` & `sleplet-1.4.7/src/sleplet/plot_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods to help in creating plots."""
+
 import logging
 
 import matplotlib as mpl
 import numpy as np
 import numpy.typing as npt
 
 import pyssht as ssht
@@ -122,34 +123,34 @@
     )
 
     # find maximum absolute value for given plot type
     return np.abs(_create_plot_type(boosted_field, plot_type)).max()
 
 
 def _create_plot_type(
-    field: npt.NDArray[np.complex_ | np.float_],
+    field: npt.NDArray[np.complex128 | np.float64],
     plot_type: str,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Get the given plot type of the field."""
     msg = f"plotting type: '{plot_type}'"
     _logger.info(msg)
     plot_dict = {
         "abs": np.abs(field),
         "imag": field.imag,
         "real": field.real,
         "sum": field.real + field.imag,
     }
     return plot_dict[plot_type]
 
 
 def _set_outside_region_to_minimum(
-    f_plot: npt.NDArray[np.float_],
+    f_plot: npt.NDArray[np.float64],
     L: int,
     region: sleplet.slepian.region.Region,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """
     For the Slepian region set the outside area to negative infinity
     hence it is clear we are only interested in the coloured region.
     """
     # create mask of interest
     mask = sleplet._mask_methods.create_mask_region(L, region)
 
@@ -158,37 +159,37 @@
     closed_mask = np.insert(mask, n_phi, mask[:, 0], axis=1)
 
     # set values outside mask to negative infinity
     return np.where(closed_mask, f_plot, sleplet._vars.SPHERE_UNSEEN)
 
 
 def _normalise_function(
-    f: npt.NDArray[np.float_],
+    f: npt.NDArray[np.float64],
     *,
     normalise: bool,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Normalise function between 0 and 1 for visualisation."""
     if not normalise:
         return f
     if (f == 0).all():
         # if all 0, set to 0
         return f + 0.5
     # if all non-zero, set to 1 otherwise scale from [0, 1]
     return f / f.max() if np.allclose(f, f.max()) else (f - f.min()) / f.ptp()
 
 
 def _boost_field(  # noqa: PLR0913
-    field: npt.NDArray[np.complex_ | np.float_],
+    field: npt.NDArray[np.complex128 | np.float64],
     L: int,
     resolution: int,
     *,
     reality: bool,
     spin: int,
     upsample: bool,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """Inverts and then boosts the field before plotting."""
     if not upsample:
         return field
     flm = ssht.forward(
         field,
         L,
         Method=sleplet._vars.SAMPLING_SCHEME,
@@ -221,16 +222,16 @@
         if f._unnoised_coefficients is not None
         else None
     )
 
 
 def _coefficients_to_field_mesh(
     f: sleplet.meshes.mesh_coefficients.MeshCoefficients,
-    coefficients: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.complex_ | np.float_]:
+    coefficients: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.complex128 | np.float64]:
     """Compute the field over the whole mesh from the harmonic/Slepian coefficients."""
     return (
         sleplet.slepian_methods.slepian_mesh_inverse(f.mesh_slepian, coefficients)
         if hasattr(f, "mesh_slepian")
         else sleplet.harmonic_methods.mesh_inverse(f.mesh, coefficients)
     )
 
@@ -252,16 +253,16 @@
         if f._unnoised_coefficients is not None
         else None
     )
 
 
 def _coefficients_to_field_sphere(
     f: sleplet.functions.coefficients.Coefficients,
-    coefficients: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.complex_ | np.float_]:
+    coefficients: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.complex128 | np.float64]:
     """Compute the field over the samples from the harmonic/Slepian coefficients."""
     return (
         sleplet.slepian_methods.slepian_inverse(coefficients, f.L, f.slepian)
         if hasattr(f, "slepian")
         else ssht.inverse(
             coefficients,
             f.L,
```

### Comparing `sleplet-1.4.6/src/sleplet/plotting/_create_plot_mesh.py` & `sleplet-1.4.7/src/sleplet/plotting/_create_plot_mesh.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 class PlotMesh:
     """Create surface mesh plot via `plotly`."""
 
     mesh: sleplet.meshes.mesh.Mesh
     """The given mesh object."""
     filename: str
     """The output filename of the plot."""
-    f: npt.NDArray[np.complex_ | np.float_]
+    f: npt.NDArray[np.complex128 | np.float64]
     """The field value sampled on the mesh."""
     _: dataclasses.KW_ONLY
     amplitude: float | None = None
     """Whether to customise the amplitude range of the colour bar."""
     normalise: bool = True
     """Whether to normalise the plot or not."""
     region: bool = False
@@ -102,29 +102,29 @@
 
         msg = f"Opening: {self.filename}"
         _logger.info(msg)
         pio.show(fig, config={"toImageButtonOptions": {"filename": self.filename}})
 
     def _prepare_field(
         self: typing_extensions.Self,
-        f: npt.NDArray[np.complex_ | np.float_],
-    ) -> npt.NDArray[np.float_]:
+        f: npt.NDArray[np.complex128 | np.float64],
+    ) -> npt.NDArray[np.float64]:
         """Scales the field before plotting."""
         return sleplet.plot_methods._normalise_function(
             sleplet._mesh_methods.average_functions_on_vertices_to_faces(
                 self.mesh.faces,
                 f,
             ),
             normalise=self.normalise,
         )
 
     def _set_outside_region_to_minimum(
         self: typing_extensions.Self,
-        f: npt.NDArray[np.float_],
-    ) -> npt.NDArray[np.float_]:
+        f: npt.NDArray[np.float64],
+    ) -> npt.NDArray[np.float64]:
         """
         For the Slepian region set the outside area to negative infinity
         hence it is clear we are only interested in the coloured region.
         """
         region_on_faces = sleplet._mask_methods.convert_region_on_vertices_to_faces(
             self.mesh,
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/plotting/_create_plot_sphere.py` & `sleplet-1.4.7/src/sleplet/plotting/_create_plot_sphere.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 _logger = logging.getLogger(__name__)
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class PlotSphere:
     """Create surface sphere plot via `plotly`."""
 
-    f: npt.NDArray[np.complex_ | np.float_]
+    f: npt.NDArray[np.complex128 | np.float64]
     """The field value sampled on the sphere."""
     L: int
     """The spherical harmonic bandlimit."""
     filename: str
     """The output filename of the plot."""
     _: dataclasses.KW_ONLY
     amplitude: float | None = None
@@ -118,27 +118,27 @@
 
         msg = f"Opening: {self.filename}"
         _logger.info(msg)
         pio.show(fig, config={"toImageButtonOptions": {"filename": self.filename}})
 
     @staticmethod
     def _setup_plot(  # noqa: PLR0913
-        f: npt.NDArray[np.float_],
+        f: npt.NDArray[np.float64],
         resolution: int,
         *,
         method: str = "MW",
         close: bool = True,
         parametric: bool = False,
         parametric_scaling: list[float] | None = None,
         color_range: list[float] | None = None,
     ) -> tuple[
-        npt.NDArray[np.float_],
-        npt.NDArray[np.float_],
-        npt.NDArray[np.float_],
-        npt.NDArray[np.float_],
+        npt.NDArray[np.float64],
+        npt.NDArray[np.float64],
+        npt.NDArray[np.float64],
+        npt.NDArray[np.float64],
         float,
         float,
     ]:
         """Create the data for the matplotlib/plotly plot."""
         if parametric_scaling is None:
             parametric_scaling = [0.0, 0.5]
 
@@ -192,16 +192,16 @@
             else ssht.s2_to_cart(thetas, phis)
         )
 
         return x, y, z, f_plot, vmin, vmax
 
     def _prepare_field(
         self: typing_extensions.Self,
-        f: npt.NDArray[np.complex_ | np.float_],
-    ) -> npt.NDArray[np.float_]:
+        f: npt.NDArray[np.complex128 | np.float64],
+    ) -> npt.NDArray[np.float64]:
         """Boosts, forces plot type and then scales the field before plotting."""
         boosted_field = sleplet.plot_methods._boost_field(
             f,
             self.L,
             self._resolution,
             reality=self.reality,
             spin=self.spin,
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/_slepian_decomposition.py` & `sleplet-1.4.7/src/sleplet/slepian/_slepian_decomposition.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class SlepianDecomposition:
     L: int
     slepian: SlepianFunctions
     _: dataclasses.KW_ONLY
-    f: npt.NDArray[np.complex_] | None = None
-    flm: npt.NDArray[np.complex_ | np.float_] | None = None
-    mask: npt.NDArray[np.float_] | None = None
+    f: npt.NDArray[np.complex128] | None = None
+    flm: npt.NDArray[np.complex128 | np.float64] | None = None
+    mask: npt.NDArray[np.float64] | None = None
     _method: str = pydantic.Field(default="", init_var=False, repr=False)
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._detect_method()
 
     def decompose(self: typing_extensions.Self, rank: int) -> complex:
         """Decompose the signal into its Slepian coefficients via the given method."""
@@ -43,17 +43,17 @@
             case _:
                 msg = f"'{self._method}' is not a valid method"
                 raise ValueError(msg)
 
     def decompose_all(
         self: typing_extensions.Self,
         n_coefficients: int,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         """Decompose all ranks of the Slepian coefficients."""
-        coefficients = np.zeros(n_coefficients, dtype=np.complex_)
+        coefficients = np.zeros(n_coefficients, dtype=np.complex128)
         for rank in range(n_coefficients):
             coefficients[rank] = self.decompose(rank)
         return coefficients
 
     def _integrate_region(self: typing_extensions.Self, rank: int) -> complex:
         r"""
         F_{p} =
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/region.py` & `sleplet-1.4.7/src/sleplet/slepian/region.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `Region` class."""
+
 import logging
 
 import pydantic
 import typing_extensions
 
 import sleplet._bool_methods
 import sleplet._string_methods
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/slepian_arbitrary.py` & `sleplet-1.4.7/src/sleplet/slepian/slepian_arbitrary.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianArbitrary` class."""
+
 import concurrent.futures
 import logging
 import os
 
 import numpy as np
 import numpy.linalg as LA  # noqa: N812
 import numpy.typing as npt
@@ -30,15 +31,15 @@
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class SlepianArbitrary(SlepianFunctions):
     """Class to create an arbitrary Slepian region on the sphere."""
 
     mask_name: str
     """The name of the mask of the arbitrary region."""
-    _weight: npt.NDArray[np.float_] = pydantic.Field(
+    _weight: npt.NDArray[np.float64] = pydantic.Field(
         default_factory=lambda: np.empty(0),
         init_var=False,
         repr=False,
     )
 
     def __post_init__(self: typing_extensions.Self) -> None:
         self._resolution = _SAMPLES * self.L
@@ -46,29 +47,29 @@
 
     def _create_fn_name(self: typing_extensions.Self) -> str:
         return f"slepian_{self.mask_name}"
 
     def _create_region(self: typing_extensions.Self) -> "sleplet.slepian.region.Region":
         return sleplet.slepian.region.Region(mask_name=self.mask_name)
 
-    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         return sleplet._mask_methods.create_mask_region(self._resolution, self.region)
 
     def _calculate_area(self: typing_extensions.Self) -> float:
         self._weight = sleplet._integration_methods.calc_integration_weight(
             self._resolution,
         )
         return (self.mask * self._weight).sum()
 
     def _create_matrix_location(self: typing_extensions.Self) -> str:
         return f"slepian_eigensolutions_D_{self.mask_name}_L{self.L}_N{self.N}"
 
     def _solve_eigenproblem(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
 
         try:
             eigenvalues = np.load(
                 sleplet._data.setup_pooch.find_on_pooch_then_local(eval_loc),
             )
@@ -79,15 +80,15 @@
             eigenvalues, eigenvectors = self._solve_D_matrix(eval_loc, evec_loc)
         return eigenvalues, eigenvectors
 
     def _solve_D_matrix(  # noqa: N802
         self: typing_extensions.Self,
         eval_loc: str,
         evec_loc: str,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         D = self._create_D_matrix()
 
         # fill in remaining triangle section
         sleplet._array_methods.fill_upper_triangle_of_hermitian_matrix(D)
 
         # solve eigenproblem
         (
@@ -96,18 +97,18 @@
         ) = sleplet._slepian_arbitrary_methods.clean_evals_and_evecs(LA.eigh(D))
         np.save(platformdirs.user_data_path() / eval_loc, eigenvalues)
         np.save(platformdirs.user_data_path() / evec_loc, eigenvectors[: self.N])
         return eigenvalues, eigenvectors
 
     def _create_D_matrix(  # noqa: N802
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         """Compute the D matrix in parallel."""
         # create dictionary for the integrals
-        self._fields: dict[int, npt.NDArray[np.complex_ | np.float_]] = {}
+        self._fields: dict[int, npt.NDArray[np.complex128 | np.float64]] = {}
 
         # initialise real and imaginary matrices
         D_r = np.zeros((self.L**2, self.L**2))
         D_i = np.zeros((self.L**2, self.L**2))
 
         D_r_ext, shm_r_ext = sleplet._parallel_methods.create_shared_memory_array(D_r)
         D_i_ext, shm_i_ext = sleplet._parallel_methods.create_shared_memory_array(D_i)
@@ -151,16 +152,16 @@
         # Free and release the shared memory block at the very end
         sleplet._parallel_methods.free_shared_memory(shm_r_ext, shm_i_ext)
         sleplet._parallel_methods.release_shared_memory(shm_r_ext, shm_i_ext)
         return D
 
     def _matrix_helper(
         self: typing_extensions.Self,
-        D_r: npt.NDArray[np.float_],
-        D_i: npt.NDArray[np.float_],
+        D_r: npt.NDArray[np.float64],
+        D_i: npt.NDArray[np.float64],
         i: int,
     ) -> None:
         """
         Use in both serial and parallel calculations.
 
         The hack with splitting into real and imaginary parts
         is not required for the serial case but here for ease
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/slepian_functions.py` & `sleplet-1.4.7/src/sleplet/slepian/slepian_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the abstract `SlepianFunctions` class."""
+
 import abc
 import dataclasses
 import logging
 
 import numpy as np
 import numpy.typing as npt
 import pydantic
@@ -16,25 +17,25 @@
 
 @pydantic.dataclasses.dataclass(config=sleplet._validation.validation)
 class SlepianFunctions:
     """Abstract parent class of creating the different Slepian regions on the sphere."""
 
     L: int
     """The spherical harmonic bandlimit."""
-    eigenvalues: npt.NDArray[np.float_] = dataclasses.field(
+    eigenvalues: npt.NDArray[np.float64] = dataclasses.field(
         default_factory=lambda: np.empty(0),
         kw_only=True,
         repr=True,
     )
-    eigenvectors: npt.NDArray[np.complex_] = dataclasses.field(
-        default_factory=lambda: np.empty(0, dtype=np.complex_),
+    eigenvectors: npt.NDArray[np.complex128] = dataclasses.field(
+        default_factory=lambda: np.empty(0, dtype=np.complex128),
         kw_only=True,
         repr=True,
     )
-    mask: npt.NDArray[np.float_] = dataclasses.field(
+    mask: npt.NDArray[np.float64] = dataclasses.field(
         default_factory=lambda: np.empty(0),
         kw_only=True,
         repr=False,
     )
     matrix_location: str = dataclasses.field(default="", kw_only=True, repr=False)
     N: int = dataclasses.field(default=0, kw_only=True, repr=False)
     name: str = dataclasses.field(default="", kw_only=True, repr=False)
@@ -69,15 +70,15 @@
 
     @abc.abstractmethod
     def _create_region(self: typing_extensions.Self) -> "sleplet.slepian.region.Region":
         """Create a region object for area of interest."""
         raise NotImplementedError
 
     @abc.abstractmethod
-    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         """Create a mask of the region of interest."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _calculate_area(self: typing_extensions.Self) -> float:
         """Calculate area of region."""
         raise NotImplementedError
@@ -86,10 +87,10 @@
     def _create_matrix_location(self: typing_extensions.Self) -> str:
         """Create the name of the matrix binary."""
         raise NotImplementedError
 
     @abc.abstractmethod
     def _solve_eigenproblem(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Solve the eigenproblem for the given function."""
         raise NotImplementedError
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/slepian_limit_lat_lon.py` & `sleplet-1.4.7/src/sleplet/slepian/slepian_limit_lat_lon.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,30 +42,30 @@
         return sleplet.slepian.region.Region(
             theta_min=self.theta_min,
             theta_max=self.theta_max,
             phi_min=self.phi_min,
             phi_max=self.phi_max,
         )
 
-    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         return sleplet._mask_methods.create_mask_region(self.L, self.region)
 
     def _calculate_area(self: typing_extensions.Self) -> float:
         return (self.phi_max - self.phi_min) * (
             np.cos(self.theta_min) - np.cos(self.theta_max)
         )
 
     def _create_matrix_location(self: typing_extensions.Self) -> str:
         return (
             f"slepian_eigensolutions_D_{self.region._name_ending}_L{self.L}_N{self.N}"
         )
 
     def _solve_eigenproblem(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
         try:
             eigenvalues = np.load(
                 sleplet._data.setup_pooch.find_on_pooch_then_local(eval_loc),
             )
             eigenvectors = np.load(
@@ -76,27 +76,27 @@
             eigenvalues, eigenvectors = self._clean_evals_and_evecs(LA.eigh(K))
             np.save(platformdirs.user_data_path() / eval_loc, eigenvalues)
             np.save(platformdirs.user_data_path() / evec_loc, eigenvectors[: self.N])
         return eigenvalues, eigenvectors
 
     def _create_K_matrix(  # noqa: N802
         self: typing_extensions.Self,
-    ) -> npt.NDArray[np.complex_]:
+    ) -> npt.NDArray[np.complex128]:
         """Compute the K matrix."""
         # Compute sub-integral matrix
         G = self._slepian_integral()
 
         # Compute Slepian matrix
         dl_array = ssht.generate_dl(np.pi / 2, self.L)
         K = self._slepian_matrix(dl_array, self.L, self.L - 1, G)
         sleplet._array_methods.fill_upper_triangle_of_hermitian_matrix(K)
 
         return K
 
-    def _slepian_integral(self: typing_extensions.Self) -> npt.NDArray[np.complex_]:
+    def _slepian_integral(self: typing_extensions.Self) -> npt.NDArray[np.complex128]:
         """
         Syntax:
         G = _slepian_integral().
 
         Output:
         G  =  Sub-integral matrix (obtained after the use of Wigner-D and
         Wigner-d functions in computing the Slepian integral) for all orders
@@ -105,15 +105,15 @@
         This piece of code computes the sub-integral matrix (obtained after the
         use of Wigner-D and Wigner-d functions in computing the Slepian integral)
         for all orders using the formulation given in "Slepian spatialspectral
         concentration problem on the sphere: Analytical formulation for limited
         colatitude-longitude spatial region" by A. P. Bates, Z. Khalid and R. A.
         Kennedy.
         """
-        G = np.zeros((4 * self.L - 3, 4 * self.L - 3), dtype=np.complex_)
+        G = np.zeros((4 * self.L - 3, 4 * self.L - 3), dtype=np.complex128)
 
         def helper(row: int, col: int, S: float) -> None:
             """Use conjugate symmetry property to reduce the number of iterations."""
             try:
                 Q = (1 / (col**2 - 1)) * (
                     np.exp(1j * col * self.theta_min)
                     * (1j * col * np.sin(self.theta_min) - np.cos(self.theta_min))
@@ -147,19 +147,19 @@
                 helper(row, col, S)
 
         return G
 
     @staticmethod
     @numba.njit(parallel=True, fastmath=True)
     def _slepian_matrix(
-        dl: npt.NDArray[np.float_],
+        dl: npt.NDArray[np.float64],
         L: int,
         N: int,
-        G: npt.NDArray[np.complex_],
-    ) -> npt.NDArray[np.complex_]:
+        G: npt.NDArray[np.complex128],
+    ) -> npt.NDArray[np.complex128]:
         """
         Syntax:
         K = _slepian_matrix(dl, L, N, G).
 
         Input:
         G  =  Sub-integral matrix (obtained after the use of Wigner-D and
         Wigner-d functions in computing the Slepian integral) for all orders
@@ -169,15 +169,15 @@
 
         Description:
         This piece of code computes the Slepian matrix using the formulation
         given in "Slepian spatialspectral concentration problem on the sphere:
         Analytical formulation for limited colatitude-longitude spatial region"
         by A. P. Bates, Z. Khalid and R. A. Kennedy.
         """
-        K = np.zeros((L**2, L**2), dtype=np.complex_)
+        K = np.zeros((L**2, L**2), dtype=np.complex128)
 
         for ell in numba.prange(L):
             for p in range(ell + 1):
                 C1 = np.sqrt((2 * ell + 1) * (2 * p + 1)) / (4 * np.pi)
 
                 for m in range(-ell, ell + 1):
                     ind_lm = ell * (ell + 1) + m
@@ -201,16 +201,18 @@
                             K[ind_lm, ind_pq] += C3 * S1
 
                         K[ind_lm, ind_pq] *= C1 * C2
         return K
 
     @staticmethod
     def _clean_evals_and_evecs(
-        eigendecomposition: tuple[npt.NDArray[np.complex_], npt.NDArray[np.complex_]],
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+        eigendecomposition: tuple[
+            npt.NDArray[np.complex128], npt.NDArray[np.complex128]
+        ],
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Need eigenvalues and eigenvectors to be in a certain format."""
         # access values
         eigenvalues_complex, eigenvectors = eigendecomposition
 
         # eigenvalues should be real
         eigenvalues = eigenvalues_complex.real
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian/slepian_polar_cap.py` & `sleplet-1.4.7/src/sleplet/slepian/slepian_polar_cap.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains the `SlepianPolarCap` class."""
+
 import concurrent.futures
 import dataclasses
 import logging
 import os
 
 import gmpy2 as gp
 import numpy as np
@@ -48,28 +49,28 @@
 
     def _create_fn_name(self: typing_extensions.Self) -> str:
         return f"slepian_{self.region._name_ending}"
 
     def _create_region(self: typing_extensions.Self) -> "sleplet.slepian.region.Region":
         return sleplet.slepian.region.Region(gap=self.gap, theta_max=self.theta_max)
 
-    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float_]:
+    def _create_mask(self: typing_extensions.Self) -> npt.NDArray[np.float64]:
         return sleplet._mask_methods.create_mask_region(self.L, self.region)
 
     def _calculate_area(self: typing_extensions.Self) -> float:
         return 2 * np.pi * (1 - np.cos(self.theta_max))
 
     def _create_matrix_location(self: typing_extensions.Self) -> str:
         return (
             f"slepian_eigensolutions_D_{self.region._name_ending}_L{self.L}_N{self.N}"
         )
 
     def _solve_eigenproblem(
         self: typing_extensions.Self,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         eval_loc = f"{self.matrix_location}_eigenvalues.npy"
         evec_loc = f"{self.matrix_location}_eigenvectors.npy"
         order_loc = f"{self.matrix_location}_orders.npy"
         try:
             eigenvalues, eigenvectors = self._solve_eigenproblem_from_files(
                 eval_loc,
                 evec_loc,
@@ -84,15 +85,15 @@
         return eigenvalues, eigenvectors
 
     def _solve_eigenproblem_from_files(
         self: typing_extensions.Self,
         eval_loc: str,
         evec_loc: str,
         order_loc: str,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Solve eigenproblem with files already saved."""
         eigenvalues = np.load(
             sleplet._data.setup_pooch.find_on_pooch_then_local(eval_loc),
         )
         eigenvectors = np.load(
             sleplet._data.setup_pooch.find_on_pooch_then_local(evec_loc),
         )
@@ -105,21 +106,21 @@
         return eigenvalues, eigenvectors
 
     def _solve_eigenproblem_from_scratch(
         self: typing_extensions.Self,
         eval_loc: str,
         evec_loc: str,
         order_loc: str,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Solve eigenproblem from scratch and then saves the files."""
         if isinstance(self.order, int):
             return self._solve_eigenproblem_order(self.order)
 
         evals_all = np.empty(0)
-        evecs_all = np.empty((0, self.L**2), dtype=np.complex_)
+        evecs_all = np.empty((0, self.L**2), dtype=np.complex128)
         emm = np.empty(0, dtype=int)
         for m in range(-(self.L - 1), self.L):
             evals_m, evecs_m = self._solve_eigenproblem_order(m)
             evals_all = np.append(evals_all, evals_m)
             evecs_all = np.concatenate((evecs_all, evecs_m))
             emm = np.append(emm, [m] * len(evals_m))
         (
@@ -132,40 +133,42 @@
         np.save(platformdirs.user_data_path() / evec_loc, eigenvectors[:limit])
         np.save(platformdirs.user_data_path() / order_loc, self.order)
         return eigenvalues, eigenvectors
 
     def _solve_eigenproblem_order(
         self: typing_extensions.Self,
         m: int,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Solve the eigenproblem for a given order m."""
         emm = sleplet.harmonic_methods._create_emm_vector(self.L)
         Dm = self._create_Dm_matrix(abs(m), emm)
         eigenvalues, gl = LA.eigh(Dm)
         eigenvalues, eigenvectors = self._clean_evals_and_evecs(eigenvalues, gl, emm, m)
         return eigenvalues, eigenvectors
 
     def _sort_all_evals_and_evecs(
         self: typing_extensions.Self,
-        eigenvalues: npt.NDArray[np.float_],
-        eigenvectors: npt.NDArray[np.complex_],
+        eigenvalues: npt.NDArray[np.float64],
+        eigenvectors: npt.NDArray[np.complex128],
         orders: npt.NDArray[np.int_],
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_], npt.NDArray[np.int_]]:
+    ) -> tuple[
+        npt.NDArray[np.float64], npt.NDArray[np.complex128], npt.NDArray[np.int_]
+    ]:
         """Sort all eigenvalues and eigenvectors for all orders."""
         idx = eigenvalues.argsort()[::-1]
         eigenvalues = eigenvalues[idx]
         eigenvectors = eigenvectors[idx]
         orders = orders[idx]
         return eigenvalues, eigenvectors, orders
 
     def _create_Dm_matrix(  # noqa: N802
         self: typing_extensions.Self,
         m: int,
-        emm: npt.NDArray[np.float_],
-    ) -> npt.NDArray[np.float_]:
+        emm: npt.NDArray[np.float64],
+    ) -> npt.NDArray[np.float64]:
         """
         Syntax:
         Dm = _create_Dm_matrix(m, P).
 
         Input:
         m  =  order
         P(:,1)  =  Pl = Legendre Polynomials column vector for l = 0 : L-1
@@ -221,30 +224,30 @@
         # Free and release the shared memory block at the very end
         sleplet._parallel_methods.free_shared_memory(shm_ext)
         sleplet._parallel_methods.release_shared_memory(shm_ext)
         return Dm
 
     def _create_legendre_polynomials_table(
         self: typing_extensions.Self,
-        emm: npt.NDArray[np.float_],
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.int_]]:
+        emm: npt.NDArray[np.float64],
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.int_]]:
         """Create Legendre polynomials table for matrix calculation."""
         Plm = ssht.create_ylm(self.theta_max, 0, 2 * self.L).real.reshape(-1)
         ind = emm == 0
         ell = np.arange(2 * self.L)[np.newaxis]
         Pl = np.sqrt((4 * np.pi) / (2 * ell + 1)) * Plm[ind]
         return Pl, ell
 
     def _dm_matrix_helper(  # noqa: PLR0913
         self: typing_extensions.Self,
-        Dm: npt.NDArray[np.float_],
+        Dm: npt.NDArray[np.float64],
         i: int,
         m: int,
         lvec: npt.NDArray[np.int_],
-        Pl: npt.NDArray[np.float_],
+        Pl: npt.NDArray[np.float64],
         ell: npt.NDArray[np.int_],
     ) -> None:
         """Use in both serial and parallel calculations."""
         el = int(lvec[i])
         for j in range(i, self.L - m):
             p = int(lvec[j])
             c = 0
@@ -364,29 +367,29 @@
         Eq 67 - Spherical Slepian functions and the polar gap in geodesy
         multiply by 1 + (-1)*(ell+ell').
         """
         return 1 + self.gap * (-1) ** (ell1 + ell2)
 
     def _clean_evals_and_evecs(
         self: typing_extensions.Self,
-        eigenvalues: npt.NDArray[np.float_],
-        gl: npt.NDArray[np.float_],
-        emm: npt.NDArray[np.float_],
+        eigenvalues: npt.NDArray[np.float64],
+        gl: npt.NDArray[np.float64],
+        emm: npt.NDArray[np.float64],
         m: int,
-    ) -> tuple[npt.NDArray[np.float_], npt.NDArray[np.complex_]]:
+    ) -> tuple[npt.NDArray[np.float64], npt.NDArray[np.complex128]]:
         """Need eigenvalues and eigenvectors to be in a certain format."""
         # Sort eigenvalues and eigenvectors in descending order of eigenvalues
         idx = eigenvalues.argsort()[::-1]
         eigenvalues = eigenvalues[idx]
         gl = gl[:, idx].conj()
 
         # put back in full D space for harmonic transform
         emm = emm[: self.L**2]
         ind = np.tile(emm == m, (self.L - abs(m), 1))
-        eigenvectors = np.zeros((self.L - abs(m), self.L**2), dtype=np.complex_)
+        eigenvectors = np.zeros((self.L - abs(m), self.L**2), dtype=np.complex128)
         eigenvectors[ind] = gl.T.flatten()
 
         # ensure first element of each eigenvector is positive
         eigenvectors *= np.where(eigenvectors[:, 0] < 0, -1, 1)[:, np.newaxis]
 
         # if -ve 'm' find orthogonal eigenvectors to +ve 'm' eigenvectors
         if m < 0:
```

### Comparing `sleplet-1.4.6/src/sleplet/slepian_methods.py` & `sleplet-1.4.7/src/sleplet/slepian_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Methods to work with Slepian coefficients."""
+
 import logging
 
 import numpy as np
 import numpy.typing as npt
 
 import pyssht as ssht
 
@@ -65,18 +66,18 @@
 
         case _:
             msg = f"{region._region_type} is an invalid region type"
             raise ValueError(msg)
 
 
 def slepian_inverse(
-    f_p: npt.NDArray[np.complex_ | np.float_],
+    f_p: npt.NDArray[np.complex128 | np.float64],
     L: int,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Compute the Slepian inverse transform up to the Shannon number.
 
     Args:
         f_p: The Slepian coefficients.
         L: The spherical harmonic bandlimit.
         slepian: The given Slepian object.
@@ -89,19 +90,19 @@
     return (f_p_reshape * s_p).sum(axis=0)
 
 
 def slepian_forward(  # noqa: PLR0913
     L: int,
     slepian: SlepianFunctions,
     *,
-    f: npt.NDArray[np.complex_] | None = None,
-    flm: npt.NDArray[np.complex_ | np.float_] | None = None,
-    mask: npt.NDArray[np.float_] | None = None,
+    f: npt.NDArray[np.complex128] | None = None,
+    flm: npt.NDArray[np.complex128 | np.float64] | None = None,
+    mask: npt.NDArray[np.float64] | None = None,
     n_coeffs: int | None = None,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """
     Compute the Slepian forward transform for all coefficients.
 
     Args:
         L: The spherical harmonic bandlimit.
         slepian: The given Slepian object.
         f: The field value.
@@ -122,27 +123,27 @@
     n_coeffs = slepian.N if n_coeffs is None else n_coeffs
     return sd.decompose_all(n_coeffs)
 
 
 def compute_s_p_omega(
     L: int,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     r"""
     Compute \(S_{p}(\omega)\) for a given region.
 
     Args:
         L: The spherical harmonic bandlimit.
         slepian: The given Slepian object.
 
     Returns:
         The complex \(S_{p}(\omega)\) values.
     """
     n_theta, n_phi = ssht.sample_shape(L, Method=sleplet._vars.SAMPLING_SCHEME)
-    sp = np.zeros((slepian.N, n_theta, n_phi), dtype=np.complex_)
+    sp = np.zeros((slepian.N, n_theta, n_phi), dtype=np.complex128)
     for p in range(slepian.N):
         if p % L == 0:
             msg = f"compute Sp(omega) p={p+1}/{slepian.N}"
             _logger.info(msg)
         sp[p] = ssht.inverse(
             slepian.eigenvectors[p],
             L,
@@ -152,33 +153,33 @@
 
 
 def _compute_s_p_omega_prime(
     L: int,
     alpha: float,
     beta: float,
     slepian: SlepianFunctions,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Pick out the desired angle from Sp(omega)."""
     sp_omega = compute_s_p_omega(L, slepian)
     p = ssht.theta_to_index(beta, L, Method=sleplet._vars.SAMPLING_SCHEME)
     q = ssht.phi_to_index(alpha, L, Method=sleplet._vars.SAMPLING_SCHEME)
     sp_omega_prime = sp_omega[:, p, q]
     # pad with zeros so it has the expected shape
     boost = L**2 - slepian.N
     return sleplet.harmonic_methods._boost_coefficient_resolution(sp_omega_prime, boost)
 
 
 def slepian_mesh_forward(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
     *,
-    u: npt.NDArray[np.complex_ | np.float_] | None = None,
-    u_i: npt.NDArray[np.complex_ | np.float_] | None = None,
+    u: npt.NDArray[np.complex128 | np.float64] | None = None,
+    u_i: npt.NDArray[np.complex128 | np.float64] | None = None,
     mask: bool = False,
     n_coeffs: int | None = None,
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """
     Compute the Slepian forward transform for all coefficients on the mesh.
 
     Args:
         mesh_slepian: The Slepian mesh object containing the eigensolutions.
         u: The signal field value on the mesh.
         u_i: The Fourier coefficients of the mesh.
@@ -196,16 +197,16 @@
     )
     n_coeffs = mesh_slepian.N if n_coeffs is None else n_coeffs
     return sd.decompose_all(n_coeffs)
 
 
 def slepian_mesh_inverse(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
-    f_p: npt.NDArray[np.complex_ | np.float_],
-) -> npt.NDArray[np.complex_ | np.float_]:
+    f_p: npt.NDArray[np.complex128 | np.float64],
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Compute the Slepian inverse transform on the mesh up to the Shannon number.
 
     Args:
         mesh_slepian: The Slepian mesh object containing the eigensolutions.
         f_p: The Slepian wavelet coefficients.
 
@@ -215,15 +216,15 @@
     f_p_reshape = f_p[: mesh_slepian.N, np.newaxis]
     s_p = _compute_mesh_s_p_pixel(mesh_slepian)
     return (f_p_reshape * s_p).sum(axis=0)
 
 
 def _compute_mesh_s_p_pixel(
     mesh_slepian: "sleplet.meshes.mesh_slepian.MeshSlepian",
-) -> npt.NDArray[np.float_]:
+) -> npt.NDArray[np.float64]:
     """Calculate Sp(omega) for a given region."""
     sp = np.zeros((mesh_slepian.N, mesh_slepian.mesh.vertices.shape[0]))
     for p in range(mesh_slepian.N):
         sp[p] = sleplet.harmonic_methods.mesh_inverse(
             mesh_slepian.mesh,
             mesh_slepian.slepian_functions[p],
         )
```

### Comparing `sleplet-1.4.6/src/sleplet/wavelet_methods.py` & `sleplet-1.4.7/src/sleplet/wavelet_methods.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Methods to work with wavelet and wavelet coefficients."""
+
 import numpy as np
 import numpy.typing as npt
 
 import pys2let
 import pyssht as ssht
 
 import sleplet._convolution_methods
 import sleplet.slepian_methods
 
 
 def slepian_wavelet_forward(
-    f_p: npt.NDArray[np.complex_ | np.float_],
-    wavelets: npt.NDArray[np.float_],
+    f_p: npt.NDArray[np.complex128 | np.float64],
+    wavelets: npt.NDArray[np.float64],
     shannon: int,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Compute the coefficients of the given tiling function in Slepian space.
 
     Args:
         f_p: The Slepian coefficients.
         wavelets: The Slepian wavelets.
         shannon: The Shannon number.
@@ -32,18 +33,18 @@
             shannon=shannon,
         ),
         axis=1,
     )
 
 
 def slepian_wavelet_inverse(
-    wav_coeffs: npt.NDArray[np.complex_ | np.float_],
-    wavelets: npt.NDArray[np.float_],
+    wav_coeffs: npt.NDArray[np.complex128 | np.float64],
+    wavelets: npt.NDArray[np.float64],
     shannon: int,
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Compute the inverse wavelet transform in Slepian space.
 
     Args:
         wav_coeffs: The Slepian wavelet coefficients.
         wavelets: The Slepian wavelets.
         shannon: The Shannon number.
@@ -59,80 +60,80 @@
         shannon=shannon,
     )
     return wavelet_reconstruction.sum(axis=0)
 
 
 def axisymmetric_wavelet_forward(
     L: int,
-    flm: npt.NDArray[np.complex_ | np.float_],
-    wavelets: npt.NDArray[np.complex_],
-) -> npt.NDArray[np.complex_]:
+    flm: npt.NDArray[np.complex128 | np.float64],
+    wavelets: npt.NDArray[np.complex128],
+) -> npt.NDArray[np.complex128]:
     """
     Compute the coefficients of the axisymmetric wavelets.
 
     Args:
         L: The spherical harmonic bandlimit.
         flm: The spherical harmonic coefficients.
         wavelets: Axisymmetric wavelets.
 
     Returns:
         Axisymmetric wavelets coefficients.
     """
-    w = np.zeros(wavelets.shape, dtype=np.complex_)
+    w = np.zeros(wavelets.shape, dtype=np.complex128)
     for ell in range(L):
         ind_m0 = ssht.elm2ind(ell, 0)
         wav_0 = np.sqrt((4 * np.pi) / (2 * ell + 1)) * wavelets[:, ind_m0].conj()
         for m in range(-ell, ell + 1):
             ind = ssht.elm2ind(ell, m)
             w[:, ind] = wav_0 * flm[ind]
     return w
 
 
 def axisymmetric_wavelet_inverse(
     L: int,
-    wav_coeffs: npt.NDArray[np.complex_],
-    wavelets: npt.NDArray[np.complex_],
-) -> npt.NDArray[np.complex_]:
+    wav_coeffs: npt.NDArray[np.complex128],
+    wavelets: npt.NDArray[np.complex128],
+) -> npt.NDArray[np.complex128]:
     """
     Compute the inverse axisymmetric wavelet transform.
 
     Args:
         L: The spherical harmonic bandlimit.
         wav_coeffs: Axisymmetric wavelet coefficients.
         wavelets: Axisymmetric wavelets.
 
     Returns:
         Spherical harmonic coefficients of the signal.
     """
-    flm = np.zeros(L**2, dtype=np.complex_)
+    flm = np.zeros(L**2, dtype=np.complex128)
     for ell in range(L):
         ind_m0 = ssht.elm2ind(ell, 0)
         wav_0 = np.sqrt((4 * np.pi) / (2 * ell + 1)) * wavelets[:, ind_m0]
         for m in range(-ell, ell + 1):
             ind = ssht.elm2ind(ell, m)
             flm[ind] = (wav_coeffs[:, ind] * wav_0).sum()
     return flm
 
 
 def _create_axisymmetric_wavelets(
     L: int,
     B: int,
     j_min: int,
-) -> npt.NDArray[np.complex_]:
+) -> npt.NDArray[np.complex128]:
     """Compute the axisymmetric wavelets."""
     kappas = create_kappas(L, B, j_min)
-    wavelets = np.zeros((kappas.shape[0], L**2), dtype=np.complex_)
+    wavelets = np.zeros((kappas.shape[0], L**2), dtype=np.complex128)
     for ell in range(L):
         factor = np.sqrt((2 * ell + 1) / (4 * np.pi))
         ind = ssht.elm2ind(ell, 0)
         wavelets[:, ind] = factor * kappas[:, ell]
     return wavelets
 
 
-def create_kappas(xlim: int, B: int, j_min: int) -> npt.NDArray[np.float_]:
+def create_kappas(xlim: int, B: int, j_min: int) -> npt.NDArray[np.float64]:
     r"""
     Compute the Slepian wavelets.
 
     Args:
         xlim: The x-axis value. \(L\) or \(L^2\) in the harmonic or Slepian case.
         B: The wavelet parameter. Represented as \(\lambda\) in the papers.
         j_min: The minimum wavelet scale. Represented as \(J_{0}\) in the papers.
@@ -141,18 +142,18 @@
         The Slepian wavelet generating functions.
     """
     kappa0, kappa = pys2let.axisym_wav_l(B, xlim, j_min)
     return np.concatenate((kappa0[np.newaxis], kappa.T))
 
 
 def find_non_zero_wavelet_coefficients(
-    wav_coeffs: npt.NDArray[np.complex_ | np.float_],
+    wav_coeffs: npt.NDArray[np.complex128 | np.float64],
     *,
     axis: int | tuple[int, ...],
-) -> npt.NDArray[np.complex_ | np.float_]:
+) -> npt.NDArray[np.complex128 | np.float64]:
     """
     Find the coefficients within the shannon number to speed up computations.
 
     Args:
         wav_coeffs: The wavelet coefficients.
         axis: The axis to search over.
```

### Comparing `sleplet-1.4.6/src/sleplet.egg-info/PKG-INFO` & `sleplet-1.4.7/src/sleplet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: sleplet
-Version: 1.4.6
+Version: 1.4.7
 Summary: Slepian Scale-Discretised Wavelets in Python
 Author-email: "Patrick J. Roddy" <patrickjamesroddy@gmail.com>
 License: BSD 3-Clause Licence
         
-        Copyright (c) 2017-2023, Patrick Roddy
+        Copyright (c) 2017-2024, Patrick Roddy
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
         
         1. Redistributions of source code must retain the above copyright notice, this
            list of conditions and the following disclaimer.
@@ -74,14 +74,15 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: tox; extra == "dev"
+Requires-Dist: tox-uv; extra == "dev"
 Requires-Dist: tuna; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: pdoc3; extra == "docs"
 Provides-Extra: readme
 Requires-Dist: pytest-codeblocks; extra == "readme"
 
@@ -89,18 +90,19 @@
 
 [![PyPI](https://badge.fury.io/py/sleplet.svg)](https://pypi.org/project/sleplet)
 [![Python](https://img.shields.io/pypi/pyversions/sleplet)](https://www.python.org)
 [![Licence](https://img.shields.io/github/license/astro-informatics/sleplet)](https://github.com/astro-informatics/sleplet/blob/main/LICENCE.txt)
 [![JOSS](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2/status.svg)](https://joss.theoj.org/papers/55d9cf16a27bf2d3141f0f66c676b7f2)
 [![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7268074.svg)](https://doi.org/10.5281/zenodo.7268074)
 [![Documentation](https://img.shields.io/badge/Documentation-SLEPLET-blueviolet.svg)](https://astro-informatics.github.io/sleplet)
-[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yml)
+[![Test](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml/badge.svg)](https://github.com/astro-informatics/sleplet/actions/workflows/test.yaml)
 [![Coverage Status](https://coveralls.io/repos/github/astro-informatics/sleplet/badge.svg?branch=main)](https://coveralls.io/github/astro-informatics/sleplet?branch=main)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![Renovate](https://img.shields.io/badge/renovate-enabled-orange?logo=renovatebot)](https://renovatebot.com)
+[![repostatus](http://www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/#active)
 
 `SLEPLET` is a Python package for the construction of Slepian wavelets in the
 spherical and manifold (via meshes) settings. The API of `SLEPLET` has been
 designed in an object-orientated manner and is easily extendible. Upon
 installation, `SLEPLET` comes with two command line interfaces - `sphere` and
 `mesh` - which allows one to easily generate plots on the sphere and a set of
 meshes using `plotly`.
```

### Comparing `sleplet-1.4.6/src/sleplet.egg-info/SOURCES.txt` & `sleplet-1.4.7/src/sleplet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

