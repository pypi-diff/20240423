# Comparing `tmp/deepinv-0.1.1.tar.gz` & `tmp/deepinv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepinv-0.1.1.tar", last modified: Fri Feb 23 17:02:21 2024, max compression
+gzip compressed data, was "deepinv-0.2.0.tar", last modified: Tue Apr 23 14:08:57 2024, max compression
```

## Comparing `deepinv-0.1.1.tar` & `deepinv-0.2.0.tar`

### file list

```diff
@@ -1,119 +1,147 @@
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.933090 deepinv-0.1.1/
--rw-r--r--   0 jtachell (496653) users      (100)     1494 2024-02-23 17:01:56.000000 deepinv-0.1.1/LICENSE
--rw-r--r--   0 jtachell (496653) users      (100)     6983 2024-02-23 17:02:21.929090 deepinv-0.1.1/PKG-INFO
--rw-r--r--   0 jtachell (496653) users      (100)     5328 2024-02-23 17:01:56.000000 deepinv-0.1.1/README.rst
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.069067 deepinv-0.1.1/deepinv/
--rw-r--r--   0 jtachell (496653) users      (100)      443 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/__about__.py
--rw-r--r--   0 jtachell (496653) users      (100)     1173 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/__init__.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.105068 deepinv-0.1.1/deepinv/datasets/
--rw-r--r--   0 jtachell (496653) users      (100)       57 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/datasets/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     8784 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/datasets/datagenerator.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.193070 deepinv-0.1.1/deepinv/loss/
--rw-r--r--   0 jtachell (496653) users      (100)      540 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     2681 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/ei.py
--rw-r--r--   0 jtachell (496653) users      (100)     1306 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/mc.py
--rw-r--r--   0 jtachell (496653) users      (100)     8170 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/measplit.py
--rw-r--r--   0 jtachell (496653) users      (100)     3764 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/metric.py
--rw-r--r--   0 jtachell (496653) users      (100)     2306 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/moi.py
--rw-r--r--   0 jtachell (496653) users      (100)     2291 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/r2r.py
--rw-r--r--   0 jtachell (496653) users      (100)     5756 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/regularisers.py
--rw-r--r--   0 jtachell (496653) users      (100)     1222 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/score.py
--rw-r--r--   0 jtachell (496653) users      (100)     1063 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/sup.py
--rw-r--r--   0 jtachell (496653) users      (100)    11893 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/sure.py
--rw-r--r--   0 jtachell (496653) users      (100)     1331 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/loss/tv.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.405076 deepinv-0.1.1/deepinv/models/
--rw-r--r--   0 jtachell (496653) users      (100)     4434 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/GSPnP.py
--rw-r--r--   0 jtachell (496653) users      (100)     4127 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/PDNet.py
--rw-r--r--   0 jtachell (496653) users      (100)      564 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     1253 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/ae.py
--rw-r--r--   0 jtachell (496653) users      (100)     2081 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/artifactremoval.py
--rw-r--r--   0 jtachell (496653) users      (100)     1948 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/bm3d.py
--rw-r--r--   0 jtachell (496653) users      (100)    35458 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/diffunet.py
--rw-r--r--   0 jtachell (496653) users      (100)     6731 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/dip.py
--rw-r--r--   0 jtachell (496653) users      (100)     5304 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/dncnn.py
--rw-r--r--   0 jtachell (496653) users      (100)    20540 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/drunet.py
--rw-r--r--   0 jtachell (496653) users      (100)     5223 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/equivariant.py
--rw-r--r--   0 jtachell (496653) users      (100)     1838 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/median.py
--rw-r--r--   0 jtachell (496653) users      (100)    15946 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/scunet.py
--rw-r--r--   0 jtachell (496653) users      (100)    41382 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/swinir.py
--rw-r--r--   0 jtachell (496653) users      (100)     9025 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/tgv.py
--rw-r--r--   0 jtachell (496653) users      (100)     5458 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/tv.py
--rw-r--r--   0 jtachell (496653) users      (100)    11615 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/unet.py
--rw-r--r--   0 jtachell (496653) users      (100)      425 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/utils.py
--rw-r--r--   0 jtachell (496653) users      (100)    13304 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/models/wavdict.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.453077 deepinv-0.1.1/deepinv/optim/
--rw-r--r--   0 jtachell (496653) users      (100)      298 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)    23440 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/data_fidelity.py
--rw-r--r--   0 jtachell (496653) users      (100)    12348 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/fixed_point.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.521079 deepinv-0.1.1/deepinv/optim/optim_iterators/
--rw-r--r--   0 jtachell (496653) users      (100)      343 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     4626 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/admm.py
--rw-r--r--   0 jtachell (496653) users      (100)     4479 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/drs.py
--rw-r--r--   0 jtachell (496653) users      (100)     3346 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/gradient_descent.py
--rw-r--r--   0 jtachell (496653) users      (100)     2502 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/hqs.py
--rw-r--r--   0 jtachell (496653) users      (100)     6215 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/optim_iterator.py
--rw-r--r--   0 jtachell (496653) users      (100)     3059 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/pgd.py
--rw-r--r--   0 jtachell (496653) users      (100)     6458 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/primal_dual_CP.py
--rw-r--r--   0 jtachell (496653) users      (100)      652 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optim_iterators/utils.py
--rw-r--r--   0 jtachell (496653) users      (100)    27210 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/optimizers.py
--rw-r--r--   0 jtachell (496653) users      (100)    12394 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/prior.py
--rw-r--r--   0 jtachell (496653) users      (100)     2413 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/optim/utils.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.629082 deepinv-0.1.1/deepinv/physics/
--rw-r--r--   0 jtachell (496653) users      (100)      576 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)    20527 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/blur.py
--rw-r--r--   0 jtachell (496653) users      (100)     7194 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/compressed_sensing.py
--rw-r--r--   0 jtachell (496653) users      (100)    25162 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/forward.py
--rw-r--r--   0 jtachell (496653) users      (100)     2041 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/haze.py
--rw-r--r--   0 jtachell (496653) users      (100)     3322 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/inpainting.py
--rw-r--r--   0 jtachell (496653) users      (100)     4033 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/lidar.py
--rw-r--r--   0 jtachell (496653) users      (100)    11020 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/mri.py
--rw-r--r--   0 jtachell (496653) users      (100)     6555 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/noise.py
--rw-r--r--   0 jtachell (496653) users      (100)     1784 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/range.py
--rw-r--r--   0 jtachell (496653) users      (100)     4346 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/remote_sensing.py
--rw-r--r--   0 jtachell (496653) users      (100)     7542 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/singlepixel.py
--rw-r--r--   0 jtachell (496653) users      (100)    11778 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/physics/tomography.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.673083 deepinv-0.1.1/deepinv/sampling/
--rw-r--r--   0 jtachell (496653) users      (100)      106 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/sampling/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)    27320 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/sampling/diffusion.py
--rw-r--r--   0 jtachell (496653) users      (100)    19732 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/sampling/langevin.py
--rw-r--r--   0 jtachell (496653) users      (100)      796 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/sampling/utils.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.757085 deepinv-0.1.1/deepinv/tests/
--rw-r--r--   0 jtachell (496653) users      (100)      613 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/conftest.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.761085 deepinv-0.1.1/deepinv/tests/dummy_datasets/
--rw-r--r--   0 jtachell (496653) users      (100)     1812 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/dummy_datasets/datasets.py
--rw-r--r--   0 jtachell (496653) users      (100)     8123 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_loss.py
--rw-r--r--   0 jtachell (496653) users      (100)     5368 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_loss_train.py
--rw-r--r--   0 jtachell (496653) users      (100)    17718 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_models.py
--rw-r--r--   0 jtachell (496653) users      (100)    22217 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_optim.py
--rw-r--r--   0 jtachell (496653) users      (100)    12271 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_physics.py
--rw-r--r--   0 jtachell (496653) users      (100)     4199 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_sampling.py
--rw-r--r--   0 jtachell (496653) users      (100)     5646 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_unfolded.py
--rw-r--r--   0 jtachell (496653) users      (100)     1701 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/tests/test_utils.py
--rw-r--r--   0 jtachell (496653) users      (100)    21241 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/training_utils.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.821087 deepinv-0.1.1/deepinv/transform/
--rw-r--r--   0 jtachell (496653) users      (100)       77 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/transform/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     1454 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/transform/rotate.py
--rw-r--r--   0 jtachell (496653) users      (100)     2656 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/transform/scale.py
--rw-r--r--   0 jtachell (496653) users      (100)     1430 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/transform/shift.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.865088 deepinv-0.1.1/deepinv/unfolded/
--rw-r--r--   0 jtachell (496653) users      (100)      102 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/unfolded/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     8074 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/unfolded/deep_equilibrium.py
--rw-r--r--   0 jtachell (496653) users      (100)     4963 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/unfolded/unfolded.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.917090 deepinv-0.1.1/deepinv/utils/
--rw-r--r--   0 jtachell (496653) users      (100)      555 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/__init__.py
--rw-r--r--   0 jtachell (496653) users      (100)     5386 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/demo.py
--rw-r--r--   0 jtachell (496653) users      (100)     2459 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/logger.py
--rw-r--r--   0 jtachell (496653) users      (100)     2484 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/metric.py
--rw-r--r--   0 jtachell (496653) users      (100)     6529 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/nn.py
--rw-r--r--   0 jtachell (496653) users      (100)     3715 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/optimization.py
--rw-r--r--   0 jtachell (496653) users      (100)     1360 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/parameters.py
--rw-r--r--   0 jtachell (496653) users      (100)     4003 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/phantoms.py
--rw-r--r--   0 jtachell (496653) users      (100)    10736 2024-02-23 17:01:56.000000 deepinv-0.1.1/deepinv/utils/plotting.py
-drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-02-23 17:02:21.921090 deepinv-0.1.1/deepinv.egg-info/
--rw-r--r--   0 jtachell (496653) users      (100)     6983 2024-02-23 17:02:20.000000 deepinv-0.1.1/deepinv.egg-info/PKG-INFO
--rw-r--r--   0 jtachell (496653) users      (100)     2802 2024-02-23 17:02:20.000000 deepinv-0.1.1/deepinv.egg-info/SOURCES.txt
--rw-r--r--   0 jtachell (496653) users      (100)        1 2024-02-23 17:02:20.000000 deepinv-0.1.1/deepinv.egg-info/dependency_links.txt
--rw-r--r--   0 jtachell (496653) users      (100)      214 2024-02-23 17:02:20.000000 deepinv-0.1.1/deepinv.egg-info/requires.txt
--rw-r--r--   0 jtachell (496653) users      (100)        8 2024-02-23 17:02:20.000000 deepinv-0.1.1/deepinv.egg-info/top_level.txt
--rw-r--r--   0 jtachell (496653) users      (100)     1815 2024-02-23 17:01:57.000000 deepinv-0.1.1/pyproject.toml
--rw-r--r--   0 jtachell (496653) users      (100)       38 2024-02-23 17:02:21.933090 deepinv-0.1.1/setup.cfg
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.582921 deepinv-0.2.0/
+-rw-r--r--   0 jtachell (496653) users      (100)     1494 2024-04-23 14:08:25.000000 deepinv-0.2.0/LICENSE
+-rw-r--r--   0 jtachell (496653) users      (100)     7174 2024-04-23 14:08:57.578921 deepinv-0.2.0/PKG-INFO
+-rw-r--r--   0 jtachell (496653) users      (100)     5386 2024-04-23 14:08:25.000000 deepinv-0.2.0/README.rst
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:56.494892 deepinv-0.2.0/deepinv/
+-rw-r--r--   0 jtachell (496653) users      (100)      405 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/__about__.py
+-rw-r--r--   0 jtachell (496653) users      (100)      918 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/__init__.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:56.566894 deepinv-0.2.0/deepinv/datasets/
+-rw-r--r--   0 jtachell (496653) users      (100)       97 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/datasets/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     9000 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/datasets/datagenerator.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1190 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/datasets/patch_dataset.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:56.670896 deepinv-0.2.0/deepinv/loss/
+-rw-r--r--   0 jtachell (496653) users      (100)      583 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2712 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/ei.py
+-rw-r--r--   0 jtachell (496653) users      (100)      960 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/loss.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1314 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/mc.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8219 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/measplit.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7636 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/metric.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2314 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/moi.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2263 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/r2r.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5915 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/regularisers.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1230 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/score.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1094 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/sup.py
+-rw-r--r--   0 jtachell (496653) users      (100)    11269 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/sure.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1512 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/loss/tv.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:56.934904 deepinv-0.2.0/deepinv/models/
+-rw-r--r--   0 jtachell (496653) users      (100)     4420 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/GSPnP.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4127 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/PDNet.py
+-rw-r--r--   0 jtachell (496653) users      (100)      639 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1253 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/ae.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2081 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/artifactremoval.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1948 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/bm3d.py
+-rw-r--r--   0 jtachell (496653) users      (100)    35450 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/diffunet.py
+-rw-r--r--   0 jtachell (496653) users      (100)     6733 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/dip.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5304 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/dncnn.py
+-rw-r--r--   0 jtachell (496653) users      (100)    18768 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/drunet.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2817 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/epll.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5219 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/equivariant.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1956 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/median.py
+-rw-r--r--   0 jtachell (496653) users      (100)    27420 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/restormer.py
+-rw-r--r--   0 jtachell (496653) users      (100)    15938 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/scunet.py
+-rw-r--r--   0 jtachell (496653) users      (100)    41388 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/swinir.py
+-rw-r--r--   0 jtachell (496653) users      (100)     9009 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/tgv.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5793 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/tv.py
+-rw-r--r--   0 jtachell (496653) users      (100)    11665 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/unet.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2274 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/utils.py
+-rw-r--r--   0 jtachell (496653) users      (100)    14086 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/models/wavdict.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.002905 deepinv-0.2.0/deepinv/optim/
+-rw-r--r--   0 jtachell (496653) users      (100)      504 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)    26347 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/data_fidelity.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2279 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/dpir.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8837 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/epll.py
+-rw-r--r--   0 jtachell (496653) users      (100)    12398 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/fixed_point.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.074907 deepinv-0.2.0/deepinv/optim/optim_iterators/
+-rw-r--r--   0 jtachell (496653) users      (100)      302 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4652 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/admm.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4513 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/drs.py
+-rw-r--r--   0 jtachell (496653) users      (100)     3354 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/gradient_descent.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2539 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/hqs.py
+-rw-r--r--   0 jtachell (496653) users      (100)     6235 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/optim_iterator.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2953 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/pgd.py
+-rw-r--r--   0 jtachell (496653) users      (100)     6514 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/primal_dual_CP.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4043 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/spectral_methods.py
+-rw-r--r--   0 jtachell (496653) users      (100)      652 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optim_iterators/utils.py
+-rw-r--r--   0 jtachell (496653) users      (100)    28565 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/optimizers.py
+-rw-r--r--   0 jtachell (496653) users      (100)    23209 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/prior.py
+-rw-r--r--   0 jtachell (496653) users      (100)    13793 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/optim/utils.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.198911 deepinv-0.2.0/deepinv/physics/
+-rw-r--r--   0 jtachell (496653) users      (100)      714 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)    21421 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/blur.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7709 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/compressed_sensing.py
+-rw-r--r--   0 jtachell (496653) users      (100)    28384 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/forward.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.242912 deepinv-0.2.0/deepinv/physics/functional/
+-rw-r--r--   0 jtachell (496653) users      (100)      462 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)    11451 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/convolution.py
+-rw-r--r--   0 jtachell (496653) users      (100)      106 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/downsampling.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7087 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/hist.py
+-rw-r--r--   0 jtachell (496653) users      (100)     6420 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/interp.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1637 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/multiplier.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2620 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/product_convolution.py
+-rw-r--r--   0 jtachell (496653) users      (100)     9836 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/functional/radon.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.290913 deepinv-0.2.0/deepinv/physics/generator/
+-rw-r--r--   0 jtachell (496653) users      (100)      262 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/generator/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4968 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/generator/base.py
+-rw-r--r--   0 jtachell (496653) users      (100)    22289 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/generator/blur.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2693 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/generator/mri.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1669 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/generator/noise.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2061 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/haze.py
+-rw-r--r--   0 jtachell (496653) users      (100)     3410 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/inpainting.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4053 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/lidar.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8774 2024-04-23 14:08:25.000000 deepinv-0.2.0/deepinv/physics/mri.py
+-rw-r--r--   0 jtachell (496653) users      (100)     9552 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/noise.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4528 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/phase_retrieval.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1849 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/range.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4561 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/remote_sensing.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7521 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/singlepixel.py
+-rw-r--r--   0 jtachell (496653) users      (100)     3757 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/physics/tomography.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.306914 deepinv-0.2.0/deepinv/sampling/
+-rw-r--r--   0 jtachell (496653) users      (100)      106 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/sampling/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)    27447 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/sampling/diffusion.py
+-rw-r--r--   0 jtachell (496653) users      (100)    19742 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/sampling/langevin.py
+-rw-r--r--   0 jtachell (496653) users      (100)      796 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/sampling/utils.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.358915 deepinv-0.2.0/deepinv/tests/
+-rw-r--r--   0 jtachell (496653) users      (100)      643 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/conftest.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.366915 deepinv-0.2.0/deepinv/tests/dummy_datasets/
+-rw-r--r--   0 jtachell (496653) users      (100)     1812 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/dummy_datasets/datasets.py
+-rw-r--r--   0 jtachell (496653) users      (100)    12033 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_generators.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7785 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_loss.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5566 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_loss_train.py
+-rw-r--r--   0 jtachell (496653) users      (100)    18677 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_models.py
+-rw-r--r--   0 jtachell (496653) users      (100)    26138 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_optim.py
+-rw-r--r--   0 jtachell (496653) users      (100)    17665 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_physics.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4196 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_sampling.py
+-rw-r--r--   0 jtachell (496653) users      (100)     5652 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_unfolded.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2635 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/tests/test_utils.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.394916 deepinv-0.2.0/deepinv/training/
+-rw-r--r--   0 jtachell (496653) users      (100)       62 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/training/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8368 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/training/testing.py
+-rw-r--r--   0 jtachell (496653) users      (100)    31331 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/training/trainer.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.438917 deepinv-0.2.0/deepinv/transform/
+-rw-r--r--   0 jtachell (496653) users      (100)       77 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/transform/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1454 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/transform/rotate.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2656 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/transform/scale.py
+-rw-r--r--   0 jtachell (496653) users      (100)     1430 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/transform/shift.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.490919 deepinv-0.2.0/deepinv/unfolded/
+-rw-r--r--   0 jtachell (496653) users      (100)      102 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/unfolded/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8058 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/unfolded/deep_equilibrium.py
+-rw-r--r--   0 jtachell (496653) users      (100)     8095 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/unfolded/unfolded.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.542920 deepinv-0.2.0/deepinv/utils/
+-rw-r--r--   0 jtachell (496653) users      (100)      604 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/__init__.py
+-rw-r--r--   0 jtachell (496653) users      (100)     6067 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/demo.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2906 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/logger.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2790 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/metric.py
+-rw-r--r--   0 jtachell (496653) users      (100)     7807 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/nn.py
+-rw-r--r--   0 jtachell (496653) users      (100)     3715 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/optimization.py
+-rw-r--r--   0 jtachell (496653) users      (100)      850 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/parameters.py
+-rw-r--r--   0 jtachell (496653) users      (100)     2493 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/patch_extractor.py
+-rw-r--r--   0 jtachell (496653) users      (100)     4003 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/phantoms.py
+-rw-r--r--   0 jtachell (496653) users      (100)    16510 2024-04-23 14:08:26.000000 deepinv-0.2.0/deepinv/utils/plotting.py
+drwxr-xr-x   0 jtachell (496653) users      (100)        0 2024-04-23 14:08:57.566921 deepinv-0.2.0/deepinv.egg-info/
+-rw-r--r--   0 jtachell (496653) users      (100)     7174 2024-04-23 14:08:56.000000 deepinv-0.2.0/deepinv.egg-info/PKG-INFO
+-rw-r--r--   0 jtachell (496653) users      (100)     3659 2024-04-23 14:08:56.000000 deepinv-0.2.0/deepinv.egg-info/SOURCES.txt
+-rw-r--r--   0 jtachell (496653) users      (100)        1 2024-04-23 14:08:56.000000 deepinv-0.2.0/deepinv.egg-info/dependency_links.txt
+-rw-r--r--   0 jtachell (496653) users      (100)      242 2024-04-23 14:08:56.000000 deepinv-0.2.0/deepinv.egg-info/requires.txt
+-rw-r--r--   0 jtachell (496653) users      (100)        8 2024-04-23 14:08:56.000000 deepinv-0.2.0/deepinv.egg-info/top_level.txt
+-rw-r--r--   0 jtachell (496653) users      (100)     1865 2024-04-23 14:08:26.000000 deepinv-0.2.0/pyproject.toml
+-rw-r--r--   0 jtachell (496653) users      (100)       38 2024-04-23 14:08:57.582921 deepinv-0.2.0/setup.cfg
```

### Comparing `deepinv-0.1.1/LICENSE` & `deepinv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/PKG-INFO` & `deepinv-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepinv
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pytorch library for solving inverse problems with deep learning
 Author-email: Julian Tachella <tachellajulian@gmail.com>
 License: BSD 3-Clause
 Project-URL: Homepage, https://deepinv.github.io/
 Project-URL: Source, https://github.com/deepinv/deepinv
 Project-URL: Tracker, https://github.com/deepinv/deepinv/issues
 Platform: any
@@ -33,20 +33,23 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_gallery; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Requires-Dist: sphinxemoji; extra == "doc"
-Requires-Dist: sphinx_exec_code; extra == "doc"
+Requires-Dist: sphinx_copybutton; extra == "doc"
+Requires-Dist: sphinx_autoapi; extra == "doc"
 Provides-Extra: denoisers
 Requires-Dist: bm3d; extra == "denoisers"
 Requires-Dist: timm; extra == "denoisers"
 Requires-Dist: PyWavelets; extra == "denoisers"
 Requires-Dist: ptwt; extra == "denoisers"
+Requires-Dist: FrEIA; extra == "denoisers"
+Requires-Dist: pyiqa; extra == "denoisers"
 
 .. image:: https://github.com/deepinv/deepinv/raw/main/docs/source/figures/deepinv_logolarge.png
    :width: 500px
    :alt: deepinv logo
    :align: center
 
 
@@ -96,30 +99,30 @@
 
 Getting Started
 ---------------
 Try out the following plug-and-play image inpainting example:
 
 .. code-block:: python
 
-    import deepinv as dinv
-    from deepinv.utils import load_url_image
-
-    url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
-    x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
-
-    physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
-                                       noise_model=dinv.physics.GaussianNoise(sigma=0.01))
-
-    data_fidelity = dinv.optim.data_fidelity.L2()
-    prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
-    model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
-                                     params_algo={"stepsize": 1.0, "g_param": 0.1, "lambda": 2.})
-    y = physics(x)
-    x_hat = model(y, physics)
-    dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
+    >>> import deepinv as dinv
+    >>> from deepinv.utils import load_url_image
+    >>>
+    >>> url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
+    >>> x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
+    >>>
+    >>> physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
+    >>>                                    noise_model=dinv.physics.GaussianNoise(sigma=0.01))
+    >>>
+    >>> data_fidelity = dinv.optim.data_fidelity.L2()
+    >>> prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
+    >>> model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
+    >>>                                 params_algo={"stepsize": 1.0, "g_param": 0.1})
+    >>> y = physics(x)
+    >>> x_hat = model(y, physics)
+    >>> dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
 
 
 Also try out `one of the examples <https://deepinv.github.io/deepinv/auto_examples/index.html>`_ to get started.
 
 Contributing
 ------------
```

### Comparing `deepinv-0.1.1/README.rst` & `deepinv-0.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -50,30 +50,30 @@
 
 Getting Started
 ---------------
 Try out the following plug-and-play image inpainting example:
 
 .. code-block:: python
 
-    import deepinv as dinv
-    from deepinv.utils import load_url_image
-
-    url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
-    x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
-
-    physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
-                                       noise_model=dinv.physics.GaussianNoise(sigma=0.01))
-
-    data_fidelity = dinv.optim.data_fidelity.L2()
-    prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
-    model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
-                                     params_algo={"stepsize": 1.0, "g_param": 0.1, "lambda": 2.})
-    y = physics(x)
-    x_hat = model(y, physics)
-    dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
+    >>> import deepinv as dinv
+    >>> from deepinv.utils import load_url_image
+    >>>
+    >>> url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
+    >>> x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
+    >>>
+    >>> physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
+    >>>                                    noise_model=dinv.physics.GaussianNoise(sigma=0.01))
+    >>>
+    >>> data_fidelity = dinv.optim.data_fidelity.L2()
+    >>> prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
+    >>> model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
+    >>>                                 params_algo={"stepsize": 1.0, "g_param": 0.1})
+    >>> y = physics(x)
+    >>> x_hat = model(y, physics)
+    >>> dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
 
 
 Also try out `one of the examples <https://deepinv.github.io/deepinv/auto_examples/index.html>`_ to get started.
 
 Contributing
 ------------
```

### Comparing `deepinv-0.1.1/deepinv/datasets/datagenerator.py` & `deepinv-0.2.0/deepinv/datasets/datagenerator.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     device="cpu",
     train_datapoints=None,
     test_datapoints=None,
     dataset_filename="dinv_dataset",
     batch_size=4,
     num_workers=0,
     supervised=True,
+    verbose=True,
+    show_progress_bar=False,
 ):
     r"""
     Generates dataset of signal/measurement pairs from base dataset.
 
     It generates the measurement data using the forward operator provided by the user.
     The dataset is saved in HD5 format and can be easily loaded using the HD5Dataset class.
     The generated dataset contains a train and test splits.
@@ -84,14 +86,17 @@
     :param int batch_size: batch size for generating the measurement data
         (it only affects the speed of the generating process)
     :param int num_workers: number of workers for generating the measurement data
         (it only affects the speed of the generating process)
     :param bool supervised: Generates supervised pairs (x,y) of measurements and signals.
         If set to ``False``, it will generate a training dataset with measurements only (y)
         and a test dataset with pairs (x,y)
+    :param bool verbose: Output progress information in the console.
+    :param bool show_progress_bar: Show progress bar during the generation
+        of the dataset (if verbose is set to True).
 
     """
     if os.path.exists(os.path.join(save_dir, dataset_filename)):
         print(
             "WARNING: Dataset already exists, this will overwrite the previous dataset."
         )
 
@@ -148,51 +153,52 @@
 
         if train_dataset is not None:
 
             hf.create_dataset("y_train", (n_train_g,) + y.shape[1:], dtype="float")
             if supervised:
                 hf.create_dataset("x_train", (n_train_g,) + x.shape[1:], dtype="float")
 
-            if G > 1:
-                print(
-                    f"Computing train measurement vectors from base dataset of operator {g + 1} out of {G}..."
-                )
-            else:
-                print("Computing train measurement vectors from base dataset...")
-
             index = 0
 
             epochs = int(n_train_g / len(train_dataset)) + 1
-            for e in tqdm(range(epochs)):
+            for e in (progress_bar := tqdm(range(epochs), ncols=150, disable=(not verbose or not show_progress_bar))):
+
+                desc = f"Generating dataset operator {g + 1}" if G > 1 else "Generating train dataset"
+                progress_bar.set_description(desc)
+
                 train_dataloader = DataLoader(
                     Subset(
                         train_dataset,
                         indices=list(range(g * n_dataset_g, (g + 1) * n_dataset_g)),
                     ),
                     batch_size=batch_size,
                     num_workers=num_workers,
                     pin_memory=False if device == "cpu" else True,
                 )
 
-                for i, x in enumerate(train_dataloader):
+                batches = len(train_dataloader) - int(train_dataloader.drop_last)
+                iterator = iter(train_dataloader)
+                for _ in range(batches):
+
+                    x = next(iterator)
                     x = x[0] if isinstance(x, list) or isinstance(x, tuple) else x
                     x = x.to(device)
 
                     # choose operator and generate measurement
                     y = physics[g](x)
 
                     # Add new data to it
                     bsize = x.size()[0]
 
                     if bsize + index > n_train_g:
                         bsize = n_train_g - index
 
-                    hf["y_train"][index : index + bsize] = y[:bsize, :].to("cpu").numpy()
+                    hf["y_train"][index: index + bsize] = y[:bsize, :].to("cpu").numpy()
                     if supervised:
-                        hf["x_train"][index : index + bsize] = (
+                        hf["x_train"][index: index + bsize] = (
                             x[:bsize, :, :, :].to("cpu").numpy()
                         )
                     index = index + bsize
 
         if test_dataset is not None:
             index = 0
             test_dataloader = DataLoader(
@@ -200,22 +206,19 @@
                     test_dataset, indices=list(range(g * n_test_g, (g + 1) * n_test_g))
                 ),
                 batch_size=batch_size,
                 num_workers=num_workers,
                 pin_memory=True,
             )
 
-            if G > 1:
-                print(
-                    f"Computing test measurement vectors from base dataset of operator {g + 1} out of {G}..."
-                )
-            else:
-                print("Computing test measurement vectors from base dataset...")
+            batches = len(test_dataloader) - int(test_dataloader.drop_last)
+            iterator = iter(test_dataloader)
+            for i in range(batches):
 
-            for i, x in enumerate(tqdm(test_dataloader)):
+                x = next(iterator)
                 x = x[0] if isinstance(x, list) or isinstance(x, tuple) else x
                 x = x.to(device)
 
                 # choose operator
                 y = physics[g](x)
 
                 if i == 0:  # create dict
@@ -224,15 +227,15 @@
                     )
                     hf.create_dataset(
                         "y_test", (n_test_g,) + y.shape[1:], dtype="float"
                     )
 
                 # Add new data to it
                 bsize = x.size()[0]
-                hf["x_test"][index : index + bsize] = x.to("cpu").numpy()
-                hf["y_test"][index : index + bsize] = y.to("cpu").numpy()
+                hf["x_test"][index: index + bsize] = x.to("cpu").numpy()
+                hf["y_test"][index: index + bsize] = y.to("cpu").numpy()
                 index = index + bsize
         hf.close()
 
     print("Dataset has been saved in " + str(save_dir))
 
     return hf_paths[0] if G == 1 else hf_paths
```

### Comparing `deepinv-0.1.1/deepinv/loss/__init__.py` & `deepinv-0.2.0/deepinv/loss/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,8 +4,9 @@
 from deepinv.loss.sup import SupLoss
 from deepinv.loss.score import ScoreLoss
 from deepinv.loss.tv import TVLoss
 from deepinv.loss.r2r import R2RLoss
 from deepinv.loss.sure import SureGaussianLoss, SurePoissonLoss, SurePGLoss
 from deepinv.loss.regularisers import JacobianSpectralNorm, FNEJacobianSpectralNorm
 from deepinv.loss.measplit import SplittingLoss, Neighbor2Neighbor
-from deepinv.loss.metric import LpNorm, CharbonnierLoss
+from deepinv.loss.metric import LpNorm, PSNR, SSIM, LPIPS, NIQE
+from deepinv.loss.loss import Loss
```

### Comparing `deepinv-0.1.1/deepinv/loss/ei.py` & `deepinv-0.2.0/deepinv/loss/ei.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 import torch.nn as nn
+from deepinv.loss.loss import Loss
 
 
-class EILoss(nn.Module):
+class EILoss(Loss):
     r"""
     Equivariant imaging self-supervised loss.
 
     Assumes that the set of signals is invariant to a group of transformations (rotations, translations, etc.)
     in order to learn from incomplete measurement data alone https://https://arxiv.org/pdf/2103.14756.pdf.
 
     The EI loss is defined as
```

### Comparing `deepinv-0.1.1/deepinv/loss/mc.py` & `deepinv-0.2.0/deepinv/loss/mc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
-import torch.nn as nn
+from deepinv.loss.loss import Loss
 
 
-class MCLoss(nn.Module):
+class MCLoss(Loss):
     r"""
     Measurement consistency loss
 
     This loss enforces that the reconstructions are measurement-consistent, i.e., :math:`y=\forw{\inverse{y}}`.
 
     The measurement consistency loss is defined as
```

### Comparing `deepinv-0.1.1/deepinv/loss/measplit.py` & `deepinv-0.2.0/deepinv/loss/measplit.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import torch
 from deepinv.physics import Inpainting
 import numpy as np
+from deepinv.loss.loss import Loss
 
 
-class SplittingLoss(torch.nn.Module):
+class SplittingLoss(Loss):
     r"""
     Measurement splitting loss.
 
     Splits the measurement and forward operator (of size :math:`m`)
     into two smaller pairs  :math:`(y_1,A_1)` (of size :math:`m_1`) and  :math:`(y_2,A_2)` (of size :math:`m_2`) ,
     to compute the self-supervised loss:
 
     .. math::
 
-        \frac{m}{m_2}\| y_2 - A_2 \inversef{y_1,A_1}\|^2
+        \frac{m}{m_2}\| y_2 - A_2 \inversef{y_1}{A_1}\|^2
 
     where :math:`R` is the trainable network. See https://pubmed.ncbi.nlm.nih.gov/32614100/.
 
     By default, the error is computed using the MSE metric, however any other metric (e.g., :math:`\ell_1`)
     can be used as well.
 
     :param torch.nn.Module metric: metric used for computing data consistency,
@@ -51,16 +52,16 @@
             mask[torch.rand_like(mask) > self.split_ratio] = 0
         else:
             stride = int(1 / (1 - self.split_ratio))
             start = np.random.randint(stride)
             mask[..., start::stride, start::stride] = 0.0
 
         # create inpainting masks
-        inp = Inpainting(tsize, mask)
-        inp2 = Inpainting(tsize, 1 - mask)
+        inp = Inpainting(tsize, mask, device=y.device)
+        inp2 = Inpainting(tsize, 1 - mask, device=y.device)
 
         # concatenate operators
         physics1 = inp * physics  # A_1 = P*A
         physics2 = inp2 * physics  # A_2 = (I-P)*A
 
         # divide measurements
         y1 = inp.A(y)
@@ -68,15 +69,15 @@
 
         loss_ms = self.metric(physics2.A(model(y1, physics1)), y2)
         loss_ms /= 1 - self.split_ratio  # normalize loss
 
         return loss_ms
 
 
-class Neighbor2Neighbor(torch.nn.Module):
+class Neighbor2Neighbor(Loss):
     r"""
     Neighbor2Neighbor loss.
 
     Splits the noisy measurements using two masks :math:`A_1` and :math:`A_2`, each choosing a different neighboring
     map (see details in `"Neighbor2Neighbor: Self-Supervised Denoising from Single Noisy Images"
     <https://openaccess.thecvf.com/content/CVPR2021/papers/Huang_Neighbor2Neighbor_Self-Supervised_Denoising_From_Single_Noisy_Images_CVPR_2021_paper.pdf>`_).
```

### Comparing `deepinv-0.1.1/deepinv/loss/moi.py` & `deepinv-0.2.0/deepinv/loss/moi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-import torch.nn as nn
 import numpy as np
+from deepinv.loss.loss import Loss
 
 
-class MOILoss(nn.Module):
+class MOILoss(Loss):
     r"""
     Multi-operator imaging loss
 
     This loss can be used to learn when signals are observed via multiple (possibly incomplete)
     forward operators :math:`\{A_g\}_{g=1}^{G}`,
     i.e., :math:`y_i = A_{g_i}x_i` where :math:`g_i\in \{1,\dots,G\}` (see https://arxiv.org/abs/2201.12151).
```

### Comparing `deepinv-0.1.1/deepinv/loss/r2r.py` & `deepinv-0.2.0/deepinv/loss/r2r.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import torch
-import torch.nn as nn
+from deepinv.loss.loss import Loss
 
-from deepinv.loss.mc import MCLoss
 
-
-class R2RLoss(nn.Module):
+class R2RLoss(Loss):
     r"""
     Recorrupted-to-Recorrupted (R2R) Loss
 
     This loss can be used for unsupervised image denoising with unorganized noisy images.
 
     The loss is designed for the noise model:
```

### Comparing `deepinv-0.1.1/deepinv/loss/regularisers.py` & `deepinv-0.2.0/deepinv/loss/regularisers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
-import torch.nn as nn
+from deepinv.loss.loss import Loss
 
 
-class JacobianSpectralNorm(nn.Module):
+class JacobianSpectralNorm(Loss):
     r"""
     Computes the spectral norm of the Jacobian.
 
     Given a function :math:`f:\mathbb{R}^n\to\mathbb{R}^n`, this module computes the spectral
     norm of the Jacobian of :math:`f` in :math:`x`, i.e.
 
     .. math::
@@ -15,30 +15,32 @@
     This spectral norm is computed with a power method leveraging jacobian vector products, as proposed in `<https://arxiv.org/abs/2012.13247v2>`_.
 
     :param int max_iter: maximum numer of iteration of the power method.
     :param float tol: tolerance for the convergence of the power method.
     :param bool eval_mode: set to `False` if one does not want to backpropagate through the spectral norm (default), set to `True` otherwise.
     :param bool verbose: whether to print computation details or not.
 
+    |sep|
 
-    Example of usage:
+    :Examples:
 
-    ::
+    .. doctest::
 
-        import torch
-        from deepinv.loss.regularisers import JacobianSpectralNorm
-
-        reg_l2 = JacobianSpectralNorm(max_iter=10, tol=1e-3, eval_mode=False, verbose=True)
-
-        A = torch.diag(torch.Tensor(range(1, 51)))  # creates a diagonal matrix with largest eigenvalue = 50
-        x = torch.randn_like(A).requires_grad_()
-        out = A @ x
-
-        regval = reg_l2(out, x)
-        print(regval) # >> returns approx 50
+        >>> import torch
+        >>> from deepinv.loss.regularisers import JacobianSpectralNorm
+        >>> _ = torch.manual_seed(0)
+        >>> _ = torch.cuda.manual_seed(0)
+        >>>
+        >>> reg_l2 = JacobianSpectralNorm(max_iter=10, tol=1e-3, eval_mode=False, verbose=True)
+        >>> A = torch.diag(torch.Tensor(range(1, 51)))  # creates a diagonal matrix with largest eigenvalue = 50
+        >>> x = torch.randn_like(A).requires_grad_()
+        >>> out = A @ x
+        >>> regval = reg_l2(out, x)
+        >>> print(regval) # returns approx 50
+        tensor([49.0202])
     """
 
     def __init__(self, max_iter=10, tol=1e-3, eval_mode=False, verbose=False):
         super(JacobianSpectralNorm, self).__init__()
         self.name = "jsn"
         self.max_iter = max_iter
         self.tol = tol
@@ -96,15 +98,15 @@
                 w.detach_()
                 v.detach_()
                 u.detach_()
 
         return z.view(-1).sqrt()
 
 
-class FNEJacobianSpectralNorm(nn.Module):
+class FNEJacobianSpectralNorm(Loss):
     r"""
     Computes the Firm-Nonexpansiveness Jacobian spectral norm.
 
     Given a function :math:`f:\mathbb{R}^n\to\mathbb{R}^n`, this module computes the spectral
     norm of the Jacobian of :math:`2f-\operatorname{Id}` (where :math:`\operatorname{Id}` denotes the
     identity) in :math:`x`, i.e.
```

### Comparing `deepinv-0.1.1/deepinv/loss/score.py` & `deepinv-0.2.0/deepinv/loss/score.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
-import torch.nn as nn
 import numpy as np
+from deepinv.loss.loss import Loss
 
 
-class ScoreLoss(nn.Module):
+class ScoreLoss(Loss):
     r"""
     Approximates score of a distribution.
 
     It approximates the score of the measurement distribution :math:`S(y)\approx \nabla \log p(y)`
     https://proceedings.neurips.cc/paper_files/paper/2021/file/077b83af57538aa183971a2fe0971ec1-Paper.pdf.
 
     The score loss is defined as
```

### Comparing `deepinv-0.1.1/deepinv/loss/sup.py` & `deepinv-0.2.0/deepinv/loss/sup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 import torch.nn as nn
+from deepinv.loss.loss import Loss
 
 
-class SupLoss(nn.Module):
+class SupLoss(Loss):
     r"""
     Standard supervised loss
 
     The supervised loss is defined as
 
     .. math::
```

### Comparing `deepinv-0.1.1/deepinv/loss/sure.py` & `deepinv-0.2.0/deepinv/loss/sure.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import torch
 import torch.nn as nn
 import numpy as np
+from deepinv.loss.loss import Loss
 
 
 def hutch_div(y, physics, f, mc_iter=1):
     r"""
     Hutch divergence for A(f(x)).
 
     :param torch.Tensor y: Measurements.
@@ -17,15 +18,15 @@
     output = physics.A(f(input, physics))
     out = 0
     for i in range(mc_iter):
         b = torch.randn_like(input)
         x = torch.autograd.grad(output, input, b, retain_graph=True, create_graph=True)[
             0
         ]
-        out += (b * x).mean()
+        out += (b * x).reshape(y.size(0), -1).mean(1)
 
     return out / mc_iter
 
 
 def exact_div(y, physics, model):
     r"""
     Exact divergence for A(f(x)).
@@ -61,22 +62,23 @@
     :param deepinv.physics.Physics physics: Forward operator associated with the measurements.
     :param torch.nn.Module f: Reconstruction network.
     :param int mc_iter: number of iterations. Default=1.
     :return: (float) hutch divergence.
     """
     b = torch.randn_like(y)
     y2 = physics.A(f(y + b * tau, physics))
-    out = (b * (y2 - y1) / tau).mean()
+    out = (b * (y2 - y1) / tau).reshape(y.size(0), -1).mean(1)
     return out
 
 
-class SureGaussianLoss(nn.Module):
+class SureGaussianLoss(Loss):
     r"""
     SURE loss for Gaussian noise
 
+
     The loss is designed for the following noise model:
 
     .. math::
 
         y \sim\mathcal{N}(u,\sigma^2 I) \quad \text{with}\quad u= A(x).
 
     The loss is computed as
@@ -118,25 +120,25 @@
         r"""
         Computes the SURE Loss.
 
         :param torch.Tensor y: Measurements.
         :param torch.Tensor x_net: reconstructed image :math:`\inverse{y}`.
         :param deepinv.physics.Physics physics: Forward operator associated with the measurements.
         :param torch.nn.Module model: Reconstruction network.
-        :return: (float) SURE loss.
+        :return: torch.nn.Tensor loss of size (batch_size,)
         """
 
         y1 = physics.A(x_net)
         div = 2 * self.sigma2 * mc_div(y1, y, model, physics, self.tau)
-        mse = (y1 - y).pow(2).mean()
+        mse = (y1 - y).pow(2).reshape(y.size(0), -1).mean(1)
         loss_sure = mse + div - self.sigma2
         return loss_sure
 
 
-class SurePoissonLoss(nn.Module):
+class SurePoissonLoss(Loss):
     r"""
     SURE loss for Poisson noise
 
     The loss is designed for the following noise model:
 
     .. math::
 
@@ -177,37 +179,38 @@
         r"""
         Computes the SURE loss.
 
         :param torch.Tensor y: measurements.
         :param torch.Tensor x_net: reconstructed image :math:`\inverse{y}`.
         :param deepinv.physics.Physics physics: Forward operator associated with the measurements
         :param torch.nn.Module model: Reconstruction network
-        :return: (float) SURE loss.
+        :return: torch.nn.Tensor loss of size (batch_size,)
         """
 
         # generate a random vector b
         b = torch.rand_like(y) > 0.5
         b = (2 * b - 1) * 1.0  # binary [-1, 1]
 
         y1 = physics.A(x_net)
         y2 = physics.A(model(y + self.tau * b, physics))
 
         # compute m (size of y)
         # m = y.numel() #(torch.abs(y) > 1e-5).flatten().sum()
 
         loss_sure = (
-            (y1 - y).pow(2).mean()
-            - self.gain * y.mean()
-            + 2.0 / self.tau * (b * y * self.gain * (y2 - y1)).mean()
+            (y1 - y).pow(2)
+            - self.gain * y
+            + 2.0 / self.tau * (b * y * self.gain * (y2 - y1))
         )
+        loss_sure = loss_sure.reshape(y.size(0), -1).mean(1)
 
         return loss_sure
 
 
-class SurePGLoss(nn.Module):
+class SurePGLoss(Loss):
     r"""
     SURE loss for Poisson-Gaussian noise
 
     The loss is designed for the following noise model:
 
     .. math::
 
@@ -257,15 +260,15 @@
         r"""
         Computes the SURE loss.
 
         :param torch.Tensor y: measurements.
         :param torch.Tensor x_net: reconstructed image :math:`\inverse{y}`.
         :param deepinv.physics.Physics physics: Forward operator associated with the measurements
         :param torch.nn.Module f: Reconstruction network
-        :return: (float) SURE loss.
+        :return: torch.nn.Tensor loss of size (batch_size,)
         """
 
         b1 = torch.rand_like(y) > 0.5
         b1 = (2 * b1 - 1) * 1.0  # binary [-1, 1]
 
         p = 0.7236  # .5 + .5*np.sqrt(1/5.)
 
@@ -276,63 +279,29 @@
         meas2 = physics.A(model(y + self.tau1 * b1, physics))
         meas2p = physics.A(model(y + self.tau2 * b2, physics))
         meas2n = physics.A(model(y - self.tau2 * b2, physics))
 
         # compute m (size of y)
         # m = (torch.abs(y) > 1e-5).flatten().sum()
 
-        loss_mc = (meas1 - y).pow(2).mean()
+        loss_mc = (meas1 - y).pow(2).reshape(y.size(0), -1).mean(1)
 
         loss_div1 = (
             2
             / self.tau1
-            * ((b1 * (self.gain * y + self.sigma2)) * (meas2 - meas1)).mean()
+            * ((b1 * (self.gain * y + self.sigma2)) * (meas2 - meas1))
+            .reshape(y.size(0), -1)
+            .mean(1)
         )
 
-        offset = -self.gain * y.mean() - self.sigma2
+        offset = -self.gain * y.reshape(y.size(0), -1).mean(1) - self.sigma2
 
         loss_div2 = (
             -2
             * self.sigma2
             * self.gain
             / (self.tau2**2)
-            * (b2 * (meas2p + meas2n - 2 * meas1)).mean()
+            * (b2 * (meas2p + meas2n - 2 * meas1)).reshape(y.size(0), -1).mean(1)
         )
 
         loss_sure = loss_mc + loss_div1 + loss_div2 + offset
         return loss_sure
-
-
-# if __name__ == "__main__":
-#     from deepinv.models import Denoiser
-#     import deepinv as dinv
-#
-#     model_spec = {
-#         "name": "waveletprior",
-#         "args": {"wv": "db8", "level": 3, "device": dinv.device},
-#     }
-#     f = dinv.models.ArtifactRemoval(Denoiser(model_spec))
-#     # test divergence
-#
-#     x = torch.ones((1, 3, 16, 16), device=dinv.device) * 0.5
-#     physics = dinv.physics.Denoising(dinv.physics.GaussianNoise(0.1))
-#     y = physics(x)
-#
-#     y1 = f(y, physics)
-#     tau = 1e-4
-#
-#     exact = exact_div(y, physics, f)
-#
-#     error_h = 0
-#     error_mc = 0
-#     for i in range(100):
-#         h = hutch_div(y, physics, f)
-#         mc = mc_div(y1, y, f, physics, tau)
-#
-#         error_h += torch.abs(h - exact)
-#         error_mc += torch.abs(mc - exact)
-#
-#     error_mc /= 100
-#     error_h /= 100
-#
-#     print(f"error_h: {error_h}")
-#     print(f"error_mc: {error_mc}")
```

### Comparing `deepinv-0.1.1/deepinv/loss/tv.py` & `deepinv-0.2.0/deepinv/loss/tv.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
-import torch.nn as nn
+from deepinv.loss.loss import Loss
 
 
-class TVLoss(nn.Module):
+class TVLoss(Loss):
     r"""
     Total variation loss (:math:`\ell_2` norm).
 
     It computes the loss :math:`\|D\hat{x}\|_2^2`,
     where :math:`D` is a normalized linear operator that computes the vertical and horizontal first order differences
     of the reconstructed image :math:`\hat{x}`.
 
@@ -19,21 +19,29 @@
         self.name = "tv"
 
     def forward(self, x_net, **kwargs):
         r"""
         Computes the TV loss.
 
         :param torch.Tensor x_net: reconstructed image.
-        :return: (torch.Tensor) loss.
+        :return: torch.nn.Tensor loss of size (batch_size,)
         """
         batch_size = x_net.size()[0]
         h_x = x_net.size()[2]
         w_x = x_net.size()[3]
         count_h = self.tensor_size(x_net[:, :, 1:, :])
         count_w = self.tensor_size(x_net[:, :, :, 1:])
-        h_tv = torch.pow((x_net[:, :, 1:, :] - x_net[:, :, : h_x - 1, :]), 2).sum()
-        w_tv = torch.pow((x_net[:, :, :, 1:] - x_net[:, :, :, : w_x - 1]), 2).sum()
-        return self.tv_loss_weight * 2 * (h_tv / count_h + w_tv / count_w) / batch_size
+        h_tv = (
+            torch.pow((x_net[:, :, 1:, :] - x_net[:, :, : h_x - 1, :]), 2)
+            .reshape(x_net.size(0), -1)
+            .sum(1)
+        )
+        w_tv = (
+            torch.pow((x_net[:, :, :, 1:] - x_net[:, :, :, : w_x - 1]), 2)
+            .reshape(x_net.size(0), -1)
+            .sum(1)
+        )
+        return self.tv_loss_weight * 2 * (h_tv / count_h + w_tv / count_w)
 
     @staticmethod
     def tensor_size(t):
         return t.size()[1] * t.size()[2] * t.size()[3]
```

### Comparing `deepinv-0.1.1/deepinv/models/GSPnP.py` & `deepinv-0.2.0/deepinv/models/GSPnP.py`

 * *Files 9% similar despite different names*

```diff
@@ -24,46 +24,44 @@
 
     def __init__(self, denoiser, alpha=1.0, train=False):
         super().__init__()
         self.student_grad = StudentGrad(denoiser)
         self.alpha = alpha
         self.train = train
 
-    def potential(self, x, sigma):
+    def potential(self, x, sigma, *args, **kwargs):
         N = self.student_grad(x, sigma)
         return (
             0.5
             * self.alpha
             * torch.norm((x - N).view(x.shape[0], -1), p=2, dim=-1) ** 2
         )
 
-    def potential_grad(self, x, sigma):
+    def potential_grad(self, x, sigma, *args, **kwargs):
         r"""
         Calculate :math:`\nabla g` the gradient of the regularizer :math:`g` at input :math:`x`.
 
-        :param torch.tensor x: Input image
+        :param torch.Tensor x: Input image
         :param float sigma: Denoiser level :math:`\sigma` (std)
         """
-        torch.set_grad_enabled(True)
-        x = x.float()
-        x = x.requires_grad_()
-        N = self.student_grad(x, sigma)
-        JN = torch.autograd.grad(
-            N, x, grad_outputs=x - N, create_graph=True, only_inputs=True
-        )[0]
-        if not self.train:
-            torch.set_grad_enabled(False)
+        with torch.enable_grad():
+            x = x.float()
+            x = x.requires_grad_()
+            N = self.student_grad(x, sigma)
+            JN = torch.autograd.grad(
+                N, x, grad_outputs=x - N, create_graph=True, only_inputs=True
+            )[0]
         Dg = x - N - JN
         return self.alpha * Dg
 
     def forward(self, x, sigma):
         r"""
         Denoising with Gradient Step Denoiser
 
-        :param torch.tensor x: Input image
+        :param torch.Tensor x: Input image
         :param float sigma: Denoiser level (std)
         """
         Dg = self.potential_grad(x, sigma)
         x_hat = x - Dg
         return x_hat
```

### Comparing `deepinv-0.1.1/deepinv/models/PDNet.py` & `deepinv-0.2.0/deepinv/models/PDNet.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/models/ae.py` & `deepinv-0.2.0/deepinv/models/ae.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/models/artifactremoval.py` & `deepinv-0.2.0/deepinv/models/artifactremoval.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                 v.requires_grad = False
             self.backbone_net = self.backbone_net.to(device)
 
     def forward(self, y, physics, **kwargs):
         r"""
         Reconstructs a signal estimate from measurements y
 
-        :param torch.tensor y: measurements
+        :param torch.Tensor y: measurements
         :param deepinv.physics.Physics physics: forward operator
         """
         if isinstance(physics, nn.DataParallel):
             physics = physics.module
 
         y_in = physics.A_adjoint(y) if not self.pinv else physics.A_dagger(y)
         if type(self.backbone_net).__name__ == "UNetRes":
```

### Comparing `deepinv-0.1.1/deepinv/models/bm3d.py` & `deepinv-0.2.0/deepinv/models/bm3d.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/models/diffunet.py` & `deepinv-0.2.0/deepinv/models/diffunet.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,24 +69,24 @@
         use_scale_shift_norm = True
         resblock_updown = True
         use_new_attention_order = False
 
         out_channels = 6 if out_channels == 3 else out_channels
         channel_mult = (1, 1, 2, 2, 4, 4)
 
-        image_size = 256
+        img_size = 256
         attention_ds = []
         for res in attention_resolutions.split(","):
-            attention_ds.append(image_size // int(res))
+            attention_ds.append(img_size // int(res))
         attention_resolutions = tuple(attention_ds)
 
         if num_heads_upsample == -1:
             num_heads_upsample = num_heads
 
-        self.image_size = image_size
+        self.img_size = img_size
         self.in_channels = in_channels
         self.model_channels = model_channels
         self.out_channels = out_channels
         self.num_res_blocks = num_res_blocks
         self.attention_resolutions = attention_resolutions
         self.dropout = dropout
         self.channel_mult = channel_mult
```

### Comparing `deepinv-0.1.1/deepinv/models/dip.py` & `deepinv-0.2.0/deepinv/models/dip.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,17 +92,17 @@
 
     This method is based on the paper `"Deep Image Prior" by Ulyanov et al. (2018)
     <https://arxiv.org/abs/1711.10925>`_, and reconstructs
     an image by minimizing the loss function
 
     .. math::
 
-        \min_{\theta}  \|y-Af_{\theta}(z)\|^2
+        \min_{\theta}  \|y-Ad_{\theta}(z)\|^2
 
-    where :math:`z` is a random input and :math:`f_{\theta}` is a convolutional decoder network with parameters
+    where :math:`z` is a random input and :math:`d_{\theta}` is a convolutional decoder network with parameters
     :math:`\theta`. The minimization should be stopped early to avoid overfitting. The method uses the Adam
     optimizer.
 
     .. note::
 
         This method only works with certain convolutional decoder networks. We recommend using the
         network :class:`deepinv.models.ConvDecoder`.
@@ -110,15 +110,15 @@
 
     .. note::
 
         The number of iterations and learning rate are set to the values used in the original paper. However, these
         values may not be optimal for all problems. We recommend experimenting with different values.
 
     :param torch.nn.Module generator: Convolutional decoder network.
-    :param list, tuple input_size: Size (C,H,W) of the input noise vector :math:`z`.
+    :param list, tuple input_size: Size `(C,H,W)` of the input noise vector :math:`z`.
     :param int iterations: Number of optimization iterations.
     :param float learning_rate: Learning rate of the Adam optimizer.
     :param bool verbose: If ``True``, print progress.
     :param bool re_init: If ``True``, re-initialize the network parameters before each reconstruction.
 
     """
```

### Comparing `deepinv-0.1.1/deepinv/models/dncnn.py` & `deepinv-0.2.0/deepinv/models/dncnn.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/models/drunet.py` & `deepinv-0.2.0/deepinv/models/drunet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Code borrowed from Kai Zhang https://github.com/cszn/DPIR/tree/master/models
 
 import numpy as np
 import torch
 import torch.nn as nn
-from .utils import get_weights_url
+from .utils import get_weights_url, test_onesplit, test_pad
 
 cuda = True if torch.cuda.is_available() else False
 Tensor = torch.cuda.FloatTensor if cuda else torch.FloatTensor
 
 
 class DRUNet(nn.Module):
     r"""
@@ -179,37 +179,33 @@
         Run the denoiser on image with noise level :math:`\sigma`.
 
         :param torch.Tensor x: noisy image
         :param float, torch.Tensor sigma: noise level. If ``sigma`` is a float, it is used for all images in the batch.
             If ``sigma`` is a tensor, it must be of shape ``(batch_size,)``.
         """
         if isinstance(sigma, torch.Tensor):
-            if len(sigma.size()) > 0:
+            if sigma.ndim > 0:
                 if x.get_device() > -1:
                     sigma = sigma[
                         int(x.get_device() * x.shape[0]) : int(
                             (x.get_device() + 1) * x.shape[0]
                         )
                     ]
                     noise_level_map = sigma.to(x.device).view(x.size(0), 1, 1, 1)
                 else:
                     noise_level_map = sigma.view(x.size(0), 1, 1, 1).to(x.device)
                 noise_level_map = noise_level_map.expand(-1, 1, x.size(2), x.size(3))
             else:
-                sigma = sigma.item()
-                noise_level_map = (
-                    torch.FloatTensor(x.size(0), 1, x.size(2), x.size(3))
-                    .fill_(sigma)
-                    .to(x.device)
-                )
+                noise_level_map = torch.ones(
+                    (x.size(0), 1, x.size(2), x.size(3)), device=x.device
+                ) * sigma[None, None, None, None].to(x.device)
         else:
             noise_level_map = (
-                torch.FloatTensor(x.size(0), 1, x.size(2), x.size(3))
-                .fill_(sigma)
-                .to(x.device)
+                torch.ones((x.size(0), 1, x.size(2), x.size(3)), device=x.device)
+                * sigma
             )
         x = torch.cat((x, noise_level_map), 1)
         if self.training or (
             x.size(2) % 8 == 0
             and x.size(3) % 8 == 0
             and x.size(2) > 31
             and x.size(3) > 31
@@ -625,65 +621,11 @@
         bias,
         mode=mode[1:],
         negative_slope=negative_slope,
     )
     return sequential(pool, pool_tail)
 
 
-"""
-Helpers for test time
-"""
-
-
-def test_onesplit(model, L, refield=32, sf=1):
-    """
-    Changes the size of the image to fit the model's expected image size.
-
-    :param model: model.
-    :param L: input Low-quality image.
-    :param refield: effective receptive field of the network, 32 is enough.
-    :param sf: scale factor for super-resolution, otherwise 1.
-    """
-    h, w = L.size()[-2:]
-    top = slice(0, (h // 2 // refield + 1) * refield)
-    bottom = slice(h - (h // 2 // refield + 1) * refield, h)
-    left = slice(0, (w // 2 // refield + 1) * refield)
-    right = slice(w - (w // 2 // refield + 1) * refield, w)
-    Ls = [
-        L[..., top, left],
-        L[..., top, right],
-        L[..., bottom, left],
-        L[..., bottom, right],
-    ]
-    Es = [model(Ls[i]) for i in range(4)]
-    b, c = Es[0].size()[:2]
-    E = torch.zeros(b, c, sf * h, sf * w).type_as(L)
-    E[..., : h // 2 * sf, : w // 2 * sf] = Es[0][..., : h // 2 * sf, : w // 2 * sf]
-    E[..., : h // 2 * sf, w // 2 * sf : w * sf] = Es[1][
-        ..., : h // 2 * sf, (-w + w // 2) * sf :
-    ]
-    E[..., h // 2 * sf : h * sf, : w // 2 * sf] = Es[2][
-        ..., (-h + h // 2) * sf :, : w // 2 * sf
-    ]
-    E[..., h // 2 * sf : h * sf, w // 2 * sf : w * sf] = Es[3][
-        ..., (-h + h // 2) * sf :, (-w + w // 2) * sf :
-    ]
-    return E
-
-
-def test_pad(model, L, modulo=16):
-    """
-    Pads the image to fit the model's expected image size.
-    """
-    h, w = L.size()[-2:]
-    padding_bottom = int(np.ceil(h / modulo) * modulo - h)
-    padding_right = int(np.ceil(w / modulo) * modulo - w)
-    L = torch.nn.ReplicationPad2d((0, padding_right, 0, padding_bottom))(L)
-    E = model(L)
-    E = E[..., :h, :w]
-    return E
-
-
 def weights_init_drunet(m):
     classname = m.__class__.__name__
     if classname.find("Conv") != -1:
         nn.init.orthogonal_(m.weight.data, gain=0.2)
```

### Comparing `deepinv-0.1.1/deepinv/models/equivariant.py` & `deepinv-0.2.0/deepinv/models/equivariant.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     if :math:`\denoisername(T_g(x)) = T_g(\denoisername(x))` for any image :math:`x` and any :math:`g\in \mathcal{G}`.
 
     The denoiser can be turned into an equivariant denoiser by averaging over the group of transforms, i.e.
 
     .. math::
         \operatorname{D}^{\text{eq}}_{\sigma}(x) = \frac{1}{|\mathcal{G}|}\sum_{g\in \mathcal{G}} T_g^{-1}(\operatorname{D}_{\sigma}(T_g(x))).
 
-    Otherwise, as proposed in <https://arxiv.org/abs/2312.01831>`_, a Monte-Carlo approximation can be obtained by
+    Otherwise, as proposed in https://arxiv.org/abs/2312.01831, a Monte Carlo approximation can be obtained by
     sampling :math:`g \sim \mathcal{G}` at random and applying
 
     .. math::
         \operatorname{D}^{\text{MC}}_{\sigma}(x) = T_g^{-1}(\operatorname{D}_{\sigma}(T_g(x))).
 
 
     :param callable denoiser: Denoiser :math:`\operatorname{D}_{\sigma}`.
```

### Comparing `deepinv-0.1.1/deepinv/models/median.py` & `deepinv-0.2.0/deepinv/models/median.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # code adapted from https://gist.github.com/rwightman/f2d3849281624be7c0f11c85c87c1598
 
 
 class MedianFilter(nn.Module):
     r"""
     Median filter.
 
+    It computes the median value of a sliding window over the input tensor. The window is defined by the kernel size.
 
     :param int kernel_size: size of pooling kernel, int or 2-tuple
     :param padding: pool padding, int or 4-tuple (l, r, t, b) as in pytorch F.pad
     :param same: override padding and enforce same padding, boolean
     """
 
     def __init__(self, kernel_size=9, padding=0, same=True):
```

### Comparing `deepinv-0.1.1/deepinv/models/scunet.py` & `deepinv-0.2.0/deepinv/models/scunet.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,15 +285,15 @@
     :param bool pretrained: use a pretrained network. If ``pretrained=None``, the weights will be initialized at random
         using Pytorch's default initialization. If ``pretrained='download'``, the weights will be downloaded from an
         online repository (only available for the default architecture).
         Finally, ``pretrained`` can also be set as a path to the user's own pretrained weights. Default: 'download'.
         See :ref:`pretrained-weights <pretrained-weights>` for more details.
     :param bool train: training or testing mode. Default: False.
     :param str device: gpu or cpu. Default: 'cpu'.
-    ....
+
     """
 
     def __init__(
         self,
         in_nc=3,
         config=[4, 4, 4, 4, 4, 4, 4],
         dim=64,
```

### Comparing `deepinv-0.1.1/deepinv/models/swinir.py` & `deepinv-0.2.0/deepinv/models/swinir.py`

 * *Files 0% similar despite different names*

```diff
@@ -789,38 +789,38 @@
 class SwinIR(nn.Module):
     r"""SwinIR denoising network.
 
     The Swin Image Restoration (SwinIR) denoising network was introduced in `SwinIR: Image Restoration Using Swin
     Transformer <https://arxiv.org/abs/2108.10257>`_. This code is adapted from the official implementation by the
     authors.
 
-    :param int|tuple img_size: Input image size. Default 128.
-    :param int|tuple patch_size: Patch size. Default: 1.
+    :param int, tuple img_size: Input image size. Default 128.
+    :param int, tuple patch_size: Patch size. Default: 1.
     :param int in_chans: Number of input image channels. Default: 3.
     :param int embed_dim: Patch embedding dimension. Default: 180.
     :param tuple depths: Depth of each Swin Transformer layer.
     :param tuple num_heads: Number of attention heads in different layers.
     :param int window_size: Window size. Default: 8.
     :param float mlp_ratio: Ratio of mlp hidden dim to embedding dim. Default: 2.
     :param bool qkv_bias: If True, add a learnable bias to query, key, value. Default: True.
     :param float qk_scale: Override default qk scale of head_dim ** -0.5 if set. Default: None.
     :param float drop_rate: Dropout rate. Default: 0.
     :param float attn_drop_rate: Attention dropout rate. Default: 0.
     :param float drop_path_rate: Stochastic depth rate. Default: 0.1.
-    :param nn.Module norm_layer: Normalization layer. Default: nn.LayerNorm.
+    :param torch.nn.Module norm_layer: Normalization layer. Default: nn.LayerNorm.
     :param bool ape: If True, add absolute position embedding to the patch embedding. Default: False.
     :param bool patch_norm: If True, add normalization after patch embedding. Default: True.
     :param bool use_checkpoint: Whether to use checkpointing to save memory. Default: False.
     :param int upscale: Upscale factor. 2/3/4/8 for image SR, 1 for denoising and compress artifact reduction
     :param float img_range: Image range. 1. or 255. Default: 1.
-    :param str|None upsampler: The reconstruction module. ''/'pixelshuffle'/'pixelshuffledirect'/'nearest+conv'/None.
+    :param str, None upsampler: The reconstruction module. ''/'pixelshuffle'/'pixelshuffledirect'/'nearest+conv'/None.
         Default: ''.
     :param str resi_connection: The convolutional block before residual connection. Should be either '1conv' or '3conv'.
         Default: '1conv'.
-    :param str|None pretrained: Use a pretrained network. If ``pretrained=None``, the weights will be initialized at
+    :param str, None pretrained: Use a pretrained network. If ``pretrained=None``, the weights will be initialized at
         random using PyTorch's default initialization. If ``pretrained='download'``, the weights will be downloaded from
         the authors' online repository https://github.com/JingyunLiang/SwinIR/releases/tag/v0.0 (only available for the
         default architecture). Finally, ``pretrained`` can also be set as a path to the user's own pretrained weights.
         Default: 'download'.
         See :ref:`pretrained-weights <pretrained-weights>` for more details.
     :param int pretrained_noise_level: The noise level of the pretrained model to be downloaded (in 0-255 scale). This
         value is directly concatenated to the download url; should be chosen in the set {15, 25, 50}. Default: 15.
@@ -1049,15 +1049,15 @@
     def no_weight_decay(self):
         return {"absolute_pos_embed"}
 
     @torch.jit.ignore
     def no_weight_decay_keywords(self):
         return {"relative_position_bias_table"}
 
-    def check_image_size(self, x):
+    def check_img_size(self, x):
         _, _, h, w = x.size()
         mod_pad_h = (self.window_size - h % self.window_size) % self.window_size
         mod_pad_w = (self.window_size - w % self.window_size) % self.window_size
         x = F.pad(x, (0, mod_pad_w, 0, mod_pad_h), "reflect")
         return x
 
     def forward_features(self, x):
@@ -1079,15 +1079,15 @@
         r"""
         Run the denoiser on noisy image. The noise level is not used in this denoiser.
 
         :param torch.Tensor x: noisy image, of shape B, C, W, H.
         :param float sigma: noise level (not used).
         """
         H, W = x.shape[2:]
-        x = self.check_image_size(x)
+        x = self.check_img_size(x)
 
         self.mean = self.mean.type_as(x)
         x = (x - self.mean) * self.img_range
 
         if self.upsampler == "pixelshuffle":
             # for classical SR
             x = self.conv_first(x)
```

### Comparing `deepinv-0.1.1/deepinv/models/tgv.py` & `deepinv-0.2.0/deepinv/models/tgv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import warnings
 import torch
 import torch.nn as nn
 
 from deepinv.models import TVDenoiser
 
 
 class TGVDenoiser(nn.Module):
@@ -33,17 +32,17 @@
         The regularization term :math:`\|r\|_{1,2} + \|J(Dx-r)\|_{1,F}` is implicitly normalized by its Lipschitz
         constant, i.e. :math:`\sqrt{72}`, see e.g. K. Bredies et al., "Total generalized variation," SIAM J. Imaging
         Sci., 3(3), 492-526, 2010.
 
     :param bool verbose: Whether to print computation details or not. Default: False.
     :param int n_it_max: Maximum number of iterations. Default: 1000.
     :param float crit: Convergence criterion. Default: 1e-5.
-    :param torch.tensor, None x2: Primary variable. Default: None.
-    :param torch.tensor, None u2: Dual variable. Default: None.
-    :param torch.tensor, None r2: Auxiliary variable. Default: None.
+    :param torch.Tensor, None x2: Primary variable. Default: None.
+    :param torch.Tensor, None u2: Dual variable. Default: None.
+    :param torch.Tensor, None r2: Auxiliary variable. Default: None.
     """
 
     def __init__(
         self, verbose=False, n_it_max=1000, crit=1e-5, x2=None, u2=None, r2=None
     ):
         super(TGVDenoiser, self).__init__()
```

### Comparing `deepinv-0.1.1/deepinv/models/tv.py` & `deepinv-0.2.0/deepinv/models/tv.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,29 +6,31 @@
     r"""
     Proximal operator of the isotropic Total Variation operator.
 
     This algorithm converges to the unique image :math:`x` that is the solution of
 
     .. math::
 
-        \underset{x}{\arg\min} \;  \frac{1}{2}\|x-y\|_2^2 + \lambda \|Dx\|_{1,2},
+        \underset{x}{\arg\min} \;  \frac{1}{2}\|x-y\|_2^2 + \gamma \|Dx\|_{1,2},
 
     where :math:`D` maps an image to its gradient field.
 
     The problem is solved with an over-relaxed Chambolle-Pock algorithm (see L. Condat, "A primal-dual splitting method
     for convex optimization  involving Lipschitzian, proximable and linear composite terms", J. Optimization Theory and
     Applications, vol. 158, no. 2, pp. 460-479, 2013.
 
     Code (and description) adapted from Laurent Condat's matlab version (https://lcondat.github.io/software.html) and
     Daniil Smolyakov's `code <https://github.com/RoundedGlint585/TGVDenoising/blob/master/TGV%20WithoutHist.ipynb>`_.
 
     This algorithm is implemented with warm restart, i.e. the primary and dual variables are kept in memory
     between calls to the forward method. This speeds up the computation when using this class in an iterative algorithm.
 
     :param bool verbose: Whether to print computation details or not. Default: False.
+    :param float tau: Stepsize for the primal update. Default: 0.01.
+    :param float rho: Over-relaxation parameter. Default: 1.99.
     :param int n_it_max: Maximum number of iterations. Default: 1000.
     :param float crit: Convergence criterion. Default: 1e-5.
     :param torch.Tensor, None x2: Primary variable for warm restart. Default: None.
     :param torch.Tensor, None u2: Dual variable for warm restart. Default: None.
 
     .. note::
         The regularization term :math:`\|Dx\|_{1,2}` is implicitly normalized by its Lipschitz constant, i.e.
@@ -39,37 +41,41 @@
         For using TV as a prior for Plug and Play algorithms, it is recommended to use the class
         :class:`~deepinv.optim.prior.TVPrior` instead. In particular, it allows to evaluate TV.
     """
 
     def __init__(
         self,
         verbose=False,
+        tau=0.01,
+        rho=1.99,
         n_it_max=1000,
         crit=1e-5,
         x2=None,
         u2=None,
     ):
         super(TVDenoiser, self).__init__()
 
         self.verbose = verbose
         self.n_it_max = n_it_max
         self.crit = crit
         self.restart = True
 
-        self.tau = 0.01  # > 0
-
-        self.rho = 1.99  # in 1,2
+        self.tau = tau
+        self.rho = rho
         self.sigma = 1 / self.tau / 8
 
         self.x2 = x2
         self.u2 = u2
 
         self.has_converged = False
 
     def prox_tau_fx(self, x, y):
+        r"""
+        Proximal operator of the function :math:`\frac{1}{2}\|x-y\|_2^2`.
+        """
         return (x + self.tau * y) / (1 + self.tau)
 
     def prox_sigma_g_conj(self, u, lambda2):
         return u / (
             torch.maximum(
                 torch.sqrt(torch.sum(u**2, axis=-1)) / lambda2,
                 torch.tensor([1], device=u.device).type(u.dtype),
@@ -77,53 +83,61 @@
         )
 
     def forward(self, y, ths=None):
         r"""
         Computes the proximity operator of the TV norm.
 
         :param torch.Tensor y: Noisy image.
-        :param float, torch.Tensor ths: Regularization parameter.
+        :param float, torch.Tensor ths: Regularization parameter :math:`\gamma`.
         :return: Denoised image.
         """
+
         restart = (
             True
-            if (self.restart or self.x2 is None or self.x2.shape != y.shape)
+            if (
+                self.restart
+                or self.x2 is None
+                or self.u2 is None
+                or self.x2.shape != y.shape
+            )
             else False
         )
 
         if restart:
-            self.x2 = y.clone()
-            self.u2 = torch.zeros((*self.x2.shape, 2), device=self.x2.device).type(
-                self.x2.dtype
-            )
+            x2 = y.clone()
+            u2 = torch.zeros((*y.shape, 2), device=y.device).type(y.dtype)
             self.restart = False
+        else:
+            x2 = self.x2.clone()
+            u2 = self.u2.clone()
 
         if ths is not None:
             lambd = ths
 
         for _ in range(self.n_it_max):
-            x_prev = self.x2.clone()
+            x_prev = x2
 
-            x = self.prox_tau_fx(self.x2 - self.tau * self.nabla_adjoint(self.u2), y)
-            u = self.prox_sigma_g_conj(
-                self.u2 + self.sigma * self.nabla(2 * x - self.x2), lambd
-            )
-            self.x2 = self.x2 + self.rho * (x - self.x2)
-            self.u2 = self.u2 + self.rho * (u - self.u2)
+            x = self.prox_tau_fx(x2 - self.tau * self.nabla_adjoint(u2), y)
+            u = self.prox_sigma_g_conj(u2 + self.sigma * self.nabla(2 * x - x2), lambd)
+            x2 = x2 + self.rho * (x - x2)
+            u2 = u2 + self.rho * (u - u2)
 
             rel_err = torch.linalg.norm(
-                x_prev.flatten() - self.x2.flatten()
-            ) / torch.linalg.norm(self.x2.flatten() + 1e-12)
+                x_prev.flatten() - x2.flatten()
+            ) / torch.linalg.norm(x2.flatten() + 1e-12)
 
             if _ > 1 and rel_err < self.crit:
                 if self.verbose:
                     print("TV prox reached convergence")
                 break
 
-        return self.x2
+        self.x2 = x2.detach()
+        self.u2 = u2.detach()
+
+        return x2
 
     @staticmethod
     def nabla(x):
         r"""
         Applies the finite differences operator associated with tensors of the same shape as x.
         """
         b, c, h, w = x.shape
```

### Comparing `deepinv-0.1.1/deepinv/models/unet.py` & `deepinv-0.2.0/deepinv/models/unet.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,29 +53,30 @@
 
 
 class UNet(nn.Module):
     r"""
     U-Net convolutional denoiser.
 
     This network is a fully convolutional denoiser based on the U-Net architecture. The number of downsample steps
-    can be controlled with the `scales` parameter. The number of trainable parameters increases with the number of
+    can be controlled with the ``scales`` parameter. The number of trainable parameters increases with the number of
     scales.
 
     .. warning::
-        When using the bias-free batch norm `BFBatchNorm2d` via `batch_norm=biasfree`, NaNs may be encountered
+        When using the bias-free batch norm ``BFBatchNorm2d`` via ``batch_norm="biasfree"``, NaNs may be encountered
         during training, causing the whole training procedure to fail.
 
     :param int in_channels: input image channels
     :param int out_channels: output image channels
     :param bool residual: use a skip-connection between output and output.
     :param bool circular_padding: circular padding for the convolutional layers.
     :param bool cat: use skip-connections between intermediate levels.
     :param bool bias: use learnable biases.
-    :param bool|str batch_norm: if False, no batchnorm applied, if True, use `nn.BatchNorm2d`, if `biasfree`, use
-        `BFBatchNorm2d` from `"Robust And Interpretable Blind Image Denoising Via Bias-Free Convolutional Neural Networks" by Mohan et al. <https://arxiv.org/abs/1906.05478>`_.
+    :param bool, str batch_norm: if False, no batchnorm applied, if ``True``, use :meth:`torch.nn.BatchNorm2d`,
+        if ``batch_norm="biasfree"``, use ``BFBatchNorm2d`` from
+        `"Robust And Interpretable Blind Image Denoising Via Bias-Free Convolutional Neural Networks" by Mohan et al. <https://arxiv.org/abs/1906.05478>`_.
     :param int scales: Number of downsampling steps used in the U-Net. The options are 2,3,4 and 5.
         The number of trainable parameters increases with the scale.
     """
 
     def __init__(
         self,
         in_channels=1,
```

### Comparing `deepinv-0.1.1/deepinv/models/wavdict.py` & `deepinv-0.2.0/deepinv/models/wavdict.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 
 try:
     import ptwt
 except:
     ptwt = ImportError("The ptwt package is not installed.")
 
 
-class WaveletPrior(nn.Module):
+class WaveletDenoiser(nn.Module):
     r"""
-    Wavelet denoising with the :math:`\ell_1` norm.
+    Orthogonal Wavelet denoising with the :math:`\ell_1` norm.
 
 
     This denoiser is defined as the solution to the optimization problem:
 
     .. math::
 
-        \underset{x}{\arg\min} \;  \|x-y\|^2 + \lambda \|\Psi x\|_n
+        \underset{x}{\arg\min} \;  \|x-y\|^2 + \gamma \|\Psi x\|_n
 
     where :math:`\Psi` is an orthonormal wavelet transform, :math:`\lambda>0` is a hyperparameter, and where
     :math:`\|\cdot\|_n` is either the :math:`\ell_1` norm (``non_linearity="soft"``) or
     the :math:`\ell_0` norm (``non_linearity="hard"``). A variant of the :math:`\ell_0` norm is also available
     (``non_linearity="topk"``), where the thresholding is done by keeping the :math:`k` largest coefficients
     in each wavelet subband and setting the others to zero.
 
@@ -38,15 +38,15 @@
     :param str non_linearity: ``"soft"``, ``"hard"`` or ``"topk"`` thresholding (default: ``"soft"``).
         If ``"topk"``, only the top-k wavelet coefficients are kept.
     """
 
     def __init__(self, level=3, wv="db8", device="cpu", non_linearity="soft", wvdim=2):
         if isinstance(ptwt, ImportError):
             raise ImportError(
-                "pytorch_wavelets is needed to use the WaveletPrior class. "
+                "pytorch_wavelets is needed to use the WaveletDenoiser class. "
                 "It should be installed with `pip install ptwt`."
             ) from ptwt
         super().__init__()
         self.level = level
         self.wv = wv
         self.device = device
         self.non_linearity = non_linearity
@@ -75,14 +75,29 @@
         elif self.dimension == 3:
             flat = torch.hstack(
                 [dec[0].flatten()]
                 + [dec[l][key].flatten() for l in range(1, len(dec)) for key in dec[l]]
             )
         return flat
 
+    @staticmethod
+    def psi(x, wavelet="db2", level=2, dimension=2):
+        r"""
+        Returns a flattened list containing the wavelet coefficients.
+        """
+        if dimension == 2:
+            dec = ptwt.wavedec2(x, pywt.Wavelet(wavelet), mode="zero", level=level)
+            dec = [list(t) if isinstance(t, tuple) else t for t in dec]
+            vec = [decl.flatten() for l in range(1, len(dec)) for decl in dec[l]]
+        elif dimension == 3:
+            dec = ptwt.wavedec3(x, pywt.Wavelet(wavelet), mode="zero", level=level)
+            dec = [list(t) if isinstance(t, tuple) else t for t in dec]
+            vec = [dec[l][key].flatten() for l in range(1, len(dec)) for key in dec[l]]
+        return vec
+
     def iwt(self, coeffs):
         r"""
         Applies the wavelet recomposition.
         """
         coeffs = [tuple(t) if isinstance(t, list) else t for t in coeffs]
         if self.dimension == 2:
             rec = ptwt.waverec2(coeffs, pywt.Wavelet(self.wv))
@@ -93,18 +108,19 @@
     def prox_l1(self, x, ths=0.1):
         r"""
         Soft thresholding of the wavelet coefficients.
 
         :param torch.Tensor x: wavelet coefficients.
         :param float, torch.Tensor ths: threshold.
         """
-        ths_map = ths
         return torch.maximum(
-            torch.tensor([0], device=x.device).type(x.dtype), x - ths_map
-        ) + torch.minimum(torch.tensor([0], device=x.device).type(x.dtype), x + ths_map)
+            torch.tensor([0], device=x.device).type(x.dtype), x - abs(ths)
+        ) + torch.minimum(
+            torch.tensor([0], device=x.device).type(x.dtype), x + abs(ths)
+        )
 
     def prox_l0(self, x, ths=0.1):
         r"""
         Hard thresholding of the wavelet coefficients.
 
         :param torch.Tensor x: wavelet coefficients.
         :param float, torch.Tensor ths: threshold.
@@ -227,16 +243,17 @@
         return out
 
     def reshape_ths(self, ths, level):
         r"""
         Reshape the thresholding parameter in the appropriate format, i.e. either:
          - a list of 3 elements, or
          - a tensor of 3 elements.
-         Since the approximation coefficients are not thresholded, we do not need to provide a thresholding parameter,
-         ths has shape (n_levels-1, 3).
+
+        Since the approximation coefficients are not thresholded, we do not need to provide a thresholding parameter,
+        ths has shape (n_levels-1, 3).
         """
         numel = 3 if self.dimension == 2 else 7
         if not torch.is_tensor(ths):
             if isinstance(ths, int) or isinstance(ths, float):
                 ths_cur = [ths] * numel
             elif len(ths) == 1:
                 ths_cur = [ths[0]] * numel
@@ -253,15 +270,16 @@
         return ths_cur
 
     def forward(self, x, ths=0.1):
         r"""
         Run the model on a noisy image.
 
         :param torch.Tensor x: noisy image.
-        :param int, float, torch.Tensor ths: thresholding parameter. If `ths` is a tensor, it should be of shape
+        :param int, float, torch.Tensor ths: thresholding parameter :math:`\gamma`.
+            If `ths` is a tensor, it should be of shape
             ``(1, )`` (same coefficent for all levels), ``(n_levels-1, )`` (one coefficient per level),
             or ``(n_levels-1, 3)`` (one coefficient per subband and per level).
             If ``non_linearity`` equals ``"soft"`` or ``"hard"``, ``ths`` serves as a (soft or hard)
             thresholding parameter for the wavelet coefficients. If ``non_linearity`` equals ``"topk"``,
             ``ths`` can indicate the number of wavelet coefficients
             that are kept (if ``int``) or the proportion of coefficients that are kept (if ``float``).
 
@@ -279,29 +297,29 @@
         y = self.iwt(coeffs)
 
         # Crop data
         y = self.crop_output(y, padding)
         return y
 
 
-class WaveletDict(nn.Module):
+class WaveletDictDenoiser(nn.Module):
     r"""
     Overcomplete Wavelet denoising with the :math:`\ell_1` norm.
 
     This denoiser is defined as the solution to the optimization problem:
 
     .. math::
 
         \underset{x}{\arg\min} \;  \|x-y\|^2 + \lambda \|\Psi x\|_n
 
     where :math:`\Psi` is an overcomplete wavelet transform, composed of 2 or more wavelets, i.e.,
     :math:`\Psi=[\Psi_1,\Psi_2,\dots,\Psi_L]`, :math:`\lambda>0` is a hyperparameter, and where
     :math:`\|\cdot\|_n` is either the :math:`\ell_1` norm (``non_linearity="soft"``),
     the :math:`\ell_0` norm (``non_linearity="hard"``) or a variant of the :math:`\ell_0` norm
-    (``non_linearity="topk"``) where only the top-k coefficients are kept; see :meth:`deepinv.models.WaveletPrior` for
+    (``non_linearity="topk"``) where only the top-k coefficients are kept; see :meth:`deepinv.models.WaveletDenoiser` for
     more details.
 
     The solution is not available in closed-form, thus the denoiser runs an optimization algorithm for each test image.
 
     :param int level: decomposition level of the wavelet transform.
     :param list[str] wv: list of mother wavelets. The names of the wavelets can be found in `here
         <https://wavelets.pybytes.com/>`_. (default: ["db8", "db4"]).
@@ -318,15 +336,15 @@
         non_linearity="soft",
         wvdim=2,
     ):
         super().__init__()
         self.level = level
         self.list_prox = nn.ModuleList(
             [
-                WaveletPrior(
+                WaveletDenoiser(
                     level=level, wv=wv, non_linearity=non_linearity, wvdim=wvdim
                 )
                 for wv in list_wv
             ]
         )
         self.max_iter = max_iter
```

### Comparing `deepinv-0.1.1/deepinv/optim/data_fidelity.py` & `deepinv-0.2.0/deepinv/optim/data_fidelity.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,46 +2,47 @@
 import torch.nn as nn
 
 from deepinv.optim.utils import gradient_descent
 
 
 class DataFidelity(nn.Module):
     r"""
-    Data fidelity term :math:`\datafid{x}{y}=\distance{Ax}{y}`.
+    Data fidelity term :math:`\datafid{x}{y}=\distance{\forw{x}}{y}`.
 
-    This is the base class for the data fidelity term :math:`\datafid{x}{y} = \distance{A(x)}{y}` where :math:`A` is a
+    This is the base class for the data fidelity term :math:`\datafid{x}{y} = \distance{\forw{x}}{y}` where :math:`A` is a
     linear or nonlinear operator, :math:`x\in\xset` is a variable , :math:`y\in\yset` is the observation and
     :math:`\distancename` is a distance function.
 
-    ::
-
-        # define a loss function
-        data_fidelity = L2()
-
-        # Create a measurement operator
-        A = torch.Tensor([[2, 0], [0, 0.5]])
-        A_forward = lambda v: A @ v
-        A_adjoint = lambda v: A.transpose(0, 1) @ v
-
-        # Define the physics model associated to this operator
-        physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
-
-        # Define two points
-        x = torch.Tensor([[1], [4]]).unsqueeze(0)
-        y = torch.Tensor([[1], [1]]).unsqueeze(0)
-
-        # Compute the loss :math:`f(x) = \datafid{A(x)}{y}`
-        f_x = data_fidelity(x, y, physics)  # print(f_x) gives tensor([1.0000])
-
-        # Compute the gradient of :math:`f`
-        grad = data_fidelity.grad(x, y, physics)  # print(grad) gives tensor([[[2.0000], [0.5000]]])
-
-        # Compute the proximity operator of :math:`f`
-        prox = data_fidelity.prox(x, y, physics, gamma=1.0)  # print(prox) gives tensor([[[0.6000], [3.6000]]])
+    .. doctest::
 
+        >>> import torch
+        >>> import deepinv as dinv
+        >>> # define a loss function
+        >>> data_fidelity = dinv.optim.L2()
+        >>>
+        >>> # Create a measurement operator
+        >>> A = torch.Tensor([[2, 0], [0, 0.5]])
+        >>> A_forward = lambda v: A @ v
+        >>> A_adjoint = lambda v: A.transpose(0, 1) @ v
+        >>>
+        >>> # Define the physics model associated to this operator
+        >>> physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
+        >>>
+        >>> # Define two points
+        >>> x = torch.Tensor([[1], [4]]).unsqueeze(0)
+        >>> y = torch.Tensor([[1], [1]]).unsqueeze(0)
+        >>>
+        >>> # Compute the loss :math:`f(x) = \datafid{A(x)}{y}`
+        >>> data_fidelity(x, y, physics)
+        tensor([1.0000])
+        >>> # Compute the gradient of :math:`f`
+        >>> grad = data_fidelity.grad(x, y, physics)
+        >>>
+        >>> # Compute the proximity operator of :math:`f`
+        >>> prox = data_fidelity.prox(x, y, physics, gamma=1.0)
 
     .. warning::
         All variables have a batch dimension as first dimension.
 
     :param callable d: data fidelity distance function :math:`\distance{u}{y}`. Outputs a tensor of size `B`, the size of the batch. Default: None.
     """
 
@@ -49,28 +50,28 @@
         super().__init__()
         self._d = d
 
     def d(self, u, y, *args, **kwargs):
         r"""
         Computes the data fidelity distance :math:`\distance{u}{y}`.
 
-        :param torch.tensor u: Variable :math:`u` at which the distance function is computed.
-        :param torch.tensor y: Data :math:`y`.
-        :return: (torch.tensor) data fidelity :math:`\distance{u}{y}`.
+        :param torch.Tensor u: Variable :math:`u` at which the distance function is computed.
+        :param torch.Tensor y: Data :math:`y`.
+        :return: (torch.Tensor) data fidelity :math:`\distance{u}{y}`.
         """
         return self._d(u, y, *args, **kwargs)
 
     def grad_d(self, u, y, *args, **kwargs):
         r"""
         Computes the gradient :math:`\nabla_u\distance{u}{y}`, computed in :math:`u`. Note that this is the gradient of
         :math:`\distancename` and not :math:`\datafidname`. By default, the gradient is computed using automatic differentiation.
 
-        :param torch.tensor u: Variable :math:`u` at which the gradient is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`u`.
-        :return: (torch.tensor) gradient of :math:`d` in :math:`u`, i.e. :math:`\nabla_u\distance{u}{y}`.
+        :param torch.Tensor u: Variable :math:`u` at which the gradient is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`u`.
+        :return: (torch.Tensor) gradient of :math:`d` in :math:`u`, i.e. :math:`\nabla_u\distance{u}{y}`.
         """
         with torch.enable_grad():
             u = u.requires_grad_()
             grad = torch.autograd.grad(
                 self.d(u, y, *args, **kwargs), u, create_graph=True, only_inputs=True
             )[0]
         return grad
@@ -86,48 +87,56 @@
         tol_inter=1e-3,
         **kwargs,
     ):
         r"""
         Computes the proximity operator :math:`\operatorname{prox}_{\gamma\distance{\cdot}{y}}(u)`, computed in :math:`u`. Note
         that this is the proximity operator of :math:`\distancename` and not :math:`\datafidname`. By default, the proximity operator is computed using internal gradient descent.
 
-        :param torch.tensor u: Variable :math:`u` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`u`.
+        :param torch.Tensor u: Variable :math:`u` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`u`.
         :param float gamma: stepsize of the proximity operator.
         :param float stepsize_inter: stepsize used for internal gradient descent
         :param int max_iter_inter: maximal number of iterations for internal gradient descent.
         :param float tol_inter: internal gradient descent has converged when the L2 distance between two consecutive iterates is smaller than tol_inter.
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma\distance{\cdot}{y}}(u)`.
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma\distance{\cdot}{y}}(u)`.
         """
         grad = lambda z: gamma * self.grad_d(z, y, *args, **kwargs) + (z - u)
         return gradient_descent(
             grad, u, step_size=stepsize_inter, max_iter=max_iter_inter, tol=tol_inter
         )
 
     def forward(self, x, y, physics, *args, **kwargs):
         r"""
-        Computes the data fidelity term :math:`\datafid{x}{y} = \distance{Ax}{y}`.
+        Computes the data fidelity term :math:`\datafid{x}{y} = \distance{\forw{x}}{y}`.
 
-        :param torch.tensor x: Variable :math:`x` at which the data fidelity is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor x: Variable :math:`x` at which the data fidelity is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param deepinv.physics.Physics physics: physics model.
-        :return: (torch.tensor) data fidelity :math:`\datafid{x}{y}`.
+        :return: (torch.Tensor) data fidelity :math:`\datafid{x}{y}`.
         """
         return self.d(physics.A(x), y, *args, **kwargs)
 
     def grad(self, x, y, physics, *args, **kwargs):
         r"""
         Calculates the gradient of the data fidelity term :math:`\datafidname` at :math:`x`.
 
-        :param torch.tensor x: Variable :math:`x` at which the gradient is computed.
-        :param torch.tensor y: Data :math:`y`.
+        The gradient is computed using the chain rule:
+
+        .. math::
+
+            \nabla_x \distance{\forw{x}}{y} = \left. \frac{\partial A}{\partial x} \right|_x^\top \nabla_u \distance{u}{y},
+
+        where :math:`\left. \frac{\partial A}{\partial x} \right|_x` is the Jacobian of :math:`A` at :math:`x`, and :math:`\nabla_u \distance{u}{y}` is computed using ``grad_d`` with :math:`u = \forw{x}`. The multiplication is computed using the ``A_vjp`` method of the physics.
+
+        :param torch.Tensor x: Variable :math:`x` at which the gradient is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param deepinv.physics.Physics physics: physics model.
-        :return: (torch.tensor) gradient :math:`\nabla_x\datafid{x}{y}`, computed in :math:`x`.
+        :return: (torch.Tensor) gradient :math:`\nabla_x \datafid{x}{y}`, computed in :math:`x`.
         """
-        return physics.A_adjoint(self.grad_d(physics.A(x), y, *args, **kwargs))
+        return physics.A_vjp(x, self.grad_d(physics.A(x), y, *args, **kwargs))
 
     def prox(
         self,
         x,
         y,
         physics,
         *args,
@@ -136,22 +145,22 @@
         max_iter_inter=50,
         tol_inter=1e-3,
         **kwargs,
     ):
         r"""
         Calculates the proximity operator of :math:`\datafidname` at :math:`x`.
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param deepinv.physics.Physics physics: physics model.
         :param float gamma: stepsize of the proximity operator.
         :param float stepsize_inter: stepsize used for internal gradient descent
         :param int max_iter_inter: maximal number of iterations for internal gradient descent.
         :param float tol_inter: internal gradient descent has converged when the L2 distance between two consecutive iterates is smaller than tol_inter.
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma \datafidname}(x)`, computed in :math:`x`.
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma \datafidname}(x)`, computed in :math:`x`.
         """
         grad = lambda z: gamma * self.grad(z, y, physics, *args, **kwargs) + (z - x)
         return gradient_descent(
             grad, x, step_size=stepsize_inter, max_iter=max_iter_inter, tol=tol_inter
         )
 
     def prox_conjugate(self, x, y, physics, *args, gamma=1.0, lamb=1.0, **kwargs):
@@ -159,20 +168,20 @@
         Calculates the proximity operator of the convex conjugate :math:`(\lambda \datafidname)^*` at :math:`x`,
         using the Moreau formula.
 
         .. warning::
 
             This function is only valid for convex :math:`\datafidname`.
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param deepinv.physics.Physics physics: physics model.
         :param float gamma: stepsize of the proximity operator.
         :param float lamb: math:`\lambda` parameter in front of :math:`f`
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma (\lambda \datafidname)^*}(x)`,
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma (\lambda \datafidname)^*}(x)`,
             computed in :math:`x`.
         """
         return x - gamma * self.prox(
             x / gamma, y, physics, *args, gamma=lamb / gamma, **kwargs
         )
 
     def prox_d_conjugate(self, u, y, *args, gamma=1.0, lamb=1.0, **kwargs):
@@ -180,65 +189,66 @@
         Calculates the proximity operator of the convex conjugate :math:`(\lambda \distancename)^*` at :math:`u`,
         using the Moreau formula.
 
         .. warning::
 
             This function is only valid for convex :math:`\distancename`.
 
-        :param torch.tensor u: Variable :math:`u` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor u: Variable :math:`u` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param float gamma: stepsize of the proximity operator.
         :param float lamb: math:`\lambda` parameter in front of :math:`\distancename`
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma (\lambda \distancename)^*}(x)`,
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma (\lambda \distancename)^*}(x)`,
             computed in :math:`x`.
         """
         return u - gamma * self.prox_d(
             u / gamma, y, *args, gamma=lamb / gamma, **kwargs
         )
 
 
 class L2(DataFidelity):
     r"""
     Implementation of :math:`\distancename` as the normalized :math:`\ell_2` norm
 
     .. math::
 
-        f(x) = \frac{1}{2\sigma^2}\|Ax-y\|^2
+        f(x) = \frac{1}{2\sigma^2}\|\forw{x}-y\|^2
 
     It can be used to define a log-likelihood function associated with additive Gaussian noise
     by setting an appropriate noise level :math:`\sigma`.
 
     :param float sigma: Standard deviation of the noise to be used as a normalisation factor.
 
 
-    ::
-
-        # define a loss function
-        loss = L2()
-
-        # create a measurement operator
-        A = torch.Tensor([[2, 0], [0, 0.5]])
-        A_forward = lambda v:A@v
-        A_adjoint = lambda v: A.transpose(0,1)@v
-
-        # Define the physics model associated to this operator
-        physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
+    .. doctest::
 
-        # Define two points
-        x = torch.Tensor([1, 4])
-        y = torch.Tensor([1, 1])
-
-        # Compute the loss f(Ax, y)
-        f = loss(x, y, physics)  # print f gives 1.0
-
-        # Compute the gradient of f
-        grad_dA = data_fidelity.grad(x, y, physics)  # print grad_d gives [2.0000, 0.5000]
-
-        # Compute the proximity operator of f
-        prox_dA = data_fidelity.prox(x, y, physics, gamma=1.0)  # print prox_dA gives [0.6000, 3.6000]
+        >>> import torch
+        >>> import deepinv as dinv
+        >>> # define a loss function
+        >>> fidelity = dinv.optim.L2()
+        >>>
+        >>> x = torch.ones(1, 1, 3, 3)
+        >>> mask = torch.ones_like(x)
+        >>> mask[0, 0, 1, 1] = 0
+        >>> physics = dinv.physics.Inpainting(tensor_size=(1, 1, 3, 3), mask = mask)
+        >>> y = physics(x)
+        >>>
+        >>> # Compute the data fidelity f(Ax, y)
+        >>> fidelity(x, y, physics)
+        tensor([0.])
+        >>> # Compute the gradient of f
+        >>> fidelity.grad(x, y, physics)
+        tensor([[[[[0., 0., 0.],
+                   [0., 0., 0.],
+                   [0., 0., 0.]]]]])
+        >>> # Compute the proximity operator of f
+        >>> fidelity.prox(x, y, physics, gamma=1.0)
+        tensor([[[[[1., 1., 1.],
+                   [1., 1., 1.],
+                   [1., 1., 1.]]]]])
     """
 
     def __init__(self, sigma=1.0):
         super().__init__()
 
         self.norm = 1 / (sigma**2)
 
@@ -247,52 +257,52 @@
         Computes the data fidelity distance :math:`\datafid{u}{y}`, i.e.
 
         .. math::
 
             \datafid{u}{y} = \frac{1}{2\sigma^2}\|u-y\|^2
 
 
-        :param torch.tensor u: Variable :math:`u` at which the data fidelity is computed.
-        :param torch.tensor y: Data :math:`y`.
-        :return: (torch.tensor) data fidelity :math:`\datafid{u}{y}` of size `B` with `B` the size of the batch.
+        :param torch.Tensor u: Variable :math:`u` at which the data fidelity is computed.
+        :param torch.Tensor y: Data :math:`y`.
+        :return: (torch.Tensor) data fidelity :math:`\datafid{u}{y}` of size `B` with `B` the size of the batch.
         """
         x = u - y
         d = 0.5 * torch.norm(x.view(x.shape[0], -1), p=2, dim=-1) ** 2
         return self.norm * d
 
     def grad_d(self, u, y):
         r"""
         Computes the gradient of :math:`\distancename`, that is  :math:`\nabla_{u}\distance{u}{y}`, i.e.
 
         .. math::
 
             \nabla_{u}\distance{u}{y} = \frac{1}{\sigma^2}(u-y)
 
 
-        :param torch.tensor u: Variable :math:`u` at which the gradient is computed.
-        :param torch.tensor y: Data :math:`y`.
-        :return: (torch.tensor) gradient of the distance function :math:`\nabla_{u}\distance{u}{y}`.
+        :param torch.Tensor u: Variable :math:`u` at which the gradient is computed.
+        :param torch.Tensor y: Data :math:`y`.
+        :return: (torch.Tensor) gradient of the distance function :math:`\nabla_{u}\distance{u}{y}`.
         """
         return self.norm * (u - y)
 
     def prox_d(self, x, y, gamma=1.0):
         r"""
         Proximal operator of :math:`\gamma \distance{x}{y} = \frac{\gamma}{2\sigma^2}\|x-y\|^2`.
 
         Computes :math:`\operatorname{prox}_{\gamma \distancename}`, i.e.
 
         .. math::
 
            \operatorname{prox}_{\gamma \distancename} = \underset{u}{\text{argmin}} \frac{\gamma}{2\sigma^2}\|u-y\|_2^2+\frac{1}{2}\|u-x\|_2^2
 
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param float gamma: thresholding parameter.
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma \distancename}(x)`.
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma \distancename}(x)`.
         """
         gamma_ = self.norm * gamma
         return (x + gamma_ * y) / (1 + gamma_)
 
     def prox(self, x, y, physics, gamma=1.0):
         r"""
         Proximal operator of :math:`\gamma \datafid{Ax}{y} = \frac{\gamma}{2\sigma^2}\|Ax-y\|^2`.
@@ -300,19 +310,19 @@
         Computes :math:`\operatorname{prox}_{\gamma \datafidname}`, i.e.
 
         .. math::
 
            \operatorname{prox}_{\gamma \datafidname} = \underset{u}{\text{argmin}} \frac{\gamma}{2\sigma^2}\|Au-y\|_2^2+\frac{1}{2}\|u-x\|_2^2
 
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y`.
         :param deepinv.physics.Physics physics: physics model.
         :param float gamma: stepsize of the proximity operator.
-        :return: (torch.tensor) proximity operator :math:`\operatorname{prox}_{\gamma \datafidname}(x)`.
+        :return: (torch.Tensor) proximity operator :math:`\operatorname{prox}_{\gamma \datafidname}(x)`.
         """
         return physics.prox_l2(x, y, self.norm * gamma)
 
 
 class IndicatorL2(DataFidelity):
     r"""
     Indicator of :math:`\ell_2` ball with radius :math:`r`.
@@ -338,18 +348,18 @@
         super().__init__()
         self.radius = radius
 
     def d(self, u, y, radius=None):
         r"""
         Computes the batched indicator of :math:`\ell_2` ball with radius `radius`, i.e. :math:`\iota_{\mathcal{B}(y,r)}(u)`.
 
-        :param torch.tensor u: Variable :math:`u` at which the indicator is computed. :math:`u` is assumed to be of shape (B, ...) where B is the batch size.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`u`.
+        :param torch.Tensor u: Variable :math:`u` at which the indicator is computed. :math:`u` is assumed to be of shape (B, ...) where B is the batch size.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`u`.
         :param float radius: radius of the :math:`\ell_2` ball. If `radius` is None, the radius of the ball is set to `self.radius`. Default: None.
-        :return: (torch.tensor) indicator of :math:`\ell_2` ball with radius `radius`. If the point is inside the ball, the output is 0, else it is 1e16.
+        :return: (torch.Tensor) indicator of :math:`\ell_2` ball with radius `radius`. If the point is inside the ball, the output is 0, else it is 1e16.
         """
         diff = u - y
         dist = torch.norm(diff.view(diff.shape[0], -1), p=2, dim=-1)
         radius = self.radius if radius is None else radius
         loss = (dist > radius) * 1e16
         return loss
 
@@ -361,19 +371,19 @@
 
             \operatorname{prox}_{\iota_{\mathcal{B}_2(y,r)}}(x) = \operatorname{proj}_{\mathcal{B}_2(y, r)}(x)
 
 
         where :math:`\operatorname{proj}_{C}(x)` denotes the projection on the closed convex set :math:`C`.
 
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`x`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`x`.
         :param float gamma: step-size. Note that this parameter is not used in this function.
         :param float radius: radius of the :math:`\ell_2` ball.
-        :return: (torch.tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
+        :return: (torch.Tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
         """
         radius = self.radius if radius is None else radius
         diff = x - y
         dist = torch.norm(diff.view(diff.shape[0], -1), p=2, dim=-1)
         return y + diff * (
             torch.min(torch.tensor([radius]).to(x.device), dist) / (dist + 1e-12)
         ).view(-1, 1, 1, 1)
@@ -394,23 +404,23 @@
         .. math::
 
             \operatorname{prox}_{\gamma \iota_{\mathcal{B}_2(y, r)}(A\cdot)}(x) = \underset{u}{\text{argmin}} \,\, \iota_{\mathcal{B}_2(y, r)}(Au)+\frac{1}{2}\|u-x\|_2^2
 
         Since no closed form is available for general measurement operators, we use a dual forward-backward algorithm,
         as suggested in `Proximal Splitting Methods in Signal Processing <https://arxiv.org/pdf/0912.3522.pdf>`_.
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`A(x)`.
-        :param torch.tensor radius: radius of the :math:`\ell_2` ball.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`\forw{x}`.
+        :param torch.Tensor radius: radius of the :math:`\ell_2` ball.
         :param float stepsize: step-size of the dual-forward-backward algorithm.
         :param float crit_conv: convergence criterion of the dual-forward-backward algorithm.
         :param int max_iter: maximum number of iterations of the dual-forward-backward algorithm.
         :param float gamma: factor in front of the indicator function. Notice that this does not affect the proximity
                             operator since the indicator is scale invariant. Default: None.
-        :return: (torch.tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
+        :return: (torch.Tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
         """
         radius = self.radius if radius is None else radius
 
         if physics.A(x).shape == x.shape and (physics.A(x) == x).all():  # Identity case
             return self.prox_d(x, y, gamma=None, radius=radius)
         else:
             norm_AtA = physics.compute_norm(x, verbose=False)
@@ -507,35 +517,35 @@
 
 
         .. note::
 
             The gradient is not defined at :math:`x=y`.
 
 
-        :param torch.tensor x: Variable :math:`x` at which the gradient is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`x`.
-        :return: (torch.tensor) gradient of the :math:`\ell_1` norm at `x`.
+        :param torch.Tensor x: Variable :math:`x` at which the gradient is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`x`.
+        :return: (torch.Tensor) gradient of the :math:`\ell_1` norm at `x`.
         """
         return torch.sign(x - y)
 
     def prox_d(self, u, y, gamma=1.0):
         r"""
         Proximal operator of the :math:`\ell_1` norm, i.e.
 
         .. math::
 
             \operatorname{prox}_{\gamma \ell_1}(x) = \underset{z}{\text{argmin}} \,\, \gamma \|z-y\|_1+\frac{1}{2}\|z-x\|_2^2
 
 
         also known as the soft-thresholding operator.
 
-        :param torch.tensor u: Variable :math:`u` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`x`.
+        :param torch.Tensor u: Variable :math:`u` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`x`.
         :param float gamma: stepsize (or soft-thresholding parameter).
-        :return: (torch.tensor) soft-thresholding of `u` with parameter `gamma`.
+        :return: (torch.Tensor) soft-thresholding of `u` with parameter `gamma`.
         """
         d = u - y
         aux = torch.sign(d) * torch.maximum(
             d.abs() - gamma, torch.tensor([0]).to(d.device)
         )
         return aux + y
 
@@ -550,21 +560,21 @@
             \operatorname{prox}_{\gamma \ell_1}(x) = \underset{u}{\text{argmin}} \,\, \gamma \|Au-y\|_1+\frac{1}{2}\|u-x\|_2^2.
 
 
 
         Since no closed form is available for general measurement operators, we use a dual forward-backward algorithm.
 
 
-        :param torch.tensor x: Variable :math:`x` at which the proximity operator is computed.
-        :param torch.tensor y: Data :math:`y` of the same dimension as :math:`A(x)`.
+        :param torch.Tensor x: Variable :math:`x` at which the proximity operator is computed.
+        :param torch.Tensor y: Data :math:`y` of the same dimension as :math:`\forw{x}`.
         :param deepinv.physics.Physics physics: physics model.
         :param float stepsize: step-size of the dual-forward-backward algorithm.
         :param float crit_conv: convergence criterion of the dual-forward-backward algorithm.
         :param int max_iter: maximum number of iterations of the dual-forward-backward algorithm.
-        :return: (torch.tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
+        :return: (torch.Tensor) projection on the :math:`\ell_2` ball of radius `radius` and centered in `y`.
         """
         norm_AtA = physics.compute_norm(x)
         stepsize = 1.0 / norm_AtA if stepsize is None else stepsize
         u = x.clone()
         for it in range(max_iter):
             u_prev = u.clone()
 
@@ -574,14 +584,86 @@
             rel_crit = ((u - u_prev).norm()) / (u.norm() + 1e-12)
             print(rel_crit)
             if rel_crit < crit_conv and it > 2:
                 break
         return t
 
 
+class AmplitudeLoss(DataFidelity):
+    r"""
+    Amplitude loss as the data fidelity term for :meth:`deepinv.physics.PhaseRetrieval` reconstrunction.
+
+    In this case, the data fidelity term is defined as
+
+    .. math::
+
+        f(x) = \sum_{i=1}^{m}{(\sqrt{|b_i x|^2}-\sqrt{y_i})^2},
+
+    where :math:`b_i` is the i-th row of the linear operator :math:`B` of the phase retrieval class and :math:`y_i` is the i-th entry of the measurements, and :math:`m` is the number of measurements.
+
+    """
+
+    def __init__(self):
+        super().__init__()
+
+    def d(self, u, y):
+        r"""
+        Computes the amplitude loss.
+
+        :param torch.Tensor u: estimated measurements.
+        :param torch.Tensor y: true measurements.
+        :return: (torch.Tensor) the amplitude loss of shape B where B is the batch size.
+        """
+        x = torch.sqrt(u) - torch.sqrt(y)
+        d = torch.norm(x.view(x.shape[0], -1), p=2, dim=-1) ** 2
+        return d
+
+    def grad_d(self, u, y, epsilon=1e-12):
+        r"""
+        Computes the gradient of the amplitude loss :math:`\distance{u}{y}`, i.e.,
+
+        .. math::
+
+            \nabla_{u}\distance{u}{y} = \frac{\sqrt{u}-\sqrt{y}}{\sqrt{u}}
+
+
+        :param torch.Tensor u: Variable :math:`u` at which the gradient is computed.
+        :param torch.Tensor y: Data :math:`y`.
+        :param float epsilon: small value to avoid division by zero.
+        :return: (torch.Tensor) gradient of the amplitude loss function.
+        """
+        return (torch.sqrt(u + epsilon) - torch.sqrt(y)) / torch.sqrt(u + epsilon)
+
+
+class LogPoissonLikelihood(DataFidelity):
+    r"""
+    Log-Poisson negative log-likelihood.
+
+    .. math::
+
+        \datafid{z}{y} =  N_0 (1^{\top} \exp(-\mu z)+ \mu \exp(-\mu y)^{\top}x)
+
+    Corresponds to LogPoissonNoise with the same arguments N0 and mu.
+    There is no closed-form of prox_d known.
+
+    :param float N0: average number of photons
+    :param float mu: normalization constant
+    """
+
+    def __init__(self, N0=1024.0, mu=1 / 50.0):
+        super().__init__()
+        self.mu = mu
+        self.N0 = N0
+
+    def d(self, x, y):
+        out1 = torch.exp(-x * self.mu) * self.N0
+        out2 = torch.exp(-y * self.mu) * self.N0 * (x * self.mu)
+        return (out1 + out2).sum()
+
+
 if __name__ == "__main__":
     import deepinv as dinv
 
     # define a loss function
     data_fidelity = L2()
 
     # create a measurement operator dxd
```

### Comparing `deepinv-0.1.1/deepinv/optim/fixed_point.py` & `deepinv-0.2.0/deepinv/optim/fixed_point.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,61 +10,46 @@
     This module implements the fixed-point iteration algorithm given a specific fixed-point iterator (e.g.
     proximal gradient iteration, the ADMM iteration, see :meth:`deepinv.optim.optim_iterators`), that is
     for :math:`k=1,2,...`
 
     .. math::
         \qquad (x_{k+1}, u_{k+1}) = \operatorname{FixedPoint}(x_k, u_k, f, g, A, y, ...) \hspace{2cm} (1)
 
+    where :math:`f` is the data-fidelity term, :math:`g` is the prior, :math:`A` is the physics model, :math:`y` is the data.
 
-    where :math:`f` is the data-fidelity term, :math:`g` is the prior, :math:`A` is the physics model, :math:`y` is the
-    data.
-
-
-    ::
-
-        # This example shows how to use the FixedPoint class to solve the problem
-        #                min_x 0.5*lambda*||Ax-y||_2^2 + ||x||_1
-        # with the PGD algorithm, where A is the identity operator, lambda = 1 and y = [2, 2].
-
-        # Create the measurement operator A
-        A = torch.tensor([[1, 0], [0, 1]], dtype=torch.float64)
-        A_forward = lambda v: A @ v
-        A_adjoint = lambda v: A.transpose(0, 1) @ v
-
-        # Define the physics model associated to this operator
-        physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
-
-        # Define the measurement y
-        y = torch.tensor([2, 2], dtype=torch.float64)
-
-        # Define the data fidelity term
-        data_fidelity = L2()
-
-        # Define the proximity operator of the prior and store it in a dictionary
-        def prox_g(x, g_param=0.1):
-            return torch.sign(x) * torch.maximum(x.abs() - g_param, torch.tensor([0]))
-
-        prior = {"prox_g": prox_g}
-
-        # Define the parameters of the algorithm
-        params = {"g_param": 1.0, "stepsize": 1.0, "lambda": 1.0}
-
-        # Choose the iterator associated to the PGD algorithm
-        iterator = PGDIteration(data_fidelity=data_fidelity)
-
-        # Iterate the iterator
-        x_init = torch.tensor([2, 2], dtype=torch.float64)  # Define initialisation of the algorithm
-        X = {"est": (x_init ,), "cost": []}                 # Iterates are stored in a dictionary of the form {'est': (x,z), 'cost': F}
-
-        max_iter = 50
-        for it in range(max_iter):
-            X = iterator(X,  prior, params, y, physics)
-
-        # Return the solution
-        sol = X["est"][0]  # sol = [1, 1]
+    :Examples: This example shows how to use the :class:`FixedPoint` class to solve the problem
+        :math:`\min_x 0.5*||Ax-y||_2^2 + \lambda*||x||_1` with the PGD algorithm, where A is the identity operator,
+        :math:`\lambda = 1` and :math:`y = [2, 2]`.
+
+        >>> import deepinv as dinv
+        >>> # Create the measurement operator A
+        >>> A = torch.tensor([[1, 0], [0, 1]], dtype=torch.float64)
+        >>> A_forward = lambda v: A @ v
+        >>> A_adjoint = lambda v: A.transpose(0, 1) @ v
+        >>> # Define the physics model associated to this operator
+        >>> physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
+        >>> # Define the measurement y
+        >>> y = torch.tensor([2, 2], dtype=torch.float64)
+        >>> # Define the data fidelity term
+        >>> data_fidelity = dinv.optim.data_fidelity.L2()
+        >>> # Define the prior term
+        >>> prior = dinv.optim.prior.L1Prior()
+        >>> # Define the parameters of the algorithm
+        >>> params_algo = {"g_param": 1.0, "stepsize": 1.0, "lambda": 1.0, "beta": 1.0}
+        >>> # Choose the iterator associated to the PGD algorithm
+        >>> iterator = dinv.optim.optim_iterators.PGDIteration()
+        >>> # Iterate the iterator
+        >>> x_init = torch.tensor([2, 2], dtype=torch.float64)  # Define initialisation of the algorithm
+        >>> X = {"est": (x_init ,), "cost": []}                 # Iterates are stored in a dictionary of the form {'est': (x,z), 'cost': F}
+        >>> max_iter = 50
+        >>> for it in range(max_iter):
+        ...     X = iterator(X, data_fidelity, prior, params_algo, y, physics)
+        >>> # Return the solution
+        >>> X["est"][0]
+        tensor([1., 1.], dtype=torch.float64)
 
 
     :param deepinv.optim.optim_iterators.optim_iterator iterator: function that takes as input the current iterate, as
                                         well as parameters of the optimization problem (prior, measurements, etc.)
     :param function update_params_fn: function that returns the parameters to be used at each iteration. Default: ``None``.
     :param function update_prior_fn: function that returns the prior to be used at each iteration. Default: ``None``.
     :param function init_iterate_fn: function that returns the initial iterate. Default: ``None``.
@@ -211,28 +196,29 @@
         return {"est": est, "cost": F}
 
     def forward(self, *args, compute_metrics=False, x_gt=None, **kwargs):
         r"""
         Loops over the fixed-point iterator as (1) and returns the fixed point.
 
         The iterates are stored in a dictionary of the form ``X = {'est': (x_k, u_k), 'cost': F_k}`` where:
-            - ``est`` is a tuple containing the current primal and auxiliary iterates,
-            - ``cost`` is the value of the cost function at the current iterate.
+
+            * ``est`` is a tuple containing the current primal and auxiliary iterates,
+            * ``cost`` is the value of the cost function at the current iterate.
 
         Since the prior and parameters (stepsize, regularisation parameter, etc.) can change at each iteration,
         the prior and parameters are updated before each call to the iterator.
 
         :param bool compute_metrics: if ``True``, the metrics are computed along the iterations. Default: ``False``.
         :param torch.Tensor x_gt: ground truth solution. Default: ``None``.
         :param args: optional arguments for the iterator. Commonly (y,physics) where ``y`` (torch.Tensor y) is the measurement and
                     ``physics`` (deepinv.physics) is the physics model.
         :param kwargs: optional keyword arguments for the iterator.
         :return tuple: ``(x,metrics)`` with ``x`` the fixed-point solution (dict) and
                     ``metrics`` the computed along the iterations if ``compute_metrics`` is ``True`` or ``None``
-                     otherwise.
+                    otherwise.
         """
         X = (
             self.init_iterate_fn(*args, F_fn=self.iterator.F_fn)
             if self.init_iterate_fn
             else None
         )
         metrics = (
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/admm.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/admm.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 
 class ADMMIteration(OptimIterator):
     r"""
     Iterator for alternating direction method of multipliers.
 
     Class for a single iteration of the Alternating Direction Method of Multipliers (ADMM) algorithm for
-    minimising :math:`\lambda f(x) + g(x)`.
+    minimising :math:` f(x) + \lambda g(x)`.
 
     If the attribute ``g_first`` is set to False (by default),
     the iteration is (`see this paper <https://www.nowpublishers.com/article/Details/MAL-016>`_):
 
     .. math::
         \begin{equation*}
         \begin{aligned}
-        u_{k+1} &= \operatorname{prox}_{\gamma \lambda f}(x_k - z_k) \\
-        x_{k+1} &= \operatorname{prox}_{\gamma g}(u_{k+1} + z_k) \\
+        u_{k+1} &= \operatorname{prox}_{\gamma f}(x_k - z_k) \\
+        x_{k+1} &= \operatorname{prox}_{\gamma \lambda g}(u_{k+1} + z_k) \\
         z_{k+1} &= z_k + \beta (u_{k+1} - x_{k+1})
         \end{aligned}
         \end{equation*}
 
     where :math:`\gamma>0` is a stepsize and :math:`\beta>0` is a relaxation parameter.
 
     If the attribute ``g_first`` is set to ``True``, the functions :math:`f` and :math:`g` are
@@ -71,47 +71,49 @@
     """
 
     def __init__(self, **kwargs):
         super(fStepADMM, self).__init__(**kwargs)
 
     def forward(self, x, z, cur_data_fidelity, cur_params, y, physics):
         r"""
-        Single iteration step on the data-fidelity term :math:`\lambda f`.
+        Single iteration step on the data-fidelity term :math:`f`.
 
         :param torch.Tensor x: current first variable
         :param torch.Tensor z: current second variable
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         :param torch.Tensor y: Input data.
         :param deepinv.physics physics: Instance of the physics modeling the observation.
         """
         if self.g_first:
             p = x + z
         else:
             p = x - z
-        return cur_data_fidelity.prox(
-            p, y, physics, gamma=cur_params["lambda"] * cur_params["stepsize"]
-        )
+        return cur_data_fidelity.prox(p, y, physics, gamma=cur_params["stepsize"])
 
 
 class gStepADMM(gStep):
     r"""
     ADMM gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepADMM, self).__init__(**kwargs)
 
     def forward(self, x, z, cur_prior, cur_params):
         r"""
-        Single iteration step on the prior term :math:`g`.
+        Single iteration step on the prior term :math:`\lambda g`.
 
         :param torch.Tensor x: current first variable
         :param torch.Tensor z: current second variable
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         """
         if self.g_first:
             p = x - z
         else:
             p = x + z
-        return cur_prior.prox(p, cur_params["g_param"], gamma=cur_params["stepsize"])
+        return cur_prior.prox(
+            p,
+            cur_params["g_param"],
+            gamma=cur_params["lambda"] * cur_params["stepsize"],
+        )
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/drs.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/drs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 
 
 class DRSIteration(OptimIterator):
     r"""
     Iterator for Douglas-Rachford Splitting.
 
     Class for a single iteration of the Douglas-Rachford Splitting (DRS) algorithm for minimising
-    :math:`\lambda f(x) + g(x)`.
+    :math:` f(x) + \lambda g(x)`.
 
     If the attribute ``g_first`` is set to False (by default), the iteration is given by
 
     .. math::
         \begin{equation*}
         \begin{aligned}
-        u_{k+1} &= \operatorname{prox}_{\gamma \lambda f}(z_k) \\
-        x_{k+1} &= \operatorname{prox}_{\gamma g}(2*u_{k+1}-z_k) \\
+        u_{k+1} &= \operatorname{prox}_{\gamma f}(z_k) \\
+        x_{k+1} &= \operatorname{prox}_{\gamma \lambda g}(2*u_{k+1}-z_k) \\
         z_{k+1} &= z_k + \beta (x_{k+1} - u_{k+1})
         \end{aligned}
         \end{equation*}
 
     where :math:`\gamma>0` is a stepsize and :math:`\beta>0` is a relaxation parameter.
 
     If the attribute ``g_first`` is set to True, the functions :math:`f` and :math:`g` are inverted in the previous iteration.
@@ -82,34 +82,36 @@
         :param torch.Tensor y: Input data.
         :param deepinv.physics physics: Instance of the physics modeling the data-fidelity term.
         """
         if self.g_first:
             p = 2 * x - z
         else:
             p = z
-        return cur_data_fidelity.prox(
-            p, y, physics, gamma=cur_params["lambda"] * cur_params["stepsize"]
-        )
+        return cur_data_fidelity.prox(p, y, physics, gamma=cur_params["stepsize"])
 
 
 class gStepDRS(gStep):
     r"""
     DRS gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepDRS, self).__init__(**kwargs)
 
     def forward(self, x, z, cur_prior, cur_params):
         r"""
-        Single iteration step on the prior term :math:`g`.
+        Single iteration step on the prior term :math:`\lambda g`.
 
         :param torch.Tensor x:  Current first variable.
         :param torch.Tensor z: Current second variable.
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         """
         if self.g_first:
             p = z
         else:
             p = 2 * x - z
-        return cur_prior.prox(p, cur_params["g_param"], gamma=cur_params["stepsize"])
+        return cur_prior.prox(
+            p,
+            cur_params["g_param"],
+            gamma=cur_params["lambda"] * cur_params["stepsize"],
+        )
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/gradient_descent.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/gradient_descent.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
         super(GDIteration, self).__init__(**kwargs)
         self.g_step = gStepGD(**kwargs)
         self.f_step = fStepGD(**kwargs)
         self.requires_grad_g = True
 
     def forward(self, X, cur_data_fidelity, cur_prior, cur_params, y, physics):
         r"""
-        Single gradient descent iteration on the objective :math:`\lambda f(x) + g(x)`.
+        Single gradient descent iteration on the objective :math:`f(x) + \lambda g(x)`.
 
         :param dict X: Dictionary containing the current iterate :math:`x_k`.
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         :param torch.Tensor y: Input data.
         :return: Dictionary `{"est": (x, ), "cost": F}` containing the updated current iterate and the estimated current cost.
@@ -64,27 +64,27 @@
 
         :param torch.Tensor x: current iterate :math:`x_k`.
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         :param torch.Tensor y: Input data.
         :param deepinv.physics physics: Instance of the physics modeling the data-fidelity term.
         """
-        return cur_params["lambda"] * cur_data_fidelity.grad(x, y, physics)
+        return cur_data_fidelity.grad(x, y, physics)
 
 
 class gStepGD(gStep):
     r"""
     GD gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepGD, self).__init__(**kwargs)
 
     def forward(self, x, cur_prior, cur_params):
         r"""
-        Single iteration step on the prior term :math:`g`.
+        Single iteration step on the prior term :math:`\lambda g`.
 
         :param torch.Tensor x: Current iterate :math:`x_k`.
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         """
-        return cur_prior.grad(x, cur_params["g_param"])
+        return cur_params["lambda"] * cur_prior.grad(x, cur_params["g_param"])
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/hqs.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/hqs.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from .optim_iterator import OptimIterator, fStep, gStep
 
 
 class HQSIteration(OptimIterator):
     r"""
     Single iteration of half-quadratic splitting.
 
-    Class for a single iteration of the Half-Quadratic Splitting (HQS) algorithm for minimising :math:`\lambda f(x) + g(x)`.
+    Class for a single iteration of the Half-Quadratic Splitting (HQS) algorithm for minimising :math:` f(x) + \lambda g(x)`.
     The iteration is given by
 
 
     .. math::
         \begin{equation*}
         \begin{aligned}
-        u_{k} &= \operatorname{prox}_{\gamma \lambda f}(x_k) \\
-        x_{k+1} &= \operatorname{prox}_{\sigma g}(u_k).
+        u_{k} &= \operatorname{prox}_{\gamma f}(x_k) \\
+        x_{k+1} &= \operatorname{prox}_{\sigma \lambda g}(u_k).
         \end{aligned}
         \end{equation*}
 
 
     where :math:`\gamma` and :math:`\sigma` are step-sizes. Note that this algorithm does not converge to
-    a minimizer of :math:`\lambda f(x) + g(x)`, but instead to a minimizer of
-    :math:`\lambda \gamma\, ^1f+\sigma g`, where :math:`^1f` denotes
+    a minimizer of :math:`f(x) + \lambda  g(x)`, but instead to a minimizer of
+    :math:` \gamma\, ^1f+\sigma \lambda g`, where :math:`^1f` denotes
     the Moreau envelope of :math:`f`
 
     """
 
     def __init__(self, **kwargs):
         super(HQSIteration, self).__init__(**kwargs)
         self.g_step = gStepHQS(**kwargs)
@@ -46,29 +46,31 @@
 
         :param torch.Tensor x: Current iterate :math:`x_k`.
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         :param torch.Tensor y: Input data.
         :param deepinv.physics physics: Instance of the physics modeling the data-fidelity term.
         """
-        return cur_data_fidelity.prox(
-            x, y, physics, gamma=cur_params["lambda"] * cur_params["stepsize"]
-        )
+        return cur_data_fidelity.prox(x, y, physics, gamma=cur_params["stepsize"])
 
 
 class gStepHQS(gStep):
     r"""
     HQS gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepHQS, self).__init__(**kwargs)
 
     def forward(self, x, cur_prior, cur_params):
         r"""
-        Single proximal step on the prior term :math:`g`.
+        Single proximal step on the prior term :math:` \lambda g`.
 
         :param torch.Tensor x: Current iterate :math:`x_k`.
         :param dict cur_prior: Class containing the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         """
-        return cur_prior.prox(x, cur_params["g_param"], gamma=cur_params["stepsize"])
+        return cur_prior.prox(
+            x,
+            cur_params["g_param"],
+            gamma=cur_params["lambda"] * cur_params["stepsize"],
+        )
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/optim_iterator.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/optim_iterator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class OptimIterator(nn.Module):
     r"""
     Base class for all :meth:`Optim` iterators.
 
     An optim iterator is an object that implements a fixed point iteration for minimizing the sum of two functions
-    :math:`F = \lambda*f + g` where :math:`f` is a data-fidelity term  that will be modeled by an instance of physics
+    :math:`F = f + \lambda g` where :math:`f` is a data-fidelity term  that will be modeled by an instance of physics
     and g is a regularizer. The fixed point iteration takes the form
 
     .. math::
         \qquad (x_{k+1}, z_{k+1}) = \operatorname{FixedPoint}(x_k, z_k, f, g, A, y, ...)
 
     where :math:`x` is a "primal" variable converging to the solution of the minimization problem, and
     :math:`z` is a "dual" variable.
@@ -35,15 +35,15 @@
     where :math:`\operatorname{step}_f` and :math:`\operatorname{step}_g` are the steps on f and g respectively.
 
     :param bool g_first: If True, the algorithm starts with a step on g and finishes with a step on f.
     :param F_fn: function that returns the function F to be minimized at each iteration. Default: None.
     :param bool has_cost: If True, the function F is computed at each iteration. Default: False.
      """
 
-    def __init__(self, g_first=False, F_fn=None, has_cost=False):
+    def __init__(self, g_first=False, F_fn=None, has_cost=False, **kwargs):
         super(OptimIterator, self).__init__()
         self.g_first = g_first
         self.F_fn = F_fn
         self.has_cost = has_cost
         if self.F_fn is None:
             self.has_cost = False
         self.f_step = fStep(g_first=self.g_first)
@@ -60,15 +60,15 @@
         :param float beta: Relaxation parameter.
         :return: Relaxed tensor.
         """
         return beta * u + (1 - beta) * v
 
     def forward(self, X, cur_data_fidelity, cur_prior, cur_params, y, physics):
         r"""
-        General form of a single iteration of splitting algorithms for minimizing :math:`F = \lambda f + g`, alternating
+        General form of a single iteration of splitting algorithms for minimizing :math:`F =  f + \lambda g`, alternating
         between a step on :math:`f` and a step on :math:`g`.
         The primal and dual variables as well as the estimated cost at the current iterate are stored in a dictionary
         $X$ of the form `{'est': (x,z), 'cost': F}`.
 
         :param dict X: Dictionary containing the current iterate and the estimated cost.
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
@@ -116,15 +116,15 @@
             :param deepinv.physics physics: Instance of the physics modeling the observation.
             """
             pass
 
 
 class gStep(nn.Module):
     r"""
-    Module for the single iteration steps on the prior term :math:`g`.
+    Module for the single iteration steps on the prior term :math:` \lambda g`.
 
     :param bool g_first: If True, the algorithm starts with a step on g and finishes with a step on f. Default: False.
     :param kwargs: Additional keyword arguments.
     """
 
     def __init__(self, g_first=False, **kwargs):
         super(gStep, self).__init__()
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/pgd.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/pgd.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 from .utils import gradient_descent_step
 
 
 class PGDIteration(OptimIterator):
     r"""
     Iterator for proximal gradient descent.
 
-    Class for a single iteration of the Proximal Gradient Descent (PGD) algorithm for minimising :math:`\lambda f(x) + g(x)`.
+    Class for a single iteration of the Proximal Gradient Descent (PGD) algorithm for minimizing :math:` f(x) + \lambda g(x)`.
 
     The iteration is given by
 
     .. math::
         \begin{equation*}
         \begin{aligned}
-        u_{k} &= x_k - \lambda \gamma \nabla f(x_k) \\
-        x_{k+1} &= \operatorname{prox}_{\gamma g}(u_k),
+        u_{k} &= x_k -  \gamma \nabla f(x_k) \\
+        x_{k+1} &= \operatorname{prox}_{\gamma \lambda g}(u_k),
         \end{aligned}
         \end{equation*}
 
 
-    where :math:`\gamma` is a stepsize that should satisfy :math:`\lambda \gamma \leq 2/\operatorname{Lip}(\|\nabla f\|)`.
+    where :math:`\gamma` is a stepsize that should satisfy :math:` \gamma \leq 2/\operatorname{Lip}(\|\nabla f\|)`.
 
     """
 
     def __init__(self, **kwargs):
         super(PGDIteration, self).__init__(**kwargs)
         self.g_step = gStepPGD(**kwargs)
         self.f_step = fStepPGD(**kwargs)
@@ -48,44 +48,42 @@
          :param torch.Tensor x: Current iterate :math:`x_k`.
          :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
          :param torch.Tensor y: Input data.
          :param deepinv.physics physics: Instance of the physics modeling the data-fidelity term.
         """
         if not self.g_first:
-            # if cur_params["lambda"] >= 2:
-            #     raise ValueError("lambda must be smaller than 2")
-            grad = (
-                cur_params["lambda"]
-                * cur_params["stepsize"]
-                * cur_data_fidelity.grad(x, y, physics)
-            )
+            grad = cur_params["stepsize"] * cur_data_fidelity.grad(x, y, physics)
             return gradient_descent_step(x, grad)
         else:
-            return cur_data_fidelity.prox(
-                x, y, physics, gamma=cur_params["lambda"] * cur_params["stepsize"]
-            )
+            return cur_data_fidelity.prox(x, y, physics, gamma=cur_params["stepsize"])
 
 
 class gStepPGD(gStep):
     r"""
     PGD gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepPGD, self).__init__(**kwargs)
 
     def forward(self, x, cur_prior, cur_params):
         r"""
-        Single iteration step on the prior term :math:`g`.
+        Single iteration step on the prior term :math:`\lambda g`.
 
         :param torch.Tensor x: Current iterate :math:`x_k`.
         :param dict cur_prior: Dictionary containing the current prior.
         :param dict cur_params: Dictionary containing the current parameters of the algorithm.
         """
         if not self.g_first:
             return cur_prior.prox(
-                x, cur_params["g_param"], gamma=cur_params["stepsize"]
+                x,
+                cur_params["g_param"],
+                gamma=cur_params["lambda"] * cur_params["stepsize"],
             )
         else:
-            grad = cur_params["stepsize"] * cur_prior.grad(x, cur_params["g_param"])
+            grad = (
+                cur_params["lambda"]
+                * cur_params["stepsize"]
+                * cur_prior.grad(x, cur_params["g_param"])
+            )
             return gradient_descent_step(x, grad)
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/primal_dual_CP.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/primal_dual_CP.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,39 @@
 
 
 class CPIteration(OptimIterator):
     r"""
     Iterator for Chambolle-Pock.
 
     Class for a single iteration of the `Chambolle-Pock <https://hal.science/hal-00490826/document>`_ Primal-Dual (PD)
-    algorithm for minimising :math:`\lambda F(Kx) + G(x)` or :math:`\lambda F(x) + G(Kx)` for generic functions :math:`F` and :math:`G`.
+    algorithm for minimising :math:`F(Kx) + \lambda G(x)` or :math:`\lambda F(x) + G(Kx)` for generic functions :math:`F` and :math:`G`.
     Our implementation corresponds to Algorithm 1 of `<https://hal.science/hal-00490826/document>`_.
 
     If the attribute ``g_first`` is set to ``False`` (by default), the iteration is given by
 
     .. math::
         \begin{equation*}
         \begin{aligned}
-        u_{k+1} &= \operatorname{prox}_{\sigma (\lambda F)^*}(u_k + \sigma K z_k) \\
-        x_{k+1} &= \operatorname{prox}_{\tau G}(x_k-\tau K^\top u_{k+1}) \\
+        u_{k+1} &= \operatorname{prox}_{\sigma F^*}(u_k + \sigma K z_k) \\
+        x_{k+1} &= \operatorname{prox}_{\tau \lambda G}(x_k-\tau K^\top u_{k+1}) \\
         z_{k+1} &= x_{k+1} + \beta(x_{k+1}-x_k) \\
         \end{aligned}
         \end{equation*}
 
-    where :math:`(\lambda F)^*` is the Fenchel-Legendre conjugate of :math:`\lambda F`, :math:`\beta>0` is a relaxation parameter, and :math:`\sigma` and :math:`\tau` are step-sizes that should
+    where :math:`F^*` is the Fenchel-Legendre conjugate of :math:`F`, :math:`\beta>0` is a relaxation parameter, and :math:`\sigma` and :math:`\tau` are step-sizes that should
     satisfy :math:`\sigma \tau \|K\|^2 \leq 1`.
 
     If the attribute ``g_first`` is set to ``True``, the functions :math:`F` and :math:`G` are inverted in the previous iteration.
 
     In particular, setting :math:`F = \distancename`, :math:`K = A` and :math:`G = \regname`, the above algorithms solves
 
     .. math::
 
         \begin{equation*}
-        \underset{x}{\operatorname{min}} \,\, \lambda \distancename(Ax, y) + \regname(x)
+        \underset{x}{\operatorname{min}} \,\,  \distancename(Ax, y) + \lambda \regname(x)
         \end{equation*}
 
 
     with a splitting on :math:`\distancename`, with not differentiability assumption needed on :math:`\distancename`
     or :math:`\regname`, not any invertibility assumption on :math:`A`.
 
     Note that the algorithm requires an intiliazation of the three variables :math:`x_0`, :math:`z_0` and :math:`u_0`.
@@ -89,55 +89,58 @@
     """
 
     def __init__(self, **kwargs):
         super(fStepCP, self).__init__(**kwargs)
 
     def forward(self, x, w, cur_data_fidelity, y, physics, cur_params):
         r"""
-        Single Chambolle-Pock iteration step on the data-fidelity term :math:`\lambda f`.
+        Single Chambolle-Pock iteration step on the data-fidelity term :math:`f`.
 
         :param torch.Tensor x: Current first variable :math:`x` if `"g_first"` and :math:`u` otherwise.
         :param torch.Tensor w: Current second variable :math:`A^\top u` if `"g_first"` and :math:`A z` otherwise.
         :param deepinv.optim.DataFidelity cur_data_fidelity: Instance of the DataFidelity class defining the current data_fidelity.
         :param torch.Tensor y: Input data.
         :param deepinv.physics physics: Instance of the physics modeling the data-fidelity term.
         :param dict cur_params: Dictionary containing the current fStep parameters (keys `"stepsize_dual"` (or `"stepsize"`) and `"lambda"`).
         """
         if self.g_first:
             p = x - cur_params["stepsize"] * w
-            return cur_data_fidelity.prox(
-                p, y, physics, gamma=cur_params["stepsize"] * cur_params["lambda"]
-            )
+            return cur_data_fidelity.prox(p, y, physics, gamma=cur_params["stepsize"])
         else:
             p = x + cur_params["stepsize_dual"] * w
             return cur_data_fidelity.prox_d_conjugate(
-                p, y, gamma=cur_params["stepsize_dual"], lamb=cur_params["lambda"]
+                p, y, gamma=cur_params["stepsize_dual"]
             )
 
 
 class gStepCP(gStep):
     r"""
     Chambolle-Pock gStep module.
     """
 
     def __init__(self, **kwargs):
         super(gStepCP, self).__init__(**kwargs)
 
     def forward(self, x, w, cur_prior, cur_params):
         r"""
-        Single Chambolle-Pock iteration step on the prior term :math:`g`.
+        Single Chambolle-Pock iteration step on the prior term :math:`\lambda g`.
 
         :param torch.Tensor x: Current first variable :math:`u` if `"g_first"` and :math:`x` otherwise.
         :param torch.Tensor w: Current second variable :math:`A z` if `"g_first"` and :math:`A^\top u` otherwise.
         :param deepinv.optim.prior cur_prior: Instance of the Prior class defining the current prior.
         :param dict cur_params: Dictionary containing the current gStep parameters (keys `"prox_g"`, `"stepsize"` (or `"stepsize_dual"`) and `"g_param"`).
         """
         if self.g_first:
             p = x + cur_params["stepsize_dual"] * w
             return cur_prior.prox_conjugate(
-                p, cur_params["g_param"], gamma=cur_params["stepsize_dual"]
+                p,
+                cur_params["g_param"],
+                gamma=cur_params["lambda"] * cur_params["stepsize_dual"],
+                lamb=cur_params["lambda"],
             )
         else:
             p = x - cur_params["stepsize"] * w
             return cur_prior.prox(
-                p, cur_params["g_param"], gamma=cur_params["stepsize"]
+                p,
+                cur_params["g_param"],
+                gamma=cur_params["stepsize"] * cur_params["lambda"],
             )
```

### Comparing `deepinv-0.1.1/deepinv/optim/optim_iterators/utils.py` & `deepinv-0.2.0/deepinv/optim/optim_iterators/utils.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/optim/optimizers.py` & `deepinv-0.2.0/deepinv/optim/optimizers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import warnings
 import torch
 import torch.nn as nn
 from deepinv.optim.fixed_point import FixedPoint
 from collections.abc import Iterable
 from deepinv.utils import cal_psnr
 from deepinv.optim.optim_iterators import *
+from deepinv.optim.prior import Zero
 
 
 class BaseOptim(nn.Module):
     r"""
     Class for optimization algorithms, consists in iterating a fixed-point operator.
 
     Module solving the problem
 
     .. math::
         \begin{equation}
         \label{eq:min_prob}
         \tag{1}
-        \underset{x}{\arg\min} \quad \lambda \datafid{x}{y} + \reg{x},
+        \underset{x}{\arg\min} \quad  \datafid{x}{y} + \lambda \reg{x},
         \end{equation}
 
 
     where the first term :math:`\datafidname:\xset\times\yset \mapsto \mathbb{R}_{+}` enforces data-fidelity, the second
     term :math:`\regname:\xset\mapsto \mathbb{R}_{+}` acts as a regularization and
     :math:`\lambda > 0` is a regularization parameter. More precisely, the data-fidelity term penalizes the discrepancy
     between the data :math:`y` and the forward operator :math:`A` applied to the variable :math:`x`, as
@@ -41,69 +42,72 @@
 
 
     where :math:`x_k` is a variable converging to the solution of the minimization problem, and
     :math:`z_k` is an additional variable that may be required in the computation of the fixed point operator.
 
     The :func:`optim_builder` function can be used to instantiate this class with a specific fixed point operator.
 
-    If the algorithm is minimizing an explicit and fixed cost function :math:`F(x) = \lambda \datafid{x}{y} + \reg{x}`,
+    If the algorithm is minimizing an explicit and fixed cost function :math:`F(x) =  \datafid{x}{y} + \lambda \reg{x}`,
     the value of the cost function is computed along the iterations and can be used for convergence criterion.
     Moreover, backtracking can be used to adapt the stepsize at each iteration. Backtracking consists in choosing
     the largest stepsize :math:`\tau` such that, at each iteration, sufficient decrease of the cost function :math:`F` is achieved.
     More precisely, Given :math:`\gamma \in (0,1/2)` and :math:`\eta \in (0,1)` and an initial stepsize :math:`\tau > 0`,
     the following update rule is applied at each iteration :math:`k`:
 
     .. math::
-        \text{ while } F(x_k) - F(x_{k+1}) < \frac{\gamma}{\tau} || x_{k-1} - x_k ||^2 \text{ do } \tau \leftarrow \eta \tau
+        \text{ while } F(x_k) - F(x_{k+1}) < \frac{\gamma}{\tau} || x_{k-1} - x_k ||^2, \,\, \text{ do } \tau \leftarrow \eta \tau
 
     The variable ``params_algo`` is a dictionary containing all the relevant parameters for running the algorithm.
     If the value associated with the key is a float, the algorithm will use the same parameter across all iterations.
     If the value is list of length max_iter, the algorithm will use the corresponding parameter at each iteration.
 
     The variable ``data_fidelity`` is a list of instances of :meth:`deepinv.optim.DataFidelity` (or a single instance).
     If a single instance, the same data-fidelity is used at each iteration. If a list, the data-fidelity can change at each iteration.
     The same holds for the variable ``prior`` which is a list of instances of :meth:`deepinv.optim.Prior` (or a single instance).
 
-    ::
+    .. doctest::
 
-        # This minimal example shows how to use the BaseOptim class to solve the problem
-        #                min_x 0.5 \lambda ||Ax-y||_2^2 + ||x||_1
-        # with the PGD algorithm, where A is the identity operator, lambda = 1 and y = [2, 2].
-
-        # Create the measurement operator A
-        A = torch.tensor([[1, 0], [0, 1]], dtype=torch.float64)
-        A_forward = lambda v: A @ v
-        A_adjoint = lambda v: A.transpose(0, 1) @ v
-
-        # Define the physics model associated to this operator
-        physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
-
-        # Define the measurement y
-        y = torch.tensor([2, 2], dtype=torch.float64)
-
-        # Define the data fidelity term
-        data_fidelity = dinv.optim.data_fidelity.L2()
-
-        # Define the prior
-        prior = dinv.optim.Prior(g = lambda x, *args: torch.norm(x, p=1))
-
-        # Define the parameters of the algorithm
-        params_algo = {"stepsize": 0.5, "lambda": 1.0}
-
-        # Define the fixed-point iterator
-        iterator = dinv.optim.optim_iterators.PGDIteration()
-
-        # Define the optimization algorithm
-        optimalgo = dinv.optim.BaseOptim(iterator,
-                            data_fidelity=data_fidelity,
-                            params_algo=params_algo,
-                            prior=prior)
-
-        # Run the optimization algorithm
-        xhat = optimalgo(y, physics)
+        >>> import deepinv as dinv
+        >>> # This minimal example shows how to use the BaseOptim class to solve the problem
+        >>> #                min_x 0.5  ||Ax-y||_2^2 + \lambda ||x||_1
+        >>> # with the PGD algorithm, where A is the identity operator, lambda = 1 and y = [2, 2].
+        >>>
+        >>> # Create the measurement operator A
+        >>> A = torch.tensor([[1, 0], [0, 1]], dtype=torch.float64)
+        >>> A_forward = lambda v: A @ v
+        >>> A_adjoint = lambda v: A.transpose(0, 1) @ v
+        >>>
+        >>> # Define the physics model associated to this operator
+        >>> physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
+        >>>
+        >>> # Define the measurement y
+        >>> y = torch.tensor([2, 2], dtype=torch.float64)
+        >>>
+        >>> # Define the data fidelity term
+        >>> data_fidelity = dinv.optim.data_fidelity.L2()
+        >>>
+        >>> # Define the prior
+        >>> prior = dinv.optim.Prior(g = lambda x, *args: torch.norm(x, p=1))
+        >>>
+        >>> # Define the parameters of the algorithm
+        >>> params_algo = {"stepsize": 0.5, "lambda": 1.0}
+        >>>
+        >>> # Define the fixed-point iterator
+        >>> iterator = dinv.optim.optim_iterators.PGDIteration()
+        >>>
+        >>> # Define the optimization algorithm
+        >>> optimalgo = dinv.optim.BaseOptim(iterator,
+        ...                     data_fidelity=data_fidelity,
+        ...                     params_algo=params_algo,
+        ...                     prior=prior)
+        >>>
+        >>> # Run the optimization algorithm
+        >>> with torch.no_grad(): xhat = optimalgo(y, physics)
+        >>> print(xhat)
+        tensor([1., 1.], dtype=torch.float64)
 
 
     :param deepinv.optim.optim_iterators.OptimIterator iterator: Fixed-point iterator of the optimization algorithm of interest.
     :param dict params_algo: dictionary containing all the relevant parameters for running the algorithm,
                             e.g. the stepsize, regularisation parameter, denoising standard deviation.
                             Each value of the dictionary can be either Iterable (distinct value for each iteration) or
                             a single float (same value for each iteration).
@@ -175,14 +179,18 @@
         self.get_output = get_output
         self.has_cost = has_cost
 
         # By default ``params_algo`` should contain a prior ``g_param`` parameter, set by default to ``None``.
         if "g_param" not in params_algo.keys():
             params_algo["g_param"] = None
 
+        # By default ``params_algo`` should contain a regularization parameter ``lambda`` parameter, which multiplies the prior term ``g``. It is set by default to ``1``.
+        if "lambda" not in params_algo.keys():
+            params_algo["lambda"] = 1.0
+
         # By default ``params_algo`` should contain a relaxation ``beta`` parameter, set by default to 1..
         if "beta" not in params_algo.keys():
             params_algo["beta"] = 1.0
 
         # By default, each parameter in ``params_algo` is a list.
         # If given as a single number, we convert it to a list of 1 element.
         # If given as a list of more than 1 element, it should have lenght ``max_iter``.
@@ -210,16 +218,18 @@
             warnings.warn(
                 "Backtracking impossible when no cost function is given. Setting backtracking to False."
             )
 
         # keep track of initial parameters in case they are changed during optimization (e.g. backtracking)
         self.init_params_algo = params_algo
 
-        # By default, ``self.prior`` should be a list of elements of the class :meth:`deepinv.optim.Prior`. The user could want the prior to change at each iteration.
-        if not isinstance(prior, Iterable):
+        # By default, ``self.prior`` should be a list of elements of the class :meth:`deepinv.optim.Prior`. The user could want the prior to change at each iteration. If no prior is given, we set it to a zero prior.
+        if prior is None:
+            self.prior = [Zero()]
+        elif not isinstance(prior, Iterable):
             self.prior = [prior]
         else:
             self.prior = prior
 
         # By default, ``self.data_fidelity`` should be a list of elements of the class :meth:`deepinv.optim.DataFidelity`. The user could want the prior to change at each iteration.
         if not isinstance(data_fidelity, Iterable):
             self.data_fidelity = [data_fidelity]
@@ -394,16 +404,16 @@
         r"""
         Performs stepsize backtracking.
 
         :param dict X_prev: dictionary containing the primal and dual previous iterates.
         :param dict X: dictionary containing the current primal and dual iterates.
         """
         if self.backtracking and self.has_cost and X_prev is not None:
-            x_prev = self.get_output(X_prev)
-            x = self.get_output(X)
+            x_prev = X_prev["est"][0]
+            x = X["est"][0]
             x_prev = x_prev.reshape((x_prev.shape[0], -1))
             x = x.reshape((x.shape[0], -1))
             F_prev, F = X_prev["cost"], X["cost"]
             diff_F, diff_x = (
                 (F_prev - F).mean(),
                 (torch.norm(x - x_prev, p=2, dim=-1) ** 2).mean(),
             )
@@ -493,17 +503,25 @@
     # If no custom objective function F_fn is given but g is explicitly given, we have an explicit objective function.
     explicit_prior = (
         prior[0].explicit_prior if isinstance(prior, list) else prior.explicit_prior
     )
     if F_fn is None and explicit_prior:
 
         def F_fn(x, data_fidelity, prior, cur_params, y, physics):
-            return cur_params["lambda"] * data_fidelity(x, y, physics) + prior(
-                x, cur_params["g_param"]
-            )
+            prior_value = prior(x, cur_params["g_param"], reduce=False)
+            if prior_value.dim() == 0:
+                reg_value = cur_params["lambda"] * prior_value
+            else:
+                if isinstance(cur_params["lambda"], float):
+                    reg_value = (cur_params["lambda"] * prior_value).sum()
+                else:
+                    reg_value = (
+                        cur_params["lambda"].flatten() * prior_value.flatten()
+                    ).sum()
+            return data_fidelity(x, y, physics) + reg_value
 
         has_cost = True  # boolean to indicate if there is a cost function to evaluate along the iterations
     else:
         has_cost = False
     # Create an instance of :class:`deepinv.optim.optim_iterators.OptimIterator`.
     if isinstance(
         iteration, str
@@ -513,28 +531,31 @@
     else:
         # If the iteration is directly given as an instance of OptimIterator, nothing to do
         return iteration
 
 
 def optim_builder(
     iteration,
-    params_algo={"lambda": 1.0, "stepsize": 1.0},
+    max_iter=100,
+    params_algo={"lambda": 1.0, "stepsize": 1.0, "g_param": 0.05},
     data_fidelity=None,
     prior=None,
     F_fn=None,
     g_first=False,
     **kwargs,
 ):
     r"""
     Helper function for building an instance of the :meth:`BaseOptim` class.
 
     :param str, deepinv.optim.optim_iterators.OptimIterator iteration: either the name of the algorithm to be used,
         or directly an optim iterator.
-        If an algorithm name (string), should be either ``"PGD"`` (proximal gradient descent), ``"ADMM"`` (ADMM),
+        If an algorithm name (string), should be either ``"GD"`` (gradient descent),
+        ``"PGD"`` (proximal gradient descent), ``"ADMM"`` (ADMM),
         ``"HQS"`` (half-quadratic splitting), ``"CP"`` (Chambolle-Pock) or ``"DRS"`` (Douglas Rachford).
+    :param int max_iter: maximum number of iterations of the optimization algorithm. Default: 100.
     :param dict params_algo: dictionary containing all the relevant parameters for running the algorithm,
                             e.g. the stepsize, regularisation parameter, denoising standart deviation.
                             Each value of the dictionary can be either Iterable (distinct value for each iteration) or
                             a single float (same value for each iteration). See :any:`optim-params` for more details.
                             Default: ``{"stepsize": 1.0, "lambda": 1.0}``.
     :param list, deepinv.optim.DataFidelity: data-fidelity term.
                             Either a single instance (same data-fidelity for each iteration) or a list of instances of
@@ -551,13 +572,14 @@
     iterator = create_iterator(iteration, prior=prior, F_fn=F_fn, g_first=g_first)
     return BaseOptim(
         iterator,
         has_cost=iterator.has_cost,
         data_fidelity=data_fidelity,
         prior=prior,
         params_algo=params_algo,
+        max_iter=max_iter,
         **kwargs,
     )
 
 
 def str_to_class(classname):
     return getattr(sys.modules[__name__], classname)
```

### Comparing `deepinv-0.1.1/deepinv/physics/blur.py` & `deepinv-0.2.0/deepinv/physics/blur.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 from torchvision.transforms.functional import rotate
 import torchvision
-import torch.nn.functional as F
 import torch
 import numpy as np
 import torch.fft as fft
-from deepinv.physics.forward import Physics, LinearPhysics, DecomposablePhysics
-from deepinv.utils import TensorList
+from torch import Tensor
+from deepinv.physics.forward import LinearPhysics, DecomposablePhysics
+from deepinv.physics.functional import (
+    conv2d,
+    conv_transpose2d,
+    filter_fft_2d,
+    product_convolution2d,
+    product_convolution2d_adjoint,
+)
 
 
-def filter_fft(filter, img_size, real_fft=True):
-    ph = int((filter.shape[2] - 1) / 2)
-    pw = int((filter.shape[3] - 1) / 2)
+def gaussian_blur(sigma=(1, 1), angle=0):
+    r"""
+    Gaussian blur filter.
+
+    Defined as
+
+    .. math::
+        \begin{equation*}
+            G(x, y) = \frac{1}{2\pi\sigma_x\sigma_y} \exp{\left(-\frac{x'^2}{2\sigma_x^2} - \frac{y'^2}{2\sigma_y^2}\right)}
+        \end{equation*}
 
-    filt2 = torch.zeros(filter.shape[:2] + img_size[-2:], device=filter.device)
+    where :math:`x'` and :math:`y'` are the rotated coordinates obtained by rotating $(x, y)$ around the origin
+    by an angle :math:`\theta`:
 
-    filt2[:, : filter.shape[1], : filter.shape[2], : filter.shape[3]] = filter
-    filt2 = torch.roll(filt2, shifts=(-ph, -pw), dims=(2, 3))
+    .. math::
 
-    return fft.rfft2(filt2) if real_fft else fft.fft2(filt2)
+        \begin{align*}
+            x' &= x \cos(\theta) - y \sin(\theta) \\
+            y' &= x \sin(\theta) + y \cos(\theta)
+        \end{align*}
 
+    with :math:`\sigma_x` and :math:`\sigma_y`  the standard deviations along the :math:`x'` and :math:`y'` axes.
 
-def gaussian_blur(sigma=(1, 1), angle=0):
-    r"""
-    Gaussian blur filter.
 
     :param float, tuple[float] sigma: standard deviation of the gaussian filter. If sigma is a float the filter is isotropic, whereas
         if sigma is a tuple of floats (sigma_x, sigma_y) the filter is anisotropic.
     :param float angle: rotation angle of the filter in degrees (only useful for anisotropic filters)
     """
     if isinstance(sigma, (int, float)):
         sigma = (sigma, sigma)
@@ -56,22 +70,59 @@
 
     filt = filt / filt.flatten().sum()
 
     return filt.unsqueeze(0).unsqueeze(0)
 
 
 def bilinear_filter(factor=2):
+    r"""
+    Bilinear filter.
+
+    It has size (2*factor, 2*factor) and is defined as
+
+    .. math::
+
+        \begin{equation*}
+            w(x, y) = \begin{cases}
+                (1 - |x|) \cdot (1 - |y|) & \text{if } |x| \leq 1 \text{ and } |y| \leq 1 \\
+                0 & \text{otherwise}
+            \end{cases}
+        \end{equation*}
+
+    for :math:`x, y \in {-\text{factor} + 0.5, -\text{factor} + 0.5 + 1/\text{factor}, \ldots, \text{factor} - 0.5}`.
+
+    :param int factor: downsampling factor
+    """
     x = np.arange(start=-factor + 0.5, stop=factor, step=1) / factor
     w = 1 - np.abs(x)
     w = np.outer(w, w)
     w = w / np.sum(w)
     return torch.Tensor(w).unsqueeze(0).unsqueeze(0)
 
 
 def bicubic_filter(factor=2):
+    r"""
+    Bicubic filter.
+
+    It has size (4*factor, 4*factor) and is defined as
+
+    .. math::
+
+        \begin{equation*}
+            w(x, y) = \begin{cases}
+                (a + 2)|x|^3 - (a + 3)|x|^2 + 1 & \text{if } |x| \leq 1 \\
+                a|x|^3 - 5a|x|^2 + 8a|x| - 4a & \text{if } 1 < |x| < 2 \\
+                0 & \text{otherwise}
+            \end{cases}
+        \end{equation*}
+
+    for :math:`x, y \in {-2\text{factor} + 0.5, -2\text{factor} + 0.5 + 1/\text{factor}, \ldots, 2\text{factor} - 0.5}`.
+
+    :param int factor: downsampling factor
+    """
     x = np.arange(start=-2 * factor + 0.5, stop=2 * factor, step=1) / factor
     a = -0.5
     x = np.abs(x)
     w = ((a + 2) * np.power(x, 3) - (a + 3) * np.power(x, 2) + 1) * (x <= 1)
     w += (
         (a * np.power(x, 3) - 5 * a * np.power(x, 2) + 8 * a * x - 4 * a)
         * (x > 1)
@@ -90,87 +141,130 @@
 
     .. math::
 
         y = S (h*x)
 
     where :math:`h` is a low-pass filter and :math:`S` is a subsampling operator.
 
+    :param torch.Tensor, str, NoneType filter: Downsampling filter. It can be ``'gaussian'``, ``'bilinear'`` or ``'bicubic'`` or a
+        custom ``torch.Tensor`` filter. If ``None``, no filtering is applied.
     :param tuple[int] img_size: size of the input image
     :param int factor: downsampling factor
-    :param torch.Tensor, str, NoneType filter: Downsampling filter. It can be 'gaussian', 'bilinear' or 'bicubic' or a
-        custom ``torch.Tensor`` filter. If ``None``, no filtering is applied.
     :param str padding: options are ``'valid'``, ``'circular'``, ``'replicate'`` and ``'reflect'``.
         If ``padding='valid'`` the blurred output is smaller than the image (no padding)
         otherwise the blurred output has the same size as the image.
 
     |sep|
 
     :Examples:
 
         Downsampling operator with a gaussian filter:
 
+        >>> from deepinv.physics import Downsampling
         >>> x = torch.zeros((1, 1, 32, 32)) # Define black image of size 32x32
         >>> x[:, :, 16, 16] = 1 # Define one white pixel in the middle
-        >>> physics = Downsampling(img_size=((1, 1, 32, 32)), filter = "gaussian", factor = 2)
+        >>> physics = Downsampling(filter = "gaussian", img_size=(1, 32, 32), factor=2)
         >>> y = physics(x)
         >>> y[:, :, 7:10, 7:10] # Display the center of the downsampled image
         tensor([[[[0.0146, 0.0241, 0.0146],
                   [0.0241, 0.0398, 0.0241],
                   [0.0146, 0.0241, 0.0146]]]])
 
     """
 
     def __init__(
         self,
         img_size,
+        filter=None,
         factor=2,
-        filter="gaussian",
         device="cpu",
         padding="circular",
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.factor = factor
         assert isinstance(factor, int), "downsampling factor should be an integer"
+        assert len(img_size) == 3, "img_size should be a tuple of length 3, C x H x W"
         self.imsize = img_size
         self.padding = padding
+        if isinstance(filter, torch.nn.Parameter):
+            self.filter = filter.requires_grad_(False).to(device)
         if isinstance(filter, torch.Tensor):
-            self.filter = filter.to(device)
+            self.filter = torch.nn.Parameter(filter, requires_grad=False).to(device)
         elif filter is None:
             self.filter = filter
         elif filter == "gaussian":
-            self.filter = (
-                gaussian_blur(sigma=(factor, factor)).requires_grad_(False).to(device)
-            )
+            self.filter = torch.nn.Parameter(
+                gaussian_blur(sigma=(factor, factor)), requires_grad=False
+            ).to(device)
         elif filter == "bilinear":
-            self.filter = bilinear_filter(self.factor).requires_grad_(False).to(device)
+            self.filter = torch.nn.Parameter(
+                bilinear_filter(self.factor), requires_grad=False
+            ).to(device)
         elif filter == "bicubic":
-            self.filter = bicubic_filter(self.factor).requires_grad_(False).to(device)
+            self.filter = torch.nn.Parameter(
+                bicubic_filter(self.factor), requires_grad=False
+            ).to(device)
         else:
             raise Exception("The chosen downsampling filter doesn't exist")
 
         if self.filter is not None:
-            self.Fh = filter_fft(self.filter, img_size, real_fft=False).to(device)
+            self.Fh = filter_fft_2d(self.filter, img_size, real_fft=False).to(device)
             self.Fhc = torch.conj(self.Fh)
             self.Fh2 = self.Fhc * self.Fh
-            self.filter = torch.nn.Parameter(self.filter, requires_grad=False)
             self.Fhc = torch.nn.Parameter(self.Fhc, requires_grad=False)
             self.Fh2 = torch.nn.Parameter(self.Fh2, requires_grad=False)
 
-    def A(self, x):
+    def A(self, x, filter=None, **kwargs):
+        r"""
+        Applies the downsampling operator to the input image.
+
+        :param torch.Tensor x: input image.
+        :param None, torch.Tensor filter: Filter :math:`h` to be applied to the input image before downsampling.
+            If not ``None``, it uses this filter and stores it as the current filter.
+        """
+        if filter is not None:
+            self.filter = torch.nn.Parameter(filter, requires_grad=False)
+
         if self.filter is not None:
-            x = conv(x, self.filter, padding=self.padding)
+            x = conv2d(x, self.filter, padding=self.padding)
+
         x = x[:, :, :: self.factor, :: self.factor]  # downsample
         return x
 
-    def A_adjoint(self, y):
-        x = torch.zeros((y.shape[0],) + self.imsize, device=y.device)
+    def A_adjoint(self, y, filter=None, **kwargs):
+        r"""
+        Adjoint operator of the downsampling operator.
+
+        :param torch.Tensor y: downsampled image.
+        :param None, torch.Tensor filter: Filter :math:`h` to be applied to the input image before downsampling.
+            If not ``None``, it uses this filter and stores it as the current filter.
+        """
+        if filter is not None:
+            self.filter = torch.nn.Parameter(filter, requires_grad=False)
+
+        imsize = self.imsize
+        if self.filter is not None:
+            if self.padding == "valid":
+                imsize = (
+                    self.imsize[0],
+                    self.imsize[1] - self.filter.shape[-2] + 1,
+                    self.imsize[2] - self.filter.shape[-1] + 1,
+                )
+            else:
+                imsize = (
+                    self.imsize[0],
+                    self.imsize[1] - (self.filter.shape[-2] + 1) % 2,
+                    self.imsize[2] - (self.filter.shape[-1] + 1) % 2,
+                )
+
+        x = torch.zeros((y.shape[0],) + imsize, device=y.device)
         x[:, :, :: self.factor, :: self.factor] = y  # upsample
         if self.filter is not None:
-            x = conv_transpose(x, self.filter, padding=self.padding)
+            x = conv_transpose2d(x, self.filter, padding=self.padding)
         return x
 
     def prox_l2(self, z, y, gamma, use_fft=True):
         r"""
         If the padding is circular, it computes the proximal operator with the closed-formula of
         https://arxiv.org/abs/1510.00143.
 
@@ -198,278 +292,92 @@
             rc = self.Fhc * (top / below).repeat(1, 1, self.factor, self.factor)
             r = torch.real(fft.ifft2(rc))
             return (z_hat - r) * gamma
         else:
             return LinearPhysics.prox_l2(self, z, y, gamma)
 
 
-def extend_filter(filter):
-    b, c, h, w = filter.shape
-    w_new = w
-    h_new = h
-
-    offset_w = 0
-    offset_h = 0
-
-    if w == 1:
-        w_new = 3
-        offset_w = 1
-    elif w % 2 == 0:
-        w_new += 1
-
-    if h == 1:
-        h_new = 3
-        offset_h = 1
-    elif h % 2 == 0:
-        h_new += 1
-
-    out = torch.zeros((b, c, h_new, w_new), device=filter.device)
-    out[:, :, offset_h : h + offset_h, offset_w : w + offset_w] = filter
-    return out
-
-
-def conv(x, filter, padding):
-    r"""
-    Convolution of x and filter. The transposed of this operation is conv_transpose(x, filter, padding)
-
-    :param x: (torch.Tensor) Image of size (B,C,W,H).
-    :param filter: (torch.Tensor) Filter of size (1,C,W,H) for colour filtering or (1,1,W,H) for filtering each channel with the same filter.
-    :param padding: (string) options = 'valid','circular','replicate','reflect'. If padding='valid' the blurred output is smaller than the image (no padding), otherwise the blurred output has the same size as the image.
-
-    """
-    b, c, h, w = x.shape
-
-    filter = filter.flip(-1).flip(
-        -2
-    )  # In order to perform convolution and not correlation like Pytorch native conv
-
-    filter = extend_filter(filter)
-
-    ph = (filter.shape[2] - 1) / 2
-    pw = (filter.shape[3] - 1) / 2
-
-    if padding == "valid":
-        h_out = int(h - 2 * ph)
-        w_out = int(w - 2 * pw)
-    else:
-        h_out = h
-        w_out = w
-        pw = int(pw)
-        ph = int(ph)
-        x = F.pad(x, (pw, pw, ph, ph), mode=padding, value=0)
-
-    if filter.shape[1] == 1:
-        y = torch.zeros((b, c, h_out, w_out), device=x.device)
-        for i in range(b):
-            for j in range(c):
-                y[i, j, :, :] = F.conv2d(
-                    x[i, j, :, :].unsqueeze(0).unsqueeze(1), filter, padding="valid"
-                ).unsqueeze(1)
-    else:
-        y = F.conv2d(x, filter, padding="valid")
-
-    return y
-
-
-def conv_transpose(y, filter, padding):
-    r"""
-    Transposed convolution of x and filter. The transposed of this operation is conv(x, filter, padding)
-
-    :param torch.tensor x: Image of size (B,C,W,H).
-    :param torch.tensor filter: Filter of size (1,C,W,H) for colour filtering or (1,C,W,H) for filtering each channel with the same filter.
-    :param str padding: options are ``'valid'``, ``'circular'``, ``'replicate'`` and ``'reflect'``.
-        If ``padding='valid'`` the blurred output is smaller than the image (no padding)
-        otherwise the blurred output has the same size as the image.
-    """
-
-    b, c, h, w = y.shape
-
-    filter = filter.flip(-1).flip(
-        -2
-    )  # In order to perform convolution and not correlation like Pytorch native conv
-
-    filter = extend_filter(filter)
-
-    ph = (filter.shape[2] - 1) / 2
-    pw = (filter.shape[3] - 1) / 2
-
-    h_out = int(h + 2 * ph)
-    w_out = int(w + 2 * pw)
-    pw = int(pw)
-    ph = int(ph)
-
-    x = torch.zeros((b, c, h_out, w_out), device=y.device)
-    if filter.shape[1] == 1:
-        for i in range(b):
-            if filter.shape[0] > 1:
-                f = filter[i, :, :, :].unsqueeze(0)
-            else:
-                f = filter
-
-            for j in range(c):
-                x[i, j, :, :] = F.conv_transpose2d(
-                    y[i, j, :, :].unsqueeze(0).unsqueeze(1), f
-                )
-    else:
-        x = F.conv_transpose2d(y, filter)
-
-    if padding == "valid":
-        out = x
-    elif padding == "zero":
-        out = x[:, :, ph:-ph, pw:-pw]
-    elif padding == "circular":
-        out = x[:, :, ph:-ph, pw:-pw]
-        # sides
-        out[:, :, :ph, :] += x[:, :, -ph:, pw:-pw]
-        out[:, :, -ph:, :] += x[:, :, :ph, pw:-pw]
-        out[:, :, :, :pw] += x[:, :, ph:-ph, -pw:]
-        out[:, :, :, -pw:] += x[:, :, ph:-ph, :pw]
-        # corners
-        out[:, :, :ph, :pw] += x[:, :, -ph:, -pw:]
-        out[:, :, -ph:, -pw:] += x[:, :, :ph, :pw]
-        out[:, :, :ph, -pw:] += x[:, :, -ph:, :pw]
-        out[:, :, -ph:, :pw] += x[:, :, :ph, -pw:]
-
-    elif padding == "reflect":
-        out = x[:, :, ph:-ph, pw:-pw]
-        # sides
-        out[:, :, 1 : 1 + ph, :] += x[:, :, :ph, pw:-pw].flip(dims=(2,))
-        out[:, :, -ph - 1 : -1, :] += x[:, :, -ph:, pw:-pw].flip(dims=(2,))
-        out[:, :, :, 1 : 1 + pw] += x[:, :, ph:-ph, :pw].flip(dims=(3,))
-        out[:, :, :, -pw - 1 : -1] += x[:, :, ph:-ph, -pw:].flip(dims=(3,))
-        # corners
-        out[:, :, 1 : 1 + ph, 1 : 1 + pw] += x[:, :, :ph, :pw].flip(dims=(2, 3))
-        out[:, :, -ph - 1 : -1, -pw - 1 : -1] += x[:, :, -ph:, -pw:].flip(dims=(2, 3))
-        out[:, :, -ph - 1 : -1, 1 : 1 + pw] += x[:, :, -ph:, :pw].flip(dims=(2, 3))
-        out[:, :, 1 : 1 + ph, -pw - 1 : -1] += x[:, :, :ph, -pw:].flip(dims=(2, 3))
-
-    elif padding == "replicate":
-        out = x[:, :, ph:-ph, pw:-pw]
-        # sides
-        out[:, :, 0, :] += x[:, :, :ph, pw:-pw].sum(2)
-        out[:, :, -1, :] += x[:, :, -ph:, pw:-pw].sum(2)
-        out[:, :, :, 0] += x[:, :, ph:-ph, :pw].sum(3)
-        out[:, :, :, -1] += x[:, :, ph:-ph, -pw:].sum(3)
-        # corners
-        out[:, :, 0, 0] += x[:, :, :ph, :pw].sum(3).sum(2)
-        out[:, :, -1, -1] += x[:, :, -ph:, -pw:].sum(3).sum(2)
-        out[:, :, -1, 0] += x[:, :, -ph:, :pw].sum(3).sum(2)
-        out[:, :, 0, -1] += x[:, :, :ph, -pw:].sum(3).sum(2)
-    return out
-
-
-class BlindBlur(Physics):
-    r"""
-    Blind blur operator.
-
-    If performs
-
-    .. math::
-
-        y = w*x
-
-    where :math:`*` denotes convolution and :math:`w` is an unknown filter.
-    This class uses ``torch.conv2d`` for performing the convolutions.
-
-    The signal is described by a tuple (x,w) where the first element is the clean image, and the second element
-    is the blurring kernel. The measurements y are a tensor representing the convolution of x and w.
-
-    :param int kernel_size: maximum support size of the (unknown) blurring kernels.
-    :param str padding: options are ``'valid'``, ``'circular'``, ``'replicate'`` and ``'reflect'``.
-        If ``padding='valid'`` the blurred output is smaller than the image (no padding)
-        otherwise the blurred output has the same size as the image.
-
-    """
-
-    def __init__(self, kernel_size=3, padding="circular", **kwargs):
-        super().__init__(**kwargs)
-        self.padding = padding
-
-        if type(kernel_size) is not list or type(kernel_size) is not tuple:
-            self.kernel_size = [kernel_size, kernel_size]
-
-    def A(self, s):
-        r"""
-
-        :param tuple, list, deepinv.utils.ListTensor x: List containing two torch.tensor, x[0] with the image and x[1] with the filter.
-        :return: (torch.tensor) blurred measurement.
-        """
-        x = s[0]
-        w = s[1]
-        return conv(x, w, self.padding)
-
-    def A_dagger(self, y):
-        r"""
-        Returns the trivial inverse where x[0] = blurry input and x[1] with a delta filter, such that
-        the convolution of x[0] and x[1] is y.
-
-        .. note:
-
-            This trivial inverse can be useful for some reconstruction networks, such as ``deepinv.models.ArtifactRemoval``.
-
-        :param torch.tensor y: blurred measurement.
-        :return: Tuple containing the trivial inverse.
-        """
-        x = y.clone()
-        mid_h = int(self.kernel_size[0] / 2)
-        mid_w = int(self.kernel_size[1] / 2)
-        w = torch.zeros((y.shape[0], 1, self.kernel_size[0], self.kernel_size[1]))
-        w[:, :, mid_h, mid_w] = 1.0
-
-        return TensorList([x, w])
-
-
 class Blur(LinearPhysics):
     r"""
 
     Blur operator.
 
     This forward operator performs
 
     .. math:: y = w*x
 
     where :math:`*` denotes convolution and :math:`w` is a filter.
 
     This class uses :meth:`torch.nn.functional.conv2d` for performing the convolutions.
 
-    :param torch.Tensor filter: Tensor of size (1, 1, H, W) or (1, C, H, W) containing the blur filter, e.g., :meth:`deepinv.physics.blur.gaussian_blur`.
+    :param torch.Tensor filter: Tensor of size (1, 1, H, W) or (1, C, H, W) containing the blur filter, e.g., :meth:`deepinv.physics.blur.gaussian_filter`.
     :param str padding: options are ``'valid'``, ``'circular'``, ``'replicate'`` and ``'reflect'``. If ``padding='valid'`` the blurred output is smaller than the image (no padding)
-        otherwise the blurred output has the same size as the image.
+        otherwise the blurred output has the same size as the image. (default is ``'valid'``)
     :param str device: cpu or cuda.
 
+
+    .. note::
+
+        This class allows to change the filter at runtime by passing a new filter to the forward method, e.g.,
+        ``y = physics(x, w)``. The new filter :math:`w` is stored as the current filter.
+
     |sep|
 
     :Examples:
 
         Blur operator with a basic averaging filter applied to a 16x16 black image with
         a single white pixel in the center:
 
+        >>> from deepinv.physics import Blur
         >>> x = torch.zeros((1, 1, 16, 16)) # Define black image of size 16x16
         >>> x[:, :, 8, 8] = 1 # Define one white pixel in the middle
         >>> w = torch.ones((1, 1, 2, 2)) / 4 # Basic 2x2 averaging filter
         >>> physics = Blur(filter=w)
         >>> y = physics(x)
         >>> y[:, :, 7:10, 7:10] # Display the center of the blurred image
-        tensor([[[[0.0000, 0.0000, 0.0000],
-                  [0.0000, 0.2500, 0.2500],
-                  [0.0000, 0.2500, 0.2500]]]])
+        tensor([[[[0.2500, 0.2500, 0.0000],
+                  [0.2500, 0.2500, 0.0000],
+                  [0.0000, 0.0000, 0.0000]]]])
 
     """
 
-    def __init__(self, filter, padding="circular", device="cpu", **kwargs):
+    def __init__(self, filter=None, padding="valid", device="cpu", **kwargs):
         super().__init__(**kwargs)
         self.padding = padding
-        self.device = device
-        self.filter = torch.nn.Parameter(filter, requires_grad=False).to(device)
+        if filter is not None:
+            self.filter = torch.nn.Parameter(filter, requires_grad=False).to(device)
 
-    def A(self, x):
-        return conv(x, self.filter, self.padding)
+    def A(self, x, filter=None, **kwargs):
+        r"""
+        Applies the filter to the input image.
 
-    def A_adjoint(self, y):
-        return conv_transpose(y, self.filter, self.padding)
+        :param torch.Tensor x: input image.
+        :param torch.Tensor filter: Filter :math:`w` to be applied to the input image.
+            If not ``None``, it uses this filter instead of the one defined in the class, and
+            the provided filter is stored as the current filter.
+        """
+        if filter is not None:
+            self.filter = torch.nn.Parameter(filter, requires_grad=False)
+
+        return conv2d(x, self.filter, self.padding)
+
+    def A_adjoint(self, y, filter=None, **kwargs):
+        r"""
+        Adjoint operator of the blur operator.
+
+        :param torch.Tensor y: blurred image.
+        :param torch.Tensor filter: Filter :math:`w` to be applied to the input image.
+            If not ``None``, it uses this filter instead of the one defined in the class, and
+            the provided filter is stored as the current filter.
+        """
+
+        if filter is not None:
+            self.filter = torch.nn.Parameter(filter, requires_grad=False)
+
+        return conv_transpose2d(y, self.filter, self.padding)
 
 
 class BlurFFT(DecomposablePhysics):
     """
 
     FFT-based blur operator.
 
@@ -481,112 +389,186 @@
 
     Blur operator based on ``torch.fft`` operations, which assumes a circular padding of the input, and allows for
     the singular value decomposition via ``deepinv.Physics.DecomposablePhysics`` and has fast pseudo-inverse and prox operators.
 
 
 
     :param tuple img_size: Input image size in the form (C, H, W).
-    :param torch.tensor filter: torch.Tensor of size (1, 1, H, W) or (1, C, H, W) containing the blur filter, e.g.,
-        :meth:`deepinv.physics.blur.gaussian_blur`.
+    :param torch.Tensor filter: torch.Tensor of size (1, c, h, w) containing the blur filter with h<=H, w<=W and c=1 or c=C e.g.,
+        :meth:`deepinv.physics.blur.gaussian_filter`.
     :param str device: cpu or cuda
 
     |sep|
 
     :Examples:
 
         BlurFFT operator with a basic averaging filter applied to a 16x16 black image with
         a single white pixel in the center:
 
+        >>> from deepinv.physics import BlurFFT
         >>> x = torch.zeros((1, 1, 16, 16)) # Define black image of size 16x16
         >>> x[:, :, 8, 8] = 1 # Define one white pixel in the middle
         >>> filter = torch.ones((1, 1, 2, 2)) / 4 # Basic 2x2 filter
-        >>> physics = BlurFFT(img_size=(1, 1, 16, 16), filter=filter)
+        >>> physics = BlurFFT(filter=filter, img_size=(1, 1, 16, 16))
         >>> y = physics(x)
+        >>> y[y<1e-5] = 0.
         >>> y[:, :, 7:10, 7:10] # Display the center of the blurred image
-        tensor([[[[ 2.5000e-01,  2.5000e-01, -3.1177e-10],
-                  [ 2.5000e-01,  2.5000e-01, -7.1280e-10],
-                  [-7.5937e-10, -5.4986e-10,  3.9221e-10]]]])
-
+        tensor([[[[0.2500, 0.2500, 0.0000],
+                  [0.2500, 0.2500, 0.0000],
+                  [0.0000, 0.0000, 0.0000]]]])
     """
 
     def __init__(self, img_size, filter, device="cpu", **kwargs):
         super().__init__(**kwargs)
+        self.device = device
         self.img_size = img_size
+        self.set_mask(filter)
 
-        if img_size[0] > filter.shape[1]:
-            filter = filter.repeat(1, img_size[0], 1, 1)
-
-        self.mask = filter_fft(filter, img_size).to("cpu")
-        self.angle = torch.angle(self.mask)
-        self.angle = torch.exp(-1j * self.angle).to(device)
-        self.mask = torch.abs(self.mask).unsqueeze(-1)
-        self.mask = torch.cat([self.mask, self.mask], dim=-1)
-
-        self.mask = torch.nn.Parameter(self.mask, requires_grad=False).to(device)
+    def set_mask(self, filter):
+        if self.img_size[0] > filter.shape[1]:
+            filter = filter.repeat(1, self.img_size[0], 1, 1)
+        self.filter = torch.nn.Parameter(filter, requires_grad=False).to(self.device)
+
+        mask = filter_fft_2d(filter, self.img_size).to(self.device)
+        self.angle = torch.angle(mask)
+        self.angle = torch.exp(-1.0j * self.angle).to(self.device)
+        mask = torch.abs(mask).unsqueeze(-1)
+        mask = torch.cat([mask, mask], dim=-1)
+        self.mask = torch.nn.Parameter(mask, requires_grad=False)
+
+    def A(self, x, filter=None, **kwargs):
+        if filter is not None:
+            self.set_mask(filter)
+        return super().A(x)
+
+    def A_adjoint(self, x, filter=None, **kwargs):
+        if filter is not None:
+            self.set_mask(filter)
+        return super().A_adjoint(x)
 
     def V_adjoint(self, x):
         return torch.view_as_real(
             fft.rfft2(x, norm="ortho")
         )  # make it a true SVD (see J. Romberg notes)
 
     def U(self, x):
         return fft.irfft2(
-            torch.view_as_complex(x) * self.angle, norm="ortho", s=self.img_size[-2:]
+            torch.view_as_complex(x) * self.angle,
+            norm="ortho",
+            s=self.img_size[-2:],
         )
 
     def U_adjoint(self, x):
         return torch.view_as_real(
             fft.rfft2(x, norm="ortho") * torch.conj(self.angle)
         )  # make it a true SVD (see J. Romberg notes)
 
     def V(self, x):
         return fft.irfft2(torch.view_as_complex(x), norm="ortho", s=self.img_size[-2:])
 
 
-# # test code
-# if __name__ == "__main__":
-#     device = "cuda:0"
-#
-#     import matplotlib.pyplot as plt
-#
-#     device = "cuda:0"
-#     x = torchvision.io.read_image("../../datasets/celeba/img_align_celeba/085307.jpg")
-#     x = x.unsqueeze(0).float().to(device) / 255
-#     x = torchvision.transforms.Resize((160, 180))(x)
-#
-#     sigma_noise = 0.0
-#     kernel = torch.zeros((1, 1, 15, 15), device=device)
-#     kernel[:, :, 7, :] = 1 / 15
-#     physics = Downsampling(img_size=x.shape[1:], filter="bilinear", device=device)
-#     physics2 = Blur(img_size=x.shape[1:], filter=kernel, device=device)
-#
-#     y = physics(x)
-#     y2 = physics2(x)
-#
-#     xhat = physics.V(physics.U_adjoint(y) / physics.mask)
-#     xhat2 = physics2.A_dagger(y2)
-#
-#     print(xhat.shape)
-#     # print(physics.adjointness_test(x))
-#     print(torch.sum((y - y2).pow(2)))
-#     print(torch.sum((xhat - xhat2).pow(2)))
-#
-#     print(torch.sum((x - xhat).pow(2)))
-#     print(torch.sum((x - xhat2).pow(2)))
-#
-#     print(physics.compute_norm(x))
-#     print(physics.adjointness_test(x))
-#     xhat = physics.prox_l2(y, y, gamma=1.0)
-#
-#     xhat = physics.A_dagger(y)
-#
-#     plt.imshow(x.squeeze(0).permute(1, 2, 0).cpu().numpy())
-#     plt.show()
-#     plt.imshow(y.squeeze(0).permute(1, 2, 0).cpu().numpy())
-#     plt.show()
-#     plt.imshow(xhat.squeeze(0).permute(1, 2, 0).cpu().numpy())
-#     plt.show()
-#     plt.imshow(xhat2.squeeze(0).permute(1, 2, 0).cpu().numpy())
-#     plt.show()
-#
-#     plt.imshow(physics.A(xhat).squeeze(0).permute(1, 2, 0).cpu().numpy())
-#     plt.show()
+class SpaceVaryingBlur(LinearPhysics):
+    r"""
+
+    Implements a space varying blur via product-convolution.
+
+    This operator performs
+
+    .. math::
+
+        y = \sum_{k=1}^K h_k \star (w_k \odot x)
+
+    where :math:`\star` is a convolution, :math:`\odot` is a Hadamard product,  :math:`w_k` are multipliers :math:`h_k` are filters.
+
+    :param torch.Tensor w: Multipliers :math:`w_k`. Tensor of size (K, b, c, H, W). b in {1, B} and c in {1, C}
+    :param torch.Tensor h: Filters :math:`h_k`. Tensor of size (K, b, c, h, w). b in {1, B} and c in {1, C}, h<=H and w<=W.
+    :param padding: options = ``'valid'``, ``'circular'``, ``'replicate'``, ``'reflect'``.
+        If ``padding = 'valid'`` the blurred output is smaller than the image (no padding),
+        otherwise the blurred output has the same size as the image.
+    :param str device: cpu or cuda
+
+    |sep|
+
+    :Examples:
+
+        We show how to instantiate a spatially varying blur operator.
+
+        >>> from deepinv.physics.generator import DiffractionBlurGenerator, ProductConvolutionBlurGenerator
+        >>> from deepinv.physics.blur import SpaceVaryingBlur
+        >>> from deepinv.utils.plotting import plot
+        >>> psf_size = 32
+        >>> img_size = (256, 256)
+        >>> delta = 16
+        >>> psf_generator = DiffractionBlurGenerator((psf_size, psf_size))
+        >>> pc_generator = ProductConvolutionBlurGenerator(psf_generator=psf_generator, img_size=img_size)
+        >>> params_pc = pc_generator.step(1)
+        >>> physics = SpaceVaryingBlur(**params_pc)
+        >>> dirac_comb = torch.zeros(img_size).unsqueeze(0).unsqueeze(0)
+        >>> dirac_comb[0,0,::delta,::delta] = 1
+        >>> psf_grid = physics(dirac_comb)
+        >>> plot(psf_grid, titles="Space varying impulse responses")
+
+    """
+
+    def __init__(self, filters=None, multipliers=None, padding=None, **kwargs):
+        super().__init__(**kwargs)
+        self.method = "product_convolution2d"
+        if self.method == "product_convolution2d":
+            self.set_params(filters, multipliers, padding)
+
+    def set_params(self, filters, multipliers, padding):
+        if filters is not None:
+            self.filters = torch.nn.Parameter(filters, requires_grad=False)
+        if multipliers is not None:
+            self.multipliers = torch.nn.Parameter(multipliers, requires_grad=False)
+        if padding is not None:
+            self.padding = padding
+
+    def A(
+        self, x: Tensor, filters=None, multipliers=None, padding=None, **kwargs
+    ) -> Tensor:
+        r"""
+        Applies the space varying blur operator to the input image.
+
+        It can receive new parameters  :math:`w_k`, :math:`h_k` and padding to be used in the forward operator, and stored
+        as the current parameters.
+
+        :param torch.Tensor filters: Multipliers :math:`w_k`. Tensor of size (K, b, c, H, W). b in {1, B} and c in {1, C}
+        :param torch.Tensor multipliers: Filters :math:`h_k`. Tensor of size (K, b, c, h, w). b in {1, B} and c in {1, C}, h<=H and w<=W
+        :param padding: options = ``'valid'``, ``'circular'``, ``'replicate'``, ``'reflect'``.
+            If `padding = 'valid'` the blurred output is smaller than the image (no padding),
+            otherwise the blurred output has the same size as the image.
+        :param str device: cpu or cuda
+        """
+        if self.method == "product_convolution2d":
+            self.set_params(filters, multipliers, padding)
+
+            return product_convolution2d(
+                x, self.multipliers, self.filters, self.padding
+            )
+        else:
+            raise NotImplementedError("Method not implemented in product-convolution")
+
+    def A_adjoint(
+        self, y: Tensor, filters=None, multipliers=None, padding=None, **kwargs
+    ) -> Tensor:
+        r"""
+        Applies the adjoint operator.
+
+        It can receive new parameters :math:`w_k`, :math:`h_k` and padding to be used in the forward operator, and stored
+        as the current parameters.
+
+        :param torch.Tensor h: Filters :math:`h_k`. Tensor of size (K, b, c, h, w). b in {1, B} and c in {1, C}, h<=H and w<=W
+        :param torch.Tensor w: Multipliers :math:`w_k`. Tensor of size (K, b, c, H, W). b in {1, B} and c in {1, C}
+        :param padding: options = ``'valid'``, ``'circular'``, ``'replicate'``, ``'reflect'``.
+            If `padding = 'valid'` the blurred output is smaller than the image (no padding),
+            otherwise the blurred output has the same size as the image.
+        :param str device: cpu or cuda
+        """
+        if self.method == "product_convolution2d":
+            self.set_params(filters, multipliers, padding)
+
+            return product_convolution2d_adjoint(
+                y, self.multipliers, self.filters, self.padding
+            )
+        else:
+            raise NotImplementedError("Method not implemented in product-convolution")
```

### Comparing `deepinv-0.1.1/deepinv/physics/compressed_sensing.py` & `deepinv-0.2.0/deepinv/physics/compressed_sensing.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def dst1(x):
     r"""
     Orthogonal Discrete Sine Transform, Type I
     The transform is performed across the last dimension of the input signal
     Due to orthogonality we have ``dst1(dst1(x)) = x``.
 
-    :param torch.tensor x: the input signal
+    :param torch.Tensor x: the input signal
     :return: (torch.tensor) the DST-I of the signal over the last dimension
 
     """
     x_shape = x.shape
 
     b = int(np.prod(x_shape[:-1]))
     n = x_shape[-1]
@@ -56,30 +56,37 @@
     .. note::
 
         If ``fast=False``, the forward operator has a norm which tends to :math:`(1+\sqrt{n/m})^2` for large :math:`n`
         and :math:`m` due to the `Marcenko-Pastur law
         <https://en.wikipedia.org/wiki/Marchenko%E2%80%93Pastur_distribution>`_.
         If ``fast=True``, the forward operator has a unit norm.
 
+    If ``dtype=torch.cfloat``, the forward operator will be generated as a random i.i.d. complex Gaussian matrix to be used with ``fast=False``
+
+    .. math::
+
+        A_{i,j} \sim \mathcal{N} \left( 0, \frac{1}{2m}) \right) + \mathrm{i} \mathcal{N} \left( 0, \frac{1}{2m} \right).
+
     :param int m: number of measurements.
     :param tuple img_shape: shape (C, H, W) of inputs.
     :param bool fast: The operator is iid Gaussian if false, otherwise A is a SORS matrix with the Discrete Sine Transform (type I).
     :param bool channelwise: Channels are processed independently using the same random forward operator.
-    :param torch.type dtype: Forward matrix is stored as a dtype.
+    :param torch.type dtype: Forward matrix is stored as a dtype. For complex matrices, use torch.cfloat. Default is torch.float.
     :param str device: Device to store the forward matrix.
 
     |sep|
 
     :Examples:
 
         Compressed sensing operator with 100 measurements for a 3x3 image:
 
+        >>> from deepinv.physics import CompressedSensing
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 1, 3, 3) # Define random 3x3 image
-        >>> physics = CompressedSensing(img_shape=(1, 3, 3), m=10)
+        >>> physics = CompressedSensing(m=10, img_shape=(1, 3, 3))
         >>> physics(x)
         tensor([[ 0.8522,  0.2133,  0.9897, -0.8714,  1.8953, -0.5284,  1.4422,  0.4238,
                   0.7754, -0.0479]])
 
     """
 
     def __init__(
@@ -112,25 +119,25 @@
             idx = np.sort(np.random.choice(self.n, size=m, replace=False))
             self.mask[torch.from_numpy(idx)] = 1
             self.mask = self.mask.type(torch.bool)
 
             self.D = torch.nn.Parameter(self.D, requires_grad=False)
             self.mask = torch.nn.Parameter(self.mask, requires_grad=False)
         else:
-            self._A = torch.randn((m, n), device=device) / np.sqrt(m)
+            self._A = torch.randn((m, n), device=device, dtype=dtype) / np.sqrt(m)
             self._A_dagger = torch.linalg.pinv(self._A)
             self._A = torch.nn.Parameter(self._A, requires_grad=False)
             self._A_dagger = torch.nn.Parameter(self._A_dagger, requires_grad=False)
             self._A_adjoint = (
-                torch.nn.Parameter(self._A.t(), requires_grad=False)
+                torch.nn.Parameter(self._A.conj().T, requires_grad=False)
                 .type(dtype)
                 .to(device)
             )
 
-    def A(self, x):
+    def A(self, x, **kwargs):
         N, C = x.shape[:2]
         if self.channelwise:
             x = x.reshape(N * C, -1)
         else:
             x = x.reshape(N, -1)
 
         if self.fast:
@@ -139,15 +146,16 @@
             y = torch.einsum("in, mn->im", x, self._A)
 
         if self.channelwise:
             y = y.view(N, C, -1)
 
         return y
 
-    def A_adjoint(self, y):
+    def A_adjoint(self, y, **kwargs):
+        y = y.type(self.dtype)
         N = y.shape[0]
         C, H, W = self.img_shape[0], self.img_shape[1], self.img_shape[2]
 
         if self.channelwise:
             N2 = N * C
             y = y.view(N2, -1)
         else:
@@ -159,15 +167,16 @@
             x = dst1(y2) * self.D
         else:
             x = torch.einsum("im, nm->in", y, self._A_adjoint)  # x:(N, n, 1)
 
         x = x.view(N, C, H, W)
         return x
 
-    def A_dagger(self, y):
+    def A_dagger(self, y, **kwargs):
+        y = y.type(self.dtype)
         if self.fast:
             return self.A_adjoint(y)
         else:
             N = y.shape[0]
             C, H, W = self.img_shape[0], self.img_shape[1], self.img_shape[2]
 
             if self.channelwise:
```

### Comparing `deepinv-0.1.1/deepinv/physics/forward.py` & `deepinv-0.2.0/deepinv/physics/forward.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import torch
 from deepinv.optim.utils import conjugate_gradient
 from deepinv.physics.noise import GaussianNoise
 from deepinv.utils import randn_like, TensorList
+from typing import Callable
 
 
-def adjoint_function(A, input_size, device="cpu"):
+def adjoint_function(A, input_size, device="cpu", dtype=torch.float):
     r"""
-    Provides adjoint function of a linear operator :math:`A`, i.e., :math:`A^{\top}`.
+    Provides the adjoint function of a linear operator :math:`A`, i.e., :math:`A^{\top}`.
 
 
-    The function can be simply called as ``A_adjoint(y)``, e.g.
+    The generated function can be simply called as ``A_adjoint(y)``, for example:
 
     >>> import torch
     >>> from deepinv.physics.forward import adjoint_function
     >>> A = lambda x: torch.roll(x, shifts=(1,1), dims=(2,3)) # shift image by one pixel
     >>> x = torch.randn((4, 1, 5, 5))
     >>> y = A(x)
     >>> A_adjoint = adjoint_function(A, (4, 1, 5, 5))
@@ -22,24 +23,24 @@
 
 
     :param callable A: linear operator :math:`A`.
     :param tuple input_size: size of the input tensor e.g. (B, C, H, W).
         The first dimension, i.e. batch size, should be equal or lower than the batch size B
         of the input tensor to the adjoint operator.
     :param str device: device where the adjoint operator is computed.
-    :return: (callable) function that computes the adjoint of :math:`A`.
+    :return: (Callable) function that computes the adjoint of :math:`A`.
 
     """
-    x = torch.ones(input_size, device=device)
+    x = torch.ones(input_size, device=device, dtype=dtype)
     (_, vjpfunc) = torch.func.vjp(A, x)
     batches = x.size()[0]
 
     def adjoint(y):
         if y.size()[0] < batches:
-            y2 = torch.zeros((batches,) + y.shape[1:], device=y.device)
+            y2 = torch.zeros((batches,) + y.shape[1:], device=y.device, dtype=y.dtype)
             y2[: y.size()[0], ...] = y
             return vjpfunc(y2)[0][: y.size()[0], ...]
         elif y.size()[0] > batches:
             raise ValueError("Batch size of A_adjoint input is larger than expected")
         else:
             return vjpfunc(y)[0]
 
@@ -57,31 +58,31 @@
         y = N(A(x))
 
     where :math:`x` is an image of :math:`n` pixels, :math:`y` is the measurements of size :math:`m`,
     :math:`A:\xset\mapsto \yset` is a deterministic mapping capturing the physics of the acquisition
     and :math:`N:\yset\mapsto \yset` is a stochastic mapping which characterizes the noise affecting
     the measurements.
 
-    :param callable A: forward operator function which maps an image to the observed measurements :math:`x\mapsto y`.
-    :param callable noise_model: function that adds noise to the measurements :math:`N(z)`.
+    :param Callable A: forward operator function which maps an image to the observed measurements :math:`x\mapsto y`.
+    :param Callable noise_model: function that adds noise to the measurements :math:`N(z)`.
         See the noise module for some predefined functions.
-    :param callable sensor_model: function that incorporates any sensor non-linearities to the sensing process,
+    :param Callable sensor_model: function that incorporates any sensor non-linearities to the sensing process,
         such as quantization or saturation, defined as a function :math:`\eta(z)`, such that
         :math:`y=\eta\left(N(A(x))\right)`. By default, the sensor_model is set to the identity :math:`\eta(z)=z`.
     :param int max_iter: If the operator does not have a closed form pseudoinverse, the gradient descent algorithm
         is used for computing it, and this parameter fixes the maximum number of gradient descent iterations.
     :param float tol: If the operator does not have a closed form pseudoinverse, the gradient descent algorithm
         is used for computing it, and this parameter fixes the absolute tolerance of the gradient descent algorithm.
 
     """
 
     def __init__(
         self,
-        A=lambda x: x,
-        noise_model=lambda x: x,
+        A=lambda x, **kwargs: x,
+        noise_model=lambda x, **kwargs: x,
         sensor_model=lambda x: x,
         max_iter=50,
         tol=1e-3,
     ):
         super().__init__()
         self.noise_model = noise_model
         self.sensor_model = sensor_model
@@ -127,16 +128,18 @@
 
         class noise(torch.nn.Module):
             def __init__(self, noise1, noise2):
                 super().__init__()
                 self.noise1 = noise1
                 self.noise2 = noise2
 
-            def forward(self, x):
-                return TensorList(self.noise1(x[:-1])).append(self.noise2(x[-1]))
+            def forward(self, x, **kwargs):
+                return TensorList(self.noise1(x[:-1], **kwargs)).append(
+                    self.noise2(x[-1], **kwargs)
+                )
 
         class sensor(torch.nn.Module):
             def __init__(self, sensor1, sensor2):
                 super().__init__()
                 self.sensor1 = sensor1
                 self.sensor2 = sensor2
 
@@ -147,86 +150,108 @@
             A=A,
             noise_model=noise(self.noise_model, other.noise_model),
             sensor_model=sensor(self.sensor_model, other.sensor_model),
             max_iter=self.max_iter,
             tol=self.tol,
         )
 
-    def reset(self, **kwargs):
-        if isinstance(self.noise_model, torch.nn.Module):
-            self.noise_model.__init__(**kwargs)
-
-    def forward(self, x):
+    def forward(self, x, **kwargs):
         r"""
-        Computes forward operator :math:`y = N(A(x))` (with noise and/or sensor non-linearities)
+        Computes forward operator
 
-        :param torch.Tensor,list[torch.Tensor] x: signal/image
+        .. math::
+
+                y = N(A(x), \sigma)
+
+
+        :param torch.Tensor, list[torch.Tensor] x: signal/image
         :return: (torch.Tensor) noisy measurements
 
         """
-        return self.sensor(self.noise(self.A(x)))
+        return self.sensor(self.noise(self.A(x, **kwargs), **kwargs))
 
-    def A(self, x):
+    def A(self, x, **kwargs):
         r"""
         Computes forward operator :math:`y = A(x)` (without noise and/or sensor non-linearities)
 
         :param torch.Tensor,list[torch.Tensor] x: signal/image
         :return: (torch.Tensor) clean measurements
 
         """
-        return self.forw(x)
+        return self.forw(x, **kwargs)
 
     def sensor(self, x):
         r"""
         Computes sensor non-linearities :math:`y = \eta(y)`
 
         :param torch.Tensor,list[torch.Tensor] x: signal/image
         :return: (torch.Tensor) clean measurements
         """
         return self.sensor_model(x)
 
-    def noise(self, x):
+    def noise(self, x, **kwargs):
         r"""
         Incorporates noise into the measurements :math:`\tilde{y} = N(y)`
 
         :param torch.Tensor x:  clean measurements
+        :param None, float noise_level: optional noise level parameter
         :return torch.Tensor: noisy measurements
 
         """
-        return self.noise_model(x)
+
+        return self.noise_model(x, **kwargs)
 
     def A_dagger(self, y, x_init=None):
         r"""
-        Computes an inverse of :math:`y = Ax` via gradient descent.
+        Computes an inverse as:
 
-        This function can be overwritten by a more efficient pseudoinverse in cases where closed form formulas exist.
+        .. math::
+
+            x^* \in \underset{x}{\arg\min} \quad \|\forw{x}-y\|^2.
+
+        This function uses gradient descent to find the inverse. It can be overwritten by a more efficient pseudoinverse in cases where closed form formulas exist.
 
         :param torch.Tensor y: a measurement :math:`y` to reconstruct via the pseudoinverse.
         :param torch.Tensor x_init: initial guess for the reconstruction.
         :return: (torch.Tensor) The reconstructed image :math:`x`.
 
         """
 
         if x_init is None:
             x_init = self.A_adjoint(y)
 
-        x = torch.nn.Parameter(x_init, requires_grad=True)
+        x = x_init
 
-        optimizer = torch.optim.SGD([x], lr=1e-1)
+        lr = 1e-1
         loss = torch.nn.MSELoss()
-        for i in range(self.max_iter):
+        for _ in range(self.max_iter):
+            x = x - lr * self.A_vjp(x, self.A(x) - y)
             err = loss(self.A(x), y)
-            optimizer.zero_grad()
-            err.backward(retain_graph=True)
-            optimizer.step()
             if err < self.tol:
                 break
 
         return x.clone()
 
+    def A_vjp(self, x, v):
+        r"""
+        Computes the product between a vector :math:`v` and the Jacobian of the forward operator :math:`A` evaluated at :math:`x`, defined as:
+
+        .. math::
+
+            A_{vjp}(x, v) = \left. \frac{\partial A}{\partial x}  \right|_x^\top  v.
+
+        By default, the Jacobian is computed using automatic differentiation.
+
+        :param torch.Tensor x: signal/image.
+        :param torch.Tensor v: vector.
+        :return: (torch.Tensor) the VJP product between :math:`v` and the Jacobian.
+        """
+        _, vjpfunc = torch.func.vjp(self.A, x)
+        return vjpfunc(v)[0]
+
 
 class LinearPhysics(Physics):
     r"""
     Parent class for linear operators.
 
     It describes the linear forward measurement process of the form
 
@@ -235,26 +260,26 @@
         y = N(A(x))
 
     where :math:`x` is an image of :math:`n` pixels, :math:`y` is the measurements of size :math:`m`,
     :math:`A:\xset\mapsto \yset` is a deterministic linear mapping capturing the physics of the acquisition
     and :math:`N:\yset\mapsto \yset` is a stochastic mapping which characterizes the noise affecting
     the measurements.
 
-    :param callable A: forward operator function which maps an image to the observed measurements :math:`x\mapsto y`.
+    :param Callable A: forward operator function which maps an image to the observed measurements :math:`x\mapsto y`.
         It is recommended to normalize it to have unit norm.
-    :param callable A_adjoint: transpose of the forward operator, which should verify the adjointness test.
+    :param Callable A_adjoint: transpose of the forward operator, which should verify the adjointness test.
 
         .. note::
 
-            A_adjoint can be generated automatically using the :meth:`deepinv.physics.LinearPhysics.compute_adjoint`
+            A_adjoint can be generated automatically using the :meth:`deepinv.physics.adjoint_function`
             method which relies on automatic differentiation, at the cost of a few extra computations per adjoint call.
 
-    :param callable noise_model: function that adds noise to the measurements :math:`N(z)`.
+    :param Callable noise_model: function that adds noise to the measurements :math:`N(z)`.
         See the noise module for some predefined functions.
-    :param callable sensor_model: function that incorporates any sensor non-linearities to the sensing process,
+    :param Callable sensor_model: function that incorporates any sensor non-linearities to the sensing process,
         such as quantization or saturation, defined as a function :math:`\eta(z)`, such that
         :math:`y=\eta\left(N(A(x))\right)`. By default, the sensor_model is set to the identity :math:`\eta(z)=z`.
     :param int max_iter: If the operator does not have a closed form pseudoinverse, the conjugate gradient algorithm
         is used for computing it, and this parameter fixes the maximum number of conjugate gradient iterations.
     :param float tol: If the operator does not have a closed form pseudoinverse, the conjugate gradient algorithm
         is used for computing it, and this parameter fixes the absolute tolerance of the conjugate gradient algorithm.
 
@@ -264,104 +289,122 @@
 
         Blur operator with a basic averaging filter applied to a 32x32 black image with
         a single white pixel in the center:
 
         >>> from deepinv.physics.blur import Blur, Downsampling
         >>> x = torch.zeros((1, 1, 32, 32)) # Define black image of size 32x32
         >>> x[:, :, 8, 8] = 1 # Define one white pixel in the middle
-        >>> w = torch.ones((1, 1, 2, 2)) / 4 # Basic 2x2 averaging filter
+        >>> w = torch.ones((1, 1, 3, 3)) / 9 # Basic 3x3 averaging filter
         >>> physics = Blur(filter=w)
         >>> y = physics(x)
 
         Linear operators can also be added. The measurements produced by the resulting
         model are :meth:`deepinv.utils.TensorList` objects, where each entry corresponds to the
         measurements of the corresponding operator:
 
         >>> physics1 = Blur(filter=w)
-        >>> physics2 = Downsampling(img_size=((1, 1, 32, 32)), filter="gaussian", factor=4)
+        >>> physics2 = Downsampling(img_size=((1, 32, 32)), filter="gaussian", factor=4)
         >>> physics = physics1 + physics2
         >>> y = physics(x)
 
         Linear operators can also be composed by multiplying them:
 
         >>> physics = physics1 * physics2
         >>> y = physics(x)
 
         Linear operators also come with an adjoint, a pseudoinverse, and proximal operators in a given norm:
 
         >>> from deepinv.utils import cal_psnr
         >>> x = torch.randn((1, 1, 16, 16)) # Define random 16x16 image
-        >>> physics = Blur(filter=w)
+        >>> physics = Blur(filter=w, padding='circular')
         >>> y = physics(x) # Compute measurements
         >>> x_dagger = physics.A_dagger(y) # Compute pseudoinverse
         >>> x_ = physics.prox_l2(y, torch.zeros_like(x), 0.1) # Compute prox at x=0
         >>> cal_psnr(x, x_dagger) > cal_psnr(x, y) # Should be closer to the orginal
         True
 
-        The adjoint can be generated automatically using the :meth:`deepinv.physics.LinearPhysics.compute_adjoint` method
+        The adjoint can be generated automatically using the :meth:`deepinv.physics.adjoint_function` method
         which relies on automatic differentiation, at the cost of a few extra computations per adjoint call:
 
+        >>> from deepinv.physics import LinearPhysics, adjoint_function
         >>> from deepinv.utils import cal_psnr
         >>> A = lambda x: torch.roll(x, shifts=(1,1), dims=(2,3)) # Shift image by one pixel
         >>> physics = LinearPhysics(A=A, A_adjoint=adjoint_function(A, (4, 1, 5, 5)))
         >>> x = torch.randn((4, 1, 5, 5))
         >>> y = physics(x)
         >>> torch.allclose(physics.A_adjoint(y), x) # We have A^T(A(x)) = x
         True
 
     """
 
     def __init__(
         self,
-        A=lambda x: x,
-        A_adjoint=lambda x: x,
-        noise_model=lambda x: x,
+        A=lambda x, **kwargs: x,
+        A_adjoint=lambda x, **kwargs: x,
+        noise_model=lambda x, **kwargs: x,
         sensor_model=lambda x: x,
         max_iter=50,
         tol=1e-3,
         **kwargs,
     ):
         super().__init__(
             A=A,
             noise_model=noise_model,
             sensor_model=sensor_model,
             max_iter=max_iter,
             tol=tol,
         )
         self.A_adj = A_adjoint
 
-    def A_adjoint(self, y):
+    def A_adjoint(self, y, **kwargs):
         r"""
         Computes transpose of the forward operator :math:`\tilde{x} = A^{\top}y`.
         If :math:`A` is linear, it should be the exact transpose of the forward matrix.
 
         .. note::
 
             If the problem is non-linear, there is not a well-defined transpose operation,
             but defining one can be useful for some reconstruction networks, such as ``deepinv.models.ArtifactRemoval``.
 
         :param torch.Tensor y: measurements.
+        :param None, torch.Tensor params: optional additional parameters for the adjoint operator.
         :return: (torch.Tensor) linear reconstruction :math:`\tilde{x} = A^{\top}y`.
 
         """
 
-        return self.A_adj(y)
+        return self.A_adj(y, **kwargs)
+
+    def A_vjp(self, x, v):
+        r"""
+        Computes the product between a vector :math:`v` and the Jacobian of the forward operator :math:`A` evaluated at :math:`x`, defined as:
+
+        .. math::
+
+            A_{vjp}(x, v) = \left. \frac{\partial A}{\partial x}  \right|_x^\top  v = \conj{A} v.
+
+        :param torch.Tensor x: signal/image.
+        :param torch.Tensor v: vector.
+        :return: (torch.Tensor) the VJP product between :math:`v` and the Jacobian.
+        """
+        return self.A_adjoint(v)
 
     def __mul__(self, other):
         r"""
         Concatenates two linear forward operators :math:`A = A_1\circ A_2` via the * operation
 
         The resulting linear operator keeps the noise and sensor models of :math:`A_1`.
 
         :param deepinv.physics.LinearPhysics other: Physics operator :math:`A_2`
         :return: (deepinv.physics.LinearPhysics) concatenated operator
 
         """
-        A = lambda x: self.A(other.A(x))  # (A' = A_1 A_2)
-        A_adjoint = lambda x: other.A_adjoint(self.A_adjoint(x))
+        A = lambda x, **kwargs: self.A(other.A(x, **kwargs), **kwargs)  # (A' = A_1 A_2)
+        A_adjoint = lambda x, **kwargs: other.A_adjoint(
+            self.A_adjoint(x, **kwargs), **kwargs
+        )
         noise = self.noise_model
         sensor = self.sensor_model
         return LinearPhysics(
             A=A,
             A_adjoint=A_adjoint,
             noise_model=noise,
             sensor_model=sensor,
@@ -381,28 +424,36 @@
             When using the ``__add__`` operator between two noise objects, the operation will retain only the second
             noise.
 
         :param deepinv.physics.LinearPhysics other: Physics operator :math:`A_2`
         :return: (deepinv.physics.LinearPhysics) stacked operator
 
         """
-        A = lambda x: TensorList(self.A(x)).append(TensorList(other.A(x)))
+        A = lambda x, **kwargs: TensorList(self.A(x, **kwargs)).append(
+            TensorList(other.A(x, **kwargs))
+        )
 
-        def A_adjoint(y):
-            at1 = self.A_adjoint(y[:-1]) if len(y) > 2 else self.A_adjoint(y[0])
-            return at1 + other.A_adjoint(y[-1])
+        def A_adjoint(y, **kwargs):
+            at1 = (
+                self.A_adjoint(y[:-1], **kwargs)
+                if len(y) > 2
+                else self.A_adjoint(y[0], **kwargs)
+            )
+            return at1 + other.A_adjoint(y[-1], **kwargs)
 
         class noise(torch.nn.Module):
             def __init__(self, noise1, noise2):
                 super().__init__()
                 self.noise1 = noise1
                 self.noise2 = noise2
 
-            def forward(self, x):
-                return TensorList(self.noise1(x[:-1])).append(self.noise2(x[-1]))
+            def forward(self, x, **kwargs):
+                return TensorList(self.noise1(x[:-1], **kwargs)).append(
+                    self.noise2(x[-1], **kwargs)
+                )
 
         class sensor(torch.nn.Module):
             def __init__(self, sensor1, sensor2):
                 super().__init__()
                 self.sensor1 = sensor1
                 self.sensor2 = sensor2
 
@@ -427,34 +478,34 @@
         using the `power method <https://en.wikipedia.org/wiki/Power_iteration>`_.
 
         :param torch.Tensor x0: initialisation point of the algorithm
         :param int max_iter: maximum number of iterations
         :param float tol: relative variation criterion for convergence
         :param bool verbose: print information
 
-        :returns z: (float) spectral norm of :math:`A^{\top}A`, i.e., :math:`\|A^{\top}A\|`.
+        :returns z: (float) spectral norm of :math:`\conj{A} A`, i.e., :math:`\|\conj{A} A\|`.
         """
         x = torch.randn_like(x0)
         x /= torch.norm(x)
         zold = torch.zeros_like(x)
         for it in range(max_iter):
             y = self.A(x)
             y = self.A_adjoint(y)
-            z = torch.matmul(x.reshape(-1), y.reshape(-1)) / torch.norm(x) ** 2
+            z = torch.matmul(x.conj().reshape(-1), y.reshape(-1)) / torch.norm(x) ** 2
 
             rel_var = torch.norm(z - zold)
             if rel_var < tol and verbose:
                 print(
                     f"Power iteration converged at iteration {it}, value={z.item():.2f}"
                 )
                 break
             zold = z
             x = y / torch.norm(y)
 
-        return z
+        return z.real
 
     def adjointness_test(self, u):
         r"""
         Numerically check that :math:`A^{\top}` is indeed the adjoint of :math:`A`.
 
         :param torch.Tensor u: initialisation point of the adjointness test method
 
@@ -465,25 +516,25 @@
         Au = self.A(u_in)
 
         if isinstance(Au, tuple) or isinstance(Au, list):
             V = [randn_like(au) for au in Au]
             Atv = self.A_adjoint(V)
             s1 = 0
             for au, v in zip(Au, V):
-                s1 += (v * au).flatten().sum()
+                s1 += (v.conj() * au).flatten().sum()
 
         else:
             v = randn_like(Au)
             Atv = self.A_adjoint(v)
 
-            s1 = (v * Au).flatten().sum()
+            s1 = (v.conj() * Au).flatten().sum()
 
-        s2 = (Atv * u_in).flatten().sum()
+        s2 = (Atv * u_in.conj()).flatten().sum()
 
-        return s1 - s2
+        return s1.conj() - s2
 
     def prox_l2(self, z, y, gamma):
         r"""
         Computes proximal operator of :math:`f(x) = \frac{1}{2}\|Ax-y\|^2`, i.e.,
 
         .. math::
 
@@ -496,18 +547,19 @@
 
         """
         b = self.A_adjoint(y) + 1 / gamma * z
         H = lambda x: self.A_adjoint(self.A(x)) + 1 / gamma * x
         x = conjugate_gradient(H, b, self.max_iter, self.tol)
         return x
 
-    def A_dagger(self, y):
+    def A_dagger(self, y, **kwargs):
         r"""
         Computes the solution in :math:`x` to :math:`y = Ax` using the
-        ` conjugate gradient method <https://en.wikipedia.org/wiki/Conjugate_gradient_method>`_.
+        `conjugate gradient method <https://en.wikipedia.org/wiki/Conjugate_gradient_method>`_,
+        see :meth:`deepinv.optim.utils.conjugate_gradient`.
 
         If the size of :math:`y` is larger than :math:`x` (overcomplete problem), it computes :math:`(A^{\top} A)^{-1} A^{\top} y`,
         otherwise (incomplete problem) it computes :math:`A^{\top} (A A^{\top})^{-1} y`.
 
         This function can be overwritten by a more efficient pseudoinverse in cases where closed form formulas exist.
 
         :param torch.Tensor y: a measurement :math:`y` to reconstruct via the pseudoinverse.
@@ -543,40 +595,42 @@
     .. math::
 
         A = U\text{diag}(s)V^{\top} \in \mathbb{R}^{m\times n}
 
     where :math:`U\in\mathbb{C}^{n\times n}` and :math:`V\in\mathbb{C}^{m\times m}`
     are orthonormal linear transformations and :math:`s\in\mathbb{R}_{+}^{n}` are the singular values.
 
-    :param callable U: orthonormal transformation
-    :param callable U_adjoint: transpose of U
-    :param callable V: orthonormal transformation
-    :param callable V_adjoint: transpose of V
-    :param torch.Tensor, float mask: Singular values of the transform
+    :param Callable U: orthonormal transformation
+    :param Callable U_adjoint: transpose of U
+    :param Callable V: orthonormal transformation
+    :param Callable V_adjoint: transpose of V
+    :param torch.nn.Parameter, float params: Singular values of the transform
 
     |sep|
 
     :Examples:
 
         Recreation of the Inpainting operator using the DecomposablePhysics class:
 
+        >>> from deepinv.physics import DecomposablePhysics
         >>> seed = torch.manual_seed(0)  # Random seed for reproducibility
         >>> tensor_size = (1, 1, 3, 3)  # Input size
         >>> mask = torch.tensor([[1, 0, 1], [1, 0, 1], [1, 0, 1]])  # Binary mask
         >>> U = lambda x: x  # U is the identity operation
         >>> U_adjoint = lambda x: x  # U_adjoint is the identity operation
         >>> V = lambda x: x  # V is the identity operation
         >>> V_adjoint = lambda x: x  # V_adjoint is the identity operation
         >>> mask_svd = mask.float().unsqueeze(0).unsqueeze(0)  # Convert the mask to torch.Tensor and adjust its dimensions
         >>> physics = DecomposablePhysics(U=U, U_adjoint=U_adjoint, V=V, V_adjoint=V_adjoint, mask=mask_svd)
 
         Apply the operator to a random tensor:
 
         >>> x = torch.randn(tensor_size)
-        >>> physics.A(x)  # Apply the masking
+        >>> with torch.no_grad():
+        ...     physics.A(x)  # Apply the masking
         tensor([[[[ 1.5410, -0.0000, -2.1788],
                   [ 0.5684, -0.0000, -1.3986],
                   [ 0.4033,  0.0000, -0.7193]]]])
 
     """
 
     def __init__(
@@ -589,39 +643,70 @@
         **kwargs,
     ):
         super().__init__(**kwargs)
         self._V = V
         self._U = U
         self._U_adjoint = U_adjoint
         self._V_adjoint = V_adjoint
-        self.mask = mask
+        self.mask = torch.nn.Parameter(
+            torch.tensor(mask) if not isinstance(mask, torch.Tensor) else mask,
+            requires_grad=False,
+        )
+
+    def A(self, x, mask=None, **kwargs):
+        r"""
+        Applies the forward operator :math:`y = A(x)`.
+
+        If a mask/singular values is provided, it is used to apply the forward operator,
+        and also stored as the current mask/singular values.
+
+        :param torch.Tensor x: input tensor
+        :param torch.nn.Parameter, float mask: singular values.
+        :return: (torch.Tensor) output tensor
+
+        """
+        if mask is not None:
+            self.mask = torch.nn.Parameter(mask, requires_grad=False)
 
-    def A(self, x):
         return self.U(self.mask * self.V_adjoint(x))
 
+    def A_adjoint(self, y, mask=None, **kwargs):
+        r"""
+        Computes the adjoint of the forward operator :math:`\tilde{x} = A^{\top}y`.
+
+        If a mask/singular values is provided, it is used to apply the adjoint operator,
+        and also stored as the current mask/singular values.
+
+        :param torch.Tensor y: input tensor
+        :param torch.nn.Parameter, float mask: singular values.
+        :return: (torch.Tensor) output tensor
+        """
+
+        if mask is not None:
+            self.mask = mask
+
+        if isinstance(self.mask, float):
+            mask = self.mask
+        else:
+            mask = torch.conj(self.mask)
+
+        return self.V(mask * self.U_adjoint(y))
+
     def U(self, x):
         return self._U(x)
 
     def V(self, x):
         return self._U(x)
 
     def U_adjoint(self, x):
         return self._U_adjoint(x)
 
     def V_adjoint(self, x):
         return self._V_adjoint(x)
 
-    def A_adjoint(self, y):
-        if isinstance(self.mask, float):
-            mask = self.mask
-        else:
-            mask = torch.conj(self.mask)
-
-        return self.V(mask * self.U_adjoint(y))
-
     def prox_l2(self, z, y, gamma):
         r"""
         Computes proximal operator of :math:`f(x)=\frac{\gamma}{2}\|Ax-y\|^2`
         in an efficient manner leveraging the singular vector decomposition.
 
         :param torch.Tensor y: measurements tensor
         :param torch.Tensor, float z: signal tensor
@@ -633,15 +718,15 @@
         if isinstance(self.mask, float):
             scaling = self.mask**2 + 1 / gamma
         else:
             scaling = torch.conj(self.mask) * self.mask + 1 / gamma
         x = self.V(self.V_adjoint(b) / scaling)
         return x
 
-    def A_dagger(self, y):
+    def A_dagger(self, y, **kwargs):
         r"""
         Computes :math:`A^{\dagger}y = x` in an efficient manner leveraging the singular vector decomposition.
 
         :param torch.Tensor y: a measurement :math:`y` to reconstruct via the pseudoinverse.
         :return: (torch.Tensor) The reconstructed image :math:`x`.
 
         """
@@ -673,15 +758,16 @@
         Denoising operator with Gaussian noise with standard deviation 0.1:
 
         >>> from deepinv.physics import Denoising, GaussianNoise
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = 0.5*torch.randn(1, 1, 3, 3) # Define random 3x3 image
         >>> physics = Denoising()
         >>> physics.noise_model = GaussianNoise(sigma=0.1)
-        >>> physics(x)
+        >>> with torch.no_grad():
+        ...     physics(x)
         tensor([[[[ 0.7302, -0.2064, -1.0712],
                   [ 0.1985, -0.4322, -0.8064],
                   [ 0.2139,  0.3624, -0.3223]]]])
 
     """
 
     def __init__(self, noise=GaussianNoise(sigma=0.1), **kwargs):
```

### Comparing `deepinv-0.1.1/deepinv/physics/haze.py` & `deepinv-0.2.0/deepinv/physics/haze.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,41 +25,41 @@
     """
 
     def __init__(self, beta=0.1, offset=0, **kwargs):
         super().__init__(**kwargs)
         self.beta = beta
         self.offset = offset
 
-    def A(self, x):
+    def A(self, x, **kwargs):
         r"""
         :param list, tuple x:  The input x should be a tuple/list such that x[0] = image torch.tensor :math:`I`,
          x[1] = depth torch.tensor :math:`d`, x[2] = scalar or torch.tensor of one element :math:`a`.
         :return: (torch.tensor) hazy image.
 
         """
         im = x[0]
         d = x[1]
         A = x[2]
 
         t = torch.exp(-self.beta * (d + self.offset))
         y = t * im + (1 - t) * A
         return y
 
-    def A_dagger(self, y):
+    def A_dagger(self, y, **kwargs):
         r"""
 
         Returns the trivial inverse where x[0] = y (trivial estimate of the image :math:`I`),
         x[1] = tensor of depth :math:`d` equal to one, x[2] = 1 for :math:`a`.
 
         .. note:
 
             This trivial inverse can be useful for some reconstruction networks, such as ``deepinv.models.ArtifactRemoval``.
 
 
-        :param torch.tensor y: Hazy image.
+        :param torch.Tensor y: Hazy image.
         :return: (deepinv.utils.ListTensor) trivial inverse.
 
         """
         b, c, h, w = y.shape
         d = torch.ones((b, 1, h, w), device=y.device)
         A = torch.ones(1, device=y.device)
         return TensorList([y, d, A])
```

### Comparing `deepinv-0.1.1/deepinv/physics/inpainting.py` & `deepinv-0.2.0/deepinv/physics/inpainting.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,70 +17,72 @@
 
     This operator is linear and has a trivial SVD decomposition, which allows for fast computation
     of the pseudo-inverse and proximal operator.
 
     An existing operator can be loaded from a saved ``.pth`` file via ``self.load_state_dict(save_path)``,
     in a similar fashion to ``torch.nn.Module``.
 
-    :param tuple tensor_size: size of the input images, e.g., (C, H, W).
-    :param torch.tensor, float mask: If the input is a float, the entries of the mask will be sampled from a bernoulli
+    :param torch.Tensor, float mask: If the input is a float, the entries of the mask will be sampled from a bernoulli
         distribution with probability equal to ``mask``. If the input is a ``torch.tensor`` matching tensor_size,
         the mask will be set to this tensor.
+    :param tuple tensor_size: size of the input images, e.g., (C, H, W).
     :param torch.device device: gpu or cpu
     :param bool pixelwise: Apply the mask in a pixelwise fashion, i.e., zero all channels in a given pixel simultaneously.
 
     |sep|
 
     :Examples:
 
         Inpainting operator using defined mask, removing the second column of a 3x3 image:
 
+        >>> from deepinv.physics import Inpainting
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 1, 3, 3) # Define random 3x3 image
-        >>> m = torch.zeros(1, 3, 3) # Define empty mask
-        >>> m[:, 2, :] = 1 # Keeping last line only
-        >>> physics = Inpainting(tensor_size=(1, 1, 3, 3), mask=m)
+        >>> mask = torch.zeros(1, 3, 3) # Define empty mask
+        >>> mask[:, 2, :] = 1 # Keeping last line only
+        >>> physics = Inpainting(mask=mask, tensor_size=(1, 1, 3, 3))
         >>> physics(x)
         tensor([[[[ 0.0000, -0.0000, -0.0000],
                   [ 0.0000, -0.0000, -0.0000],
                   [ 0.4033,  0.8380, -0.7193]]]])
 
         Inpainting operator using random mask, keeping 70% of the entries of a 3x3 image:
 
+        >>> from deepinv.physics import Inpainting
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 3, 3) # Define random 3x3 image
-        >>> physics = Inpainting(tensor_size=(1, 1, 3, 3), mask=0.7)
+        >>> physics = Inpainting(mask=0.7, tensor_size=(1, 1, 3, 3))
         >>> physics(x)
         tensor([[[[[ 1.5410, -0.0000, -2.1788],
                    [ 0.0000, -1.0845, -1.3986],
                    [ 0.0000,  0.8380, -0.7193]]]]])
 
     """
 
-    def __init__(self, tensor_size, mask=0.3, pixelwise=True, device="cpu", **kwargs):
+    def __init__(self, tensor_size, mask, pixelwise=True, device="cpu", **kwargs):
         super().__init__(**kwargs)
-        self.tensor_size = tensor_size
-
-        if isinstance(mask, torch.Tensor):  # check if the user created mask
-            self.mask = mask
-        else:  # otherwise create new random mask
+        if isinstance(mask, torch.nn.Parameter) or isinstance(mask, torch.Tensor):
+            mask = mask.to(device)
+        elif type(mask) == float:
             mask_rate = mask
-            self.mask = torch.ones(tensor_size, device=device)
-            aux = torch.rand_like(self.mask)
+            mask = torch.ones(tensor_size, device=device)
+            aux = torch.rand_like(mask)
             if not pixelwise:
-                self.mask[aux > mask_rate] = 0
+                mask[aux > mask_rate] = 0
             else:
-                self.mask[:, aux[0, :, :] > mask_rate] = 0
+                mask[:, aux[0, :, :] > mask_rate] = 0
 
-        self.mask = torch.nn.Parameter(self.mask.unsqueeze(0), requires_grad=False)
+        self.mask = torch.nn.Parameter(mask.unsqueeze(0), requires_grad=False)
 
-    def noise(self, x):
+    def noise(self, x, **kwargs):
         r"""
         Incorporates noise into the measurements :math:`\tilde{y} = N(y)`
 
         :param torch.Tensor x:  clean measurements
         :return torch.Tensor: noisy measurements
         """
         noise = self.U(
-            self.V_adjoint(self.V(self.U_adjoint(self.noise_model(x)) * self.mask))
+            self.V_adjoint(
+                self.V(self.U_adjoint(self.noise_model(x, **kwargs)) * self.mask)
+            )
         )
         return noise
```

### Comparing `deepinv-0.1.1/deepinv/physics/lidar.py` & `deepinv-0.2.0/deepinv/physics/lidar.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,36 +41,36 @@
         h = ((self.grid - 3 * sigma) / self.sigma).pow(2)
         h = torch.exp(-h / 2.0)
         h = h[: int(6 * sigma)]
         h = h / h.sum()
         self.irf = h.unsqueeze(0).unsqueeze(0)  # set impulse response function
         self.grid = self.grid.unsqueeze(0).unsqueeze(2).unsqueeze(3)
 
-    def A(self, x):
+    def A(self, x, **kwargs):
         r"""
         Applies the forward operator.
 
         Input is of size (B, 3, H, W) and output is of size (B, bins, H, W)
 
-        :param torch.tensor x: tensor containing the depth, intensity and background noise levels.
+        :param torch.Tensor x: tensor containing the depth, intensity and background noise levels.
         """
 
         h = ((self.grid - x[:, 0, :, :]) / self.sigma).pow(2)
         h = torch.exp(-h / 2.0)
         h = h / h.sum(dim=1, keepdim=True)
         y = x[:, 1, :, :] * h + x[:, 2, :, :]
         return y
 
-    def A_dagger(self, y):
+    def A_dagger(self, y, **kwargs):
         r"""
         Applies Matched filtering to find the peaks.
 
         Input is of size (B, bins, H, W), output of size (B, 3, H, W).
 
-        :param torch.tensor y: measurements
+        :param torch.Tensor y: measurements
         """
         B, T, H, W = y.shape
 
         # reshape to (B*H*W, 1, T)
         y = y.permute(0, 2, 3, 1).reshape(B * H * W, 1, T)
 
         # Apply irf using convolution
```

### Comparing `deepinv-0.1.1/deepinv/physics/mri.py` & `deepinv-0.2.0/deepinv/physics/mri.py`

 * *Files 27% similar despite different names*

```diff
@@ -18,78 +18,53 @@
     where :math:`S` applies a mask (subsampling operator), and :math:`F` is the 2D discrete Fourier Transform.
     This operator has a simple singular value decomposition, so it inherits the structure of
     :meth:`deepinv.physics.DecomposablePhysics` and thus have a fast pseudo-inverse and prox operators.
 
     The complex images :math:`x` and measurements :math:`y` should be of size (B, 2, H, W) where the first channel corresponds to the real part
     and the second channel corresponds to the imaginary part.
 
-    :param torch.tensor mask: the mask values should be binary.
+    :param torch.Tensor mask: binary mask.
         The mask size should be of the form (H,W) where H is the image height and W is the image width.
     :param torch.device device: cpu or gpu.
 
     |sep|
 
     :Examples:
 
         Single-coil MRI operator with 4x acceleration:
 
+        >>> from deepinv.physics import MRI
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 2, 3, 3) # Define random 3x3 image
         >>> mask = torch.ones((3, 3))
         >>> mask[:, ::2] = 0
         >>> physics = MRI(mask=mask)
         >>> physics(x)
         tensor([[-0.5305,  0.0351,  0.3326,  2.1730,  1.7072,  0.0418]])
 
     """
 
     def __init__(
         self,
-        mask=None,
-        image_size=(320, 320),
-        acceleration_factor=4,
+        mask,
+        img_size=(320, 320),
         device="cpu",
-        seed=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.device = device
-        self.image_size = image_size
+        self.img_size = img_size
 
-        if mask is not None:
-            mask = mask.to(device).unsqueeze(0).unsqueeze(0)
-        else:
-            mask = (
-                self.sample_mask(
-                    image_size=image_size,
-                    acceleration_factor=acceleration_factor,
-                    seed=seed,
-                )
-                .unsqueeze(0)
-                .unsqueeze(0)
-            )
+        mask = mask.to(device)
+        if len(mask.shape) == 2:
+            mask = mask.unsqueeze(0).unsqueeze(0)
 
         self.mask = torch.nn.Parameter(
             torch.cat([mask, mask], dim=1), requires_grad=False
-        )
-
-    def reset(self, **kwargs):
-        r"""
-        Resets the physics, i.e. re-samples a new mask and new noise realization (if any).
-        """
-        super().reset(**kwargs)
-        mask = (
-            self.sample_mask(image_size=self.image_size, **kwargs)
-            .unsqueeze(0)
-            .unsqueeze(0)
-        )
-
-        self.mask = torch.nn.Parameter(
-            torch.cat([mask, mask], dim=1), requires_grad=False
-        )
+        ).to(device)
 
     def V_adjoint(self, x):  # (B, 2, H, W) -> (B, H, W, 2)
         y = fft2c_new(x.permute(0, 2, 3, 1)).permute(0, 3, 1, 2)
         return y
 
     def U(self, x):
         return x[:, self.mask.squeeze(0) > 0]
@@ -100,56 +75,21 @@
         out[:, self.mask.squeeze(0) > 0] = x
         return out
 
     def V(self, x):  # (B, 2, H, W) -> (B, H, W, 2)
         x = x.permute(0, 2, 3, 1)
         return ifft2c_new(x).permute(0, 3, 1, 2)
 
-    def sample_mask(self, image_size=(320, 320), acceleration_factor=4, seed=None):
-        r"""
-        Create a mask of vertical lines.
-
-        :param tuple image_size: image size.
-        :param int acceleration_factor: acceleration factor.
-        :param int seed: random seed.
-        :return: mask of size (H, W) with values in {0, 1}.
-        """
-        if seed is not None:
-            np.random.seed(seed)
-        if acceleration_factor == 4:
-            central_lines_percent = 0.08
-            num_lines_center = int(central_lines_percent * image_size[-1])
-            side_lines_percent = 0.25 - central_lines_percent
-            num_lines_side = int(side_lines_percent * image_size[-1])
-        if acceleration_factor == 8:
-            central_lines_percent = 0.04
-            num_lines_center = int(central_lines_percent * image_size[-1])
-            side_lines_percent = 0.125 - central_lines_percent
-            num_lines_side = int(side_lines_percent * image_size[-1])
-        mask = torch.zeros(image_size)
-        center_line_indices = torch.linspace(
-            image_size[0] // 2 - num_lines_center // 2,
-            image_size[0] // 2 + num_lines_center // 2 + 1,
-            steps=50,
-            dtype=torch.long,
-        )
-        mask[:, center_line_indices] = 1
-        random_line_indices = np.random.choice(
-            image_size[0], size=(num_lines_side // 2,), replace=False
-        )
-        mask[:, random_line_indices] = 1
-        return mask.float().to(self.device)
-
 
 #
 # reference: https://github.com/facebookresearch/fastMRI/blob/main/fastmri/fftc.py
 def fft2c_new(data: torch.Tensor, norm: str = "ortho") -> torch.Tensor:
     r"""
     Apply centered 2 dimensional Fast Fourier Transform.
-    :param torch.tensor data: Complex valued input data containing at least 3 dimensions:
+    :param torch.Tensor data: Complex valued input data containing at least 3 dimensions:
         dimensions -2 & -1 are spatial dimensions and dimension -3 has size
         2. All other dimensions are assumed to be batch dimensions.
     :param bool norm: Normalization mode. See ``torch.fft.fft``.
     :return: (torch.tensor) the FFT of the input.
     """
     if not data.shape[-1] == 2:
         raise ValueError("Tensor does not have separate complex dim.")
@@ -285,15 +225,15 @@
 #         device,
 #     )
 #     import deepinv as dinv
 #     from fastmri.data import subsample
 #
 #     imsize = (25, 32)
 #     # Create a mask function
-#     mask_func = subsample.RandomMaskFunc(center_fractions=[0.08], accelerations=[4])
+#     mask_func = subsample.RandommaskFunc(center_fractions=[0.08], accelerations=[4])
 #     m = mask_func.sample_mask((imsize[1], imsize[0]), offset=None)
 #
 #     # mask = torch.ones((imsize[0], 1)) * (m[0] + m[1]).permute(1, 0)
 #     mask = torch.ones(imsize)
 #     mask[mask > 1] = 1
 #
 #     sigma = 0.1
```

### Comparing `deepinv-0.1.1/deepinv/physics/range.py` & `deepinv-0.2.0/deepinv/physics/range.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,27 +13,28 @@
 
     |sep|
 
     :Examples:
 
         Decolorize a 3x3 image:
 
+        >>> from deepinv.physics import Decolorize
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 3, 3, 3) # Define random 3x3 RGB image
         >>> physics = Decolorize()
-        >>> physics(x)
+        >>> with torch.no_grad():
+        ...     physics(x)
         tensor([[[[-1.1343, -0.1329,  0.1517],
                   [-0.0790,  0.6711, -0.1414],
                   [-0.1716, -0.9021,  0.0819]]]])
 
     """
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.mask = 1.0
 
     def V_adjoint(self, x):
         y = x[:, 0, :, :] * 0.2989 + x[:, 1, :, :] * 0.5870 + x[:, 2, :, :] * 0.1140
         return y.unsqueeze(1)
 
     def V(self, y):
         return torch.cat([y * 0.2989, y * 0.5870, y * 0.1140], dim=1)
```

### Comparing `deepinv-0.1.1/deepinv/physics/remote_sensing.py` & `deepinv-0.2.0/deepinv/physics/remote_sensing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import torch
-import numpy as np
 from deepinv.physics.noise import GaussianNoise
 from deepinv.physics.forward import LinearPhysics
 from deepinv.physics.blur import Downsampling
 from deepinv.physics.range import Decolorize
 from deepinv.utils import TensorList
 
 
@@ -16,49 +15,52 @@
     element is the grayscale image.
 
     By default, the downsampling is done with a gaussian filter with standard deviation equal to the downsampling,
     however, the user can provide a custom downsampling filter.
 
     It is possible to assign a different noise model to the RGB and grayscale images.
 
+
     :param tuple[int] img_size: size of the input image.
+    :param torch.Tensor, str, NoneType filter: Downsampling filter. It can be 'gaussian', 'bilinear' or 'bicubic' or a
+        custom ``torch.Tensor`` filter. If ``None``, no filtering is applied.
     :param int factor: downsampling factor.
     :param torch.nn.Module noise_color: noise model for the RGB image.
     :param torch.nn.Module noise_gray: noise model for the grayscale image.
-    :param torch.Tensor, str, NoneType filter: Downsampling filter. It can be 'gaussian', 'bilinear' or 'bicubic' or a
-        custom ``torch.Tensor`` filter. If ``None``, no filtering is applied.
+
     :param str padding: options are ``'valid'``, ``'circular'``, ``'replicate'`` and ``'reflect'``.
         If ``padding='valid'`` the blurred output is smaller than the image (no padding)
         otherwise the blurred output has the same size as the image.
 
     |sep|
 
     :Examples:
 
         Pansharpen operator applied to a random 32x32 image:
 
+        >>> from deepinv.physics import Pansharpen
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn(1, 3, 32, 32) # Define random 32x32 image
         >>> physics = Pansharpen(img_size=x.shape[1:], device=x.device)
         >>> physics(x)[0][:, :, 0, :3] # Display first pixels of RGB image
-        tensor([[[-0.0009, -0.0251, -0.0411],
-                 [-0.1576, -0.1098, -0.0340],
-                 [ 0.0086, -0.0257, -0.0856]]])
+        tensor([[[-0.1291,  0.0594, -0.1425],
+                 [-0.3199, -0.2397,  0.1460],
+                 [ 0.0975, -0.0053, -0.0941]]])
         >>> physics(x)[1][:, :, 0, :3] # Display first pixels of grayscale image
         tensor([[[-0.9084, -0.2966, -0.4015]]])
 
     """
 
     def __init__(
         self,
         img_size,
+        filter="bilinear",
         factor=4,
         noise_color=GaussianNoise(sigma=0.0),
         noise_gray=GaussianNoise(sigma=0.05),
-        filter="gaussian",
         device="cpu",
         padding="circular",
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         self.downsampling = Downsampling(
@@ -69,23 +71,30 @@
             padding=padding,
         )
 
         self.noise_color = noise_color
         self.noise_gray = noise_gray
         self.colorize = Decolorize()
 
-    def A(self, x):
-        return TensorList([self.downsampling.A(x), self.colorize.A(x)])
+    def A(self, x, **kwargs):
+        return TensorList(
+            [self.downsampling.A(x, **kwargs), self.colorize.A(x, **kwargs)]
+        )
 
-    def A_adjoint(self, y):
-        return self.downsampling.A_adjoint(y[0]) + self.colorize.A_adjoint(y[1])
+    def A_adjoint(self, y, **kwargs):
+        return self.downsampling.A_adjoint(y[0], **kwargs) + self.colorize.A_adjoint(
+            y[1], **kwargs
+        )
 
-    def forward(self, x):
+    def forward(self, x, **kwargs):
         return TensorList(
-            [self.noise_color(self.downsampling(x)), self.noise_gray(self.colorize(x))]
+            [
+                self.noise_color(self.downsampling(x, **kwargs)),
+                self.noise_gray(self.colorize(x, **kwargs)),
+            ]
         )
 
 
 # test code
 # if __name__ == "__main__":
 #     device = "cuda:0"
 #     import torch
```

### Comparing `deepinv-0.1.1/deepinv/physics/singlepixel.py` & `deepinv-0.2.0/deepinv/physics/singlepixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,25 +51,26 @@
 
     It is recommended to use ``fast=True`` for image sizes bigger than 32 x 32, since the forward computation with
     ``fast=False`` has an :math:`O(mn)` complexity, whereas with ``fast=True`` it has an :math:`O(n \log n)` complexity.
 
     An existing operator can be loaded from a saved ``.pth`` file via ``self.load_state_dict(save_path)``,
     in a similar fashion to :meth:`torch.nn.Module`.
 
-    :param int m: number of single pixel measurements per acquisition.
+    :param int m: number of single pixel measurements per acquisition (m).
     :param tuple img_shape: shape (C, H, W) of images.
     :param bool fast: The operator is iid binary if false, otherwise A is a 2D subsampled hadamard transform.
     :param str device: Device to store the forward matrix.
 
     |sep|
 
     :Examples:
 
         SinglePixelCamera operators with 16 binary patterns for 32x32 image:
 
+        >>> from deepinv.physics import SinglePixelCamera
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
         >>> x = torch.randn((1, 1, 32, 32)) # Define random 32x32 image
         >>> physics = SinglePixelCamera(m=16, img_shape=(1, 32, 32), fast=True)
         >>> torch.sum(physics.mask).item() # Number of measurements
         48.0
         >>> torch.round(physics(x)[:, :, :3, :3]).abs() # Compute measurements
         tensor([[[[1., 0., 0.],
@@ -100,30 +101,30 @@
 
             mask = torch.zeros(img_shape).unsqueeze(0)
             for i in range(len(revi)):
                 for j in range(len(revj)):
                     mask[0, :, revi[i], revj[j]] = 1
 
             mask = mask.to(device)
-            self.mask = torch.nn.Parameter(mask, requires_grad=False)
 
         else:
             n = int(np.prod(img_shape[1:]))
             A = torch.ones((m, n), device=device)
             A[torch.randn_like(A) > 0.5] = -1.0
             A /= np.sqrt(m)  # normalize
             u, mask, vh = torch.linalg.svd(A, full_matrices=False)
 
-            self.mask = mask.to(device).unsqueeze(0).type(dtype)
+            mask = mask.to(device).unsqueeze(0).type(dtype)
             self.vh = vh.to(device).type(dtype)
             self.u = u.to(device).type(dtype)
 
             self.u = torch.nn.Parameter(self.u, requires_grad=False)
             self.vh = torch.nn.Parameter(self.vh, requires_grad=False)
-            self.mask = torch.nn.Parameter(self.mask, requires_grad=False)
+
+        self.mask = torch.nn.Parameter(mask, requires_grad=False)
 
     def V_adjoint(self, x):
         if self.fast:
             y = hadamard_2d(x)
         else:
             N, C = x.shape[0], self.img_shape[0]
             x = x.reshape(N, C, -1)
```

### Comparing `deepinv-0.1.1/deepinv/sampling/diffusion.py` & `deepinv-0.2.0/deepinv/sampling/diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,20 +83,22 @@
     |sep|
 
     :Examples:
 
         Denoising diffusion restoration model using a pretrained DRUNet denoiser:
 
         >>> import deepinv as dinv
-        >>> device = dinv.utils.get_freer_gpu() if torch.cuda.is_available() else 'cpu'
+        >>> device = dinv.utils.get_freer_gpu(verbose=False) if torch.cuda.is_available() else 'cpu'
         >>> seed = torch.manual_seed(0) # Random seed for reproducibility
-        >>> x = 0.5 * torch.ones(1, 3, 32, 32) # Define plain gray 32x32 image
+        >>> seed = torch.cuda.manual_seed(0) # Random seed for reproducibility on GPU
+        >>> x = 0.5 * torch.ones(1, 3, 32, 32, device=device) # Define plain gray 32x32 image
         >>> physics = dinv.physics.Inpainting(
         ...   mask=0.5, tensor_size=(3, 32, 32),
-        ...   noise_model=dinv.physics.GaussianNoise(0.1)
+        ...   noise_model=dinv.physics.GaussianNoise(0.1),
+        ...   device=device,
         ... )
         >>> y = physics(x) # measurements
         >>> denoiser = dinv.models.DRUNet(pretrained="download").to(device)
         >>> model = dinv.sampling.DDRM(denoiser=denoiser, sigmas=np.linspace(1, 0, 10), verbose=True) # define the DDRM model
         >>> xhat = model(y, physics) # sample from the posterior distribution
         >>> dinv.utils.cal_psnr(xhat, x) > dinv.utils.cal_psnr(y, x) # Should be closer to the original
         True
@@ -247,26 +249,26 @@
     |sep|
 
     :Examples:
 
         Denoising diffusion restoration model using a pretrained DRUNet denoiser:
 
         >>> import deepinv as dinv
-        >>> device = dinv.utils.get_freer_gpu() if torch.cuda.is_available() else 'cpu'
-        >>> seed = torch.manual_seed(0) # Random seed for reproducibility
-        >>> x = 0.5 * torch.ones(1, 3, 32, 32) # Define a plain gray 32x32 image
+        >>> device = dinv.utils.get_freer_gpu(verbose=False) if torch.cuda.is_available() else 'cpu' 
+        >>> x = 0.5 * torch.ones(1, 3, 32, 32, device=device) # Define a plain gray 32x32 image
         >>> physics = dinv.physics.Inpainting(
         ...   mask=0.5, tensor_size=(3, 32, 32),
-        ...   noise_model=dinv.physics.GaussianNoise(0.1)
+        ...   noise_model=dinv.physics.GaussianNoise(0.1),
+        ...   device=device
         ... )
         >>> y = physics(x) # Measurements
         >>> denoiser = dinv.models.DRUNet(pretrained="download").to(device)
         >>> model = DiffPIR(
         ...   model=denoiser,
-        ...   data_fidelity=dinv.optim.L2(),
+        ...   data_fidelity=dinv.optim.L2()
         ... ) # Define the DiffPIR model
         >>> xhat = model(y, physics) # Run the DiffPIR algorithm
         >>> dinv.utils.cal_psnr(xhat, x) > dinv.utils.cal_psnr(y, x) # Should be closer to the original
         True
         
     """
```

### Comparing `deepinv-0.1.1/deepinv/sampling/langevin.py` & `deepinv-0.2.0/deepinv/sampling/langevin.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.save_chain = save_chain
         self.chain = []
 
     def forward(self, y, physics, seed=None, x_init=None):
         r"""
         Runs an Monte Carlo chain to obtain the posterior mean and variance of the reconstruction of the measurements y.
 
-        :param torch.tensor y: Measurements
+        :param torch.Tensor y: Measurements
         :param deepinv.physics.Physics physics: Forward operator associated with the measurements
         :param float seed: Random seed for generating the Monte Carlo samples
         :return: (tuple of torch.tensor) containing the posterior mean and variance.
         """
         with torch.no_grad():
             if seed is not None:
                 np.random.seed(seed)
@@ -218,15 +218,15 @@
         self.alpha = alpha
         self.noise_std = np.sqrt(2 * step_size)
         self.sigma = sigma
 
     def forward(self, x, y, physics, likelihood, prior):
         noise = torch.randn_like(x) * self.noise_std
         lhood = -likelihood.grad(x, y, physics)
-        lprior = -prior(x, self.sigma) * self.alpha
+        lprior = -prior.grad(x, self.sigma) * self.alpha
         return x + self.step_size * (lhood + lprior) + noise
 
 
 class ULA(MonteCarlo):
     r"""
     Projected Plug-and-Play Unadjusted Langevin Algorithm.
 
@@ -311,15 +311,15 @@
         self.alpha = alpha
         self.eta = eta
         self.inner_iter = inner_iter
         self.noise_std = np.sqrt(2 * step_size)
         self.sigma = sigma
 
     def forward(self, x, y, physics, likelihood, prior):
-        posterior = lambda u: likelihood.grad(u, y, physics) + self.alpha * prior(
+        posterior = lambda u: likelihood.grad(u, y, physics) + self.alpha * prior.grad(
             u, self.sigma
         )
 
         # First kind Chebyshev function
         T_s = lambda s, u: np.cosh(s * np.arccosh(u))
         # First derivative Chebyshev polynomial first kind
         T_prime_s = lambda s, u: s * np.sinh(s * np.arccosh(u)) / np.sqrt(u**2 - 1)
```

### Comparing `deepinv-0.1.1/deepinv/sampling/utils.py` & `deepinv-0.2.0/deepinv/sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/tests/conftest.py` & `deepinv-0.2.0/deepinv/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 import deepinv as dinv
 from deepinv.tests.dummy_datasets.datasets import DummyCircles
 
 
 @pytest.fixture
 def device():
-    return dinv.utils.get_freer_gpu() if torch.cuda.is_available() else "cpu"
+    return (
+        dinv.utils.get_freer_gpu() if torch.cuda.is_available() else torch.device("cpu")
+    )
 
 
 @pytest.fixture
 def toymatrix():
     w = 50
     A = torch.diag(torch.Tensor(range(1, w + 1)))
     return A
```

### Comparing `deepinv-0.1.1/deepinv/tests/dummy_datasets/datasets.py` & `deepinv-0.2.0/deepinv/tests/dummy_datasets/datasets.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/tests/test_loss.py` & `deepinv-0.2.0/deepinv/tests/test_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import deepinv
 from deepinv.tests.dummy_datasets.datasets import DummyCircles
 from torch.utils.data import DataLoader
 import deepinv as dinv
 from deepinv.loss.regularisers import JacobianSpectralNorm, FNEJacobianSpectralNorm
 
 LOSSES = ["sup", "mcei", "mcei-scale", "r2r"]
-LIST_SURE = ["Gaussian", "Poisson", "PoissonGaussian", "UniformGaussian"]
+LIST_SURE = ["Gaussian", "Poisson", "PoissonGaussian"]
 
 
 def test_jacobian_spectral_values(toymatrix):
     # Define the Jacobian regularisers we want to check
     reg_l2 = JacobianSpectralNorm(max_iter=100, tol=1e-3, eval_mode=False, verbose=True)
     reg_FNE_l2 = FNEJacobianSpectralNorm(
         max_iter=100, tol=1e-3, eval_mode=False, verbose=True
@@ -62,19 +62,14 @@
     sigma = 0.1
     if noise_type == "PoissonGaussian":
         loss = dinv.loss.SurePGLoss(sigma=sigma, gain=gain)
         noise_model = dinv.physics.PoissonGaussianNoise(sigma=sigma, gain=gain)
     elif noise_type == "Gaussian":
         loss = dinv.loss.SureGaussianLoss(sigma=sigma)
         noise_model = dinv.physics.GaussianNoise(sigma)
-    elif noise_type == "UniformGaussian":
-        loss = dinv.loss.SureGaussianLoss(sigma=sigma)
-        noise_model = dinv.physics.UniformGaussianNoise(
-            sigma=sigma
-        )  # This is equivalent to GaussianNoise when sigma is fixed
     elif noise_type == "Poisson":
         loss = dinv.loss.SurePoissonLoss(gain=gain)
         noise_model = dinv.physics.PoissonNoise(gain)
     elif noise_type == "Neighbor2Neighbor":
         loss = dinv.loss.Neighbor2Neighbor()
         noise_model = dinv.physics.PoissonNoise(gain)
     else:
@@ -239,16 +234,14 @@
 
         error_h += torch.abs(h - exact)
         error_mc += torch.abs(mc - exact)
 
     error_mc /= num_it
     error_h /= num_it
 
-    # print(f"error_h: {error_h}")
-    # print(f"error_mc: {error_mc}")
     assert error_h < 5e-2
     assert error_mc < 5e-2
 
 
 def test_measplit(device):
     sigma = 0.1
     physics = dinv.physics.Denoising()
```

### Comparing `deepinv-0.1.1/deepinv/tests/test_loss_train.py` & `deepinv-0.2.0/deepinv/tests/test_loss_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from torch.utils.data import DataLoader
 
 import deepinv as dinv
 from deepinv.optim.data_fidelity import L2
 from deepinv.optim.prior import PnP
 from deepinv.tests.dummy_datasets.datasets import DummyCircles
 from deepinv.unfolded import unfolded_builder
-from deepinv.training_utils import train
-from deepinv.training_utils import test as feature_test
+from deepinv.training import train
+from deepinv.training import test as feature_test
 
 
 def test_generate_dataset(tmp_path, imsize, device):
     N = 10
     max_N = 10
     train_dataset = DummyCircles(samples=N, imsize=imsize)
     test_dataset = DummyCircles(samples=N, imsize=imsize)
@@ -48,15 +48,15 @@
 # ]
 
 optim_algos = ["PGD"]
 
 
 @pytest.mark.parametrize("name_algo", optim_algos)
 def test_optim_algo(name_algo, imsize, device):
-    # This test uses WaveletPrior, which requires pytorch_wavelets
+    # This test uses WaveletDenoiser, which requires pytorch_wavelets
     # TODO: we could use a dummy trainable denoiser with a linear layer instead
     pytest.importorskip("ptwt")
 
     # pths
     BASE_DIR = Path(".")
     CKPT_DIR = BASE_DIR / "ckpts"
 
@@ -66,15 +66,15 @@
     # Set up the trainable denoising prior; here, the soft-threshold in a wavelet basis.
     # If the prior is initialized with a list of length max_iter,
     # then a distinct weight is trained for each PGD iteration.
     # For fixed trained model prior across iterations, initialize with a single model.
     max_iter = 30 if torch.cuda.is_available() else 3  # Number of unrolled iterations
     level = 3
     prior = [
-        PnP(denoiser=dinv.models.WaveletPrior(wv="db8", level=level, device=device))
+        PnP(denoiser=dinv.models.WaveletDenoiser(wv="db8", level=level, device=device))
         for i in range(max_iter)
     ]
 
     # Unrolled optimization algorithm parameters
     lamb = [
         1.0
     ] * max_iter  # initialization of the regularization parameter. A distinct lamb is trained for each iteration.
@@ -150,34 +150,35 @@
         losses=losses,
         physics=physics,
         optimizer=optimizer,
         device=device,
         save_path=str(CKPT_DIR),
         verbose=True,
         wandb_vis=False,
+        online_measurements=True,
     )
 
     results = feature_test(
         model=trained_unfolded_model,
         test_dataloader=test_dataloader,
         physics=physics,
         device=device,
         plot_images=False,
         verbose=True,
         wandb_vis=False,
     )
 
-    # Now check that training with online measurements works as well
-    train(
-        model=model_unfolded,
-        train_dataloader=train_dataloader,
-        eval_dataloader=test_dataloader,
-        epochs=epochs,
-        losses=losses,
-        physics=physics,
-        optimizer=optimizer,
-        device=device,
-        save_path=str(CKPT_DIR),
-        verbose=True,
-        wandb_vis=False,
-        online_measurements=True,
-    )
+
+def test_epll_parameter_estimation(imsize, dummy_dataset, device):
+    from deepinv.datasets import PatchDataset
+
+    imgs = dummy_dataset.x
+    patch_dataset = PatchDataset(imgs)
+    patch_dataloader = torch.utils.data.DataLoader(
+        patch_dataset, batch_size=2, shuffle=True, drop_last=False
+    )
+    epll = dinv.optim.EPLL(channels=imsize[0], pretrained=None, n_components=3)
+    epll.GMM.fit(patch_dataloader, max_iters=10)
+
+    assert not torch.any(torch.isnan(epll.GMM.mu))
+    assert not torch.any(torch.isnan(epll.GMM.get_cov()))
+    assert not torch.any(torch.isnan(epll.GMM.get_weights()))
```

### Comparing `deepinv-0.1.1/deepinv/tests/test_models.py` & `deepinv-0.2.0/deepinv/tests/test_models.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,31 +7,33 @@
 
 MODEL_LIST_1_CHANNEL = [
     "autoencoder",
     "drunet",
     "dncnn",
     "median",
     "tgv",
-    "waveletprior",
+    "waveletdenoiser",
     "waveletdict",
+    "epll",
+    "restormer",
 ]
 MODEL_LIST = MODEL_LIST_1_CHANNEL + [
     "bm3d",
     "gsdrunet",
     "scunet",
     "swinir",
     "tv",
     "unet",
     "waveletdict_hard",
     "waveletdict_topk",
 ]
 
 
 def choose_denoiser(name, imsize):
-    if name.startswith("waveletdict") or name == "waveletprior":
+    if name.startswith("waveletdict") or name == "waveletdenoiser":
         pytest.importorskip(
             "ptwt",
             reason="This test requires pytorch_wavelets. It should be "
             "installed with `pip install "
             "git+https://github.com/fbcotter/pytorch_wavelets.git`",
         )
     if name == "bm3d":
@@ -55,32 +57,36 @@
         out = dinv.models.SCUNet(in_nc=imsize[0])
     elif name == "gsdrunet":
         out = dinv.models.GSDRUNet(in_channels=imsize[0], out_channels=imsize[0])
     elif name == "bm3d":
         out = dinv.models.BM3D()
     elif name == "dncnn":
         out = dinv.models.DnCNN(in_channels=imsize[0], out_channels=imsize[0])
-    elif name == "waveletprior":
-        out = dinv.models.WaveletPrior()
+    elif name == "waveletdenoiser":
+        out = dinv.models.WaveletDenoiser()
     elif name == "waveletdict":
-        out = dinv.models.WaveletDict()
+        out = dinv.models.WaveletDictDenoiser()
     elif name == "waveletdict_hard":
-        out = dinv.models.WaveletDict(non_linearity="hard")
+        out = dinv.models.WaveletDictDenoiser(non_linearity="hard")
     elif name == "waveletdict_topk":
-        out = dinv.models.WaveletDict(non_linearity="topk")
+        out = dinv.models.WaveletDictDenoiser(non_linearity="topk")
     elif name == "tgv":
         out = dinv.models.TGVDenoiser(n_it_max=10)
     elif name == "tv":
         out = dinv.models.TVDenoiser(n_it_max=10)
     elif name == "median":
         out = dinv.models.MedianFilter()
     elif name == "autoencoder":
         out = dinv.models.AutoEncoder(dim_input=imsize[0] * imsize[1] * imsize[2])
     elif name == "swinir":
         out = dinv.models.SwinIR(in_chans=imsize[0])
+    elif name == "epll":
+        out = dinv.models.EPLLDenoiser(channels=imsize[0])
+    elif name == "restormer":
+        out = dinv.models.Restormer(in_channels=imsize[0], out_channels=imsize[0])
     else:
         raise Exception("Unknown denoiser")
 
     return out
 
 
 def test_TVs_adjoint():
@@ -113,15 +119,14 @@
     Atv = model.epsilon_adjoint(v)
     e = v.flatten() @ Au.flatten() - Atv.flatten() @ u.flatten()
 
     assert torch.allclose(e, torch.tensor([0.0], dtype=torch.float64))
 
 
 def test_wavelet_adjoints():
-
     pytest.importorskip(
         "ptwt",
         reason="This test requires pytorch_wavelets. It should be "
         "installed with `pip install "
         "git+https://github.com/fbcotter/pytorch_wavelets.git`",
     )
 
@@ -141,15 +146,15 @@
             for l in range(1, len(Au)):
                 out = out + [{key: torch.randn_like(Au[l][key]) for key in Au[l]}]
         return out
 
     for dimension in ["2d", "3d"]:
         wvdim = 2 if dimension == "2d" else 3
 
-        model = dinv.models.WaveletPrior(wvdim=wvdim)
+        model = dinv.models.WaveletDenoiser(wvdim=wvdim)
 
         def A_f(x):
             dx = model.dwt(x)
             Ax = model.flatten_coeffs(dx)
             return dx, Ax
 
         def gen_rand(Au):
@@ -178,43 +183,62 @@
     pytest.importorskip(
         "ptwt",
         reason="This test requires pytorch_wavelets. It should be "
         "installed with `pip install "
         "git+https://github.com/fbcotter/pytorch_wavelets.git`",
     )
 
-    # 1. Wavelet Prior & dictionary
+    # 1. Wavelet denoiser (single & dictionary)
     for dimension in ["2d", "3d"]:
         wvdim = 2 if dimension == "2d" else 3
         x = (
             torch.randn((4, 3, 31, 27))
             if dimension == "2d"
             else torch.randn((4, 3, 31, 27, 29))
         )
         for non_linearity in ["soft", "hard"]:
-            model = dinv.models.WaveletPrior(non_linearity=non_linearity, wvdim=wvdim)
+            model = dinv.models.WaveletDenoiser(
+                non_linearity=non_linearity, wvdim=wvdim
+            )
             ths = (
                 0.0 if non_linearity in ["soft", "hard"] else 1.0
             )  # topk counts the number of coefficients to keep
             x_hat = model(x, ths)
             assert x_hat.shape == x.shape
             assert torch.allclose(
                 x, x_hat, atol=1e-5
             )  # The model should be the identity
 
-        model = dinv.models.WaveletDict(
+        model = dinv.models.WaveletDictDenoiser(
             list_wv=["haar", "db3", "db8"], non_linearity="soft", wvdim=wvdim
         )
         x_hat = model(x, 0.0)
         assert x_hat.shape == x.shape
         assert torch.allclose(x, x_hat, atol=1e-5)  # The model should be the identity
 
+    # 2. Wavelet Prior
+    for dimension in ["2d", "3d"]:
+        wvdim = 2 if dimension == "2d" else 3
+        x = (
+            torch.ones((4, 3, 31, 27))
+            if dimension == "2d"
+            else torch.ones((4, 3, 31, 27, 29))
+        )
+        level = 3
+        prior = dinv.optim.prior.WaveletPrior(wvdim=wvdim, p=1, level=level)
+        g_nonflat = prior.g(x, reduce=False)
+        g_flat = prior.g(x, reduce=True)
+        assert g_nonflat.dim() > 0
+        assert len(g_nonflat) == 3 * level if wvdim == 2 else 7 * level
+        assert g_flat.dim() == 0
 
-def test_TV_models_identity():
+        assert torch.allclose(g_nonflat.abs().sum(), g_flat)
 
+
+def test_TV_models_identity():
     # Next priors are checked for 2D only
     x = torch.randn((4, 3, 31, 27))
 
     # 3. TV
     model = dinv.models.TVDenoiser(n_it_max=10)
     x_hat = model(x, 0.0)
     assert x_hat.shape == x.shape
@@ -500,16 +524,16 @@
 
 @pytest.mark.parametrize(
     "denoiser, dep",
     [
         ("BM3D", "bm3d"),
         ("SCUNet", "timm"),
         ("SwinIR", "timm"),
-        ("WaveletPrior", "ptwt"),
-        ("WaveletDict", "ptwt"),
+        ("WaveletDenoiser", "ptwt"),
+        ("WaveletDictDenoiser", "ptwt"),
     ],
 )
 def test_optional_dependencies(denoiser, dep):
     # Skip the test if the optional dependency is installed
     if dep in sys.modules:
         pytest.skip(f"Optional dependency {dep} is installed.")
```

### Comparing `deepinv-0.1.1/deepinv/tests/test_optim.py` & `deepinv-0.2.0/deepinv/tests/test_optim.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import pytest
 
 import torch
 from torch.utils.data import DataLoader
 
 import deepinv as dinv
 from deepinv.optim import DataFidelity
-from deepinv.optim.data_fidelity import L2, IndicatorL2, L1
+from deepinv.optim.data_fidelity import L2, IndicatorL2, L1, AmplitudeLoss
 from deepinv.optim.prior import Prior, PnP, RED
 from deepinv.optim.optimizers import optim_builder
+from deepinv.optim.optim_iterators import GDIteration
 
 
 def custom_init_CP(y, physics):
     x_init = physics.A_adjoint(y)
     u_init = y
     return {"est": (x_init, x_init, u_init)}
 
@@ -167,14 +168,60 @@
 
     # Check prox
     threshold = 0.5
     prox_manual = torch.Tensor([[[1.0], [3.5], [0.0]]]).to(device)
     assert torch.allclose(data_fidelity.prox_d(x, y, threshold), prox_manual)
 
 
+def test_zero_prior():
+    A = torch.eye(3, dtype=torch.float64)
+
+    def A_forward(v):
+        return A @ v
+
+    def A_adjoint(v):
+        return A.T @ v
+
+    physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
+    data_fidelity = dinv.optim.data_fidelity.L2()
+    params_algo = {"stepsize": 0.5, "lambda": 1.0}
+    iterator = GDIteration()
+    optimalgo = dinv.optim.BaseOptim(
+        iterator,
+        data_fidelity=data_fidelity,
+        params_algo=params_algo,
+    )
+    for _ in range(10):
+        x = torch.randn((3,), dtype=torch.float64)
+        xhat = optimalgo(x, physics)
+        assert torch.allclose(xhat, x)
+
+
+def test_data_fidelity_amplitude_loss(device):
+    r"""
+    Tests if the gradient computed with grad_d method of amplitude loss is consistent with the autograd gradient.
+
+    :param device: (torch.device) cpu or cuda:x
+    :return: assertion error if the relative difference between the two gradients is more than 1e-5
+    """
+    # essential to enable autograd
+    with torch.enable_grad():
+        x = torch.randn(
+            (1, 1, 3, 3), dtype=torch.cfloat, device=device, requires_grad=True
+        )
+        physics = dinv.physics.RandomPhaseRetrieval(
+            m=10, img_shape=(1, 3, 3), device=device
+        )
+        loss = AmplitudeLoss()
+        func = lambda x: loss(x, torch.ones_like(physics(x)), physics)[0]
+        grad_value = torch.func.grad(func)(x)
+        jvp_value = loss.grad(x, torch.ones_like(physics(x)), physics)
+    assert torch.isclose(grad_value[0], jvp_value, rtol=1e-5).all()
+
+
 # we do not test CP (Chambolle-Pock) as we have a dedicated test (due to more specific optimality conditions)
 @pytest.mark.parametrize("name_algo", ["PGD", "ADMM", "DRS", "HQS"])
 def test_optim_algo(name_algo, imsize, dummy_dataset, device):
     for g_first in [True, False]:
         # Define two points
         x = torch.tensor([[[10], [10]]], dtype=torch.float64)
 
@@ -185,30 +232,30 @@
 
         # Define the physics model associated to this operator
         physics = dinv.physics.LinearPhysics(A=B_forward, A_adjoint=B_adjoint)
         y = physics(x)
 
         data_fidelity = L2()  # The data fidelity term
 
-        def prior_g(x, *args):
+        def prior_g(x, *args, **kwargs):
             ths = 0.1
             return ths * torch.norm(x.view(x.shape[0], -1), p=1, dim=-1)
 
         prior = Prior(g=prior_g)  # The prior term
 
         if (
             name_algo == "CP"
         ):  # In the case of primal-dual, stepsizes need to be bounded as reg_param*stepsize < 1/physics.compute_norm(x, tol=1e-4).item()
             stepsize = 0.9 / physics.compute_norm(x, tol=1e-4).item()
             sigma = 1.0
         else:  # Note that not all other algos need such constraints on parameters, but we use these to check that the computations are correct
             stepsize = 0.9 / physics.compute_norm(x, tol=1e-4).item()
             sigma = None
 
-        lamb = 1.1
+        lamb = 0.9
         max_iter = 1000
         params_algo = {"stepsize": stepsize, "lambda": lamb, "sigma": sigma}
 
         optimalgo = optim_builder(
             name_algo,
             prior=prior,
             data_fidelity=data_fidelity,
@@ -225,43 +272,43 @@
         x = optimalgo(y, physics)
 
         assert optimalgo.has_converged
 
         # Compute the subdifferential of the regularisation at the limit point of the algorithm.
 
         if name_algo == "HQS":
-            # In this case, the algorithm does not converge to the minimum of :math:`\lambda f+g` but to that of
-            # :math:`\lambda M_{\lambda \tau f}+g` where :math:` M_{\lambda \tau f}` denotes the Moreau envelope of :math:`f` with parameter :math:`\lambda \tau`.
+            # In this case, the algorithm does not converge to the minimum of :math:`f+\lambda g` but to that of
+            # :math:` M_{\tau f}+ \lambda g` where :math:` M_{\tau f}` denotes the Moreau envelope of :math:`f` with parameter :math:`\tau`.
             # Beware, these are not fetch automatically here but handwritten in the test.
-            # The optimality condition is then :math:`0 \in \lambda M_{\lambda \tau f}(x)+\partial g(x)`
+            # The optimality condition is then :math:`0 \in M_{\tau f}(x)+ \lambda \partial g(x)`
             if not g_first:
                 subdiff = prior.grad(x)
                 moreau_grad = (
-                    x - data_fidelity.prox(x, y, physics, gamma=lamb * stepsize)
+                    x - data_fidelity.prox(x, y, physics, gamma=stepsize)
                 ) / (
-                    lamb * stepsize
+                    stepsize
                 )  # Gradient of the moreau envelope
                 assert torch.allclose(
-                    lamb * moreau_grad, -subdiff, atol=1e-8
+                    moreau_grad, -lamb * subdiff, atol=1e-8
                 )  # Optimality condition
             else:
-                subdiff = lamb * data_fidelity.grad(x, y, physics)
-                moreau_grad = (
-                    x - prior.prox(x, gamma=stepsize)
-                ) / stepsize  # Gradient of the moreau envelope
+                subdiff = data_fidelity.grad(x, y, physics)
+                moreau_grad = (x - prior.prox(x, gamma=lamb * stepsize)) / (
+                    lamb * stepsize
+                )  # Gradient of the moreau envelope
                 assert torch.allclose(
-                    moreau_grad, -subdiff, atol=1e-8
+                    lamb * moreau_grad, -subdiff, atol=1e-8
                 )  # Optimality condition
         else:
             subdiff = prior.grad(x)
-            # In this case, the algorithm converges to the minimum of :math:`\lambda f+g`.
-            # The optimality condition is then :math:`0 \in \lambda \nabla f(x)+\partial g(x)`
+            # In this case, the algorithm converges to the minimum of :math:`f+\lambda g`.
+            # The optimality condition is then :math:`0 \in  \nabla f(x)+ \lambda \partial g(x)`
             grad_deepinv = data_fidelity.grad(x, y, physics)
             assert torch.allclose(
-                lamb * grad_deepinv, -subdiff, atol=1e-8
+                grad_deepinv, -lamb * subdiff, atol=1e-8
             )  # Optimality condition
 
 
 def test_denoiser(imsize, dummy_dataset, device):
     dataloader = DataLoader(
         dummy_dataset, batch_size=1, shuffle=False, num_workers=0
     )  # 1. Generate a dummy dataset
@@ -299,27 +346,29 @@
 
     # 1. Generate a dummy dataset
     dataloader = DataLoader(dummy_dataset, batch_size=1, shuffle=False, num_workers=0)
     test_sample = next(iter(dataloader)).to(device)
 
     # 2. Set a physical experiment (here, deblurring)
     physics = dinv.physics.Blur(
-        dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0), device=device
+        dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0),
+        device=device,
+        padding="circular",
     )
     y = physics(test_sample)
     max_iter = 1000
     # Note: results are better for sigma_denoiser=0.001, but it takes longer to run.
     sigma_denoiser = torch.tensor([[0.1]])
     stepsize = 1.0
     lamb = 1.0
 
     data_fidelity = L2()
 
     # here the prior model is common for all iterations
-    prior = PnP(denoiser=dinv.models.WaveletPrior(wv="db8", level=3, device=device))
+    prior = PnP(denoiser=dinv.models.WaveletDenoiser(wv="db8", level=3, device=device))
 
     stepsize_dual = 1.0 if pnp_algo == "CP" else None
     params_algo = {
         "stepsize": stepsize,
         "g_param": sigma_denoiser,
         "lambda": lamb,
         "stepsize_dual": stepsize_dual,
@@ -366,15 +415,17 @@
         dataloader = DataLoader(
             dummy_dataset, batch_size=1, shuffle=False, num_workers=0
         )
         test_sample = next(iter(dataloader)).to(device)
 
         # 2. Set a physical experiment (here, deblurring)
         physics = dinv.physics.Blur(
-            dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0), device=device
+            dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0),
+            padding="circular",
+            device=device,
         )
         y = physics(test_sample)
         max_iter = 1000
         # Note: results are better for sigma_denoiser=0.001, but it takes longer to run.
         # sigma_denoiser = torch.tensor([[0.1]])
         sigma_denoiser = torch.tensor([[1.0]], device=device)
         stepsize = 1.0
@@ -429,35 +480,36 @@
         #     )
 
         assert opt_algo.has_converged
 
 
 @pytest.mark.parametrize("red_algo", ["GD", "PGD"])
 def test_red_algo(red_algo, imsize, dummy_dataset, device):
-    # This test uses WaveletPrior, which requires pytorch_wavelets
+    # This test uses WaveletDenoiser, which requires pytorch_wavelets
     # TODO: we could use a dummy trainable denoiser with a linear layer instead
     pytest.importorskip("ptwt")
 
     # 1. Generate a dummy dataset
     dataloader = DataLoader(dummy_dataset, batch_size=1, shuffle=False, num_workers=0)
     test_sample = next(iter(dataloader)).to(device)
 
     # 2. Set a physical experiment (here, deblurring)
     physics = dinv.physics.Blur(
-        dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0), device=device
+        dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0),
+        device=device,
     )
     y = physics(test_sample)
     max_iter = 1000
     sigma_denoiser = 1.0  # Note: results are better for sigma_denoiser=0.001, but it takes longer to run.
     stepsize = 1.0
     lamb = 1.0
 
     data_fidelity = L2()
 
-    prior = RED(denoiser=dinv.models.WaveletPrior(wv="db8", level=3, device=device))
+    prior = RED(denoiser=dinv.models.WaveletDenoiser(wv="db8", level=3, device=device))
 
     params_algo = {"stepsize": stepsize, "g_param": sigma_denoiser, "lambda": lamb}
 
     red = optim_builder(
         red_algo,
         prior=prior,
         data_fidelity=data_fidelity,
@@ -470,21 +522,43 @@
     )
 
     red(y, physics)
 
     assert red.has_converged
 
 
+def test_dpir(imsize, dummy_dataset, device):
+    # 1. Generate a dummy dataset
+    dataloader = DataLoader(dummy_dataset, batch_size=1, shuffle=False, num_workers=0)
+    test_sample = next(iter(dataloader)).to(device)
+
+    # 2. Set a physical experiment (here, deblurring)
+    physics = dinv.physics.Blur(
+        dinv.physics.blur.gaussian_blur(sigma=(2, 0.1), angle=45.0),
+        device=device,
+        noise_model=dinv.physics.GaussianNoise(0.1),
+        padding="circular",
+    )
+    y = physics(test_sample)
+    model = dinv.optim.DPIR(0.1, device=device)
+    out = model(y, physics)
+
+    in_psnr = dinv.utils.cal_psnr(test_sample, y)
+    out_psnr = dinv.utils.cal_psnr(out, test_sample)
+
+    assert out_psnr > in_psnr
+
+
 def test_CP_K(imsize, dummy_dataset, device):
     r"""
     This test checks that the CP algorithm converges to the solution of the following problem:
 
     .. math::
 
-        \min_x \lambda a(x) + b(Kx)
+        \min_x  a(x) + \lambda b(Kx)
 
 
     where :math:`a` and :math:`b` are functions and :math:`K` is a linear operator. In this setting, we test both for
     :math:`a(x) = d(Ax-y)` and :math:`b(z) = g(z)`, and for :math:`a(x) = g(x)` and :math:`b(z) = f(z-y)`.
     """
 
     for g_first in [True, False]:
@@ -497,31 +571,30 @@
 
         # Define the physics model associated to this operator
         physics = dinv.physics.LinearPhysics(A=Id_forward, A_adjoint=Id_adjoint)
         y = physics(x)
 
         data_fidelity = L2()  # The data fidelity term
 
-        def prior_g(x, *args):
+        def prior_g(x, *args, **kwargs):
             ths = 1.0
             return ths * torch.norm(x.view(x.shape[0], -1), p=1, dim=-1)
 
         prior = Prior(g=prior_g)  # The prior term
 
         # Define a linear operator
         K = torch.tensor([[2, 1], [-1, 0.5]], dtype=torch.float64).to(device)
         K_forward = lambda v: K @ v
         K_adjoint = lambda v: K.transpose(0, 1) @ v
 
-        # stepsize = 0.9 / physics.compute_norm(x, tol=1e-4).item()
         stepsize = 0.9 / torch.linalg.norm(K, ord=2).item() ** 2
         reg_param = 1.0
         stepsize_dual = 1.0
 
-        lamb = 1.5
+        lamb = 0.6
         max_iter = 1000
 
         params_algo = {
             "stepsize": stepsize,
             "g_param": reg_param,
             "lambda": lamb,
             "stepsize_dual": stepsize_dual,
@@ -547,39 +620,37 @@
         x = optimalgo(y, physics)
 
         print("g_first: ", g_first)
         assert optimalgo.has_converged
 
         # Compute the subdifferential of the regularisation at the limit point of the algorithm.
         if not g_first:
-            subdiff = prior.grad(x, 0)
-
+            subdiff = prior.grad(x)
             grad_deepinv = K_adjoint(
                 data_fidelity.grad(K_forward(x), y, physics)
             )  # This test is only valid for differentiable data fidelity terms.
             assert torch.allclose(
-                lamb * grad_deepinv, -subdiff, atol=1e-12
+                grad_deepinv, -lamb * subdiff, atol=1e-12
             )  # Optimality condition
 
         else:
-            subdiff = K_adjoint(prior.grad(K_forward(x), 0))
-
+            subdiff = K_adjoint(prior.grad(K_forward(x)))
             grad_deepinv = data_fidelity.grad(x, y, physics)
             assert torch.allclose(
-                lamb * grad_deepinv, -subdiff, atol=1e-12
+                grad_deepinv, -lamb * subdiff, atol=1e-12
             )  # Optimality condition
 
 
 def test_CP_datafidsplit(imsize, dummy_dataset, device):
     r"""
     This test checks that the CP algorithm converges to the solution of the following problem:
 
     .. math::
 
-        \min_x \lambda d(Ax,y) + g(x)
+        \min_x d(Ax,y) + \lambda g(x)
 
 
     where :math:`d` is a distance function and :math:`g` is a prior term.
     """
 
     g_first = False
     # Define two points
@@ -592,26 +663,26 @@
 
     # Define the physics model associated to this operator
     physics = dinv.physics.LinearPhysics(A=A_forward, A_adjoint=A_adjoint)
     y = physics(x)
 
     data_fidelity = L2()  # The data fidelity term
 
-    def prior_g(x, *args):
+    def prior_g(x, *args, **kwargs):
         ths = 1.0
         return ths * torch.norm(x.view(x.shape[0], -1), p=1, dim=-1)
 
     prior = Prior(g=prior_g)  # The prior term
 
     # stepsize = 0.9 / physics.compute_norm(x, tol=1e-4).item()
     stepsize = 0.9 / torch.linalg.norm(A, ord=2).item() ** 2
     reg_param = 1.0
     stepsize_dual = 1.0
 
-    lamb = 1.5
+    lamb = 0.6
     max_iter = 1000
 
     params_algo = {
         "stepsize": stepsize,
         "g_param": reg_param,
         "lambda": lamb,
         "stepsize_dual": stepsize_dual,
@@ -635,15 +706,56 @@
 
     # Run the optimization algorithm
     x = optimalgo(y, physics)
 
     assert optimalgo.has_converged
 
     # Compute the subdifferential of the regularisation at the limit point of the algorithm.
-    subdiff = prior.grad(x, 0)
+    subdiff = prior.grad(x)
 
     grad_deepinv = A_adjoint(
         data_fidelity.grad_d(A_forward(x), y)
     )  # This test is only valid for differentiable data fidelity terms.
     assert torch.allclose(
-        lamb * grad_deepinv, -subdiff, atol=1e-12
+        grad_deepinv, -lamb * subdiff, atol=1e-12
     )  # Optimality condition
+
+
+def test_patch_prior(imsize, dummy_dataset, device):
+    pytest.importorskip(
+        "FrEIA",
+        reason="This test requires FrEIA. It should be "
+        "installed with `pip install FrEIA",
+    )
+    torch.manual_seed(0)
+
+    dataloader = DataLoader(
+        dummy_dataset, batch_size=1, shuffle=False, num_workers=0
+    )  # 1. Generate a dummy dataset
+    # gray-valued
+    test_sample = next(iter(dataloader)).mean(1, keepdim=True).to(device)
+
+    with torch.enable_grad():
+        physics = dinv.physics.Denoising(
+            noise_model=dinv.physics.GaussianNoise(0.1)
+        )  # 2. Set a physical experiment (here, denoising)
+        y = physics(test_sample).type(test_sample.dtype).to(device)
+
+        epll = dinv.optim.EPLL(channels=test_sample.shape[1], device=device)
+        patchnr = dinv.optim.PatchNR(channels=test_sample.shape[1], device=device)
+        prior1 = dinv.optim.PatchPrior(epll.negative_log_likelihood)
+        prior2 = dinv.optim.PatchPrior(patchnr)
+        data_fidelity = L2()
+
+        lam = 1.0
+        x_out = []
+        for prior in [prior1, prior2]:
+            x = y.detach().clone().requires_grad_(True)
+            optimizer = torch.optim.Adam([x], lr=0.01)
+            for i in range(10):
+                optimizer.zero_grad()
+                loss = data_fidelity(x, y, physics) + prior(x, lam)
+                loss.backward()
+                optimizer.step()
+            x_out.append(x.detach())
+
+    assert torch.sum((x_out[0] - test_sample) ** 2) < torch.sum((y - test_sample) ** 2)
```

### Comparing `deepinv-0.1.1/deepinv/tests/test_sampling.py` & `deepinv-0.2.0/deepinv/tests/test_sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 
 class GaussianScore(torch.nn.Module):
     def __init__(self, sigma_prior):
         super().__init__()
         self.sigma_prior2 = sigma_prior**2
 
-    def forward(self, x, sigma):
+    def grad(self, x, sigma):
         return x / self.sigma_prior2
 
 
 class GaussianDenoiser(torch.nn.Module):
     def __init__(self, sigma_prior):
         super().__init__()
         self.sigma_prior2 = sigma_prior**2
```

### Comparing `deepinv-0.1.1/deepinv/tests/test_unfolded.py` & `deepinv-0.2.0/deepinv/tests/test_unfolded.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     # Set up the trainable denoising prior; here, the soft-threshold in a wavelet basis.
     # If the prior is initialized with a list of length max_iter,
     # then a distinct weight is trained for each PGD iteration.
     # For fixed trained model prior across iterations, initialize with a single model.
     max_iter = 30 if torch.cuda.is_available() else 20  # Number of unrolled iterations
     level = 3
     prior = [
-        PnP(denoiser=dinv.models.WaveletPrior(wv="db8", level=level, device=device))
+        PnP(denoiser=dinv.models.WaveletDenoiser(wv="db8", level=level, device=device))
         for i in range(max_iter)
     ]
 
     # Unrolled optimization algorithm parameters
     lamb = [
         1.0
     ] * max_iter  # initialization of the regularization parameter. A distinct lamb is trained for each iteration.
@@ -78,15 +78,15 @@
     # Set up the trainable denoising prior; here, the soft-threshold in a wavelet basis.
     # If the prior is initialized with a list of length max_iter,
     # then a distinct weight is trained for each PGD iteration.
     # For fixed trained model prior across iterations, initialize with a single model.
     max_iter = 30 if torch.cuda.is_available() else 20  # Number of unrolled iterations
     level = 3
     prior = [
-        PnP(denoiser=dinv.models.WaveletPrior(wv="db8", level=level, device=device))
+        PnP(denoiser=dinv.models.WaveletDenoiser(wv="db8", level=level, device=device))
         for i in range(max_iter)
     ]
 
     # Unrolled optimization algorithm parameters
     lamb = [
         1.0
     ] * max_iter  # initialization of the regularization parameter. A distinct lamb is trained for each iteration.
```

### Comparing `deepinv-0.1.1/deepinv/transform/rotate.py` & `deepinv-0.2.0/deepinv/transform/rotate.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/transform/scale.py` & `deepinv-0.2.0/deepinv/transform/scale.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/transform/shift.py` & `deepinv-0.2.0/deepinv/transform/shift.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/unfolded/deep_equilibrium.py` & `deepinv-0.2.0/deepinv/unfolded/deep_equilibrium.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
     F_fn=None,
     g_first=False,
     **kwargs,
 ):
     r"""
     Helper function for building an instance of the :meth:`BaseDEQ` class.
 
-    :param str, deepinv.optim.optim_iterators.OptimIterator iteration: either the name of the algorithm to be used,
+    :param str, deepinv.optim.OptimIterator iteration: either the name of the algorithm to be used,
         or directly an optim iterator.
         If an algorithm name (string), should be either ``"PGD"`` (proximal gradient descent), ``"ADMM"`` (ADMM),
         ``"HQS"`` (half-quadratic splitting), ``"CP"`` (Chambolle-Pock) or ``"DRS"`` (Douglas Rachford).
     :param dict params_algo: dictionary containing all the relevant parameters for running the algorithm,
                             e.g. the stepsize, regularisation parameter, denoising standard deviation.
                             Each value of the dictionary can be either Iterable (distinct value for each iteration) or
                             a single float (same value for each iteration).
```

### Comparing `deepinv-0.1.1/deepinv/unfolded/unfolded.py` & `deepinv-0.2.0/deepinv/unfolded/unfolded.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,87 +1,162 @@
 import torch
 import torch.nn as nn
-from deepinv.optim.optim_iterators import *
 from deepinv.optim.optimizers import BaseOptim, create_iterator
 
 
 class BaseUnfold(BaseOptim):
     r"""
     Base class for unfolded algorithms. Child of :class:`deepinv.optim.BaseOptim`.
 
     Enables to turn any iterative optimization algorithm into an unfolded algorithm, i.e. an algorithm
     that can be trained end-to-end, with learnable parameters. Recall that the algorithms have the
-    following form (see :meth:`deepinv.optim.optim_iterators.BaseIterator`):
+    following form (see :meth:`deepinv.optim.OptimIterator`):
 
     .. math::
         \begin{aligned}
-        z_{k+1} &= \operatorname{step}_f(x_k, z_k, y, A, \lambda, \gamma, ...)\\
-        x_{k+1} &= \operatorname{step}_g(x_k, z_k, y, A, \sigma, ...)
+        z_{k+1} &= \operatorname{step}_f(x_k, z_k, y, A, \gamma, ...)\\
+        x_{k+1} &= \operatorname{step}_g(x_k, z_k, y, A, \lambda, \sigma, ...)
         \end{aligned}
 
-    where :math:`\operatorname{step}_f` and :math:`\operatorname{step}_g` are learnable modules. 
+    where :math:`\operatorname{step}_f` and :math:`\operatorname{step}_g` are learnable modules.
     These modules encompass trainable parameters of the algorithm (e.g. stepsize :math:`\gamma`, regularization parameter :math:`\lambda`, prior parameter (`g_param`) :math:`\sigma` ...)
     as well as trainable priors (e.g. a deep denoiser).
 
-    :param list trainable_params: List of parameters to be trained. Each parameter should be a key of the ``params_algo`` dictionary for the :class:`deepinv.optim.optim_iterators.BaseIterator` class.
-                    This does not encompass the trainable weights of the prior module . 
-    :param torch.device device: Device on which to perform the computations. Default: `torch.device("cpu")`.
-    :param args:  Non-keyword arguments to be passed to the :class:`deepinv.optim.BaseOptim` class.
+    :param str, deepinv.optim.OptimIterator iteration: either the name of the algorithm to be used,
+        or directly an optim iterator.
+        If an algorithm name (string), should be either ``"GD"`` (gradient descent), ``"PGD"`` (proximal gradient descent),
+        ``"ADMM"`` (ADMM),
+        ``"HQS"`` (half-quadratic splitting), ``"CP"`` (Chambolle-Pock) or ``"DRS"`` (Douglas Rachford). See
+        <optim> for more details.
+    :param dict params_algo: dictionary containing all the relevant parameters for running the algorithm,
+        e.g. the stepsize, regularisation parameter, denoising standard deviation.
+        Each value of the dictionary can be either Iterable (distinct value for each iteration) or
+        a single float (same value for each iteration).
+        Default: ``{"stepsize": 1.0, "lambda": 1.0}``. See :any:`optim-params` for more details.
+    :param list, deepinv.optim.DataFidelity: data-fidelity term.
+        Either a single instance (same data-fidelity for each iteration) or a list of instances of
+        :meth:`deepinv.optim.DataFidelity` (distinct data-fidelity for each iteration). Default: ``None``.
+    :param list, deepinv.optim.Prior prior: regularization prior.
+        Either a single instance (same prior for each iteration) or a list of instances of
+        deepinv.optim.Prior (distinct prior for each iteration). Default: ``None``.
+    :param int max_iter: number of iterations of the unfolded algorithm. Default: 5.
+    :param list trainable_params: List of parameters to be trained. Each parameter should be a key of the ``params_algo``
+        dictionary for the :meth:`deepinv.optim.OptimIterator` class.
+        This does not encompass the trainable weights of the prior module.
+    :param torch.device device: Device on which to perform the computations. Default: ``torch.device("cpu")``.
+    :param bool g_first: whether to perform the step on :math:`g` before that on :math:`f` before or not. default: False
     :param kwargs: Keyword arguments to be passed to the :class:`deepinv.optim.BaseOptim` class.
     """
 
-    def __init__(self, *args, trainable_params=[], device="cpu", **kwargs):
-        super().__init__(*args, **kwargs)
+    def __init__(
+        self,
+        iterator,
+        params_algo={"lambda": 1.0, "stepsize": 1.0},
+        data_fidelity=None,
+        prior=None,
+        max_iter=5,
+        trainable_params=["lambda", "stepsize"],
+        device=torch.device("cpu"),
+        *args,
+        **kwargs,
+    ):
+        super().__init__(
+            iterator,
+            max_iter=max_iter,
+            data_fidelity=data_fidelity,
+            prior=prior,
+            params_algo=params_algo,
+            **kwargs,
+        )
         # Each parameter in `init_params_algo` is a list, which is converted to a `nn.ParameterList` if they should be trained.
         for param_key in trainable_params:
             if param_key in self.init_params_algo.keys():
                 param_value = self.init_params_algo[param_key]
                 self.init_params_algo[param_key] = nn.ParameterList(
                     [nn.Parameter(torch.tensor(el).to(device)) for el in param_value]
                 )
         self.init_params_algo = nn.ParameterDict(self.init_params_algo)
         self.params_algo = self.init_params_algo.copy()
-        # The prior (list of instances of :class:`deepinv.optim.Prior) is converted to a `nn.ModuleList` to be trainable.
+        # The prior (list of instances of :class:`deepinv.optim.Prior`) is converted to a `nn.ModuleList` to be trainable.
         self.prior = nn.ModuleList(self.prior)
         self.data_fidelity = nn.ModuleList(self.data_fidelity)
 
 
 def unfolded_builder(
     iteration,
     params_algo={"lambda": 1.0, "stepsize": 1.0},
     data_fidelity=None,
     prior=None,
+    max_iter=5,
+    trainable_params=["lambda", "stepsize"],
+    device=torch.device("cpu"),
     F_fn=None,
     g_first=False,
     **kwargs,
 ):
     r"""
-    Helper function for building an instance of the :meth:`BaseUnfold` class.
+    Helper function for building an unfolded architecture.
 
-    :param str, deepinv.optim.optim_iterators.OptimIterator iteration: either the name of the algorithm to be used,
+    :param str, deepinv.optim.OptimIterator iteration: either the name of the algorithm to be used,
         or directly an optim iterator.
-        If an algorithm name (string), should be either ``"PGD"`` (proximal gradient descent), ``"ADMM"`` (ADMM),
-        ``"HQS"`` (half-quadratic splitting), ``"CP"`` (Chambolle-Pock) or ``"DRS"`` (Douglas Rachford).
+        If an algorithm name (string), should be either ``"GD"`` (gradient descent), ``"PGD"`` (proximal gradient descent),
+        ``"ADMM"`` (ADMM),
+        ``"HQS"`` (half-quadratic splitting), ``"CP"`` (Chambolle-Pock) or ``"DRS"`` (Douglas Rachford). See
+        <optim> for more details.
     :param dict params_algo: dictionary containing all the relevant parameters for running the algorithm,
-                            e.g. the stepsize, regularisation parameter, denoising standard deviation.
-                            Each value of the dictionary can be either Iterable (distinct value for each iteration) or
-                            a single float (same value for each iteration).
-                            Default: ``{"stepsize": 1.0, "lambda": 1.0}``. See :any:`optim-params` for more details.
+        e.g. the stepsize, regularisation parameter, denoising standard deviation.
+        Each value of the dictionary can be either Iterable (distinct value for each iteration) or
+        a single float (same value for each iteration).
+        Default: ``{"stepsize": 1.0, "lambda": 1.0}``. See :any:`optim-params` for more details.
     :param list, deepinv.optim.DataFidelity: data-fidelity term.
-                            Either a single instance (same data-fidelity for each iteration) or a list of instances of
-                            :meth:`deepinv.optim.DataFidelity` (distinct data-fidelity for each iteration). Default: `None`.
+        Either a single instance (same data-fidelity for each iteration) or a list of instances of
+        :meth:`deepinv.optim.DataFidelity` (distinct data-fidelity for each iteration). Default: ``None``.
     :param list, deepinv.optim.Prior prior: regularization prior.
-                            Either a single instance (same prior for each iteration) or a list of instances of
-                            deepinv.optim.Prior (distinct prior for each iteration). Default: `None`.
+        Either a single instance (same prior for each iteration) or a list of instances of
+        deepinv.optim.Prior (distinct prior for each iteration). Default: ``None``.
+    :param int max_iter: number of iterations of the unfolded algorithm. Default: 5.
+    :param list trainable_params: List of parameters to be trained. Each parameter should be a key of the ``params_algo``
+        dictionary for the :class:`deepinv.optim.OptimIterator` class.
+        This does not encompass the trainable weights of the prior module.
     :param callable F_fn: Custom user input cost function. default: None.
+    :param torch.device device: Device on which to perform the computations. Default: ``torch.device("cpu")``.
     :param bool g_first: whether to perform the step on :math:`g` before that on :math:`f` before or not. default: False
-    :param kwargs: additional arguments to be passed to the :meth:`BaseUnfold` class.
+    :param kwargs: additional arguments to be passed to the :meth:`BaseOptim` class.
+    :return: an unfolded architecture (instance of :meth:`BaseUnfold`).
+
+    |sep|
+
+    :Example:
+
+    .. doctest::
+
+        >>> import torch
+        >>> import deepinv as dinv
+        >>>
+        >>> # Create a trainable unfolded architecture
+        >>> model = dinv.unfolded.unfolded_builder(
+        ...     iteration="PGD",
+        ...     data_fidelity=dinv.optim.L2(),
+        ...     prior=dinv.optim.PnP(dinv.models.DnCNN(in_channels=1, out_channels=1, train=True)),
+        ...     params_algo={"stepsize": 1.0, "g_param": 1.0},
+        ...     trainable_params=["stepsize", "g_param"]
+        ... )
+        >>> # Forward pass
+        >>> x = torch.randn(1, 1, 16, 16)
+        >>> physics = dinv.physics.Denoising()
+        >>> y = physics(x)
+        >>> x_hat = model(y, physics)
+
+
     """
     iterator = create_iterator(iteration, prior=prior, F_fn=F_fn, g_first=g_first)
     return BaseUnfold(
         iterator,
+        max_iter=max_iter,
+        trainable_params=trainable_params,
         has_cost=iterator.has_cost,
         data_fidelity=data_fidelity,
         prior=prior,
         params_algo=params_algo,
+        device=device,
         **kwargs,
     )
```

### Comparing `deepinv-0.1.1/deepinv/utils/__init__.py` & `deepinv-0.2.0/deepinv/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from .logger import AverageMeter, ProgressMeter, get_timestamp
-from .nn import save_model, load_checkpoint, investigate_model
+from .nn import load_checkpoint, investigate_model
 from .metric import cal_psnr, cal_mse, cal_psnr_complex
 from .plotting import (
     rescale_img,
     plot,
     torch2cpu,
     plot_curves,
     plot_parameters,
+    plot_inset,
     make_grid,
     wandb_imgs,
     wandb_plot_curves,
     resize_pad_square_tensor,
 )
 from .demo import load_url_image
 from .nn import get_freer_gpu, TensorList, rand_like, zeros_like, randn_like, ones_like
 from .phantoms import RandomPhantomDataset, SheppLoganDataset
+from .patch_extractor import patch_extractor
```

### Comparing `deepinv-0.1.1/deepinv/utils/demo.py` & `deepinv-0.2.0/deepinv/utils/demo.py`

 * *Files 12% similar despite different names*

```diff
@@ -133,18 +133,22 @@
         print(f"{name} degradation downloaded in {data_dir}")
     deg = np.load(path, allow_pickle=True)
     deg_torch = torch.from_numpy(deg[index])  # .unsqueeze(0).unsqueeze(0)
     return deg_torch
 
 
 def load_url_image(
-    url=None, img_size=None, grayscale=False, resize_mode="crop", device="cpu"
+    url=None,
+    img_size=None,
+    grayscale=False,
+    resize_mode="crop",
+    device="cpu",
+    dtype=torch.float32,
 ):
     r"""
-
     Load an image from a URL and return a torch.Tensor.
 
     :param str url: URL of the image file.
     :param int, tuple[int] img_size: Size of the image to return.
     :param bool grayscale: Whether to convert the image to grayscale.
     :param str resize_mode: If ``img_size`` is not None, options are ``"crop"`` or ``"resize"``.
     :param str device: Device on which to load the image (gpu or cpu).
@@ -163,9 +167,35 @@
             raise ValueError(
                 f"resize_mode must be either 'crop' or 'resize', got {resize_mode}"
             )
     if grayscale:
         transform_list.append(transforms.Grayscale())
     transform_list.append(transforms.ToTensor())
     transform = transforms.Compose(transform_list)
-    x = transform(img).unsqueeze(0).to(device)
+    x = transform(img).unsqueeze(0).to(device=device, dtype=dtype)
     return x
+
+
+def load_torch_url(url):
+    r"""
+    Load an array from url and read it by torch.load.
+
+    :param str url: URL of the image file.
+    :return: whatever is pickled in the file.
+    """
+    response = requests.get(url)
+    response.raise_for_status()
+    out = torch.load(BytesIO(response.content))
+    return out
+
+
+def load_np_url(url=None):
+    r"""
+    Load a numpy array from url.
+
+    :param str url: URL of the image file.
+    :return: :class:`np.array` containing the data.
+    """
+    response = requests.get(url)
+    response.raise_for_status()
+    array = np.load(BytesIO(response.content))
+    return array
```

### Comparing `deepinv-0.1.1/deepinv/utils/logger.py` & `deepinv-0.2.0/deepinv/utils/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import os
 import csv
 from datetime import datetime
+import numpy as np
 
 
 # utils
 class AverageMeter(object):
     """Computes and stores the average and current value"""
 
     def __init__(self, name, fmt=":f"):
         self.name = name
         self.fmt = fmt
         self.reset()
 
     def reset(self):
-        self.val = 0
-        self.avg = 0
-        self.sum = 0
-        self.count = 0
+        self.val = 0.0
+        self.avg = 0.0
+        self.sum = 0.0
+        self.count = 0.0
+        self.std = 0.0
+        self.sum2 = 0.0
 
     def update(self, val, n=1):
-        self.val = val
-        self.sum += val * n
-        self.count += n
+        if isinstance(val, np.ndarray):
+            self.val = np.mean(val)
+            self.sum += np.sum(val) * n
+            self.sum2 += np.sum(val**2) * n
+            self.count += n * np.prod(val.shape)
+        else:
+            self.val = val
+            self.sum += val * n
+            self.sum2 += val**2 * n
+            self.count += n
+
         self.avg = self.sum / self.count
+        var = self.sum2 / self.count - self.avg**2
+        self.std = np.sqrt(var) if var > 0 else 0
 
     def __str__(self):
         fmtstr = "{name}={avg" + self.fmt + "}"
         return fmtstr.format(**self.__dict__)
 
 
 class ProgressMeter(object):
```

### Comparing `deepinv-0.1.1/deepinv/utils/metric.py` & `deepinv-0.2.0/deepinv/utils/metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,60 +1,75 @@
 import torch
+import numpy as np
 
 
 def norm(a):
-    return a.pow(2).sum(dim=3).sum(dim=2).sqrt().unsqueeze(2).unsqueeze(3)
+    return a.pow(2).sum(dim=(-1, -2), keepdim=True).sqrt()
 
 
 def cal_angle(a, b):
-    norm_a = (a * a).flatten().sum().sqrt()
-    norm_b = (b * b).flatten().sum().sqrt()
+    norm_a = norm(a)
+    norm_b = norm(b)
     angle = (a * b).flatten().sum() / (norm_a * norm_b)
-    angle = angle.acos() / 3.14159265359
+    angle = angle.acos() / np.pi
+
     return angle.detach().cpu().numpy()
 
 
-def cal_psnr(a, b, max_pixel=1, normalize=False):
+def cal_psnr(
+    a: torch.Tensor,
+    b: torch.Tensor,
+    max_pixel: float = 1.0,
+    normalize: bool = False,
+    mean_batch: bool = True,
+    to_numpy: bool = True,
+):
     r"""
     Computes the peak signal-to-noise ratio (PSNR)
 
     If the tensors have size (N, C, H, W), then the PSNR is computed as
 
     .. math::
-        \text{PSNR} = \frac{20}{N} \log_{10} \frac{MAX_I}{\sqrt{\|a- b\|^2_2 / (CHW) }}
+        \text{PSNR} = \frac{20}{N} \log_{10} \frac{\text{MAX}_I}{\sqrt{\|a- b\|^2_2 / (CHW) }}
 
-    where :math:`MAX_I` is the maximum possible pixel value of the image (e.g. 1.0 for a
+    where :math:`\text{MAX}_I` is the maximum possible pixel value of the image (e.g. 1.0 for a
     normalized image), and :math:`a` and :math:`b` are the estimate and reference images.
 
     :param torch.Tensor a: tensor estimate
     :param torch.Tensor b: tensor reference
     :param float max_pixel: maximum pixel value
     :param bool normalize: if ``True``, a is normalized to have the same norm as b.
+    :param bool mean_batch: if ``True``, the PSNR is averaged over the batch dimension.
+    :param bool to_numpy: if ``True``, the output is converted to a numpy array.
     """
     with torch.no_grad():
         if type(a) is list or type(a) is tuple:
             a = a[0]
             b = b[0]
 
         if normalize:
             an = a / norm(a) * norm(b)
         else:
             an = a
 
-        mse = (an - b).pow(2).reshape(an.shape[0], -1).mean(dim=1)
-        mse[mse == 0] = 1e-10
-        psnr = 20 * torch.log10(max_pixel / mse.sqrt())
+        mse = (an - b).pow(2).mean(dim=tuple(range(1, an.ndim)), keepdim=False)
+        psnr = -10.0 * torch.log10(mse / max_pixel**2 + 1e-8)
+
+    if mean_batch:
+        psnr = psnr.mean()
 
-    return psnr.mean().detach().cpu().item()
+    if to_numpy:
+        return psnr.detach().cpu().numpy()
+    else:
+        return psnr
 
 
 def cal_mse(a, b):
     """Computes the mean squared error (MSE)"""
-    with torch.no_grad():
-        mse = torch.mean((a - b) ** 2)
+    mse = torch.mean((a - b) ** 2)
     return mse
 
 
 def cal_psnr_complex(a, b):
     """
     first permute the dimension, such that the last dimension of the tensor is 2 (real, imag)
     :param a: shape [N,2,H,W]
```

### Comparing `deepinv-0.1.1/deepinv/utils/nn.py` & `deepinv-0.2.0/deepinv/utils/nn.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,17 @@
         elif isinstance(x, torch.Tensor):
             self.x = [x]
         else:
             raise TypeError("x must be a list of torch.Tensor or a single torch.Tensor")
 
         self.shape = [xi.shape for xi in self.x]
 
+    def __repr__(self):
+        return f"TensorList({self.x})"
+
     def __len__(self):
         r"""
         Returns the number of tensors in the list.
         """
         return len(self.x)
 
     def __getitem__(self, item):
@@ -78,14 +81,25 @@
 
         """
         if not isinstance(other, list) and not isinstance(other, TensorList):
             return TensorList([xi * other for xi in self.x])
         else:
             return TensorList([xi * otheri for xi, otheri in zip(self.x, other)])
 
+    def __rmul__(self, other):
+        r"""
+
+        Multiply two TensorLists. The sizes of the tensor lists must match.
+
+        """
+        if not isinstance(other, list) and not isinstance(other, TensorList):
+            return TensorList([xi * other for xi in self.x])
+        else:
+            return TensorList([xi * otheri for xi, otheri in zip(self.x, other)])
+
     def __truediv__(self, other):
         r"""
 
         Divide two TensorLists. The sizes of the tensor lists must match.
 
         """
         if not isinstance(other, list) and not isinstance(other, TensorList):
@@ -107,14 +121,72 @@
 
         """
         if not isinstance(other, list) and not isinstance(other, TensorList):
             return TensorList([xi - other for xi in self.x])
         else:
             return TensorList([xi - otheri for xi, otheri in zip(self.x, other)])
 
+    def conj(self):
+        r"""
+
+        Computes the conjugate of the elements of the TensorList.
+
+        """
+        return TensorList([xi.conj() for xi in self.x])
+
+    def sum(self, dim, keepdim=False):
+        r"""
+
+        Computes the sum of each elements of the TensorList along the given dimension(s).
+
+        """
+        return TensorList([xi.sum(dim, keepdim) for xi in self.x])
+
+    def reshape(self, shape):
+        r"""
+
+        Reshape each tensor of the TensorList into the given list of shapes.
+
+        """
+        return TensorList([self.x[i].reshape(shape[i]) for i in range(len(self.x))])
+
+    def __any__(self):
+        r"""
+
+        Returns True if any of the elements of the TensorList is True.
+
+        """
+        return any([xi.any() for xi in self.x])
+
+    def __all__(self):
+        r"""
+
+        Returns True if all the elements of the TensorList are True.
+
+        """
+        return all([xi.all() for xi in self.x])
+
+    def __gt__(self, other):
+        r"""
+
+        Returns a TensorList of True if the elements of the input TensorList are greater than other.
+
+        """
+
+        return TensorList([xi > other for xi in self.x])
+
+    def __lt__(self, other):
+        r"""
+
+        Returns a TensorList of True if the elements of the TensorList are smaller than other.
+
+        """
+
+        return TensorList([xi < other for xi in self.x])
+
 
 def randn_like(x):
     r"""
     Returns a :class:`deepinv.utils.TensorList` or :class:`torch.Tensor`
     with the same type as x, filled with standard gaussian numbers.
     """
     if isinstance(x, torch.Tensor):
@@ -152,54 +224,37 @@
     """
     if isinstance(x, torch.Tensor):
         return torch.ones_like(x)
     else:
         return TensorList([torch.ones_like(xi) for xi in x])
 
 
-def get_freer_gpu():
+def get_freer_gpu(verbose=True):
     """
     Returns the GPU device with the most free memory.
 
     """
     try:
         if os.name == "posix":
             os.system("nvidia-smi -q -d Memory |grep -A5 GPU|grep Free >tmp")
             memory_available = [int(x.split()[2]) for x in open("tmp", "r").readlines()]
         else:
             os.system('bash -c "nvidia-smi -q -d Memory |grep -A5 GPU|grep Free >tmp"')
             memory_available = [int(x.split()[2]) for x in open("tmp", "r").readlines()]
         idx = np.argmax(memory_available)
         device = torch.device(f"cuda:{idx}")
-        print(f"Selected GPU {idx} with {np.max(memory_available)} MB free memory ")
+        if verbose:
+            print(f"Selected GPU {idx} with {np.max(memory_available)} MB free memory ")
     except:
         device = torch.device(f"cuda")
         print("Couldn't find free GPU")
 
     return device
 
 
-def save_model(
-    epoch, model, optimizer, ckp_interval, epochs, loss, save_path, eval_psnr=None
-):
-    if (epoch > 0 and epoch % ckp_interval == 0) or epoch + 1 == epochs:
-        os.makedirs(save_path, exist_ok=True)
-
-        state = {
-            "epoch": epoch,
-            "state_dict": model.state_dict(),
-            "loss": loss,
-            "optimizer": optimizer.state_dict(),
-        }
-        if eval_psnr is not None:
-            state["eval_psnr"] = eval_psnr
-        torch.save(state, os.path.join(save_path, "ckp_{}.pth.tar".format(epoch)))
-    pass
-
-
 def load_checkpoint(model, path_checkpoint, device):
     checkpoint = torch.load(path_checkpoint, map_location=device)
     model.load_state_dict(checkpoint["state_dict"])
     return model
 
 
 def investigate_model(model, idx_max=1, check_name="iterator.g_step.g_param.0"):
```

### Comparing `deepinv-0.1.1/deepinv/utils/optimization.py` & `deepinv-0.2.0/deepinv/utils/optimization.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv/utils/phantoms.py` & `deepinv-0.2.0/deepinv/utils/phantoms.py`

 * *Files identical despite different names*

### Comparing `deepinv-0.1.1/deepinv.egg-info/PKG-INFO` & `deepinv-0.2.0/deepinv.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepinv
-Version: 0.1.1
+Version: 0.2.0
 Summary: Pytorch library for solving inverse problems with deep learning
 Author-email: Julian Tachella <tachellajulian@gmail.com>
 License: BSD 3-Clause
 Project-URL: Homepage, https://deepinv.github.io/
 Project-URL: Source, https://github.com/deepinv/deepinv
 Project-URL: Tracker, https://github.com/deepinv/deepinv/issues
 Platform: any
@@ -33,20 +33,23 @@
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: coverage; extra == "test"
 Provides-Extra: doc
 Requires-Dist: sphinx; extra == "doc"
 Requires-Dist: sphinx_gallery; extra == "doc"
 Requires-Dist: sphinx_rtd_theme; extra == "doc"
 Requires-Dist: sphinxemoji; extra == "doc"
-Requires-Dist: sphinx_exec_code; extra == "doc"
+Requires-Dist: sphinx_copybutton; extra == "doc"
+Requires-Dist: sphinx_autoapi; extra == "doc"
 Provides-Extra: denoisers
 Requires-Dist: bm3d; extra == "denoisers"
 Requires-Dist: timm; extra == "denoisers"
 Requires-Dist: PyWavelets; extra == "denoisers"
 Requires-Dist: ptwt; extra == "denoisers"
+Requires-Dist: FrEIA; extra == "denoisers"
+Requires-Dist: pyiqa; extra == "denoisers"
 
 .. image:: https://github.com/deepinv/deepinv/raw/main/docs/source/figures/deepinv_logolarge.png
    :width: 500px
    :alt: deepinv logo
    :align: center
 
 
@@ -96,30 +99,30 @@
 
 Getting Started
 ---------------
 Try out the following plug-and-play image inpainting example:
 
 .. code-block:: python
 
-    import deepinv as dinv
-    from deepinv.utils import load_url_image
-
-    url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
-    x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
-
-    physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
-                                       noise_model=dinv.physics.GaussianNoise(sigma=0.01))
-
-    data_fidelity = dinv.optim.data_fidelity.L2()
-    prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
-    model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
-                                     params_algo={"stepsize": 1.0, "g_param": 0.1, "lambda": 2.})
-    y = physics(x)
-    x_hat = model(y, physics)
-    dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
+    >>> import deepinv as dinv
+    >>> from deepinv.utils import load_url_image
+    >>>
+    >>> url = ("https://huggingface.co/datasets/deepinv/images/resolve/main/cameraman.png?download=true")
+    >>> x = load_url_image(url=url, img_size=512, grayscale=True, device='cpu')
+    >>>
+    >>> physics = dinv.physics.Inpainting((1, 512, 512), mask = 0.5, \
+    >>>                                    noise_model=dinv.physics.GaussianNoise(sigma=0.01))
+    >>>
+    >>> data_fidelity = dinv.optim.data_fidelity.L2()
+    >>> prior = dinv.optim.prior.PnP(denoiser=dinv.models.MedianFilter())
+    >>> model = dinv.optim.optim_builder(iteration="HQS", prior=prior, data_fidelity=data_fidelity, \
+    >>>                                 params_algo={"stepsize": 1.0, "g_param": 0.1})
+    >>> y = physics(x)
+    >>> x_hat = model(y, physics)
+    >>> dinv.utils.plot([x, y, x_hat], ["signal", "measurement", "estimate"], rescale_mode='clip')
 
 
 Also try out `one of the examples <https://deepinv.github.io/deepinv/auto_examples/index.html>`_ to get started.
 
 Contributing
 ------------
```

### Comparing `deepinv-0.1.1/deepinv.egg-info/SOURCES.txt` & `deepinv-0.2.0/deepinv.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 LICENSE
 README.rst
 pyproject.toml
 deepinv/__about__.py
 deepinv/__init__.py
-deepinv/training_utils.py
 deepinv.egg-info/PKG-INFO
 deepinv.egg-info/SOURCES.txt
 deepinv.egg-info/dependency_links.txt
 deepinv.egg-info/requires.txt
 deepinv.egg-info/top_level.txt
 deepinv/datasets/__init__.py
 deepinv/datasets/datagenerator.py
+deepinv/datasets/patch_dataset.py
 deepinv/loss/__init__.py
 deepinv/loss/ei.py
+deepinv/loss/loss.py
 deepinv/loss/mc.py
 deepinv/loss/measplit.py
 deepinv/loss/metric.py
 deepinv/loss/moi.py
 deepinv/loss/r2r.py
 deepinv/loss/regularisers.py
 deepinv/loss/score.py
@@ -29,74 +30,98 @@
 deepinv/models/ae.py
 deepinv/models/artifactremoval.py
 deepinv/models/bm3d.py
 deepinv/models/diffunet.py
 deepinv/models/dip.py
 deepinv/models/dncnn.py
 deepinv/models/drunet.py
+deepinv/models/epll.py
 deepinv/models/equivariant.py
 deepinv/models/median.py
+deepinv/models/restormer.py
 deepinv/models/scunet.py
 deepinv/models/swinir.py
 deepinv/models/tgv.py
 deepinv/models/tv.py
 deepinv/models/unet.py
 deepinv/models/utils.py
 deepinv/models/wavdict.py
 deepinv/optim/__init__.py
 deepinv/optim/data_fidelity.py
+deepinv/optim/dpir.py
+deepinv/optim/epll.py
 deepinv/optim/fixed_point.py
 deepinv/optim/optimizers.py
 deepinv/optim/prior.py
 deepinv/optim/utils.py
 deepinv/optim/optim_iterators/__init__.py
 deepinv/optim/optim_iterators/admm.py
 deepinv/optim/optim_iterators/drs.py
 deepinv/optim/optim_iterators/gradient_descent.py
 deepinv/optim/optim_iterators/hqs.py
 deepinv/optim/optim_iterators/optim_iterator.py
 deepinv/optim/optim_iterators/pgd.py
 deepinv/optim/optim_iterators/primal_dual_CP.py
+deepinv/optim/optim_iterators/spectral_methods.py
 deepinv/optim/optim_iterators/utils.py
 deepinv/physics/__init__.py
 deepinv/physics/blur.py
 deepinv/physics/compressed_sensing.py
 deepinv/physics/forward.py
 deepinv/physics/haze.py
 deepinv/physics/inpainting.py
 deepinv/physics/lidar.py
 deepinv/physics/mri.py
 deepinv/physics/noise.py
+deepinv/physics/phase_retrieval.py
 deepinv/physics/range.py
 deepinv/physics/remote_sensing.py
 deepinv/physics/singlepixel.py
 deepinv/physics/tomography.py
+deepinv/physics/functional/__init__.py
+deepinv/physics/functional/convolution.py
+deepinv/physics/functional/downsampling.py
+deepinv/physics/functional/hist.py
+deepinv/physics/functional/interp.py
+deepinv/physics/functional/multiplier.py
+deepinv/physics/functional/product_convolution.py
+deepinv/physics/functional/radon.py
+deepinv/physics/generator/__init__.py
+deepinv/physics/generator/base.py
+deepinv/physics/generator/blur.py
+deepinv/physics/generator/mri.py
+deepinv/physics/generator/noise.py
 deepinv/sampling/__init__.py
 deepinv/sampling/diffusion.py
 deepinv/sampling/langevin.py
 deepinv/sampling/utils.py
 deepinv/tests/conftest.py
+deepinv/tests/test_generators.py
 deepinv/tests/test_loss.py
 deepinv/tests/test_loss_train.py
 deepinv/tests/test_models.py
 deepinv/tests/test_optim.py
 deepinv/tests/test_physics.py
 deepinv/tests/test_sampling.py
 deepinv/tests/test_unfolded.py
 deepinv/tests/test_utils.py
 deepinv/tests/dummy_datasets/datasets.py
+deepinv/training/__init__.py
+deepinv/training/testing.py
+deepinv/training/trainer.py
 deepinv/transform/__init__.py
 deepinv/transform/rotate.py
 deepinv/transform/scale.py
 deepinv/transform/shift.py
 deepinv/unfolded/__init__.py
 deepinv/unfolded/deep_equilibrium.py
 deepinv/unfolded/unfolded.py
 deepinv/utils/__init__.py
 deepinv/utils/demo.py
 deepinv/utils/logger.py
 deepinv/utils/metric.py
 deepinv/utils/nn.py
 deepinv/utils/optimization.py
 deepinv/utils/parameters.py
+deepinv/utils/patch_extractor.py
 deepinv/utils/phantoms.py
 deepinv/utils/plotting.py
```

### Comparing `deepinv-0.1.1/pyproject.toml` & `deepinv-0.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Utilities",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries",
 ]
 requires-python = ">=3.8"
-version = "0.1.1"
+version = "0.2.0"
 dependencies = [
     "numpy",
     "matplotlib",
     "hdf5storage",
     "tqdm",
     "torch",
     "torchvision",
@@ -51,23 +51,27 @@
 ]
 
 doc = [
     "sphinx",
     "sphinx_gallery",
     "sphinx_rtd_theme",
     "sphinxemoji",
-    "sphinx_exec_code"
+    "sphinx_copybutton",
+    "sphinx_autoapi"
+
 ]
 
 # optional dependencies for specific denoisers
 denoisers = [
     "bm3d",
     "timm",
     "PyWavelets",
-    "ptwt"
+    "ptwt",
+    "FrEIA",
+    "pyiqa"
 ]
 
 
 #####################################################################
 # Pytest configuration and coverage reporting
 
 [tool.pytest.ini_options]
```

