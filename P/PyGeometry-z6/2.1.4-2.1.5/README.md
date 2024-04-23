# Comparing `tmp/PyGeometry-z6-2.1.4.tar.gz` & `tmp/PyGeometry-z6-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGeometry-z6-2.1.4.tar", last modified: Mon Nov  1 11:48:19 2021, max compression
+gzip compressed data, was "PyGeometry-z6-2.1.5.tar", last modified: Tue Apr 23 20:58:12 2024, max compression
```

## Comparing `PyGeometry-z6-2.1.4.tar` & `PyGeometry-z6-2.1.5.tar`

### file list

```diff
@@ -1,99 +1,198 @@
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.652963 PyGeometry-z6-2.1.4/
--rw-r--r--   0 andrea     (501) admin       (80)       96 2021-11-01 00:27:17.000000 PyGeometry-z6-2.1.4/.bumpversion.cfg
--rw-r--r--   0 andrea     (501) admin       (80)     2021 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/.compmake_history.txt
--rw-r--r--   0 andrea     (501) admin       (80)      348 2021-11-01 11:48:19.653152 PyGeometry-z6-2.1.4/PKG-INFO
--rw-r--r--   0 andrea     (501) admin       (80)      540 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/README.md
--rw-r--r--   0 andrea     (501) admin       (80)     1200 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/pypackage.mk
--rw-r--r--   0 andrea     (501) admin       (80)      143 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/requirements.txt
--rw-r--r--   0 andrea     (501) admin       (80)      153 2021-11-01 11:48:19.653790 PyGeometry-z6-2.1.4/setup.cfg
--rw-r--r--   0 andrea     (501) admin       (80)      650 2021-10-31 23:49:00.000000 PyGeometry-z6-2.1.4/setup.json
--rw-r--r--   0 andrea     (501) admin       (80)     1210 2021-10-31 23:18:01.000000 PyGeometry-z6-2.1.4/setup.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.570522 PyGeometry-z6-2.1.4/src/
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.581061 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/
--rw-r--r--   0 andrea     (501) admin       (80)      348 2021-11-01 11:48:19.000000 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/PKG-INFO
--rw-r--r--   0 andrea     (501) admin       (80)     3186 2021-11-01 11:48:19.000000 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/SOURCES.txt
--rw-r--r--   0 andrea     (501) admin       (80)        1 2021-11-01 11:48:19.000000 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/dependency_links.txt
--rw-r--r--   0 andrea     (501) admin       (80)       42 2021-11-01 11:48:19.000000 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/requires.txt
--rw-r--r--   0 andrea     (501) admin       (80)        9 2021-11-01 11:48:19.000000 PyGeometry-z6-2.1.4/src/PyGeometry_z6.egg-info/top_level.txt
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.590513 PyGeometry-z6-2.1.4/src/geometry/
--rw-r--r--   0 andrea     (501) admin       (80)     1777 2021-11-01 00:27:17.000000 PyGeometry-z6-2.1.4/src/geometry/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)     2049 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/basic_utils.py
--rw-r--r--   0 andrea     (501) admin       (80)      145 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/constants.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.591930 PyGeometry-z6-2.1.4/src/geometry/distances/
--rw-r--r--   0 andrea     (501) admin       (80)      112 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/distances/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)      310 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/distances/generic.py
--rw-r--r--   0 andrea     (501) admin       (80)     1731 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/distances/spherical.py
--rw-r--r--   0 andrea     (501) admin       (80)     2662 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/formatting.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.637418 PyGeometry-z6-2.1.4/src/geometry/manifolds/
--rw-r--r--   0 andrea     (501) admin       (80)     1262 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)    10220 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/differentiable_manifold.py
--rw-r--r--   0 andrea     (501) admin       (80)     4184 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/embedding_relations.py
--rw-r--r--   0 andrea     (501) admin       (80)     1448 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/euclidean.py
--rw-r--r--   0 andrea     (501) admin       (80)      748 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/exceptions.py
--rw-r--r--   0 andrea     (501) admin       (80)      529 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/group.py
--rw-r--r--   0 andrea     (501) admin       (80)     4821 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/manifold_embedding_propagation.py
--rw-r--r--   0 andrea     (501) admin       (80)     4347 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/manifold_relations.py
--rw-r--r--   0 andrea     (501) admin       (80)     1470 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_algebra.py
--rw-r--r--   0 andrea     (501) admin       (80)     5362 2021-07-23 13:37:21.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_group.py
--rw-r--r--   0 andrea     (501) admin       (80)     2187 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_group_tangent.py
--rw-r--r--   0 andrea     (501) admin       (80)     2019 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_linear_space.py
--rw-r--r--   0 andrea     (501) admin       (80)     1655 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/point_set.py
--rw-r--r--   0 andrea     (501) admin       (80)     1645 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/product_manifold.py
--rw-r--r--   0 andrea     (501) admin       (80)     3597 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/special_euclidean_algebra.py
--rw-r--r--   0 andrea     (501) admin       (80)     4289 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/special_euclidean_group.py
--rw-r--r--   0 andrea     (501) admin       (80)     2087 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/special_orthogonal_algebra.py
--rw-r--r--   0 andrea     (501) admin       (80)     2887 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/special_orthogonal_group.py
--rw-r--r--   0 andrea     (501) admin       (80)     6011 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/sphere.py
--rw-r--r--   0 andrea     (501) admin       (80)     1664 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/square.py
--rw-r--r--   0 andrea     (501) admin       (80)     1732 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tangent_bundle.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.640880 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/
--rw-r--r--   0 andrea     (501) admin       (80)     3406 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)     3181 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/checks_generation.py
--rw-r--r--   0 andrea     (501) admin       (80)     2031 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/embedding_test.py
--rw-r--r--   0 andrea     (501) admin       (80)     4648 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/manifold_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)     1222 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/matrix_groups_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)      225 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/pickling_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)      399 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/sphere_tests.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.643887 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/
--rw-r--r--   0 andrea     (501) admin       (80)       86 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)     1316 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/grassman.py
--rw-r--r--   0 andrea     (501) admin       (80)      657 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/moebius.py
--rw-r--r--   0 andrea     (501) admin       (80)       15 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/orthogonal_group.py
--rw-r--r--   0 andrea     (501) admin       (80)       15 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/posdef_matrices.py
--rw-r--r--   0 andrea     (501) admin       (80)      941 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/stiefel.py
--rw-r--r--   0 andrea     (501) admin       (80)     1507 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/torus.py
--rw-r--r--   0 andrea     (501) admin       (80)     3401 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/torus01.py
--rw-r--r--   0 andrea     (501) admin       (80)     1400 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/translation_algebra.py
--rw-r--r--   0 andrea     (501) admin       (80)     2258 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/manifolds/translation_group.py
--rw-r--r--   0 andrea     (501) admin       (80)     5655 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/mds_algos.py
--rw-r--r--   0 andrea     (501) admin       (80)    12782 2021-07-23 13:26:06.000000 PyGeometry-z6-2.1.4/src/geometry/poses.py
--rw-r--r--   0 andrea     (501) admin       (80)     2625 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/poses_embedding.py
--rw-r--r--   0 andrea     (501) admin       (80)     1404 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/procrustes.py
--rw-r--r--   0 andrea     (501) admin       (80)    12885 2021-07-23 13:26:06.000000 PyGeometry-z6-2.1.4/src/geometry/rotations.py
--rw-r--r--   0 andrea     (501) admin       (80)      969 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/rotations_embedding.py
--rw-r--r--   0 andrea     (501) admin       (80)    10681 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/spheres.py
--rw-r--r--   0 andrea     (501) admin       (80)      847 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/spheres_embedding.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.644896 PyGeometry-z6-2.1.4/src/geometry/subspaces/
--rw-r--r--   0 andrea     (501) admin       (80)       40 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/subspaces/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)      924 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/subspaces/subspaces.py
--rw-r--r--   0 andrea     (501) admin       (80)      226 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/tex.py
--rw-r--r--   0 andrea     (501) admin       (80)     1650 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/types.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.651559 PyGeometry-z6-2.1.4/src/geometry/unittests/
--rw-r--r--   0 andrea     (501) admin       (80)       15 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)       15 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/distances_test.py
--rw-r--r--   0 andrea     (501) admin       (80)     2443 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/mds_test.py
--rw-r--r--   0 andrea     (501) admin       (80)      234 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/misc_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)     3438 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/poses_test.py
--rw-r--r--   0 andrea     (501) admin       (80)     1370 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/procrustes_test.py
--rw-r--r--   0 andrea     (501) admin       (80)     1654 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/quaternions_test.py
--rw-r--r--   0 andrea     (501) admin       (80)     2008 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/random_geometry_density_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)     4778 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/random_geometry_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)     2192 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/rotations_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)       15 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/spheres_tests.py
--rw-r--r--   0 andrea     (501) admin       (80)      757 2021-06-19 20:08:41.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/uniform_dist_pvalue_paranoia.py
--rw-r--r--   0 andrea     (501) admin       (80)     2027 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/utils.py
--rw-r--r--   0 andrea     (501) admin       (80)      497 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/unittests/utils_test.py
-drwxr-xr-x   0 andrea     (501) admin       (80)        0 2021-11-01 11:48:19.652524 PyGeometry-z6-2.1.4/src/geometry/utils/
--rw-r--r--   0 andrea     (501) admin       (80)       45 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/utils/__init__.py
--rw-r--r--   0 andrea     (501) admin       (80)     1042 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/utils/numpy_backport.py
--rw-r--r--   0 andrea     (501) admin       (80)     3493 2021-06-19 20:08:36.000000 PyGeometry-z6-2.1.4/src/geometry/yaml_.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.268186 PyGeometry-z6-2.1.5/
+-rw-r--r--   0 andreacensi   (501) staff       (20)       96 2024-04-23 20:53:30.000000 PyGeometry-z6-2.1.5/.bumpversion.cfg
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2021 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/.compmake_history.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)      348 2024-04-23 20:58:12.268285 PyGeometry-z6-2.1.5/PKG-INFO
+-rw-r--r--   0 andreacensi   (501) staff       (20)      540 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/README.md
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.237599 PyGeometry-z6-2.1.5/docs/
+-rw-r--r--   0 andreacensi   (501) staff       (20)        8 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/.gitignore
+-rw-r--r--   0 andreacensi   (501) staff       (20)       87 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/Makefile
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1493 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/docs.mk
+-rw-r--r--   0 andreacensi   (501) staff       (20)      328 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/epydoc.cfg
+-rwxr-xr-x   0 andreacensi   (501) staff       (20)       66 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/gitadd.zsh
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.238899 PyGeometry-z6-2.1.5/docs/source/
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.251155 PyGeometry-z6-2.1.5/docs/source/api/
+-rw-r--r--   0 andreacensi   (501) staff       (20)      145 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.basic_utils.assert_allclose.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      118 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.basic_utils.finite.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      148 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.basic_utils.normalize_length.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.basic_utils.normalize_length_or_zero.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      133 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.basic_utils.safe_arccos.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      550 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.distances.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      100 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.S1.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      100 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.S2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      103 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.SE2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      103 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.SE3.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      103 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.SO2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      103 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.SO3.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      210 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.base.DifferentiableManifold.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      159 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.base.Group.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      186 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.euclidean.Euclidean.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      228 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.matrix_lie_group.MatrixLieAlgebra.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      222 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.matrix_lie_group.MatrixLieGroup.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      199 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.moebius.Moebius.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     5095 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      291 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.special_euclidean.SE.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      302 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.special_orthogonal.SO.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      195 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.sphere.Sphere.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1508 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.tests.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1202 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.todo.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      192 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.manifolds.torus.Torus.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      170 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.SE2_from_translation_angle.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      138 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.SE2_from_xytheta.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      124 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.combine_pieces.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      124 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.extract_pieces.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      161 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.linear_angular_from_se2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.pose_from_rotation_translation.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.rotation_translation_from_pose.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      161 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.se2_from_linear_angular.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      170 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.poses.translation_angle_from_SE2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.procrustes.best_orthogonal_transform.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.procrustes.closest_orthogonal_matrix.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.axis_angle_from_quaternion.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      166 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.axis_angle_from_rotation.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      197 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.geodesic_distance_for_rotations.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      115 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.hat_map.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      115 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.map_hat.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      124 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.orthogonal.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      172 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.quaternion_from_axis_angle.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      166 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.quaternion_from_rotation.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      175 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.random_orthogonal_transform.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      145 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.random_quaternion.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      139 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.random_rotation.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      166 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.rotation_from_axis_angle.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      169 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.rotation_from_axis_angle2.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      166 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.rotation_from_quaternion.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      139 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.rotation_matrix.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      136 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rotations.skew_symmetric.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2266 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      151 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.any_distant_direction.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      160 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.any_orthogonal_direction.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      139 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.assert_orthogonal.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      118 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.directions.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      130 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.distances_from.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      145 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.distribution_radius.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      169 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.geodesic_distance_on_sphere.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      136 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.random_direction.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      139 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.random_directions.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      163 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.random_directions_bounded.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      169 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.random_orthogonal_direction.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      139 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.sorted_directions.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      121 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.spheres.unit_length.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      380 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.subspaces.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2757 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.unittests.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)      373 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/geometry.utils.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)       51 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api/modules.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     6250 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/api_summary.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)     7915 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/conf.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      322 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/definitions.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)      750 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/download.html
+-rw-r--r--   0 andreacensi   (501) staff       (20)      220 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/fork.html
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1651 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/index.rst
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.251925 PyGeometry-z6-2.1.5/docs/source/my_static/
+-rw-r--r--   0 andreacensi   (501) staff       (20)        0 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/my_static/.empty
+-rw-r--r--   0 andreacensi   (501) staff       (20)        8 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/my_static/.gitignore
+-rw-r--r--   0 andreacensi   (501) staff       (20)    70749 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/my_static/manifolds.png
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.252303 PyGeometry-z6-2.1.5/docs/source/my_templates/
+-rw-r--r--   0 andreacensi   (501) staff       (20)      846 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/my_templates/layout.html
+-rw-r--r--   0 andreacensi   (501) staff       (20)      157 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/source/todo.rst
+-rw-r--r--   0 andreacensi   (501) staff       (20)    10367 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/docs/sphinxtogithub.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1200 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/pypackage.mk
+-rw-r--r--   0 andreacensi   (501) staff       (20)      143 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/requirements.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)      153 2024-04-23 20:58:12.268571 PyGeometry-z6-2.1.5/setup.cfg
+-rw-r--r--   0 andreacensi   (501) staff       (20)      650 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/setup.json
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1210 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/setup.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      360 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/shippable.yml
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.234238 PyGeometry-z6-2.1.5/src/
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.253032 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/
+-rw-r--r--   0 andreacensi   (501) staff       (20)      348 2024-04-23 20:58:12.000000 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/PKG-INFO
+-rw-r--r--   0 andreacensi   (501) staff       (20)     7543 2024-04-23 20:58:12.000000 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/SOURCES.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)        1 2024-04-23 20:58:12.000000 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/dependency_links.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)       42 2024-04-23 20:58:12.000000 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/requires.txt
+-rw-r--r--   0 andreacensi   (501) staff       (20)        9 2024-04-23 20:58:12.000000 PyGeometry-z6-2.1.5/src/PyGeometry_z6.egg-info/top_level.txt
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.256186 PyGeometry-z6-2.1.5/src/geometry/
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1777 2024-04-23 20:53:30.000000 PyGeometry-z6-2.1.5/src/geometry/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2049 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/basic_utils.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      145 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/constants.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.256832 PyGeometry-z6-2.1.5/src/geometry/distances/
+-rw-r--r--   0 andreacensi   (501) staff       (20)      112 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/distances/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      310 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/distances/generic.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1731 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/distances/spherical.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2662 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/formatting.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.261659 PyGeometry-z6-2.1.5/src/geometry/manifolds/
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1262 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)    10220 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/differentiable_manifold.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4184 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/embedding_relations.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1448 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/euclidean.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      748 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/exceptions.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      529 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4821 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/manifold_embedding_propagation.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4347 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/manifold_relations.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1470 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_algebra.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     5362 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2187 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_group_tangent.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2019 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_linear_space.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1655 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/point_set.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1645 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/product_manifold.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3597 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/special_euclidean_algebra.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4289 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/special_euclidean_group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2087 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/special_orthogonal_algebra.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2887 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/special_orthogonal_group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     6011 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/sphere.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1664 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/square.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1732 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tangent_bundle.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.262796 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3406 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3181 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/checks_generation.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2031 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/embedding_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4648 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/manifold_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1222 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/matrix_groups_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      225 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/pickling_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      399 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/sphere_tests.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.263825 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/
+-rw-r--r--   0 andreacensi   (501) staff       (20)       86 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1316 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/grassman.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      657 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/moebius.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)       15 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/orthogonal_group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)       15 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/posdef_matrices.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      941 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/stiefel.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1507 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/torus.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3401 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/torus01.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1400 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/translation_algebra.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2258 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/manifolds/translation_group.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     5655 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/mds_algos.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)    12782 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/poses.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2625 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/poses_embedding.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1404 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/procrustes.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)    12885 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/rotations.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      969 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/rotations_embedding.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)    10681 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/spheres.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      847 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/spheres_embedding.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.264164 PyGeometry-z6-2.1.5/src/geometry/subspaces/
+-rw-r--r--   0 andreacensi   (501) staff       (20)       40 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/subspaces/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      924 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/subspaces/subspaces.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      226 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/tex.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1650 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/types.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.266492 PyGeometry-z6-2.1.5/src/geometry/unittests/
+-rw-r--r--   0 andreacensi   (501) staff       (20)       15 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)       15 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/distances_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2443 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/mds_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      234 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/misc_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3438 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/poses_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1370 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/procrustes_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1654 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/quaternions_test.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2008 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/random_geometry_density_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     4778 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/random_geometry_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2192 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/rotations_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)       15 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/spheres_tests.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      757 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/uniform_dist_pvalue_paranoia.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     2027 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/utils.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)      497 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/unittests/utils_test.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.266785 PyGeometry-z6-2.1.5/src/geometry/utils/
+-rw-r--r--   0 andreacensi   (501) staff       (20)       45 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/utils/__init__.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1167 2024-04-23 20:53:23.000000 PyGeometry-z6-2.1.5/src/geometry/utils/numpy_backport.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     3493 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/src/geometry/yaml_.py
+drwxr-xr-x   0 andreacensi   (501) staff       (20)        0 2024-04-23 20:58:12.268044 PyGeometry-z6-2.1.5/utils/
+-rw-r--r--   0 andreacensi   (501) staff       (20)    14577 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/utils/dot_parser.py
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1640 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/utils/manifolds.dot
+-rw-r--r--   0 andreacensi   (501) staff       (20)    70749 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/utils/manifolds.png
+-rw-r--r--   0 andreacensi   (501) staff       (20)    56373 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/utils/pydot_a.py.old
+-rw-r--r--   0 andreacensi   (501) staff       (20)     1756 2022-08-04 10:37:18.000000 PyGeometry-z6-2.1.5/utils/show_manifolds_relations.py
```

### Comparing `PyGeometry-z6-2.1.4/.compmake_history.txt` & `PyGeometry-z6-2.1.5/.compmake_history.txt`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/README.md` & `PyGeometry-z6-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/pypackage.mk` & `PyGeometry-z6-2.1.5/pypackage.mk`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/setup.json` & `PyGeometry-z6-2.1.5/setup.json`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/setup.py` & `PyGeometry-z6-2.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/__init__.py` & `PyGeometry-z6-2.1.5/src/geometry/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # coding=utf-8
-__version__ = "2.1.4"
+__version__ = "2.1.5"
 
 # If True, additional checks are done at runtime
 from zuper_commons.logs import ZLogger
 
 development = False
 
 # Does extra checks to make sure things are ok.
```

### Comparing `PyGeometry-z6-2.1.4/src/geometry/basic_utils.py` & `PyGeometry-z6-2.1.5/src/geometry/basic_utils.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/distances/spherical.py` & `PyGeometry-z6-2.1.5/src/geometry/distances/spherical.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/formatting.py` & `PyGeometry-z6-2.1.5/src/geometry/formatting.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/__init__.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/differentiable_manifold.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/differentiable_manifold.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/embedding_relations.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/embedding_relations.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/euclidean.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/euclidean.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/exceptions.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/group.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/group.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/manifold_embedding_propagation.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/manifold_embedding_propagation.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/manifold_relations.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/manifold_relations.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_algebra.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_algebra.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_group.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_group.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_lie_group_tangent.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_lie_group_tangent.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/matrix_linear_space.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/matrix_linear_space.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/point_set.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/point_set.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/product_manifold.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/product_manifold.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/special_euclidean_algebra.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/special_euclidean_algebra.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/special_euclidean_group.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/special_euclidean_group.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/special_orthogonal_algebra.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/special_orthogonal_algebra.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/special_orthogonal_group.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/special_orthogonal_group.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/sphere.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/sphere.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/square.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/square.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tangent_bundle.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tangent_bundle.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/__init__.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/checks_generation.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/checks_generation.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/embedding_test.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/embedding_test.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/manifold_tests.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/manifold_tests.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/tests/matrix_groups_tests.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/tests/matrix_groups_tests.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/grassman.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/grassman.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/moebius.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/moebius.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/todo/stiefel.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/todo/stiefel.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/torus.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/torus.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/torus01.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/torus01.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/translation_algebra.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/translation_algebra.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/manifolds/translation_group.py` & `PyGeometry-z6-2.1.5/src/geometry/manifolds/translation_group.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/mds_algos.py` & `PyGeometry-z6-2.1.5/src/geometry/mds_algos.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/poses.py` & `PyGeometry-z6-2.1.5/src/geometry/poses.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/poses_embedding.py` & `PyGeometry-z6-2.1.5/src/geometry/poses_embedding.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/procrustes.py` & `PyGeometry-z6-2.1.5/src/geometry/procrustes.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/rotations.py` & `PyGeometry-z6-2.1.5/src/geometry/rotations.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/rotations_embedding.py` & `PyGeometry-z6-2.1.5/src/geometry/rotations_embedding.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/spheres.py` & `PyGeometry-z6-2.1.5/src/geometry/spheres.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/spheres_embedding.py` & `PyGeometry-z6-2.1.5/src/geometry/spheres_embedding.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/subspaces/subspaces.py` & `PyGeometry-z6-2.1.5/src/geometry/subspaces/subspaces.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/types.py` & `PyGeometry-z6-2.1.5/src/geometry/types.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/mds_test.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/mds_test.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/poses_test.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/poses_test.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/procrustes_test.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/procrustes_test.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/quaternions_test.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/quaternions_test.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/random_geometry_density_tests.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/random_geometry_density_tests.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/random_geometry_tests.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/random_geometry_tests.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/rotations_tests.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/rotations_tests.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/uniform_dist_pvalue_paranoia.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/uniform_dist_pvalue_paranoia.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/unittests/utils.py` & `PyGeometry-z6-2.1.5/src/geometry/unittests/utils.py`

 * *Files identical despite different names*

### Comparing `PyGeometry-z6-2.1.4/src/geometry/utils/numpy_backport.py` & `PyGeometry-z6-2.1.5/src/geometry/utils/numpy_backport.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 
 try:
     from numpy.testing.utils import assert_allclose  # @UnusedImport
 except ImportError:
 
     def assert_allclose(actual, desired, rtol=1e-7, atol=0, err_msg="", verbose=True):
         """ Backporting assert_allclose from Numpy 1.5 to 1.4 """
-        from numpy.testing.utils import assert_array_compare  # @UnresolvedImport
+        try:
+            from numpy.testing.utils import assert_array_compare  # @UnresolvedImport
+        except ImportError:
+            from numpy.testing import assert_array_compare  # @UnresolvedImport
 
         def compare(x, y):
             return np.allclose(x, y, rtol=rtol, atol=atol)
 
         actual, desired = np.asanyarray(actual), np.asanyarray(desired)
         header = "Not equal to tolerance rtol=%g, atol=%g" % (rtol, atol)
         assert_array_compare(compare, actual, desired, err_msg=str(err_msg), verbose=verbose, header=header)
```

### Comparing `PyGeometry-z6-2.1.4/src/geometry/yaml_.py` & `PyGeometry-z6-2.1.5/src/geometry/yaml_.py`

 * *Files identical despite different names*

