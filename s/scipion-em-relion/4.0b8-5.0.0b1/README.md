# Comparing `tmp/scipion-em-relion-4.0b8.tar.gz` & `tmp/scipion-em-relion-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-relion-4.0b8.tar", last modified: Sat Nov 27 18:21:59 2021, max compression
+gzip compressed data, was "scipion-em-relion-5.0.0b1.tar", last modified: Mon Apr 22 13:37:24 2024, max compression
```

## Comparing `scipion-em-relion-4.0b8.tar` & `scipion-em-relion-5.0.0b1.tar`

### file list

```diff
@@ -1,93 +1,103 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.437534 scipion-em-relion-4.0b8/
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      230 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6017 2021-11-27 18:21:59.437534 scipion-em-relion-4.0b8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4299 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.429534 scipion-em-relion-4.0b8/relion/
--rw-r--r--   0 runner    (1001) docker     (121)     3932 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4265 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     4342 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.429534 scipion-em-relion-4.0b8/relion/convert/
--rw-r--r--   0 runner    (1001) docker     (121)     8093 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4457 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert30.py
--rw-r--r--   0 runner    (1001) docker     (121)    24811 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert31.py
--rw-r--r--   0 runner    (1001) docker     (121)     8085 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     7506 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (121)    21375 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     8692 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/convert_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17745 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/dataimport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.429534 scipion-em-relion-4.0b8/relion/convert/mtfs/
--rw-r--r--   0 runner    (1001) docker     (121)     9038 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_de20_300.star
--rw-r--r--   0 runner    (1001) docker     (121)    15520 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f2_300.star
--rw-r--r--   0 runner    (1001) docker     (121)     1428 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f3_200_ec.star
--rw-r--r--   0 runner    (1001) docker     (121)     1422 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f3_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f4_200_ec.star
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f4_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_k2_300_ec.star
--rw-r--r--   0 runner    (1001) docker     (121)     5133 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.433534 scipion-em-relion-4.0b8/relion/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     3039 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.433534 scipion-em-relion-4.0b8/relion/protocols/_legacy/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23085 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/_legacy/protocol31_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    15592 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_assign_optic_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     5195 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_autopick.py
--rw-r--r--   0 runner    (1001) docker     (121)     7532 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_autopick_log.py
--rw-r--r--   0 runner    (1001) docker     (121)    24635 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_autopick_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)    72066 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    23016 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_bayesian_polishing.py
--rw-r--r--   0 runner    (1001) docker     (121)     3781 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_center_averages.py
--rw-r--r--   0 runner    (1001) docker     (121)     5111 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_classify2d.py
--rw-r--r--   0 runner    (1001) docker     (121)     6767 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_classify3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_compress_movies.py
--rw-r--r--   0 runner    (1001) docker     (121)     9305 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_create_mask3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     6901 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_crop_resize.py
--rw-r--r--   0 runner    (1001) docker     (121)    15726 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_ctf_refinement.py
--rw-r--r--   0 runner    (1001) docker     (121)     5079 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_estimate_gain.py
--rw-r--r--   0 runner    (1001) docker     (121)     5226 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_expand_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3439 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_export_coords.py
--rw-r--r--   0 runner    (1001) docker     (121)     6545 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_export_ctf.py
--rw-r--r--   0 runner    (1001) docker     (121)     5966 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_export_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)    21115 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_extract_particles.py
--rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_gentle_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)    18466 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_initialmodel.py
--rw-r--r--   0 runner    (1001) docker     (121)    10098 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_localres.py
--rw-r--r--   0 runner    (1001) docker     (121)    29794 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_motioncor.py
--rw-r--r--   0 runner    (1001) docker     (121)    18530 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_multibody.py
--rw-r--r--   0 runner    (1001) docker     (121)    14927 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)    13050 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     7387 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_reconstruct.py
--rw-r--r--   0 runner    (1001) docker     (121)     7671 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_refine3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     7257 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_remove_views.py
--rw-r--r--   0 runner    (1001) docker     (121)     5947 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_select_classes.py
--rw-r--r--   0 runner    (1001) docker     (121)    15704 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_subtract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3519 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols/protocol_symmetrize_volume.py
--rw-r--r--   0 runner    (1001) docker     (121)     5946 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/protocols.conf
--rw-r--r--   0 runner    (1001) docker     (121)    15098 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/relion_logo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.433534 scipion-em-relion-4.0b8/relion/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1486 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    36717 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/test_convert_relion.py
--rw-r--r--   0 runner    (1001) docker     (121)     6328 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/test_projection_subtraction_no_relion.py
--rw-r--r--   0 runner    (1001) docker     (121)    63612 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/test_protocols_relion.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    15690 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/test_protocols_relion3.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7238 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/tests/test_workflow_relion3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.433534 scipion-em-relion-4.0b8/relion/viewers/
--rw-r--r--   0 runner    (1001) docker     (121)     1459 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38359 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    16162 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_ctfrefine.py
--rw-r--r--   0 runner    (1001) docker     (121)     5896 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_locres.py
--rw-r--r--   0 runner    (1001) docker     (121)     7208 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_motioncor.py
--rw-r--r--   0 runner    (1001) docker     (121)     6209 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_multibody.py
--rw-r--r--   0 runner    (1001) docker     (121)     4537 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_polishing.py
--rw-r--r--   0 runner    (1001) docker     (121)    10929 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/viewers/viewer_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)     7732 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/relion/wizards.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-27 18:21:59.433534 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6017 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2915 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-11-27 18:21:59.000000 scipion-em-relion-4.0b8/scipion_em_relion.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-27 18:21:59.437534 scipion-em-relion-4.0b8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8485 2021-11-27 18:20:25.000000 scipion-em-relion-4.0b8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.858610 scipion-em-relion-5.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)     8898 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-22 13:37:24.858610 scipion-em-relion-5.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.846609 scipion-em-relion-5.0.0b1/relion/
+-rw-r--r--   0 runner    (1001) docker     (127)     6108 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24744 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.846609 scipion-em-relion-5.0.0b1/relion/convert/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4457 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert30.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27420 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert31.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8480 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21454 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/convert_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17428 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/dataimport.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.850609 scipion-em-relion-5.0.0b1/relion/convert/mtfs/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_apollo_300_ec_stdres.star
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_apollo_300_ec_superres.star
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_de20_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)    19051 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_eigerX500K_100.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15525 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f1_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15520 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f2_300.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f3_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    45351 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f3_200_linear.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f3_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f4_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f4_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    16093 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_k2_200_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_k2_300_ec.star
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.854610 scipion-em-relion-5.0.0b1/relion/protocols/
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_assign_optic_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23860 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72076 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22684 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_bayesian_polishing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10567 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_calculate_fsc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_center_averages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5146 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_classify2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6977 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_classify3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8097 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_compress_movies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_create_mask3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7376 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_crop_resize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15811 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_ctf_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_dynamight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5136 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_estimate_gain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_expand_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3439 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6573 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20875 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_extract_particles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_gentle_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_import_coords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18508 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_initialmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9977 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_localres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_motioncor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24114 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_multibody.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16883 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13197 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9956 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7959 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_refine3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_remove_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6933 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_select_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15643 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_subtract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols/protocol_symmetrize_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6024 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/protocols.conf
+-rw-r--r--   0 runner    (1001) docker     (127)    15098 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/relion_logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.854610 scipion-em-relion-5.0.0b1/relion/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    31770 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/templates/betagal-turorial.json.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.854610 scipion-em-relion-5.0.0b1/relion/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36724 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_projection_subtraction_no_relion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39097 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_protocols_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29462 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_protocols_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_protocols_base.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7491 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/tests/test_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.858610 scipion-em-relion-5.0.0b1/relion/viewers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38984 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16060 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_ctfrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_locres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7208 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_motioncor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_multibody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_polishing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/viewers/viewer_reconstruct.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/relion/wizards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 13:37:24.858610 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-22 13:37:24.000000 scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-22 13:37:24.858610 scipion-em-relion-5.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8493 2024-04-22 13:36:55.000000 scipion-em-relion-5.0.0b1/setup.py
```

### Comparing `scipion-em-relion-4.0b8/LICENSE` & `scipion-em-relion-5.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/PKG-INFO` & `scipion-em-relion-5.0.0b1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 1.2
 Name: scipion-em-relion
-Version: 4.0b8
+Version: 5.0.0b1
 Summary: Plugin to use Relion programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-relion
 Author: Grigory Sharov, J.M. De la Rosa Trevin, Josue Gomez Blanco
 Author-email: gsharov@mrc-lmb.cam.ac.uk, delarosatrevin@scilifelab.se, josue.gomez-blanco@mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-relion/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-relion/
 Description: =============
         Relion plugin
         =============
         
-        This plugin provide wrappers around several programs of `RELION <https://www3.mrc-lmb.cam.ac.uk/relion/index.php/Main_Page>`_ software suite.
+        This plugin provides wrappers for several programs of `RELION <https://relion.readthedocs.io/en/latest/index.html>`_ software suite.
         
         .. image:: https://img.shields.io/pypi/v/scipion-em-relion.svg
                 :target: https://pypi.python.org/pypi/scipion-em-relion
                 :alt: PyPI release
         
         .. image:: https://img.shields.io/pypi/l/scipion-em-relion.svg
                 :target: https://pypi.python.org/pypi/scipion-em-relion
@@ -34,15 +34,15 @@
                 :target: https://pypi.python.org/pypi/scipion-em-relion
                 :alt: Downloads
         
         
         **IMPORTANT NOTES!**
         
             1. If you have imported movies with a gain file in **DM4** format, you need to **flip the gain reference upside-down** in the motion correction protocol! (`bug details <https://github.com/I2PC/xmippCore/issues/39>`_)
-            2. If you have provided a gain reference or defects file during movie import or motion correction, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in this polishing protocol.
+            2. If you have provided a gain reference or defects file during movie import or motion correction and plan to run bayesian polishing, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in the polishing protocol.
             3. When importing EER movies, you should specify dose per single EER frame during import step. Pixel size should be the physical pixel size unless you plan to render EER on 8K grid. In the Motioncor protocol choose binning, EER fractionation and upsampling (default=1 is for 4K grid).
         
         Installation
         ------------
         
         You will need to use 3.0+ version of Scipion to be able to run these protocols. To install the plugin, you have two options:
         
@@ -54,58 +54,63 @@
         
         b) Developer's version
         
            * download repository
         
            .. code-block::
         
-              git clone https://github.com/scipion-em/scipion-em-relion.git
+              git clone -b devel https://github.com/scipion-em/scipion-em-relion.git
         
            * install
         
            .. code-block::
         
-              scipion installp -p path_to_scipion-em-relion --devel
+              scipion installp -p /path/to/scipion-em-relion --devel
         
-        - RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-4.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
-        - If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file.
+        - RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-5.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
+        - If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file. Optionally, you can also specify *RELION_CUDA_BIN* path for nvcc.
         - If you have to use a MPI for Relion different from Scipion MPI, you can set *RELION_MPI_BIN* and *RELION_MPI_LIB* variables in the config file.
-        - If you want to use **2D class ranker** protocol, you also need to set *RELION_PYTHON* that points to a Python which includes torch and numpy modules.
+        - To add support for Python modules (e.g. Blush, ModelAngelo and DynaMight) you will have to setup a Python environment with dependencies. You need to set *RELION_ENV_ACTIVATION* that points to a conda environment. Default = ``conda activate relion-5.0``
+        - You might want to set *TORCH_HOME* pointing to the path with downloaded models. Default = ``software/em/modelangelomodels-1.0`` (shared with ModelAngelo plugin).
+        - If you want to use SIDESPLITTER, you need the `sidesplitter <https://github.com/scipion-em/scipion-em-sidesplitter>`_ plugin installed and *SIDESPLITTER_HOME* set properly. After that, you only need to add *--external_reconstruct* into Additional arguments field of a 3D auto-refine or multi-body job.
         
         To check the installation, simply run one of the tests. A complete list of tests can be displayed by executing ``scipion test --show --grep relion``
         
         Supported versions
         ------------------
         
-        3.1.3, 4.0
+        4.0, 5.0
         
         Protocols
         ---------
         
         * 2D class ranker
         * 2D classification         
         * 3D auto-refine            
         * 3D classification         
         * 3D initial model          
         * 3D multi-body
         * assign optics groups
         * auto-picking (reference-based)
         * auto-picking LoG          
-        * bayesian polishing        
+        * bayesian polishing
+        * calculate fsc
         * center averages
         * clean project
         * compress movies
         * create 3d mask
         * crop / resize volumes
         * ctf refinement
+        * DynaMight flexibility
         * estimate gain to compress
         * expand symmetry
         * export coordinates
         * export ctf                
-        * export particles          
+        * export particles
+        * import coordinates
         * local resolution          
         * motion correction
         * particles extraction
         * post-processing           
         * preprocess particles      
         * reconstruct
         * remove preferential views
@@ -115,13 +120,14 @@
         References
         ----------
         
         1. Scheres et al., JMB, 2012 
         2. Scheres et al., JSB, 2012 
         3. Kimanius et al., eLife, 2016 
         4. Zivanov et al., eLife, 2018
+        5. Kimanius et al., Biochemical Journal, 2021
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-relion-4.0b8/README.rst` & `scipion-em-relion-5.0.0b1/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 =============
 Relion plugin
 =============
 
-This plugin provide wrappers around several programs of `RELION <https://www3.mrc-lmb.cam.ac.uk/relion/index.php/Main_Page>`_ software suite.
+This plugin provides wrappers for several programs of `RELION <https://relion.readthedocs.io/en/latest/index.html>`_ software suite.
 
 .. image:: https://img.shields.io/pypi/v/scipion-em-relion.svg
         :target: https://pypi.python.org/pypi/scipion-em-relion
         :alt: PyPI release
 
 .. image:: https://img.shields.io/pypi/l/scipion-em-relion.svg
         :target: https://pypi.python.org/pypi/scipion-em-relion
@@ -24,15 +24,15 @@
         :target: https://pypi.python.org/pypi/scipion-em-relion
         :alt: Downloads
 
 
 **IMPORTANT NOTES!**
 
     1. If you have imported movies with a gain file in **DM4** format, you need to **flip the gain reference upside-down** in the motion correction protocol! (`bug details <https://github.com/I2PC/xmippCore/issues/39>`_)
-    2. If you have provided a gain reference or defects file during movie import or motion correction, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in this polishing protocol.
+    2. If you have provided a gain reference or defects file during movie import or motion correction and plan to run bayesian polishing, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in the polishing protocol.
     3. When importing EER movies, you should specify dose per single EER frame during import step. Pixel size should be the physical pixel size unless you plan to render EER on 8K grid. In the Motioncor protocol choose binning, EER fractionation and upsampling (default=1 is for 4K grid).
 
 Installation
 ------------
 
 You will need to use 3.0+ version of Scipion to be able to run these protocols. To install the plugin, you have two options:
 
@@ -44,58 +44,63 @@
 
 b) Developer's version
 
    * download repository
 
    .. code-block::
 
-      git clone https://github.com/scipion-em/scipion-em-relion.git
+      git clone -b devel https://github.com/scipion-em/scipion-em-relion.git
 
    * install
 
    .. code-block::
 
-      scipion installp -p path_to_scipion-em-relion --devel
+      scipion installp -p /path/to/scipion-em-relion --devel
 
-- RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-4.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
-- If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file.
+- RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-5.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
+- If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file. Optionally, you can also specify *RELION_CUDA_BIN* path for nvcc.
 - If you have to use a MPI for Relion different from Scipion MPI, you can set *RELION_MPI_BIN* and *RELION_MPI_LIB* variables in the config file.
-- If you want to use **2D class ranker** protocol, you also need to set *RELION_PYTHON* that points to a Python which includes torch and numpy modules.
+- To add support for Python modules (e.g. Blush, ModelAngelo and DynaMight) you will have to setup a Python environment with dependencies. You need to set *RELION_ENV_ACTIVATION* that points to a conda environment. Default = ``conda activate relion-5.0``
+- You might want to set *TORCH_HOME* pointing to the path with downloaded models. Default = ``software/em/modelangelomodels-1.0`` (shared with ModelAngelo plugin).
+- If you want to use SIDESPLITTER, you need the `sidesplitter <https://github.com/scipion-em/scipion-em-sidesplitter>`_ plugin installed and *SIDESPLITTER_HOME* set properly. After that, you only need to add *--external_reconstruct* into Additional arguments field of a 3D auto-refine or multi-body job.
 
 To check the installation, simply run one of the tests. A complete list of tests can be displayed by executing ``scipion test --show --grep relion``
 
 Supported versions
 ------------------
 
-3.1.3, 4.0
+4.0, 5.0
 
 Protocols
 ---------
 
 * 2D class ranker
 * 2D classification         
 * 3D auto-refine            
 * 3D classification         
 * 3D initial model          
 * 3D multi-body
 * assign optics groups
 * auto-picking (reference-based)
 * auto-picking LoG          
-* bayesian polishing        
+* bayesian polishing
+* calculate fsc
 * center averages
 * clean project
 * compress movies
 * create 3d mask
 * crop / resize volumes
 * ctf refinement
+* DynaMight flexibility
 * estimate gain to compress
 * expand symmetry
 * export coordinates
 * export ctf                
-* export particles          
+* export particles
+* import coordinates
 * local resolution          
 * motion correction
 * particles extraction
 * post-processing           
 * preprocess particles      
 * reconstruct
 * remove preferential views
@@ -105,7 +110,8 @@
 References
 ----------
 
 1. Scheres et al., JMB, 2012 
 2. Scheres et al., JSB, 2012 
 3. Kimanius et al., eLife, 2016 
 4. Zivanov et al., eLife, 2018
+5. Kimanius et al., Biochemical Journal, 2021
```

### Comparing `scipion-em-relion-4.0b8/relion/bibtex.py` & `scipion-em-relion-5.0.0b1/relion/bibtex.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,99 +29,132 @@
 @article{Scheres2012a,
 title = "A Bayesian View on Cryo-EM Structure Determination ",
 journal = "JMB",
 volume = "415",
 number = "2",
 pages = "406 - 418",
 year = "2012",
-doi = "http://dx.doi.org/10.1016/j.jmb.2011.11.010",
-url = "http://www.sciencedirect.com/science/article/pii/S0022283611012290",
+doi = "https://dx.doi.org/10.1016/j.jmb.2011.11.010",
+url = "https://www.sciencedirect.com/science/article/pii/S0022283611012290",
 author = "Scheres, Sjors H.W.",
 }
 
 @article{Scheres2012b,
 title = "RELION: Implementation of a Bayesian approach to cryo-EM structure determination ",
 journal = "JSB",
 volume = "180",
 number = "3",
 pages = "519 - 530",
 year = "2012",
-doi = "http://dx.doi.org/10.1016/j.jsb.2012.09.006",
-url = "http://www.sciencedirect.com/science/article/pii/S1047847712002481",
+doi = "https://dx.doi.org/10.1016/j.jsb.2012.09.006",
+url = "https://www.sciencedirect.com/science/article/pii/S1047847712002481",
 author = "Scheres, Sjors H.W.",
 }
 
 @article{Kimanius2016,
 title = "Accelerated cryo-EM structure determination with parallelisation using GPUs in RELION-2",
 journal = "eLife",
 volume = "5",
 pages = "e18722",
 year = "2016",
-doi = "http://dx.doi.org/10.7554/eLife.18722",
+doi = "https://dx.doi.org/10.7554/eLife.18722",
 author = "Kimanius, Dari and Forsberg, Björn O. and Scheres, Sjors H.W. and Lindahl, Erik",
 }
 
 @article{Scheres2015,
 title = "Semi-automated selection of cryo-EM particles in RELION-1.3",
 journal = "JSB",
 volume = "189",
 issue = "2",
 pages = "114-122",
 year = "2015",
-doi = "http://dx.doi.org/10.1016/j.jsb.2014.11.010",
+doi = "https://dx.doi.org/10.1016/j.jsb.2014.11.010",
 author = "Scheres, Sjors H.W.",
 }
 
 @article{Chen2012,
 title = "Prevention of overfitting in cryo-EM structure determination",
 journal = "Nat. Meth.",
 volume = "9",
 number = "3",
 pages = "853 - 854",
 year = "2012",
-doi = "http://dx.doi.org/10.1038/nmeth.2115",
+doi = "https://dx.doi.org/10.1038/nmeth.2115",
 author = "Chen, Shaoxia and Scheres, Sjors H.W.",
 }
 
 @article{Chen2013,
 title = "High-resolution noise substitution to measure overfitting and validate resolution in 3D structure determination by single particle electron cryomicroscopy.",
 journal = "JSB",
 volume = "135",
 number = "3",
 pages = "24-35",
 year = "2013",
-doi = "http://dx.doi.org/10.1016/j.ultramic.2013.06.004",
+doi = "https://dx.doi.org/10.1016/j.ultramic.2013.06.004",
 author = "Chen, Shaoxia and McMullan, Greg and Faruqi, Abdul R. and Murshudov, Garib N. and Short, Judith M. and Scheres, Sjors H.W. and Henderson, Richard",
 }
 
 @article{Zivanov2018,
 title = "New tools for automated high-resolution cryo-EM structure determination in RELION-3",
 journal = "eLife",
 volume = "7",
 pages = "e42166",
 year = "2018",
-doi = "http://dx.doi.org/10.7554/eLife.42166",
+doi = "https://dx.doi.org/10.7554/eLife.42166",
 author = "Zivanov, Jasenko and Nakane, Takanori and Forsberg, Björn O and Kimanius, Dari and Hagen, Wim JH and Lindahl, Erik and Scheres, Sjors H.W.",
 }
 
 @article{Nakane2018,
 title = "Characterisation of molecular motions in cryo-EM single-particle data by multi-body refinement in RELION",
 journal = "eLife",
 volume = "7",
 pages = "e36861",
 year = "2018",
-doi = "http://dx.doi.org/10.7554/eLife.36861",
+doi = "https://dx.doi.org/10.7554/eLife.36861",
 author = "Nakane, Takanori and Kimanius, Dari and Lindahl, Erik and Scheres, Sjors H.W.",
 }
 
 @article{Zivanov2019,
 author = "Zivanov, Jasenko and Nakane, Takanori and Scheres, Sjors H. W.",
 title = "A Bayesian approach to beam-induced motion correction in cryo-EM single-particle analysis",
 journal = "IUCrJ",
 year = "2019",
 volume = "6",
 number = "1",
 pages = "5-17",
-doi = {http://dx.doi.org/10.1107/S205225251801463X},
+doi = {https://dx.doi.org/10.1107/S205225251801463X},
 }
 
+@article{Kimanius2021,
+author = {Kimanius, Dari and Dong, Liyi and Sharov, Grigory and Nakane, Takanori and Scheres, Sjors H. W.},
+title = "{New tools for automated cryo-EM single-particle analysis in RELION-4.0}",
+journal = {Biochemical Journal},
+volume = {478},
+number = {24},
+pages = {4169-4185},
+year = {2021},
+month = {12},
+doi = {https://dx.doi.org/10.1042/BCJ20210708},
+}
+
+@article{Amunts2014,
+author = {Alexey Amunts  and Alan Brown  and Xiao-chen Bai and Jose L. Llacer  and Tanweer Hussain  and Paul Emsley  and Fei Long  and Garib Murshudov  and Sjors H. W. Scheres  and V. Ramakrishnan },
+title = {Structure of the Yeast Mitochondrial Large Ribosomal Subunit},
+journal = {Science},
+volume = {343},
+number = {6178},
+pages = {1485-1489},
+year = {2014},
+doi = {https://dx.doi.org/10.1126/science.1249410}
+}
+
+@article {Schwab2023,
+author = {Johannes Schwab and Dari Kimanius and Alister Burt and Tom Dendooven and Sjors H.W. Scheres},
+title = {DynaMight: estimating molecular motions with improved reconstruction from cryo-EM images},
+year = {2023},
+doi = {https://dx.doi.org/10.1101/2023.10.18.562877},
+publisher = {Cold Spring Harbor Laboratory},
+journal = {bioRxiv}
+}
+
+
 """
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/__init__.py` & `scipion-em-relion-5.0.0b1/relion/convert/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,16 @@
         self._loadClassesInfo(iteration)
 
         dataStar = prot._getFileName('data', iter=iteration)
         pixelSize = prot.inputParticles.get().getSamplingRate()
         self._reader = createReader(alignType=self._alignType,
                                     pixelSize=pixelSize)
 
-        mdIter = Table.iterRows('particles@' + dataStar, key='rlnImageId')
+        mdIter = Table.iterRows('particles@' + dataStar, key='rlnImageId',
+                                types=LABELS_DICT)
         clsSet.classifyItems(updateItemCallback=self._updateParticle,
                              updateClassCallback=self._updateClass,
                              itemDataIterator=mdIter,
                              doClone=False)
 
     def _updateParticle(self, item, row):
         item.setClassId(row.rlnClassNumber)
@@ -143,15 +144,15 @@
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesInfo:
             index, fn, row = self._classesInfo[classId]
             item.setAlignment(self._alignType)
             if self._alignType == ALIGN_PROJ:
-                fn += ':mrc'  # mark reference as a MRC volume
+                fn += ':mrc'  # FIXME: mark reference as a MRC volume
             item.getRepresentative().setLocation(index, fn)
             item._rlnClassDistribution = Float(row.rlnClassDistribution)
             item._rlnAccuracyRotations = Float(row.rlnAccuracyRotations)
             item._rlnAccuracyTranslationsAngst = Float(row.rlnAccuracyTranslationsAngst)
 
 
 class DefocusGroups:
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert30.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert30.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert31.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert31.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,24 +30,24 @@
 """
 import os
 import io
 import numpy as np
 from collections import OrderedDict
 from emtable import Table
 
-
+import pyworkflow.utils as pwutils
 from pwem.constants import ALIGN_NONE, ALIGN_PROJ, ALIGN_2D, ALIGN_3D
 from pwem.objects import (Micrograph, SetOfMicrographsBase, SetOfMovies,
                           Particle, CTFModel, Acquisition, Transform, Coordinate)
 import pwem.convert.transformations as tfs
 
 from .convert_base import WriterBase, ReaderBase
 from .convert_utils import (convertBinaryFiles, locationToRelion,
                             relionToLocation)
-from relion.constants import PARTICLE_EXTRA_LABELS
+from relion.constants import PARTICLE_EXTRA_LABELS, LABELS_DICT
 
 
 def getPixelSizeLabel(imageSet):
     """ Return the proper label for pixel size. """
     if (isinstance(imageSet, SetOfMicrographsBase)
             or isinstance(imageSet, Micrograph)):
         return 'rlnMicrographPixelSize'
@@ -387,16 +387,18 @@
 
         # Convert binaries if required
         if self.outputStack:
             self._relOutputStack = os.path.relpath(self.outputStack,
                                                    os.path.dirname(starFile))
         if self.outputDir is not None:
             forceConvert = kwargs.get('forceConvert', False)
+            incompatibleExtensions = kwargs.get('incompatibleExtensions', None)
             self._filesDict = convertBinaryFiles(partsSet, self.outputDir,
-                                                 forceConvert=forceConvert)
+                                                 forceConvert=forceConvert,
+                                                 incompatibleExtensions=incompatibleExtensions)
 
         # Compute some flags from the first particle...
         # when flags are True, some operations will be applied to all particles
         self._preprocessImageRow = kwargs.get('preprocessImageRow', None)
 
         self._setCtf = kwargs.get('writeCtf', True) and firstPart.hasCTF()
 
@@ -519,15 +521,16 @@
 
         self._optics = OpticsGroups.fromStar(starFile)
 
         self._pixelSize = getattr(self._optics.first(),
                                   'rlnImagePixelSize', 1.0)
         self._invPixelSize = 1. / self._pixelSize
 
-        partsReader = Table.Reader(starFile, tableName='particles')
+        partsReader = Table.Reader(starFile, tableName='particles',
+                                   types=LABELS_DICT)
 
         firstRow = partsReader.getRow()
         self._setClassId = hasattr(firstRow, 'rlnClassNumber')
         self._setCtf = partsReader.hasAllColumns(self.CTF_LABELS[:3])
         self._setCoord = partsReader.hasAllColumns(self.COORD_LABELS[:3])
         particle = Particle()
 
@@ -584,29 +587,85 @@
             self.rowToCtf(row, particle.getCTF())
 
         self.setParticleTransform(particle, row)
         self.setExtraLabels(particle, row)
 
         # TODO: coord extra labels, partId, micId,
         if self._setCoord:
-            coord = self.rowToCoord(row)
+            coord = Coordinate()
+            self.rowToCoord(row, coord)
             particle.setCoordinate(coord)
 
         if self._postprocessImageRow:
             self._postprocessImageRow(particle, row)
 
+    def readSetOfCoordinates(self, starFile, coordSet, micList=None, **kwargs):
+        """ Convert a star file into a set of coordinates.
+
+        Params:
+            starFile: the filename of the star file
+            coordSet: output coordinates set
+            micList: list of micNames to match coordSet
+
+        Keyword Arguments:
+            postprocessCoordRow:
+            extraLabels:
+
+        """
+        self._postprocessCoordRow = kwargs.get('postprocessCoordRow', None)
+        coordsReader = Table.Reader(starFile, types=LABELS_DICT)
+        if coordsReader.hasColumn('rlnOpticsGroup'):
+            coordsReader = Table.Reader(starFile, tableName='particles', types=LABELS_DICT)
+
+        if not coordsReader.hasAllColumns(self.COORD_LABELS[:3]):
+            raise RuntimeError("STAR file should include columns: ", self.COORD_LABELS[:3])
+
+        coordsReader = sorted(coordsReader, key=lambda r: getattr(r, 'rlnMicrographName'))
+        coordsReader = [row for row in coordsReader if pwutils.removeExt(os.path.basename(row.rlnMicrographName)) in micList]
+        if not len(coordsReader):
+            raise RuntimeError("Could not match micNames between micrographs and star file!")
+
+        firstRow = coordsReader[0]
+        hasMicId = hasattr(firstRow, 'rlnMicrographId')
+
+        coord = Coordinate()
+        self.rowToCoord(firstRow, coord)
+        if hasMicId:
+            coord.setMicId(firstRow.rlnMicrographId)
+        else:
+            coord.setMicId(1)
+
+        extraLabels = kwargs.get('extraLabels', []) + self.COORD_LABELS[3:]
+        self.createExtraLabels(coord, firstRow, extraLabels)
+        if self._postprocessCoordRow:
+            self._postprocessCoordRow(coord, firstRow)
+        coordSet.append(coord)
+
+        objId = 1
+        for row in coordsReader[1:]:
+            objId += 1
+            self.rowToCoord(row, coord)
+            coord.setObjId(objId)
+            if hasMicId:
+                coord.setMicId(row.rlnMicrographId)
+            else:
+                micId = micList.index(pwutils.removeExt(os.path.basename(row.rlnMicrographName))) + 1
+                coord.setMicId(micId)
+            self.setExtraLabels(coord, row)
+            if self._postprocessCoordRow:
+                self._postprocessCoordRow(coord, row)
+
+            coordSet.append(coord)
+
     @staticmethod
-    def rowToCoord(row):
+    def rowToCoord(row, coord):
         """ Create a Coordinate from the row. """
-        coord = Coordinate()
         coord.setPosition(row.rlnCoordinateX,
                           row.rlnCoordinateY)
-        coord.setMicName(row.rlnMicrographName)
-
-        return coord
+        coord.setMicName(pwutils.removeExt(os.path.basename(row.rlnMicrographName)))
 
     @staticmethod
     def rowToCtf(row, ctf):
         """ Create a CTFModel from the row. """
         ctf.setDefocusU(row.rlnDefocusU)
         ctf.setDefocusV(row.rlnDefocusV)
         ctf.setDefocusAngle(row.rlnDefocusAngle)
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert_base.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,23 +65,23 @@
         # Not used now
         # self.convertPolicy = kwargs.get('convertPolicy', self.CONVERT_IF_NEEDED)
         self.rootDir = None
         self.outputDir = None
         self.outputStack = None
         self.useBaseName = False
         self.extensions = ['mrc']
-        self.update(['rootDir', 'outputDir', 'userBaseName', 'extensions'],
+        self.update(['rootDir', 'outputDir', 'useBaseName', 'extensions'],
                     **kwargs)
         self._ih = ImageHandler()  # used to convert images
         self._filesDict = {}  # used to map file names (converted or linked)
         self._dimensionality = 2
         self._imageSize = None
 
     def update(self, attrsList, **kwargs):
-        """ Update the some attributes with values from kwargs. """
+        """ Update some attributes with values from kwargs. """
         for attr in attrsList:
             if attr in kwargs:
                 setattr(self, attr, kwargs[attr])
 
     def writeSetOfMovies(self, moviesIterable, starFile, **kwargs):
         pass
 
@@ -190,14 +190,28 @@
             blockName: The name of the data block (default particles)
             alignType:
             removeDisabled:
 
         """
         pass
 
+    def readSetOfCoordinates(self, starFile, coordSet, micList=None, **kwargs):
+        """ Convert a star file into a set of coordinates.
+
+        Params:
+            starFile: the filename of the star file
+            coordSet: output coordinates set
+            micList: list of micrographs to match coordSet
+
+        Keyword Arguments:
+            postprocessCoordRow:
+
+        """
+        pass
+
     def setParticleTransform(self, particle, row):
         """ Set the transform values from the row. """
         pass
 
     def createExtraLabels(self, item, row, extraLabels):
         """ Create new Objects for each extra label if contained in
         the columnObj. It will set the self._extraLabels property.
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert_coordinates.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert_coordinates.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 """
 Utility functions for conversions that will be used from both
 newer Relion3.1 routines and old ones.
 """
 
 import os
 from emtable import Table
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.utils as pwutils
 from pwem.constants import NO_INDEX
 
 
 def openStar(fn, extraLabels=False):
     # We are going to write metadata directly to file to do it faster
@@ -82,15 +84,15 @@
     doScale = abs(scale - 1) > 0.001
 
     for coord in coordSet.iterItems(orderBy='_micId'):
         micId = coord.getMicId()
 
         if micId != lastMicId:
             if micId not in posDict:
-                print("Warning: micId %s not found" % micId)
+                logger.warning(f"Warning: micId {micId} not found")
                 continue
             # we need to close previous opened file
             if f:
                 f.close()
             f = openStar(posDict[micId], extraLabels)
             lastMicId = micId
 
@@ -173,15 +175,15 @@
     """ Write the config.xmd file needed for Xmipp picker.
     Params:
         configFn: The filename were to store the configuration.
         boxSize: the box size in pixels for extraction.
         state: picker state
     """
     # Write config.xmd metadata
-    print("writeCoordsConfig: state=", state)
+    logger.debug(f"writeCoordsConfig: state={state}")
     table = Table(columns=['particleSize', 'pickingState'])
     table.addRow(int(boxSize), state)
     table.write(configFn, tableName='properties')
 
 
 def openMd(fn, state='Manual'):
     # We are going to write metadata directly to file to do it faster
@@ -217,15 +219,15 @@
         isManual: if the coordinates are 'Manual' or 'Supervised'
         getPosFunc: a function to get the positions from the coordinate,
             it can be useful for scaling the coordinates if needed.
     """
     if getPosFunc is None:
         getPosFunc = lambda coord: coord.getPosition()
 
-    extraLabels = coordList[0].hasAttribute('_rlnClassNumber')
+    extraLabels = coordList[0].hasAttribute('_rlnAutopickFigureOfMerit')
     f = openStar(outputFn, extraLabels)
 
     for coord in coordList:
         x, y = getPosFunc(coord)
         if not extraLabels:
             f.write("%d %d \n" % (x, y))
         else:
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert_deprecated.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert_deprecated.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from os.path import basename
 import numpy as np
+import logging
+logger = logging.getLogger(__name__)
 
 from pyworkflow.object import ObjectWrap, String, Integer
 from pwem.constants import ALIGN_2D, ALIGN_3D, ALIGN_PROJ, ALIGN_NONE
 import pwem.convert.transformations as tfs
 import pwem.objects as pwobj
 
 from relion.constants import *
@@ -199,15 +201,15 @@
 
     if is2D:
         angle = angles[0] + angles[2]
         alignmentRow.set(md.RLN_ORIENT_PSI, -angle)
 
         flip = bool(np.linalg.det(matrix[0:2, 0:2]) < 0)
         if flip:
-            print("FLIP in 2D not implemented")
+            logger.error("FLIP in 2D not implemented")
     elif is3D:
         raise Exception("3D alignment conversion for Relion not implemented. "
                         "It seems the particles were generated with an "
                         "incorrect alignment type. You may either re-launch "
                         "the protocol that generates the particles "
                         "with angles or set 'Consider previous alignment?' "
                         "to No")
@@ -298,20 +300,20 @@
     """
     if micList is None:
         micList = coordSet.getMicrographs()
 
     for mic, coordFn in zip(micList, coordFiles):
 
         if not os.path.exists(coordFn):
-            print("WARNING: Missing coordinates star file: ", coordFn)
+            logger.warning(f"WARNING: Missing coordinates star file: {coordFn}")
 
         try:
             readCoordinates(mic, coordFn, coordSet)
         except Exception:
-            print("WARNING: Error reading coordinates star file: ", coordFn)
+            logger.warning(f"WARNING: Error reading coordinates star file: {coordFn}")
 
 
 def readCoordinates(mic, fileName, coordsSet):
     for row in md.iterRows(fileName):
         coord = rowToCoordinate(row)
         coord.setX(coord.getX())
         coord.setY(coord.getY())
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/convert_utils.py` & `scipion-em-relion-5.0.0b1/relion/convert/convert_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 Utility functions for conversions that will be used from both
 newer Relion3.1 routines and old ones.
 """
 
 import os
 import math
 from emtable import Table
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.utils as pwutils
 from pwem.constants import NO_INDEX
 from pwem.emlib.image import ImageHandler
 
 from relion import Plugin
 
@@ -57,35 +59,40 @@
     if '@' in filename:
         indexStr, fn = filename.split('@')
         return int(indexStr), str(fn)
     else:
         return NO_INDEX, str(filename)
 
 
-def convertBinaryFiles(imgSet, outputDir, extension='mrcs', forceConvert=False):
+def convertBinaryFiles(imgSet, outputDir, extension='mrcs', forceConvert=False,
+                       incompatibleExtensions=None):
     """ Convert binary images files to a format read by Relion.
     Or create links if there is no need to convert the binary files.
 
     Params:
         imgSet: input image set to be converted.
         outputDir: where to put the converted file(s)
         extension: extension accepted by the program
         forceConvert: if True, the files will be converted and no root will be used
+        incompatibleExtensions: list of incompatible extension
     Return:
         A dictionary with old-file as key and new-file as value
         If empty, not conversion was done.
     """
     filesDict = {}
     ih = ImageHandler()
     outputRoot = outputDir if forceConvert else os.path.join(outputDir, 'input')
     # Get the extension without the dot
     stackFiles = imgSet.getFiles()
     ext = pwutils.getExt(next(iter(stackFiles)))[1:]
     rootDir = pwutils.commonPath(list(stackFiles))
 
+    if incompatibleExtensions is None:
+        incompatibleExtensions = ['hdf']
+
     def getUniqueFileName(fn, extension):
         """ Get an unique file for either link or convert files.
         It is possible that the base name overlap if they come
         from different runs. (like particles.mrcs after relion preprocess)
         """
         newFn = os.path.join(outputRoot, pwutils.replaceBaseExt(fn, extension))
         newRoot = pwutils.removeExt(newFn)
@@ -102,46 +109,45 @@
     def createBinaryLink(fn):
         """ Just create a link named .mrcs to Relion understand
         that it is a binary stack file and not a volume.
         """
         newFn = getUniqueFileName(fn, extension)
         if not os.path.exists(newFn):
             pwutils.createLink(fn, newFn)
-            print("   %s -> %s" % (newFn, fn))
+            logger.info(f"\t{newFn} -> {fn}")
         return newFn
 
     def convertStack(fn):
         """ Convert from a format that is not read by Relion
         to an spider stack.
         """
         newFn = getUniqueFileName(fn, 'mrcs')
         ih.convertStack(fn, newFn)
-        print("   %s -> %s" % (newFn, fn))
+        logger.info(f"\t{newFn} -> {fn}")
         return newFn
 
     def replaceRoot(fn):
         """ Link create to the root folder, so just replace that
         in the name, no need to do anything else.
         """
         return fn.replace(rootDir, outputRoot)
 
     if forceConvert:
-        print("convertBinaryFiles: forceConvert = True")
+        logger.debug("convertBinaryFiles: forceConvert = True")
         mapFunc = convertStack
     elif ext == extension:
-        print("convertBinaryFiles: creating soft links.")
-        print("   Root: %s -> %s" % (outputRoot, rootDir))
+        logger.debug(f"convertBinaryFiles: creating soft links."
+                     f"\tRoot: {outputRoot} -> {rootDir}")
         mapFunc = replaceRoot
         pwutils.createAbsLink(os.path.abspath(rootDir), outputRoot)
     elif ext == 'mrc' and extension == 'mrcs':
-        print("convertBinaryFiles: creating soft links (mrcs -> mrc).")
+        logger.debug("convertBinaryFiles: creating soft links (mrcs -> mrc).")
         mapFunc = createBinaryLink
-    elif ext.endswith('hdf'):  # assume eman .hdf format
-        print("convertBinaryFiles: converting stacks. (%s -> %s)"
-              % (extension, ext))
+    elif ext in incompatibleExtensions:  # assume eman .hdf or any incompatible format
+        logger.debug(f"convertBinaryFiles: converting stacks ({extension} -> {ext})")
         mapFunc = convertStack
     else:
         mapFunc = None
 
     if mapFunc is not None:
         pwutils.makePath(outputRoot)
         for fn in stackFiles:
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/dataimport.py` & `scipion-em-relion-5.0.0b1/relion/convert/dataimport.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 from collections import OrderedDict
 from emtable import Table
+import logging
+logger = logging.getLogger(__name__)
 
 from pyworkflow.object import Float
 from pwem.constants import ALIGN_PROJ, ALIGN_2D, ALIGN_NONE
 from pwem.objects import Micrograph
 import pwem.emlib.metadata as md
 import pyworkflow.utils as pwutils
 
@@ -126,15 +128,15 @@
         if self._classesFunc is not None:
             self._createClasses(partSet)
 
     def _updateClass(self, item):
         classId = item.getObjId()
         if classId in self._classesDict:
             index, fn, row = self._classesDict[classId]
-            if fn.endswith('.mrc'):
+            if fn.endswith('.mrc'):  # FIXME
                 fn += ':mrc'  # Specify that are volumes to read them properly in xmipp
             item.getRepresentative().setLocation(index, fn)
             item._rlnclassDistribution = Float(row.get('rlnClassDistribution'))
             item._rlnAccuracyRotations = Float(row.get('rlnAccuracyRotations'))
             if self.version30:
                 accInAngst = row.get('rlnAccuracyTranslations') * self._pixelSize
                 item._rlnAccuracyTranslationsAngst = Float(accInAngst)
@@ -202,57 +204,50 @@
 
     def _findImagesPath(self, label, warnings=True):
         # read the first table
         table = Table(fileName=self._starFile)
         acqRow = row = table[0]
 
         if row is None:
-            raise Exception("Cannot import from empty metadata: %s"
-                            % self._starFile)
+            raise ValueError("Cannot import from empty metadata: %s"
+                             % self._starFile)
 
         if not row.get('rlnOpticsGroup', False):
             self.version30 = True
             self.protocol.warning("Import from Relion version < 3.1 ...")
         else:
             acqRow = OpticsGroups.fromStar(self._starFile).first()
             # read particles table
             table = Table(fileName=self._starFile, tableName='particles')
             row = table[0]
 
         if not row.get(label, False):
-            raise Exception("Label *%s* is missing in metadata: %s"
-                            % (label, self._starFile))
+            raise ValueError("Label *%s* is missing in metadata: %s"
+                             % (label, self._starFile))
 
-        index, fn = relionToLocation(row.get(label))
+        _, fn = relionToLocation(row.get(label))
         # Relion does not allow abs paths
         if fn.startswith("/"):
-            raise Exception("ERROR: %s cannot be an absolute path: %s\n"
-                            "Please create a symlink to an abs path instead."
-                            % (label, fn))
+            raise ValueError("ERROR: %s cannot be an absolute path: %s\n"
+                             "Please create a symlink to an abs path instead."
+                             % (label, fn))
         self._imgPath = pwutils.findRootFrom(self._starFile, fn)
 
         if warnings and self._imgPath is None:
             self.protocol.warning("Binary data was not found from metadata: %s"
                                   % self._starFile)
 
         if (self._starFile.endswith('_data.star') and
                 self._getModelFile(self._starFile)):
             self._modelStarFile = self._getModelFile(self._starFile)
             modelRow = Table(fileName=self._modelStarFile,
                              tableName='model_general')[0]
             classDimensionality = int(modelRow.rlnReferenceDimensionality)
-            self._optimiserFile = self._starFile.replace('_data.star',
-                                                         '_optimiser.star')
-            if not os.path.exists(self._optimiserFile):
-                autoRefine = int(modelRow.rlnNrClasses) == 1
-            else:
-                optimiserRow = Table(fileName=self._optimiserFile,
-                                     tableName='optimiser_general')[0]
-                autoRefine = optimiserRow.get('rlnModelStarFile2', False)
-
+            autoRefine = (int(modelRow.rlnNrClasses) == 1 and
+                          modelRow.rlnTau2FudgeFactor == 1.0)
             self.alignType = ALIGN_PROJ
 
             if not autoRefine:
                 if classDimensionality == 3:
                     self._classesFunc = self.protocol._createSetOfClasses3D
                 else:
                     self._classesFunc = self.protocol._createSetOfClasses2D
@@ -271,15 +266,15 @@
                 self.alignType = ALIGN_PROJ
             elif (row.get('rlnAnglePsi', False) and
                   float(row.rlnAnglePsi) != 0.0):
                 self.alignType = ALIGN_2D
             else:
                 self.alignType = ALIGN_NONE
 
-        print("alignType: ", self.alignType)
+        logger.debug(f"alignType: {self.alignType}")
             
         # Check if the MetaData contains either rlnMicrographName
         # or rlnMicrographId, this will be used when imported
         # particles to keep track of the particle's micrograph
         self._micIdOrName = (row.get('rlnMicrographName', False) or
                              row.get('rlnMicrographId', False))
         # init dictionary. It will be used in the preprocessing
@@ -399,30 +394,30 @@
         """ Return a dictionary with acquisition values and 
         the sampling rate information.
         In the case of Relion, they are stored in the optics table
         """
         acquisitionDict = OrderedDict()
 
         try:
-            _, modelRow, acqRow = self._findImagesPath('rlnImageName', warnings=False)
+            _, _, acqRow = self._findImagesPath('rlnImageName', warnings=False)
 
             if acqRow.get('rlnVoltage', False):
                 acquisitionDict['voltage'] = acqRow.rlnVoltage
 
             if acqRow.get('rlnAmplitudeContrast', False):
                 acquisitionDict['amplitudeContrast'] = acqRow.rlnAmplitudeContrast
 
             if acqRow.get('rlnSphericalAberration', False):
                 acquisitionDict['sphericalAberration'] = acqRow.rlnSphericalAberration
 
-            if modelRow is not None and modelRow.get('rlnPixelSize', False):
-                acquisitionDict['samplingRate'] = modelRow.rlnPixelSize
+            if acqRow.get('rlnImagePixelSize', False):
+                acquisitionDict['samplingRate'] = acqRow.rlnImagePixelSize
 
         except Exception as ex:
-            print("Error loading acquisition: ", str(ex))
+            logger.error(f"Error loading acquisition: {str(ex)}")
 
         return acquisitionDict
 
     def importCoordinates(self, fileName, addCoordinate):
         from .convert_deprecated import rowToCoordinate
         for row in md.iterRows(fileName):
             coord = rowToCoordinate(row)
```

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_de20_300.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_de20_300.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f2_300.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f2_300.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f3_200_ec.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f3_200_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f3_300_ec.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f3_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f4_200_ec.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f4_200_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_f4_300_ec.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_f4_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/convert/mtfs/mtf_k2_300_ec.star` & `scipion-em-relion-5.0.0b1/relion/convert/mtfs/mtf_k2_300_ec.star`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/objects.py` & `scipion-em-relion-5.0.0b1/relion/objects.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/protocols/__init__.py` & `scipion-em-relion-5.0.0b1/relion/protocols/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,43 +19,45 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+
 from relion import Plugin
 
 from .protocol_assign_optic_groups import ProtRelionAssignOpticsGroup
 from .protocol_autopick_log import ProtRelionAutopickLoG
 from .protocol_autopick_ref import ProtRelion2Autopick
 from .protocol_bayesian_polishing import ProtRelionBayesianPolishing
+from .protocol_calculate_fsc import ProtRelionCalculateFSC
 from .protocol_center_averages import ProtRelionCenterAverages
 from .protocol_classify2d import ProtRelionClassify2D
 from .protocol_classify3d import ProtRelionClassify3D
 from .protocol_estimate_gain import ProtRelionCompressEstimateGain
 from .protocol_compress_movies import ProtRelionCompressMovies
 from .protocol_create_mask3d import ProtRelionCreateMask3D
 from .protocol_crop_resize import ProtRelionResizeVolume
 from .protocol_ctf_refinement import ProtRelionCtfRefinement
 from .protocol_expand_symmetry import ProtRelionExpandSymmetry
 from .protocol_export_coords import ProtRelionExportCoordinates
 from .protocol_export_ctf import ProtRelionExportCtf
 from .protocol_export_particles import ProtRelionExportParticles
 from .protocol_extract_particles import ProtRelionExtractParticles
 from .protocol_gentle_clean import ProtRelionCleanJobs
+from .protocol_import_coords import ProtRelionImportCoords
+from .protocol_initialmodel import ProtRelionInitialModel
 from .protocol_localres import ProtRelionLocalRes
 from .protocol_motioncor import ProtRelionMotioncor
 from .protocol_multibody import ProtRelionMultiBody
 from .protocol_postprocess import ProtRelionPostprocess
 from .protocol_preprocess import ProtRelionPreprocessParticles
 from .protocol_reconstruct import ProtRelionReconstruct
 from .protocol_refine3d import ProtRelionRefine3D
 from .protocol_remove_views import ProtRelionRemovePrefViews
+from .protocol_select_classes import ProtRelionSelectClasses2D
 from .protocol_subtract import ProtRelionSubtract
 from .protocol_symmetrize_volume import ProtRelionSymmetrizeVolume
 
-if Plugin.IS_GT31():
-    from .protocol_select_classes import ProtRelionSelectClasses2D
-    from .protocol_initialmodel import ProtRelionInitialModel
-else:
-    from ._legacy.protocol31_initialmodel import ProtRelionInitialModel
+#if Plugin.IS_GT50():
+#    from .protocol_dynamight import ProtRelionDynaMight
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/_legacy/protocol31_initialmodel.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_initialmodel.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,44 +25,49 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 from emtable import Table
 
 from pwem.constants import ALIGN_PROJ
 from pwem.protocols import ProtInitialVolume
-from pwem.objects import Volume
+from pwem.objects import Volume, SetOfVolumes, SetOfParticles
+from pyworkflow.constants import PROD
 from pyworkflow.protocol.params import (PointerParam, FloatParam,
                                         LabelParam, IntParam,
-                                        EnumParam, StringParam,
-                                        BooleanParam,
-                                        LEVEL_ADVANCED)
+                                        StringParam, BooleanParam)
 
-import relion
 import relion.convert as convert
-from ..protocol_base import ProtRelionBase
+from .protocol_base import ProtRelionBase
 
 
 class ProtRelionInitialModel(ProtInitialVolume, ProtRelionBase):
     """ This protocols creates a 3D initial model using Relion.
 
     Generate a 3D initial model _de novo_ from 2D particles using
     Relion Stochastic Gradient Descent (SGD) algorithm.
     """
     _label = '3D initial model'
+    _devStatus = PROD
+    _possibleOutputs = {
+        "outputVolume": Volume,
+        "outputVolumeSymmetrized": Volume,
+        "outputVolumes": SetOfVolumes,
+        "outputParticles": SetOfParticles
+    }
     IS_CLASSIFY = False
     IS_3D_INIT = True
     IS_2D = False
     CHANGE_LABELS = ['rlnChangesOptimalOrientations',
                      'rlnChangesOptimalOffsets']
 
     def __init__(self, **args):
         ProtRelionBase.__init__(self, **args)
 
     def _initialize(self):
-        """ This function is mean to be called after the
+        """ This function is meant to be called after the
         working dir for the protocol have been set.
         (maybe after recovery from mapper)
         """
         self._createFilenameTemplates()
         self._createIterTemplates()
         if not self.doContinue:
             self.continueRun.set(None)
@@ -163,14 +168,32 @@
                       label='minimum size for defocus group',
                       condition='doCtfManualGroups and not doContinue',
                       help='If defocus group is smaller than this value, '
                            'it will be expanded until number of particles '
                            'per defocus group is reached')
 
         form.addSection('Optimisation')
+        form.addParam('numberOfIter', IntParam, default=200,
+                      label="Number of VDAM mini-batches",
+                      help="How many iterations (i.e. mini-batches) "
+                           "to perform with the VDAM algorithm?")
+        form.addParam('regularisationParamT', FloatParam,
+                      default=4,
+                      label='Regularisation parameter T',
+                      help='Bayes law strictly determines the relative '
+                           'weight between the contribution of the '
+                           'experimental data and the prior. '
+                           'However, in practice one may need to adjust '
+                           'this weight to put slightly more weight on the '
+                           'experimental data to allow optimal results. '
+                           'Values greater than 1 for this regularisation '
+                           'parameter (T in the JMB2011 paper) put more '
+                           'weight on the experimental data. Values around '
+                           '2-4 have been observed to be useful for 3D '
+                           'initial model calculations.')
         form.addParam('numberOfClasses', IntParam, default=1,
                       condition='not doContinue',
                       label='Number of classes',
                       help='The number of classes (K) for a multi-reference '
                            'ab initio SGD refinement. These classes will be '
                            'made in an unsupervised manner, starting from a '
                            'single reference in the initial iterations of '
@@ -184,151 +207,56 @@
                       help='If set to Yes, the job will apply a spherical '
                            'mask and enforce all values in the reference '
                            'to be non-negative.')
 
         form.addParam('symmetryGroup', StringParam, default='c1',
                       condition='not doContinue',
                       label="Symmetry",
-                      help='SGD sometimes works better in C1. If you make an '
-                           'initial model in C1 but want to run Class3D/Refine3D '
-                           'with a higher point group symmetry, the reference model '
-                           'must be rotated to conform the symmetry convention. '
-                           'You can do this by the relion_align_symmetry command.')
-
-        group = form.addGroup('Sampling')
-        group.addParam('angularSamplingDeg', EnumParam, default=1,
-                       choices=relion.ANGULAR_SAMPLING_LIST,
-                       label='Initial angular sampling (deg)',
-                       help='There are only a few discrete angular samplings'
-                            ' possible because we use the HealPix library to'
-                            ' generate the sampling of the first two Euler '
-                            'angles on the sphere. The samplings are '
-                            'approximate numbers and vary slightly over '
-                            'the sphere.')
-        group.addParam('offsetSearchRangePix', FloatParam, default=6,
-                       label='Offset search range (pix)',
-                       help='Probabilities will be calculated only for '
-                            'translations in a circle with this radius (in '
-                            'pixels). The center of this circle changes at '
-                            'every iteration and is placed at the optimal '
-                            'translation for each image in the previous '
-                            'iteration.')
-        group.addParam('offsetSearchStepPix', FloatParam, default=2,
-                       label='Offset search step (pix)',
-                       help='Translations will be sampled with this step-size '
-                            '(in pixels). Translational sampling is also done '
-                            'using the adaptive approach. Therefore, if '
-                            'adaptive=1, the translations will first be '
-                            'evaluated on a 2x coarser grid.')
+                      help='The initial model is always generated in C1 '
+                           'and then aligned to and symmetrized with the '
+                           'specified point group. If the automatic alignment '
+                           'fails, please manually rotate run_itNNN_class001.mrc '
+                           '(NNN is the number of iterations) so that it '
+                           'conforms the symmetry convention.')
 
-        form.addSection(label='SGD')
-        self._defineSGD3(form)
-
-        form.addParam('sgdNoiseVar', IntParam, default=-1,
+        form.addParam('runInC1', BooleanParam, default=True,
                       condition='not doContinue',
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Increased noise variance half-life',
-                      help='When set to a positive value, the initial '
-                           'estimates of the noise variance will internally '
-                           'be multiplied by 8, and then be gradually '
-                           'reduced, having 50% after this many particles '
-                           'have been processed. By default, this option '
-                           'is switched off by setting this value to a '
-                           'negative number. In some difficult cases, '
-                           'switching this option on helps. In such cases, '
-                           'values around 1000 have found to be useful. '
-                           'Change the factor of eight with the additional '
-                           'argument *--sgd_sigma2fudge_ini*')
+                      label='Run in C1 and apply symmetry later?',
+                      help='If set to Yes, the gradient-driven optimisation '
+                           'is run in C1 and the symmetry orientation is searched '
+                           'and applied later. If set to No, the entire '
+                           'optimisation is run in the symmetry point group '
+                           'indicated above.')
 
         form.addSection('Compute')
         self._defineComputeParams(form)
 
         form.addParam('extraParams', StringParam, default='',
                       label='Additional arguments',
                       help="In this box command-line arguments may be "
                            "provided that are not generated by the GUI. This "
                            "may be useful for testing developmental options "
                            "and/or expert use of the program, e.g: \n"
                            "--dont_combine_weights_via_disc\n"
                            "--verb 1\n"
                            "--pad 2\n")
 
-        form.addParallelSection(threads=1, mpi=3)
-
-    def _defineSGD3(self, form):
-        """ Define SGD parameters for Relion version 3. """
-        group = form.addGroup('Iterations')
-        group.addParam('numberOfIterInitial', IntParam, default=50,
-                       label='Number of initial iterations',
-                       help='Number of initial SGD iterations, at which the '
-                            'initial resolution cutoff and the initial subset '
-                            'size will be used, and multiple references are '
-                            'kept the same. 50 seems to work well in many '
-                            'cases. Increase if the correct solution is not '
-                            'found.')
-        group.addParam('numberOfIterInBetween', IntParam, default=200,
-                       label='Number of in-between iterations',
-                       help='Number of SGD iterations between the initial and '
-                            'final ones. During these in-between iterations, '
-                            'the resolution is linearly increased, together '
-                            'with the mini-batch or subset size. In case of a '
-                            'multi-class refinement, the different references '
-                            'are also increasingly left to become dissimilar. '
-                            '200 seems to work well in many cases. Increase '
-                            'if multiple references have trouble separating, '
-                            'or the correct solution is not found.')
-        group.addParam('numberOfIterFinal', IntParam, default=50,
-                       label='Number of final iterations',
-                       help='Number of final SGD iterations, at which the '
-                            'final resolution cutoff and the final subset '
-                            'size will be used, and multiple references are '
-                            'left dissimilar. 50 seems to work well in many '
-                            'cases. Perhaps increase when multiple reference '
-                            'have trouble separating.')
-        group.addParam('writeIter', IntParam, default=10,
-                       expertLevel=LEVEL_ADVANCED,
-                       label='Write-out frequency (iter)',
-                       help='Every how many iterations do you want to write the '
-                            'model to disk. Negative value means only write '
-                            'out model after entire iteration.')
-
-        line = form.addLine('Resolution (A)',
-                            help='This is the resolution cutoff (in A) that '
-                                 'will be applied during the initial and final '
-                                 'SGD iterations. 35A and 15A respectively '
-                                 'seems to work well in many cases.')
-        line.addParam('initialRes', IntParam, default=35, label='Initial')
-        line.addParam('finalRes', IntParam, default=15, label='Final')
-
-        line = form.addLine('Mini-batch size',
-                            help='The number of particles that will be processed '
-                                 'during the initial and final iterations. \n\n'
-                                 'For initial, 100 seems to work well in many '
-                                 'cases. Lower values may result in wider '
-                                 'searches of the energy landscape, but possibly '
-                                 'at reduced resolutions. \n\n'
-                                 'For final, 300-500 seems to work well in many '
-                                 'cases. Higher values may result in increased '
-                                 'resolutions, but at increased computational '
-                                 'costs.')
-        line.addParam('initialBatch', IntParam, default=100, label='Initial')
-        line.addParam('finalBatch', IntParam, default=500, label='Final')
+        form.addParallelSection(threads=1, mpi=0)
 
     def addSymmetry(self, container):
         pass
 
     # -------------------------- INSERT steps functions -----------------------
 
     # -------------------------- STEPS functions ------------------------------
     def _getVolumes(self):
         """ Return the list of volumes generated.
         The number of volumes in the list will be equal to
         the number of classes requested by the user in the protocol. """
-        # Provide 1 as default value for making it backward compatible
-        k = self.getAttributeValue('numberOfClasses', 1)
+        k = self.numberOfClasses.get()
         pixelSize = self._getInputParticles().getSamplingRate()
         lastIter = self._lastIter()
         volumes = []
 
         for i in range(1, k + 1):
             vol = Volume(self._getExtraPath('relion_it%03d_class%03d.mrc')
                          % (lastIter, i))
@@ -355,17 +283,35 @@
             output = volumes[0]
             self._defineOutputs(outputVolume=output)
 
         self._defineSourceRelation(self.inputParticles, output)
         self._defineOutputs(outputParticles=outImgSet)
         self._defineTransformRelation(self.inputParticles, outImgSet)
 
+        # Run symmetrization for the largest volume if necessary
+        sym = self.symmetryGroup.get()
+        if sym.lower() != "c1" and self.runInC1:
+            inFn = self._getFileName('model', iter=self._lastIter())
+            symFn = self._getPath('volume_sym%s.mrc' % sym)
+            pixSize = imgSet.getSamplingRate()
+
+            self.runJob("relion_align_symmetry",
+                        "--apply_sym --select_largest_class "
+                        "--i %s --o %s --sym %s --angpix %0.5f" % (
+                            inFn, symFn, sym, pixSize))
+
+            vol = Volume()
+            vol.copyInfo(volumes[0])
+            vol.setLocation(symFn)
+            self._defineOutputs(outputVolumeSymmetrized=vol)
+
     # -------------------------- INFO functions -------------------------------
     def _validateNormal(self):
         errors = []
+
         return errors
 
     def _validateContinue(self):
         errors = []
         continueRun = self.continueRun.get()
         continueRun._initialize()
         lastIter = continueRun._lastIter()
@@ -396,55 +342,50 @@
         summary = ["Continue from iteration %01d" % self._getContinueIter()]
         return summary
 
     # -------------------------- UTILS functions ------------------------------
     def _setBasicArgs(self, args):
         """ Return a dictionary with basic arguments. """
         args.update({'--o': self._getExtraPath('relion'),
-                     '--oversampling': '1'
+                     '--oversampling': 1,
+                     '--pad': 1,
+                     '--tau2_fudge': self.regularisationParamT.get()
                      })
 
         if self.doFlattenSolvent:
             args['--flatten_solvent'] = ''
         if not self.doContinue:
-            args.update({'--sym': self.symmetryGroup.get()})
-        args['--pad'] = 1 if self.skipPadding else 2
-        if self.skipGridding:
-            args['--skip_gridding'] = ''
+            args['--sym'] = 'C1' if self.runInC1 else self.symmetryGroup.get()
 
-        self._setSGDArgs(args)
+        self._setGradArgs(args)
         self._setSamplingArgs(args)
 
-    def _setSGDArgs(self, args):
-        args['--sgd'] = ''
-        args['--sgd_ini_iter'] = self.numberOfIterInitial.get()
-        args['--sgd_inbetween_iter'] = self.numberOfIterInBetween.get()
-        args['--sgd_fin_iter'] = self.numberOfIterFinal.get()
-        args['--sgd_write_iter'] = self.writeIter.get()
-        args['--sgd_ini_resol'] = self.initialRes.get()
-        args['--sgd_fin_resol'] = self.finalRes.get()
-        args['--sgd_ini_subset'] = self.initialBatch.get()
-        args['--sgd_fin_subset'] = self.finalBatch.get()
+    def _setGradArgs(self, args):
+        args['--iter'] = self.numberOfIter.get()
+        args['--grad'] = ''
         args['--K'] = self.numberOfClasses.get()
 
         if not self.doContinue:
             args['--denovo_3dref'] = ''
-            args['--sgd_sigma2fudge_halflife'] = self.sgdNoiseVar.get()
 
     def _setSamplingArgs(self, args):
         """ Set sampling related params"""
         if not self.doContinue:
-            args['--healpix_order'] = self.angularSamplingDeg.get()
-            args['--offset_range'] = self.offsetSearchRangePix.get()
-            args['--offset_step'] = self.offsetSearchStepPix.get() * 2
+            args['--healpix_order'] = 1
+            args['--offset_range'] = 6
+            args['--offset_step'] = 2
+            args['--auto_sampling'] = ''
 
     def _fillDataFromIter(self, imgSet, iteration):
         outImgsFn = self._getFileName('data', iter=iteration)
         imgSet.setAlignmentProj()
-        self.reader = convert.createReader(alignType=ALIGN_PROJ)
-        mdIter = convert.Table.iterRows('particles@' + outImgsFn, key='rlnImageId')
+        px = imgSet.getSamplingRate()
+        self.reader = convert.createReader(alignType=ALIGN_PROJ,
+                                           pixelSize=px)
+        mdIter = convert.Table.iterRows('particles@' + outImgsFn, key='rlnImageId',
+                                        types=convert.LABELS_DICT)
         imgSet.copyItems(self._getInputParticles(), doClone=False,
                          updateItemCallback=self._createItemMatrix,
                          itemDataIterator=mdIter)
 
     def _createItemMatrix(self, item, row):
         self.reader.setParticleTransform(item, row)
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_assign_optic_groups.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_assign_optic_groups.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,14 +41,17 @@
     """ Assign Optics Group name and related parameters to an input set.
      Input set can be: movies, micrographs or particles.
 
      Warning: all optics parameters from the input set itself are removed!
     """
     _label = 'assign optics groups'
     _devStatus = PROD
+    _possibleOutputs = {"outputMovies": SetOfMovies,
+                        "outputMicrographs": SetOfMicrographs,
+                        "outputParticles": SetOfParticles}
     
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputSet', params.PointerParam,
                       pointerClass='SetOfMovies,SetOfMicrographs,SetOfParticles',
                       label="Input set", important=True,
@@ -175,30 +178,28 @@
             outputSet = self._createSetOfMicrographs()
             outputName = 'outputMicrographs'
         elif isinstance(inputSet, SetOfParticles):
             outputSet = self._createSetOfParticles()
             outputName = 'outputParticles'
             getMicName = lambda item: item.getCoordinate().getMicName()
         else:
-            raise Exception("Invalid input of type %s, expecting:\n"
+            raise TypeError("Invalid input of type %s, expecting:\n"
                             "SetOfMovies, SetOfMicrographs or SetOfParticles"
                             % inputSet.getClassName())
 
         # Copy general info from input set
         outputSet.copyInfo(inputSet)
 
         if self.inputType == 0:  # single group params
             og = OpticsGroups.fromImages(inputSet)
             outputSet.copyItems(inputSet)
 
             if len(og) > 1:
-                raise Exception("Multiple optics groups detected in the input!\n"
-                                "Assigning single optics group params "
-                                "is valid only when the input set contains "
-                                "one optics group.")
+                # force a single group assignment
+                og = OpticsGroups([og.first()])
 
             acq = inputSet.getAcquisition()
             params = {
                 'rlnVoltage': acq.getVoltage(),
                 'rlnSphericalAberration': acq.getSphericalAberration(),
                 'rlnAmplitudeContrast': acq.getAmplitudeContrast(),
                 getPixelSizeLabel(inputSet): inputSet.getSamplingRate(),
@@ -230,47 +231,47 @@
             micDict = {row.rlnMicrographName: row.rlnOpticsGroup
                        for row in micTable}
 
             # check if MTF file exists
             if og.hasColumn('rlnMtfFileName'):
                 for i in og:
                     if not os.path.exists(i.rlnMtfFileName):
-                        self.warning("MTF file %s not found for %s" % (
-                            i.rlnMtfFileName, i.rlnOpticsGroupName
-                        ))
-
+                        self.warning("MTF file %s not found for %s" %
+                                     (i.rlnMtfFileName, i.rlnOpticsGroupName))
             # check if gain file exists
             if og.hasColumn('rlnMicrographGainName'):
                 for i in og:
                     if not pwutils.exists(i.rlnMicrographGainName):
                         self.warning("Gain reference file %s not found for %s" % (
                             i.rlnMicrographGainName, i.rlnOpticsGroupName
                         ))
 
             def updateItem(item, row):
                 micName = getMicName(item)
 
-                if micName not in micDict:
-                    raise Exception("Micrograph name (aka micName) '%s' was "
-                                    "not found in the 'data_micrographs' table of "
-                                    "the input star file: %s"
-                                    % (micName, inputStar))
-
-                ogNumber = micDict[micName]
-
-                if not hasattr(item, '_rlnOpticsGroup'):
-                    item._rlnOpticsGroup = Integer()
-
-                item._rlnOpticsGroup.set(ogNumber)
+                if micName in micDict:
+                    item._appendItem = True
+                    ogNumber = micDict[micName]
+
+                    if not hasattr(item, '_rlnOpticsGroup'):
+                        item._rlnOpticsGroup = Integer()
+
+                    item._rlnOpticsGroup.set(ogNumber)
+                else:
+                    item._appendItem = False  # Do not add this row to the output set
+                    self.warning("Micrograph name (aka micName) '%s' was "
+                                 "not found in the 'data_micrographs' table of "
+                                 "the input star file: %s"
+                                 % (micName, inputStar))
 
             outputSet.copyItems(inputSet,
                                 updateItemCallback=updateItem,
                                 doClone=False)
 
-        print(og)
+        self.info(og)
 
         og.toImages(outputSet)
 
         self._defineOutputs(**{outputName: outputSet})
         self._defineTransformRelation(inputSet, outputSet)
     
     # --------------------------- INFO functions ------------------------------
@@ -282,28 +283,48 @@
 
         if self.defectFile.hasValue() and not os.path.exists(self.defectFile.get()):
             validateMsgs.append("Defect file %s does not exist!" % self.defectFile.get())
 
         if self.gainRot.get() or self.gainFlip.get():
             try:
                 from pwem import Domain
-                eman2 = Domain.importFromPlugin('eman2', doRaise=True)
+                _ = Domain.importFromPlugin('eman2', doRaise=True)
             except:
                 validateMsgs.append("EMAN2 plugin not found!\nTransforming gain image "
                                     "requires EMAN2 plugin and binaries installed.")
 
         return validateMsgs
     
     def _summary(self):
         summary = []
+
+        if any(hasattr(self, out) for out in self._possibleOutputs.keys()):
+            if self.inputType == 0:
+                summary.append("Assigned optics group: %s" % self.opticsGroupName.get())
+            else:
+                summary.append("Assigned optics group(s) from star file: %s" % self.inputStar.get())
+
         return summary
     
     def _methods(self):
         return []
 
+    def _warnings(self):
+        warnings = []
+
+        if self.inputType == 0:  # single group params
+            inputSet = self.inputSet.get()
+            og = OpticsGroups.fromImages(inputSet)
+            if len(og) > 1:
+                warnings.append("Multiple optics groups detected in the input!\n"
+                                "Are you sure you want to assign a single optics "
+                                "group params?")
+
+        return warnings
+
     # -------------------------- UTILS functions ------------------------------
     def _convertGain(self):
         """ We need to transform gain file for a possible polishing job. """
         rotation = self.gainRot.get()
         flip = self.gainFlip.get()
         gainFn = self.gainFile.get()
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_autopick.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
                                         + '_autopick.star') for mic in micSet]
         convert.readSetOfCoordinates(coordSet, starFiles)
         return self._writeXmippCoords(coordSet)
 
     def __getMicListPrefix(self, micList):
         n = len(micList)
         if n == 0:
-            raise Exception("Empty micrographs list!")
+            raise ValueError("Empty micrographs list!")
         micsPrefix = 'mic_%06d' % micList[0].getObjId()
         if n > 1:
             micsPrefix += "-%06d" % micList[-1].getObjId()
         return micsPrefix
 
     def _getMicStarFile(self, micList):
         return self._getTmpPath(self.__getMicListPrefix(micList) + '.star')
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_autopick_log.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick_log.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 from os.path import relpath
 
 import pyworkflow.protocol.params as params
+from pyworkflow.utils.properties import Message
 from pyworkflow.constants import PROD
 from pyworkflow.protocol import STEPS_SERIAL
 from pwem.protocols import ProtParticlePickingAuto
 
 from .protocol_autopick import ProtRelionAutopickBase
 
 
@@ -56,26 +57,24 @@
                            'If using the *Optimize* mode, just a subset of '
                            'micrographs are used to compute the FOM maps. '
                            'If in *Compute* mode, all micrographs will be '
                            'auto-picked.')
 
         form.addParam('boxSize', params.IntParam,
                       label='Box size (px)',
+                      allowsPointers=True,
                       help="Box size in pixels.")
 
         group = form.addGroup('Laplacian of Gaussian')
 
-        line = group.addLine('Diameter for LoG filter (A)',
-                             help="Min and Max of LoG filter")
+        group.addParam('minDiameter', params.IntParam, default=200, allowsPointers=True,
+                       label='Min diameter (A)')
 
-        line.addParam('minDiameter', params.IntParam, default=200,
-                      label='Min')
-
-        line.addParam('maxDiameter', params.IntParam, default=250,
-                      label='Max')
+        group.addParam('maxDiameter', params.IntParam, default=250, allowsPointers=True,
+                       label='Max diameter (A)')
 
         group.addParam('areParticlesWhite', params.BooleanParam,
                        default=False,
                        label='Are the particles white?',
                        help='Set this option to No if the particles are black, '
                             'and to Yes if the particles are white.')
 
@@ -163,13 +162,25 @@
     # -------------------------- INFO functions --------------------------------
     def _validate(self):
         errors = []
         return errors
 
     def _summary(self):
         summary = []
+
+        if self.getInputMicrographs() is not None:
+            summary.append("Using Relion LoG picker.")
+            summary.append("Number of input micrographs: *%d*"
+                           % self.getInputMicrographs().getSize())
+        if self.getOutputsSize() > 0:
+            summary.append("Number of particles picked: *%d*"
+                           % self.getCoords().getSize())
+            summary.append("Particle size: *%d* px"
+                           % self.getCoords().getBoxSize())
+        else:
+            summary.append(Message.TEXT_NO_OUTPUT_CO)
         return summary
 
     # -------------------------- UTILS functions -------------------------------
     def getBoxSize(self):
         """ Return a reasonable box-size in pixels. """
         return self.boxSize.get()
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_autopick_ref.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_autopick_ref.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,17 +30,16 @@
 from pwem.protocols import ProtParticlePickingAuto
 from pwem.constants import RELATION_CTF
 from pwem.emlib.image import ImageHandler
 from pyworkflow.utils.properties import Message
 import pyworkflow.utils as pwutils
 from pyworkflow.constants import PROD
 
-from relion import Plugin
 import relion.convert
-from ..constants import *
+from ..constants import REF_AVERAGES, REF_VOLUME, ANGULAR_SAMPLING_LIST
 from .protocol_autopick import ProtRelionAutopickBase
 
 
 class ProtRelion2Autopick(ProtRelionAutopickBase):
     """ This protocol runs Relion autopicking (version > 3.0).
 
     This Relion protocol uses the 'relion_autopick' program to pick particles
@@ -124,22 +123,14 @@
                            "angles on the sphere. The samplings are approximate "
                            "numbers and vary slightly over the sphere.\n"
                            "For autopicking, 30 degrees is usually fine enough, "
                            "but for highly symmetrical objects one may need to "
                            "go finer to adequately sample the asymmetric part of "
                            "the sphere.")
 
-        if not Plugin.IS_GT31():
-            form.addParam('particleDiameter', params.IntParam, default=-1,
-                          label='Mask diameter (A)',
-                          help='Diameter of the circular mask that will be applied '
-                               'around the templates in Angstroms. When set to a '
-                               'negative value, this value is estimated '
-                               'automatically from the templates themselves.')
-
         form.addParam('lowpassFilterRefs', params.IntParam, default=20,
                       label='Lowpass filter references (A)',
                       help='Lowpass filter that will be applied to the '
                            'references before template matching. \n'
                            'Do NOT use very high-resolution templates to '
                            'search your micrographs. \n'
                            'The signal will be too weak at high resolution '
@@ -338,17 +329,14 @@
         # - minDistance
         # - maxStd
         params = ' --pickname autopick'
         params += ' --odir "./"'
         params += ' --angpix %0.5f' % self.getInputMicrographs().getSamplingRate()
         params += ' --shrink %0.3f' % self.shrinkFactor
 
-        if not Plugin.IS_GT31():
-            params += ' --particle_diameter %d' % self.particleDiameter
-
         if self.doGpu:
             params += ' --gpu "%s"' % self.gpusToUse
 
         if self.useInputReferences():
             params += ' --ref %s' % abspath(self._getPath('reference_2d.stk'))
         else:  # 3D reference
             params += ' --ref %s' % abspath(self._getPath('reference_3d.mrc'))
@@ -400,50 +388,50 @@
         params += ' --max_stddev_noise %0.3f' % maxStddevNoise
         params += ' --min_avg_noise %0.3f' % minAvgNoise
 
         program = self._getProgram('relion_autopick')
 
         self.runJob(program, params, cwd=cwd)
 
-    # -------------------------- STEPS functions -------------------------------
     def createOutputStep(self):
-        micSet = self.getInputMicrographs()
+        micSet = self.getInputMicrographsPointer()
         outputCoordinatesName = 'outputCoordinates'
         coordSet = self._createSetOfCoordinates(micSet)
-        self.readCoordsFromMics(None, micSet, coordSet)
+        self.readCoordsFromMics(None, micSet.get(), coordSet)
 
         self._defineOutputs(**{outputCoordinatesName: coordSet})
-        self._defineSourceRelation(self.getInputMicrographsPointer(),
-                                   coordSet)
+        self._defineSourceRelation(micSet, coordSet)
 
     # -------------------------- INFO functions --------------------------------
     def _validate(self):
         errors = []
 
-        if self.useInputReferences():
-            if not Plugin.IS_GT31() and (self.particleDiameter > self.getInputDimA()):
-                errors.append('Particle diameter (%d) can not be greater than '
-                              'size (%d)' % (self.particleDiameter,
-                                             self.getInputDimA()))
-            if self.getInputReferences().isOddX():
-                errors.append("Relion only works with even values for the "
-                              "average dimensions!")
-        else:
-            if self.particleDiameter <= 0:
-                errors.append('When using Gaussian blobs, you need to specify '
-                              'the particles diameter manually. ')
+        if self.useInputReferences() and self.getInputReferences().isOddX():
+            errors.append("Relion only works with even values for the "
+                          "average dimensions!")
 
         if self.ctfRelations.get() is None and self.refsCtfCorrected:
             errors.append("References CTF corrected parameter must be set to "
                           "False or set ctf relations.")
 
         return errors
 
     def _summary(self):
         summary = []
+        if self.getInputMicrographs() is not None:
+            summary.append("Using Relion reference-based picker.")
+            summary.append("Number of input micrographs: *%d*"
+                           % self.getInputMicrographs().getSize())
+        if self.getOutputsSize() > 0:
+            summary.append("Number of particles picked: *%d*"
+                           % self.getCoords().getSize())
+            summary.append("Particle size: *%d* px"
+                           % self.getCoords().getBoxSize())
+        else:
+            summary.append(Message.TEXT_NO_OUTPUT_CO)
         return summary
 
     def _citations(self):
         return ['Scheres2015']
 
     def _methods(self):
         methodsMsgs = []
@@ -473,18 +461,15 @@
     def getBoxSize(self):
         """ Return a reasonable box-size in pixels. """
         inputRefs = self.getInputReferences()
         inputMics = self.getInputMicrographs()
         micsSampling = inputMics.getSamplingRate()
 
         if inputRefs is None:
-            if Plugin.IS_GT31():
-                boxSize = 128
-            else:
-                boxSize = int(self.particleDiameter.get() * 1.25 / micsSampling)
+            boxSize = 128
         else:
             # Scale boxsize if the pixel size of the references is not the same
             # of the micrographs
             scale = inputRefs.getSamplingRate() / micsSampling
             boxSize = int(inputRefs.getXDim() * scale)
 
         if boxSize % 2 == 1:
@@ -506,15 +491,15 @@
         inputMics = self.getInputMicrographs()
 
         return inputMics
 
     def __getMicListPrefix(self, micList):
         n = len(micList)
         if n == 0:
-            raise Exception("Empty micrographs list!")
+            raise ValueError("Empty micrographs list!")
         micsPrefix = 'mic_%06d' % micList[0].getObjId()
         if n > 1:
             micsPrefix += "-%06d" % micList[-1].getObjId()
         return micsPrefix
 
     def _getMicStarFile(self, micList):
         return self._getTmpPath(self.__getMicListPrefix(micList) + '.star')
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_base.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,42 +48,43 @@
 
 class ProtRelionBase(EMProtocol):
     """ This class contains the common functions for all Relion protocols.
     In subclasses there should be little changes about how to create the command
     line and the files produced.
 
     Most of the Relion protocols, have two modes: NORMAL or CONTINUE. That's why
-    some of the function have a template pattern approach to define the behaviour
+    some functions have a template pattern approach to define the behaviour
     depending on the case.
     """
     _label = None
     IS_CLASSIFY = True
     IS_2D = False
     IS_3D_INIT = False
+    IS_3D_MB = False
     OUTPUT_TYPE = SetOfClasses3D
     FILE_KEYS = ['data', 'optimiser', 'sampling']
     CLASS_LABEL = 'rlnClassNumber'
     CHANGE_LABELS = ['rlnChangesOptimalOrientations',
                      'rlnChangesOptimalOffsets',
                      'rlnOverallAccuracyRotations',
                      'rlnOverallAccuracyTranslationsAngst',
                      'rlnChangesOptimalClasses']
     PREFIXES = ['']
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
 
     def _initialize(self):
-        """ This function is mean to be called after the
+        """ This function is meant to be called after the
         working dir for the protocol have been set. (maybe after recovery from mapper)
         """
         self._createFilenameTemplates()
         self._createIterTemplates()
 
-        self.ClassFnTemplate = '%(rootDir)s/relion_it%(iter)03d_class%(ref)03d.mrc:mrc'
+        self.ClassFnTemplate = '%(rootDir)s/relion_it%(iter)03d_class%(ref)03d.mrc'
         if not self.doContinue:
             self.continueRun.set(None)
         else:
             if not self.IS_2D:
                 self.referenceVolume.set(None)
 
     def _createFilenameTemplates(self):
@@ -100,44 +101,44 @@
             'optimiser': self.extraIter + 'optimiser.star',
             'angularDist_xmipp': self.extraIter + 'angularDist_xmipp.xmd',
             'all_avgPmax': self._getPath('iterations_avgPmax.star'),
             'all_changes': self._getPath('iterations_changes.star'),
             'selected_volumes': self._getPath('selected_volumes_xmipp.xmd'),
             'dataFinal': self._getExtraPath("relion_data.star"),
             'modelFinal': self._getExtraPath("relion_model.star"),
-            'finalvolume': self._getExtraPath("relion_class%(ref3d)03d.mrc:mrc"),
-            'final_half1_volume': self._getExtraPath("relion_half1_class%(ref3d)03d_unfil.mrc:mrc"),
-            'final_half2_volume': self._getExtraPath("relion_half2_class%(ref3d)03d_unfil.mrc:mrc"),
-            'finalSGDvolume': self._getExtraPath("relion_it%(iter)03d_class%(ref3d)03d.mrc:mrc"),
+            'finalvolume': self._getExtraPath("relion_class%(ref3d)03d.mrc"),
+            'final_half1_volume': self._getExtraPath("relion_half1_class%(ref3d)03d_unfil.mrc"),
+            'final_half2_volume': self._getExtraPath("relion_half2_class%(ref3d)03d_unfil.mrc"),
+            'finalSGDvolume': self._getExtraPath("relion_it%(iter)03d_class%(ref3d)03d.mrc"),
             'preprocess_particles': self._getPath("preprocess_particles.mrcs"),
             'preprocess_particles_star': self._getPath("preprocess_particles.star"),
             'preprocess_particles_prefix': "preprocess_particles",
-            'finalvolume_mbody': self._getExtraPath("relion_body%(ref3d)03d.mrc:mrc"),
-            'final_half1_volume_mbody': self._getExtraPath("relion_half1_body%(ref3d)03d_unfil.mrc:mrc"),
-            'final_half2_volume_mbody': self._getExtraPath("relion_half2_body%(ref3d)03d_unfil.mrc:mrc"),
+            'finalvolume_mbody': self._getExtraPath("relion_body%(ref3d)03d.mrc"),
+            'final_half1_volume_mbody': self._getExtraPath("relion_half1_body%(ref3d)03d_unfil.mrc"),
+            'final_half2_volume_mbody': self._getExtraPath("relion_half2_body%(ref3d)03d_unfil.mrc"),
         }
         # add to keys, data.star, optimiser.star and sampling.star
         for key in self.FILE_KEYS:
             myDict[key] = self.extraIter + '%s.star' % key
             key_xmipp = key + '_xmipp'
             myDict[key_xmipp] = self.extraIter + '%s.xmd' % key
         # add other keys that depends on prefixes
         for p in self.PREFIXES:
             myDict['%smodel' % p] = self.extraIter + '%smodel.star' % p
-            myDict['%svolume' % p] = self.extraIter + p + 'class%(ref3d)03d.mrc:mrc'
-            myDict['%svolume_mbody' % p] = self.extraIter + p + 'body%(ref3d)03d.mrc:mrc'
+            myDict['%svolume' % p] = self.extraIter + p + 'class%(ref3d)03d.mrc'
+            myDict['%svolume_mbody' % p] = self.extraIter + p + 'body%(ref3d)03d.mrc'
 
         self._updateFilenamesDict(myDict)
 
     def _createIterTemplates(self):
         """ Setup the regex on how to find iterations. """
         self._iterTemplate = self._getFileName('data', iter=0).replace('000', '???')
         # Iterations will be identify by _itXXX_ where XXX is the iteration number
         # and is restricted to only 3 digits.
-        self._iterRegex = re.compile('_it(\d{3})_')
+        self._iterRegex = re.compile(r'_it(\d{3})_')
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineConstants(self):
         self.IS_3D = not self.IS_2D
 
     def _defineParams(self, form):
         self._defineConstants()
@@ -338,24 +339,14 @@
         form.addParam('doCTF', BooleanParam, default=True,
                       label='Do CTF-correction?', condition='not doContinue',
                       help='If set to Yes, CTFs will be corrected inside the '
                            'MAP refinement. The resulting algorithm '
                            'intrinsically implements the optimal linear, or '
                            'Wiener filter. Note that input particles should '
                            'contains CTF parameters.')
-        if not Plugin.IS_GT31():
-            form.addParam('hasReferenceCTFCorrected', BooleanParam, default=False,
-                          condition='not is2D and not doContinue',
-                          label='Has reference been CTF-corrected?',
-                          help='Set this option to Yes if the reference map '
-                               'represents CTF-unaffected density, e.g. it was '
-                               'created using Wiener filtering inside RELION or '
-                               'from a PDB. If set to No, then in the first '
-                               'iteration, the Fourier transforms of the reference '
-                               'projections are not multiplied by the CTFs.')
         form.addParam('haveDataBeenPhaseFlipped', LabelParam,
                       condition='not doContinue',
                       label='Have data been phase-flipped?      '
                             '(Don\'t answer, see help)',
                       help='The phase-flip status is recorded and managed by '
                            'Scipion. \n In other words, when you import or '
                            'extract particles, \nScipion will record whether '
@@ -421,15 +412,15 @@
                                'weight on the experimental data. Values around '
                                '2-4 have been observed to be useful for 3D '
                                'refinements, values of 1-2 for 2D refinements. '
                                'Too small values yield too-low resolution '
                                'structures; too high values result in '
                                'over-estimated resolutions and overfitting.')
 
-            if Plugin.IS_GT31() and self.IS_2D:  # relion4 2D cls case
+            if self.IS_2D:  # 2D cls case
                 form.addParam('useGradientAlg', BooleanParam, default=True,
                               condition='not doContinue',
                               label='Use VDAM algorithm?',
                               help='If set to Yes, the faster VDAM algorithm '
                                    'will be used. This algorithm was introduced '
                                    'with Relion-4.0. If set to No, then the '
                                    'slower EM algorithm needs to be used.')
@@ -461,15 +452,14 @@
                                    'by the user if further iterations do not yield '
                                    'improvements in resolution or classes. '
                                    'If continue option is True, you going to do '
                                    'this number of new iterations (e.g. if '
                                    '*Continue from iteration* is set 3 and this '
                                    'param is set 25, the final iteration of the '
                                    'protocol will be the 28th.')
-
             else:
                 form.addParam('numberOfIterations', IntParam, default=25,
                               label='Number of iterations',
                               help='Number of iterations to be performed. Note '
                                    'that the current implementation does NOT '
                                    'comprise a convergence criterium. Therefore, '
                                    'the calculations will need to be stopped '
@@ -477,26 +467,34 @@
                                    'improvements in resolution or classes. '
                                    'If continue option is True, you going to do '
                                    'this number of new iterations (e.g. if '
                                    '*Continue from iteration* is set 3 and this '
                                    'param is set 25, the final iteration of the '
                                    'protocol will be the 28th.')
 
-            if (Plugin.IS_GT31() and self.IS_3D) or not Plugin.IS_GT31():
+            if self.IS_3D:
                 form.addParam('useFastSubsets', BooleanParam, default=False,
                               condition='not doContinue',
                               label='Use fast subsets (for large data sets)?',
                               help='If set to Yes, the first 5 iterations will '
                                    'be done with random subsets of only K*100 '
                                    'particles (K being the number of classes); '
                                    'the next 5 with K*300 particles, the next '
                                    '5 with 30% of the data set; and the final '
                                    'ones with all data. This was inspired by '
                                    'a cisTEM implementation by Niko Grigorieff'
                                    ' et al.')
+                if Plugin.IS_GT50():
+                    form.addParam('useBlush', BooleanParam, default=False,
+                                  condition='not doContinue',
+                                  label='Use Blush regularisation?',
+                                  help='If set to Yes, relion_refine will use a neural '
+                                       'network to perform regularisation by denoising '
+                                       'at every iteration, instead of the standard '
+                                       'smoothness regularisation.')
 
             form.addParam('limitResolEStep', FloatParam, default=-1,
                           label='Limit resolution E-step to (A)',
                           condition="not doContinue",
                           help='If set to a positive number, then the '
                                'expectation step (i.e. the alignment) will be '
                                'done only including the Fourier components up '
@@ -643,14 +641,21 @@
                                    'sampling go down if the current '
                                    'resolution already requires that '
                                    'sampling at the edge of the particle.\n\n'
                                    'This option will make the computation '
                                    'faster, but has not been tested for '
                                    'many cases for potential loss in '
                                    'reconstruction quality upon convergence.')
+                if Plugin.IS_GT50():
+                    form.addParam('useBlush', BooleanParam, default=False,
+                                  label='Use Blush regularisation?',
+                                  help='If set to Yes, relion_refine will use a neural '
+                                       'network to perform regularisation by denoising '
+                                       'at every iteration, instead of the standard '
+                                       'smoothness regularisation.')
 
         if self.IS_CLASSIFY:
             form.addParam('allowCoarserSampling', BooleanParam,
                           condition='doImageAlignment',
                           default=False,
                           label='Allow coarser sampling?',
                           help='If set to Yes, the program will use '
@@ -719,31 +724,25 @@
                            'for each thread. If it is set to 3 and one '
                            'uses 8 threads, batches of 3x8=24 particles '
                            'will be read together. This may improve '
                            'performance on systems where disk access, and '
                            'particularly metadata handling of disk '
                            'access, is a problem. It has a modest cost of '
                            'increased RAM usage.')
-        if self.IS_3D:
-            if not (Plugin.IS_GT31() and self.IS_3D_INIT):
-                form.addParam('skipPadding', BooleanParam, default=False,
-                              label='Skip padding',
-                              help='If set to Yes, the calculations will not use '
-                                   'padding in Fourier space for better '
-                                   'interpolation in the references. Otherwise, '
-                                   'references are padded 2x before Fourier '
-                                   'transforms are calculated. Skipping padding '
-                                   '(i.e. use --pad 1) gives nearly as good results '
-                                   'as using --pad 2, but some artifacts may appear '
-                                   'in the corners from signal that is folded back.')
-            form.addParam('skipGridding', BooleanParam, default=True,
-                          label='Skip gridding',
-                          help='If set to Yes, the calculations will '
-                               'skip gridding in the M step to save time, '
-                               'typically with just as good results.')
+        if self.IS_3D and not self.IS_3D_INIT:
+            form.addParam('skipPadding', BooleanParam, default=False,
+                          label='Skip padding',
+                          help='If set to Yes, the calculations will not use '
+                               'padding in Fourier space for better '
+                               'interpolation in the references. Otherwise, '
+                               'references are padded 2x before Fourier '
+                               'transforms are calculated. Skipping padding '
+                               '(i.e. use --pad 1) gives nearly as good results '
+                               'as using --pad 2, but some artifacts may appear '
+                               'in the corners from signal that is folded back.')
 
         form.addParam('allParticlesRam', BooleanParam, default=False,
                       label='Pre-read all particles into RAM?',
                       help='If set to Yes, all particle images will be '
                            'read into computer memory, which will greatly '
                            'speed up calculations on systems with slow '
                            'disk access. However, one should of course be '
@@ -856,15 +855,15 @@
             # If copyAlignment is set to False pass alignType to ALIGN_NONE
             alignType = imgSet.getAlignment() if copyAlignment else ALIGN_NONE
             hasAlign = alignType != ALIGN_NONE
             alignToPrior = hasAlign and getattr(self, 'alignmentAsPriors', False)
 
             if self.doCtfManualGroups:
                 self._defocusGroups = self.createDefocusGroups()
-                print(self._defocusGroups)
+                self.info(self._defocusGroups)
 
             relion.convert.writeSetOfParticles(
                 imgSet, imgStar,
                 outputDir=self._getExtraPath(),
                 alignType=alignType,
                 postprocessImageRow=self._postprocessParticleRow)
 
@@ -887,15 +886,15 @@
         """ Execute the relion steps with the give params. """
         params += ' --j %d' % self.numberOfThreads
         self.runJob(self._getProgram(), params)
 
     def _getEnviron(self):
         env = Plugin.getEnviron()
 
-        if self.useGpu():
+        if self.usesGpu():
             prepend = env.get('RELION_PREPEND', '')
         else:
             prepend = env.get('RELION_PREPEND_CPU', '')
 
         env.setPrepend(prepend)
 
         return env
@@ -1020,15 +1019,15 @@
         if self.maskZero == MASK_FILL_ZERO:
             args['--zero_mask'] = ''
 
         if self.IS_CLASSIFY:
             args['--K'] = self.numberOfClasses.get()
             if self.limitResolEStep > 0:
                 args['--strict_highres_exp'] = self.limitResolEStep.get()
-            if self.IS_2D and Plugin.IS_GT31():
+            if self.IS_2D:
                 if self.useGradientAlg:
                     args['--grad'] = ''
                     args['--grad_write_iter'] = 10
                     args['--class_inactivity_threshold'] = 0.1
                 if self.centerAvg:
                     args['--center_classes'] = ''
 
@@ -1037,14 +1036,17 @@
                 args['--firstiter_cc'] = ''
             args['--ini_high'] = self.initialLowPassFilterA.get()
             args['--sym'] = self.symmetryGroup.get()
             # We use the same pixel size as input particles, since
             # we convert anyway the input volume to match same size
             args['--ref_angpix'] = ps
 
+            if Plugin.IS_GT50() and self.useBlush:
+                args['--blush'] = ''
+
         refArg = self._getRefArg()
         if refArg:
             args['--ref'] = refArg
 
         self._setBasicArgs(args)
 
     def _setContinueArgs(self, args):
@@ -1076,22 +1078,15 @@
         else:
             if self._getScratchDir():
                 args['--scratch_dir'] = self._getScratchDir()
 
         args['--pool'] = self.pooledParticles.get()
 
         if self.doGpu:
-            gpuStr = self.gpusToUse.get().strip()
-            if gpuStr:
-                if not gpuStr.startswith('"'):
-                    gpuStr = '"' + gpuStr
-                if not gpuStr.endswith('"'):
-                    gpuStr += '"'
-
-            args['--gpu'] = gpuStr
+            args['--gpu'] = self._getGpuStr()
 
     def _getSamplingFactor(self):
         return 1 if self.oversampling == 0 else 2 * self.oversampling.get()
 
     def _setBasicArgs(self, args):
         """ Return a dictionary with basic arguments. """
         args['--norm'] = ''
@@ -1106,33 +1101,26 @@
 
             if not self.doContinue:
                 self._setSubsetArgs(args)
 
         # Padding can be set in a normal run or in a continue
         if self.IS_3D:
             args['--pad'] = 1 if self.skipPadding else 2
-            if self.skipGridding:
-                args['--skip_gridding'] = ''
 
         self._setSamplingArgs(args)
         self._setMaskArgs(args)
 
     def _setSamplingArgs(self, args):
         """ Should be implemented in subclasses. """
         pass
 
     def _setCTFArgs(self, args):
-        # CTF stuff
         if self.doCTF:
             args['--ctf'] = ''
 
-            # this only can be true if is 3D
-            if not Plugin.IS_GT31() and self.hasReferenceCTFCorrected:
-                args['--ctf_corrected_ref'] = ''
-
             if self._getInputParticles().isPhaseFlipped():
                 args['--ctf_phase_flipped'] = ''
 
             if self.ignoreCTFUntilFirstPeak:
                 args['--ctf_intact_first_peak'] = ''
 
     def _setMaskArgs(self, args):
@@ -1208,15 +1196,15 @@
         data_classes = self._getFileName('classes_scipion', iter=it)
 
         if clean:
             pwutils.cleanPath(data_classes)
 
         if not os.path.exists(data_classes):
             clsSet = self.OUTPUT_TYPE(filename=data_classes)
-            clsSet.setImages(self.inputParticles.get())
+            clsSet.setImages(self.inputParticles)
             self._fillClassesFromIter(clsSet, it)
             clsSet.write()
             clsSet.close()
 
         return data_classes
 
     def _fillClassesFromIter(self, clsSet, iteration):
@@ -1253,15 +1241,15 @@
                 continueIter = int(self.continueIter.get())
         else:
             continueIter = 0
 
         return continueIter
 
     def _getnumberOfIters(self):
-        if Plugin.IS_GT31() and self.IS_2D and self.useGradientAlg:
+        if self.IS_2D and self.useGradientAlg:
             return self._getContinueIter() + self.numberOfVDAMBatches.get()
         else:
             return self._getContinueIter() + self.numberOfIterations.get()
 
     def _getReferenceVolumes(self):
         """ Return a list with all input references.
         (Could be one or more volumes).
@@ -1269,15 +1257,15 @@
         inputObj = self.referenceVolume.get()
 
         if isinstance(inputObj, Volume):
             return [inputObj]
         elif isinstance(inputObj, SetOfVolumes):
             return [vol.clone() for vol in inputObj]
         else:
-            raise Exception("Invalid input reference of class: %s"
+            raise TypeError("Invalid input reference of class: %s"
                             % inputObj.getClassName())
 
     def _getRefArg(self):
         """ Return the filename that will be used for the --ref argument.
         The value will depend if in 2D and 3D or if input references will
         be used.
         It will return None if no --ref should be used. """
@@ -1346,20 +1334,43 @@
         if self.doCtfManualGroups:
             groupId = self._defocusGroups.getGroup(part.getCTF().getDefocusU()).id
             partRow['rlnGroupName'] = "ctf_group_%03d" % groupId
 
     def _useFastSubsets(self):
         return self.getAttributeValue('useFastSubsets', False)
 
-    def useGpu(self):
-        """
-        Return True if the protocol has gpu option and it has been selected.
-        """
+    def _getGpuStr(self):
+        gpuStr = self.getAttributeValue('gpusToUse', '')
+        gpuStr = gpuStr.strip().strip('"')
+
+        return f'"{gpuStr}"'
+
+    def usesGpu(self):
+        """ Return True if the protocol has gpu option and
+        it has been selected. """
         return self.getAttributeValue('doGpu', False)
 
+    def getGpuList(self):
+        gpuStr = self._getGpuStr()
+        if gpuStr.startswith('"'):
+            gpuStr = gpuStr[1:-1]
+
+        gpuList = []
+        parts = gpuStr.split(':')
+        for p in parts:
+            parts2 = p.split(',')
+            for p2 in parts2:
+                if p2:
+                    gpu = int(p2)
+                    if gpu not in gpuList:
+                        gpuList.append(gpu)
+        gpuList.sort()
+
+        return gpuList
+
     def _copyAlignAsPriors(self, mdParts, alignType):
         # set priors equal to orig. values
         mdParts.addColumns('rlnOriginXPriorAngst=rlnOriginXAngst')
         mdParts.addColumns('rlnOriginYPriorAngst=rlnOriginYAngst')
         mdParts.addColumns('rlnAnglePsiPrior=rlnAnglePsi')
 
         if alignType == ALIGN_PROJ:
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_bayesian_polishing.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_bayesian_polishing.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,28 +24,33 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
 
 import os
 import json
+from enum import Enum
 from emtable import Table
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
 from pwem.protocols import ProtParticles
 import pwem.emlib.metadata as md
 from pwem.constants import ALIGN_PROJ
+from pwem.objects import SetOfParticles
 
-from relion import Plugin
 import relion.convert as convert
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputParticles = SetOfParticles
+
+
 class ProtRelionBayesianPolishing(ProtParticles, ProtRelionBase):
     """
     Wrapper protocol for the Relion's Bayesian Polishing.
 
     As of release 3.0, Relion also implements a new Bayesian approach to beam
     induced motion correction. This approach aims to optimise a regularised
     likelihood, which allows us to associate with each hypothetical set of
@@ -59,14 +64,15 @@
     particles in the data set and to produce adequately weighted averages of
     the aligned movie frames.
 
     """
 
     _label = 'bayesian polishing'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
     OP_TRAIN = 0
     OP_POLISH = 1
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called for iterations and references. """
         myDict = {
@@ -94,42 +100,38 @@
                       important=True,
                       label='Input Postprocess',
                       pointerClass='ProtRelionPostprocess',
                       help='Select a PostProcess job. The mask used for this '
                            'postprocessing will be applied to the unfiltered '
                            'half-maps and should encompass the entire complex. '
                            'The resulting FSC curve will be used for weighting '
-                           'the different frequencies. ')
+                           'the different frequencies.')
         line = form.addLine('Movie frames',
                             help='First and last frames to take into account '
-                                 'in motion fit and combination step. '
-                                 '(starts counting at 1 and 0 as last '
-                                 'means util the last frame in the movie).')
+                                 'in motion fit and combination step '
+                                 '(first frame is 1, last is 0).')
         line.addParam('frame0', params.IntParam, default=1,
                       label='first')
         line.addParam('frameN', params.IntParam, default=0,
                       label='last')
 
         form.addParam('extrSize', params.IntParam, default=-1,
                       label="Extraction size (px in unbinned movie)",
                       help="Size of the extracted particles in the "
-                           "unbinned original movie(in pixels). "
+                           "unbinned original movie (in pixels). "
                            "This should be an even number.")
         form.addParam('rescaledSize', params.IntParam, default=-1,
                       label="Re-scaled size (px)",
                       help="The re-scaled value needs to be an even number.")
 
-        if Plugin.IS_GT31():
-            form.addParam('saveFloat16', params.BooleanParam, default=False,
-                          label="Write output in float16?",
-                          expertLevel=params.LEVEL_ADVANCED,
-                          lavel="Write output in float16?",
-                          help="Relion can write output images in float16 "
-                               "MRC (mode 12) format to save disk space. "
-                               "By default, float32 format is used.")
+        form.addParam('saveFloat16', params.BooleanParam, default=True,
+                      label="Write output in float16?",
+                      help="Relion can write output images in float16 "
+                           "MRC (mode 12) format to save disk space. "
+                           "By default, float32 format is used.")
 
         form.addSection(label='Train or Polish')
         form.addParam('operation', params.EnumParam, default=1,
                       choices=['Train optimal parameters',
                                'Perform particle polishing'],
                       display=params.EnumParam.DISPLAY_COMBO,
                       label='Operation',
@@ -352,15 +354,15 @@
             args += "--s_vel %0.3f " % self.sigmaVel
             args += "--s_div %0.3f " % self.sigmaDiv
             args += "--s_acc %0.3f " % self.sigmaAcc
             args += "--bfac_minfreq %0.3f " % self.minResBfactor
             args += "--bfac_maxfreq %0.3f " % self.maxResBfactor
             args += "--combine_frames "
 
-        if Plugin.IS_GT31() and self.saveFloat16:
+        if self.saveFloat16:
             args += "--float16 "
 
         args += "--j %d " % self.numberOfThreads
 
         self.runJob(self._getProgram('relion_motion_refine'), args)
 
     def createOutputStep(self, id=1):
@@ -373,26 +375,26 @@
         outImgsFn = md.MetaData('particles@' + self._getFileName('shiny'))
         rowIterator = md.SetMdIterator(outImgsFn, sortByLabel=md.RLN_IMAGE_ID,
                                        keyLabel=md.RLN_IMAGE_ID,
                                        updateItemCallback=self._updatePtcl)
         outImgSet.copyItems(imgSet,
                             updateItemCallback=rowIterator.updateItem)
 
-        self._defineOutputs(outputParticles=outImgSet)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
         self._defineTransformRelation(self.inputParticles, outImgSet)
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
 
         def _params(label, *params):
-            summary.append('*%s params:*' % label)
-            summary.append('    Sigma for velocity: %0.3f' % params[0])
-            summary.append('    Sigma for divergence: %0.1f' % params[1])
-            summary.append('    Sigma for acceleration: %0.2f' % params[2])
+            summary.append('%s params:' % label)
+            summary.append('    Sigma for velocity: *%0.3f*' % params[0])
+            summary.append('    Sigma for divergence: *%0.1f*' % params[1])
+            summary.append('    Sigma for acceleration: *%0.2f*' % params[2])
 
         if self.operation != self.OP_TRAIN:
             _params('Input', self.sigmaVel, self.sigmaDiv, self.sigmaAcc)
         else:
             outputFn = None
             for fn in ['opt_params.txt', 'opt_params_all_groups.txt']:
                 if os.path.exists(self._getExtraPath(fn)):
@@ -425,18 +427,14 @@
             if scale > win:
                 errors.append("ERROR: The downsampled box size cannot be "
                               "larger than the extraction size")
 
         if self.operation == self.OP_TRAIN and self.numberOfMpi > 1:
             errors.append("MPI is not supported for parameters estimation.")
 
-        if self.hasAttribute('saveFloat16') and self.saveFloat16:
-            errors.append("MRC float16 format is not yet supported by XMIPP, "
-                          "so you cannot use this option.")
-
         return errors
 
     def _warnings(self):
         warnings = ['If you have provided a gain reference or defects file during '
                     'movie import or motion correction, please *make sure to '
                     'run first "assign optics groups" protocol for aligned '
                     'movies*, specifying the gain file etc. Currently, Scipion '
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_center_averages.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_center_averages.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,28 +20,36 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+from enum import Enum
+
 from pwem.protocols import ProtProcessParticles
+from pwem.objects import SetOfAverages
 from pyworkflow.protocol.params import PointerParam
 from pyworkflow.constants import PROD
 
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputAverages = SetOfAverages
+
+
 class ProtRelionCenterAverages(ProtProcessParticles, ProtRelionBase):
     """
     Align class averages by their center of mass using *relion_image_handler*.
      (With *--shift_com* option)
     """
     _label = 'center averages'
     _devStatus = PROD
+    _possibleOutputs = outputs
     
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputAverages', PointerParam,
                       pointerClass='SetOfAverages',
                       label="Input averages", important=True,
@@ -68,29 +76,33 @@
 
     def createOutputStep(self):
         inputSet = self.inputAverages.get()
         avgSet = self._createSetOfAverages()
 
         avgSet.copyInfo(inputSet)
         avgSet.copyItems(inputSet, updateItemCallback=self._setFileName)
-        self._defineOutputs(outputAverages=avgSet)
+        self._defineOutputs(**{outputs.outputAverages.name: avgSet})
         self._defineTransformRelation(inputSet, avgSet)
 
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         """ Just overwrite the default behaviour of the base class. """
         return []
 
     def _summary(self):
-        summary = ['']
+        summary = []
+
+        if hasattr(self, "outputAverages"):
+            summary.append('Class averages were aligned by relion_image_handler '
+                           'using their center of mass.')
+
         return summary
 
     def _methods(self):
-        return ['Class averages were aligned by relion_image_handler '
-                'using their center of mass.']
+        return []
 
     def _getStackFn(self):
         return self._getPath('centered_averages.mrcs')
 
     def _setFileName(self, item, row):
         self._counter = getattr(self, '_counter', 0)
         self._counter += 1
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_classify2d.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_classify2d.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,29 +20,35 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+from enum import Enum
+
 from pyworkflow.constants import PROD
 from pwem.constants import ALIGN_2D
 from pwem.objects import SetOfClasses2D
 from pwem.protocols import ProtClassify2D
 
 import relion.convert as convert
-from relion import Plugin
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputClasses = SetOfClasses2D
+
+
 class ProtRelionClassify2D(ProtRelionBase, ProtClassify2D):
     """ This protocol runs Relion 2D classification."""
 
     _label = '2D classification'
     _devStatus = PROD
+    _possibleOutputs = outputs
     IS_2D = True
     OUTPUT_TYPE = SetOfClasses2D
     
     def __init__(self, **args):        
         ProtRelionBase.__init__(self, **args)
         
     def _initialize(self):
@@ -70,26 +76,24 @@
     # --------------------------- STEPS functions -----------------------------
     def _fillClassesFromIter(self, clsSet, iteration):
         """ Create the SetOfClasses2D from a given iteration. """
         classLoader = convert.ClassesLoader(self, ALIGN_2D)
         classLoader.fillClassesFromIter(clsSet, iteration)
 
     def createOutputStep(self):
-        partSet = self.inputParticles.get()       
-        
-        classes2D = self._createSetOfClasses2D(partSet)
+        classes2D = self._createSetOfClasses2D(self.inputParticles)
         self._fillClassesFromIter(classes2D, self._lastIter())
         
-        self._defineOutputs(outputClasses=classes2D)
+        self._defineOutputs(**{outputs.outputClasses.name: classes2D})
         self._defineSourceRelation(self.inputParticles, classes2D)
         
     # --------------------------- INFO functions ------------------------------
     def _validateNormal(self):
         errors = []
-        if Plugin.IS_GT31() and self.useGradientAlg and self.numberOfMpi > 1:
+        if self.useGradientAlg and self.numberOfMpi > 1:
             errors.append("Gradient refinement (running the VDAM algorithm) "
                           "is not supported together with MPI")
 
         return errors
     
     def _validateContinue(self):
         errors = []
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_classify3d.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_classify3d.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,35 +19,43 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from enum import Enum
 from emtable import Table
 
 from pyworkflow.constants import PROD
 from pwem.constants import ALIGN_PROJ
+from pwem.objects import SetOfClasses3D, SetOfVolumes
 from pwem.protocols import ProtClassify3D
 
 import relion.convert as convert
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputClasses = SetOfClasses3D
+    outputVolumes = SetOfVolumes
+
+
 class ProtRelionClassify3D(ProtClassify3D, ProtRelionBase):
     """
     Protocol to classify 3D using Relion Bayesian approach.
     Relion employs an empirical Bayesian approach to refinement of (multiple)
     3D reconstructions or 2D class averages in electron cryo-EM. Many
     parameters of a statistical model are learned from the data, which
     leads to objective and high-quality results.
     """
 
     _label = '3D classification'
     _devStatus = PROD
+    _possibleOutputs = outputs
     CHANGE_LABELS = ['rlnChangesOptimalOrientations',
                      'rlnChangesOptimalOffsets',
                      'rlnOverallAccuracyRotations',
                      'rlnOverallAccuracyTranslationsAngst',
                      'rlnChangesOptimalClasses']
     
     def __init__(self, **args):        
@@ -83,32 +91,32 @@
                 args['--allow_coarser_sampling'] = ''
 
         else:
             args['--skip_align'] = ''
     
     # -------------------------- STEPS functions ------------------------------
     def createOutputStep(self):
-        partSet = self.inputParticles.get()
+        partSet = self.inputParticles
         classes3D = self._createSetOfClasses3D(partSet)
         self._fillClassesFromIter(classes3D, self._lastIter())
         
-        self._defineOutputs(outputClasses=classes3D)
-        self._defineSourceRelation(self.inputParticles, classes3D)
+        self._defineOutputs(**{outputs.outputClasses.name: classes3D})
+        self._defineSourceRelation(partSet, classes3D)
 
         # create a SetOfVolumes and define its relations
         volumes = self._createSetOfVolumes()
-        volumes.setSamplingRate(partSet.getSamplingRate())
+        volumes.setSamplingRate(partSet.get().getSamplingRate())
         
         for class3D in classes3D:
             vol = class3D.getRepresentative()
             vol.setObjId(class3D.getObjId())
             volumes.append(vol)
         
-        self._defineOutputs(outputVolumes=volumes)
-        self._defineSourceRelation(self.inputParticles, volumes)
+        self._defineOutputs(**{outputs.outputVolumes.name: volumes})
+        self._defineSourceRelation(partSet, volumes)
         
         if not self.doContinue:
             self._defineSourceRelation(self.referenceVolume, classes3D)
             self._defineSourceRelation(self.referenceVolume, volumes)
     
     # -------------------------- INFO functions -------------------------------
     def _validateNormal(self):
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_compress_movies.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_compress_movies.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,15 +123,17 @@
             args += " --eer_grouping %d" % self.eerGroup
             args += " --eer_upsampling %d" % (self.eerSampling.get() + 1)
 
         self.runJob('relion_convert_to_tiff', args, cwd=self._getTmpPath())
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
-        summary = []
+        summary = ["Movies compressed by relion_convert_to_tiff, "
+                   "compression type: %s" % self.getEnumText('compression')]
+
         return summary
 
     def _citations(self):
         return ['Zivanov2019']
 
     def _validate(self):
         errors = []
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_create_mask3d.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_create_mask3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,30 +21,36 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import math
+from enum import Enum
 
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
 from pwem.protocols import ProtCreateMask3D
 from pwem.objects import VolumeMask
 
 import relion.convert as convert
 from ..constants import MASK_AND
 
 
+class outputs(Enum):
+    outputMask = VolumeMask
+
+
 class ProtRelionCreateMask3D(ProtCreateMask3D):
     """ This protocols creates a 3D mask using Relion.
     The mask is created from a 3d volume or by comparing two input volumes.
     """
     _label = 'create 3d mask'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Mask generation')
         form.addParam('inputVolume', params.PointerParam,
                       pointerClass="Volume",
                       label="Input volume",
@@ -155,15 +161,15 @@
         return [self.maskFile]
 
     def createOutputStep(self):
         volMask = VolumeMask()
         volMask.setFileName(self.maskFile)
         volMask.setSamplingRate(self.inputVolume.get().getSamplingRate())
 
-        self._defineOutputs(outputMask=volMask)
+        self._defineOutputs(**{outputs.outputMask.name: volMask})
         self._defineSourceRelation(self.inputVolume, self.outputMask)
         
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
 
         if self.doCompare:
@@ -173,19 +179,19 @@
             if not math.isclose(pixVol1, pixVol2, abs_tol=0.001):
                 errors.append('Pixel size should be the same for both input volumes.')
 
         return errors
 
     def _summary(self):
         messages = [
-            "Created a mask from input volume using threshold %0.3f"
+            "Created a mask from input volume using threshold *%0.5f*"
             % self.threshold.get(),
             "*Mask processing*",
-            "   Extend by %d pixels" % self.extend,
-            "   Apply soft edge of %d pixels" % self.edge]
+            "   Extend by *%d* pixels" % self.extend,
+            "   Apply soft edge of *%d* pixels" % self.edge]
         if self.doInvert:
             messages.append("   Inverted")
 
         return messages
 
     def _citations(self):
         return []
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_crop_resize.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_crop_resize.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 
 import pyworkflow.protocol.params as params
 import pyworkflow.utils as pwutils
 from pyworkflow.constants import PROD
 from pwem.protocols import ProtPreprocessVolumes
 from pwem.emlib.image import ImageHandler
 from pwem.objects import Volume
+from pwem.convert import Ccp4Header
 
 
 class ProtRelionResizeVolume(ProtPreprocessVolumes):
     """ This protocol rescales/resizes 3D volumes using relion_image_handler. """
 
     _label = 'crop/resize volumes'
     _devStatus = PROD
@@ -133,29 +134,33 @@
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         errors = []
 
         if not self.doRescale and not self.doResize:
             errors.append("You have to select at least one option!")
 
-        if self.doResize:
-            if not self.resizeSize.get() % 2 == 0:
-                errors.append("Only even box sizes are allowed!")
+        if self.doResize and not (self.resizeSize.get() % 2 == 0):
+            errors.append("Only even box sizes are allowed!")
 
         return errors
 
     def _summary(self):
         messages = []
 
-        if self.doRescale:
-            messages.append("- Rescaled volumes to pixel size of %0.3f"
-                            % self.rescaleSamplingRate.get())
-        if self.doResize:
-            messages.append("- Resized volumes to box size of %d"
-                            % self.resizeSize.get())
+        if hasattr(self, "outputVol"):
+            if self.doResize:
+                messages.append(f"Resized volumes to box size of "
+                                f"*{self.resizeSize.get()}* px")
+            if self.doRescale:
+                messages.append(f"The output pixel size might be different than the "
+                                f"requested {self.rescaleSamplingRate.get()}A "
+                                f"due to rounding of the box size "
+                                f"to an even number by RELION")
+        else:
+            messages.append("Output is not ready")
 
         return messages
 
     # -------------------------- UTILS functions ------------------------------
     def _convertVol(self, vol, index):
         ih = ImageHandler()
         fn = vol.getFileName()
@@ -163,10 +168,14 @@
             newFn = self._getFileName('input_vol', volId=index)
             ih.convert(fn, newFn)
             return newFn
         return fn
 
     def _getNewSampling(self):
         if self.doRescale:
-            return self.rescaleSamplingRate.get()
+            ccp4header = Ccp4Header(self._getFileName('output_vol', volId=1),
+                                    readHeader=True)
+            sampling, _, _ = ccp4header.getSampling()
+
+            return sampling
         else:
             return self.inputVolumes.get().getSamplingRate()
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_ctf_refinement.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_ctf_refinement.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,55 +20,63 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
 
+from enum import Enum
+
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
 from pwem.constants import ALIGN_PROJ
+from pwem.objects import SetOfParticles
 from pwem.protocols import ProtParticles
 
 import relion
 import relion.convert as convert
 from relion.convert.convert31 import Reader, OpticsGroups
 from .protocol_base import ProtRelionBase
 
 from ..objects import CtfRefineGlobalInfo
 
 
+class outputs(Enum):
+    outputParticles = SetOfParticles
+
+
 class ProtRelionCtfRefinement(ProtParticles, ProtRelionBase):
     """ Wrapper protocol for the Relion's CTF refinement. """
     _label = 'ctf refinement'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
     def _initialize(self):
         self._createFilenameTemplates()
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
         myDict = {
             'output_star': self._getExtraPath("particles_ctf_refine.star"),
             'ctf_sqlite': self._getExtraPath("ctf_analyze.sqlite"),
-            'mag_obs_x': self._getExtraPath("mag_disp_x_optics-group_%(og)d.mrc:mrc"),
-            'mag_obs_y': self._getExtraPath("mag_disp_y_optics-group_%(og)d.mrc:mrc"),
-            'mag_fit_x': self._getExtraPath("mag_disp_x_fit_optics-group_%(og)d.mrc:mrc"),
-            'mag_fit_y': self._getExtraPath("mag_disp_y_fit_optics-group_%(og)d.mrc:mrc"),
-            'tetrafoil_it_fit': self._getExtraPath("aberr_delta-phase_iter-fit_optics-group_%(og)d_N-4.mrc:mrc"),
-            'tetrafoil_fit': self._getExtraPath("aberr_delta-phase_lin-fit_optics-group_%(og)d_N-4.mrc:mrc"),
-            'tetrafoil_residual_fit': self._getExtraPath("aberr_delta-phase_lin-fit_optics-group_%(og)d_N-4_residual.mrc:mrc"),
-            'tetrafoil_obs': self._getExtraPath("aberr_delta-phase_per-pixel_optics-group_%(og)d.mrc:mrc"),
-            'beamtilt_it_fit': self._getExtraPath("beamtilt_delta-phase_iter-fit_optics-group_%(og)d.mrc:mrc"),
-            'beamtilt_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d.mrc:mrc"),
-            'trefoil_it_fit': self._getExtraPath("beamtilt_delta-phase_iter-fit_optics-group_%(og)d_N-3.mrc:mrc"),
-            'trefoil_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d_N-3.mrc:mrc"),
-            'trefoil_residual_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d_N-3_residual.mrc:mrc"),
-            'beamtilt_obs': self._getExtraPath("beamtilt_delta-phase_per-pixel_optics-group_%(og)d.mrc:mrc")
+            'mag_obs_x': self._getExtraPath("mag_disp_x_optics-group_%(og)d.mrc"),
+            'mag_obs_y': self._getExtraPath("mag_disp_y_optics-group_%(og)d.mrc"),
+            'mag_fit_x': self._getExtraPath("mag_disp_x_fit_optics-group_%(og)d.mrc"),
+            'mag_fit_y': self._getExtraPath("mag_disp_y_fit_optics-group_%(og)d.mrc"),
+            'tetrafoil_it_fit': self._getExtraPath("aberr_delta-phase_iter-fit_optics-group_%(og)d_N-4.mrc"),
+            'tetrafoil_fit': self._getExtraPath("aberr_delta-phase_lin-fit_optics-group_%(og)d_N-4.mrc"),
+            'tetrafoil_residual_fit': self._getExtraPath("aberr_delta-phase_lin-fit_optics-group_%(og)d_N-4_residual.mrc"),
+            'tetrafoil_obs': self._getExtraPath("aberr_delta-phase_per-pixel_optics-group_%(og)d.mrc"),
+            'beamtilt_it_fit': self._getExtraPath("beamtilt_delta-phase_iter-fit_optics-group_%(og)d.mrc"),
+            'beamtilt_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d.mrc"),
+            'trefoil_it_fit': self._getExtraPath("beamtilt_delta-phase_iter-fit_optics-group_%(og)d_N-3.mrc"),
+            'trefoil_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d_N-3.mrc"),
+            'trefoil_residual_fit': self._getExtraPath("beamtilt_delta-phase_lin-fit_optics-group_%(og)d_N-3_residual.mrc"),
+            'beamtilt_obs': self._getExtraPath("beamtilt_delta-phase_per-pixel_optics-group_%(og)d.mrc")
         }
 
         self._updateFilenamesDict(myDict)
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
@@ -254,25 +262,24 @@
     def createOutputStep(self):
         imgSet = self.inputParticles.get()
         outImgSet = self._createSetOfParticles()
         outImgSet.copyInfo(imgSet)
         outImgsFn = self._getFileName("output_star")
         imgSet.setAlignmentProj()
 
-        # self._optics = convert.getOpticsDict(outImgsFn)
         mdIter = convert.Table.iterRows('particles@' + outImgsFn,
-                                        key='rlnImageId')
+                                        key='rlnImageId', types=convert.LABELS_DICT)
         outImgSet.copyItems(imgSet,
                             updateItemCallback=self._updateItem,
                             itemDataIterator=mdIter,
                             doClone=False)
         og = OpticsGroups.fromStar(outImgsFn)
         og.toImages(outImgSet)
 
-        self._defineOutputs(outputParticles=outImgSet)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
         self._defineTransformRelation(self.inputParticles, outImgSet)
 
     def createGlobalInfo(self, filename):
         pwutils.cleanPath(filename)
         ctfInfo = CtfRefineGlobalInfo(filename=filename)
         ctfInfo.loadFromParticles(self.inputParticles.get(),
                                   self.outputParticles)
@@ -286,15 +293,15 @@
         # Reader.rowToAcquisition(self._optics[row.rlnOpticsGroup],
         #                         particle.getAcquisition())
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
         if self.estimateAnisoMag:
-            summary.append("Estimate anisotropic Magnification: *Yes*")
+            summary.append("Estimate anisotropic magnification: *Yes*")
         else:
             if self.doCtfFitting:
                 summary.append("CTF parameter fitting: *Yes*")
                 for p in ['fitPhaseShift', 'fitDefocus', 'fitAstig', 'fitBfactor']:
                     summary.append("   - %s: *%s*" % (self.getParam(p).getLabel(),
                                                       self.getEnumText(p)))
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_estimate_gain.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_estimate_gain.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         pass
 
     def _stepsCheck(self):
         pass
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
-        summary = []
+        summary = ["Using relion_convert_to_tiff to estimate gain reference"]
         return summary
 
     def _citations(self):
         return ['Zivanov2019']
 
     def _validate(self):
         errors = []
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_expand_symmetry.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_expand_symmetry.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,33 +19,40 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from enum import Enum
 from emtable import Table
 
 from pyworkflow.protocol.params import StringParam
 from pyworkflow.constants import PROD
 from pyworkflow.object import String
 from pwem.constants import ALIGN_PROJ
 from pwem.protocols import ProtProcessParticles
+from pwem.objects import SetOfParticles
 
 import relion.convert as convert
 
+
+class outputs(Enum):
+    outputParticles = SetOfParticles
+
  
 class ProtRelionExpandSymmetry(ProtProcessParticles):
     """ This protocols wraps relion_particle_symmetry_expand program.
 
     Given an input set of particles with angular assignment,
     expand the set by applying a pseudo-symmetry.
     """
     _label = 'expand symmetry'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineProcessParams(self, form):
         form.addParam('symmetryGroup', StringParam, default="c1",
                       label='Symmetry group',
                       help='See [[https://relion.readthedocs.io'
                            '/en/latest/Reference/Conventions.html#symmetry]'
@@ -90,15 +97,15 @@
 
         reader = convert.createReader()
         reader.readSetOfParticles(
             outImagesMd, partSet,
             alignType=ALIGN_PROJ,
             postprocessImageRow=self._postprocessImageRow)
 
-        self._defineOutputs(outputParticles=partSet)
+        self._defineOutputs(**{outputs.outputParticles.name: partSet})
         self._defineSourceRelation(imgSet, partSet)
 
     # -------------------------- INFO functions -------------------------------
     def _summary(self):
         summary = []
         if not hasattr(self, 'outputParticles'):
             summary.append("Output particles not ready yet.")
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_export_coords.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_coords.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_export_ctf.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_ctf.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,49 +89,49 @@
 
         psd = inputCTF.getFirstItem().getPsdFile()
         hasPsd = psd and os.path.exists(psd)
 
         if hasPsd:
             psdPath = self._getExportPath('PSD')
             pwutils.makePath(psdPath)
-            print("Writing PSD files to %s" % psdPath)
+            self.info(f"Writing PSD files to {psdPath}")
 
         for ctf in inputCTF:
             # Get the corresponding micrograph
             mic = ctfMicSet[ctf.getObjId()]
             if mic is None:
-                print("Skipping CTF id: %s, it is missing from input "
-                      "micrographs. " % ctf.getObjId())
+                self.warning(f"Skipping CTF id: {ctf.getObjId()}, it is missing from input "
+                             f"micrographs. ")
                 continue
 
             micFn = mic.getFileName()
             if not os.path.exists(micFn):
-                print("Skipping micrograph %s, it does not exists. " % micFn)
+                self.warning(f"Skipping micrograph {micFn}, it does not exists.")
                 continue
 
             mic2 = mic.clone()
             mic2.setCTF(ctf)
             if hasPsd:
                 psdFile = ctf.getPsdFile()
                 newPsdFile = os.path.join(psdPath,
                                           '%s_psd.mrc' % pwutils.removeExt(mic.getMicName()))
                 if not os.path.exists(psdFile):
-                    print("PSD file %s does not exits" % psdFile)
-                    print("Skipping micrograph %s" % micFn)
+                    self.warning(f"PSD file {psdFile} does not exits\n"
+                                 f"Skipping micrograph {micFn}")
                     continue
                 pwutils.copyFile(psdFile, newPsdFile)
                 # PSD path is relative to Export dir
                 newPsdFile = os.path.relpath(newPsdFile, self._getExportPath())
                 ctf.setPsdFile(newPsdFile)
             else:
                 # remove pointer to non-existing psd file
                 ctf.setPsdFile(None)
             micSet.append(mic2)
 
-        print("Writing set: %s to: %s" % (inputCTF, self._getStarFile()))
+        self.info(f"Writing set: {inputCTF} to: {self._getStarFile()}")
 
         micDir = self._getExportPath('Micrographs')
         pwutils.makePath(micDir)
         starWriter = convert.createWriter(rootDir=self._getExportPath(),
                                           outputDir=micDir,
                                           useBaseName=True)
         starWriter.writeSetOfMicrographs(micSet, self._getStarFile())
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_export_particles.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_export_particles.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_extract_particles.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_extract_particles.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,15 +52,15 @@
     def __init__(self, **kwargs):
         ProtExtractParticles.__init__(self, **kwargs)
 
     # -------------------------- DEFINE param functions -----------------------
     def _definePreprocessParams(self, form):
         form.addParam('boxSize', params.IntParam,
                       label='Particle box size (px)',
-                      validators=[params.Positive],
+                      allowsPointers=True,
                       help='This is size of the boxed particles (in pixels).')
 
         form.addParam('doRescale', params.BooleanParam, default=False,
                       label='Rescale particles?',
                       help='If set to Yes, particles will be re-scaled. '
                            'Note that the re-scaled size below will be in '
                            'the down-scaled images.')
@@ -68,21 +68,19 @@
         form.addParam('rescaledSize', params.IntParam, default=128,
                       validators=[params.Positive],
                       condition='doRescale',
                       label='Re-scaled size (px)',
                       help='Final size in pixels of the extracted particles. '
                            'The provided value should be an even number. ')
 
-        if relion.Plugin.IS_GT31():
-            form.addParam('saveFloat16', params.BooleanParam, default=False,
-                          expertLevel=params.LEVEL_ADVANCED,
-                          label="Write output in float16?",
-                          help="Relion can write output images in float16 "
-                               "MRC (mode 12) format to save disk space. "
-                               "By default, float32 format is used.")
+        form.addParam('saveFloat16', params.BooleanParam, default=True,
+                      label="Write output in float16?",
+                      help="Relion can write output images in float16 "
+                           "MRC (mode 12) format to save disk space. "
+                           "By default, float32 format is used.")
 
         form.addSection(label='Preprocess')
 
         form.addParam('doInvert', params.BooleanParam, default=None,
                       label='Invert contrast?',
                       help='Invert the contrast if your particles are black '
                            'over a white background.  Xmipp, Spider, Relion '
@@ -152,27 +150,27 @@
         pass  # used to avoid some streaming functions
 
     # -------------------------- STEPS functions ------------------------------
     def convertInputStep(self, micsId):
         self.info("Relion version:")
         self.runJob("relion_refine --version", "", numberOfMpi=1)
         self.info("Detected version from config: %s"
-                  % relion.Plugin.getActiveVersion())
+                  % Plugin.getActiveVersion())
 
     def _convertCoordinates(self, mic, coordList):
         relion.convert.writeMicCoordinates(
             mic, coordList, self._getMicPos(mic), getPosFunc=self._getPos)
 
     def _extractMicrograph(self, mic, params):
         """ Extract particles from one micrograph, ignore if the .star
         with the coordinates is not present. """
         self._extractMicrographList([mic], params)
 
     def _extractMicrographList(self, micList, params):
-        if not micList:  # do not process when empty list, need to check this properly
+        if len(micList) <= 0:  # do not process when empty list, need to check this properly
             return
 
         workingDir = self.getWorkingDir()
         micsStar = self._getMicsStar(micList)
         og = OpticsGroups.fromImages(self.getInputMicrographs())
         starWriter = relion.convert.createWriter(rootDir=workingDir,
                                                  outputDir=self._getTmpPath(),
@@ -204,33 +202,32 @@
             errors.append("Background diameter for normalization should "
                           "be equal or less than the box size.")
 
         if self.doRescale and self.rescaledSize.get() % 2 == 1:
             errors.append("Only re-scaling to even-sized images is allowed "
                           "in RELION.")
 
-        if self.hasAttribute('saveFloat16') and self.saveFloat16:
-            errors.append("MRC float16 format is not yet supported by XMIPP, "
-                          "so you cannot use this option.")
-
         return errors
 
     def _citations(self):
         return ['Scheres2012b']
 
     def _summary(self):
         summary = list()
         summary.append("Micrographs source: %s"
                        % self.getEnumText("downsampleType"))
-        summary.append("Particle box size: %d" % self.boxSize)
+        summary.append("Particle box size: *%d* px" % self.boxSize)
+
+        if self.doRescale:
+            summary.append("Rescaled box size: *%d* px" % self.rescaledSize)
 
         if not hasattr(self, 'outputParticles'):
             summary.append("Output images not ready yet.")
         else:
-            summary.append("Particles extracted: %d" %
+            summary.append("Particles extracted: *%d*" %
                            self.outputParticles.getSize())
 
         return summary
 
     def _methods(self):
         methodsMsgs = []
 
@@ -282,15 +279,15 @@
         # - the micrographs (or links) and coordinate files will be in 'extra'
         # - coordinate files have the 'coords.star' suffix
         params = ' --coord_dir "."'
         params += ' --coord_suffix .coords.star'
         params += ' --part_dir "." --extract '
         params += ' --extract_size %d' % self.boxSize
 
-        if Plugin.IS_GT31() and self.saveFloat16:
+        if self.saveFloat16:
             params += " --float16 "
 
         if self.backDiameter <= 0:
             diameter = self.boxSize.get() * 0.75
         else:
             diameter = self.backDiameter.get()
 
@@ -349,24 +346,24 @@
             pwutils.moveFile(stackFile, endStackFile)
 
             for part in partsTable:
                 pos = (int(float(part.rlnCoordinateX)),
                        int(float(part.rlnCoordinateY)))
 
                 if pos in posSet:
-                    print("Duplicate coordinate at: %s, IGNORED. " % str(pos))
+                    self.warning(f"Duplicate coordinate at: {str(pos)}, IGNORED.")
                     coord = None
                 else:
                     coord = coordDict.get(pos, None)
 
                 if coord is not None:
                     # scale the coordinates according to particles dimension.
                     coord.scale(self.getBoxScale())
                     p.copyObjId(coord)
-                    idx, fn = relionToLocation(part.rlnImageName)
+                    idx, _ = relionToLocation(part.rlnImageName)
                     p.setLocation(idx, endStackFile)
                     p.setCoordinate(coord)
                     p.setMicId(mic.getObjId())
                     p.setCTF(mic.getCTF())
                     p._rlnOpticsGroup.set(ogNumber)
                     outputParts.append(p)
                     posSet.add(pos)
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_gentle_clean.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_gentle_clean.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 # **************************************************************************
 
 import os
 import re
 from glob import glob
 
 from pyworkflow.protocol import Protocol
-from pyworkflow.constants import BETA
+from pyworkflow.constants import PROD
 from pyworkflow.protocol.params import LabelParam
 
 
 class ProtRelionCleanJobs(Protocol):
     """
     Run Relion gentle clean procedure for the whole project.
     """
     _label = 'clean project'
-    _devStatus = BETA
+    _devStatus = PROD
 
     def __init__(self, **kwargs):
         Protocol.__init__(self, **kwargs)
         self.moveDict = dict()
 
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
@@ -122,15 +122,15 @@
             elif prot in baseProts:
                 for protDir in protDict[prot]:
                     files = sorted(glob(os.path.join(prjPath, protDir, "relion_?t???_*")))
                     # Move all files except for the last iteration
                     self.debug(files)
                     result = None
                     if files:
-                        s = re.search("_?t(\d{3})_", files[-1])
+                        s = re.search(r"_?t(\d{3})_", files[-1])
                         if s:
                             # group 1 is 3 digits iteration number
                             result = "relion_[ic]t%03d_" % int(s.group(1))
                             self.info("I'll keep files: %s from %s" % (result, protDir))
                     if result:
                         for f in files:
                             match = re.search(result, f)
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_initialmodel.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_postprocess.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # **************************************************************************
 # *
-# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk) [1]
-# *              J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [2]
+# * Authors:     Josue Gomez Blanco     (josue.gomez-blanco@mcgill.ca) [1]
+# *              J.M. de la Rosa Trevin (delarosatrevin@scilifelab.se) [2]
 # *
-# * [1] MRC Laboratory of Molecular Biology, MRC-LMB
+# * [1] Department of Anatomy and Cell Biology, McGill University
 # * [2] SciLifeLab, Stockholm University
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
@@ -21,371 +21,330 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+
+import os
+from enum import Enum
 from emtable import Table
 
-from pwem.constants import ALIGN_PROJ
-from pwem.protocols import ProtInitialVolume
-from pwem.objects import Volume
+import pyworkflow.utils as pwutils
+import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
-from pyworkflow.protocol.params import (PointerParam, FloatParam,
-                                        LabelParam, IntParam,
-                                        EnumParam, StringParam,
-                                        BooleanParam)
+from pwem.protocols import ProtAnalysis3D
+from pwem.emlib.image import ImageHandler
+from pwem.objects import Volume
 
-import relion
 import relion.convert as convert
 from .protocol_base import ProtRelionBase
 
 
-class ProtRelionInitialModel(ProtInitialVolume, ProtRelionBase):
-    """ This protocols creates a 3D initial model using Relion.
+class outputs(Enum):
+    outputVolume = Volume
 
-    Generate a 3D initial model _de novo_ from 2D particles using
-    Relion Stochastic Gradient Descent (SGD) algorithm.
+
+class ProtRelionPostprocess(ProtAnalysis3D, ProtRelionBase):
+    """
+    Relion post-processing protocol for automated masking,
+    overfitting estimation, MTF-correction and B-factor sharpening.
     """
-    _label = '3D initial model'
+    _label = 'post-processing'
     _devStatus = PROD
-    IS_CLASSIFY = False
-    IS_3D_INIT = True
-    IS_2D = False
-    CHANGE_LABELS = ['rlnChangesOptimalOrientations',
-                     'rlnChangesOptimalOffsets']
-
-    def __init__(self, **args):
-        ProtRelionBase.__init__(self, **args)
-
-    def _initialize(self):
-        """ This function is mean to be called after the
-        working dir for the protocol have been set.
-        (maybe after recovery from mapper)
-        """
-        self._createFilenameTemplates()
-        self._createIterTemplates()
-        if not self.doContinue:
-            self.continueRun.set(None)
-        self.maskZero = False
-        self.copyAlignment = False
-        self.hasReferenceCTFCorrected = False
+    _possibleOutputs = outputs
+
+    def _getInputPath(self, *paths):
+        return self._getPath('input', *paths)
+
+    def _createFilenameTemplates(self):
+        """ Centralize how files are called for iterations and references. """
+        myDict = {
+            'finalVolume': self._getInputPath("relion_class001.mrc"),
+            'half1': self._getInputPath("relion_half1_class001_unfil.mrc"),
+            'half2': self._getInputPath("relion_half2_class001_unfil.mrc"),
+            'mask': self._getInputPath("input_mask.mrc"),
+            'outputVolume': self._getExtraPath('postprocess.mrc')
+        }
+        self._updateFilenamesDict(myDict)
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
-        self._defineConstants()
-
-        self.IS_3D = not self.IS_2D
         form.addSection(label='Input')
-        form.addParam('doContinue', BooleanParam, default=False,
-                      label='Continue from a previous run?',
-                      help='If you set to *Yes*, you should select a previous'
-                           'run of type *%s* class and most of the input '
-                           'parameters will be taken from it.'
-                           % self.getClassName())
-        form.addParam('inputParticles', PointerParam,
-                      pointerClass='SetOfParticles',
-                      condition='not doContinue',
-                      important=True,
-                      label="Input particles",
-                      help='Select the input images from the project.')
-        form.addParam('maskDiameterA', IntParam, default=-1,
-                      label='Particle mask diameter (A)',
-                      help='The experimental images will be masked with a '
-                           'soft circular mask with this <diameter>. '
-                           'Make sure this diameter is not set too small '
-                           'because that may mask away part of the signal! If '
-                           'set to a value larger than the image size no '
-                           'masking will be performed.\n\n'
-                           'The same diameter will also be used for a '
-                           'spherical mask of the reference structures if no '
-                           'user-provided mask is specified.')
-        form.addParam('continueRun', PointerParam,
-                      pointerClass=self.getClassName(),
-                      condition='doContinue', allowsNull=True,
-                      label='Select previous run',
-                      help='Select a previous run to continue from.')
-        form.addParam('continueIter', StringParam, default='last',
-                      condition='doContinue',
-                      label='Continue from iteration',
-                      help='Select from which iteration do you want to '
-                           'continue. If you use *last*, then the last '
-                           'iteration will be used. Otherwise, a valid '
-                           'iteration number should be provided.')
-
-        self.addSymmetry(form)
-
-        form.addSection(label='CTF')
-        form.addParam('continueMsg', LabelParam, default=True,
-                      condition='doContinue',
-                      label='CTF parameters are not available in continue mode')
-        form.addParam('doCTF', BooleanParam, default=True,
-                      label='Do CTF-correction?', condition='not doContinue',
-                      help='If set to Yes, CTFs will be corrected inside the '
-                           'MAP refinement. The resulting algorithm '
-                           'intrinsically implements the optimal linear, or '
-                           'Wiener filter. Note that input particles should '
-                           'contains CTF parameters.')
-        form.addParam('haveDataBeenPhaseFlipped', LabelParam,
-                      condition='not doContinue',
-                      label='Have data been phase-flipped?      '
-                            '(Don\'t answer, see help)',
-                      help='The phase-flip status is recorded and managed by '
-                           'Scipion. \n In other words, when you import or '
-                           'extract particles, \nScipion will record whether '
-                           'or not phase flipping has been done.\n\n'
-                           'Note that CTF-phase flipping is NOT a necessary '
-                           'pre-processing step \nfor MAP-refinement in '
-                           'RELION, as this can be done inside the internal\n'
-                           'CTF-correction. However, if the phases have been '
-                           'flipped, the program will handle it.')
-        form.addParam('ignoreCTFUntilFirstPeak', BooleanParam, default=False,
-                      label='Ignore CTFs until first peak?',
-                      condition='not doContinue',
-                      help='If set to Yes, then CTF-amplitude correction will '
-                           'only be performed from the first peak '
-                           'of each CTF onward. This can be useful if the CTF '
-                           'model is inadequate at the lowest resolution. '
-                           'Still, in general using higher amplitude contrast '
-                           'on the CTFs (e.g. 10-20%) often yields better '
-                           'results. Therefore, this option is not generally '
-                           'recommended.')
-        form.addParam('doCtfManualGroups', BooleanParam, default=False,
-                      label='Do manual grouping ctfs?',
-                      condition='not doContinue',
-                      help='Set this to Yes the CTFs will grouping manually.')
-        form.addParam('defocusRange', FloatParam, default=1000,
-                      label='Defocus range for group creation (in Angstroms)',
-                      condition='doCtfManualGroups and not doContinue',
-                      help='Particles will be grouped by defocus.'
-                           'This parameter is the bin for a histogram.'
-                           'All particles assigned to a bin form a group')
-        form.addParam('numParticles', FloatParam, default=10,
-                      label='minimum size for defocus group',
-                      condition='doCtfManualGroups and not doContinue',
-                      help='If defocus group is smaller than this value, '
-                           'it will be expanded until number of particles '
-                           'per defocus group is reached')
-
-        form.addSection('Optimisation')
-        form.addParam('numberOfIter', IntParam, default=200,
-                      label="Number of VDAM mini-batches",
-                      help="How many iterations (i.e. mini-batches) "
-                           "to perform with the VDAM algorithm?")
-        form.addParam('regularisationParamT', FloatParam,
-                      default=4,
-                      label='Regularisation parameter T',
-                      help='Bayes law strictly determines the relative '
-                           'weight between the contribution of the '
-                           'experimental data and the prior. '
-                           'However, in practice one may need to adjust '
-                           'this weight to put slightly more weight on the '
-                           'experimental data to allow optimal results. '
-                           'Values greater than 1 for this regularisation '
-                           'parameter (T in the JMB2011 paper) put more '
-                           'weight on the experimental data. Values around '
-                           '2-4 have been observed to be useful for 3D '
-                           'initial model calculations.')
-        form.addParam('numberOfClasses', IntParam, default=1,
-                      condition='not doContinue',
-                      label='Number of classes',
-                      help='The number of classes (K) for a multi-reference '
-                           'ab initio SGD refinement. These classes will be '
-                           'made in an unsupervised manner, starting from a '
-                           'single reference in the initial iterations of '
-                           'the SGD, and the references will become '
-                           'increasingly dissimilar during the in between '
-                           'iterations.')
-
-        form.addParam('doFlattenSolvent', BooleanParam, default=True,
-                      condition='not doContinue',
-                      label='Flatten and enforce non-negative solvent?',
-                      help='If set to Yes, the job will apply a spherical '
-                           'mask and enforce all values in the reference '
-                           'to be non-negative.')
-
-        form.addParam('symmetryGroup', StringParam, default='c1',
-                      condition='not doContinue',
-                      label="Symmetry",
-                      help='The initial model is always generated in C1 '
-                           'and then aligned to and symmetrized with the '
-                           'specified point group. If the automatic alignment '
-                           'fails, please manually rotate run_itNNN_class001.mrc '
-                           '(NNN is the number of iterations) so that it '
-                           'conforms the symmetry convention.')
-
-        form.addParam('runInC1', BooleanParam, default=True,
-                      condition='not doContinue',
-                      label='Run in C1 and apply symmetry later?',
-                      help='If set to Yes, the gradient-driven optimisation '
-                           'is run in C1 and the symmetry orientation is searched '
-                           'and applied later. If set to No, the entire '
-                           'optimisation is run in the symmetry point group '
-                           'indicated above.')
-
-        form.addSection('Compute')
-        self._defineComputeParams(form)
-
-        form.addParam('extraParams', StringParam, default='',
-                      label='Additional arguments',
-                      help="In this box command-line arguments may be "
-                           "provided that are not generated by the GUI. This "
-                           "may be useful for testing developmental options "
-                           "and/or expert use of the program, e.g: \n"
-                           "--dont_combine_weights_via_disc\n"
-                           "--verb 1\n"
-                           "--pad 2\n")
-
-        form.addParallelSection(threads=1, mpi=0)
-
-    def addSymmetry(self, container):
-        pass
-
-    # -------------------------- INSERT steps functions -----------------------
-
-    # -------------------------- STEPS functions ------------------------------
-    def _getVolumes(self):
-        """ Return the list of volumes generated.
-        The number of volumes in the list will be equal to
-        the number of classes requested by the user in the protocol. """
-        k = self.numberOfClasses.get()
-        pixelSize = self._getInputParticles().getSamplingRate()
-        lastIter = self._lastIter()
-        volumes = []
-
-        for i in range(1, k + 1):
-            vol = Volume(self._getExtraPath('relion_it%03d_class%03d.mrc')
-                         % (lastIter, i))
-            vol.setSamplingRate(pixelSize)
-            volumes.append(vol)
+        form.addParam('relionInput', params.BooleanParam,
+                      default=True,
+                      expertLevel=params.LEVEL_ADVANCED,
+                      label="Start from Relion refinement?",
+                      help="Set to Yes if you wish to use as input "
+                           "a Relion protocol. Otherwise set it to No")
+        form.addParam('inputHalf1', params.PointerParam, pointerClass='Volume',
+                      label="Input half map 1",
+                      important=True, allowsNull=True,
+                      condition="not relionInput",
+                      help='You might want to provide input half maps manually, '
+                           'in case you did not use 3D auto-refine or multi-body protocol '
+                           'that generates them automatically.')
+        form.addParam('inputHalf2', params.PointerParam, pointerClass='Volume',
+                      label="Input half map 2",
+                      important=True, allowsNull=True,
+                      condition="not relionInput",
+                      help='You might want to provide input half maps manually, '
+                           'in case you did not use 3D auto-refine or multi-body protocol '
+                           'that generates them automatically.')
+
+        form.addParam('protRefine', params.PointerParam,
+                      pointerClass="ProtRefine3D, ProtRelionMultiBody",
+                      condition="relionInput",
+                      label='Select a previous refinement protocol',
+                      help='Select any previous refinement protocol to get the '
+                           '3D half maps. Note that it is recommended that the '
+                           'refinement protocol uses a gold-standard method.')
+        form.addParam('bodyNum', params.IntParam, default=1,
+                      condition="relionInput",
+                      label="Which body to process?",
+                      help="Only relevant if input protocol is 3D multi-body.")
+        form.addParam('solventMask', params.PointerParam,
+                      pointerClass="VolumeMask",
+                      label='Solvent mask',
+                      help="Provide a soft mask where the protein is white "
+                           "(1) and the solvent is black (0). Often, the "
+                           "softer the mask the higher resolution estimates "
+                           "you will get. A soft edge of 5-10 pixels is often "
+                           "a good edge width.")
+        form.addParam('calibratedPixelSize', params.FloatParam, default=0,
+                      label='Calibrated pixel size (A)',
+                      help="Provide the final, calibrated pixel size in "
+                           "Angstroms. If 0, the input pixel size will be used. "
+                           "This value may be different from the pixel-size "
+                           "used thus far, e.g. when you have recalibrated "
+                           "the pixel size using the fit to a PDB model. "
+                           "The X-axis of the output FSC plot will use this "
+                           "calibrated value.")
+
+        form.addSection(label='Sharpening')
+        group = form.addGroup('MTF')
+        group.addParam('mtf', params.FileParam,
+                       label='MTF of the detector',
+                       help='User-provided STAR-file with the MTF-curve '
+                            'of the detector. Use the wizard to load one '
+                            'of the predefined ones provided at:\n'
+                            '- [[https://www3.mrc-lmb.cam.ac.uk/relion/index.php/'
+                            'FAQs#Where_can_I_find_MTF_curves_for_typical_detectors.3F]'
+                            '[Relion\'s Wiki FAQs]]\n'
+                            ' - [[https://www.gatan.com/techniques/cryo-em#MTF][Gatan\'s website]]\n\n'
+                            'Relion param: *--mtf*')
+        group.addParam('origPixelSize', params.FloatParam,
+                       default=-1.0,
+                       label='Original detector pixel size (A)',
+                       help='This is the original pixel size (in Angstroms)'
+                            ' in the raw (non-super-resolution!) micrographs')
+
+        form.addParam('doAutoBfactor', params.BooleanParam, default=True,
+                      label='Estimate B-factor automatically?',
+                      help='If set to Yes, then the program will use the '
+                           'automated procedure described by Rosenthal and '
+                           'Henderson (2003, JMB) to estimate an overall '
+                           'B-factor for your map, and sharpen it accordingly.')
+        line = form.addLine('B-factor resolution (A): ',
+                            condition='doAutoBfactor',
+                            help='There are the frequency (in Angstroms), '
+                                 'lowest and highest, that will be included in '
+                                 'the linear fit of the Guinier plot as '
+                                 'described in Rosenthal and Henderson '
+                                 '(2003, JMB).')
+        line.addParam('bfactorLowRes', params.FloatParam,
+                      default=10.0, label='low')
+        line.addParam('bfactorHighRes', params.FloatParam,
+                      default=0.0, label='high')
+        form.addParam('bfactor', params.FloatParam, default=-350,
+                      condition='not doAutoBfactor',
+                      label='Provide B-factor:',
+                      help='User-provided B-factor (in A^2) for map '
+                           'sharpening, e.g. -400. Use negative values for '
+                           'sharpening. Be careful: if you over-sharpen\n'
+                           'your map, you may end up interpreting noise for '
+                           'signal!\n'
+                           'Relion param: *--adhoc_bfac*')
+
+        form.addSection(label='Filtering')
+        form.addParam('skipFscWeighting', params.BooleanParam, default=False,
+                      label='Skip FSC-weighting for sharpening?',
+                      help='If set to No (the default), then the output map '
+                           'will be low-pass filtered according to the '
+                           'mask-corrected, gold-standard FSC-curve. '
+                           'Sometimes, it is also useful to provide an ad-hoc '
+                           'low-pass filter (option below), as due to local '
+                           'resolution variations some parts of the map may '
+                           'be better and other parts may be worse than the '
+                           'overall resolution as measured by the FSC. In '
+                           'such  cases, set this option to Yes and provide '
+                           'an ad-hoc filter as described below.')
+        form.addParam('lowRes', params.FloatParam, default=5,
+                      condition='skipFscWeighting',
+                      label='Ad-hoc low-pass filter (A):',
+                      help='This option allows one to low-pass filter the map '
+                           'at a user-provided frequency (in Angstroms). When '
+                           'using a resolution that is higher than the '
+                           'gold-standard FSC-reported resolution, take care '
+                           'not to interpret noise in the map for signal.')
+        form.addParam('filterEdgeWidth', params.IntParam, default=2,
+                      expertLevel=params.LEVEL_ADVANCED,
+                      label='Low-pass filter edge width:',
+                      help='Width of the raised cosine on the low-pass filter '
+                           'edge (in resolution shells)\n'
+                           'Relion param: *--filter_edge_width*')
+        form.addParam('randomizeAtFsc', params.FloatParam, default=0.8,
+                      expertLevel=params.LEVEL_ADVANCED,
+                      label='Randomize phases threshold',
+                      help='Randomize phases from the resolution where FSC '
+                           'drops below this value\n'
+                           'Relion param: *--randomize_at_fsc*')
+        form.addParam('forceMask', params.BooleanParam, default=False,
+                      expertLevel=params.LEVEL_ADVANCED,
+                      label='Force mask?',
+                      help='Use the mask even when the masked resolution '
+                           'is worse than the unmasked resolution.')
+
+        form.addParallelSection(threads=0, mpi=0)
+
+    # -------------------------- INSERT steps functions ------------------------
+    def _insertAllSteps(self):
+        if self.relionInput:
+            objsId = [self.protRefine.get().getObjId()]
+        else:
+            objsId = [self.inputHalf1.get().getObjId(),
+                      self.inputHalf2.get().getObjId()]
+        self._createFilenameTemplates()
+        self._defineParamDict()
+        self._insertFunctionStep('convertInputStep', objsId)
+        self._insertFunctionStep('postProcessStep', self.paramDict)
+        self._insertFunctionStep('createOutputStep')
+
+    # -------------------------- STEPS functions -------------------------------
+    def convertInputStep(self, objsId):
+        pwutils.makePath(self._getInputPath())
+        ih = ImageHandler()
+
+        if self.relionInput:
+            protRef = self.protRefine.get()
+
+            if self._isInputMbody():
+                for i, vol in enumerate(protRef.outputVolumes):
+                    if i == self.bodyNum.get()-1:
+                        outVol = vol
+                        self.info("Using multi-body input: %s" % outVol.getHalfMaps())
+                        break
+            else:  # ProtRefine3D
+                outVol = protRef.outputVolume
+
+            newDim = outVol.getXDim()
+            newPix = outVol.getSamplingRate()
+            vols = outVol.getHalfMaps().split(',')
 
-        return volumes
+            for vol, key in zip(vols, ['half1', 'half2']):
+                ih.convert(vol, self._getFileName(key))
+        else:
+            half1 = self.inputHalf1.get()
+            half2 = self.inputHalf2.get()
+            newDim = half1.getXDim()
+            newPix = half1.getSamplingRate()
+
+            ih.convert(half1.getFileName(), self._getFileName('half1'))
+            ih.convert(half2.getFileName(), self._getFileName('half2'))
+
+        convert.convertMask(self.solventMask.get(),
+                            self._getFileName('mask'), newPix, newDim)
+
+    def postProcessStep(self, paramDict):
+        params = ' '.join(['%s %s' % (k, str(v))
+                           for k, v in paramDict.items()])
+        self._runProgram('relion_postprocess', params)
 
     def createOutputStep(self):
-        imgSet = self._getInputParticles()
-        volumes = self._getVolumes()
-
-        outImgSet = self._createSetOfParticles()
-        outImgSet.copyInfo(imgSet)
-        self._fillDataFromIter(outImgSet, self._lastIter())
-
-        if len(volumes) > 1:
-            output = self._createSetOfVolumes()
-            output.setSamplingRate(imgSet.getSamplingRate())
-            for vol in volumes:
-                output.append(vol)
-            self._defineOutputs(outputVolumes=output)
+        volume = Volume()
+        volume.setFileName(self._getFileName('outputVolume'))
+        if not self.relionInput:
+            vol = self.inputHalf1
+        elif self._isInputMbody():
+            vol = self.protRefine.get().outputVolumes
         else:
-            output = volumes[0]
-            self._defineOutputs(outputVolume=output)
-
-        self._defineSourceRelation(self.inputParticles, output)
-        self._defineOutputs(outputParticles=outImgSet)
-        self._defineTransformRelation(self.inputParticles, outImgSet)
-
-        # Run symmetrization for the largest volume if necessary
-        sym = self.symmetryGroup.get()
-        if sym.lower() != "c1" and self.runInC1:
-            inFn = self._getFileName('model', iter=self._lastIter())
-            symFn = self._getPath('volume_sym%s.mrc' % sym)
-            pixSize = imgSet.getSamplingRate()
-
-            self.runJob("relion_align_symmetry",
-                        "--apply_sym --select_largest_class "
-                        "--i %s --o %s --sym %s --angpix %0.5f" % (
-                            inFn, symFn, sym, pixSize))
-
-            def _defineOutputVol(name, fn):
-                vol = Volume()
-                vol.copyInfo(volumes[0])
-                vol.setLocation(fn)
-                self._defineOutputs(**{name: vol})
-
-            _defineOutputVol('outputVolumeSymmetrized', symFn)
+            vol = self.protRefine.get().outputVolume
 
-    # -------------------------- INFO functions -------------------------------
-    def _validateNormal(self):
-        errors = []
-
-        return errors
+        volume.setSamplingRate(self._getOutputPixelSize())
+        self._defineOutputs(**{outputs.outputVolume.name: volume})
+        self._defineSourceRelation(vol, volume)
 
-    def _validateContinue(self):
+    # -------------------------- INFO functions --------------------------------
+    def _validate(self):
         errors = []
-        continueRun = self.continueRun.get()
-        continueRun._initialize()
-        lastIter = continueRun._lastIter()
+        mtfFile = self.mtf.get()
 
-        if self.continueIter.get() == 'last':
-            continueIter = lastIter
-        else:
-            continueIter = int(self.continueIter.get())
-
-        if continueIter > lastIter:
-            errors += ["The iteration from you want to continue must be "
-                       "%01d or less" % lastIter]
+        if mtfFile and not os.path.exists(mtfFile):
+            errors.append("Missing MTF-file '%s'" % mtfFile)
 
         return errors
 
-    def _summaryNormal(self):
+    def _citations(self):
+        return ['Chen2013']
+
+    def _summary(self):
         summary = []
-        it = self._lastIter() or -1
-        if it >= 1:
-            table = Table(fileName=self._getFileName('model', iter=it),
-                          tableName='model_general')
+        postStarFn = self._getExtraPath("postprocess.star")
+        if os.path.exists(postStarFn):
+            table = Table(fileName=postStarFn, tableName='general')
             row = table[0]
-            resol = float(row.rlnCurrentResolution)
-            summary.append("Current resolution: *%0.2f*" % resol)
-        return summary
+            summary.append("Final resolution: *%0.2f A*" %
+                           float(row.rlnFinalResolution))
+            summary.append("B-factor: *%0.2f A\u00B2*" %
+                           float(row.rlnBfactorUsedForSharpening))
 
-    def _summaryContinue(self):
-        summary = ["Continue from iteration %01d" % self._getContinueIter()]
         return summary
 
     # -------------------------- UTILS functions ------------------------------
-    def _setBasicArgs(self, args):
-        """ Return a dictionary with basic arguments. """
-        args.update({'--o': self._getExtraPath('relion'),
-                     '--oversampling': 1,
-                     '--pad': 1,
-                     '--tau2_fudge': self.regularisationParamT.get()
-                     })
-
-        if self.doFlattenSolvent:
-            args['--flatten_solvent'] = ''
-        if not self.doContinue:
-            args['--sym'] = 'C1' if self.runInC1 else self.symmetryGroup.get()
-        if self.skipGridding:
-            args['--skip_gridding'] = ''
-
-        self._setGradArgs(args)
-        self._setSamplingArgs(args)
-
-    def _setGradArgs(self, args):
-        args['--iter'] = self.numberOfIter.get()
-        args['--grad'] = ''
-        args['--K'] = self.numberOfClasses.get()
-
-        if not self.doContinue:
-            args['--denovo_3dref'] = ''
-
-    def _setSamplingArgs(self, args):
-        """ Set sampling related params"""
-        if not self.doContinue:
-            args['--healpix_order'] = 1
-            args['--offset_range'] = 6
-            args['--offset_step'] = 2
-            args['--auto_sampling'] = ''
-
-    def _fillDataFromIter(self, imgSet, iteration):
-        outImgsFn = self._getFileName('data', iter=iteration)
-        imgSet.setAlignmentProj()
-        px = imgSet.getSamplingRate()
-        self.reader = convert.createReader(alignType=ALIGN_PROJ,
-                                           pixelSize=px)
-        mdIter = convert.Table.iterRows('particles@' + outImgsFn, key='rlnImageId')
-        imgSet.copyItems(self._getInputParticles(), doClone=False,
-                         updateItemCallback=self._createItemMatrix,
-                         itemDataIterator=mdIter)
+    def _defineParamDict(self):
+        """ Define all parameters to run relion_postprocess"""
+        inputFn = self._getFileName('half1')
+
+        self.paramDict = {'--i': inputFn,
+                          '--o': self._getExtraPath('postprocess'),
+                          '--angpix': self._getOutputPixelSize(),
+                          '--filter_edge_width': self.filterEdgeWidth.get(),
+                          '--randomize_at_fsc': self.randomizeAtFsc.get(),
+                          '--mask': self._getFileName('mask')
+                          }
+
+        mtfFile = self.mtf.get()
+        if mtfFile:
+            self.paramDict['--mtf'] = mtfFile
+
+        if self.doAutoBfactor:
+            self.paramDict['--auto_bfac'] = ''
+            self.paramDict['--autob_lowres'] = self.bfactorLowRes.get()
+            self.paramDict['--autob_highres'] = self.bfactorHighRes.get()
+        else:
+            self.paramDict['--adhoc_bfac'] = self.bfactor.get()
 
-    def _createItemMatrix(self, item, row):
-        self.reader.setParticleTransform(item, row)
+        if self.skipFscWeighting:
+            self.paramDict['--skip_fsc_weighting'] = ''
+            self.paramDict['--low_pass'] = self.lowRes.get()
+
+        if self.origPixelSize.get() != -1.0:
+            self.paramDict['--mtf_angpix'] = self.origPixelSize.get()
+
+        if self.forceMask:
+            self.paramDict['--force_mask'] = ''
+
+    def _isInputMbody(self):
+        return self.protRefine.get().getClassName() == "ProtRelionMultiBody"
+
+    def _getOutputPixelSize(self):
+        """ Return the output pixel size, using the calibrated
+        pixel size if non zero, or the input one. """
+        if not self.relionInput:
+            volume = self.inputHalf1.get()
+        elif self._isInputMbody():
+            volume = self.protRefine.get().outputVolumes
+        else:
+            volume = self.protRefine.get().outputVolume
+        cps = self.calibratedPixelSize.get()
+        return cps if cps > 0 else volume.getSamplingRate()
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_localres.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_localres.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     This program basically performs a series of post-processing operations
     with a small soft, spherical mask that is moved over the entire map,
     while using phase-randomisation to estimate the convolution effects
     of that mask.
     """
     _label = 'local resolution'
     _devStatus = PROD
+    relionInput = True
 
     def _createFilenameTemplates(self):
         """ Centralize how files are called for iterations and references. """
         myDict = {
                  'half1': self._getInputPath("relion_half1_class001_unfil.mrc"),
                  'half2': self._getInputPath("relion_half2_class001_unfil.mrc"),
                  'outputVolume': self._getExtraPath('relion_locres_filtered.mrc'),
@@ -195,13 +196,7 @@
         if mtfFile:
             self.paramDict['--mtf'] = mtfFile
         if self.origPixelSize.get() != -1.0:
             self.paramDict['--mtf_angpix'] = self.origPixelSize.get()
 
         if self.solventMask.hasValue():
             self.paramDict['--mask'] = self._getFileName('solventMask')
-
-    def _getRelionMapFn(self, fn):
-        return fn.split(':')[0]
-
-    def _getMaskFn(self):
-        return self._getPath('solvent_mask.mrc')
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_motioncor.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_motioncor.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,35 +88,32 @@
                       label='Save non-dose weighted as well?',
                       help='Aligned but non-dose weighted images are '
                            'sometimes useful in CTF estimation, although '
                            'there is no difference in most cases. Whichever '
                            'the choice, CTF refinement job is always done on '
                            'dose-weighted particles.')
 
-        form.addParam('savePSsum', params.BooleanParam, default=False,
+        form.addParam('savePSsum', params.BooleanParam, default=True,
                       label='Save sum of power spectra?',
                       help='Sum of non-dose weighted power spectra '
                            'provides better signal for CTF estimation. '
                            'The power spectra can be used by CTFFIND4 '
                            'but not by GCTF.')
         form.addParam('dosePSsum', params.FloatParam, default=4.0,
                       condition='savePSsum',
                       label='Sum power spectra every e/A2',
                       help='McMullan et al. (Ultramicroscopy, 2015) '
                            'suggests summing power spectra every '
                            '4.0 e/A2 gives optimal Thon rings.')
 
-        if Plugin.IS_GT31():
-            form.addParam('saveFloat16', params.BooleanParam, default=False,
-                          label="Write output in float16?",
-                          expertLevel=params.LEVEL_ADVANCED,
-                          lavel="Write output in float16?",
-                          help="Relion can write output images in float16 "
-                               "MRC (mode 12) format to save disk space. "
-                               "By default, float32 format is used.")
+        form.addParam('saveFloat16', params.BooleanParam, default=True,
+                      label="Write output in float16?",
+                      help="Relion can write output images in float16 "
+                           "MRC (mode 12) format to save disk space. "
+                           "By default, float32 format is used.")
 
         form.addParam('doComputePSD', params.BooleanParam, default=False,
                       label="Compute PSD?",
                       help="If Yes, the protocol will compute for each "
                            "aligned micrograph the PSD using EMAN2.")
 
         form.addParam('doComputeMicThumbnail', params.BooleanParam,
@@ -124,15 +121,15 @@
                       label='Compute micrograph thumbnail?',
                       help='When using this option, we will compute a '
                            'micrograph thumbnail with EMAN2 and keep it with the '
                            'micrograph object for visualization purposes.')
 
         form.addParam('extraParams', params.StringParam, default='',
                       expertLevel=cons.LEVEL_ADVANCED,
-                      label='Additional parameters',
+                      label='Additional arguments',
                       help="Extra parameters for Relion motion correction. ")
 
         form.addSection("Motion")
         form.addParam('bfactor', params.IntParam, default=150,
                       label='Bfactor',
                       help="The B-factor that will be applied to the "
                            "micrographs.")
@@ -215,21 +212,21 @@
                       choices=['1', '2'],
                       display=params.EnumParam.DISPLAY_HLIST,
                       label='EER upsampling',
                       help="EER upsampling (1 = 4K or 2 = 8K). 8K rendering is not "
                            "recommended by Relion. See "
                            "https://relion.readthedocs.io/en/latest/Reference/MovieCompression.html")
 
-        form.addParallelSection(threads=4, mpi=1)
+        form.addParallelSection(threads=4, mpi=0)
 
     # --------------------------- STEPS functions -------------------------------
     def _convertInputStep(self):
         self.info("Relion version:")
         self.runJob("relion_run_motioncorr --version", "", numberOfMpi=1)
-        self.info("Detected version from config: %s" % relion.Plugin.getActiveVersion())
+        self.info("Detected version from config: %s" % Plugin.getActiveVersion())
 
         ProtAlignMovies._convertInputStep(self)
 
     def _processMovie(self, movie):
         movieFolder = self._getOutputMovieFolder(movie)
         inputStar = os.path.join(movieFolder,
                                  '%s_input.star' % self._getMovieRoot(movie))
@@ -241,15 +238,15 @@
         # from the movieFolder
         movie.setFileName(os.path.basename(movie.getFileName()))
         writer.writeSetOfMovies([movie], inputStar)
 
         # The program will run in the movie folder, so let's put
         # the input files relative to that
         args = "--i %s --o output/ " % os.path.basename(inputStar)
-        args += "--use_own "
+        args += "--use_own --skip_logfile "
         args += "--first_frame_sum %d --last_frame_sum %d " % (self._getFrameRange())
         args += "--bin_factor %f --bfactor %d " % (self.binFactor, self.bfactor)
         args += "--angpix %0.5f " % (movie.getSamplingRate())
         args += "--patch_x %d --patch_y %d " % (self.patchX, self.patchY)
         args += "--group_frames %d " % self.groupFrames
         args += "--j %d " % self.numberOfThreads
 
@@ -277,15 +274,15 @@
             if self.saveNonDW:
                 args += "--save_noDW "
 
         if self.isEER:
             args += "--eer_grouping %d " % self.eerGroup
             args += "--eer_upsampling %d " % (self.eerSampling.get() + 1)
 
-        if Plugin.IS_GT31() and self.saveFloat16:
+        if self.saveFloat16:
             args += "--float16 "
 
         if self.extraParams.hasValue():
             args += " " + self.extraParams.get()
 
         try:
             self._runProgram('relion_run_motioncorr', args, cwd=movieFolder)
@@ -295,19 +292,24 @@
             except:
                 self.error("ERROR: Extra work "
                            "(i.e plots, PSD, thumbnail) has failed for %s\n"
                            % movie.getFileName())
 
             self._moveFiles(movie)
         except:
-            print("ERROR processing movie: ", movie.getFileName())
+            self.error(f"ERROR processing movie: {movie.getFileName()}")
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
         summary = []
+
+        if any([hasattr(self, "outputMicrographs"),
+                hasattr(self, "outputMicrographsDoseWeighted")]):
+            summary.append("Ran relion_motioncorr%s" % (" with dose-weighting" if self.doDW else ""))
+
         return summary
 
     def _citations(self):
         return ['Zivanov2019']
 
     def _validate(self):
         errors = []
@@ -353,23 +355,19 @@
                           "EER movies. Please use *EER fractionation* option "
                           "instead.")
 
         # check eman2 plugin
         if self.doComputeMicThumbnail or self.doComputePSD:
             try:
                 from pwem import Domain
-                eman2 = Domain.importFromPlugin('eman2', doRaise=True)
+                _ = Domain.importFromPlugin('eman2', doRaise=True)
             except:
                 errors.append("EMAN2 plugin not found!\nComputing thumbnails "
                               "or PSD requires EMAN2 plugin and binaries installed.")
 
-        if self.hasAttribute('saveFloat16') and self.saveFloat16:
-            errors.append("MRC float16 format is not yet supported by XMIPP, "
-                          "so you cannot use this option.")
-
         return errors
 
     # ------------------------ Extra BASE functions ---------------------------
     def _getNameExt(self, movie, postFix, ext, extra=False):
         fn = self._getMovieRoot(movie) + postFix + '.' + ext
         return self._getExtraPath(fn) if extra else fn
 
@@ -518,16 +516,16 @@
         # Load local motion values only if the patches are more than one
         if self.patchX.get() > 2 and self.patchY.get() > 2:
             try:
                 table = md.Table(fileName=self._getMovieExtraFn(movie, '.star'),
                                  tableName='local_motion_model')
                 coeffs = [row.rlnMotionModelCoeff for row in table]
             except:
-                print("Failed to parse local motion from: %s" %
-                      os.path.abspath(self._getMovieExtraFn(movie, '.star')))
+                self.warning(f"Failed to parse local motion from: "
+                             f"{os.path.abspath(self._getMovieExtraFn(movie, '.star'))}")
                 coeffs = []  # Failed to parse the local motion
             m._rlnMotionModelCoeff = pwobj.String(json.dumps(coeffs))
 
         try:
             table = md.Table(fileName=self._getMovieExtraFn(movie, '.star'),
                              tableName='hot_pixels')
             hotPixels = [(row.rlnCoordinateX, row.rlnCoordinateY) for row in table]
@@ -544,22 +542,22 @@
         if self._createOutputMovies():
             output = self.outputMovies
         elif self._createOutputMicrographs():
             output = self.outputMicrographs
         elif self._createOutputWeightedMicrographs():
             output = self.outputMicrographsDoseWeighted
         else:
-            raise Exception("It does not seem like any output is produced!")
+            raise RuntimeError("It does not seem like any output is produced!")
 
         inputSize = len(self.listOfMovies)
         outputSize = output.getSize()
 
         if outputSize == 0 and inputSize != 0:
-            raise Exception("All movies failed, didn't create outputMicrographs."
-                            "Please review movie processing steps above.")
+            raise RuntimeError("All movies failed, didn't create outputMicrographs."
+                               "Please review movie processing steps above.")
 
         if outputSize < inputSize:
             self.warning(pwutils.yellowStr("WARNING - Failed to align %d movies."
                                            % (inputSize - outputSize)))
 
     def _updateOutputSet(self, outputName, outputSet,
                          state=pwobj.Set.STREAM_OPEN):
@@ -568,14 +566,18 @@
         ogDict = {'rlnMicrographOriginalPixelSize': self.inputMovies.get().getSamplingRate(),
                   'rlnMicrographStartFrame': self.sumFrame0.get()}
 
         if self.isEER:
             ogDict.update({'rlnEERUpsampling': self.eerSampling.get() + 1,
                            'rlnEERGrouping': self.eerGroup.get()})
 
+        gain = self.inputMovies.get().getGain()
+        if gain:
+            ogDict['rlnMicrographGainName'] = gain
+
         if outputName not in self.updatedSets:
             og = OpticsGroups.fromImages(outputSet)
             og.updateAll(**ogDict)
             og.toImages(outputSet)
             self.updatedSets.append(outputName)
 
         ProtAlignMovies._updateOutputSet(self, outputName, outputSet,
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_multibody.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_multibody.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,132 +21,174 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
+from enum import Enum
 from emtable import Table
 
 import pyworkflow.utils as pwutils
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
-from pwem.objects import Volume, Float
+from pwem.objects import Volume, Float, SetOfVolumes, SetOfParticles
 from pwem.protocols import ProtAnalysis3D
+from pwem.constants import ALIGN_PROJ
 
+from relion import Plugin
 import relion.convert as convert
-from ..constants import ANGULAR_SAMPLING_LIST
+from ..constants import ANGULAR_SAMPLING_LIST, LABELS_DICT, PARTICLE_EXTRA_LABELS
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputVolumes = SetOfVolumes
+    outputParticles = SetOfParticles
+
+
 class ProtRelionMultiBody(ProtAnalysis3D, ProtRelionBase):
     """
     Relion protocol for multi-body refinement.
 
     This approach models flexible complexes as a user-defined number of rigid
-    bodies that move independently from each other.
+    bodies that move independently of each other.
     Using separate focused refinements with iteratively improved partial
     signal subtraction, improved reconstructions are generated for
     each of the defined bodies.
 
     Moreover, using PCA on the relative orientations of the bodies
     over all particle images in the data set, we generate movies that describe
     the most important motions in the data.
     """
     _label = '3D multi-body'
     _devStatus = PROD
+    _possibleOutputs = outputs
     IS_CLASSIFY = False
+    IS_3D_MB = True
     PREFIXES = ['half1_', 'half2_']
 
     def _initialize(self):
-        """ This function is mean to be called after the
+        """ This function is meant to be called after the
         working dir for the protocol have been set. (maybe after recovery from mapper)
         """
         self._createFilenameTemplates()
         self._createIterTemplates()
 
     def _getInputPath(self, *paths):
         return self._getPath('input', *paths)
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         self._defineConstants()
 
         form.addSection(label='Input')
+        form.addParam('doContinue', params.BooleanParam, default=False,
+                      label='Continue from a previous run?',
+                      help='If you set to *Yes*, you should select a previous '
+                           'MultiBody protocol and most of the input parameters '
+                           'will be taken from it.')
         form.addParam('protRefine', params.PointerParam,
+                      condition='not doContinue',
                       pointerClass="ProtRefine3D",
                       label='Consensus refinement protocol',
                       help='Select any previous refinement protocol from '
                            'where to run the multi-body refinement. '
                            'The output volume will be used and some '
                            'parameters from the optimiser.star file. ')
         # FIXME: Find an easy way to avoid input a file here
         form.addParam('bodyStarFile', params.FileParam,
+                      condition='not doContinue',
                       label='Body STAR file',
                       help='Provide the STAR file with all information '
                            'about the bodies to be used in multi-body '
                            'refinement. An example for a three-body '
-                           'refinement would look like this:\n'
+                           'refinement would look like this:\n\n'
                            'data_\n'
                            'loop_\n'
                            '_rlnBodyMaskName\n'
                            '_rlnBodyRotateRelativeTo\n'
                            '_rlnBodySigmaAngles\n'
                            '_rlnBodySigmaOffset\n'
                            'large_body_mask.mrc 2 10 2\n'
-                           'small_body_mask.mrc 1 10 2 \n'
-                           'head_body_mask.mrc 2 10 2 \n')
+                           'small_body_mask.mrc 1 10 2\n'
+                           'head_body_mask.mrc 2 10 2\n\n'
+                           ''
 
-        """
+                           """
  Where each data line represents a different body, and:
-  - rlnBodyMaskName contains the name of a soft-edged mask with values in [0,1] that define the body;
+ - rlnBodyMaskName contains the name of a soft-edged mask with values in [0,1] that define the body; the mask name should be relative to the project folder;
  - rlnBodyRotateRelativeTo defines relative to which other body this body rotates (first body is number 1);
  - rlnBodySigmaAngles and _rlnBodySigmaOffset are the standard deviations (widths) of Gaussian priors on the consensus rotations and translations;
 
  Optionally, there can be a fifth column with _rlnBodyReferenceName. Entries can be 'None' (without the ''s) or the name of a MRC map with an initial reference for that body. In case the entry is None, the reference will be taken from the density in the consensus refinement.
 
-Also note that larger bodies should be above smaller bodies in the STAR file. For more information, see the multi-body paper.')
-        """
+Also note that larger bodies should be above smaller bodies in the STAR file. For more information, see the multi-body paper.
+                           """)
 
         form.addParam('recSubtractedBodies', params.BooleanParam, default=True,
+                      condition='not doContinue',
                       label='Reconstruct subtracted bodies?',
                       help='If set to Yes, then the reconstruction of each of '
                            'the bodies will use the subtracted images. This '
                            'may give useful insights about how well the '
                            'subtraction worked. If set to No, the original '
                            'particles are used for reconstruction (while the '
                            'subtracted ones are still used for alignment). '
                            'This will result in fuzzy densities for bodies '
                            'outside the one used for refinement.')
+        if Plugin.IS_GT50():
+            form.addParam('useBlush', params.BooleanParam, default=False,
+                          label='Use Blush regularisation?',
+                          help='If set to Yes, relion_refine will use a neural '
+                               'network to perform regularisation by denoising '
+                               'at every iteration, instead of the standard '
+                               'smoothness regularisation.')
+        form.addParam('continueRun', params.PointerParam,
+                      pointerClass='ProtRelionMultiBody',
+                      condition='doContinue', allowsNull=True,
+                      label='Select previous run',
+                      help='Select a previous run to continue from.')
+        form.addParam('continueIter', params.StringParam, default='last',
+                      condition='doContinue',
+                      label='Continue from iteration',
+                      help='Select from which iteration do you want to '
+                           'continue. If you use *last*, then the last '
+                           'iteration will be used. Otherwise, a valid '
+                           'iteration number should be provided.')
 
-        group = form.addGroup('Auto-Sampling')
+        group = form.addGroup('Auto-Sampling',
+                              condition='not doContinue')
         group.addParam('initialAngularSampling', params.EnumParam, default=4,
+                       condition='not doContinue',
                        choices=ANGULAR_SAMPLING_LIST,
                        label='Initial angular sampling (deg)',
                        help='There are only a few discrete angular samplings'
                             ' possible because we use the HealPix library to'
                             ' generate the sampling of the first two Euler '
                             'angles on the sphere. The samplings are '
                             'approximate numbers and vary slightly over '
                             'the sphere. \n\n'
                             'Note that this will only be the value for the '
                             'first few iteration(s): the sampling rate will '
                             'be increased automatically after that.')
         group.addParam('initialOffsetRange', params.FloatParam, default=3,
+                       condition='not doContinue',
                        label='Initial offset range (pix)',
                        help='Probabilities will be calculated only for '
                             'translations in a circle with this radius (in '
                             'pixels). The center of this circle changes at '
                             'every iteration and is placed at the optimal '
                             'translation for each image in the previous '
                             'iteration. \n\n'
                             'Note that this will only be the value for the '
                             'first few iteration(s): the sampling rate will '
                             'be increased automatically after that.')
         group.addParam('initialOffsetStep', params.FloatParam, default=0.75,
+                       condition='not doContinue',
                        label='Initial offset step (pix)',
                        help='Translations will be sampled with this step-size '
                             '(in pixels). Translational sampling is also done '
                             'using the adaptive approach. Therefore, if '
                             'adaptive=1, the translations will first be '
                             'evaluated on a 2x coarser grid. \n\n'
                             'Note that this will only be the value for the '
@@ -192,86 +234,124 @@
         line.addParam('minEigenvalue', params.IntParam, default=-999, label='min')
         line.addParam('maxEigenvalue', params.IntParam, default=999, label='max')
 
         form.addSection('Compute')
         self._defineComputeParams(form)
         form.addParam('extraParams', params.StringParam,
                       default='',
-                      label='Additional parameters',
+                      label='Additional arguments',
                       help="In this box command-line arguments may be "
-                           "provided that are not generated by the GUI. ")
+                           "provided that are not generated by the GUI. They will "
+                           "be appended to the relion_refine command.")
 
         form.addParallelSection(threads=1, mpi=3)
     
     # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
-        self._createFilenameTemplates()
-        objId = self.protRefine.get().getObjId()
+        self._initialize()
+        if self.doContinue:
+            objId = self.continueRun.get().getObjId()
+        else:
+            objId = self.protRefine.get().getObjId()
         self._insertFunctionStep('convertInputStep', objId)
         self._insertFunctionStep('multibodyRefineStep',
                                  self._getRefineArgs())
         if self.runFlexAnalysis:
             self._insertFunctionStep('flexAnalysisStep',
                                      self._getAnalyseArgs())
         self._insertFunctionStep('createOutputStep')
     
     # -------------------------- STEPS functions ------------------------------
     def convertInputStep(self, protId):
-        self.info("Relion version:")
-        self.runJob("relion_refine --version", "", numberOfMpi=1)
+        if self.doContinue:
+            bodyFn = self.continueRun.get().bodyStarFile.get()
+        else:
+            bodyFn = self.bodyStarFile.get()
 
-        pwutils.copyFile(self.bodyStarFile.get(),
-                         self._getExtraPath('input_body.star'))
+        pwutils.copyFile(bodyFn, self._getExtraPath('input_body.star'))
 
     def multibodyRefineStep(self, args):
         params = ' '.join(['%s %s' % (k, str(v)) for k, v in args.items()])
+        if self.extraParams.hasValue():
+            params += ' ' + self.extraParams.get()
+
         self._runProgram('relion_refine', params)
 
     def flexAnalysisStep(self, args):
         params = ' '.join(['%s %s' % (k, str(v)) for k, v in args.items()])
         # use runJob since MPI is not allowed
         self.runJob('relion_flex_analyse', params, numberOfMpi=1,
                     numberOfThreads=1)
 
     def createOutputStep(self):
-        protRefine = self.protRefine.get()
-        sampling = protRefine._getInputParticles().getSamplingRate()
+        protRefine = self._getProtRefine()
+        if self.doContinue:
+            # get original 3D refine protocol
+            protRefine = protRefine.protRefine.get()
+
+        # get refine 3d output parts pointer
+        inputPartsSet = protRefine.outputParticles
+        sampling = inputPartsSet.getSamplingRate()
         volumes = self._createSetOfVolumes()
         volumes.setSamplingRate(sampling)
 
         self._loadVolsInfo()
 
         for item in range(1, self._getNumberOfBodies() + 1):
             vol = Volume()
             self._updateVolume(item, vol)
             volumes.append(vol)
 
-        self._defineOutputs(outputVolumes=volumes)
-        vol = self.protRefine.get().outputVolume
-        self._defineSourceRelation(vol, volumes)
+        outImgSet = self._createSetOfParticles()
+        outImgSet.copyInfo(inputPartsSet)
+        self._fillDataFromIter(inputPartsSet, outImgSet, self._lastIter())
+
+        self._defineOutputs(**{outputs.outputVolumes.name: volumes})
+        self._defineSourceRelation(protRefine.outputVolume, volumes)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
+        self._defineTransformRelation(inputPartsSet, outImgSet)
 
     # -------------------------- INFO functions -------------------------------
     def _validate(self):
         errors = []
-        bodyFn = self.bodyStarFile.get()
-        if not os.path.exists(bodyFn):
-            errors.append("Input body star file %s does not exist." % bodyFn)
+        if self.doContinue:
+            continueProtocol = self.continueRun.get()
+            if (continueProtocol is not None and
+                    continueProtocol.getObjId() == self.getObjId()):
+                errors.append('In Scipion you must create a new Relion run '
+                              'and select the continue option rather than '
+                              'select continue from the same run.\n')
+
+            continueProtocol._initialize()
+            lastIter = continueProtocol._lastIter()
+
+            if self.continueIter.get() == 'last':
+                continueIter = lastIter
+            else:
+                continueIter = int(self.continueIter.get())
+
+            if continueIter > lastIter:
+                errors.append("You can continue only from the iteration %01d or less" % lastIter)
         else:
-            table = Table(fileName=bodyFn)
-            missing = []
-            for row in table:
-                if not os.path.exists(row.rlnBodyMaskName):
-                    missing.append(row.rlnBodyMaskName)
-                ref = getattr(row, 'rlnBodyReferenceName', 'None')
-                if ref != 'None' and not os.path.exists(ref):
-                    missing.append(ref)
-            if missing:
-                errors.append("Missing files from input star file: ")
-                for f in missing:
-                    errors.append(" - %s" % f)
+            bodyFn = self.bodyStarFile.get()
+            if not os.path.exists(bodyFn):
+                errors.append("Input body star file %s does not exist." % bodyFn)
+            else:
+                table = Table(fileName=bodyFn)
+                missing = []
+                for row in table:
+                    if not os.path.exists(row.rlnBodyMaskName):
+                        missing.append(row.rlnBodyMaskName)
+                    ref = getattr(row, 'rlnBodyReferenceName', 'None')
+                    if ref != 'None' and not os.path.exists(ref):
+                        missing.append(ref)
+                if missing:
+                    errors.append("Missing files from input star file: ")
+                    for f in missing:
+                        errors.append(" - %s" % f)
         return errors
 
     def _citations(self):
         return ['Nakane2018']
 
     def _summary(self):
         self._initialize()
@@ -317,61 +397,70 @@
     def _getNumberOfBodies(self):
         table = Table(fileName=self._getExtraPath("input_body.star"))
         return int(table.size())
 
     def _updateVolume(self, bodyNum, item):
         item.setFileName(self._getFileName('finalvolume_mbody', ref3d=bodyNum))
         half1 = self._getFileName('final_half1_volume_mbody', ref3d=bodyNum)
-        half2 = self._getFileName('final_half1_volume_mbody', ref3d=bodyNum)
+        half2 = self._getFileName('final_half2_volume_mbody', ref3d=bodyNum)
         item.setHalfMaps([half1, half2])
 
         row = self._volsInfo[bodyNum]
         item._rlnAccuracyRotations = Float(row.rlnAccuracyRotations)
         item._rlnAccuracyTranslationsAngst = Float(row.rlnAccuracyTranslationsAngst)
 
     def _getRefineArgs(self):
-        """ Define all parameters to run relion_refine.
-        """
-        protRefine = self.protRefine.get()
+        """ Define all parameters to run relion_refine. """
+        args = {'--o': self._getExtraPath('relion')}
+        protRefine = self._getProtRefine()
         protRefine._initialize()
-        fnOptimiser = protRefine._getFileName('optimiser',
-                                              iter=protRefine._lastIter())
-        healpix = self.initialAngularSampling.get()
 
-        args = {
-            '--continue': fnOptimiser,
-            '--multibody_masks': self._getExtraPath('input_body.star'),
-            '--o': self._getExtraPath('relion'),
-            '--solvent_correct_fsc': '',
-            '--oversampling': 1,
-            '--pad': 1 if self.skipPadding else 2,
-            '--healpix_order': healpix,
-            '--auto_local_healpix_order': healpix,
-            '--offset_range': self.initialOffsetRange.get(),
-            '--offset_step': self.initialOffsetStep.get()
-        }
+        if self.doContinue:
+            continueIter = self._getContinueIter()
+            fnOptimiser = protRefine._getFileName('optimiser',
+                                                  iter=continueIter)
+
+            if protRefine.recSubtractedBodies:
+                args['--reconstruct_subtracted_bodies'] = ''
 
-        if self.skipGridding:
-            args['--skip_gridding'] = ''
+        else:
+            fnOptimiser = protRefine._getFileName('optimiser',
+                                                  iter=protRefine._lastIter())
+            args.update({
+                '--multibody_masks': self._getExtraPath('input_body.star'),
+                '--solvent_correct_fsc': '',
+                '--oversampling': 1,
+                '--pad': 1 if self.skipPadding else 2,
+                '--healpix_order': self.initialAngularSampling.get(),
+                '--auto_local_healpix_order': self.initialAngularSampling.get(),
+                '--offset_range': self.initialOffsetRange.get(),
+                '--offset_step': self.initialOffsetStep.get()
+            })
 
-        # Due to Relion bug we recreate mask from previous refinement protocol
-        # it's not used by multibody
-        if protRefine.referenceMask.hasValue():
-            table = Table(fileName=fnOptimiser,
-                          tableName='optimiser_general')
-            maskFn = table[0].rlnSolventMaskName
-            newDim = protRefine._getInputParticles().getXDim()
-            newPix = protRefine._getInputParticles().getSamplingRate()
-            convert.convertMask(protRefine.referenceMask.get(), maskFn,
-                                newPix, newDim)
+            if self.recSubtractedBodies:
+                args['--reconstruct_subtracted_bodies'] = ''
 
-        self._setComputeArgs(args)
+            if Plugin.IS_GT50() and self.useBlush:
+                args['--blush'] = ''
 
-        if self.recSubtractedBodies:
-            args['--reconstruct_subtracted_bodies'] = ''
+            # Due to Relion bug we create a fake mask from previous refinement protocol
+            # it's not used by multi-body
+            if protRefine.referenceMask.hasValue():
+                table = Table(fileName=fnOptimiser,
+                              tableName='optimiser_general',
+                              types=LABELS_DICT)
+                maskFn = table[0].rlnSolventMaskName
+                bodyFn = self.bodyStarFile.get()
+                maskBody1 = Table(fileName=bodyFn)[0].rlnBodyMaskName
+                os.makedirs(os.path.dirname(maskFn), exist_ok=True)
+                pwutils.createAbsLink(os.path.abspath(maskBody1), maskFn)
+
+        args['--continue'] = fnOptimiser
+
+        self._setComputeArgs(args)
 
         return args
 
     def _getAnalyseArgs(self):
         args = {
             '--PCA_orient': '',
             '--model': self._getFileName('modelFinal'),
@@ -386,7 +475,31 @@
             args.update({
                 '--select_eigenvalue': self.selectEigenvalueNumber.get(),
                 '--select_eigenvalue_min': self.minEigenvalue.get(),
                 '--select_eigenvalue_max': self.maxEigenvalue.get()
             })
 
         return args
+
+    def _getProtRefine(self):
+        return self.continueRun.get() if self.doContinue else self.protRefine.get()
+
+    def _fillDataFromIter(self, inputSet, outSet, iteration):
+        outImgsFn = self._getFileName('data', iter=iteration)
+        outSet.setAlignmentProj()
+        self.reader = convert.createReader(alignType=ALIGN_PROJ,
+                                           pixelSize=outSet.getSamplingRate())
+
+        mdIter = Table.iterRows('particles@' + outImgsFn, key='rlnImageId',
+                                types=convert.LABELS_DICT)
+        outSet.copyItems(inputSet, doClone=False,
+                         updateItemCallback=self._updateParticle,
+                         itemDataIterator=mdIter)
+
+    def _updateParticle(self, particle, row):
+        self.reader.setParticleTransform(particle, row)
+
+        if getattr(self, '__updatingFirst', True):
+            self.reader.createExtraLabels(particle, row, PARTICLE_EXTRA_LABELS)
+            self.__updatingFirst = False
+        else:
+            self.reader.setExtraLabels(particle, row)
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_postprocess.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_ctfrefine.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-# **************************************************************************
+# ******************************************************************************
 # *
-# * Authors:     Josue Gomez Blanco     (josue.gomez-blanco@mcgill.ca) [1]
-# *              J.M. de la Rosa Trevin (delarosatrevin@scilifelab.se) [2]
+# * Authors:    Roberto Marabini       (roberto@cnb.csic.es) [1]
+# *             J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [2]
 # *
-# * [1] Department of Anatomy and Cell Biology, McGill University
+# * [1] Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # * [2] SciLifeLab, Stockholm University
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
@@ -20,290 +20,353 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# ******************************************************************************
 
-import os
-from emtable import Table
+import sys
+import matplotlib as mpl
+import numpy as np
 
-import pyworkflow.utils as pwutils
-import pyworkflow.protocol.params as params
-from pyworkflow.constants import PROD
-from pwem.protocols import ProtAnalysis3D
+from pwem.viewers.plotter import plt
 from pwem.emlib.image import ImageHandler
-from pwem.objects import Volume
+from pyworkflow.viewer import ProtocolViewer
 
-import relion.convert as convert
-from .protocol_base import ProtRelionBase
+from .viewer_base import *
+from ..objects import CtfRefineGlobalInfo
+from ..protocols import ProtRelionCtfRefinement
+
+
+class ProtCtfRefineViewer(ProtocolViewer):
+    """ Viewer for Relion CTF refine results. """
+    _label = 'ctf refine viewer'
+    _environments = [DESKTOP_TKINTER, WEB_DJANGO]
+    _targets = [ProtRelionCtfRefinement]
+
+    def __init__(self,  **kwargs):
+        ProtocolViewer.__init__(self,  **kwargs)
+        self.protocol._initialize()
+        self._micInfoList = None
+        self.xMax = None
+        self.yMax = None
+        self._currentMicIndex = 0
+        self._oldCurrentMicIndex = 0
+        self._currentMicId = 1
+        self._loadAnalyzeInfo()
 
-
-class ProtRelionPostprocess(ProtAnalysis3D, ProtRelionBase):
-    """
-    Relion post-processing protocol for automated masking,
-    overfitting estimation, MTF-correction and B-factor sharpening.
-    """
-    _label = 'post-processing'
-    _devStatus = PROD
-
-    def _getInputPath(self, *paths):
-        return self._getPath('input', *paths)
-
-    def _createFilenameTemplates(self):
-        """ Centralize how files are called for iterations and references. """
-        myDict = {
-            'finalVolume': self._getInputPath("relion_class001.mrc"),
-            'half1': self._getInputPath("relion_half1_class001_unfil.mrc"),
-            'half2': self._getInputPath("relion_half2_class001_unfil.mrc"),
-            'mask': self._getInputPath("input_mask.mrc"),
-            'outputVolume': self._getExtraPath('postprocess.mrc')
-        }
-        self._updateFilenamesDict(myDict)
-
-    # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
-        form.addSection(label='Input')
-        form.addParam('protRefine', params.PointerParam,
-                      pointerClass="ProtRefine3D, ProtRelionMultiBody",
-                      label='Select a previous refinement protocol',
-                      help='Select any previous refinement protocol to get the '
-                           '3D half maps. Note that it is recommended that the '
-                           'refinement protocol uses a gold-standard method.')
-        form.addParam('bodyNum', params.IntParam, default=1,
-                      label="Which body to process?",
-                      help="Only relevant if input protocol is 3D multi-body.")
-        form.addParam('solventMask', params.PointerParam,
-                      pointerClass="VolumeMask",
-                      label='Solvent mask',
-                      help="Provide a soft mask where the protein is white "
-                           "(1) and the solvent is black (0). Often, the "
-                           "softer the mask the higher resolution estimates "
-                           "you will get. A soft edge of 5-10 pixels is often "
-                           "a good edge width.")
-        form.addParam('calibratedPixelSize', params.FloatParam, default=0,
-                      label='Calibrated pixel size (A)',
-                      help="Provide the final, calibrated pixel size in "
-                           "Angstroms. If 0, the input pixel size will be used. "
-                           "This value may be different from the pixel-size "
-                           "used thus far, e.g. when you have recalibrated "
-                           "the pixel size using the fit to a PDB model. "
-                           "The X-axis of the output FSC plot will use this "
-                           "calibrated value.")
-
-        form.addSection(label='Sharpening')
-        group = form.addGroup('MTF')
-        group.addParam('mtf', params.FileParam,
-                       label='MTF of the detector',
-                       help='User-provided STAR-file with the MTF-curve '
-                            'of the detector. Use the wizard to load one '
-                            'of the predefined ones provided at:\n'
-                            '- [[https://www3.mrc-lmb.cam.ac.uk/relion/index.php/'
-                            'FAQs#Where_can_I_find_MTF_curves_for_typical_detectors.3F]'
-                            '[Relion\'s Wiki FAQs]]\n'
-                            ' - [[https://www.gatan.com/techniques/cryo-em#MTF][Gatan\'s website]]\n\n'
-                            'Relion param: *--mtf*')
-        group.addParam('origPixelSize', params.FloatParam,
-                       default=-1.0,
-                       label='Original detector pixel size (A)',
-                       help='This is the original pixel size (in Angstroms)'
-                            ' in the raw (non-super-resolution!) micrographs')
-
-        form.addParam('doAutoBfactor', params.BooleanParam, default=True,
-                      label='Estimate B-factor automatically?',
-                      help='If set to Yes, then the program will use the '
-                           'automated procedure described by Rosenthal and '
-                           'Henderson (2003, JMB) to estimate an overall '
-                           'B-factor for your map, and sharpen it accordingly.')
-        line = form.addLine('B-factor resolution (A): ',
-                            condition='doAutoBfactor',
-                            help='There are the frequency (in Angstroms), '
-                                 'lowest and highest, that will be included in '
-                                 'the linear fit of the Guinier plot as '
-                                 'described in Rosenthal and Henderson '
-                                 '(2003, JMB).')
-        line.addParam('bfactorLowRes', params.FloatParam,
-                      default=10.0, label='low')
-        line.addParam('bfactorHighRes', params.FloatParam,
-                      default=0.0, label='high')
-        form.addParam('bfactor', params.FloatParam, default=-350,
-                      condition='not doAutoBfactor',
-                      label='Provide B-factor:',
-                      help='User-provided B-factor (in A^2) for map '
-                           'sharpening, e.g. -400. Use negative values for '
-                           'sharpening. Be careful: if you over-sharpen\n'
-                           'your map, you may end up interpreting noise for '
-                           'signal!\n'
-                           'Relion param: *--adhoc_bfac*')
-
-        form.addSection(label='Filtering')
-        form.addParam('skipFscWeighting', params.BooleanParam, default=False,
-                      label='Skip FSC-weighting for sharpening?',
-                      help='If set to No (the default), then the output map '
-                           'will be low-pass filtered according to the '
-                           'mask-corrected, gold-standard FSC-curve. '
-                           'Sometimes, it is also useful to provide an ad-hoc '
-                           'low-pass filter (option below), as due to local '
-                           'resolution variations some parts of the map may '
-                           'be better and other parts may be worse than the '
-                           'overall resolution as measured by the FSC. In '
-                           'such  cases, set this option to Yes and provide '
-                           'an ad-hoc filter as described below.')
-        form.addParam('lowRes', params.FloatParam, default=5,
-                      condition='skipFscWeighting',
-                      label='Ad-hoc low-pass filter (A):',
-                      help='This option allows one to low-pass filter the map '
-                           'at a user-provided frequency (in Angstroms). When '
-                           'using a resolution that is higher than the '
-                           'gold-standard FSC-reported resolution, take care '
-                           'not to interpret noise in the map for signal.')
-        form.addParam('filterEdgeWidth', params.IntParam, default=2,
-                      expertLevel=params.LEVEL_ADVANCED,
-                      label='Low-pass filter edge width:',
-                      help='Width of the raised cosine on the low-pass filter '
-                           'edge (in resolution shells)\n'
-                           'Relion param: *--filter_edge_width*')
-        form.addParam('randomizeAtFsc', params.FloatParam, default=0.8,
-                      expertLevel=params.LEVEL_ADVANCED,
-                      label='Randomize phases threshold',
-                      help='Randomize phases from the resolution where FSC '
-                           'drops below this value\n'
-                           'Relion param: *--randomize_at_fsc*')
-        form.addParam('forceMask', params.BooleanParam, default=False,
-                      expertLevel=params.LEVEL_ADVANCED,
-                      label='Force mask?',
-                      help='Use the mask even when the masked resolution '
-                           'is worse than the unmasked resolution.')
-
-        form.addParallelSection(threads=0, mpi=0)
-
-    # -------------------------- INSERT steps functions ------------------------
-    def _insertAllSteps(self):
-        objId = self.protRefine.get().getObjId()
-        self._createFilenameTemplates()
-        self._defineParamDict()
-        self._insertFunctionStep('convertInputStep', objId)
-        self._insertFunctionStep('postProcessStep', self.paramDict)
-        self._insertFunctionStep('createOutputStep')
-
-    # -------------------------- STEPS functions -------------------------------
-    def convertInputStep(self, protId):
-        pwutils.makePath(self._getInputPath())
-        protRef = self.protRefine.get()
-
-        if self._isInputMbody():
-            for i, vol in enumerate(protRef.outputVolumes):
-                if i == self.bodyNum.get()-1:
-                    outVol = vol
-                    print("Using multi-body input:", vol.getFileName())
-                    break
-        else:  # ProtRefine3D
-            outVol = protRef.outputVolume
-
-        newDim = outVol.getXDim()
-        newPix = outVol.getSamplingRate()
-        vols = outVol.getHalfMaps().split(',')
-        vols.insert(0, outVol.getFileName())
-        ih = ImageHandler()
-
-        convert.convertMask(self.solventMask.get(),
-                            self._getFileName('mask'), newPix, newDim)
-
-        for vol, key in zip(vols, ['outputVolume', 'half1', 'half2']):
-            ih.convert(vol, self._getFileName(key))
+        self._env = os.environ.copy()
+        showBeamTilt = self.protocol.doBeamtiltEstimation.get()
+        showTrefoil = self.protocol.doEstimateTrefoil.get() and showBeamTilt
+        showTetrafoil = self.protocol.doEstimate4thOrder.get()
+        showDefocus = self.protocol.doCtfFitting.get()
+        showAnisoMag = self.protocol.estimateAnisoMag.get()
+
+        form.addSection(label="Results")
+        form.addParam('useMatplotlib', params.BooleanParam, default=True,
+                      label='Use matplotlib for display',
+                      condition="not {}".format(showDefocus),
+                      help='If False, images will be displayed with ImageJ')
+
+        form.addParam('displayAnisoMag', params.LabelParam,
+                      label="Show X/Y mag. anisotropy estimation",
+                      condition="{}".format(showAnisoMag),
+                      help="Display four images (X and Y): (1) phase "
+                           "differences from which this estimate was "
+                           "derived and\n(2) the model fitted through it.")
+        form.addParam('displayDefocus', params.LabelParam,
+                      label="Show defocus estimation",
+                      condition="{}".format(showDefocus),
+                      help="Display the defocus estimation.\n "
+                           "Plot defocus difference (Angstroms) vs "
+                           "position in micrograph\n"
+                           "You may move between micrographs by using: \n\n"
+                           "Left/Right keys (move +1/-1 micrograph)\n"
+                           "Up/Down keys (move +10/-10 micrographs)\n"
+                           "Page_up/Page_down keys (move +100/-100 "
+                           "micrographs)\n"
+                           "Home/End keys (move +1000/-1000 micrographs)")
+        form.addParam('displayBeamTilt', params.LabelParam,
+                      label="Show beam tilt estimation",
+                      condition="{} and not {}".format(showBeamTilt, showTrefoil),
+                      help="Display two images: (1) phase differences from "
+                           "which this estimate was derived and\n"
+                           "(2) the model fitted through it.")
+        form.addParam('displayTrefoil', params.LabelParam,
+                      label="Show beam tilt and 3-fold astigmatism estimation",
+                      condition="{}".format(showTrefoil),
+                      help="Display two images: (1) phase differences from "
+                           "which this estimate was derived and\n"
+                           "(2) the model fitted through it.")
+        form.addParam('displayTetrafoil', params.LabelParam,
+                      label="Show 4-fold aberrations estimation",
+                      condition="{}".format(showTetrafoil),
+                      help="Display two images: (1) phase differences from "
+                           "which this estimate was derived and\n"
+                           "(2) the model fitted through it.")
+        form.addParam('displayParticles', params.LabelParam,
+                      label="Display particles",
+                      help="See the particles with the new CTF "
+                           "values")
+
+    def _getVisualizeDict(self):
+        return {
+            'displayAnisoMag': self._displayAnisoMag,
+            'displayDefocus': self._displayDefocus,
+            'displayBeamTilt': self._displayBeamTilt,
+            'displayTrefoil': self._displayTrefoil,
+            'displayTetrafoil': self._displayTetrafoil,
+            'displayParticles': self._displayParticles
+        }
 
-    def postProcessStep(self, paramDict):
-        params = ' '.join(['%s %s' % (k, str(v))
-                           for k, v in self.paramDict.items()])
-        self._runProgram('relion_postprocess', params)
-
-    def createOutputStep(self):
-        volume = Volume()
-        volume.setFileName(self._getFileName('outputVolume'))
-        if self._isInputMbody():
-            vol = self.protRefine.get().outputVolumes
-        else:
-            vol = self.protRefine.get().outputVolume
-        volume.setSamplingRate(self._getOutputPixelSize())
-        self._defineOutputs(outputVolume=volume)
-        self._defineSourceRelation(vol, volume)
-
-    # -------------------------- INFO functions --------------------------------
-    def _validate(self):
-        errors = []
-        mtfFile = self.mtf.get()
-
-        if mtfFile and not os.path.exists(mtfFile):
-            errors.append("Missing MTF-file '%s'" % mtfFile)
-
-        return errors
-
-    def _citations(self):
-        return ['Chen2013']
-
-    def _summary(self):
-        summary = []
-        postStarFn = self._getExtraPath("postprocess.star")
-        if os.path.exists(postStarFn):
-            table = Table(fileName=postStarFn, tableName='general')
-            row = table[0]
-            summary.append("Final resolution: *%0.2f A*" %
-                           float(row.rlnFinalResolution))
-            summary.append("B-factor: *%0.2f A\u00B2*" %
-                           float(row.rlnBfactorUsedForSharpening))
-
-        return summary
-
-    # -------------------------- UTILS functions ------------------------------
-    def _defineParamDict(self):
-        """ Define all parameters to run relion_postprocess"""
-        # It seems that in Relion3 now the input should be the map
-        # filename and not the prefix as before
-        inputFn = self._getFileName('half1')
-
-        self.paramDict = {'--i': inputFn,
-                          '--o': self._getExtraPath('postprocess'),
-                          '--angpix': self._getOutputPixelSize(),
-                          # Expert params
-                          '--filter_edge_width': self.filterEdgeWidth.get(),
-                          '--randomize_at_fsc': self.randomizeAtFsc.get(),
-                          '--mask': self._getFileName('mask')
-                          }
-
-        mtfFile = self.mtf.get()
-        if mtfFile:
-            self.paramDict['--mtf'] = mtfFile
-
-        if self.doAutoBfactor:
-            self.paramDict['--auto_bfac'] = ''
-            self.paramDict['--autob_lowres'] = self.bfactorLowRes.get()
-            self.paramDict['--autob_highres'] = self.bfactorHighRes.get()
+    def _displayAnisoMag(self, param=None):
+        obs_x = self.protocol._getFileName("mag_obs_x", og=1)
+        obs_y = self.protocol._getFileName("mag_obs_y", og=1)
+        fit_x = self.protocol._getFileName("mag_fit_x", og=1)
+        fit_y = self.protocol._getFileName("mag_fit_y", og=1)
+
+        return self._showImages(obs_x, obs_y, fit_x, fit_y,
+                                title="Anisotropy magnification")
+
+    def _displayDefocus(self, e=None):
+        """Show matplotlib with defocus values."""
+        micInfo = self._micInfoList[self._currentMicIndex]
+        self._currentMicId = micInfo.micId.get()
+        # disable default binding for arrows
+        # because I want to use them
+        # to navigate between micrographs
+        # wrap in try, except because matplotlib will raise
+        # an exception if the value is not in the list
+        try:
+            mpl.rcParams['keymap.back'].remove('left')
+            mpl.rcParams['keymap.forward'].remove('right')
+        except:
+            pass
+
+        self.plotter = EmPlotter(windowTitle="CTF Refinement", x=1, y=2)
+        self._plotDefocusStdev()
+
+        self.fig = self.plotter.getFigure()
+        self.ax2 = self.plotter.createSubPlot(
+            self._getTitle(micInfo), "Mic-Xdim", "Mic-Ydim",
+            xpos=1, ypos=2)
+
+        # call self.press after pressing any key
+        self.fig.canvas.mpl_connect('key_press_event', self.press)
+
+        # Maximize plot, valid for the 3 most common backends
+        # Not sure if we need it since scipion installs it own TK
+        # but I guess somebody may use the system one
+        backend = mpl.get_backend()
+        manager = plt.get_current_fig_manager()
+        if backend == 'QT':
+            # Option 1
+            # QT backend
+            manager.window.showMaximized()
+        elif backend == 'TkAgg':
+            # Option 2
+            # TkAgg backend
+            manager.resize(*manager.window.maxsize())
+        elif backend == 'WX':
+            # Option 3
+            # WX backend
+            manager.frame.Maximize(True)
+
+        self.show()
+
+    def _showImages(self, *imgs, **kwargs):
+        title = kwargs.get('title', '')
+        if self.useMatplotlib:
+            return self._showImagesMatplotlib(title, *imgs)
         else:
-            self.paramDict['--adhoc_bfac'] = self.bfactor.get()
+            return [DataView(img) for img in imgs]
 
-        if self.skipFscWeighting:
-            self.paramDict['--skip_fsc_weighting'] = ''
-            self.paramDict['--low_pass'] = self.lowRes.get()
-
-        if self.origPixelSize.get() != -1.0:
-            self.paramDict['--mtf_angpix'] = self.origPixelSize.get()
-
-        if self.forceMask:
-            self.paramDict['--force_mask'] = ''
-
-    def _getRelionMapFn(self, fn):
-        return fn.split(':')[0]
-
-    def _isInputMbody(self):
-        return self.protRefine.get().getClassName() == "ProtRelionMultiBody"
-
-    def _getOutputPixelSize(self):
-        """ Return the output pixel size, using the calibrated
-        pixel size if non zero, or the input one. """
-        if self._isInputMbody():
-            volume = self.protRefine.get().outputVolumes
-        else:
-            volume = self.protRefine.get().outputVolume
-        cps = self.calibratedPixelSize.get()
-        return cps if cps > 0 else volume.getSamplingRate()
+    def _showImagesMatplotlib(self, title, *imgs):
+        ih = ImageHandler()
+        xdim = 2 if len(imgs) > 2 else 1
+        ydim = 2
+        plotter = EmPlotter(windowTitle=title, x=xdim, y=ydim, figsize=(8, 6))
+        positions = [(1, 1), (1, 2), (2, 1), (2, 2)]
+        for i, imgFn in enumerate(imgs):
+            x, y = positions[i]
+            ax = plotter.createSubPlot("", "x", "y", x, y)
+            img = ih.read(imgFn)
+            ax.imshow(img.getData(), cmap='jet')
+
+        return [plotter]
+
+    def _displayBeamTilt(self, param=None):
+        beamtilt_obs = self.protocol._getFileName("beamtilt_obs", og=1)
+        beamtilt_fit = self.protocol._getFileName("beamtilt_fit", og=1)
+
+        return self._showImages(beamtilt_obs, beamtilt_fit,
+                                title="Beam Tilt")
+
+    def _displayTrefoil(self, param=None):
+        trefoil_obs = self.protocol._getFileName("beamtilt_obs", og=1)
+        trefoil_fit = self.protocol._getFileName("trefoil_fit", og=1)
+
+        return self._showImages(trefoil_obs, trefoil_fit,
+                                title="Trefoil")
+
+    def _displayTetrafoil(self, param=None):
+        tetrafoil_obs = self.protocol._getFileName("tetrafoil_obs", og=1)
+        tetrafoil_fit = self.protocol._getFileName("tetrafoil_fit", og=1)
+
+        return self._showImages(tetrafoil_obs, tetrafoil_fit,
+                                title="Tetrafoil")
+
+    def createScipionPartView(self, filename):
+        inputParticlesId = self.protocol.inputParticles.get().strId()
+        labels = 'enabled id _size _filename '
+        labels += ' _ctfModel._defocusU _ctfModel._defocusV '
+
+        if self.protocol.doBeamtiltEstimation:
+            labels += ' _rlnBeamTiltX _rlnBeamTiltY'
+
+        viewParams = {showj.ORDER: labels,
+                      showj.VISIBLE: labels,
+                      showj.MODE: showj.MODE_MD,
+                      showj.RENDER: '_filename',
+                      'labels': 'id',
+                      }
+
+        return ObjectView(self._project,
+                          self.protocol.strId(),
+                          filename,
+                          other=inputParticlesId,
+                          env=self._env,
+                          viewParams=viewParams)
+
+    def _displayParticles(self, param=None):
+        views = []
+        fn = self.protocol.outputParticles.getFileName()
+        v = self.createScipionPartView(fn)
+        views.append(v)
+        return views
+
+    # ------------------- UTILS functions -------------------------
+    def _loadAnalyzeInfo(self):
+        # Only load once
+        if self._micInfoList is None:
+            ctfInfoFn = self.protocol._getFileName("ctf_sqlite")
+            if not os.path.exists(ctfInfoFn):
+                ctfInfo = self.protocol.createGlobalInfo(ctfInfoFn)
+            else:
+                ctfInfo = CtfRefineGlobalInfo(ctfInfoFn)
+            self._micInfoList = [mi.clone() for mi in ctfInfo]
+            self.xMax, self.yMax = ctfInfo.getMaxXY()
+            self.ctfInfoMapper = ctfInfo
+            ctfInfo.close()
+            self.len_micInfoList = len(self._micInfoList)
+            micList = [mi.micId.get() for mi in self._micInfoList]
+            # instead of creating this dict we have
+            # access the mapper and make a query to the database
+            self.micDict = {k: v for v, k in enumerate(micList)}
+
+    def onClick(self, event):
+        # try is needed because if clicked outside plot
+        # xdata, ydata are Nonetype
+        try:
+            ix, iy = int(round(event.xdata)), int(round(event.ydata))
+            # once the user has selected a point
+            # he have a pair of float numbers,
+            # search for the closest micrograph
+            # with the right stdev in a neighbourhood
+            if ix <= self.maxMicId:
+                while ix not in self.micDict:
+                    ix += 1
+                iix = self.micDict[ix]
+                start = max(0, iix-40)
+                end = min(iix+40, self.maxMicId)
+                dist = np.sqrt((np.array(self.x[start:end]) - ix) ** 2 +
+                               (np.array(self.y[start:end]) - iy) ** 2)
+                self._currentMicId = self.x[start + np.argmin(dist)]
+                self._oldCurrentMicIndex = self._currentMicIndex
+                self._currentMicIndex = self.micDict[self._currentMicId]
+                self.show()
+        except:
+            pass
+
+    def _plotDefocusStdev(self, e=None):
+        self.fig = self.plotter.getFigure()
+        self.ax1 = self.plotter.createSubPlot("Defocus stdev per Micrograph\n"
+                                              "Click on any point to get the "
+                                              "corresponding micrograph\n "
+                                              "in the defocus plot",
+                                              "# Micrograph", "stdev",
+                                              xpos=1, ypos=1)
+        self.fig.canvas.mpl_connect('button_press_event', self.onClick)
+        self.ax1.grid(True)
+        self.maxMicId = self._micInfoList[-1].micId.get()
+        self.x = [mi.micId.get() for mi in self._micInfoList]
+        self.y = [mi.stdev.get() for mi in self._micInfoList]
+        self.ax1.scatter(self.x, self.y, s=50, marker='o',
+                         c='blue')
+
+    def _getTitle(self, micInfo):
+        return ("Use arrows or Page up/Down or Home/End to navigate.\n"
+                "Mic = %s (%d)\nColorBar indicates defocus difference" %
+                (micInfo.micName.get()[-40:], micInfo.micId))
+
+    def press(self, event):
+        """ Change the currently shown micrograph
+        when a key is pressed (increment/decrement)
+        """
+        sys.stdout.flush()
+
+        if event.key == 'q':
+            plt.close('all')
+
+        shiftDict = {
+            'left': -1, 'right': 1,
+            'up': 10, 'down': -10,
+            'pageup': -100, 'pagedown': 100,
+            'home': -1000, 'end': 1000
+        }
+        # if pressed key is not left, up, etc, do nothing
+        if event.key in shiftDict:
+            shift = shiftDict[event.key]
+            # Check the new micrograph index is between first and last
+            newIndex = self._currentMicIndex + shift
+            self._oldCurrentMicIndex = self._currentMicIndex
+            self._currentMicIndex = min(max(0, newIndex),
+                                        self.len_micInfoList - 1)
+            self.show()
+
+    def show(self, event=None):
+        """ Draw plot """
+        # stdev plot
+        self.ax1.scatter(self.x[self._oldCurrentMicIndex],
+                         self.y[self._oldCurrentMicIndex], s=50,
+                         marker='o', c='blue')
+        self.ax1.scatter(self.x[self._currentMicIndex],
+                         self.y[self._currentMicIndex], s=50,
+                         marker='o', c='red')
+
+        # defocus plot
+        micInfo = self._micInfoList[self._currentMicIndex]
+        if event is None:
+            # I need to clear the plot otherwise
+            # old points are not removed
+            self.ax2.clear()
+            self.ax2.margins(0.05)
+            self.ax2.set_title(self._getTitle(micInfo))
+            newFontSize = self.plotter.plot_axis_fontsize + 2
+            self.ax2.set_xlabel("Mic Xdim (px)", fontsize=newFontSize)
+            self.ax2.set_ylabel("Mic Ydim (px)", fontsize=newFontSize)
+
+            self.ax2.set_xlim(0, self.xMax)  # np.max(micInfo.x))
+            self.ax2.set_ylim(0, self.yMax)  # np.max(micInfo.y))
+            self.ax2.grid(True)
+
+            # if I do not use subplots_adjust the window shrinks
+            #  after redraw
+            plt.subplots_adjust(left=0.1, right=0.9, top=0.9, bottom=0.1)
+
+        sc2 = self.ax2.scatter(micInfo.x, micInfo.y,
+                               c=micInfo.defocusDiff, s=100, marker='o')
+        self.plotter.getColorBar(sc2)
+        self.plotter.show()
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_preprocess.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,36 +19,42 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from enum import Enum
 
 import pyworkflow.utils as pwutils
 from pyworkflow.protocol.params import (PointerParam, BooleanParam,
                                         FloatParam, IntParam, Positive)
 from pyworkflow.protocol import STEPS_PARALLEL
 from pyworkflow.constants import PROD
 from pwem.constants import NO_INDEX
-from pwem.objects import SetOfAverages
+from pwem.objects import SetOfAverages, SetOfParticles
 from pwem.protocols import ProtProcessParticles
 
 import relion.convert as convert
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputParticles = SetOfParticles
+
+
 class ProtRelionPreprocessParticles(ProtProcessParticles, ProtRelionBase):
     """ This protocol wraps relion_preprocess program.
 
     It is used to perform normalisation, filtering or scaling of
     the particles.
     """
     _label = 'preprocess particles'
     _devStatus = PROD
+    _possibleOutputs = outputs
     
     def __init__(self, **args):
         ProtProcessParticles.__init__(self, **args)
         self.stepsExecutionMode = STEPS_PARALLEL
     
     # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
@@ -182,15 +188,15 @@
         if self.doScale:
             oldSampling = inputSet.getSamplingRate()
             scaleFactor = self._getScaleFactor(inputSet)
             newSampling = oldSampling * scaleFactor
             imgSet.setSamplingRate(newSampling)
 
         imgSet.copyItems(inputSet, updateItemCallback=self._setFileName)
-        self._defineOutputs(outputParticles=imgSet)
+        self._defineOutputs(**{outputs.outputParticles.name: imgSet})
         self._defineTransformRelation(inputSet, imgSet)
     
     # --------------------------- INFO functions ------------------------------
     def _validate(self):
         validateMsgs = []
 
         if self.doScale and self.scaleSize.get() % 2 != 0:
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_reconstruct.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_remove_views.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# **************************************************************************
+# ******************************************************************************
 # *
-# * Authors:     J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [1]
+# * Authors:     Grigory Sharov     (gsharov@mrc-lmb.cam.ac.uk)
 # *
-# * [1] SciLifeLab, Stockholm University
+# * MRC Laboratory of Molecular Biology, MRC-LMB
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -18,156 +18,162 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# ******************************************************************************
 
-from pyworkflow.protocol.params import (PointerParam, FloatParam,  
-                                        StringParam, BooleanParam,
-                                        EnumParam, IntParam, LEVEL_ADVANCED)
+import numpy as np
+from random import sample
+from enum import Enum
+
+import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
-from pwem.objects import Volume
-from pwem.protocols import ProtReconstruct3D
-from pwem.constants import ALIGN_PROJ
+from pwem.protocols import ProtParticles
+from pwem.objects import SetOfParticles
+import pwem.convert.transformations as tfs
+
 
-import relion.convert as convert
-from .protocol_base import ProtRelionBase
+class outputs(Enum):
+    outputParticles = SetOfParticles
 
 
-class ProtRelionReconstruct(ProtReconstruct3D, ProtRelionBase):
-    """ This protocol reconstructs a volume using Relion.
+class ProtRelionRemovePrefViews(ProtParticles):
+    """ Protocol to remove preferential views from a particle set.
+
+    Inspired by https://github.com/leschzinerlab/Relion
 
-    Reconstruct a volume from a given set of particles.
-    The alignment parameters will be converted to a Relion star file
-    and used as direction projections to reconstruct.
     """
-    _label = 'reconstruct'
+    _label = 'remove preferential views'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
-    # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
-
-        form.addParam('inputParticles', PointerParam,
-                      pointerClass='SetOfParticles',
+        form.addParam('inputParticles', params.PointerParam,
                       pointerCondition='hasAlignmentProj',
-                      label="Input particles",
-                      help='Select the input images from the project.')
-        form.addParam('symmetryGroup', StringParam, default='c1',
-                      label="Symmetry group",
-                      help='See [[https://relion.readthedocs.io/'
-                           'en/latest/Reference/Conventions.html#symmetry]'
-                           '[Relion Symmetry]] page for a description '
-                           'of the symmetry format accepted by Relion')
-        form.addParam('maxRes', FloatParam, default=-1,
-                      label="Maximum resolution (A)",  
-                      help='Maximum resolution (in Angstrom) to consider \n'
-                           'in Fourier space (default Nyquist).')
-        form.addParam('pad', FloatParam, default=2,
-                      label="Padding factor")
-        form.addParam('subset', EnumParam, default=0,
-                      choices=['all', 'half1', 'half2'],
-                      display=EnumParam.DISPLAY_HLIST,
-                      label='Subset to reconstruct',
-                      help='Subset of images to consider.')
-        form.addParam('classNum', IntParam, default=-1,
-                      label='Use only this class',
-                      help='Consider only this class (-1: use all classes)')
-        
-        form.addParam('extraParams', StringParam, default='',
-                      expertLevel=LEVEL_ADVANCED,
-                      label='Extra parameters: ', 
-                      help='Extra parameters to *relion_reconstruct* program. '
-                           'Address to Relion to see full list of options.')
-        form.addSection('CTF')
-        form.addParam('doCTF', BooleanParam, default=False,
-                      label='Apply CTF correction?')
-        form.addParam('ctfIntactFirstPeak', BooleanParam, default=False,
-                      condition='doCTF',
-                      label='Leave CTFs intact until first peak?')
-        
-        form.addParallelSection(threads=0, mpi=1)
+                      important=True,
+                      label='Input particles',
+                      pointerClass='SetOfParticles',
+                      help='Provide a set of particles.')
+        form.addParam('numToRemove', params.IntParam,
+                      default=0,
+                      label="Number of particles to remove",
+                      help="Number of particles to remove "
+                           "WITHIN the limits below.")
+
+        group = form.addGroup("Remove views WITHIN the limits below")
+        line = group.addLine('Rot')
+        line.addParam('rotMin', params.IntParam, default=-180,
+                      label='min')
+        line.addParam('rotMax', params.IntParam, default=180,
+                      label='max')
+
+        line = group.addLine('Tilt')
+        line.addParam('tiltMin', params.IntParam, default=0,
+                      label='min')
+        line.addParam('tiltMax', params.IntParam, default=180,
+                      label='max')
+
+        group.addParam('removePsi', params.BooleanParam, default=False,
+                       label="Remove views with specific in-plane rotation?",
+                       help="Particle orientation on Euler sphere is "
+                            "defined by rot and tilt angles. Psi is for "
+                            "in-plane rotation only. Select *Yes* "
+                            "if you want to provide psi limits.")
+        line = group.addLine('Psi', condition='removePsi')
+        line.addParam('psiMin', params.IntParam, default=-180,
+                      condition='removePsi', label='min')
+        line.addParam('psiMax', params.IntParam, default=180,
+                      condition='removePsi', label='max')
 
-    # -------------------------- INSERT steps functions -----------------------
+    # -------------------------- STEPS functions ------------------------------
     def _insertAllSteps(self):
-        self._createFilenameTemplates()
         self._insertFunctionStep('convertInputStep')
-        self._insertReconstructStep()
+        self._insertFunctionStep('processAnglesStep')
         self._insertFunctionStep('createOutputStep')
 
-    def _insertReconstructStep(self):
-        imgSet = self.inputParticles.get()
-
-        params = ' --i %s' % self._getFileName('input_particles')
-        params += ' --o %s' % self._getFileName('output_volume')
-        params += ' --sym %s' % self.symmetryGroup.get()
-        params += ' --angpix %0.5f' % imgSet.getSamplingRate()
-        params += ' --maxres %0.3f' % self.maxRes.get()
-        params += ' --pad %0.3f' % self.pad.get()
-
-        subset = -1 if self.subset.get() == 0 else self.subset
-        params += ' --subset %d' % subset
-        params += ' --class %d' % self.classNum.get()
-
-        if self.doCTF:
-            params += ' --ctf'
-            if self.ctfIntactFirstPeak:
-                params += ' --ctf_intact_first_peak'
-
-            if imgSet.isPhaseFlipped():
-                params += ' --ctf_phase_flipped'
-
-        if self.extraParams.hasValue():
-            params += " " + self.extraParams.get()
-
-        self._insertFunctionStep('reconstructStep', params)
+    def convertInputStep(self):
+        inputParts = self.inputParticles.get()
+        self.rotDict, self.tiltDict, self.psiDict = {}, {}, {}
+        for part in inputParts:
+            alignment = part.getTransform()
+            matrix = np.linalg.inv(alignment.getMatrix())
+            angles = -np.rad2deg(tfs.euler_from_matrix(matrix, axes='szyz'))
+            self.rotDict[part.getObjId()] = angles[0]
+            self.tiltDict[part.getObjId()] = angles[1]
+            self.psiDict[part.getObjId()] = angles[2]
+
+    def processAnglesStep(self):
+        self.removedList = []
+        ptclToRemove = self.numToRemove.get()
+        rmin, rmax = self.rotMin.get(), self.rotMax.get()
+        tmin, tmax = self.tiltMin.get(), self.tiltMax.get()
+        pmin, pmax = self.psiMin.get(), self.psiMax.get()
+
+        for (k, r), (k2, t), (k3, p) in zip(self.rotDict.items(),
+                                            self.tiltDict.items(),
+                                            self.psiDict.items()):
+            if not self.removePsi:
+                # check only rot & tilt
+                if (self.withinLimits(r, rmin, rmax) and
+                        self.withinLimits(t, tmin, tmax)):
+                    self.removedList.append(k)
+            else:
+                if (self.withinLimits(r, rmin, rmax) and
+                        self.withinLimits(t, tmin, tmax) and
+                        self.withinLimits(p, pmin, pmax)):
+                    self.removedList.append(k)
+
+        if ptclToRemove > len(self.removedList):
+            self.info("Number to remove (%d) is more than maximum available (%d). "
+                      "Removing %d particles..." % (ptclToRemove,
+                                                    len(self.removedList),
+                                                    len(self.removedList)))
+        else:
+            self.info("Randomly removing %d particles within "
+                      "specified limits..." % ptclToRemove)
+            self.removedList = sample(self.removedList, ptclToRemove)
 
-    # -------------------------- STEPS functions ------------------------------
-    def reconstructStep(self, params):
-        self._runProgram('relion_reconstruct', params)
+    def createOutputStep(self):
+        imgSet = self.inputParticles.get()
+        outImgSet = self._createSetOfParticles()
+        outImgSet.copyInfo(imgSet)
+        imgSet.setAlignmentProj()
+        outImgSet.copyItems(imgSet, updateItemCallback=self._removeViews)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
+        self._defineTransformRelation(self.inputParticles, outImgSet)
+
+    def _removeViews(self, item, row):
+        if item.getObjId() in self.removedList:
+            setattr(item, "_appendItem", False)
 
-    def _createFilenameTemplates(self):
-        """ Centralize how files are called for iterations and references. """
-        myDict = {
-            'input_particles': self._getTmpPath('input_particles.star'),
-            'output_volume': self._getExtraPath('output_volume.mrc')
-            }
-        self._updateFilenamesDict(myDict)
+    # --------------------------- INFO functions ------------------------------
+    def _summary(self):
+        summary = []
 
-    def convertInputStep(self):
-        """ Create the input file in STAR format as expected by Relion.
-        If the input particles comes from Relion, just link the file.
-        """
-        imgSet = self.inputParticles.get()
-        imgStar = self._getFileName('input_particles')
+        if hasattr(self, "outputParticles"):
+            summary.append("Input particles: %d" % self.inputParticles.get().getSize())
+            summary.append("Output particles: %d" % self.outputParticles.get().getSize())
 
-        # Pass stack file as None to avoid write the images files
-        convert.writeSetOfParticles(imgSet, imgStar,
-                                    outputDir=self._getTmpPath(),
-                                    alignType=ALIGN_PROJ)
+        return summary
 
-    def createOutputStep(self):
-        imgSet = self.inputParticles.get()
-        volume = Volume()
-        volume.setFileName(self._getFileName('output_volume'))
-        volume.setSamplingRate(imgSet.getSamplingRate())
-        
-        self._defineOutputs(outputVolume=volume)
-        self._defineSourceRelation(self.inputParticles, volume)
-    
-    # -------------------------- INFO functions -------------------------------
     def _validate(self):
         errors = []
 
+        if self.numToRemove > self.inputParticles.get().getSize():
+            errors.append("You cannot remove more particles "
+                          "than provided in the input.")
+
+        if (self.rotMin < -180 or self.psiMin < -180 or
+                self.rotMax > 180 or self.tiltMax > 180 or
+                self.psiMax > 180 or self.tiltMin < 0):
+            errors.append("Angles must be within the following limits:\n\n"
+                          "-180 < rot < 180\n0 < tilt < 180\n-180 < psi < 180\n")
+
         return errors
-    
-    def _summary(self):
-        summary = []
-        if not hasattr(self, 'outputVolume'):
-            summary.append("Output volume not ready yet.")
-        else:
-            summary.append("Output volume has been reconstructed.")
 
-        return summary
+    # -------------------------- UTILS functions ------------------------------
+    def withinLimits(self, value, min, max):
+        return min < float(value) < max
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_refine3d.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_refine3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,45 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
+from enum import Enum
 from emtable import Table
 
 from pyworkflow.constants import PROD
 from pwem.constants import ALIGN_PROJ
-from pwem.objects import Volume, FSC
+from pwem.objects import Volume, FSC, SetOfParticles
 from pwem.protocols import ProtRefine3D
 
 import relion.convert as convert
 from ..constants import PARTICLE_EXTRA_LABELS
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputVolume = Volume
+    outputParticles = SetOfParticles
+    outputFSC = FSC
+
+
 class ProtRelionRefine3D(ProtRefine3D, ProtRelionBase):
     """ Protocol to refine a 3D map using Relion.
 
 Relion employs an empirical Bayesian approach to refinement
 of (multiple) 3D reconstructions
 or 2D class averages in electron cryo-microscopy (cryo-EM). Many
 parameters of a statistical model are learned from the data,which
 leads to objective and high-quality results.
     """    
     _label = '3D auto-refine'
     _devStatus = PROD
+    _possibleOutputs = outputs
     IS_CLASSIFY = False
     CHANGE_LABELS = ['rlnChangesOptimalOrientations',
                      'rlnChangesOptimalOffsets',
                      'rlnOverallAccuracyRotations',
                      'rlnOverallAccuracyTranslationsAngst']
 
     PREFIXES = ['half1_', 'half2_']
@@ -98,27 +106,27 @@
         half2 = self._getFileName("final_half2_volume", ref3d=1)
         vol.setHalfMaps([half1, half2])
 
         outImgSet = self._createSetOfParticles()
         outImgSet.copyInfo(imgSet)
         self._fillDataFromIter(outImgSet, self._lastIter())
 
-        self._defineOutputs(outputVolume=vol)
+        self._defineOutputs(**{outputs.outputVolume.name: vol})
         self._defineSourceRelation(self.inputParticles, vol)
-        self._defineOutputs(outputParticles=outImgSet)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
         self._defineTransformRelation(self.inputParticles, outImgSet)
 
         fsc = FSC(objLabel=self.getRunName())
         fn = self._getExtraPath("relion_model.star")
         table = Table(fileName=fn, tableName='model_class_1')
         resolution_inv = table.getColumnValues('rlnResolution')
         frc = table.getColumnValues('rlnGoldStandardFsc')
         fsc.setData(resolution_inv, frc)
 
-        self._defineOutputs(outputFSC=fsc)
+        self._defineOutputs(**{outputs.outputFSC.name: fsc})
         self._defineSourceRelation(vol, fsc)
 
     # -------------------------- INFO functions -------------------------------
     def _validateNormal(self):
         errors = []
 
         if self.IS_3D and self.solventFscMask and not self.referenceMask.get():
@@ -169,15 +177,16 @@
     # -------------------------- UTILS functions ------------------------------
     def _fillDataFromIter(self, imgSet, iteration):
         outImgsFn = self._getFileName('data', iter=iteration)
         imgSet.setAlignmentProj()
         self.reader = convert.createReader(alignType=ALIGN_PROJ,
                                            pixelSize=imgSet.getSamplingRate())
 
-        mdIter = Table.iterRows('particles@' + outImgsFn, key='rlnImageId')
+        mdIter = Table.iterRows('particles@' + outImgsFn, key='rlnImageId',
+                                types=convert.LABELS_DICT)
         imgSet.copyItems(self._getInputParticles(), doClone=False,
                          updateItemCallback=self._updateParticle,
                          itemDataIterator=mdIter)
 
     def _updateParticle(self, particle, row):
         self.reader.setParticleTransform(particle, row)
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_remove_views.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_select_classes.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# ******************************************************************************
+# **************************************************************************
 # *
-# * Authors:     Grigory Sharov     (gsharov@mrc-lmb.cam.ac.uk)
+# * Authors:     Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk)
 # *
-# * MRC Laboratory of Molecular Biology, MRC-LMB
+# * MRC Laboratory of Molecular Biology (MRC-LMB)
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -18,151 +18,138 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# ******************************************************************************
+# **************************************************************************
 
-import numpy as np
-from random import sample
+from enum import Enum
+from emtable import Table
 
+from pyworkflow.object import Float
 import pyworkflow.protocol.params as params
 from pyworkflow.constants import PROD
-from pwem.protocols import ProtParticles
-import pwem.convert.transformations as tfs
+from pwem.protocols import ProtProcessParticles
+from pwem.objects import SetOfClasses2D, SetOfParticles
 
+from relion import Plugin
+from .protocol_base import ProtRelionBase
+from relion.convert import locationToRelion
 
-class ProtRelionRemovePrefViews(ProtParticles):
-    """ Protocol to remove preferential views from a particle set.
 
-    Inspired by https://github.com/leschzinerlab/Relion
+class outputs(Enum):
+    outputClasses = SetOfClasses2D
+    outputParticles = SetOfParticles
 
+
+class ProtRelionSelectClasses2D(ProtProcessParticles, ProtRelionBase):
+    """
+    Relion protocol to auto-select 2D class averages.
     """
-    _label = 'remove preferential views'
+    _label = '2D class ranker'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
+    # --------------------------- DEFINE param functions ----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
-        form.addParam('inputParticles', params.PointerParam,
-                      pointerCondition='hasAlignmentProj',
-                      important=True,
-                      label='Input particles',
-                      pointerClass='SetOfParticles',
-                      help='Provide a set of particles.')
-        form.addParam('numToRemove', params.IntParam,
-                      default=0,
-                      label="Number of particles to remove",
-                      help="Number of particles to remove "
-                           "WITHIN the limits below.")
-
-        group = form.addGroup("Remove views WITHIN the limits below")
-        line = group.addLine('Rot')
-        line.addParam('rotMin', params.IntParam, default=-180,
-                      label='min')
-        line.addParam('rotMax', params.IntParam, default=180,
-                      label='max')
-
-        line = group.addLine('Tilt')
-        line.addParam('tiltMin', params.IntParam, default=0,
-                      label='min')
-        line.addParam('tiltMax', params.IntParam, default=180,
-                      label='max')
-
-        group.addParam('removePsi', params.BooleanParam, default=False,
-                       label="Remove views with specific in-plane rotation?",
-                       help="Particle orientation on Euler sphere is "
-                            "defined by rot and tilt angles. Psi is for "
-                            "in-plane rotation only. Select *Yes* "
-                            "if you want to provide psi limits.")
-        line = group.addLine('Psi', condition='removePsi')
-        line.addParam('psiMin', params.IntParam, default=-180,
-                      condition='removePsi', label='min')
-        line.addParam('psiMax', params.IntParam, default=180,
-                      condition='removePsi', label='max')
+        form.addParam('inputProtocol', params.PointerParam,
+                      pointerClass='ProtRelionClassify2D',
+                      label="Input Relion 2D classification",
+                      important=True)
+        form.addParam('minThreshold', params.FloatParam, default=0.5,
+                      label='Min. threshold for auto-selection',
+                      help='Only classes with a predicted threshold '
+                           'above this value will be selected.')
+        form.addParam('minParts', params.IntParam, default=-1,
+                      label='Select at least this many particles',
+                      help='Even if they have scores below the minimum '
+                           'threshold, select at least this many particles '
+                           'with the best scores.')
+        form.addParam('minCls', params.IntParam, default=-1,
+                      label='OR: Select at least this many classes',
+                      help='Even if they have scores below the minimum '
+                           'threshold, select at least this many classes '
+                           'with the best scores.')
 
-    # -------------------------- STEPS functions ------------------------------
+    # --------------------------- INSERT steps functions ----------------------
     def _insertAllSteps(self):
-        self._insertFunctionStep('convertInputStep')
-        self._insertFunctionStep('processAnglesStep')
+        self._insertFunctionStep('runSelectStep')
         self._insertFunctionStep('createOutputStep')
 
-    def convertInputStep(self):
-        inputParts = self.inputParticles.get()
-        self.rotDict, self.tiltDict, self.psiDict = {}, {}, {}
-        for part in inputParts:
-            alignment = part.getTransform()
-            matrix = np.linalg.inv(alignment.getMatrix())
-            angles = -np.rad2deg(tfs.euler_from_matrix(matrix, axes='szyz'))
-            self.rotDict[part.getObjId()] = angles[0]
-            self.tiltDict[part.getObjId()] = angles[1]
-            self.psiDict[part.getObjId()] = angles[2]
-
-    def processAnglesStep(self):
-        self.removedList = []
-        ptclToRemove = self.numToRemove.get()
-        rmin, rmax = self.rotMin.get(), self.rotMax.get()
-        tmin, tmax = self.tiltMin.get(), self.tiltMax.get()
-        pmin, pmax = self.psiMin.get(), self.psiMax.get()
-
-        for (k, r), (k2, t), (k3, p) in zip(self.rotDict.items(),
-                                            self.tiltDict.items(),
-                                            self.psiDict.items()):
-            if not self.removePsi:
-                # check only rot & tilt
-                if (self.withinLimits(r, rmin, rmax) and
-                        self.withinLimits(t, tmin, tmax)):
-                    self.removedList.append(k)
-            else:
-                if (self.withinLimits(r, rmin, rmax) and
-                        self.withinLimits(t, tmin, tmax) and
-                        self.withinLimits(p, pmin, pmax)):
-                    self.removedList.append(k)
-
-        if ptclToRemove > len(self.removedList):
-            self.info("Number to remove (%d) is more than maximum available (%d). "
-                      "Removing %d particles..." % (ptclToRemove,
-                                                    len(self.removedList),
-                                                    len(self.removedList)))
-        else:
-            self.info("Randomly removing %d particles within "
-                      "specified limits..." % ptclToRemove)
-            self.removedList = sample(self.removedList, ptclToRemove)
+    # --------------------------- STEPS functions -----------------------------
+    def runSelectStep(self):
+        inputProt = self.inputProtocol.get()
+        inputProt._initialize()
+        fnOptimiser = inputProt._getFileName('optimiser',
+                                             iter=inputProt._lastIter())
+        params = " --opt %s --o %s --min_score %s" % (fnOptimiser,
+                                                      self._getExtraPath(),
+                                                      self.minThreshold.get())
+        params += " --fn_sel_parts particles.star"
+        params += " --fn_sel_classavgs class_averages.star"
+        params += " --fn_root rank --do_granularity_features"
+        params += " --auto_select"
+
+        if not Plugin.IS_GT50():
+            params += " --python $CONDA_PREFIX/bin/python"
+
+        if self.minParts != -1:
+            params += " --select_min_nr_particles %d" % self.minParts
+        if self.minCls != -1:
+            params += " --select_min_nr_classes %d" % self.minCls
+
+        self.runJob("%s && relion_class_ranker" % Plugin.getActivationCmd(), params)
 
     def createOutputStep(self):
-        imgSet = self.inputParticles.get()
-        outImgSet = self._createSetOfParticles()
-        outImgSet.copyInfo(imgSet)
-        imgSet.setAlignmentProj()
-        outImgSet.copyItems(imgSet, updateItemCallback=self._removeViews)
-        self._defineOutputs(outputParticles=outImgSet)
-        self._defineTransformRelation(self.inputParticles, outImgSet)
-
-    def _removeViews(self, item, row):
-        if item.getObjId() in self.removedList:
-            setattr(item, "_appendItem", False)
+        table = Table(fileName=self._getExtraPath('backup_selection.star'))
+        selected = len([s for s in table.getColumnValues('rlnSelected') if s])
+
+        if selected:
+            classesStar = self._getExtraPath('class_averages.star')
+            clsDict = {row.rlnReferenceImage: row
+                       for row in Table.iterRows(classesStar)}
+
+            inputClasses = self.inputProtocol.get().outputClasses
+            outputClasses = SetOfClasses2D.create(self._getExtraPath())
+            outputClasses.copyInfo(inputClasses)
+            inputParticles = inputClasses.getImages()
+            outputParticles = SetOfParticles.create(self._getExtraPath())
+            outputParticles.copyInfo(inputParticles)
+
+            def _getClassRow(cls2d):
+                idx, fn = cls2d.getRepresentative().getLocation()
+                return clsDict.get(locationToRelion(idx, fn), None)
+
+            def _updateClass(cls2d):
+                row = _getClassRow(cls2d)
+                cls2d._rlnPredictedClassScore = Float(row.rlnPredictedClassScore)
+                cls2d._rlnEstimatedResolution = Float(row.rlnEstimatedResolution)
+
+            outputClasses.appendFromClasses(inputClasses,
+                                            filterClassFunc=_getClassRow,
+                                            updateClassCallback=_updateClass)
+
+            self.summaryVar.set(f"Selected *{selected}* best classes.\n"
+                                f"Threshold: *{self.minThreshold.get()}*")
+            outputParticles.appendFromClasses(outputClasses)
+            self._defineOutputs(**{outputs.outputClasses.name: outputClasses,
+                                   outputs.outputParticles.name: outputParticles})
+            self._defineSourceRelation(inputClasses, outputClasses)
+            self._defineSourceRelation(inputParticles, outputParticles)
+        else:
+            self.summaryVar.set("No classes were selected.\n"
+                                "Try with a lower threshold.")
 
     # --------------------------- INFO functions ------------------------------
     def _summary(self):
-        summary = []
-
-        return summary
+        return [self.summaryVar.get(default="No summary information")]
 
     def _validate(self):
         errors = []
-
-        if self.numToRemove > self.inputParticles.get().getSize():
-            errors.append("You cannot remove more particles "
-                          "than provided in the input.")
-
-        if (self.rotMin < -180 or self.psiMin < -180 or
-                self.rotMax > 180 or self.tiltMax > 180 or
-                self.psiMax > 180 or self.tiltMin < 0):
-            errors.append("Angles must be within the following limits:\n\n"
-                          "-180 < rot < 180\n0 < tilt < 180\n-180 < psi < 180\n")
+        if self.minParts != -1 and self.minCls != -1:
+            errors.append("You cannot choose both min. number of particles "
+                          "and classes.")
 
         return errors
-
-    # -------------------------- UTILS functions ------------------------------
-    def withinLimits(self, value, min, max):
-        return min < float(value) < max
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_subtract.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_subtract.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,35 +20,42 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
+from enum import Enum
+
 from pyworkflow.object import String, Integer
 from pyworkflow.constants import PROD
 from pyworkflow.protocol.params import (PointerParam, BooleanParam,
-                                        IntParam, LabelParam, LEVEL_ADVANCED)
+                                        IntParam, LabelParam)
 from pwem.constants import ALIGN_PROJ
 from pwem.protocols import ProtOperateParticles
+from pwem.objects import SetOfParticles
 
 import relion.convert as convert
-from relion import Plugin
 from .protocol_base import ProtRelionBase
 
 
+class outputs(Enum):
+    outputParticles = SetOfParticles
+
+
 class ProtRelionSubtract(ProtOperateParticles, ProtRelionBase):
     """ Signal subtraction protocol of Relion.
 
     Subtract volume projections from the experimental particles.
     The particles must have projection alignment in order to
     properly generate volume projections.
     """
     _label = 'subtract projection'
     _devStatus = PROD
+    _possibleOutputs = outputs
 
     def _initialize(self):
         self._createFilenameTemplates()
     
     def _createFilenameTemplates(self):
         """ Centralize how files are called. """
         myDict = {
@@ -63,20 +70,21 @@
         form.addParam('relionInput', BooleanParam,
                       default=True, important=True,
                       label="Start from Relion protocol?",
                       help="Set to Yes if you wish to use as input "
                            "a Relion protocol. Otherwise set it to No")
         form.addParam('inputProtocol', PointerParam,
                       important=True,
-                      pointerClass='ProtRelionRefine3D, ProtRelionClassify3D',
+                      pointerClass='ProtRelionRefine3D, ProtRelionClassify3D,'
+                                   'ProtRelionMultiBody',
                       label="Input Relion protocol",
                       condition="relionInput",
-                      help="Select the 3D refinement/classification run which "
-                           "you want to use for subtraction. It will use the "
-                           "maps from this run for the subtraction.")
+                      help="Select the 3D refinement/classification or multi-body "
+                           "run which you want to use for subtraction. It will "
+                           "use the maps from this run for the subtraction.")
         form.addParam('inputVolume', PointerParam, pointerClass='Volume',
                       label="Input map to be projected",
                       important=True,
                       condition="not relionInput",
                       help='Provide the input volume that will be used to '
                            'calculate projections, which will be subtracted '
                            'from the experimental particles. Make sure this '
@@ -111,21 +119,19 @@
                       help="Provide a soft mask where the protein density "
                            "you wish to subtract from the experimental "
                            "particles is black (0) and the density you "
                            "wish to keep is white (1).\n"
                            "That is: *the mask should INCLUDE the part of the "
                            "volume that you wish to KEEP.*")
 
-        if Plugin.IS_GT31():
-            form.addParam('saveFloat16', BooleanParam, default=False,
-                          expertLevel=LEVEL_ADVANCED,
-                          label="Write output in float16?",
-                          help="Relion can write output images in float16 "
-                               "MRC (mode 12) format to save disk space. "
-                               "By default, float32 format is used.")
+        form.addParam('saveFloat16', BooleanParam, default=True,
+                      label="Write output in float16?",
+                      help="Relion can write output images in float16 "
+                           "MRC (mode 12) format to save disk space. "
+                           "By default, float32 format is used.")
 
         form.addSection('Centering')
         form.addParam('help1', LabelParam,
                       condition="not relionInput",
                       label="This section is only used if "
                             "starting from Relion input.")
         form.addParam('centerOnMask', BooleanParam, default=True,
@@ -219,15 +225,14 @@
         volume = self.inputVolume.get()
         volFn = convert.convertBinaryVol(volume,
                                          self._getExtraPath())
         params = ' --i %s --subtract_exp' % volFn
         params += ' --angpix %0.3f' % volume.getSamplingRate()
         params += self._convertMask(resize=False, invert=True)
 
-
         if self.doCTF:
             params += ' --ctf'
             if self.ignoreCTFUntilFirstPeak:
                 params += ' --ctf_intact_first_peak'
             if self._getInputParticles().isPhaseFlipped():
                 params += ' --ctf_phase_flip'
 
@@ -250,15 +255,15 @@
             params += " --data %s" % self._getFileName('input_star')
         if self.centerOnMask:
             params += " --recenter_on_mask"
         elif self.centerOnCoord:
             params += " --center_x %d --center_y %d --center_z %d" % (
                 self.cX, self.cY, self.cZ)
 
-        if Plugin.IS_GT31() and self.saveFloat16:
+        if self.saveFloat16:
             params += " --float16"
 
         params += self._convertMask()
         self.runJob(self._getProgram('relion_particle_subtract'), params)
 
     def createOutputStep(self):
         imgSet = self._getInputParticles()
@@ -266,36 +271,35 @@
         outImgsFn = self._getFileName('output_star')
         outImgSet.copyInfo(imgSet)
         outImgSet.setAlignmentProj()
 
         px = imgSet.getSamplingRate()
         self.reader = convert.createReader(alignType=ALIGN_PROJ,
                                            pixelSize=px)
-        mdIter = convert.Table.iterRows('particles@' + outImgsFn)
+        mdIter = convert.Table.iterRows('particles@' + outImgsFn,
+                                        types=convert.LABELS_DICT)
         outImgSet.copyItems(imgSet, doClone=False,
                             updateItemCallback=self._updateItem,
                             itemDataIterator=mdIter)
 
-        self._defineOutputs(outputParticles=outImgSet)
+        self._defineOutputs(**{outputs.outputParticles.name: outImgSet})
         self._defineTransformRelation(imgSet, outImgSet)
 
     # -------------------------- INFO functions -------------------------------
     def _validate(self):
         errors = []
         if not self.useAll:
             self._validateDim(self.inputParticles(),
                               self._getInputParticles().getXDim(),
                               errors, 'Input particles subset',
                               'Input particles from 3D protocol')
         if self.numberOfMpi > 1 and (not self.relionInput.get()):
             errors.append("Use of several CPUs when input is not relion "
                           "protocol is not supported")
-        if self.hasAttribute('saveFloat16') and self.saveFloat16:
-            errors.append("MRC float16 format is not yet supported by XMIPP, "
-                          "so you cannot use this option.")
+
         return errors
     
     def _summary(self):
         summary = []
         if not hasattr(self, 'outputParticles'):
             summary.append("Output is not ready yet.")
         else:
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols/protocol_symmetrize_volume.py` & `scipion-em-relion-5.0.0b1/relion/protocols/protocol_symmetrize_volume.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,18 @@
 class ProtRelionSymmetrizeVolume(ProtAlignVolume):
     """
     Symmetrize a volume using Relion programs:
         *relion_align_symmetry* and *relion_image_handler*.
     """
     _label = 'symmetrize volume'
     _devStatus = PROD
+    _possibleOutputs = {
+        'outputVolumeAligned': Volume,
+        'outputVolumeSymmetrized': Volume
+    }
     
     # --------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection(label='Input')
         form.addParam('inputVolume', params.PointerParam,
                       pointerClass='Volume',
                       label="Input volume", important=True,
@@ -80,7 +84,16 @@
             vol.copyInfo(self.inputVolume.get())
             vol.setLocation(fn)
             self._defineOutputs(**{name: vol})
             self._defineTransformRelation(self.inputVolume, vol)
 
         _defineOutputVol('outputVolumeAligned', alignedFn)
         _defineOutputVol('outputVolumeSymmetrized', symFn)
+
+    # -------------------------- INFO functions -------------------------------
+    def _summary(self):
+        summary = []
+        if not hasattr(self, 'outputVolumeSymmetrized'):
+            summary.append("Output is not ready yet.")
+        else:
+            summary.append("Symmetry used: *%s*" % self.symmetryGroup.get())
+        return summary
```

### Comparing `scipion-em-relion-4.0b8/relion/protocols.conf` & `scipion-em-relion-5.0.0b1/relion/protocols.conf`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,17 @@
   {"tag": "protocol", "value": "ProtRelionMultiBody", "text": "default"},
 	{"tag": "section", "text": "more", "openItem": "False", "children": []}
 	]},
 	{"tag": "protocol_group", "text": "Postprocess", "openItem": "False", "children": [
 	{"tag": "protocol", "value": "ProtRelionPostprocess", "text": "default"}
 	]},
 	{"tag": "protocol_group", "text": "Analysis", "openItem": "False", "children": [
-	{"tag": "section", "text": "Heterogeneity", "openItem": "False", "children": []},
+	{"tag": "section", "text": "Heterogeneity", "openItem": "False", "children": [
+	    {"tag": "protocol", "value": "ProtRelionDynaMight", "text": "default"}
+	]},
 	{"tag": "section", "text": "Validation", "openItem": "False", "children": []},
 	{"tag": "section", "text": "Resolution", "openItem": "False", "children": [
 	{"tag": "protocol", "value": "ProtRelionLocalRes", "text": "default"}
 	]},
 	{"tag": "section", "text": "more", "openItem": "False", "children": [
 	{"tag": "protocol", "value": "ProtRelionExpandSymmetry", "text": "default"},
   {"tag": "protocol", "value": "ProtRelionSubtract", "text": "default"},
```

### Comparing `scipion-em-relion-4.0b8/relion/relion_logo.jpg` & `scipion-em-relion-5.0.0b1/relion/relion_logo.jpg`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/tests/__init__.py` & `scipion-em-relion-5.0.0b1/relion/tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,18 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from .test_convert_relion import *
-from .test_protocols_relion import *
-from .test_protocols_relion3 import *
-from .test_workflow_relion3 import *
+from .test_convert import *
+from .test_protocols_2d import *
+from .test_protocols_3d import *
+from .test_workflow import *
 from .test_projection_subtraction_no_relion import *
 
 from pyworkflow.tests import DataSet
 
 DataSet(name='relion31_tutorial_precalculated',
         folder='relion31_tutorial_precalculated',
         files={})
```

### Comparing `scipion-em-relion-4.0b8/relion/tests/test_convert_relion.py` & `scipion-em-relion-5.0.0b1/relion/tests/test_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,15 +783,16 @@
 
         fog = OpticsGroups.fromImages(partsSet).first()
         self.assertEqual(fog.rlnMtfFileName, 'mtf_k2_200kV.star')
         self.assertEqual(fog.rlnOpticsGroupName, 'opticsGroup1')
 
     def test_readSetOfParticlesAfterCtf(self):
         starFile = self.ds.getFile("CtfRefine/job023/particles_ctf_refine.star")
-        partsReader = Table.Reader(starFile, tableName='particles')
+        partsReader = Table.Reader(starFile, tableName='particles',
+                                   types=convert.LABELS_DICT)
         firstRow = partsReader.getRow()
 
         partsSet = self.__readParticles(starFile)
         first = partsSet.getFirstItem()
 
         ogLabels = ['rlnBeamTiltX', 'rlnBeamTiltY']
         extraLabels = ['rlnCtfBfactor', 'rlnCtfScalefactor', 'rlnPhaseShift']
@@ -808,15 +809,16 @@
         print(">>> Writing to particles star: %s" % outputStar)
         starWriter = convert.createWriter()
         starWriter.writeSetOfParticles(partsSet, outputStar)
 
         fog = OpticsGroups.fromStar(outputStar).first()
         self.assertTrue(all(hasattr(fog, l) for l in ogLabels))
 
-        partsReader = Table.Reader(outputStar, tableName='particles')
+        partsReader = Table.Reader(outputStar, tableName='particles',
+                                   types=convert.LABELS_DICT)
         firstRow = partsReader.getRow()
         for l in extraLabels:
             value = getattr(first, '_%s' % l)
             self.assertIsNotNone(value, "Missing label: %s" % l)
             self.assertAlmostEqual(getattr(firstRow, l), value)
 
     def test_readOldStarFormat(self):
@@ -848,35 +850,32 @@
         og = OpticsGroups.fromStar(partsStar)
         fog = og.first()
 
         # test hasColumn method
         for colName in ['rlnMtfFileName', 'rlnOpticsGroupName']:
             self.assertTrue(og.hasColumn(colName))
 
-        # acq = first.getAcquisition()
         self.assertEqual(fog.rlnMtfFileName, 'mtf_k2_200kV.star')
         self.assertEqual(fog.rlnOpticsGroupName, 'opticsGroup1')
         self.assertEqual(og['opticsGroup1'], fog)
 
     def test_string(self):
         og = OpticsGroups.create(rlnMtfFileName='mtf_k2_200kV.star')
         fog = og.first()
 
-        # acq = first.getAcquisition()
         self.assertEqual(fog.rlnMtfFileName, 'mtf_k2_200kV.star')
         self.assertEqual(fog.rlnOpticsGroupName, 'opticsGroup1')
         self.assertEqual(og['opticsGroup1'], fog)
 
         # try update by id
         og.update(1, rlnMtfFileName="new_mtf_k2.star")
         # try update by name
         og.update('opticsGroup1', rlnImageSize=512)
 
         fog = og.first()
-        # acq = first.getAcquisition()
         self.assertEqual(fog.rlnMtfFileName, 'new_mtf_k2.star')
         self.assertEqual(fog.rlnImageSize, 512)
         self.assertEqual(fog.rlnOpticsGroupName, 'opticsGroup1')
         self.assertEqual(og['opticsGroup1'], fog)
 
     def test_add(self):
         """ Testing adding more groups or columns. """
```

### Comparing `scipion-em-relion-4.0b8/relion/tests/test_projection_subtraction_no_relion.py` & `scipion-em-relion-5.0.0b1/relion/tests/test_projection_subtraction_no_relion.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/tests/test_protocols_relion.py` & `scipion-em-relion-5.0.0b1/relion/tests/test_protocols_2d.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # **************************************************************************
 # *
-# * Authors:    Laura del Cano (ldelcano@cnb.csic.es)
+# * Authors:    Laura del Cano (ldelcano@cnb.csic.es) [1]
+# *             Grigory Sharov (gsharov@mrc-lmb.cam.ac.uk) [2]
+# *             J.M. De la Rosa Trevin (delarosatrevin@scilifelab.se) [3]
 # *
-# * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
+# * [1] Unidad de Bioinformatica of Centro Nacional de Biotecnologia, CSIC
+# * [2] MRC Laboratory of Molecular Biology, MRC-LMB
+# * [3] SciLifeLab, Stockholm University
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
 # * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
@@ -20,247 +24,182 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from pyworkflow.tests import BaseTest, setupTestProject, DataSet
+from glob import glob
+
+from pyworkflow.tests import setupTestProject, DataSet
 from pyworkflow.plugin import Domain
-from pyworkflow.protocol.constants import STATUS_FINISHED
 from pyworkflow.utils import magentaStr
-from pwem import Config
-from pwem.objects import SetOfParticles
-from pwem.protocols import *
+from pwem.objects import SetOfMovies
+from pwem.protocols import ProtImportAverages, ProtImportCTF, ProtImportParticles
 
 from ..protocols import *
 from ..convert import *
 from ..constants import *
+from relion.convert.convert31 import OpticsGroups
+from .test_protocols_base import TestRelionBase, USE_GPU, RUN_CPU, CPUS, MTF_FILE
 
 
-def useGpu():
-    """ Helper function to determine if GPU can be used.
-    Return a boolean and a label to be used in protocol's label. """
-    cudaPath = Plugin.getVar('RELION_CUDA_LIB', Config.CUDA_LIB)
-
-    if cudaPath and os.path.exists(cudaPath):
-        return True, 'GPU'
-    else:
-        return False, 'CPU'
-
-
-USE_GPU = useGpu()[0]
-ONLY_GPU = int(os.environ.get('SCIPION_TEST_RELION_ONLY_GPU', 0))
-RUN_CPU = not USE_GPU or ONLY_GPU
-
-
-class TestRelionBase(BaseTest):
+class TestRelionAssignOptics(TestRelionBase):
     @classmethod
-    def setData(cls, dataProject='mda'):
-        cls.dataset = DataSet.getDataSet(dataProject)
-        cls.particlesFn = cls.dataset.getFile('particles')
-        cls.vol = cls.dataset.getFile('volumes')
-
-    def checkOutput(self, prot, outputName, conditions=[]):
-        """ Check that an output was generated and
-        the condition is valid.
-        """
-        o = getattr(prot, outputName, None)
-        locals()[outputName] = o
-        self.assertIsNotNone(o, "Output: %s is None" % outputName)
-        for cond in conditions:
-            self.assertTrue(eval(cond), 'Condition failed: ' + cond)
-    
-    @classmethod
-    def runImportParticles(cls, pattern, samplingRate, checkStack=False):
-        """ Run an Import particles protocol. """
-        print(magentaStr("\n==> Importing data - particles from files:"))
-        protImport = cls.newProtocol(ProtImportParticles, 
-                                     filesPath=pattern,
-                                     samplingRate=samplingRate,
-                                     checkStack=checkStack)
-        cls.launchProtocol(protImport)
-        cls.assertIsNotNone(protImport.outputParticles,
-                            "SetOfParticles has not been produced.")
-
-        return protImport
-
-    @classmethod
-    def runImportParticlesStar(cls, partStar, mag, samplingRate):
-        """ Import particles from Relion star file. """
-        print(magentaStr("\n==> Importing data - particles from star:"))
-        protImport = cls.newProtocol(ProtImportParticles,
-                                     importFrom=ProtImportParticles.IMPORT_FROM_RELION,
-                                     starFile=partStar,
-                                     magnification=mag,
-                                     samplingRate=samplingRate,
-                                     haveDataBeenPhaseFlipped=True
-                                     )
-        cls.launchProtocol(protImport)
-        cls.assertIsNotNone(protImport.outputParticles,
-                            "SetOfParticles has not been produced.")
-
-        return protImport
-
-    @classmethod
-    def runNormalizeParticles(cls, particles):
-        """ Run normalize particles protocol """
-        print(magentaStr("\n==> Running relion - preprocess particles:"))
-        protPreproc = cls.newProtocol(ProtRelionPreprocessParticles,
-                                      doNormalize=True)
-        protPreproc.inputParticles.set(particles)
-        cls.launchProtocol(protPreproc)
-        return protPreproc
-    
-    @classmethod
-    def runImportVolumes(cls, pattern, samplingRate):
-        """ Run an Import particles protocol. """
-        print(magentaStr("\n==> Importing data - volumes:"))
-        protImport = cls.newProtocol(ProtImportVolumes, 
-                                     filesPath=pattern,
-                                     samplingRate=samplingRate)
-        cls.launchProtocol(protImport)
-        return protImport
+    def setUpClass(cls):
+        setupTestProject(cls)
+        cls.ds = DataSet.getDataSet('relion30_tutorial')
+        cls.protImport = cls.runImportMovies(filesPath=cls.ds.getFile('Movies/'),
+                                             filesPattern='20170629_000?5*tiff',
+                                             samplingRate=0.885,
+                                             voltage=200,
+                                             sphericalAberration=1.4,
+                                             dose=1.277,
+                                             gain=cls.ds.getFile("Movies/gain.mrc"))
+
+    def _checkOutputMovies(self, prot, size, exists=True,
+                           hasAlignment=True):
+        movies = getattr(prot, 'outputMovies', None)
+        self.assertIsNotNone(movies, "No movies were generated")
+        self.assertEqual(size, movies.getSize())
+
+        if hasAlignment:
+            self.assertTrue(movies.getFirstItem().hasAlignment())
+
+        if exists:
+            for m in movies:
+                self.assertTrue(os.path.exists(m.getFileName()))
+
+    def test_single(self):
+        def _checkAcq(output):
+            og = OpticsGroups.fromImages(output)
+            fog = og.first()
+            self.assertEqual(fog.rlnOpticsGroupName, "opticsGroupTest")
+            self.assertEqual(os.path.basename(fog.rlnMtfFileName),
+                             os.path.basename(MTF_FILE))
+
+        print(pwutils.magentaStr("\n==> Testing relion - assign optics groups:"))
+        protAssign = self.newProtocol(ProtRelionAssignOpticsGroup,
+                                      inputSet=self.protImport.outputMovies,
+                                      inputType=0,
+                                      opticsGroupName="opticsGroupTest",
+                                      mtfFile=MTF_FILE)
+        protAssign = self.launchProtocol(protAssign)
+
+        output = protAssign.outputMovies
+        self._checkOutputMovies(protAssign, 3, hasAlignment=False)
+        _checkAcq(output)
+        output.close()
+
+        print("Loading db: %s" % os.path.abspath(output.getFileName()))
+        moviesSet = SetOfMovies(filename=output.getFileName())
+        moviesSet.loadAllProperties()
+
+    def test_fromStar(self):
+        mtfStar = self.getOutputPath('input_mtf.star')
+        f = open(mtfStar, 'w')
+        f.write("""
+data_optics
+
+loop_ 
+_rlnOpticsGroupName #1 
+_rlnOpticsGroup #2 
+_rlnMtfFileName #3 
+_rlnMicrographOriginalPixelSize #4 
+_rlnVoltage #5 
+_rlnSphericalAberration #6 
+_rlnAmplitudeContrast #7 
+_rlnMicrographPixelSize #8 
+opticsGroup1            1 mtf_k2_200kV.star     0.885000   200.000000     1.400000     0.100000     0.885000
+opticsGroup2            2 mtf_k2_200kV.star     0.885000   200.000000     1.400000     0.100000     0.885000
+opticsGroup3            3 mtf_k2_200kV.star     0.885000   200.000000     1.400000     0.100000     0.885000
+
+data_micrographs
+
+loop_
+_rlnMicrographName #1 
+_rlnOpticsGroup #2 
+20170629_00025_frameImage.tiff 1
+20170629_00035_frameImage.tiff 2
+20170629_00045_frameImage.tiff 3
+        """)
+        f.close()
+
+        print(pwutils.magentaStr("\n==> Testing relion - assign optics groups (from star):"))
+        protAssign = self.newProtocol(ProtRelionAssignOpticsGroup,
+                                      objLabel='assign optics - from star',
+                                      inputSet=self.protImport.outputMovies,
+                                      inputType=1,  # from star file
+                                      inputStar=mtfStar)
+        protAssign = self.launchProtocol(protAssign)
+
+        outputMovies = protAssign.outputMovies
+        og = OpticsGroups.fromImages(outputMovies)
+        self.assertEqual(3, len(og))
 
-    @classmethod
-    def runImportMovies(cls, pattern, mag, samplingRate, dose):
-        """ Run an Import movies protocol. """
-        print(magentaStr("\n==> Importing data - movies:"))
-        protImport = cls.newProtocol(ProtImportMovies,
-                                     filesPath=pattern,
-                                     magnification=mag,
-                                     samplingRate=samplingRate,
-                                     dosePerFrame=dose)
-        cls.launchProtocol(protImport)
-        return protImport
+        for i, movie in enumerate(outputMovies):
+            self.assertEqual(i + 1, movie.getAttributeValue('_rlnOpticsGroup'))
 
 
-class TestRelionPicking(TestRelionBase):
+class TestRelionCenterAverages(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('relion_tutorial')
-        cls.partFn = cls.ds.getFile('import/classify2d/extra/relion_it015_data.star')
-
-        print(magentaStr("\n==> Importing data - micrographs:"))
-        cls.protImportMics = cls.newProtocol(
-            ProtImportMicrographs,
-            samplingRateMode=0,
-            filesPath='%s/*.mrc' % cls.ds.getFile('micrographs'),
-            samplingRate=7.08,
-            magnification=50000,
-            voltage=300,
-            sphericalAberration=0.1)
-        cls.launchProtocol(cls.protImportMics)
-
-    def _checkOutput(self, pickProt, minCoords, maxCoords):
-        """ Check that the outputCoordinates is not None
-         and that it should be between 300 and 400 coordinates
-         per micrograph.
-        """
-        coordSet = getattr(pickProt, 'outputCoordinates', None)
-        self.assertIsNotNone(coordSet)
-        for micAgg in coordSet.aggregate(["count"], "_micId", ["_micId"]):
-            self.assertGreaterEqual(micAgg['count'], minCoords)
-            self.assertLessEqual(micAgg['count'], maxCoords)
-
-    def testPickingLog(self):
-        print(magentaStr("\n==> Testing relion - autopick LoG:"))
-        protPickLog = self.newProtocol(
-            ProtRelionAutopickLoG,
-            objLabel='autopick LoG',
-            inputMicrographs=self.protImportMics.outputMicrographs,
-            boxSize=64,
-            minDiameter=260,
-            maxDiameter=360,
-            streamingBatchSize=5,
-        )
-        self.launchProtocol(protPickLog)
-        self._checkOutput(protPickLog, 300, 400)
-
-    def testPickingRef(self):
-        # Create a subset with a few good averages
-        ih = ImageHandler()
-        avgsFn = self.ds.getFile('import/classify2d/extra/'
-                                 'relion_it015_classes.mrcs')
-        outAvgsFn = os.path.abspath(self.proj.getTmpPath('averages.mrcs'))
-
-        for i, index in enumerate([5, 16, 17, 18, 31]):
-            ih.convert((index, avgsFn), (i + 1, outAvgsFn))
+        cls.ds = DataSet.getDataSet('mda')
 
+    def test_basic(self):
+        """ Run an Import averages protocol. """
         print(magentaStr("\n==> Importing data - averages:"))
-        protAvg = self.newProtocol(ProtImportAverages,
-                                   importFrom=ProtImportParticles.IMPORT_FROM_FILES,
-                                   filesPath=outAvgsFn,
-                                   samplingRate=7.08
-                                   )
-        self.launchProtocol(protAvg)
-
-        # We need CTF estimation for picking ref with Relion
-        # Now estimate CTF on the micrographs with ctffind
-        ProtCTFFind = Domain.importFromPlugin(
-            'cistem.protocols', 'CistemProtCTFFind', doRaise=True)
-
-        print(magentaStr("\n==> Running cistem - ctffind:"))
-        protCtf = self.newProtocol(
-            ProtCTFFind,
-            inputMicrographs=self.protImportMics.outputMicrographs,
-            minDefocus=12000, maxDefocus=30000,
-            slowSearch=False,
-            resamplePix=False,
-        )
-        self.launchProtocol(protCtf)
+        protImport = self.newProtocol(ProtImportAverages,
+                                      filesPath=self.ds.getFile('averages/averages.stk'),
+                                      samplingRate=5.04)
+        self.launchProtocol(protImport)
+        inputAvgs = protImport.outputAverages
+        print(magentaStr("\n==> Testing relion - center averages:"))
+        protCenter = self.newProtocol(ProtRelionCenterAverages)
+        protCenter.inputAverages.set(inputAvgs)
+        self.launchProtocol(protCenter)
 
-        print(magentaStr("\n==> Testing relion - autopick ref:"))
-        protPickRef = self.newProtocol(
-            ProtRelion2Autopick,
-            inputMicrographs=self.protImportMics.outputMicrographs,
-            ctfRelations=protCtf.outputCTF,
-            inputReferences=protAvg.outputAverages,
-            streamingBatchSize=5,
-        )
-        self.launchProtocol(protPickRef)
-        self._checkOutput(protPickRef, 320, 370)
+        conditions = ['outputAverages.getSize()==%d' % inputAvgs.getSize(),
+                      'outputAverages.getSamplingRate() - %0.5f < 0.00001'
+                      % inputAvgs.getSamplingRate()]
+        self.checkOutput(protCenter, 'outputAverages', conditions)
 
 
 class TestRelionClassify2D(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         TestRelionBase.setData('mda')
         cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
         cls.protNormalize = cls.runNormalizeParticles(cls.protImport.outputParticles)
-    
+
     def testRelion2D(self):
         def _runRelionClassify2D(doGpu=False, label=''):
             print(magentaStr("\n==> Testing relion - classify 2d:"))
             prot2D = self.newProtocol(ProtRelionClassify2D,
                                       doCTF=False, maskDiameterA=340,
                                       numberOfMpi=1, numberOfThreads=8)
             prot2D.numberOfClasses.set(4)
-            if Plugin.IS_GT31():
-                prot2D.numberOfVDAMBatches.set(100)
-            else:
-                prot2D.numberOfIterations.set(3)
+            prot2D.numberOfVDAMBatches.set(100)
             prot2D.inputParticles.set(self.protNormalize.outputParticles)
             prot2D.setObjLabel(label)
             prot2D.doGpu.set(doGpu)
             self.launchProtocol(prot2D)
             return prot2D
 
         def _checkAsserts(relionProt):
-
             self.assertIsNotNone(relionProt.outputClasses,
                                  "There was a problem with Relion 2D classify")
-        
+
             partsPixSize = self.protNormalize.outputParticles.getSamplingRate()
             classsesPixSize = relionProt.outputClasses.getImages().getSamplingRate()
             self.assertAlmostEquals(partsPixSize, classsesPixSize,
                                     msg="There was a problem with the sampling rate "
-                                    "of the particles", delta=0.001)
+                                        "of the particles", delta=0.001)
 
             for class2D in relionProt.outputClasses:
                 self.assertTrue(class2D.hasAlignment2D())
 
         if RUN_CPU:
             relionProt = _runRelionClassify2D(doGpu=False,
                                               label="Run Relion classify2D CPU")
@@ -268,687 +207,149 @@
 
         if USE_GPU:
             relionGpu = _runRelionClassify2D(doGpu=True,
                                              label="Relion classify2D GPU")
             _checkAsserts(relionGpu)
 
 
-class TestRelionClassify3D(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestRelionBase.setData('mda')
-        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
-        cls.protImportVol = cls.runImportVolumes(cls.vol, 3.5)
-    
-    def testProtRelionClassify3D(self):
-        print(magentaStr("\n==> Running relion - preprocess particles:"))
-        relionNormalize = self.newProtocol(ProtRelionPreprocessParticles)
-        relionNormalize.inputParticles.set(self.protImport.outputParticles)
-        relionNormalize.doNormalize.set(True)
-        self.launchProtocol(relionNormalize)
-
-        def _runRelionClassify3D(doGpu=False, label=''):
-            relion3DClass = self.newProtocol(ProtRelionClassify3D,
-                                             numberOfClasses=3,
-                                             numberOfIterations=4,
-                                             doCTF=False, runMode=1,
-                                             maskDiameterA=320,
-                                             numberOfMpi=2, numberOfThreads=2)
-
-            relion3DClass.setObjLabel(label)
-            relion3DClass.inputParticles.set(relionNormalize.outputParticles)
-            relion3DClass.referenceVolume.set(self.protImportVol.outputVolume)
-            relion3DClass.doGpu.set(doGpu)
-            self.launchProtocol(relion3DClass)
-            return relion3DClass
-
-        def _checkAsserts(relionProt):
-            self.assertIsNotNone(relionProt.outputClasses, "There was a "
-                                                           "problem with "
-                                                           "Relion 3D classify")
-
-            for class3D in relionProt.outputClasses:
-                self.assertTrue(class3D.hasAlignmentProj())
-
-        if RUN_CPU:
-            print(magentaStr("\n==> Testing relion - classify 3d on CPU:"))
-            relionProt = _runRelionClassify3D(doGpu=False,
-                                              label="Run Relion classify3D CPU")
-            _checkAsserts(relionProt)
-
-        if USE_GPU:
-            print(magentaStr("\n==> Testing relion - classify 3d on GPU:"))
-            relionGpu = _runRelionClassify3D(doGpu=True,
-                                             label="Relion classify3D GPU")
-            _checkAsserts(relionGpu)
-
-
-class TestRelionRefine(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestRelionBase.setData('mda')
-        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
-        cls.protImportVol = cls.runImportVolumes(cls.vol, 3.5)
-    
-    def testProtRelionRefine(self):
-        print(magentaStr("\n==> Running relion - preprocess particles:"))
-        relNorm = self.newProtocol(ProtRelionPreprocessParticles)
-        relNorm.inputParticles.set(self.protImport.outputParticles)
-        relNorm.doNormalize.set(True)
-        self.launchProtocol(relNorm)
-        
-        def _runRelionRefine(doGpu=False, label=''):
-            relionRefine = self.newProtocol(ProtRelionRefine3D,
-                                            doCTF=False, runMode=1,
-                                            maskDiameterA=340,
-                                            symmetryGroup="d6",
-                                            numberOfMpi=3, numberOfThreads=2)
-            relionRefine.setObjLabel(label)
-            relionRefine.inputParticles.set(relNorm.outputParticles)
-            relionRefine.referenceVolume.set(self.protImportVol.outputVolume)
-            relionRefine.doGpu.set(doGpu)
-            self.launchProtocol(relionRefine)
-            return relionRefine
-        
-        def _checkAsserts(relionRefine):
-            relionRefine._initialize()  # Load filename templates
-            dataSqlite = relionRefine._getIterData(3)
-            outImgSet = SetOfParticles(filename=dataSqlite)
-            
-            self.assertIsNotNone(relionRefine.outputVolume,
-                                 "There was a problem with Relion autorefine")
-            self.assertAlmostEqual(outImgSet[1].getSamplingRate(),
-                                   relNorm.outputParticles[1].getSamplingRate(),
-                                   msg="The sampling rate is wrong", delta=0.00001)
-            
-            self.assertAlmostEqual(outImgSet[1].getFileName(),
-                                   relNorm.outputParticles[1].getFileName(),
-                                   msg="The particles filenames are wrong")
-        
-        if RUN_CPU:
-            print(magentaStr("\n==> Testing relion - refine 3d on CPU:"))
-            relionProt = _runRelionRefine(doGpu=False,
-                                          label="Run Relion auto-refine CPU")
-            _checkAsserts(relionProt)
-
-        if USE_GPU:
-            print(magentaStr("\n==> Testing relion - refine 3d on GPU:"))
-            relionGpu = _runRelionRefine(doGpu=True,
-                                         label="Run Relion auto-refine GPU")
-            _checkAsserts(relionGpu)
-
-
-class TestRelionInitialModel(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet('relion_tutorial')
-        cls.partFn = cls.dataset.getFile('import/classify2d/extra/relion_it015_data.star')
-        cls.protImport = cls.runImportParticlesStar(cls.partFn, 50000, 7.08)
-
-    def testProtRelionIniModel(self):
-        def _runRelionIniModel(doGpu=True, label=''):
-            kwargs = {
-                'doCTF': False,
-                'doGpu': doGpu,
-                'maskDiameterA': 340,
-                'symmetryGroup': 'C1',
-                'allParticlesRam': True,
-                'numberOfMpi': 1,
-                'numberOfThreads': 8
-            }
-
-            print(magentaStr("\n==> Testing relion - initial model:"))
-            relionIniModel = self.newProtocol(ProtRelionInitialModel, **kwargs)
-            relionIniModel.setObjLabel(label)
-            relionIniModel.inputParticles.set(self.protImport.outputParticles)
-            self.launchProtocol(relionIniModel)
-
-            return relionIniModel
-
-        def _checkAsserts(relionProt):
-            relionProt._initialize()  # Load filename templates
-            dataSqlite = relionProt._getIterData(relionProt._lastIter())
-            outImgSet = SetOfParticles(filename=dataSqlite)
-
-            self.assertIsNotNone(relionProt.outputVolume,
-                                 "There was a problem with Relion initial model")
-            self.assertAlmostEqual(outImgSet[1].getSamplingRate(),
-                                   self.protImport.outputParticles[1].getSamplingRate(),
-                                   msg="The sampling rate is wrong", delta=0.00001)
-
-        relionProt = _runRelionIniModel(
-            doGpu=USE_GPU, label="Relion initial model %s"
-                                 % ('GPU' if USE_GPU else 'CPU'))
-        _checkAsserts(relionProt)
-
-        
-class TestRelionPreprocess(TestRelionBase):
-    """ This class helps to test all different preprocessing particles options
-    on Relion. """
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestRelionBase.setData('mda')
-        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
-
-    def _validations(self, imgSet, dims, pxSize):
-        self.assertIsNotNone(imgSet, "There was a problem with preprocess "
-                                     "particles")
-        xDim = imgSet.getXDim()
-        sr = imgSet.getSamplingRate()
-        self.assertEqual(xDim, dims, "The dimension of your particles are %d x "
-                                     "%d and must be  %d x %d" % (xDim, xDim,
-                                                                  dims, dims))
-        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
-                               msg="Pixel size of your particles are  %0.5f and"
-                               " must be %0.5f" % (sr, pxSize))
-
-    def test_NormalizeAndDust(self):
-        print(magentaStr("\n==> Testing relion - preprocess particles (norm, remove dust):"))
-        protocol = self.newProtocol(ProtRelionPreprocessParticles,
-                                    doNormalize=True, backRadius=40,
-                                    doRemoveDust=True, whiteDust=4, blackDust=8)
-        protocol.setObjLabel('relion: norm-dust')
-        protocol.inputParticles.set(self.protImport.outputParticles)
-        self.launchProtocol(protocol)
-        
-        self._validations(protocol.outputParticles, 100, 3.5)
-        
-    def test_ScaleAndInvert(self):
-        print(magentaStr("\n==> Testing relion - preprocess particles (scale, invert):"))
-        protocol = self.newProtocol(ProtRelionPreprocessParticles,
-                                    doNormalize=False,
-                                    doScale=True, scaleSize=50,
-                                    doInvert=True)
-        protocol.setObjLabel('relion: scale-invert')
-        protocol.inputParticles.set(self.protImport.outputParticles)
-        
-        self.launchProtocol(protocol)
-        self._validations(protocol.outputParticles, 50, 7.0)
-
-
-class TestRelionSubtract(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        TestRelionBase.setData('mda')
-        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
-        cls.protImportVol = cls.runImportVolumes(cls.vol, 3.5)
-
-    def test_subtract(self):
-        print(magentaStr("\n==> Running relion - refine 3d:"))
-        relionRefine = self.newProtocol(ProtRelionRefine3D,
-                                        doCTF=False, runMode=1,
-                                        maskDiameterA=340,
-                                        symmetryGroup="d6",
-                                        numberOfMpi=3, numberOfThreads=2)
-        relionRefine.inputParticles.set(self.protImport.outputParticles)
-        relionRefine.referenceVolume.set(self.protImportVol.outputVolume)
-        relionRefine.doGpu.set(False)
-        self.launchProtocol(relionRefine)
-
-        print(magentaStr("\n==> Running relion - create mask 3d:"))
-        protMask = self.newProtocol(ProtRelionCreateMask3D, threshold=0.045)
-        protMask.inputVolume.set(relionRefine.outputVolume)
-        self.launchProtocol(protMask)
-
-        print(magentaStr("\n==> Testing relion - subtract projection:"))
-        protSubtract = self.newProtocol(ProtRelionSubtract,
-                                        refMask=protMask.outputMask,
-                                        numberOfMpi=2)
-        protSubtract.inputProtocol.set(relionRefine)
-        self.launchProtocol(protSubtract)
-        self.assertIsNotNone(protSubtract.outputParticles,
-                             "There was a problem with subtract projection")
-
-
-class TestRelionPostprocess(TestRelionBase):
-    """ This class helps to test postprocess protocol from Relion. """
-
+class TestRelionExportCtf(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('relion_tutorial')
-        pathFns = 'import/refine3d/extra'
-        cls.volFn = cls.ds.getFile(join(pathFns, 'relion_class001.mrc'))
-        cls.half1Fn = cls.ds.getFile(join(pathFns, 'relion_it025_half1_class001.mrc'))
-        cls.half2Fn = cls.ds.getFile(join(pathFns, 'relion_it025_half2_class001.mrc'))
-
-    def importVolume(self):
-
-        protVol = self.newProtocol(ProtImportVolumes,
-                                   objLabel='import volume',
-                                   filesPath=self.volFn,
-                                   samplingRate=3)
-        self.launchProtocol(protVol)
-        return protVol
-
-    def importPartsFromScipion(self):
-        partFn = self.ds.getFile('import/particles.sqlite')
-        protPart = self.newProtocol(ProtImportParticles,
-                                    objLabel='Import Particles',
-                                    importFrom=ProtImportParticles.IMPORT_FROM_SCIPION,
-                                    sqliteFile=partFn,
-                                    magnification=10000,
-                                    samplingRate=3,
-                                    haveDataBeenPhaseFlipped=True
-                                    )
-        self.launchProtocol(protPart)
-        return protPart
-
-    def _createRef3DProtBox(self, label, protocol,
-                            storeIter=False, iterN=0):
-        from pyworkflow.protocol.constants import STATUS_FINISHED
-
-        prot = self.newProtocol(protocol)
-        self.saveProtocol(prot)
-
-        prot.setObjLabel(label)
-        pwutils.makePath(prot._getPath())
-        pwutils.makePath(prot._getExtraPath())
-        pwutils.makePath(prot._getTmpPath())
-
-        prot.inputParticles.set(self.importPartsFromScipion().outputParticles)
-
-        protClassName = prot.getClassName()
-        outputVol = self.importVolume().outputVolume
-        if protClassName.startswith('ProtRelionRefine3D'):
-            prot.referenceVolume.set(outputVol)
-        elif protClassName.startswith('XmippProtProjMatch'):
-            prot.input3DReferences.set(outputVol)
-        elif protClassName.startswith('EmanProtRefine'):
-            prot.input3DReference.set(outputVol)
-
-        volume = Volume()
-        volume.setFileName(prot._getExtraPath('test.mrc'))
-        pxSize = prot.inputParticles.get().getSamplingRate()
-        volume.setSamplingRate(pxSize)
-        if storeIter:
-            prot._setLastIter(iterN)
-        prot._defineOutputs(outputVolume=volume)
-
-        prot.setStatus(STATUS_FINISHED)
-
-        # Create a mask protocol, because now it is not part of post-process
-        protMask = self.newProtocol(ProtRelionCreateMask3D)
-        protMask.inputVolume.set(outputVol)
-        self.launchProtocol(protMask)
-
-        return prot, protMask
-
-    def _validations(self, vol, dims, pxSize, prot=""):
-        self.assertIsNotNone(vol, "There was a problem with postprocess "
-                                  "protocol, using %s protocol as input" % prot)
-        xDim = vol.getXDim()
-        sr = vol.getSamplingRate()
-        self.assertEqual(xDim, dims, "The dimension of your volume is (%d)^3 "
-                                     "and must be (%d)^3" % (xDim, dims))
-
-        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
-                               msg="Pixel size of your volume is %0.5f and"
-                               " must be %0.5f" % (sr, pxSize))
+        cls.dsXmipp = DataSet.getDataSet('xmipp_tutorial')
+        cls.dsGrigorieff = DataSet.getDataSet('grigorieff')
+        cls.dsEman2 = DataSet.getDataSet('eman')
+        cls.protImport = cls.runImportMics(cls.dsXmipp.getFile('allMics'), 1.237)
 
-    def test_postProcess_from_autorefine(self):
-        print(magentaStr("\n==> Testing relion - postprocess after refine 3d:"))
-        protRef, protMask = self._createRef3DProtBox("auto-refine",
-                                                     ProtRelionRefine3D)
-        protRef._createFilenameTemplates()
-        volPath = protRef._getFileName('finalvolume', ref3d=1).split(':')[0]
-        volHalf1 = protRef._getFileName('final_half1_volume', ref3d=1).split(':')[0]
-        volHalf2 = protRef._getFileName('final_half2_volume', ref3d=1).split(':')[0]
-
-        pwutils.copyFile(self.volFn, volPath)
-        pwutils.copyFile(self.half1Fn, volHalf1)
-        pwutils.copyFile(self.half2Fn, volHalf2)
-
-        protRef.outputVolume.setFileName(volPath)
-        protRef.outputVolume.setHalfMaps([volHalf1, volHalf2])
-        project = protRef.getProject()
-        project._storeProtocol(protRef)
-
-        postProt = self.newProtocol(ProtRelionPostprocess,
-                                    protRefine=protRef,
-                                    solventMask=protMask.outputMask)
-        postProt.setObjLabel('post process Auto-refine')
-
-        self.launchProtocol(postProt)
-        self._validations(postProt.outputVolume, 60, 3, "Relion auto-refine")
-
-    def test_postProcess_from_projMatch(self):
-        print(magentaStr("\n==> Testing relion - postprocess after xmipp proj. match.:"))
-        XmippProtProjMatch = Domain.importFromPlugin('xmipp3.protocols',
-                                                     'XmippProtProjMatch')
+    def runImportXmipp(self):
+        print(magentaStr("\n==> Importing data - ctfs (from xmipp):"))
+        protCTF = self.newProtocol(ProtImportCTF,
+                                   importFrom=ProtImportCTF.IMPORT_FROM_XMIPP3,
+                                   filesPath=self.dsXmipp.getFile('ctfsDir'),
+                                   filesPattern='*.ctfparam')
+        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
+        protCTF.setObjLabel('import ctfs from xmipp ')
+        self.launchProtocol(protCTF)
 
-        if XmippProtProjMatch is None:
-            print("WARNING: Can not load xmipp3.protocols.XmippProtProjMatch."
-                  "Skipping the tests.")
-            return
+        self.assertIsNotNone(protCTF.outputCTF,
+                             "There was a problem when importing ctfs.")
+        return protCTF
 
-        protRef, protMask = self._createRef3DProtBox(
-            "Proj Match", XmippProtProjMatch, storeIter=True, iterN=2)
+    def runImportCtffind4(self):
+        print(magentaStr("\n==> Importing data - ctfs (from ctffind):"))
+        protCTF = self.newProtocol(ProtImportCTF,
+                                   importFrom=ProtImportCTF.IMPORT_FROM_GRIGORIEFF,
+                                   filesPath=self.dsGrigorieff.getFile('ctffind4'),
+                                   filesPattern='BPV*/*txt')
+        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
+        protCTF.setObjLabel('import from ctffind4')
+        self.launchProtocol(protCTF)
 
-        pwutils.makePath(join(protRef._getExtraPath(), 'iter_002'))
-        protRef._initialize()
-        volXmipp = protRef._getFileName('reconstructedFileNamesIters',
-                                        iter=2, ref=1)
-        half1Xmipp = protRef._getFileName('reconstructedFileNamesItersSplit1',
-                                          iter=2, ref=1)
-        half2Xmipp = protRef._getFileName('reconstructedFileNamesItersSplit2',
-                                          iter=2, ref=1)
-        
-        ih = ImageHandler()
-        ih.convert(ih.getVolFileName(self.volFn), volXmipp)
-        ih.convert(ih.getVolFileName(self.half1Fn), half1Xmipp)
-        ih.convert(ih.getVolFileName(self.half2Fn), half2Xmipp)
-
-        protRef.outputVolume.setFileName(volXmipp)
-        protRef.outputVolume.setHalfMaps([half1Xmipp, half2Xmipp])
-        project = protRef.getProject()
-        project._storeProtocol(protRef)
-
-        postProt = self.newProtocol(ProtRelionPostprocess,
-                                    protRefine=protRef,
-                                    solventMask=protMask.outputMask)
-        postProt.setObjLabel('post process Xmipp Projection Matching')
-        self.launchProtocol(postProt)
-        self._validations(postProt.outputVolume, 60, 3, "Projection Matching")
-    
-    def test_postProcess_from_eman_refineEasy(self):
-        print(magentaStr("\n==> Testing relion - postprocess after eman2 refine easy:"))
-        EmanProtRefine = Domain.importFromPlugin('eman2.protocols', 'EmanProtRefine')
-        convertImage = Domain.importFromPlugin('eman2.convert', 'convertImage')
-
-        protRef, protMask = self._createRef3DProtBox(
-            "Eman refine Easy", EmanProtRefine)
-
-        pwutils.makePath(join(protRef._getExtraPath(), 'refine_01'))
-        protRef._createFilenameTemplates()
-        volEman = protRef._getFileName("mapFull", run=1, iter=2)
-        half1Eman = protRef._getFileName("mapEvenUnmasked", run=1)
-        half2Eman = protRef._getFileName("mapOddUnmasked", run=1)
-        
-        convertImage(self.volFn, volEman)
-        convertImage(self.half1Fn, half1Eman)
-        convertImage(self.half2Fn, half2Eman)
-
-        protRef.outputVolume.setFileName(volEman)
-        protRef.outputVolume.setHalfMaps([half1Eman, half2Eman])
-        project = protRef.getProject()
-        project._storeProtocol(protRef)
-
-        postProt = self.newProtocol(ProtRelionPostprocess,
-                                    protRefine=protRef,
-                                    solventMask=protMask.outputMask)
-        postProt.setObjLabel('post process Eman2 refine-easy')
-        self.launchProtocol(postProt)
-        self._validations(postProt.outputVolume, 60, 3, "Eman refine easy")
+        self.assertIsNotNone(protCTF.outputCTF,
+                             "There was a problem when importing ctfs.")
+        return protCTF
 
+    def runImportScipion(self):
+        print(magentaStr("\n==> Importing data - ctfs (from scipion):"))
+        ctfSqlite = self.dsGrigorieff.getFile('ctffind3/ctfs.sqlite')
 
-class TestRelionLocalRes(TestRelionBase):
-    """ This class helps to test local resolution protocol from Relion. """
+        protCTF = self.newProtocol(ProtImportCTF,
+                                   objLabel='import from scipion',
+                                   importFrom=ProtImportCTF.IMPORT_FROM_SCIPION,
+                                   filesPath=ctfSqlite)
 
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('relion_tutorial')
-        pathFns = 'import/refine3d/extra'
-        cls.partFn = cls.ds.getFile(join(pathFns, 'relion_it025_data.star'))
-        cls.protImport = cls.runImportParticlesStar(cls.partFn, 50000, 7.08)
-        cls.volFn = cls.ds.getFile(join(pathFns, 'relion_class001.mrc'))
-        cls.half1Fn = cls.ds.getFile(join(pathFns, 'relion_it025_half1_class001.mrc'))
-        cls.half2Fn = cls.ds.getFile(join(pathFns, 'relion_it025_half2_class001.mrc'))
-        cls.modelFn = cls.ds.getFile(join(pathFns, 'relion_model.star'))
-
-    def importVolume(self):
-        print(magentaStr("\n==> Importing data - volume:"))
-        protVol = self.newProtocol(ProtImportVolumes,
-                                   objLabel='import volume',
-                                   filesPath=self.volFn,
-                                   samplingRate=7.08)
-        self.launchProtocol(protVol)
-        return protVol
-
-    def _createRef3DProtBox(self, label):
-        prot = self.newProtocol(ProtRelionRefine3D)
-        self.saveProtocol(prot)
-
-        prot.setObjLabel(label)
-        pwutils.makePath(prot._getPath())
-        pwutils.makePath(prot._getExtraPath())
-        pwutils.makePath(prot._getTmpPath())
-
-        prot.inputParticles.set(self.protImport.outputParticles)
-        prot.referenceVolume.set(self.importVolume().outputVolume)
-
-        volume = Volume()
-        volume.setFileName(prot._getExtraPath('test.mrc'))
-        pxSize = prot.inputParticles.get().getSamplingRate()
-        volume.setSamplingRate(pxSize)
-
-        prot._defineOutputs(outputVolume=volume)
-        prot.setStatus(STATUS_FINISHED)
-
-        return prot
-
-    def _validations(self, vol, dims, pxSize):
-        self.assertIsNotNone(vol, "There was a problem with localres protocol ")
-        xDim = vol.getXDim()
-        sr = vol.getSamplingRate()
-        self.assertEqual(xDim, dims, "The dimension of your volume is (%d)^3 "
-                                     "and must be (%d)^3" % (xDim, dims))
-        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
-                               msg="Pixel size of your volume is %0.5f and"
-                               " must be %0.5f" % (sr, pxSize))
+        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
+        self.launchProtocol(protCTF)
 
-    def test_runRelionLocalRes(self):
-        protRef = self._createRef3DProtBox("auto-refine")
+        self.assertIsNotNone(protCTF.outputCTF,
+                             "There was a problem when importing ctfs.")
+        return protCTF
 
-        protRef._createFilenameTemplates()
-        volPath = protRef._getFileName('finalvolume', ref3d=1).split(':')[0]
-        volHalf1 = protRef._getFileName('final_half1_volume', ref3d=1).split(':')[0]
-        volHalf2 = protRef._getFileName('final_half2_volume', ref3d=1).split(':')[0]
-
-        pwutils.copyFile(self.volFn, volPath)
-        pwutils.copyFile(self.half1Fn, volHalf1)
-        pwutils.copyFile(self.half2Fn, volHalf2)
-        pwutils.copyFile(self.modelFn,
-                         protRef._getExtraPath('relion_model.star'))
-
-        protRef.outputVolume.setFileName(volPath)
-        protRef.outputVolume.setHalfMaps([volHalf1, volHalf2])
-        project = protRef.getProject()
-        project._storeProtocol(protRef)
-
-        restProt = self.newProtocol(ProtRelionLocalRes, protRefine=protRef)
-        print(magentaStr("\n==> Testing relion - local resolution:"))
-        restProt.setObjLabel('Relion local resolution')
-
-        self.launchProtocol(restProt)
-        self._validations(restProt.outputVolume, 60, 7.08)
-
-        # Add also a test case for the mask
-        print(magentaStr("\n==> Importing data - mask 3D:"))
-        protMask = self.newProtocol(ProtRelionCreateMask3D,
-                                    inputVolume=protRef.outputVolume,
-                                    initialLowPassFilterA=30)
-        self.launchProtocol(protMask)
-
-        print(magentaStr("\n==> Testing relion - local resolution (with mask):"))
-        restProt = self.newProtocol(ProtRelionLocalRes,
-                                    objLabel='relion localres (with mask)',
-                                    protRefine=protRef,
-                                    solventMask=protMask.outputMask)
-        self.launchProtocol(restProt)
+    def runImportEman2(self):
+        print(magentaStr("\n==> Importing data - ctfs (from eman2):"))
+        protCTF = self.newProtocol(ProtImportCTF,
+                                   importFrom=ProtImportCTF.IMPORT_FROM_EMAN2,
+                                   filesPath=self.dsEman2.getFile('ctfs'),
+                                   filesPattern='BPV*json')
+        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
+        protCTF.setObjLabel('import from eman2')
+        self.launchProtocol(protCTF)
 
+        self.assertIsNotNone(protCTF.outputCTF,
+                             "There was a problem when importing ctfs.")
+        return protCTF
 
-class TestRelionExpandSymmetry(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.dataset = DataSet.getDataSet('relion_tutorial')
-        cls.partRef3dFn = cls.dataset.getFile('import/refine3d/extra/relion_data.star')
+    def testExportCtf(self):
+        ctfs = [(self.runImportXmipp().outputCTF, 'xmipp'),
+                (self.runImportCtffind4().outputCTF, 'ctffind'),
+                (self.runImportScipion().outputCTF, 'scipion'),
+                (self.runImportEman2().outputCTF, 'eman2')]
 
-    def importParticles(self, partStar):
-        """ Import particles from Relion star file. """
-        print(magentaStr("\n==> Importing data - particles:"))
-        protPart = self.newProtocol(ProtImportParticles,
-                                    importFrom=ProtImportParticles.IMPORT_FROM_RELION,
-                                    starFile=partStar,
-                                    magnification=10000,
-                                    samplingRate=7.08,
-                                    haveDataBeenPhaseFlipped=False
-                                    )
-        self.launchProtocol(protPart)
-        return protPart
-
-    def test_ExpandSymmetry(self):
-        print(magentaStr("\n==> Testing relion - expand symmetry:"))
-        prot = self.newProtocol(ProtRelionExpandSymmetry)
-        importRun = self.importParticles(self.partRef3dFn)
-        prot.inputParticles.set(importRun.outputParticles)
-        prot.symmetryGroup.set("D2")
-        self.launchProtocol(prot)
+        for i in ctfs:
+            protExport = self.newProtocol(ProtRelionExportCtf)
+            protExport.inputCTF.set(i[0])
+            print(magentaStr("\n==> Testing relion - export ctf (from %s):" % i[1]))
+            self.launchProtocol(protExport)
 
-        self.assertIsNotNone(prot.outputParticles,
-                             "There was a problem with expand symmetry protocol")
-        sizeIn = importRun.outputParticles.getSize()
-        sizeOut = prot.outputParticles.getSize()
-        self.assertAlmostEqual(sizeIn * 4, sizeOut, delta=0.0001,
-                               msg="Number of output particles is %d and"
-                               " must be %d" % (sizeOut, sizeIn * 4))
+            outFn = os.path.exists(protExport._getStarFile()) or None
+            self.assertIsNotNone(outFn,
+                                 "There was a problem when exporting ctfs.")
 
 
-class TestRelionCreate3dMask(TestRelionBase):
+class TestRelionExportParticles(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.ds = DataSet.getDataSet('relion_tutorial')
+        cls.ds2 = DataSet.getDataSet('xmipp_tutorial')
+        cls.particlesFn = cls.ds.getFile('import/refine3d/extra/relion_data.star')
+        cls.particlesFn2 = cls.ds2.getFile('particles')
+        cls.starImport = cls.runImportParticlesStar(cls.particlesFn, 7.08)
+        cls.protImport = cls.runImportParticles(cls.particlesFn2, 1.237, checkStack=True)
 
-    def importVolume(self):
-        print(magentaStr("\n==> Importing data - volume:"))
-        volFn = self.ds.getFile('import/refine3d/extra/relion_class001.mrc')
-        protVol = self.newProtocol(ProtImportVolumes,
-                                   objLabel='import volume',
-                                   filesPath=volFn,
-                                   samplingRate=3)
-        self.launchProtocol(protVol)
-        return protVol
-
-    def _validations(self, mask, dims, pxSize, prot):
-        self.assertIsNotNone(mask, "There was a problem with mask 3d protocol, "
-                                   "using %s protocol as input" % prot)
-        xDim = mask.getXDim()
-        sr = mask.getSamplingRate()
-        self.assertEqual(xDim, dims, "The dimension of your volume is (%d)^3 "
-                                     "and must be (%d)^3" % (xDim, dims))
-
-        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
-                               msg="Pixel size of your volume is %0.5f and"
-                               " must be %0.5f" % (sr, pxSize))
-
-    def test_createMask(self):
-        importProt = self.importVolume()
+    def run_combinations(self, inputProt, name=''):
+        """ Run an Import particles protocol. """
+        inputParts = inputProt.outputParticles
 
-        maskProt = self.newProtocol(ProtRelionCreateMask3D,
-                                    initialLowPassFilterA=10)  # filter at 10 A
-        vol = importProt.outputVolume
-        maskProt.inputVolume.set(vol)
-        print(magentaStr("\n==> Testing relion - create mask 3d:"))
-        self.launchProtocol(maskProt)
+        print(magentaStr("\n==> Testing relion - export particles:"))
 
-        self._validations(maskProt.outputMask, vol.getXDim(),
-                          vol.getSamplingRate(), maskProt)
+        def _checkProt(prot, stackType):
+            stackFiles = glob(prot._getExportPath('Particles', '*mrcs'))
+            print("stackFiles: ", stackFiles)
 
-        ih = ImageHandler()
-        img = ih.read(maskProt.outputMask)
-        mean, std, _min, _max = img.computeStats()
-        # Check the mask is non empty and between 0 and 1
-        self.assertAlmostEqual(_min, 0)
-        self.assertAlmostEqual(_max, 1)
-        self.assertTrue(mean > 0)
+            n = len(stackFiles)
+            if stackType == 0:
+                self.assertEqual(n, 0)
+            elif stackType == 1:
+                self.assertGreaterEqual(n, 1)
+            else:
+                self.assertEqual(n, 1)
 
+        stackTypes = [0, 1, 2]
+        stackNames = ['no', 'multi', 'single']
+        alignments = [True, False]
+        combinations = [(s, a) for s in stackTypes for a in alignments]
 
-class TestRelionSymmetrizeVolume(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('resmap')
+        for s, a in combinations:
+            label = 'export %s (stack: %s - align: %s)' % (name, stackNames[s], a)
+            exportProt = self.newProtocol(ProtRelionExportParticles,
+                                          inputParticles=inputParts,
+                                          objLabel=label,
+                                          stackType=s, alignmentType=a)
+            self.launchProtocol(exportProt)
+            _checkProt(exportProt, s)
 
-    def test_symmetrizeVolume(self):
-        print(magentaStr("\n==> Importing data - volume:"))
-        importVol = self.newProtocol(
-            ProtImportVolumes,
-            objLabel='import volume',
-            filesPath=self.ds.getFile('betaGal.mrc'),
-            samplingRate=3.54)
-
-        self.launchProtocol(importVol)
-
-        print(magentaStr("\n==> Testing relion - symmetrize volume:"))
-        symmVol = self.newProtocol(
-            ProtRelionSymmetrizeVolume,
-            objLabel='symmetryze d2',
-            inputVolume=importVol.outputVolume,
-            symmetryGroup='d2'
-        )
-        self.launchProtocol(symmVol)
+    def test_basic(self):
+        self.run_combinations(self.starImport)
 
-        self.assertIsNotNone(getattr(symmVol, 'outputVolumeAligned'))
-        self.assertIsNotNone(getattr(symmVol, 'outputVolumeSymmetrized'))
+    def test_extra(self):
+        self.run_combinations(self.protImport)
 
 
 class TestRelionExtractParticles(TestRelionBase):
-    """This class check if the protocol to extract particles
-    in Relion works properly.
-    """
-
-    @classmethod
-    def runImportMicrograph(cls, pattern, samplingRate, voltage,
-                            scannedPixelSize, magnification,
-                            sphericalAberration):
-        """ Run an Import micrograph protocol. """
-
-        # We have two options:
-        # 1) pass the SamplingRate or
-        # 2) the ScannedPixelSize + microscope magnification
-        if samplingRate is not None:
-            cls.protImport = cls.newProtocol(ProtImportMicrographs,
-                                             samplingRateMode=0,
-                                             filesPath=pattern,
-                                             samplingRate=samplingRate,
-                                             magnification=magnification,
-                                             voltage=voltage,
-                                             sphericalAberration=sphericalAberration)
-        else:
-            cls.protImport = cls.newProtocol(ProtImportMicrographs,
-                                             samplingRateMode=1,
-                                             filesPath=pattern,
-                                             scannedPixelSize=scannedPixelSize,
-                                             voltage=voltage,
-                                             magnification=magnification,
-                                             sphericalAberration=sphericalAberration)
-
-        cls.protImport.setObjLabel('import mics')
-        cls.launchProtocol(cls.protImport)
-        cls.assertIsNotNone(cls.protImport.outputMicrographs,
-                            "SetOfMicrographs has not been produced.")
-
-        return cls.protImport
-
-    @classmethod
-    def runImportMicrographBPV(cls, pattern):
-        """ Run an Import micrograph protocol. """
-        print(magentaStr("\n==> Importing data - micrographs:"))
-        return cls.runImportMicrograph(pattern, samplingRate=1.237,
-                                       voltage=300, sphericalAberration=2,
-                                       scannedPixelSize=None, magnification=56000)
-
     @classmethod
     def runDownsamplingMicrographs(cls, mics, downFactorValue, threads=1):
         # test downsampling a set of micrographs
         XmippProtPreprocessMicrographs = Domain.importFromPlugin(
             'xmipp3.protocols', 'XmippProtPreprocessMicrographs')
 
         if XmippProtPreprocessMicrographs is None:
@@ -961,61 +362,59 @@
                                                       downFactor=downFactorValue,
                                                       numberOfThreads=threads)
         cls.protDown.inputMicrographs.set(mics)
         cls.proj.launchProtocol(cls.protDown, wait=True)
         return cls.protDown
 
     @classmethod
-    def runFakedPicking(cls, mics, pattern):
-        """ Run a faked particle picking. Coordinates already existing. """
+    def runFakePicking(cls, mics, pattern):
+        """ Run a fake particle picking. Coordinates already exist. """
 
         # TODO This fake picking depends on Xmipp particle picking
         # TODO: Can we change this to an import coordinates?
 
         XmippProtParticlePicking = Domain.importFromPlugin(
             'xmipp3.protocols', 'XmippProtParticlePicking')
 
         if XmippProtParticlePicking is None:
             print("WARNING: Can not load xmipp3.protocols.XmippProtParticlePicking."
-                  "Skipping the tests.")
+                  "Skipping the test.")
             return None
 
         print(magentaStr("\n==> Running xmipp - fake particle picking:"))
         cls.protPP = XmippProtParticlePicking(importFolder=pattern, runMode=1)
         cls.protPP.inputMicrographs.set(mics)
         cls.proj.launchProtocol(cls.protPP, wait=True)
-        # check that faked picking has run ok
+        # check that fake picking has run ok
         cls.assertIsNotNone(cls.protPP.outputCoordinates,
                             "SetOfCoordinates has not been produced.")
 
         return cls.protPP
 
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.dataset = DataSet.getDataSet('xmipp_tutorial')
         cls.micFn = cls.dataset.getFile('mic1')
         cls.micsFn = cls.dataset.getFile('allMics')
         cls.coordsDir = cls.dataset.getFile('posSupervisedDir')
         cls.allCrdsDir = cls.dataset.getFile('posAllDir')
-
-        cls.DOWNSAMPLING = 5.0
-        cls.protImport = cls.runImportMicrographBPV(cls.micsFn)
+        cls.protImport = cls.runImportMics(cls.micsFn, 1.237)
         cls.protDown = cls.runDownsamplingMicrographs(cls.protImport.outputMicrographs,
-                                                      cls.DOWNSAMPLING)
+                                                      downFactorValue=5.0)
 
         print(magentaStr("\n==> Importing data - ctfs:"))
         cls.protCTF = cls.newProtocol(ProtImportCTF,
                                       importFrom=ProtImportCTF.IMPORT_FROM_XMIPP3,
                                       filesPath=cls.dataset.getFile('ctfsDir'),
                                       filesPattern='*.ctfparam')
         cls.protCTF.inputMicrographs.set(cls.protImport.outputMicrographs)
         cls.proj.launchProtocol(cls.protCTF, wait=True)
 
-        cls.protPP = cls.runFakedPicking(cls.protDown.outputMicrographs, cls.allCrdsDir)
+        cls.protPP = cls.runFakePicking(cls.protDown.outputMicrographs, cls.allCrdsDir)
 
     def _checkSamplingConsistency(self, outputSet):
         """ Check that the set sampling is the same as item sampling. """
         first = outputSet.getFirstItem()
 
         self.assertAlmostEqual(outputSet.getSamplingRate(),
                                first.getSamplingRate())
@@ -1183,248 +582,292 @@
 
         self.assertIsNotNone(outputParts,
                              "There was a problem generating the output.")
         self.assertTrue(outputParts.hasCTF(), "Output does not have CTF.")
         self._checkSamplingConsistency(outputParts)
 
 
-class TestRelionCenterAverages(TestRelionBase):
+class TestRelionImportCoords(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('mda')
-
-    def test_basic(self):
-        """ Run an Import averages protocol. """
-        print(magentaStr("\n==> Importing data - averages:"))
-        protImport = self.newProtocol(ProtImportAverages,
-                                      filesPath=self.ds.getFile('averages/averages.stk'),
-                                      samplingRate=5.04)
-        self.launchProtocol(protImport)
-        inputAvgs = protImport.outputAverages
-        print(magentaStr("\n==> Testing relion - center averages:"))
-        protCenter = self.newProtocol(ProtRelionCenterAverages)
-        protCenter.inputAverages.set(inputAvgs)
-        self.launchProtocol(protCenter)
+        cls.ds = DataSet.getDataSet('relion31_tutorial_precalculated')
+        cls.mics = cls.ds.getFile('MotionCorr/job002/Movies/*frameImage.mrc')
+        cls.parts = cls.ds.getFile('Refine3D/job029/run_it018_data.star')
+        cls.protImportMics = cls.runImportMics(cls.mics, 0.885)
 
-        conditions = ['outputAverages.getSize()==%d' % inputAvgs.getSize(),
-                      'outputAverages.getSamplingRate() - %0.5f < 0.00001'
-                      % inputAvgs.getSamplingRate()]
-        self.checkOutput(protCenter, 'outputAverages', conditions)
+    def testImportCoords(self):
+        """ Run an Import coords protocol. """
+        print(magentaStr("\n==> Importing coordinates (from star file):"))
+        self.protImport = self.newProtocol(ProtRelionImportCoords,
+                                           filePath=self.parts,
+                                           boxSize=128)
+        self.protImport.inputMicrographs.set(self.protImportMics.outputMicrographs)
+        self.launchProtocol(self.protImport)
+        self.assertIsNotNone(self.protImport.outputCoordinates,
+                             "SetOfCoordinates has not been produced.")
+        self.assertEqual(self.protImport.outputCoordinates.getSize(),
+                         4501, "Output size is not 4501!")
 
 
-class TestRelionExportParticles(TestRelionBase):
+class TestRelionImportParticles(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('relion_tutorial')
-        cls.ds2 = DataSet.getDataSet('xmipp_tutorial')
-        cls.particlesFn = cls.ds.getFile('import/refine3d/extra/relion_data.star')
-        cls.particlesFn2 = cls.ds2.getFile('particles')
-        cls.starImport = cls.runImportParticlesStar(cls.particlesFn, 10000, 7.08)
-        cls.runImportParticles(cls.particlesFn2, 1.237, True)
-
-    @classmethod
-    def runImportParticles(cls, pattern, samplingRate, checkStack=False,
-                           phaseFlip=False):
-        """ Run an Import particles protocol. """
-        print(magentaStr("\n==> Importing data - particles (from xmipp):"))
-        cls.protImport = cls.newProtocol(ProtImportParticles,
-                                         filesPath=pattern,
-                                         samplingRate=samplingRate,
-                                         checkStack=checkStack,
-                                         haveDataBeenPhaseFlipped=phaseFlip)
-        cls.launchProtocol(cls.protImport)
-        cls.assertIsNotNone(cls.protImport.outputParticles,
-                            "SetOfParticles has not been produced.")
+        cls.ds = DataSet.getDataSet('relion31_tutorial_precalculated')
 
-        return cls.protImport
-
-    def run_combinations(self, inputProt, name=''):
-        """ Run an Import particles protocol. """
-        inputParts = inputProt.outputParticles
+    def checkOutput(self, prot, outputName, conditions=[]):
+        """ Check that an ouput was generated and
+        the condition is valid.
+        """
+        o = getattr(prot, outputName, None)
+        locals()[outputName] = o
+        self.assertIsNotNone(o, "Output: %s is None" % outputName)
+        for cond in conditions:
+            self.assertTrue(eval(cond), 'Condition failed: ' + cond)
 
-        print(magentaStr("\n==> Testing relion - export particles:"))
+    def test_fromExtract(self):
+        """ Import particles.star from Extract job. """
+        starFile = self.ds.getFile('Extract/job018/particles.star')
+        optics = OpticsGroups.fromStar(starFile).first()
+        prot1 = self.runImportParticlesStar(starFile, samplingRate=optics.rlnImagePixelSize,
+                                            label="from relion (extract job)")
 
-        def _checkProt(prot, stackType):
-            stackFiles = glob(prot._getExportPath('Particles', '*mrcs'))
-            print("stackFiles: ", stackFiles)
+        self.checkOutput(prot1, 'outputParticles', [])
 
-            n = len(stackFiles)
-            if stackType == 0:
-                self.assertEqual(n, 0)
-            elif stackType == 1:
-                self.assertGreaterEqual(n, 1)
-            else:
-                self.assertEqual(n, 1)
-
-        stackTypes = [0, 1, 2]
-        stackNames = ['no', 'multi', 'single']
-        alignments = [True, False]
-        combinations = [(s, a) for s in stackTypes for a in alignments]
-
-        for s, a in combinations:
-            label = 'export %s (stack: %s - align: %s)' % (name, stackNames[s], a)
-            exportProt = self.newProtocol(ProtRelionExportParticles,
-                                          inputParticles=inputParts,
-                                          objLabel=label,
-                                          stackType=s, alignmentType=a)
-            self.launchProtocol(exportProt)
-            _checkProt(exportProt, s)
-
-    def test_basic(self):
-        self.run_combinations(self.starImport)
-
-    def test_extra(self):
-        self.run_combinations(self.protImport)
+    def test_fromClassify2D(self):
+        """ Import particles from Classify 2d job star file.
+        """
+        starFile = self.ds.getFile('Class2D/job013/run_it025_data.star')
+        optics = OpticsGroups.fromStar(starFile).first()
+        prot1 = self.runImportParticlesStar(starFile, samplingRate=optics.rlnImagePixelSize,
+                                            label="from relion (classify 2d)")
+
+        self.checkOutput(prot1, 'outputParticles', ['outputParticles.hasAlignment2D()'])
+        self.checkOutput(prot1, 'outputClasses')
+
+    def test_fromRefine3D(self):
+        """ Import particles from Refine3D job star file. """
+        starFile = self.ds.getFile('Refine3D/job019/run_it020_data.star')
+        optics = OpticsGroups.fromStar(starFile).first()
+        prot1 = self.runImportParticlesStar(starFile, samplingRate=optics.rlnImagePixelSize,
+                                            label="from relion (refine 3d)")
+
+        self.checkOutput(prot1, 'outputParticles', ['outputParticles.hasAlignmentProj()'])
+
+    def test_fromClassify3D(self):
+        """ Import particles from Classify3D job star file. """
+        starFile = self.ds.getFile('Class3D/job016/run_it025_data.star')
+        optics = OpticsGroups.fromStar(starFile).first()
+        prot1 = self.runImportParticlesStar(starFile, samplingRate=optics.rlnImagePixelSize,
+                                            label="from relion (classify 3d)")
+
+        self.checkOutput(prot1, 'outputParticles', ['outputParticles.hasAlignmentProj()'])
+        self.checkOutput(prot1, 'outputClasses')
+
+
+class TestRelionMotioncor(TestRelionBase):
+    @classmethod
+    def setUpClass(cls):
+        setupTestProject(cls)
+        cls.ds = DataSet.getDataSet('relion30_tutorial')
+        cls.protImport = cls.runImportMovies(filesPath=cls.ds.getFile('Movies/'),
+                                             filesPattern='20170629_000?5*tiff',
+                                             samplingRate=0.885,
+                                             voltage=200,
+                                             sphericalAberration=1.4,
+                                             dose=1.277,
+                                             gain=cls.ds.getFile("Movies/gain.mrc"))
+
+    def _runRelionMc(self, protImport, **kwargs):
+        protInput = protImport
+
+        args = {
+            'objLabel': 'relion - motioncor',
+            'patchX': 5,
+            'patchY': 5,
+            'numberOfThreads': CPUS
+        }
+        args.update(kwargs)
+        protRelionMc = self.newProtocol(ProtRelionMotioncor, **args)
+        protRelionMc.inputMovies.set(protInput.outputMovies)
+        protRelionMc = self.launchProtocol(protRelionMc)
+
+        return protRelionMc
+
+    def _checkOutputMovies(self, prot, size, exists=True,
+                           hasAlignment=True):
+        movies = getattr(prot, 'outputMovies', None)
+        self.assertIsNotNone(movies, "No movies were generated")
+        self.assertEqual(size, movies.getSize())
+
+        if hasAlignment:
+            self.assertTrue(movies.getFirstItem().hasAlignment())
+
+        if exists:
+            for m in movies:
+                self.assertTrue(os.path.exists(m.getFileName()))
+
+    def test_1x1(self):
+        print(magentaStr("\n==> Testing relion - motioncor (global):"))
+        protRelionMc = self._runRelionMc(self.protImport, objLabel='relion - mc 1x1',
+                                         patchX=1, patchY=1)
+        self._checkOutputMovies(protRelionMc, 3)
+
+    def test_1x1_PS(self):
+        print(magentaStr("\n==> Testing relion - motioncor (global + PS):"))
+        protRelionMc = self._runRelionMc(self.protImport, objLabel='relion - mc PS',
+                                         patchX=1, patchY=1,
+                                         savePSsum=True)
+        self._checkOutputMovies(protRelionMc, 3)
+
+    def test_3x3_DW(self):
+        print(magentaStr("\n==> Testing relion - motioncor (local + DW):"))
+        protRelionMc = self._runRelionMc(self.protImport, objLabel='relion - mc 3x3 DW',
+                                         patchX=3, patchY=3, doDW=True)
+        self._checkOutputMovies(protRelionMc, 3)
 
 
-class TestRelionExportCtf(TestRelionBase):
+class TestRelionPicking(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.dsXmipp = DataSet.getDataSet('xmipp_tutorial')
-        cls.dsGrigorieff = DataSet.getDataSet('grigorieff')
-        cls.dsEman2 = DataSet.getDataSet('eman')
-
-        print(magentaStr("\n==> Importing data - micrographs:"))
-        cls.protImport = cls.newProtocol(ProtImportMicrographs,
-                                         filesPath=cls.dsXmipp.getFile('allMics'),
-                                         samplingRate=1.237, voltage=300)
-        cls.launchProtocol(cls.protImport)
-
-    def runImportXmipp(self):
-        print(magentaStr("\n==> Importing data - ctfs (from xmipp)"))
-        protCTF = self.newProtocol(ProtImportCTF,
-                                   importFrom=ProtImportCTF.IMPORT_FROM_XMIPP3,
-                                   filesPath=self.dsXmipp.getFile('ctfsDir'),
-                                   filesPattern='*.ctfparam')
-        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
-        protCTF.setObjLabel('import ctfs from xmipp ')
-        self.launchProtocol(protCTF)
+        cls.ds = DataSet.getDataSet('relion_tutorial')
+        cls.partFn = cls.ds.getFile('import/classify2d/extra/relion_it015_data.star')
+        cls.protImportMics = cls.runImportMics('%s/*.mrc' % cls.ds.getFile('micrographs'),
+                                               samplingRate=7.08)
 
-        self.assertIsNotNone(protCTF.outputCTF,
-                             "There was a problem when importing ctfs.")
-        return protCTF
+    def _checkOutput(self, pickProt, minCoords, maxCoords):
+        """ Check that the outputCoordinates is not None
+         and that it should be between 300 and 400 coordinates
+         per micrograph.
+        """
+        coordSet = getattr(pickProt, 'outputCoordinates', None)
+        self.assertIsNotNone(coordSet)
+        for micAgg in coordSet.aggregate(["count"], "_micId", ["_micId"]):
+            self.assertGreaterEqual(micAgg['count'], minCoords)
+            self.assertLessEqual(micAgg['count'], maxCoords)
 
-    def runImportCtffind4(self):
-        print(magentaStr("\n==> Importing data - ctfs (from ctffind)"))
-        protCTF = self.newProtocol(ProtImportCTF,
-                                   importFrom=ProtImportCTF.IMPORT_FROM_GRIGORIEFF,
-                                   filesPath=self.dsGrigorieff.getFile('ctffind4'),
-                                   filesPattern='BPV*/*txt')
-        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
-        protCTF.setObjLabel('import from ctffind4')
-        self.launchProtocol(protCTF)
+    def testPickingLog(self):
+        print(magentaStr("\n==> Testing relion - autopick LoG:"))
+        protPickLog = self.newProtocol(
+            ProtRelionAutopickLoG,
+            objLabel='autopick LoG',
+            inputMicrographs=self.protImportMics.outputMicrographs,
+            boxSize=64,
+            minDiameter=260,
+            maxDiameter=360,
+            streamingBatchSize=5
+        )
+        self.launchProtocol(protPickLog)
+        self._checkOutput(protPickLog, 300, 400)
 
-        self.assertIsNotNone(protCTF.outputCTF,
-                             "There was a problem when importing ctfs.")
-        return protCTF
+    def testPickingRef(self):
+        # Create a subset with a few good averages
+        ih = ImageHandler()
+        avgsFn = self.ds.getFile('import/classify2d/extra/'
+                                 'relion_it015_classes.mrcs')
+        outAvgsFn = os.path.abspath(self.proj.getTmpPath('averages.mrcs'))
 
-    def runImportScipion(self):
-        print(magentaStr("\n==> Importing data - ctfs (from scipion)"))
-        ctfSqlite = self.dsGrigorieff.getFile('ctffind3/ctfs.sqlite')
+        for i, index in enumerate([5, 16, 17, 18, 31]):
+            ih.convert((index, avgsFn), (i + 1, outAvgsFn))
 
-        protCTF = self.newProtocol(ProtImportCTF,
-                                   objLabel='import from scipion',
-                                   importFrom=ProtImportCTF.IMPORT_FROM_SCIPION,
-                                   filesPath=ctfSqlite)
+        print(magentaStr("\n==> Importing data - averages:"))
+        protAvg = self.newProtocol(ProtImportAverages,
+                                   importFrom=ProtImportParticles.IMPORT_FROM_FILES,
+                                   filesPath=outAvgsFn,
+                                   samplingRate=7.08
+                                   )
+        self.launchProtocol(protAvg)
 
-        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
-        self.launchProtocol(protCTF)
+        # We need CTF estimation for picking ref with Relion
+        # Now estimate CTF on the micrographs with ctffind
+        ProtCTFFind = Domain.importFromPlugin(
+            'cistem.protocols', 'CistemProtCTFFind', doRaise=True)
 
-        self.assertIsNotNone(protCTF.outputCTF,
-                             "There was a problem when importing ctfs.")
-        return protCTF
+        print(magentaStr("\n==> Running cistem - ctffind:"))
+        protCtf = self.newProtocol(
+            ProtCTFFind,
+            inputMicrographs=self.protImportMics.outputMicrographs,
+            minDefocus=12000, maxDefocus=30000,
+            slowSearch=False,
+            resamplePix=False
+        )
+        self.launchProtocol(protCtf)
 
-    def runImportEman2(self):
-        print(magentaStr("\n==> Importing data - ctfs (from eman2)"))
-        protCTF = self.newProtocol(ProtImportCTF,
-                                   importFrom=ProtImportCTF.IMPORT_FROM_EMAN2,
-                                   filesPath=self.dsEman2.getFile('ctfs'),
-                                   filesPattern='BPV*json')
-        protCTF.inputMicrographs.set(self.protImport.outputMicrographs)
-        protCTF.setObjLabel('import from eman2')
-        self.launchProtocol(protCTF)
+        print(magentaStr("\n==> Testing relion - autopick ref:"))
+        protPickRef = self.newProtocol(
+            ProtRelion2Autopick,
+            inputMicrographs=self.protImportMics.outputMicrographs,
+            ctfRelations=protCtf.outputCTF,
+            inputReferences=protAvg.outputAverages,
+            streamingBatchSize=5
+        )
+        self.launchProtocol(protPickRef)
+        self._checkOutput(protPickRef, 320, 370)
 
-        self.assertIsNotNone(protCTF.outputCTF,
-                             "There was a problem when importing ctfs.")
-        return protCTF
 
-    def testExportCtf(self):
-        ctfs = [(self.runImportXmipp().outputCTF, 'xmipp'),
-                (self.runImportCtffind4().outputCTF, 'ctffind'),
-                (self.runImportScipion().outputCTF, 'scipion'),
-                (self.runImportEman2().outputCTF, 'eman2')]
+class TestRelionPreprocess(TestRelionBase):
+    """ This class helps to test all different preprocessing particles options
+    on Relion. """
+    @classmethod
+    def setUpClass(cls):
+        setupTestProject(cls)
+        TestRelionBase.setData('mda')
+        cls.protImport = cls.runImportParticles(cls.particlesFn, 3.5)
 
-        for i in ctfs:
-            protExport = self.newProtocol(ProtRelionExportCtf)
-            protExport.inputCTF.set(i[0])
-            print(magentaStr("\n==> Testing relion - export ctf (from %s)" % i[1]))
-            self.launchProtocol(protExport)
+    def _validations(self, imgSet, dims, pxSize):
+        self.assertIsNotNone(imgSet, "There was a problem with preprocess "
+                                     "particles")
+        xDim = imgSet.getXDim()
+        sr = imgSet.getSamplingRate()
+        self.assertEqual(xDim, dims, "The dimension of your particles are %d x "
+                                     "%d and must be  %d x %d" % (xDim, xDim,
+                                                                  dims, dims))
+        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
+                               msg="Pixel size of your particles are  %0.5f and"
+                                   " must be %0.5f" % (sr, pxSize))
 
-            outFn = os.path.exists(protExport._getStarFile()) or None
-            self.assertIsNotNone(outFn,
-                                 "There was a problem when exporting ctfs.")
+    def test_NormalizeAndDust(self):
+        print(magentaStr("\n==> Testing relion - preprocess particles (norm, remove dust):"))
+        protocol = self.newProtocol(ProtRelionPreprocessParticles,
+                                    doNormalize=True, backRadius=40,
+                                    doRemoveDust=True, whiteDust=4, blackDust=8)
+        protocol.setObjLabel('relion: norm-dust')
+        protocol.inputParticles.set(self.protImport.outputParticles)
+        self.launchProtocol(protocol)
+        
+        self._validations(protocol.outputParticles, 100, 3.5)
+        
+    def test_ScaleAndInvert(self):
+        print(magentaStr("\n==> Testing relion - preprocess particles (scale, invert):"))
+        protocol = self.newProtocol(ProtRelionPreprocessParticles,
+                                    doNormalize=False,
+                                    doScale=True, scaleSize=50,
+                                    doInvert=True)
+        protocol.setObjLabel('relion: scale-invert')
+        protocol.inputParticles.set(self.protImport.outputParticles)
+        
+        self.launchProtocol(protocol)
+        self._validations(protocol.outputParticles, 50, 7.0)
 
 
 class TestRelionRemovePrefViews(TestRelionBase):
     @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
         cls.ds = DataSet.getDataSet('relion_tutorial')
         cls.particlesFn = cls.ds.getFile('import/refine3d/extra/relion_data.star')
-        cls.starImport = cls.runImportParticlesStar(cls.particlesFn, 10000, 7.08)
+        cls.starImport = cls.runImportParticlesStar(cls.particlesFn, 7.08)
 
     def test_removePrefViews(self):
         print(magentaStr("\n==> Testing relion - remove preferential views"))
         inputParts = self.starImport.outputParticles
         prot = self.newProtocol(ProtRelionRemovePrefViews,
                                 inputParticles=inputParts,
                                 numToRemove=50)
         self.launchProtocol(prot)
 
         self.assertIsNotNone(prot.outputParticles,
                              "There was a problem with remove preferential views protocol.")
         outSize = prot.outputParticles.getSize()
         self.assertEqual(outSize, 4080, "Output size is not 4080!")
-
-
-class TestRelionResizeVolume(TestRelionBase):
-    @classmethod
-    def setUpClass(cls):
-        setupTestProject(cls)
-        cls.ds = DataSet.getDataSet('relion_tutorial')
-
-    def importVolume(self):
-        print(magentaStr("\n==> Importing data - volume:"))
-        volFn = self.ds.getFile('import/refine3d/extra/relion_class001.mrc')
-        protVol = self.newProtocol(ProtImportVolumes,
-                                   objLabel='import volume',
-                                   filesPath=volFn,
-                                   samplingRate=3)
-        self.launchProtocol(protVol)
-        return protVol
-
-    def _validations(self, vol, dims, pxSize):
-        self.assertIsNotNone(vol, "There was a problem with crop/resize "
-                                  "volumes protocol")
-        xDim = vol.getXDim()
-        sr = vol.getSamplingRate()
-        self.assertEqual(xDim, dims, "The dimension of your volume is (%d)^3 "
-                                     "and must be (%d)^3" % (xDim, dims))
-
-        self.assertAlmostEqual(sr, pxSize, delta=0.0001,
-                               msg="Pixel size of your volume is %0.5f and"
-                               " must be %0.5f" % (sr, pxSize))
-
-    def test_resizeVol(self):
-        importProt = self.importVolume()
-        resizeProt = self.newProtocol(ProtRelionResizeVolume,
-                                      doRescale=True, rescaleSamplingRate=1.5,
-                                      doResize=True, resizeSize=128)
-        vol = importProt.outputVolume
-        resizeProt.inputVolumes.set(vol)
-        print(magentaStr("\n==> Testing relion - crop/resize volumes:"))
-        self.launchProtocol(resizeProt)
-
-        self._validations(resizeProt.outputVol, 128, 1.5)
```

### Comparing `scipion-em-relion-4.0b8/relion/tests/test_workflow_relion3.py` & `scipion-em-relion-5.0.0b1/relion/tests/test_workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from ..protocols import *
 
 
 CPUS = os.environ.get('SCIPION_TEST_CPUS', 4)
 GPUS = os.environ.get('SCIPION_TEST_GPUS', 2)
 
 
-class TestWorkflowRelion3Betagal(TestWorkflow):
+class TestWorkflowRelionBetagal(TestWorkflow):
     @classmethod
     def setUpClass(cls):
         pwtests.setupTestProject(cls)
         cls.ds = pwtests.DataSet.getDataSet('relion30_tutorial')
 
     def _importMovies(self):
         print(magentaStr("\n==> Importing data - movies:"))
@@ -83,31 +83,31 @@
         return self.launchProtocol(protAssign)
 
     def _runRelionMc(self, protImport):
         print(magentaStr("\n==> Testing relion - motioncor:"))
         protRelionMc = self.newProtocol(
             ProtRelionMotioncor,
             objLabel='relion - motioncor',
-            patchX=5, patchY=5,
-            numberOfThreads=CPUS)
+            patchX=1, patchY=1,
+            numberOfMpi=CPUS//2)
 
         protRelionMc.inputMovies.set(protImport.outputMovies)
         protRelionMc = self.launchProtocol(protRelionMc)
 
         return protRelionMc
 
     def _runRelionLog(self, protRelionMc):
         print(magentaStr("\n==> Testing relion - autopick LoG:"))
         protRelionLog = self.newProtocol(
             ProtRelionAutopickLoG,
             objLabel='relion - autopick log',
-            boxSize=250,
+            boxSize=100,
             minDiameter=150, maxDiameter=180,
-            areParticlesWhite=False,
-            numberOfThreads=CPUS)
+            threshold2=5.0,
+            numberOfMpi=CPUS//2)
 
         protRelionLog.inputMicrographs.set(protRelionMc.outputMicrographsDoseWeighted)
         protRelionLog = self.launchProtocol(protRelionLog)
 
         return protRelionLog
 
     def _runGctf(self, protMc):
@@ -132,55 +132,59 @@
         print(magentaStr("\n==> Testing relion - extract particles:"))
         protRelionExtract = self.newProtocol(
             ProtRelionExtractParticles,
             objLabel='relion - extract',
             boxSize=256, doRescale=True, rescaledSize=64,
             doInvert=True, doNormalize=True,
             backDiameter=200,
-            numberOfMpi=CPUS/2,
-            downsamplingType=0,  # Micrographs same as picking
+            numberOfMpi=CPUS,
+            downsamplingType=0  # Micrographs same as picking
         )
 
         protRelionExtract.ctfRelations.set(protCtf.outputCTF)
         protRelionExtract.inputCoordinates.set(protPicking.outputCoordinates)
         protRelionExtract = self.launchProtocol(protRelionExtract)
 
         return protRelionExtract
 
     def _runRelion2D(self, protExtract):
         print(magentaStr("\n==> Testing relion - classify 2D:"))
         protRelion2D = self.newProtocol(
             ProtRelionClassify2D,
             objLabel='relion - 2d',
+            inplaneAngularSamplingDeg=11,
             maskDiameterA=200,
-            numberOfClasses=100,
+            numberOfClasses=20,
             extraParams='--maxsig 25',
             pooledParticles=30,
             doGpu=True,
-            numberOfThreads=8,
+            numberOfThreads=CPUS,
             numberOfMpi=1,
             allParticlesRam=True
         )
 
         protRelion2D.inputParticles.set(protExtract.outputParticles)
         return self.launchProtocol(protRelion2D)
 
-    def _runInitModel(self, protRelion2D):
+    def _runInitModel(self, protExtract):
         print(magentaStr("\n==> Testing relion - initial model:"))
         relionIniModel = self.newProtocol(ProtRelionInitialModel,
-                                          doCTF=False, doGpu=True,
+                                          doCTF=True, doGpu=True,
                                           maskDiameterA=200,
-                                          numberOfIterations=50,
-                                          symmetryGroup='d2',
-                                          numberOfMpi=1, numberOfThreads=8)
-        relionIniModel.inputParticles.set(protRelion2D.outputParticles)
+                                          numberOfIter=50,
+                                          symmetryGroup='D2',
+                                          pooledParticles=30,
+                                          numberOfThreads=CPUS)
+        relionIniModel.inputParticles.set(protExtract.outputParticles)
         protInitModel = self.launchProtocol(relionIniModel)
         return protInitModel
 
     def test_workflow(self):
         protImport = self._importMovies()
         protRelionMc = self._runRelionMc(protImport)
         protGctf = self._runGctf(protRelionMc)
         protRelionLog = self._runRelionLog(protRelionMc)
         protRelionExtract = self._runRelionExtract(protRelionLog, protGctf)
         protRelion2D = self._runRelion2D(protRelionExtract)
-        # protInitModel = self._runRelion2D(protRelion2D)
+        protInitModel = self._runInitModel(protRelionExtract)
+        self.assertIsNotNone(protRelion2D.outputClasses, protRelion2D.getErrorMessage())
+        self.assertIsNotNone(protInitModel.outputVolume, protInitModel.getErrorMessage())
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/__init__.py` & `scipion-em-relion-5.0.0b1/relion/viewers/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,12 +22,13 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
 
 from .viewer_base import *
 from .viewer_ctfrefine import ProtCtfRefineViewer
-from .viewer_postprocess import PostprocessViewer
+from .viewer_postprocess import PostprocessViewer, ProtFSCViewer
 from .viewer_motioncor import RelionMotioncorrViewer
 from .viewer_locres import RelionLocalResViewer
 from .viewer_polishing import RelionPolishViewer
 from .viewer_multibody import MultibodyViewer
+from .viewer_reconstruct import ReconstructViewer
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_base.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,27 +25,31 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
 
 import os
 from math import radians, log
 from emtable import Table
+import logging
+logger = logging.getLogger(__name__)
 
 import pyworkflow.protocol.params as params
 from pyworkflow.protocol.constants import LEVEL_ADVANCED
-from pyworkflow.viewer import (DESKTOP_TKINTER, WEB_DJANGO)
+from pyworkflow.viewer import (DESKTOP_TKINTER, WEB_DJANGO, Viewer)
+import pyworkflow.utils as pwutils
 from pwem.viewers import (EmPlotter, EmProtocolViewer, showj,
                           FscViewer, DataView, ObjectView, ChimeraView,
                           ClassesView, Classes3DView, ChimeraAngDist)
 from pwem.constants import ALIGN_PROJ, NO_INDEX
 from pwem.objects import FSC
 
 from relion.convert.convert_utils import relionToLocation
 from ..protocols import (ProtRelionClassify2D, ProtRelionClassify3D,
-                         ProtRelionRefine3D, ProtRelionInitialModel)
+                         ProtRelionRefine3D, ProtRelionInitialModel,
+                         ProtRelionSelectClasses2D)
 from ..constants import *
 
 
 class RelionPlotter(EmPlotter):
     """ Class to create several plots. """
 
     def __init__(self, x=1, y=1, mainTitle="", **kwargs):
@@ -192,18 +196,16 @@
                            expertLevel=LEVEL_ADVANCED,
                            condition='displayAngDist == %d' % ANGDIST_CHIMERA,
                            label='Spheres distance',
                            help='If the value is -1 then the distance is set '
                                 'to 0.75 * xVolDim')
 
             group = form.addGroup('Resolution')
-            group.addParam('figure', params.EnumParam, default=0,
-                           choices=['new', 'active'],
-                           label='Figure',
-                           display=params.EnumParam.DISPLAY_HLIST)
+            group.addHidden('figure', params.EnumParam, default=0,
+                            choices=['new', 'active'])
             group.addParam('resolutionPlotsSSNR', params.LabelParam,
                            default=True,
                            label='Display SSNR plots',
                            help='Display signal to noise ratio plots (SSNR)')
             if not self.protocol.IS_CLASSIFY and not self.protocol.IS_3D_INIT:
                 group.addParam('resolutionPlotsFSC', params.LabelParam,
                                default=True,
@@ -319,32 +321,30 @@
     @protected_show
     def _showImagesAngularAssignment(self, paramName=None):
         views = []
 
         for it in self._iterations:
             fn = self.protocol._getIterData(it, alignType=ALIGN_PROJ)
             if not os.path.exists(fn):
-                raise Exception("Missing data star file '%s'. \n"
-                                "Plese select a valid iteration. "
-                                % fn)
+                raise FileNotFoundError(f"Missing data star file '{fn}'.\n"
+                                        "Please select a valid iteration.")
             v = self.createScipionPartView(fn)
             views.append(v)
 
         return views
 
     @protected_show
     def _showOptimiserFile(self, paramName=None):
         views = []
 
         for it in self._iterations:
             optimiserFile = self.protocol._getFileName('optimiser', iter=it)
             if not os.path.exists(optimiserFile):
-                raise Exception("Missing optimiser file '%s'. \n"
-                                "Plese select a valid iteration. "
-                                % optimiserFile)
+                raise FileNotFoundError(f"Missing optimiser file '{optimiserFile}'.\n"
+                                        "Please select a valid iteration. ")
             v = self.createDataView(optimiserFile)
             views.append(v)
         return views
 
     # =============================================================================
     # showLLRelion
     # =============================================================================
@@ -391,16 +391,16 @@
     # =============================================================================
     # Get classes info per iteration
     # =============================================================================
     def _plotClassDistribution(self, paramName=None):
         labels = ["rlnClassDistribution", "rlnAccuracyRotations",
                   "rlnAccuracyTranslationsAngst"]
 
-        iterations = range(self.firstIter, self.lastIter + 1)
         classInfo = {}
+        iterations = self._getAllIters()
 
         for it in iterations:
             modelStar = self.protocol._getFileName('model', iter=it)
             table = Table(fileName=modelStar, tableName='model_classes')
             for row in table:
                 i, fn = relionToLocation(row.rlnReferenceImage)
                 if i == NO_INDEX:  # the case for 3D classes
@@ -469,22 +469,22 @@
     # =============================================================================
     # ShowChanges
     # =============================================================================
     def _showChanges(self, paramName=None):
         labels = ['rlnIterationNumber'] + self.protocol.CHANGE_LABELS
         tableChanges = Table(columns=labels)
 
-        print("Computing average changes in offset, angles, and class membership")
+        logger.info("Computing average changes in offset, angles, and class membership")
         for it in self._getAllIters():
             fn = self.protocol._getFileName('optimiser', iter=it)
             if not os.path.exists(fn):
                 continue
-            print("Computing data for iteration; %03d" % it)
+            logger.info(f"Computing data for iteration {it:03d}")
             fn = self.protocol._getFileName('optimiser', iter=it)
-            table = Table(fileName=fn, tableName='optimiser_general')
+            table = Table(fileName=fn, tableName='optimiser_general', types=LABELS_DICT)
             row = table[0]
             cols = [getattr(row, value) for value in self.protocol.CHANGE_LABELS]
             tableChanges.addRow(it, *cols)
 
         fn = self.protocol._getFileName('all_changes')
 
         with open(fn, 'w') as f:
@@ -506,35 +506,34 @@
         """ Write an sqlite with all volumes selected for visualization. """
         path = self.protocol._getExtraPath('relion_viewer_volumes.sqlite')
         samplingRate = self.protocol.inputParticles.get().getSamplingRate()
 
         files = []
         volumes = self._getVolumeNames()
         for volFn in volumes:
-            if not os.path.exists(volFn.replace(':mrc', '')):
-                raise Exception("Missing volume file: %s\n Please select "
-                                "a valid class or iteration number."
-                                % volFn)
-            print("Adding vol: %s" % volFn)
-            files.append(volFn)
+            if not os.path.exists(volFn):
+                raise FileNotFoundError(f"Missing volume file: {volFn}\n Please select "
+                                        "a valid class or iteration number.")
+            logger.debug(f"Adding vol: {volFn}")
+            if not volFn.endswith(":mrc"):
+                files.append(volFn + ":mrc")
 
         self.createVolumesSqlite(files, path, samplingRate)
         return [ObjectView(self._project, self.protocol.strId(), path)]
 
     def _showVolumesChimera(self):
         """ Create a chimera script to visualize selected volumes. """
         volumes = self._getVolumeNames()
         cmdFile = self.protocol._getExtraPath('chimera_volumes.cxc')
         with open(cmdFile, 'w+') as f:
             for vol in volumes:
-                # remove ":mrc" extension needed by xmipp
-                vol = vol.replace(":mrc", "")
                 # We assume that the chimera script will be generated
                 # at the same folder as relion volumes
                 localVol = os.path.basename(vol)
+                vol = vol.replace(":mrc", "")
                 if os.path.exists(vol):
                     f.write("open %s\n" % localVol)
             f.write('tile\n')
         view = ChimeraView(cmdFile)
         return [view]
 
     # =============================================================================
@@ -563,16 +562,16 @@
 
         if len(self._refsList) != 1:
             return self.infoMessage("Please select only one class to display "
                                     "angular distribution", "Input selection")
         # If just one reference we can show the angular distribution
         ref3d = self._refsList[0]
         volFn = self._getVolumeNames()[0]
-        if not os.path.exists(volFn.replace(":mrc", "")):
-            raise Exception("This class is empty. Please try with another class")
+        if not os.path.exists(volFn):
+            raise FileNotFoundError("This class is empty. Please try with another class")
 
         for prefix in prefixes:
             sqliteFn = self.protocol._getFileName('projections',
                                                   iter=it, ref3d=ref3d,
                                                   half=prefix)
             if not os.path.exists(sqliteFn):
                 mdOut = self._getMdOut(it, prefix, ref3d)
@@ -626,25 +625,20 @@
                 return plotter
             else:
                 return
 
     # =============================================================================
     # plotSSNR
     # =============================================================================
-
-    def _getFigure(self):
-        return None if self.figure == 0 else 'active'
-
     def _showSSNR(self, paramName=None):
         prefixes = self._getPrefixes()
         nrefs = len(self._refsList)
         n = nrefs * len(prefixes)
         gridsize = self._getGridSize(n)
-        xplotter = RelionPlotter(x=gridsize[0], y=gridsize[1],
-                                 figure=self._getFigure())
+        xplotter = RelionPlotter(x=gridsize[0], y=gridsize[1])
 
         for prefix in prefixes:
             for ref3d in self._refsList:
                 plot_title = 'Resolution SSNR %s, for Class %s' % (prefix, ref3d)
                 a = xplotter.createSubPlot(plot_title, 'Angstroms^-1', 'log(SSNR)')
                 blockName = 'model_class_%d' % ref3d
                 for it in self._iterations:
@@ -673,30 +667,30 @@
         a.plot(resolution_inv, frc, label=label)
         a.xaxis.set_major_formatter(self._plotFormatter)
 
     # =============================================================================
     # plotFSC
     # =============================================================================
     def _showFSC(self, paramName=None):
-        print("Showing FSC for iterations: ", self._iterations)
+        logger.info(f"Showing FSC for iterations: {self._iterations}")
         threshold = self.resolutionThresholdFSC.get()
 
         fscViewer = FscViewer(project=self.protocol.getProject(),
                               threshold=threshold,
+                              figure=None,
                               protocol=self.protocol,
-                              figure=self._getFigure(),
                               addButton=True)
         fscSet = self.protocol._createSetOfFSCs()
         for it in self._iterations:
             model_star = self._getModelStar('half1_', it)
             if os.path.exists(model_star):
                 fsc = self._plotFSC(None, model_star, 'iter %d' % it)
                 fscSet.append(fsc)
+
         fscViewer.visualize(fscSet)
-        return [fscViewer]
 
     def _plotFSC(self, a, model_star, label, legend=None):
         if legend is None:
             legend = label
         table = Table(fileName=model_star, tableName='model_class_1')
         resolution_inv = table.getColumnValues('rlnResolution')
         frc = table.getColumnValues('rlnGoldStandardFsc')
@@ -754,15 +748,15 @@
         :return: the list with the range of values, empty
         """
         value = var.get()
         if value is None or not value.strip():
             self._errors.append('Provide %s selection.' % label)
             result = []
         else:
-            result = self._getListFromRangeString(value)
+            result = pwutils.getListFromRangeString(value)
 
         return result
 
     def _hasClasses(self):
         p = self.protocol
         return p.IS_CLASSIFY or p.IS_3D_INIT
 
@@ -816,15 +810,15 @@
             n = len(self._refsList)
 
         if n == 1:
             gridsize = [1, 1]
         elif n == 2:
             gridsize = [2, 1]
         else:
-            gridsize = [(n + 1) / 2, 2]
+            gridsize = [(n + 1) // 2, 2]
 
         return gridsize
 
     def _getPrefixes(self):
         prefixes = self.protocol.PREFIXES
         halves = getattr(self, 'showHalves', None)
         if halves:
@@ -849,26 +843,26 @@
         if prefixes[0] == 'final' and self.protocol.IS_3D_INIT:
             prefixes = ['finalSGD']
         return prefixes
 
     def _getVolumeNames(self):
         vols = []
         prefixes = self._getVolumePrefixes()
-        print("self._iterations: ", self._iterations)
+        logger.debug(f"self._iterations: {self._iterations}")
         for it in self._iterations:
             for ref3d in self._refsList:
                 for prefix in prefixes:
                     volFn = self.protocol._getFileName(prefix + 'volume',
                                                        iter=it, ref3d=ref3d)
-                    if os.path.exists(volFn.replace(':mrc', '')):
+                    if os.path.exists(volFn):
+                        volFn = volFn.replace(":mrc", "")
                         vols.append(volFn)
                     else:
-                        raise Exception("Volume %s does not exists. \n"
-                                        "Please select a valid iteration "
-                                        "number. " % volFn)
+                        raise FileNotFoundError(f"Volume {volFn} does not exists.\n"
+                                                "Please select a valid iteration number.")
         return vols
 
     def _getMdOut(self, it, prefix, ref3d):
         randomSet = self._getRandomSet(prefix)
         dataStar = self._getDataStar(prefix, it)
         mdOut = []
 
@@ -904,7 +898,27 @@
             return 0
         elif prefix == "half1_":
             return 1
         elif prefix == "half2_":
             return 2
         else:
             return 3
+
+
+class RelionSelectClassesViewer(Viewer):
+    _targets = [ProtRelionSelectClasses2D]
+
+    def _visualize(self, obj, **kwargs):
+        labels = 'enabled id _size _representative._filename '
+        labels += '_rlnClassDistribution _rlnPredictedClassScore '
+        labels += '_rlnEstimatedResolution '
+        viewParams = {showj.ORDER: labels,
+                      showj.VISIBLE: labels,
+                      showj.RENDER: '_representative._filename',
+                      showj.SORT_BY: '_rlnPredictedClassScore desc',
+                      showj.MODE: showj.MODE_MD
+                      }
+        prot = self.protocol
+        output = prot.outputClasses
+        view = ClassesView(self.getProject(), prot.strId(), output.getFileName(),
+                           viewParams=viewParams)
+        return [view]
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_locres.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_locres.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,16 @@
         imageFile = self.getResolutionVolumeFileName()
         imgData, _, _, _ = self.getImgData(imageFile)
 
         xplotter = RelionPlotter(x=2, y=2, mainTitle="Local Resolution Slices "
                                                      "along %s-axis."
                                                      % self._getAxis())
         for i in range(4):
-            slice = self._getSlice(i + 1, imgData)
-            a = xplotter.createSubPlot("Slice %s" % slice, '', '')
+            sliceN = self._getSlice(i + 1, imgData)
+            a = xplotter.createSubPlot("Slice %s" % sliceN, '', '')
             matrix = self._getSliceImage(imgData, i + 1, self._getAxis())
             plot = xplotter.plotMatrix(a, matrix, self.lowest.get(), self.highest.get(),
                                        cmap=self._getColorName(),
                                        interpolation="nearest")
         xplotter.getColorBar(plot)
         return [xplotter]
 
@@ -121,15 +121,15 @@
     def _getAxis(self):
         return self.getEnumText('sliceAxis')
 
     def _getSlice(self, index, volumeData):
         return int((index + 3) * volumeData.shape[0] / 9)
 
     def _getSliceImage(self, volumeData, index, dataAxis):
-        slice = self._getSlice(index, volumeData)
+        sliceN = self._getSlice(index, volumeData)
         if dataAxis == 'y':
-            imgSlice = volumeData[:, slice, :]
+            imgSlice = volumeData[:, sliceN, :]
         elif dataAxis == 'x':
-            imgSlice = volumeData[:, :, slice]
+            imgSlice = volumeData[:, :, sliceN]
         else:
-            imgSlice = volumeData[slice, :, :]
+            imgSlice = volumeData[sliceN, :, :]
         return imgSlice
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_motioncor.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_motioncor.py`

 * *Files identical despite different names*

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_multibody.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_multibody.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
+import logging
+logger = logging.getLogger(__name__)
 
 from pyworkflow.protocol.constants import STATUS_FINISHED
 
 from .viewer_base import *
 from ..protocols import ProtRelionMultiBody
 
 
@@ -81,60 +83,65 @@
     def _getVisualizeDict(self):
         self._load()
         return {'displayVol': self._showVolumes,
                 'showMovie': self._showMovie
                 }
 
     def _createVolumesSqlite(self):
-        """ Write an sqlite with all volumes selected for visualization. """
+        """ Write a sqlite with all volumes selected for visualization. """
         path = self.protocol._getExtraPath('relion_viewer_volumes.sqlite')
-        samplingRate = self.protocol.protRefine.get()._getInputParticles().getSamplingRate()
+        if self.protocol.doContinue:
+            protRef = self.protocol.continueRun.get().protRefine.get()
+        else:
+            protRef = self.protocol.protRefine.get()
+
+        samplingRate = protRef._getInputParticles().getSamplingRate()
 
         files = []
         volumes = self._getVolumeNames()
         for volFn in volumes:
-            if not os.path.exists(volFn.replace(':mrc', '')):
-                raise Exception("Missing volume file: %s\n Please select "
-                                "a valid class or iteration number."
-                                % volFn)
-            print("Adding vol: %s" % volFn)
-            files.append(volFn)
+            if not os.path.exists(volFn):
+                raise FileNotFoundError(f"Missing volume file: {volFn}\n Please select "
+                                        "a valid class or iteration number.")
+            logger.debug(f"Adding vol: {volFn}")
+            if not volFn.endswith(":mrc"):
+                files.append(volFn + ":mrc")
 
         self.createVolumesSqlite(files, path, samplingRate)
         return [ObjectView(self._project, self.protocol.strId(), path)]
 
     def _getVolumeNames(self):
         vols = []
         prefixes = self._getVolumePrefixes()
         num = self.protocol._getNumberOfBodies()
-        print("self._iterations: ", self._iterations)
+        logger.debug(f"self._iterations: {self._iterations}")
         for it in self._iterations:
             for ref3d in range(1, num+1):
                 for prefix in prefixes:
                     volFn = self.protocol._getFileName(prefix + 'volume_mbody',
                                                        iter=it, ref3d=ref3d)
-                    if os.path.exists(volFn.replace(':mrc', '')):
+                    if os.path.exists(volFn):
+                        volFn = volFn.replace(":mrc", "")
                         vols.append(volFn)
                     else:
-                        raise Exception("Volume %s does not exists. \n"
-                                        "Please select a valid iteration "
-                                        "number." % volFn)
+                        raise FileNotFoundError(f"Volume {volFn} does not exists.\n"
+                                                "Please select a valid iteration number.")
         return vols
 
     @protected_show
     def _showMovie(self, paramName=None):
         """ Create a chimera script to visualize animation. """
         prot = self.protocol
         if prot.getStatus() != STATUS_FINISHED:
-            raise Exception("Protocol has not finished yet, results are not ready!")
+            raise ValueError("Protocol has not finished yet, results are not ready!")
 
         compToShow = self.component.get()
         totalComp = prot.numberOfEigenvectors.get()
         if compToShow > totalComp:
-            raise Exception("You only have %d components!" % totalComp)
+            raise ValueError("You only have %d components!" % totalComp)
 
         vols = "analyse_component%03d_bin*.mrc" % compToShow
         cmdFile = prot._getExtraPath('chimera_animation_comp%d.cxc' % compToShow)
 
         with open(cmdFile, 'w') as f:
             f.write("open %s vseries true\n" % vols)
             f.write('vseries play #1 loop true direction oscillate\n')
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_polishing.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_polishing.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 
             plotter = Plotter()
             figure = plotter.getFigure()
             a = figure.add_subplot(111)
             a.grid(True)
             a.set_xlabel('Movie frame number')
             a.set_ylabel(label)
-            a.invert_yaxis()
             a.plot(frame, list(bfactor))
             a.set_title(title)
             plotter.tightLayout()
 
             return [plotter]
 
     def _load(self):
```

### Comparing `scipion-em-relion-4.0b8/relion/viewers/viewer_postprocess.py` & `scipion-em-relion-5.0.0b1/relion/viewers/viewer_postprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,18 +20,19 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # ******************************************************************************
 
-from pyworkflow.viewer import ProtocolViewer
+import numpy as np
+from pyworkflow.viewer import ProtocolViewer, Viewer
 
 from .viewer_base import *
-from ..protocols import ProtRelionPostprocess
+from ..protocols import ProtRelionPostprocess, ProtRelionCalculateFSC
 
 
 class PostprocessViewer(ProtocolViewer):
     """ Visualization of Relion postprocess results. """
     _targets = [ProtRelionPostprocess]
     _environments = [DESKTOP_TKINTER]
 
@@ -59,19 +60,16 @@
         group.addParam('displayMaskedVol', params.EnumParam,
                        choices=['slices', 'chimera'],
                        display=params.EnumParam.DISPLAY_HLIST,
                        default=VOLUME_SLICES,
                        label='Display masked volume with',
                        help='*slices*: display masked volume as 2D slices along z axis.\n'
                             '*chimera*: display masked volume as surface with Chimera.')
-        group.addParam('figure', params.EnumParam, default=0,
-                       choices=['new', 'active'],
-                       label='Figure',
-                       display=params.EnumParam.DISPLAY_HLIST,
-                       help="Plot in a new window vs the last opened one")
+        group.addHidden('figure', params.EnumParam, default=0,
+                        choices=['new', 'active'])
         group.addParam('resolutionPlotsFSC', params.EnumParam,
                        choices=['Corrected', 'Unmasked Maps', 'Masked Maps',
                                 'Phase Randomized Masked Maps', 'all'],
                        default=FSC_ALL,
                        display=params.EnumParam.DISPLAY_COMBO,
                        label='Display resolution plots (FSC)')
         group.addParam('resolutionThresholdFSC',
@@ -110,55 +108,52 @@
 
     def _showVolumesChimera(self, volPath):
         """ Create a chimera script to visualize selected volumes. """
         view = ChimeraView(volPath)
         return [view]
 
     def _showVolume(self, paramName=None):
-        volPath = self.protocol._getExtraPath('postprocess.mrc:mrc')
+        volPath = self.protocol._getExtraPath('postprocess.mrc')
 
         if self.displayVol == VOLUME_CHIMERA:
             return self._showVolumesChimera(volPath)
 
         elif self.displayVol == VOLUME_SLICES:
             return self._showVolumeShowj(volPath)
 
     def _showMaskedVolume(self, paramName=None):
-        volPath = self.protocol._getExtraPath('postprocess_masked.mrc:mrc')
+        volPath = self.protocol._getExtraPath('postprocess_masked.mrc')
 
         if self.displayMaskedVol == VOLUME_CHIMERA:
             return self._showVolumesChimera(volPath)
 
         elif self.displayMaskedVol == VOLUME_SLICES:
             return self._showVolumeShowj(volPath)
 
     # =========================================================================
     # plotFSC
     # =========================================================================
-    def _getFigure(self):
-        return None if self.figure == 0 else 'active'
-
     def _showFSC(self, paramName=None):
         threshold = self.resolutionThresholdFSC.get()
 
         fscViewer = FscViewer(project=self.protocol.getProject(),
                               threshold=threshold,
                               protocol=self.protocol,
-                              figure=self._getFigure(),
+                              figure=None,
                               addButton=True)
         fscSet = self.protocol._createSetOfFSCs()
 
         modelStar = self.protocol._getExtraPath('postprocess.star')
         for label in self._getFSCLabels():
             if os.path.exists(modelStar):
                 legend = self._getLegend(label)
                 fsc = self._plotFSC(None, modelStar, label, legend)
                 fscSet.append(fsc)
+
         fscViewer.visualize(fscSet)
-        return [fscViewer]
 
     # ROB this function is duplicated
     def _plotFSC(self, a, model_star, label, legend=None):
         if legend is None:
             legend = label
         table = Table(fileName=model_star, tableName='fsc')
         resolution_inv = table.getColumnValues('rlnResolution')
@@ -184,20 +179,21 @@
         xplotter.showLegend(legends)
         a.grid(True)
 
         return [xplotter]
 
     def _plotGuinier(self, a, model, label):
         table = Table(fileName=model, tableName='guinier')
-        resolSqInv = table.getColumnValues('rlnResolutionSquared')
-        logAmp = table.getColumnValues(label)
+        resolSqInv = np.array(table.getColumnValues('rlnResolutionSquared'))
+        logAmp = np.array(table.getColumnValues(label))
 
-        self.maxfsc = max(logAmp)
-        self.minInv = min(resolSqInv)
-        self.maxInv = max(resolSqInv)
+        # remove values < -99.0
+        mask = logAmp > -99.0
+        logAmp = logAmp[mask]
+        resolSqInv = resolSqInv[mask]
 
         a.plot(resolSqInv, logAmp)
         a.xaxis.set_major_formatter(self._plotFormatter)
 
     # =========================================================================
     # Utils Functions
     # =========================================================================
@@ -249,7 +245,30 @@
             return 'log(Amplitudes) Original'
         elif label == 'rlnLogAmplitudesWeighted':
             return 'log(Amplitudes) Weighted'
         elif label == 'rlnLogAmplitudesSharpened':
             return 'log(Amplitudes) Sharpened'
         else:
             return 'log(Amplitudes) Intercept'
+
+
+class ProtFSCViewer(Viewer):
+    """ Modified FSC viewer to pass the threshold param. """
+    _environments = [DESKTOP_TKINTER]
+    _label = 'fsc viewer'
+    _targets = [ProtRelionCalculateFSC]
+
+    def __init__(self, **args):
+        Viewer.__init__(self, **args)
+
+    def _visualize(self, obj, **kwargs):
+        thr = 0.143 if self.protocol._getFSCType() == 0 else 0.5
+        viewer = FscViewer(
+            project=self.getProject(),
+            figure=None,
+            protocol=self.protocol,
+            threshold=thr)
+
+        if self.protocol._getFSCType() == 2:
+            return [viewer.visualize(self.protocol.outputSetOfFSCs)]
+        else:
+            return [viewer.visualize(self.protocol.outputFSC)]
```

### Comparing `scipion-em-relion-4.0b8/relion/wizards.py` & `scipion-em-relion-5.0.0b1/relion/wizards.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
+import logging
+logger = logging.getLogger(__name__)
 
 from pwem.constants import UNIT_PIXEL, UNIT_ANGSTROM, FILTER_LOW_PASS_NO_DECAY
 from pwem.viewers import EmPlotter
 from pwem.wizards.wizard import (ParticleMaskRadiusWizard, FilterVolumesWizard,
                                  EmWizard, ColorScaleWizardBase,
                                  BandPassFilterDialog, dialog)
 from pyworkflow.gui.browser import FileBrowserWindow
@@ -191,15 +193,15 @@
                 (ProtRelionClassify3D, ['defocusRange']),
                 (ProtRelionRefine3D, ['defocusRange']),
                 (ProtRelionInitialModel, ['defocusRange'])]
 
     def show(self, form, *args):
         prot = form.protocol
         defocusGroups = prot.createDefocusGroups()
-        print(defocusGroups)
+        logger.info(defocusGroups)
 
         plotter = EmPlotter(windowTitle='%d Defocus Groups' % len(defocusGroups),
                             figsize=(8, 6))
         ax = plotter.createSubPlot("", "defocus (A)", "count", 1, 1)
 
         for group in defocusGroups:
             ax.bar(group.minDefocus, group.count,
```

### Comparing `scipion-em-relion-4.0b8/scipion_em_relion.egg-info/PKG-INFO` & `scipion-em-relion-5.0.0b1/scipion_em_relion.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 1.2
 Name: scipion-em-relion
-Version: 4.0b8
+Version: 5.0.0b1
 Summary: Plugin to use Relion programs within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-relion
 Author: Grigory Sharov, J.M. De la Rosa Trevin, Josue Gomez Blanco
 Author-email: gsharov@mrc-lmb.cam.ac.uk, delarosatrevin@scilifelab.se, josue.gomez-blanco@mcgill.ca
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-relion/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-relion/
 Description: =============
         Relion plugin
         =============
         
-        This plugin provide wrappers around several programs of `RELION <https://www3.mrc-lmb.cam.ac.uk/relion/index.php/Main_Page>`_ software suite.
+        This plugin provides wrappers for several programs of `RELION <https://relion.readthedocs.io/en/latest/index.html>`_ software suite.
         
         .. image:: https://img.shields.io/pypi/v/scipion-em-relion.svg
                 :target: https://pypi.python.org/pypi/scipion-em-relion
                 :alt: PyPI release
         
         .. image:: https://img.shields.io/pypi/l/scipion-em-relion.svg
                 :target: https://pypi.python.org/pypi/scipion-em-relion
@@ -34,15 +34,15 @@
                 :target: https://pypi.python.org/pypi/scipion-em-relion
                 :alt: Downloads
         
         
         **IMPORTANT NOTES!**
         
             1. If you have imported movies with a gain file in **DM4** format, you need to **flip the gain reference upside-down** in the motion correction protocol! (`bug details <https://github.com/I2PC/xmippCore/issues/39>`_)
-            2. If you have provided a gain reference or defects file during movie import or motion correction, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in this polishing protocol.
+            2. If you have provided a gain reference or defects file during movie import or motion correction and plan to run bayesian polishing, please **make sure to run first "assign optics groups" protocol for aligned movies**, specifying the gain file etc. Currently, Scipion has no other way of knowing if you have e.g. rotated the gain during motion correction. Output movies then can be used in the polishing protocol.
             3. When importing EER movies, you should specify dose per single EER frame during import step. Pixel size should be the physical pixel size unless you plan to render EER on 8K grid. In the Motioncor protocol choose binning, EER fractionation and upsampling (default=1 is for 4K grid).
         
         Installation
         ------------
         
         You will need to use 3.0+ version of Scipion to be able to run these protocols. To install the plugin, you have two options:
         
@@ -54,58 +54,63 @@
         
         b) Developer's version
         
            * download repository
         
            .. code-block::
         
-              git clone https://github.com/scipion-em/scipion-em-relion.git
+              git clone -b devel https://github.com/scipion-em/scipion-em-relion.git
         
            * install
         
            .. code-block::
         
-              scipion installp -p path_to_scipion-em-relion --devel
+              scipion installp -p /path/to/scipion-em-relion --devel
         
-        - RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-4.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
-        - If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file.
+        - RELION sources will be downloaded and compiled automatically with the plugin, but you can also link an existing installation. Default installation path assumed is ``software/em/relion-5.0``, if you want to change it, set *RELION_HOME* in ``scipion.conf`` file to the folder where the RELION is installed.
+        - If you need to use CUDA different from the one used during Scipion installation (defined by *CUDA_LIB*), you can add *RELION_CUDA_LIB* variable to the config file. Optionally, you can also specify *RELION_CUDA_BIN* path for nvcc.
         - If you have to use a MPI for Relion different from Scipion MPI, you can set *RELION_MPI_BIN* and *RELION_MPI_LIB* variables in the config file.
-        - If you want to use **2D class ranker** protocol, you also need to set *RELION_PYTHON* that points to a Python which includes torch and numpy modules.
+        - To add support for Python modules (e.g. Blush, ModelAngelo and DynaMight) you will have to setup a Python environment with dependencies. You need to set *RELION_ENV_ACTIVATION* that points to a conda environment. Default = ``conda activate relion-5.0``
+        - You might want to set *TORCH_HOME* pointing to the path with downloaded models. Default = ``software/em/modelangelomodels-1.0`` (shared with ModelAngelo plugin).
+        - If you want to use SIDESPLITTER, you need the `sidesplitter <https://github.com/scipion-em/scipion-em-sidesplitter>`_ plugin installed and *SIDESPLITTER_HOME* set properly. After that, you only need to add *--external_reconstruct* into Additional arguments field of a 3D auto-refine or multi-body job.
         
         To check the installation, simply run one of the tests. A complete list of tests can be displayed by executing ``scipion test --show --grep relion``
         
         Supported versions
         ------------------
         
-        3.1.3, 4.0
+        4.0, 5.0
         
         Protocols
         ---------
         
         * 2D class ranker
         * 2D classification         
         * 3D auto-refine            
         * 3D classification         
         * 3D initial model          
         * 3D multi-body
         * assign optics groups
         * auto-picking (reference-based)
         * auto-picking LoG          
-        * bayesian polishing        
+        * bayesian polishing
+        * calculate fsc
         * center averages
         * clean project
         * compress movies
         * create 3d mask
         * crop / resize volumes
         * ctf refinement
+        * DynaMight flexibility
         * estimate gain to compress
         * expand symmetry
         * export coordinates
         * export ctf                
-        * export particles          
+        * export particles
+        * import coordinates
         * local resolution          
         * motion correction
         * particles extraction
         * post-processing           
         * preprocess particles      
         * reconstruct
         * remove preferential views
@@ -115,13 +120,14 @@
         References
         ----------
         
         1. Scheres et al., JMB, 2012 
         2. Scheres et al., JSB, 2012 
         3. Kimanius et al., eLife, 2016 
         4. Zivanov et al., eLife, 2018
+        5. Kimanius et al., Biochemical Journal, 2021
         
 Keywords: scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `scipion-em-relion-4.0b8/setup.py` & `scipion-em-relion-5.0.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     packages=find_packages(),
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['scipion-em', 'emtable'],  # Optional
+    install_requires=['scipion-em', 'emtable>=0.0.14'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

