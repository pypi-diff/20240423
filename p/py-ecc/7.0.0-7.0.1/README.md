# Comparing `tmp/py-ecc-7.0.0.tar.gz` & `tmp/py_ecc-7.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-ecc-7.0.0.tar", last modified: Wed Dec  6 19:29:08 2023, max compression
+gzip compressed data, was "py_ecc-7.0.1.tar", last modified: Tue Apr 23 15:54:50 2024, max compression
```

## Comparing `py-ecc-7.0.0.tar` & `py_ecc-7.0.1.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.336661 py-ecc-7.0.0/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1083 2023-12-06 19:21:17.000000 py-ecc-7.0.0/LICENSE
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      168 2023-12-06 19:21:17.000000 py-ecc-7.0.0/MANIFEST.in
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     6132 2023-12-06 19:29:08.336661 py-ecc-7.0.0/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4359 2023-12-06 19:21:17.000000 py-ecc-7.0.0/README.md
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      288 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/__init__.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/bls/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       95 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11014 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/ciphersuites.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      655 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/constants.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1125 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/g2_primitives.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2521 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/hash.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2614 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/hash_to_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7085 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/point_compression.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      409 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls/typing.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/bls12_381/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      482 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls12_381/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4371 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls12_381/bls12_381_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3033 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bls12_381/bls12_381_pairing.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/bn128/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      458 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bn128/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3920 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bn128/bn128_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3031 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/bn128/bn128_pairing.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/fields/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2768 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/fields/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12313 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/fields/field_elements.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1111 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/fields/field_properties.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14497 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/fields/optimized_field_elements.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/optimized_bls12_381/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      680 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4931 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/constants.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      525 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_clear_cofactor.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5371 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5823 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_pairing.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3673 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_swu.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/optimized_bn128/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      521 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bn128/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4914 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bn128/optimized_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5530 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/optimized_bn128/optimized_pairing.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-11-01 22:15:34.000000 py-ecc-7.0.0/py_ecc/py.typed
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc/secp256k1/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      155 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/secp256k1/__init__.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5060 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/secp256k1/secp256k1.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2173 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/typing.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1497 2023-12-06 19:21:17.000000 py-ecc-7.0.0/py_ecc/utils.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/py_ecc.egg-info/
--rw-r--r--   0 pacrob    (1000) pacrob    (1000)     6132 2023-12-06 19:29:08.000000 py-ecc-7.0.0/py_ecc.egg-info/PKG-INFO
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1733 2023-12-06 19:29:08.000000 py-ecc-7.0.0/py_ecc.egg-info/SOURCES.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-06 19:29:08.000000 py-ecc-7.0.0/py_ecc.egg-info/dependency_links.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-12-06 17:13:19.000000 py-ecc-7.0.0/py_ecc.egg-info/not-zip-safe
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      342 2023-12-06 19:29:08.000000 py-ecc-7.0.0/py_ecc.egg-info/requires.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        7 2023-12-06 19:29:08.000000 py-ecc-7.0.0/py_ecc.egg-info/top_level.txt
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3428 2023-12-06 19:21:17.000000 py-ecc-7.0.0/pyproject.toml
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2023-12-06 19:29:08.336661 py-ecc-7.0.0/setup.cfg
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2007 2023-12-06 19:28:38.000000 py-ecc-7.0.0/setup.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/tests/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/tests/bls/
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/tests/bls/ciphersuites/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3474 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_basic.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      965 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_message_augmentation.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3538 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_pop.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4830 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_expand_message_xmd.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1748 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_g2_core.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      772 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_g2_primatives.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10803 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_hash_to_curve.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2497 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_hkdf.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5707 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/bls/test_point_compression.py
-drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2023-12-06 19:29:08.332661 py-ecc-7.0.0/tests/core/
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       51 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/core/test_import.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      856 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/test_backward_compatibility.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11044 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/test_bn128_and_bls12_381.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      944 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/test_secp256k1.py
--rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      290 2023-12-06 19:21:17.000000 py-ecc-7.0.0/tests/test_utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1083 2024-03-11 16:15:51.000000 py_ecc-7.0.1/LICENSE
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      196 2024-04-22 21:35:10.000000 py_ecc-7.0.1/MANIFEST.in
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     6302 2024-04-23 15:54:50.210238 py_ecc-7.0.1/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4359 2024-03-11 16:15:51.000000 py_ecc-7.0.1/README.md
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      288 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/__init__.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/bls/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       95 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11014 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/ciphersuites.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      655 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1125 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/g2_primitives.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2521 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/hash.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2614 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/hash_to_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     7085 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/point_compression.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      409 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/bls/typing.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/bls12_381/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      433 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bls12_381/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4322 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bls12_381/bls12_381_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2984 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bls12_381/bls12_381_pairing.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/bn128/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      409 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bn128/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3871 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bn128/bn128_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2982 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/bn128/bn128_pairing.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/fields/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2768 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/fields/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    12297 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/fields/field_elements.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1052 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/fields/field_properties.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    14481 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/fields/optimized_field_elements.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/optimized_bls12_381/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      631 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4931 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/constants.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      525 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_clear_cofactor.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5322 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5774 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_pairing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3673 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_swu.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/py_ecc/optimized_bn128/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      472 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bn128/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4865 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bn128/optimized_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5481 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/optimized_bn128/optimized_pairing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        0 2023-12-04 20:09:46.000000 py_ecc-7.0.1/py_ecc/py.typed
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/py_ecc/secp256k1/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      106 2024-04-22 21:35:10.000000 py_ecc-7.0.1/py_ecc/secp256k1/__init__.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5060 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/secp256k1/secp256k1.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2173 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/typing.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1497 2024-03-11 16:15:51.000000 py_ecc-7.0.1/py_ecc/utils.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/py_ecc.egg-info/
+-rw-r--r--   0 pacrob    (1000) pacrob    (1000)     6302 2024-04-23 15:54:50.000000 py_ecc-7.0.1/py_ecc.egg-info/PKG-INFO
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1765 2024-04-23 15:54:50.000000 py_ecc-7.0.1/py_ecc.egg-info/SOURCES.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2024-04-23 15:54:50.000000 py_ecc-7.0.1/py_ecc.egg-info/dependency_links.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        1 2023-10-29 19:43:57.000000 py_ecc-7.0.1/py_ecc.egg-info/not-zip-safe
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      398 2024-04-23 15:54:50.000000 py_ecc-7.0.1/py_ecc.egg-info/requires.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)        7 2024-04-23 15:54:50.000000 py_ecc-7.0.1/py_ecc.egg-info/top_level.txt
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3426 2024-04-22 21:35:10.000000 py_ecc-7.0.1/pyproject.toml
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       38 2024-04-23 15:54:50.210238 py_ecc-7.0.1/setup.cfg
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2096 2024-04-23 15:54:31.000000 py_ecc-7.0.1/setup.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.206238 py_ecc-7.0.1/tests/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/tests/bls/
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/tests/bls/ciphersuites/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3475 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_basic.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      965 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_message_augmentation.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     3538 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_pop.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     4829 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/bls/test_expand_message_xmd.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     1748 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/test_g2_core.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      772 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/test_g2_primatives.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    10827 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/bls/test_hash_to_curve.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     2497 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/test_hkdf.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)     5707 2024-03-11 16:15:51.000000 py_ecc-7.0.1/tests/bls/test_point_compression.py
+drwxrwxr-x   0 pacrob    (1000) pacrob    (1000)        0 2024-04-23 15:54:50.210238 py_ecc-7.0.1/tests/core/
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      856 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/core/test_backward_compatibility.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)    11044 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/core/test_bn128_and_bls12_381.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)       97 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/core/test_import_and_version.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      944 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/core/test_secp256k1.py
+-rw-rw-r--   0 pacrob    (1000) pacrob    (1000)      290 2024-04-22 21:35:10.000000 py_ecc-7.0.1/tests/core/test_utils.py
```

### Comparing `py-ecc-7.0.0/LICENSE` & `py_ecc-7.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/PKG-INFO` & `py_ecc-7.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ecc
-Version: 7.0.0
+Version: 7.0.1
 Summary: py-ecc: Elliptic curve crypto in python including secp256k1, alt_bn128, and bls12_381
 Home-page: https://github.com/ethereum/py_ecc
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-typing>=3.0.0
 Requires-Dist: eth-utils>=2.0.0
 Requires-Dist: cached-property>=1.5.1
 Provides-Extra: dev
@@ -27,20 +28,22 @@
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
 
 # py_ecc
```

### Comparing `py-ecc-7.0.0/README.md` & `py_ecc-7.0.1/README.md`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/ciphersuites.py` & `py_ecc-7.0.1/py_ecc/bls/ciphersuites.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/constants.py` & `py_ecc-7.0.1/py_ecc/bls/constants.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/g2_primitives.py` & `py_ecc-7.0.1/py_ecc/bls/g2_primitives.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/hash.py` & `py_ecc-7.0.1/py_ecc/bls/hash.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/hash_to_curve.py` & `py_ecc-7.0.1/py_ecc/bls/hash_to_curve.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls/point_compression.py` & `py_ecc-7.0.1/py_ecc/bls/point_compression.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/bls12_381/bls12_381_curve.py` & `py_ecc-7.0.1/py_ecc/bls12_381/bls12_381_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     bls12_381_FQ as FQ,
     bls12_381_FQ2 as FQ2,
     bls12_381_FQ12 as FQ12,
     bls12_381_FQP as FQP,
 )
 from py_ecc.fields.field_properties import (
```

### Comparing `py-ecc-7.0.0/py_ecc/bls12_381/bls12_381_pairing.py` & `py_ecc-7.0.1/py_ecc/bls12_381/bls12_381_pairing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     bls12_381_FQ as FQ,
     bls12_381_FQ2 as FQ2,
     bls12_381_FQ12 as FQ12,
 )
 from py_ecc.fields.field_properties import (
     field_properties,
```

### Comparing `py-ecc-7.0.0/py_ecc/bn128/bn128_curve.py` & `py_ecc-7.0.1/py_ecc/bn128/bn128_curve.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     bn128_FQ as FQ,
     bn128_FQ2 as FQ2,
     bn128_FQ12 as FQ12,
     bn128_FQP as FQP,
 )
 from py_ecc.fields.field_properties import (
```

### Comparing `py-ecc-7.0.0/py_ecc/bn128/bn128_pairing.py` & `py_ecc-7.0.1/py_ecc/bn128/bn128_pairing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     bn128_FQ as FQ,
     bn128_FQ2 as FQ2,
     bn128_FQ12 as FQ12,
 )
 from py_ecc.fields.field_properties import (
     field_properties,
```

### Comparing `py-ecc-7.0.0/py_ecc/fields/__init__.py` & `py_ecc-7.0.1/py_ecc/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/fields/field_elements.py` & `py_ecc-7.0.1/py_ecc/fields/field_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 T_FQ = TypeVar("T_FQ", bound="FQ")
 T_FQP = TypeVar("T_FQP", bound="FQP")
 T_FQ2 = TypeVar("T_FQ2", bound="FQ2")
 T_FQ12 = TypeVar("T_FQ12", bound="FQ12")
 IntOrFQ = Union[int, T_FQ]
 
 
-class FQ(object):
+class FQ:
     """
     A class for field elements in FQ. Wrap a number in this class,
     and it becomes a field element.
     """
 
     n = None  # type: int
     field_modulus = None  # type: int
@@ -181,15 +181,15 @@
     def zero(cls: Type[T_FQ]) -> T_FQ:
         return cls(0)
 
 
 int_types_or_FQ = (int, FQ)
 
 
-class FQP(object):
+class FQP:
     """
     A class for elements in polynomial extension fields
     """
 
     degree = 0
     field_modulus = None  # type: int
```

### Comparing `py-ecc-7.0.0/py_ecc/fields/optimized_field_elements.py` & `py_ecc-7.0.1/py_ecc/fields/optimized_field_elements.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         return x % n
     elif isinstance(x, FQ):
         return x.n % n
     else:
         raise TypeError("Only int and T_FQ types are accepted: got %s" % type(x))
 
 
-class FQ(object):
+class FQ:
     """
     A class for field elements in FQ. Wrap a number in this class,
     and it becomes a field element.
     """
 
     n = None  # type: int
     field_modulus = None  # type: int
@@ -205,15 +205,15 @@
         return cls(1)
 
     @classmethod
     def zero(cls: Type[T_FQ]) -> T_FQ:
         return cls(0)
 
 
-class FQP(object):
+class FQP:
     """
     A class for elements in polynomial extension fields
     """
 
     degree: int = 0
     field_modulus: Union[int, None] = None
     mc_tuples: Union[List[Tuple[int, int]], None] = None
```

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/__init__.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     optimized_bls12_381_FQ as FQ,
     optimized_bls12_381_FQ2 as FQ2,
     optimized_bls12_381_FQ12 as FQ12,
     optimized_bls12_381_FQP as FQP,
 )
```

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/constants.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/constants.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_clear_cofactor.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_clear_cofactor.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_curve.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     optimized_bls12_381_FQ as FQ,
     optimized_bls12_381_FQ2 as FQ2,
     optimized_bls12_381_FQ12 as FQ12,
     optimized_bls12_381_FQP as FQP,
 )
 from py_ecc.fields.field_properties import (
```

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_pairing.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_pairing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     optimized_bls12_381_FQ as FQ,
     optimized_bls12_381_FQ2 as FQ2,
     optimized_bls12_381_FQ12 as FQ12,
 )
 from py_ecc.fields.field_properties import (
     field_properties,
```

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bls12_381/optimized_swu.py` & `py_ecc-7.0.1/py_ecc/optimized_bls12_381/optimized_swu.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bn128/optimized_curve.py` & `py_ecc-7.0.1/py_ecc/optimized_bn128/optimized_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     optimized_bn128_FQ as FQ,
     optimized_bn128_FQ2 as FQ2,
     optimized_bn128_FQ12 as FQ12,
     optimized_bn128_FQP as FQP,
 )
 from py_ecc.fields.field_properties import (
```

### Comparing `py-ecc-7.0.0/py_ecc/optimized_bn128/optimized_pairing.py` & `py_ecc-7.0.1/py_ecc/optimized_bn128/optimized_pairing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-from __future__ import (
-    absolute_import,
-)
-
 from py_ecc.fields import (
     optimized_bn128_FQ as FQ,
     optimized_bn128_FQ2 as FQ2,
     optimized_bn128_FQ12 as FQ12,
 )
 from py_ecc.fields.field_properties import (
     field_properties,
```

### Comparing `py-ecc-7.0.0/py_ecc/secp256k1/secp256k1.py` & `py_ecc-7.0.1/py_ecc/secp256k1/secp256k1.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/typing.py` & `py_ecc-7.0.1/py_ecc/typing.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc/utils.py` & `py_ecc-7.0.1/py_ecc/utils.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/py_ecc.egg-info/PKG-INFO` & `py_ecc-7.0.1/py_ecc.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-ecc
-Version: 7.0.0
+Version: 7.0.1
 Summary: py-ecc: Elliptic curve crypto in python including secp256k1, alt_bn128, and bls12_381
 Home-page: https://github.com/ethereum/py_ecc
 Author: The Ethereum Foundation
 Author-email: snakecharmers@ethereum.org
 License: MIT
 Keywords: ethereum
 Classifier: Development Status :: 3 - Alpha
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eth-typing>=3.0.0
 Requires-Dist: eth-utils>=2.0.0
 Requires-Dist: cached-property>=1.5.1
 Provides-Extra: dev
@@ -27,20 +28,22 @@
 Requires-Dist: bumpversion>=0.5.3; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: pre-commit>=3.4.0; extra == "dev"
 Requires-Dist: tox>=4.0.0; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: wheel; extra == "dev"
 Requires-Dist: sphinx>=6.0.0; extra == "dev"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "dev"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "dev"
 Requires-Dist: towncrier<22,>=21; extra == "dev"
 Requires-Dist: pytest>=7.0.0; extra == "dev"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx>=6.0.0; extra == "docs"
+Requires-Dist: sphinx-autobuild>=2021.3.14; extra == "docs"
 Requires-Dist: sphinx_rtd_theme>=1.0.0; extra == "docs"
 Requires-Dist: towncrier<22,>=21; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest>=7.0.0; extra == "test"
 Requires-Dist: pytest-xdist>=2.4.0; extra == "test"
 
 # py_ecc
```

### Comparing `py-ecc-7.0.0/py_ecc.egg-info/SOURCES.txt` & `py_ecc-7.0.1/py_ecc.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -38,21 +38,21 @@
 py_ecc/optimized_bls12_381/optimized_pairing.py
 py_ecc/optimized_bls12_381/optimized_swu.py
 py_ecc/optimized_bn128/__init__.py
 py_ecc/optimized_bn128/optimized_curve.py
 py_ecc/optimized_bn128/optimized_pairing.py
 py_ecc/secp256k1/__init__.py
 py_ecc/secp256k1/secp256k1.py
-tests/test_backward_compatibility.py
-tests/test_bn128_and_bls12_381.py
-tests/test_secp256k1.py
-tests/test_utils.py
 tests/bls/test_expand_message_xmd.py
 tests/bls/test_g2_core.py
 tests/bls/test_g2_primatives.py
 tests/bls/test_hash_to_curve.py
 tests/bls/test_hkdf.py
 tests/bls/test_point_compression.py
 tests/bls/ciphersuites/test_g2_basic.py
 tests/bls/ciphersuites/test_g2_message_augmentation.py
 tests/bls/ciphersuites/test_g2_pop.py
-tests/core/test_import.py
+tests/core/test_backward_compatibility.py
+tests/core/test_bn128_and_bls12_381.py
+tests/core/test_import_and_version.py
+tests/core/test_secp256k1.py
+tests/core/test_utils.py
```

### Comparing `py-ecc-7.0.0/pyproject.toml` & `py_ecc-7.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [tool.autoflake]
-remove_all_unused_imports = "True"
 exclude = "__init__.py"
+remove_all_unused_imports = true
 
 [tool.isort]
-combine_as_imports = "True"
+combine_as_imports = true
 extra_standard_library = "pytest"
 force_grid_wrap = 1
-force_sort_within_sections = "True"
-known_third_party = "hypothesis,pytest"
+force_sort_within_sections = true
+honor_noqa = true
 known_first_party = "py_ecc"
+known_third_party = "hypothesis"
 multi_line_output = 3
 profile = "black"
+use_parentheses = true
 
 [tool.mypy]
-check_untyped_defs = "True"
-disallow_incomplete_defs = "True"
-disallow_untyped_defs = "True"
-disallow_any_generics = "True"
-disallow_untyped_calls = "True"
-disallow_untyped_decorators = "True"
-disallow_subclassing_any = "True"
-ignore_missing_imports = "True"
-strict_optional = "True"
-strict_equality = "True"
-warn_redundant_casts = "True"
-warn_return_any = "True"
-warn_unused_configs = "True"
-warn_unused_ignores = "True"
+check_untyped_defs = true
+disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
+ignore_missing_imports = true
+strict_equality = true
+strict_optional = true
+warn_redundant_casts = true
+warn_return_any = true
+warn_unused_configs = true
+warn_unused_ignores = true
 
 
 [tool.pydocstyle]
 # All error codes found here:
 # http://www.pydocstyle.org/en/3.0.0/error_codes.html
 #
 # Ignored:
@@ -59,26 +61,26 @@
 # D400 - Enabling this error code seems to make it a requirement that the first
 # sentence in a docstring is not split across two lines.  It also makes it a
 # requirement that no docstring can have a multi-sentence description without a
 # summary line.  Neither one of those requirements seem appropriate.
 
 [tool.pytest.ini_options]
 addopts = "-v --showlocals --durations 10"
-xfail_strict = "True"
-log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
 log_date_format = "%m-%d %H:%M:%S"
+log_format = "%(levelname)8s  %(asctime)s  %(filename)20s  %(message)s"
+xfail_strict = true
 
 [tool.towncrier]
 # Read https://github.com/ethereum/py_ecc/blob/main/newsfragments/README.md for instructions
-package = "py_ecc"
-filename = "CHANGELOG.rst"
 directory = "newsfragments"
-underlines = ["-", "~", "^"]
-title_format = "py_ecc v{version} ({project_date})"
+filename = "CHANGELOG.rst"
 issue_format = "`#{issue} <https://github.com/ethereum/py_ecc/issues/{issue}>`__"
+package = "py_ecc"
+title_format = "py_ecc v{version} ({project_date})"
+underlines = ["-", "~", "^"]
 
 [[tool.towncrier.type]]
 directory = "breaking"
 name = "Breaking Changes"
 showcontent = true
 
 [[tool.towncrier.type]]
```

### Comparing `py-ecc-7.0.0/setup.py` & `py_ecc-7.0.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import (
     find_packages,
     setup,
 )
 
 extras_require = {
     "dev": [
@@ -13,14 +12,15 @@
         "pre-commit>=3.4.0",
         "tox>=4.0.0",
         "twine",
         "wheel",
     ],
     "docs": [
         "sphinx>=6.0.0",
+        "sphinx-autobuild>=2021.3.14",
         "sphinx_rtd_theme>=1.0.0",
         "towncrier>=21,<22",
     ],
     "test": [
         "pytest>=7.0.0",
         "pytest-xdist>=2.4.0",
     ],
@@ -34,15 +34,15 @@
 with open("./README.md") as readme:
     long_description = readme.read()
 
 
 setup(
     name="py-ecc",
     # *IMPORTANT*: Don't manually change the version here. Use `make bump`, as described in readme
-    version="7.0.0",
+    version="7.0.1",
     description="""py-ecc: Elliptic curve crypto in python including secp256k1, alt_bn128, and bls12_381""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="The Ethereum Foundation",
     author_email="snakecharmers@ethereum.org",
     url="https://github.com/ethereum/py_ecc",
     include_package_data=True,
@@ -53,21 +53,22 @@
     ],
     python_requires=">=3.8, <4",
     extras_require=extras_require,
     py_modules=["py_ecc"],
     license="MIT",
     zip_safe=False,
     keywords="ethereum",
-    packages=find_packages(exclude=["tests", "tests.*"]),
+    packages=find_packages(exclude=["scripts", "scripts.*", "tests", "tests.*"]),
     package_data={"py_ecc": ["py.typed"]},
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_basic.py` & `py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import pytest
+
 from eth_utils import (
     ValidationError,
 )
-import pytest
 
 from py_ecc.bls import (
     G2Basic,
 )
 from py_ecc.bls.g2_primitives import (
     G1_to_pubkey,
     G2_to_signature,
```

### Comparing `py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_message_augmentation.py` & `py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_message_augmentation.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/bls/ciphersuites/test_g2_pop.py` & `py_ecc-7.0.1/tests/bls/ciphersuites/test_g2_pop.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/bls/test_expand_message_xmd.py` & `py_ecc-7.0.1/tests/bls/test_expand_message_xmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from hashlib import (
     sha256,
 )
-
 import pytest
 
 from py_ecc.bls.hash import (
     expand_message_xmd,
 )
 
 # The test vectors from
```

### Comparing `py-ecc-7.0.0/tests/bls/test_g2_core.py` & `py_ecc-7.0.1/tests/bls/test_g2_core.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/bls/test_g2_primatives.py` & `py_ecc-7.0.1/tests/bls/test_g2_primatives.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/bls/test_hash_to_curve.py` & `py_ecc-7.0.1/tests/bls/test_hash_to_curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 These are temporary tests to check the functionality of helper functions in `hash_to_G2`
 They should be removed and replaced with a final version when hash to curve is complete.
 """
 from hashlib import (
     sha256,
 )
-
 import pytest
 
 from py_ecc.bls.hash_to_curve import (
     hash_to_G2,
 )
 from py_ecc.fields import (
     optimized_bls12_381_FQ as FQ,
@@ -161,15 +160,15 @@
     result_x = result_x / result_z
     result_y = result_y / result_z
 
     assert g2_x == result_x
     assert g2_y == result_y
 
 
-# Tests taken from: https://github.com/cfrg/draft-irtf-cfrg-hash-to-curve/blob/master/draft-irtf-cfrg-hash-to-curve.md#bls12381g2_xmdsha-256_sswu_ro_  # noqa: E501
+# Tests taken from: https://github.com/cfrg/draft-irtf-cfrg-hash-to-curve/blob/master/draft-irtf-cfrg-hash-to-curve.md#bls12381g2_xmdsha-256_sswu_ro_  # blocklint: URL pragma  # noqa: E501
 @pytest.mark.parametrize("H", [sha256])
 @pytest.mark.parametrize(
     "msg,x,y",
     [
         (
             b"",
             FQ2(
```

### Comparing `py-ecc-7.0.0/tests/bls/test_hkdf.py` & `py_ecc-7.0.1/tests/bls/test_hkdf.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/bls/test_point_compression.py` & `py_ecc-7.0.1/tests/bls/test_point_compression.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/test_backward_compatibility.py` & `py_ecc-7.0.1/tests/core/test_backward_compatibility.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/test_bn128_and_bls12_381.py` & `py_ecc-7.0.1/tests/core/test_bn128_and_bls12_381.py`

 * *Files identical despite different names*

### Comparing `py-ecc-7.0.0/tests/test_secp256k1.py` & `py_ecc-7.0.1/tests/core/test_secp256k1.py`

 * *Files identical despite different names*

