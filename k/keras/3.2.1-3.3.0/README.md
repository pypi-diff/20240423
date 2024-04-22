# Comparing `tmp/keras-3.2.1.tar.gz` & `tmp/keras-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-3.2.1.tar", last modified: Wed Apr 10 20:34:07 2024, max compression
+gzip compressed data, was "keras-3.3.0.tar", last modified: Mon Apr 22 18:30:47 2024, max compression
```

## Comparing `keras-3.2.1.tar` & `keras-3.3.0.tar`

### file list

```diff
@@ -1,691 +1,921 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.329379 keras-3.2.1/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-04-10 20:34:07.329096 keras-3.2.1/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4673 2024-04-10 20:33:59.000000 keras-3.2.1/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.230218 keras-3.2.1/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2095 2024-04-10 20:34:04.000000 keras-3.2.1/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.231670 keras-3.2.1/keras/_tf_keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.231829 keras-3.2.1/keras/_tf_keras/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2248 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.231998 keras-3.2.1/keras/_tf_keras/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.232164 keras-3.2.1/keras/_tf_keras/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.232333 keras-3.2.1/keras/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.232576 keras-3.2.1/keras/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.232782 keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.232974 keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233144 keras-3.2.1/keras/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233305 keras-3.2.1/keras/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233474 keras-3.2.1/keras/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233645 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233811 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.233998 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.234181 keras-3.2.1/keras/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.234368 keras-3.2.1/keras/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.234546 keras-3.2.1/keras/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.234733 keras-3.2.1/keras/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.234938 keras-3.2.1/keras/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235125 keras-3.2.1/keras/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235302 keras-3.2.1/keras/_tf_keras/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235478 keras-3.2.1/keras/_tf_keras/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6809 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235649 keras-3.2.1/keras/_tf_keras/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235805 keras-3.2.1/keras/_tf_keras/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.235952 keras-3.2.1/keras/_tf_keras/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.236109 keras-3.2.1/keras/_tf_keras/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.236292 keras-3.2.1/keras/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.236505 keras-3.2.1/keras/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.236695 keras-3.2.1/keras/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.236871 keras-3.2.1/keras/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237052 keras-3.2.1/keras/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237240 keras-3.2.1/keras/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237394 keras-3.2.1/keras/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237542 keras-3.2.1/keras/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237691 keras-3.2.1/keras/_tf_keras/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237839 keras-3.2.1/keras/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.237990 keras-3.2.1/keras/_tf_keras/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.238166 keras-3.2.1/keras/_tf_keras/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.238340 keras-3.2.1/keras/_tf_keras/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10079 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.238595 keras-3.2.1/keras/_tf_keras/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.238756 keras-3.2.1/keras/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.238920 keras-3.2.1/keras/_tf_keras/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3265 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239079 keras-3.2.1/keras/_tf_keras/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5156 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239260 keras-3.2.1/keras/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239427 keras-3.2.1/keras/_tf_keras/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239581 keras-3.2.1/keras/_tf_keras/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8668 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239787 keras-3.2.1/keras/_tf_keras/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.239936 keras-3.2.1/keras/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240085 keras-3.2.1/keras/_tf_keras/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240229 keras-3.2.1/keras/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5607 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240391 keras-3.2.1/keras/_tf_keras/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240544 keras-3.2.1/keras/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240689 keras-3.2.1/keras/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240831 keras-3.2.1/keras/_tf_keras/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      757 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.240979 keras-3.2.1/keras/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1365 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241127 keras-3.2.1/keras/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      510 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241270 keras-3.2.1/keras/_tf_keras/keras/preprocessing/text/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/preprocessing/text/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241425 keras-3.2.1/keras/_tf_keras/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241582 keras-3.2.1/keras/_tf_keras/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241740 keras-3.2.1/keras/_tf_keras/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.241880 keras-3.2.1/keras/_tf_keras/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      915 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242020 keras-3.2.1/keras/_tf_keras/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242164 keras-3.2.1/keras/_tf_keras/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242321 keras-3.2.1/keras/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-10 20:34:04.000000 keras-3.2.1/keras/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242478 keras-3.2.1/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1348 2024-04-10 20:34:04.000000 keras-3.2.1/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242625 keras-3.2.1/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3228 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242768 keras-3.2.1/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.242915 keras-3.2.1/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      415 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243061 keras-3.2.1/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      759 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243199 keras-3.2.1/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      734 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243344 keras-3.2.1/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      259 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243501 keras-3.2.1/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      342 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243653 keras-3.2.1/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243797 keras-3.2.1/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      304 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.243933 keras-3.2.1/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      315 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244073 keras-3.2.1/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      255 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244222 keras-3.2.1/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      352 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244377 keras-3.2.1/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      398 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244527 keras-3.2.1/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      294 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244683 keras-3.2.1/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      419 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244821 keras-3.2.1/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.244968 keras-3.2.1/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      288 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245109 keras-3.2.1/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      300 2024-04-10 20:34:04.000000 keras-3.2.1/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245253 keras-3.2.1/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      884 2024-04-10 20:34:04.000000 keras-3.2.1/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245414 keras-3.2.1/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1045 2024-04-10 20:34:04.000000 keras-3.2.1/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245565 keras-3.2.1/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1144 2024-04-10 20:34:04.000000 keras-3.2.1/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245707 keras-3.2.1/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      798 2024-04-10 20:34:04.000000 keras-3.2.1/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.245845 keras-3.2.1/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246000 keras-3.2.1/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246139 keras-3.2.1/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      183 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246300 keras-3.2.1/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246448 keras-3.2.1/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      173 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246598 keras-3.2.1/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246739 keras-3.2.1/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      220 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.246878 keras-3.2.1/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247027 keras-3.2.1/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      281 2024-04-10 20:34:04.000000 keras-3.2.1/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247182 keras-3.2.1/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      776 2024-04-10 20:34:04.000000 keras-3.2.1/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247343 keras-3.2.1/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      323 2024-04-10 20:34:04.000000 keras-3.2.1/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247494 keras-3.2.1/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-10 20:34:04.000000 keras-3.2.1/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247633 keras-3.2.1/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2746 2024-04-10 20:34:04.000000 keras-3.2.1/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247772 keras-3.2.1/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9757 2024-04-10 20:34:04.000000 keras-3.2.1/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.247972 keras-3.2.1/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      155 2024-04-10 20:34:04.000000 keras-3.2.1/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248112 keras-3.2.1/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-10 20:34:04.000000 keras-3.2.1/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248253 keras-3.2.1/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2294 2024-04-10 20:34:04.000000 keras-3.2.1/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248398 keras-3.2.1/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4231 2024-04-10 20:34:04.000000 keras-3.2.1/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248559 keras-3.2.1/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-10 20:34:04.000000 keras-3.2.1/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248703 keras-3.2.1/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      417 2024-04-10 20:34:04.000000 keras-3.2.1/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.248846 keras-3.2.1/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8668 2024-04-10 20:34:04.000000 keras-3.2.1/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249051 keras-3.2.1/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      394 2024-04-10 20:34:04.000000 keras-3.2.1/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249199 keras-3.2.1/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      519 2024-04-10 20:34:04.000000 keras-3.2.1/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249344 keras-3.2.1/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1425 2024-04-10 20:34:04.000000 keras-3.2.1/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249497 keras-3.2.1/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5607 2024-04-10 20:34:04.000000 keras-3.2.1/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249655 keras-3.2.1/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      958 2024-04-10 20:34:04.000000 keras-3.2.1/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249797 keras-3.2.1/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      517 2024-04-10 20:34:04.000000 keras-3.2.1/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.249940 keras-3.2.1/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      865 2024-04-10 20:34:04.000000 keras-3.2.1/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250082 keras-3.2.1/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      437 2024-04-10 20:34:04.000000 keras-3.2.1/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250227 keras-3.2.1/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      380 2024-04-10 20:34:04.000000 keras-3.2.1/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250376 keras-3.2.1/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      180 2024-04-10 20:34:04.000000 keras-3.2.1/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250535 keras-3.2.1/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      423 2024-04-10 20:34:04.000000 keras-3.2.1/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250679 keras-3.2.1/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      629 2024-04-10 20:34:04.000000 keras-3.2.1/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250817 keras-3.2.1/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      811 2024-04-10 20:34:04.000000 keras-3.2.1/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.250952 keras-3.2.1/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      915 2024-04-10 20:34:04.000000 keras-3.2.1/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.251390 keras-3.2.1/keras/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      649 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.251678 keras-3.2.1/keras/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3541 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12443 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.255021 keras-3.2.1/keras/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24920 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16849 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25275 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40461 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16035 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14510 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15521 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17169 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17935 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23522 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30695 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19007 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6364 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9111 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9434 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12706 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.255590 keras-3.2.1/keras/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1972 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.256877 keras-3.2.1/keras/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      584 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9738 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9809 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/dtypes.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3007 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8981 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2546 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/name_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3660 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20234 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7140 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1057 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.259308 keras-3.2.1/keras/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1174 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12772 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9680 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5711 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       26 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1756 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8758 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18796 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29444 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3688 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3595 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7559 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13805 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    36171 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.261181 keras-3.2.1/keras/src/backend/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1013 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6862 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6920 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       28 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1921 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10587 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17760 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27723 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3962 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7659 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10708 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.264967 keras-3.2.1/keras/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1459 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9503 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2427 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7676 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6112 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11446 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26462 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    67409 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9264 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34607 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32141 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1994 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33608 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.267582 keras-3.2.1/keras/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1893 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16169 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9756 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1279 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1755 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15074 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24038 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    45949 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.269444 keras-3.2.1/keras/src/backend/torch/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       79 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1673 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1890 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      151 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1042 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2422 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1804 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      791 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2054 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1176 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8293 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13711 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17489 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.272110 keras-3.2.1/keras/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6944 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9831 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5262 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3207 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8934 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1302 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3442 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2966 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18489 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3105 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5340 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2728 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6844 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26400 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      670 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/callbacks/terminate_on_nan.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.272437 keras-3.2.1/keras/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1716 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7334 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/constraints/constraints.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.274166 keras-3.2.1/keras/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      384 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2645 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3851 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      705 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3087 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2915 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2930 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7150 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2394 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7204 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.274470 keras-3.2.1/keras/src/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      719 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/distribution/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31208 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/distribution/distribution_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.275226 keras-3.2.1/keras/src/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1033 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9952 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/dtype_policies/dtype_policy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.275563 keras-3.2.1/keras/src/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       55 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/export/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32837 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/export/export_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.276204 keras-3.2.1/keras/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3959 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4885 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2634 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23463 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/initializers/random_initializers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.276776 keras-3.2.1/keras/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8786 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.280072 keras-3.2.1/keras/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      273 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1237 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      810 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1901 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3454 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2671 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2259 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/activations/softmax.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.281000 keras-3.2.1/keras/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4331 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11890 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17953 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27410 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/attention/multi_head_attention.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.284045 keras-3.2.1/keras/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12031 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10696 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11618 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12644 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7301 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5572 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5671 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5692 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5894 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5898 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6000 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6088 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6451 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6532 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/convolutional/separable_conv2d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.285610 keras-3.2.1/keras/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16970 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33719 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15723 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      824 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5108 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8996 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2630 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1536 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9834 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    62881 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.287371 keras-3.2.1/keras/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2151 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9250 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6587 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12808 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2215 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2213 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2685 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.288484 keras-3.2.1/keras/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13441 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8535 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9837 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4307 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1832 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/normalization/unit_normalization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.290879 keras-3.2.1/keras/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3345 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4151 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3236 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1461 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2426 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3132 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2470 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2358 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2452 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2586 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4126 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3226 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/pooling/max_pooling3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.296073 keras-3.2.1/keras/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14573 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8706 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5490 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13176 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29620 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8318 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10937 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    41400 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18459 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13921 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6462 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3815 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6316 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3806 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9646 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10615 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10816 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2178 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4615 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17735 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27821 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2140 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.297156 keras-3.2.1/keras/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1199 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3596 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3005 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2017 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2063 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7301 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/regularization/spatial_dropout.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.300089 keras-3.2.1/keras/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2761 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9045 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11266 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3060 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2088 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1336 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2323 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1593 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5993 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4911 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2107 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4647 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5061 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/reshaping/zero_padding3d.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.304175 keras-3.2.1/keras/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13204 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27249 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8295 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8380 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8288 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27708 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26551 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18875 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17538 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4950 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4798 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/layers/rnn/time_distributed.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.305194 keras-3.2.1/keras/src/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    70242 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/backend.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8413 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/layers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      524 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.306446 keras-3.2.1/keras/src/legacy/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    65546 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11173 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11111 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.307480 keras-3.2.1/keras/src/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7297 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22746 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      486 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9282 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21809 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.308324 keras-3.2.1/keras/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6173 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5899 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    66376 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/losses/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.310853 keras-3.2.1/keras/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7190 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15605 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61580 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11744 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3256 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26857 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8187 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26612 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10538 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7213 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19819 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/metrics/regression_metrics.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.311968 keras-3.2.1/keras/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      144 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11101 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32151 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22650 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13020 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/sequential.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2165 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/models/variable_mapping.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.314494 keras-3.2.1/keras/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      645 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22873 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15341 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31490 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17411 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30619 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    62114 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5585 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   190019 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10476 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13766 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1701 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/ops/symbolic_arguments.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.316809 keras-3.2.1/keras/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3932 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4568 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7446 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3727 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5718 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4892 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3593 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    36798 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8908 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4778 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11554 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5735 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      814 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5811 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/rmsprop.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.317121 keras-3.2.1/keras/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      520 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35508 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4365 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/optimizers/sgd.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.317430 keras-3.2.1/keras/src/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1580 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/quantizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3231 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/quantizers/quantizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.318514 keras-3.2.1/keras/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      421 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13439 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4660 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/random/seed_generator.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.318863 keras-3.2.1/keras/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1732 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11800 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/regularizers/regularizers.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.319793 keras-3.2.1/keras/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      615 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7359 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9668 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27009 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28701 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/saving/serialization_lib.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.320333 keras-3.2.1/keras/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      267 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26564 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6198 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/testing/test_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.320968 keras-3.2.1/keras/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25825 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/compile_utils.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.322560 keras-3.2.1/keras/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5424 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14330 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17068 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3102 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9724 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2870 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19413 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5231 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2650 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3924 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    45200 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/trainers/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.327904 keras-3.2.1/keras/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1415 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2877 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14203 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4144 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1443 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28538 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1484 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16372 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/file_utils.py
--rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16624 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16545 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3492 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26577 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/jax_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      264 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/jax_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15206 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1219 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/module_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1777 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4572 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10350 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4004 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1678 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4715 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14519 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10575 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4631 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/tf_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9843 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4988 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/torch_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9004 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8274 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/tracking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20703 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/utils/tree.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      190 2024-04-10 20:33:59.000000 keras-3.2.1/keras/src/version.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.328110 keras-3.2.1/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      549 2024-04-10 20:34:04.000000 keras-3.2.1/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.328261 keras-3.2.1/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-10 20:34:04.000000 keras-3.2.1/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.328409 keras-3.2.1/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      271 2024-04-10 20:34:04.000000 keras-3.2.1/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-10 20:34:07.328718 keras-3.2.1/keras.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5615 2024-04-10 20:34:07.000000 keras-3.2.1/keras.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19988 2024-04-10 20:34:07.000000 keras-3.2.1/keras.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-10 20:34:07.000000 keras-3.2.1/keras.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-10 20:34:07.000000 keras-3.2.1/keras.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-10 20:34:07.000000 keras-3.2.1/keras.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-10 20:34:07.329432 keras-3.2.1/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1861 2024-04-10 20:33:59.000000 keras-3.2.1/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.593129 keras-3.3.0/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11356 2023-09-22 16:55:14.000000 keras-3.3.0/LICENSE
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5753 2024-04-22 18:30:47.593031 keras-3.3.0/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4789 2024-04-20 16:30:07.000000 keras-3.3.0/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.345190 keras-3.3.0/benchmarks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.349220 keras-3.3.0/benchmarks/layer_benchmark/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3754 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/activation_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3052 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/attention_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9434 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/base_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7246 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/conv_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3033 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/core_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5706 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/merge_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3507 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/normalization_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8179 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/pooling_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4668 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/regularization_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7154 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/reshaping_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6189 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/rnn_benchmark.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.350277 keras-3.3.0/benchmarks/model_benchmark/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      790 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/benchmark_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4661 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/bert_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4498 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/image_classification_benchmark.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.351320 keras-3.3.0/benchmarks/torch_ctl_benchmark/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1087 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/benchmark_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2638 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2574 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.351581 keras-3.3.0/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      828 2024-04-20 19:17:05.000000 keras-3.3.0/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.353225 keras-3.3.0/keras/api/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.353607 keras-3.3.0/keras/api/_tf_keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-20 19:17:01.000000 keras-3.3.0/keras/api/_tf_keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.354274 keras-3.3.0/keras/api/_tf_keras/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2057 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.354854 keras-3.3.0/keras/api/_tf_keras/keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355077 keras-3.3.0/keras/api/_tf_keras/keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355454 keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355676 keras-3.3.0/keras/api/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355899 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356149 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356412 keras-3.3.0/keras/api/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356649 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356880 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357093 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357324 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357545 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357769 keras-3.3.0/keras/api/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358001 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358218 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358439 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358667 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358913 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359138 keras-3.3.0/keras/api/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359339 keras-3.3.0/keras/api/_tf_keras/keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359530 keras-3.3.0/keras/api/_tf_keras/keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359775 keras-3.3.0/keras/api/_tf_keras/keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359979 keras-3.3.0/keras/api/_tf_keras/keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360187 keras-3.3.0/keras/api/_tf_keras/keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360390 keras-3.3.0/keras/api/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360598 keras-3.3.0/keras/api/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360806 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361009 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361304 keras-3.3.0/keras/api/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361654 keras-3.3.0/keras/api/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.362807 keras-3.3.0/keras/api/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363008 keras-3.3.0/keras/api/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363194 keras-3.3.0/keras/api/_tf_keras/keras/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363379 keras-3.3.0/keras/api/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.0/keras/api/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363684 keras-3.3.0/keras/api/_tf_keras/keras/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363871 keras-3.3.0/keras/api/_tf_keras/keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364064 keras-3.3.0/keras/api/_tf_keras/keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364395 keras-3.3.0/keras/api/_tf_keras/keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364580 keras-3.3.0/keras/api/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364757 keras-3.3.0/keras/api/_tf_keras/keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364928 keras-3.3.0/keras/api/_tf_keras/keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365270 keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365438 keras-3.3.0/keras/api/_tf_keras/keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365621 keras-3.3.0/keras/api/_tf_keras/keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366004 keras-3.3.0/keras/api/_tf_keras/keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366188 keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366364 keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.373453 keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.373894 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374141 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374337 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374534 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374735 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374932 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.375931 keras-3.3.0/keras/api/_tf_keras/keras/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376149 keras-3.3.0/keras/api/_tf_keras/keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376337 keras-3.3.0/keras/api/_tf_keras/keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376539 keras-3.3.0/keras/api/_tf_keras/keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376738 keras-3.3.0/keras/api/_tf_keras/keras/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376935 keras-3.3.0/keras/api/_tf_keras/keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.377122 keras-3.3.0/keras/api/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.381399 keras-3.3.0/keras/api/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.381699 keras-3.3.0/keras/api/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.382463 keras-3.3.0/keras/api/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.382731 keras-3.3.0/keras/api/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.383547 keras-3.3.0/keras/api/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.384442 keras-3.3.0/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385250 keras-3.3.0/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385443 keras-3.3.0/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385647 keras-3.3.0/keras/api/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385873 keras-3.3.0/keras/api/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386084 keras-3.3.0/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386281 keras-3.3.0/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386463 keras-3.3.0/keras/api/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386802 keras-3.3.0/keras/api/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387013 keras-3.3.0/keras/api/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387202 keras-3.3.0/keras/api/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387383 keras-3.3.0/keras/api/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387599 keras-3.3.0/keras/api/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387803 keras-3.3.0/keras/api/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387986 keras-3.3.0/keras/api/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388185 keras-3.3.0/keras/api/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388382 keras-3.3.0/keras/api/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388575 keras-3.3.0/keras/api/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388778 keras-3.3.0/keras/api/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388952 keras-3.3.0/keras/api/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389148 keras-3.3.0/keras/api/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389370 keras-3.3.0/keras/api/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389570 keras-3.3.0/keras/api/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389764 keras-3.3.0/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390003 keras-3.3.0/keras/api/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390230 keras-3.3.0/keras/api/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390444 keras-3.3.0/keras/api/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390641 keras-3.3.0/keras/api/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390839 keras-3.3.0/keras/api/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.0/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391138 keras-3.3.0/keras/api/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391349 keras-3.3.0/keras/api/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391750 keras-3.3.0/keras/api/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392138 keras-3.3.0/keras/api/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392329 keras-3.3.0/keras/api/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392516 keras-3.3.0/keras/api/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392799 keras-3.3.0/keras/api/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393143 keras-3.3.0/keras/api/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393318 keras-3.3.0/keras/api/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393493 keras-3.3.0/keras/api/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393779 keras-3.3.0/keras/api/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393945 keras-3.3.0/keras/api/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.394189 keras-3.3.0/keras/api/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.394496 keras-3.3.0/keras/api/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395392 keras-3.3.0/keras/api/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395632 keras-3.3.0/keras/api/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395815 keras-3.3.0/keras/api/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396005 keras-3.3.0/keras/api/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396175 keras-3.3.0/keras/api/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396357 keras-3.3.0/keras/api/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396578 keras-3.3.0/keras/api/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396802 keras-3.3.0/keras/api/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.397096 keras-3.3.0/keras/api/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.398296 keras-3.3.0/keras/api/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.398577 keras-3.3.0/keras/api/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.399719 keras-3.3.0/keras/api/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.399911 keras-3.3.0/keras/api/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.400700 keras-3.3.0/keras/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      648 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.401439 keras-3.3.0/keras/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3540 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12442 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30862 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/activations_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.408011 keras-3.3.0/keras/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10394 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/applications_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24919 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16848 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25274 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40460 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16034 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11284 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/imagenet_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15520 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17168 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17934 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23521 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19006 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9110 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9433 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12705 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.409246 keras-3.3.0/keras/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1971 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.414887 keras-3.3.0/keras/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      583 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17099 2024-04-21 17:37:40.000000 keras-3.3.0/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8151 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/backend_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2118 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/compute_output_spec_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9808 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8548 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/dtypes_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      499 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/global_state_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8974 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15026 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/keras_tensor_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2101 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/name_scope_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3692 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1990 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/stateless_scope_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21446 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31785 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/variables_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7139 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1056 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.421169 keras-3.3.0/keras/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12765 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9679 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13481 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/distribution_lib_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14746 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       25 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1800 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8757 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26214 2024-04-22 16:38:23.000000 keras-3.3.0/keras/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30833 2024-04-22 17:47:17.000000 keras-3.3.0/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3856 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13804 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    36259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.425361 keras-3.3.0/keras/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6855 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13086 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       27 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1964 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18006 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28098 2024-04-21 17:26:32.000000 keras-3.3.0/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3961 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7652 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10738 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.432774 keras-3.3.0/keras/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1458 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9444 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4406 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/distribute_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2747 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14197 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4639 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6161 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11451 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1624 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/name_scope_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26595 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    77771 2024-04-21 17:37:08.000000 keras-3.3.0/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9334 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7667 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/optimizer_distribute_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34600 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13290 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/saved_model_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32268 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1993 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33111 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.437089 keras-3.3.0/keras/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1892 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16162 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14001 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1865 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15073 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24278 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    47434 2024-04-21 17:37:08.000000 keras-3.3.0/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.439641 keras-3.3.0/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       78 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1672 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2421 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1803 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      783 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2053 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8292 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13704 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17577 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.447451 keras-3.3.0/keras/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      922 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6109 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/backup_and_restore_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9830 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5255 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3206 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5831 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/csv_logger_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8933 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9528 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/early_stopping_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1301 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3441 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6061 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/lambda_callback_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2965 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3806 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/learning_rate_scheduler_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18488 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18107 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/model_checkpoint_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3104 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5339 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4313 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3766 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/remote_monitor_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6843 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6707 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/swap_ema_weights_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26393 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27236 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/tensorboard_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/terminate_on_nan.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1717 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/terminate_on_nan_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.448188 keras-3.3.0/keras/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1715 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7333 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/constraints.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3505 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/constraints_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.450084 keras-3.3.0/keras/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      383 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3850 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      704 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3086 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2914 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2929 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7149 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2393 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.450753 keras-3.3.0/keras/src/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      718 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31207 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18510 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/distribution_lib_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.451868 keras-3.3.0/keras/src/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3506 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12480 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/dtype_policy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19083 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/dtype_policy_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.452870 keras-3.3.0/keras/src/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       54 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32830 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/export_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33240 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/export_lib_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.454896 keras-3.3.0/keras/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3958 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4884 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/constant_initializers_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2633 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23462 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/random_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6637 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/random_initializers_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.456649 keras-3.3.0/keras/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8848 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.459603 keras-3.3.0/keras/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      272 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1236 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1108 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/activation_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      844 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/elu_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1900 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/leaky_relu_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3453 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1167 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/prelu_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2864 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/relu_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2258 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/softmax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1679 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/softmax_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.462138 keras-3.3.0/keras/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4330 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3030 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/additive_attention_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11889 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14343 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/attention_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17952 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7755 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/grouped_query_attention_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28353 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/multi_head_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13745 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/multi_head_attention_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.468561 keras-3.3.0/keras/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17263 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10695 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11617 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12643 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5571 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5691 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5893 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5897 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32424 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27575 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv_transpose_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5999 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6087 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6531 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11914 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.476049 keras-3.3.0/keras/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25345 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26286 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/dense_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    42181 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31411 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/layers/core/einsum_dense_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17364 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15413 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/embedding_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      817 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1098 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/identity_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5107 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/input_layer_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8989 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/lambda_layer_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2629 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1712 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/masking_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1535 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2589 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/wrapper_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9827 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    63788 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/layers/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34277 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/layer_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.478530 keras-3.3.0/keras/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9249 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6586 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12807 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9678 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/merging_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2211 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2684 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.481170 keras-3.3.0/keras/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13440 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8094 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/batch_normalization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8534 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5919 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/group_normalization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9836 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4832 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/layer_normalization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4306 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3034 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/spectral_normalization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1831 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/unit_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2062 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/unit_normalization_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.486574 keras-3.3.0/keras/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3235 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12382 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1460 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2425 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3131 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2469 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2603 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6009 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2357 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2451 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2585 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5370 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3343 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4125 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3225 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9863 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.501723 keras-3.3.0/keras/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14572 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8705 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/category_encoding_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5489 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/center_crop_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13145 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6031 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/discretization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29613 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21053 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/feature_space_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8317 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6810 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10936 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20526 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashing_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    41399 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21777 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/index_lookup_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18458 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3480 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/integer_lookup_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13920 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5271 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/normalization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6463 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4199 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_brightness_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3814 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1553 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_contrast_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6315 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_crop_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3805 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5398 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_flip_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9645 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2685 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_rotation_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10614 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11944 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_translation_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10820 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5186 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_zoom_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2177 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3007 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/rescaling_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5349 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/resizing_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17734 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1940 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/string_lookup_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27820 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5959 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/text_vectorization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.504175 keras-3.3.0/keras/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1198 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/activity_regularization_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2161 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/alpha_dropout_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2978 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2125 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/dropout_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1074 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_dropout_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1020 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_noise_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/spatial_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/spatial_dropout_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.512085 keras-3.3.0/keras/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2760 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2921 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping1d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9044 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5253 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping2d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11265 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7196 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping3d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3059 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4368 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/flatten_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2087 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2736 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/permute_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1335 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1548 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/repeat_vector_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3956 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/reshape_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1592 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2244 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling1d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5992 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5096 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling2d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4862 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling3d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1920 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding1d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3781 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding2d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4288 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding3d_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.520038 keras-3.3.0/keras/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9359 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/bidirectional_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27242 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8294 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2838 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm1d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8379 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3194 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm2d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8287 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3832 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm3d_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2275 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2132 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3299 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27701 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9441 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/gru_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26544 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9743 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/lstm_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19159 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15320 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/rnn_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17537 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9276 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/simple_rnn_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4943 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9872 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4797 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/time_distributed.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2814 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/time_distributed_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.521616 keras-3.3.0/keras/src/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    70241 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/backend.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/layers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      523 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.523180 keras-3.3.0/keras/src/legacy/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    65545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11172 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11110 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.525815 keras-3.3.0/keras/src/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7296 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3318 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/json_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22750 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19413 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/legacy_h5_format_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      485 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9275 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21808 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.527753 keras-3.3.0/keras/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5892 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9374 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/loss_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    69132 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/losses.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    54720 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/losses_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.535845 keras-3.3.0/keras/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7198 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15604 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17463 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/accuracy_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61579 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    63267 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/confusion_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11743 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15184 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/f_score_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3255 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/hinge_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26976 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17104 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/iou_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8186 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metric_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26611 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10692 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8939 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/probabilistic_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7212 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5044 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/reduction_metrics_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19818 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/regression_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14185 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/regression_metrics_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.539723 keras-3.3.0/keras/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      143 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11094 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4113 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/cloning_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32453 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14762 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/functional_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23789 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24695 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/models/model_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13013 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/sequential.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8380 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/sequential_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2164 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/variable_mapping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1350 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/variable_mapping_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.553292 keras-3.3.0/keras/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      644 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22866 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31327 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/core_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15334 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4890 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/function_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    37256 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31485 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/image_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18342 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19959 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/linalg_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30618 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    47868 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/math_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    64046 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    83662 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/ops/nn_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5583 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2206 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/node_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   195627 2024-04-21 17:37:09.000000 keras-3.3.0/keras/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   285133 2024-04-21 17:37:12.000000 keras-3.3.0/keras/src/ops/numpy_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10732 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5533 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13759 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7368 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/symbolic_arguments.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3615 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/symbolic_arguments_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.561781 keras-3.3.0/keras/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3931 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4759 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2744 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adadelta_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7637 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3791 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adafactor_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3918 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3249 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adagrad_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5909 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3657 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adam_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5083 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamax_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3784 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3254 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamw_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40410 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2634 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/ftrl_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4969 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2985 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/lion_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11553 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/loss_scale_optimizer_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5926 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3304 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/nadam_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      813 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11204 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer_sparse_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13009 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6003 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2761 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/rmsprop_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.562476 keras-3.3.0/keras/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      546 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    35507 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15392 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4556 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3392 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/sgd_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.563294 keras-3.3.0/keras/src/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1784 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4810 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/quantizers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3006 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/quantizers_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.564882 keras-3.3.0/keras/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      420 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13438 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17949 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/random_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4905 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/seed_generator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2855 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/seed_generator_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.565811 keras-3.3.0/keras/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1731 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/regularizers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5675 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/regularizers_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.569527 keras-3.3.0/keras/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      614 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7358 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4701 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/object_registration_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9737 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9033 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_api_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27008 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33448 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_lib_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29052 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/saving/serialization_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13761 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/saving/serialization_lib_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.570664 keras-3.3.0/keras/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      266 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6197 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10599 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_utils_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.572732 keras-3.3.0/keras/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25940 2024-04-22 17:46:41.000000 keras-3.3.0/keras/src/trainers/compile_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/compile_utils_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.577269 keras-3.3.0/keras/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5423 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14323 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9404 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17071 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3101 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9717 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2863 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6621 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5224 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10998 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2643 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7146 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3923 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5843 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/epoch_iterator_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    46449 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/trainers/trainer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    54651 2024-04-22 17:46:42.000000 keras-3.3.0/keras/src/trainers/trainer_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.578657 keras-3.3.0/keras/src/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      521 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4970 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11138 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/optree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/tree_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10359 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/tree_test.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.592112 keras-3.3.0/keras/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2876 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14664 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16561 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/audio_dataset_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4130 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1442 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5709 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/code_stats_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28554 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12500 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dataset_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5986 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dtype_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16371 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/file_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28322 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/file_utils_test.py
+-rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16538 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20039 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_dataset_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16544 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3491 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2361 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/io_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26570 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23050 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_layer_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      263 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1276 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1776 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4269 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/naming_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/numerical_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10349 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4003 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3512 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/python_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/rng_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4714 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4558 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/sequence_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14512 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1675 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/summary_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11279 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/text_dataset_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4630 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/tf_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9842 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7769 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/timeseries_dataset_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4991 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/torch_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8232 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/torch_utils_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8997 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8980 2024-04-21 17:38:44.000000 keras-3.3.0/keras/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2907 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/tracking_test.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      189 2024-04-22 18:30:45.000000 keras-3.3.0/keras/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.592605 keras-3.3.0/keras.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5753 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30370 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       17 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1128 2023-09-22 16:55:14.000000 keras-3.3.0/pyproject.toml
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      285 2024-04-22 18:30:47.593487 keras-3.3.0/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1769 2024-04-20 16:30:07.000000 keras-3.3.0/setup.py
```

### Comparing `keras-3.2.1/PKG-INFO` & `keras-3.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.2.1
+Version: 3.3.0
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
@@ -75,14 +76,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras-3.2.1/README.md` & `keras-3.3.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/activations/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.activations import deserialize
 from keras.src.activations import get
 from keras.src.activations import serialize
 from keras.src.activations.activations import elu
 from keras.src.activations.activations import exponential
 from keras.src.activations.activations import gelu
 from keras.src.activations.activations import hard_sigmoid
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/applications/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/applications/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.applications import convnext
-from keras.applications import densenet
-from keras.applications import efficientnet
-from keras.applications import efficientnet_v2
-from keras.applications import imagenet_utils
-from keras.applications import inception_resnet_v2
-from keras.applications import inception_v3
-from keras.applications import mobilenet
-from keras.applications import mobilenet_v2
-from keras.applications import mobilenet_v3
-from keras.applications import nasnet
-from keras.applications import resnet
-from keras.applications import resnet50
-from keras.applications import resnet_v2
-from keras.applications import vgg16
-from keras.applications import vgg19
-from keras.applications import xception
+from keras.api.applications import convnext
+from keras.api.applications import densenet
+from keras.api.applications import efficientnet
+from keras.api.applications import efficientnet_v2
+from keras.api.applications import imagenet_utils
+from keras.api.applications import inception_resnet_v2
+from keras.api.applications import inception_v3
+from keras.api.applications import mobilenet
+from keras.api.applications import mobilenet_v2
+from keras.api.applications import mobilenet_v3
+from keras.api.applications import nasnet
+from keras.api.applications import resnet
+from keras.api.applications import resnet50
+from keras.api.applications import resnet_v2
+from keras.api.applications import vgg16
+from keras.api.applications import vgg19
+from keras.api.applications import xception
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.densenet import DenseNet121
 from keras.src.applications.densenet import DenseNet169
@@ -49,16 +48,16 @@
 from keras.src.applications.inception_v3 import InceptionV3
 from keras.src.applications.mobilenet import MobileNet
 from keras.src.applications.mobilenet_v2 import MobileNetV2
 from keras.src.applications.mobilenet_v3 import MobileNetV3Large
 from keras.src.applications.mobilenet_v3 import MobileNetV3Small
 from keras.src.applications.nasnet import NASNetLarge
 from keras.src.applications.nasnet import NASNetMobile
+from keras.src.applications.resnet import ResNet50
 from keras.src.applications.resnet import ResNet101
 from keras.src.applications.resnet import ResNet152
-from keras.src.applications.resnet import ResNet50
+from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.resnet_v2 import ResNet101V2
 from keras.src.applications.resnet_v2 import ResNet152V2
-from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.vgg16 import VGG16
 from keras.src.applications.vgg19 import VGG19
 from keras.src.applications.xception import Xception
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/applications/convnext/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.convnext import decode_predictions
 from keras.src.applications.convnext import preprocess_input
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet import EfficientNetB0
 from keras.src.applications.efficientnet import EfficientNetB1
 from keras.src.applications.efficientnet import EfficientNetB2
 from keras.src.applications.efficientnet import EfficientNetB3
 from keras.src.applications.efficientnet import EfficientNetB4
 from keras.src.applications.efficientnet import EfficientNetB5
 from keras.src.applications.efficientnet import EfficientNetB6
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B0
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B1
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B2
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B3
 from keras.src.applications.efficientnet_v2 import EfficientNetV2L
 from keras.src.applications.efficientnet_v2 import EfficientNetV2M
 from keras.src.applications.efficientnet_v2 import EfficientNetV2S
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/callbacks/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.callbacks.backup_and_restore import BackupAndRestore
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.callback_list import CallbackList
 from keras.src.callbacks.csv_logger import CSVLogger
 from keras.src.callbacks.early_stopping import EarlyStopping
 from keras.src.callbacks.history import History
 from keras.src.callbacks.lambda_callback import LambdaCallback
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/config/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.config import backend
 from keras.src.backend.config import epsilon
 from keras.src.backend.config import floatx
 from keras.src.backend.config import image_data_format
 from keras.src.backend.config import set_epsilon
 from keras.src.backend.config import set_floatx
 from keras.src.backend.config import set_image_data_format
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/constraints/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.constraints import deserialize
 from keras.src.constraints import get
 from keras.src.constraints import serialize
 from keras.src.constraints.constraints import Constraint
 from keras.src.constraints.constraints import MaxNorm
 from keras.src.constraints.constraints import MaxNorm as max_norm
 from keras.src.constraints.constraints import MinMaxNorm
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/distribution/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.distribution.distribution_lib import DataParallel
 from keras.src.distribution.distribution_lib import DeviceMesh
 from keras.src.distribution.distribution_lib import LayoutMap
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/initializers/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/initializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.initializers import deserialize
 from keras.src.initializers import get
 from keras.src.initializers import serialize
 from keras.src.initializers.constant_initializers import Constant
 from keras.src.initializers.constant_initializers import Constant as constant
 from keras.src.initializers.constant_initializers import Identity
-from keras.src.initializers.constant_initializers import Identity as IdentityInitializer
+from keras.src.initializers.constant_initializers import (
+    Identity as IdentityInitializer,
+)
 from keras.src.initializers.constant_initializers import Identity as identity
 from keras.src.initializers.constant_initializers import Ones
 from keras.src.initializers.constant_initializers import Ones as ones
 from keras.src.initializers.constant_initializers import Zeros
 from keras.src.initializers.constant_initializers import Zeros as zeros
 from keras.src.initializers.initializer import Initializer
 from keras.src.initializers.random_initializers import GlorotNormal
-from keras.src.initializers.random_initializers import GlorotNormal as glorot_normal
+from keras.src.initializers.random_initializers import (
+    GlorotNormal as glorot_normal,
+)
 from keras.src.initializers.random_initializers import GlorotUniform
-from keras.src.initializers.random_initializers import GlorotUniform as glorot_uniform
+from keras.src.initializers.random_initializers import (
+    GlorotUniform as glorot_uniform,
+)
 from keras.src.initializers.random_initializers import HeNormal
 from keras.src.initializers.random_initializers import HeNormal as he_normal
 from keras.src.initializers.random_initializers import HeUniform
 from keras.src.initializers.random_initializers import HeUniform as he_uniform
 from keras.src.initializers.random_initializers import LecunNormal
-from keras.src.initializers.random_initializers import LecunNormal as lecun_normal
+from keras.src.initializers.random_initializers import (
+    LecunNormal as lecun_normal,
+)
 from keras.src.initializers.random_initializers import LecunUniform
-from keras.src.initializers.random_initializers import LecunUniform as lecun_uniform
+from keras.src.initializers.random_initializers import (
+    LecunUniform as lecun_uniform,
+)
 from keras.src.initializers.random_initializers import OrthogonalInitializer
-from keras.src.initializers.random_initializers import OrthogonalInitializer as Orthogonal
-from keras.src.initializers.random_initializers import OrthogonalInitializer as orthogonal
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as Orthogonal,
+)
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as orthogonal,
+)
 from keras.src.initializers.random_initializers import RandomNormal
-from keras.src.initializers.random_initializers import RandomNormal as random_normal
+from keras.src.initializers.random_initializers import (
+    RandomNormal as random_normal,
+)
 from keras.src.initializers.random_initializers import RandomUniform
-from keras.src.initializers.random_initializers import RandomUniform as random_uniform
+from keras.src.initializers.random_initializers import (
+    RandomUniform as random_uniform,
+)
 from keras.src.initializers.random_initializers import TruncatedNormal
-from keras.src.initializers.random_initializers import TruncatedNormal as truncated_normal
+from keras.src.initializers.random_initializers import (
+    TruncatedNormal as truncated_normal,
+)
 from keras.src.initializers.random_initializers import VarianceScaling
-from keras.src.initializers.random_initializers import VarianceScaling as variance_scaling
+from keras.src.initializers.random_initializers import (
+    VarianceScaling as variance_scaling,
+)
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/layers/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,56 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.export.export_lib import TFSMLayer
 from keras.src.layers import deserialize
 from keras.src.layers import serialize
 from keras.src.layers.activations.activation import Activation
 from keras.src.layers.activations.elu import ELU
 from keras.src.layers.activations.leaky_relu import LeakyReLU
 from keras.src.layers.activations.prelu import PReLU
 from keras.src.layers.activations.relu import ReLU
 from keras.src.layers.activations.softmax import Softmax
 from keras.src.layers.attention.additive_attention import AdditiveAttention
 from keras.src.layers.attention.attention import Attention
-from keras.src.layers.attention.grouped_query_attention import GroupedQueryAttention as GroupQueryAttention
+from keras.src.layers.attention.grouped_query_attention import (
+    GroupedQueryAttention as GroupQueryAttention,
+)
 from keras.src.layers.attention.multi_head_attention import MultiHeadAttention
 from keras.src.layers.convolutional.conv1d import Conv1D
 from keras.src.layers.convolutional.conv1d import Conv1D as Convolution1D
 from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose
-from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose as Convolution1DTranspose
+from keras.src.layers.convolutional.conv1d_transpose import (
+    Conv1DTranspose as Convolution1DTranspose,
+)
 from keras.src.layers.convolutional.conv2d import Conv2D
 from keras.src.layers.convolutional.conv2d import Conv2D as Convolution2D
 from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose
-from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose as Convolution2DTranspose
+from keras.src.layers.convolutional.conv2d_transpose import (
+    Conv2DTranspose as Convolution2DTranspose,
+)
 from keras.src.layers.convolutional.conv3d import Conv3D
 from keras.src.layers.convolutional.conv3d import Conv3D as Convolution3D
 from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose
-from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose as Convolution3DTranspose
+from keras.src.layers.convolutional.conv3d_transpose import (
+    Conv3DTranspose as Convolution3DTranspose,
+)
 from keras.src.layers.convolutional.depthwise_conv1d import DepthwiseConv1D
 from keras.src.layers.convolutional.depthwise_conv2d import DepthwiseConv2D
 from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D
-from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D as SeparableConvolution1D
+from keras.src.layers.convolutional.separable_conv1d import (
+    SeparableConv1D as SeparableConvolution1D,
+)
 from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D
-from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D as SeparableConvolution2D
+from keras.src.layers.convolutional.separable_conv2d import (
+    SeparableConv2D as SeparableConvolution2D,
+)
 from keras.src.layers.core.dense import Dense
 from keras.src.layers.core.einsum_dense import EinsumDense
 from keras.src.layers.core.embedding import Embedding
 from keras.src.layers.core.identity import Identity
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.core.lambda_layer import Lambda
@@ -59,37 +70,69 @@
 from keras.src.layers.merging.maximum import maximum
 from keras.src.layers.merging.minimum import Minimum
 from keras.src.layers.merging.minimum import minimum
 from keras.src.layers.merging.multiply import Multiply
 from keras.src.layers.merging.multiply import multiply
 from keras.src.layers.merging.subtract import Subtract
 from keras.src.layers.merging.subtract import subtract
-from keras.src.layers.normalization.batch_normalization import BatchNormalization
-from keras.src.layers.normalization.group_normalization import GroupNormalization
-from keras.src.layers.normalization.layer_normalization import LayerNormalization
-from keras.src.layers.normalization.spectral_normalization import SpectralNormalization
+from keras.src.layers.normalization.batch_normalization import (
+    BatchNormalization,
+)
+from keras.src.layers.normalization.group_normalization import (
+    GroupNormalization,
+)
+from keras.src.layers.normalization.layer_normalization import (
+    LayerNormalization,
+)
+from keras.src.layers.normalization.spectral_normalization import (
+    SpectralNormalization,
+)
 from keras.src.layers.normalization.unit_normalization import UnitNormalization
 from keras.src.layers.pooling.average_pooling1d import AveragePooling1D
-from keras.src.layers.pooling.average_pooling1d import AveragePooling1D as AvgPool1D
+from keras.src.layers.pooling.average_pooling1d import (
+    AveragePooling1D as AvgPool1D,
+)
 from keras.src.layers.pooling.average_pooling2d import AveragePooling2D
-from keras.src.layers.pooling.average_pooling2d import AveragePooling2D as AvgPool2D
+from keras.src.layers.pooling.average_pooling2d import (
+    AveragePooling2D as AvgPool2D,
+)
 from keras.src.layers.pooling.average_pooling3d import AveragePooling3D
-from keras.src.layers.pooling.average_pooling3d import AveragePooling3D as AvgPool3D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D as GlobalAvgPool1D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D as GlobalAvgPool2D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D as GlobalAvgPool3D
+from keras.src.layers.pooling.average_pooling3d import (
+    AveragePooling3D as AvgPool3D,
+)
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D,
+)
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D as GlobalAvgPool1D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D as GlobalAvgPool2D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D as GlobalAvgPool3D,
+)
 from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D
-from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D as GlobalMaxPool1D
+from keras.src.layers.pooling.global_max_pooling1d import (
+    GlobalMaxPooling1D as GlobalMaxPool1D,
+)
 from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D
-from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D as GlobalMaxPool2D
+from keras.src.layers.pooling.global_max_pooling2d import (
+    GlobalMaxPooling2D as GlobalMaxPool2D,
+)
 from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D
-from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D as GlobalMaxPool3D
+from keras.src.layers.pooling.global_max_pooling3d import (
+    GlobalMaxPooling3D as GlobalMaxPool3D,
+)
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D as MaxPool1D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D as MaxPool2D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D as MaxPool3D
 from keras.src.layers.preprocessing.audio_preprocessing import MelSpectrogram
@@ -107,15 +150,17 @@
 from keras.src.layers.preprocessing.random_rotation import RandomRotation
 from keras.src.layers.preprocessing.random_translation import RandomTranslation
 from keras.src.layers.preprocessing.random_zoom import RandomZoom
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
-from keras.src.layers.regularization.activity_regularization import ActivityRegularization
+from keras.src.layers.regularization.activity_regularization import (
+    ActivityRegularization,
+)
 from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
@@ -144,19 +189,7 @@
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
 from keras.src.utils.jax_layer import FlaxLayer
 from keras.src.utils.jax_layer import JaxLayer
 from keras.src.utils.torch_utils import TorchModuleWrapper
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.layers import AlphaDropout
-from keras.src.legacy.layers import RandomHeight
-from keras.src.legacy.layers import RandomWidth
-from keras.src.legacy.layers import ThresholdedReLU
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/losses/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/losses/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
+from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
-from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
 from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
@@ -24,14 +23,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -43,28 +43,8 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.losses import Reduction
-from keras.src.losses.losses import kl_divergence as KLD
-from keras.src.losses.losses import kl_divergence as kld
-from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
-from keras.src.losses.losses import log_cosh as logcosh
-from keras.src.losses.losses import mean_absolute_error as MAE
-from keras.src.losses.losses import mean_absolute_error as mae
-from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
-from keras.src.losses.losses import mean_absolute_percentage_error as mape
-from keras.src.losses.losses import mean_squared_error as MSE
-from keras.src.losses.losses import mean_squared_error as mse
-from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
-from keras.src.losses.losses import mean_squared_logarithmic_error as msle
+from keras.src.losses.losses import tversky
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/metrics/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/metrics/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
@@ -57,39 +56,21 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
 from keras.src.metrics.regression_metrics import MeanSquaredError
 from keras.src.metrics.regression_metrics import MeanSquaredLogarithmicError
 from keras.src.metrics.regression_metrics import R2Score
 from keras.src.metrics.regression_metrics import RootMeanSquaredError
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.losses.losses import kl_divergence as KLD
-from keras.src.losses.losses import kl_divergence as kld
-from keras.src.losses.losses import kl_divergence as kullback_leibler_divergence
-from keras.src.losses.losses import log_cosh as logcosh
-from keras.src.losses.losses import mean_absolute_error as MAE
-from keras.src.losses.losses import mean_absolute_error as mae
-from keras.src.losses.losses import mean_absolute_percentage_error as MAPE
-from keras.src.losses.losses import mean_absolute_percentage_error as mape
-from keras.src.losses.losses import mean_squared_error as MSE
-from keras.src.losses.losses import mean_squared_error as mse
-from keras.src.losses.losses import mean_squared_logarithmic_error as MSLE
-from keras.src.losses.losses import mean_squared_logarithmic_error as msle
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/mixed_precision/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import DTypePolicy as Policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy as global_policy
 from keras.src.dtype_policies.dtype_policy import set_dtype_policy
-from keras.src.dtype_policies.dtype_policy import set_dtype_policy as set_global_policy
+from keras.src.dtype_policies.dtype_policy import (
+    set_dtype_policy as set_global_policy,
+)
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/ops/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/ops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.ops import image
-from keras.ops import linalg
-from keras.ops import nn
-from keras.ops import numpy
+from keras.api.ops import image
+from keras.api.ops import linalg
+from keras.api.ops import nn
+from keras.api.ops import numpy
 from keras.src.ops.core import cast
 from keras.src.ops.core import cond
 from keras.src.ops.core import convert_to_numpy
 from keras.src.ops.core import convert_to_tensor
 from keras.src.ops.core import custom_gradient
 from keras.src.ops.core import fori_loop
 from keras.src.ops.core import is_tensor
@@ -24,14 +23,15 @@
 from keras.src.ops.core import stop_gradient
 from keras.src.ops.core import unstack
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
@@ -52,14 +52,15 @@
 from keras.src.ops.math import top_k
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
@@ -147,17 +148,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
@@ -186,14 +187,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
@@ -214,11 +216,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/ops/linalg/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/ops/nn/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/ops/numpy/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.numpy import abs
 from keras.src.ops.numpy import absolute
 from keras.src.ops.numpy import add
 from keras.src.ops.numpy import all
 from keras.src.ops.numpy import amax
 from keras.src.ops.numpy import amin
 from keras.src.ops.numpy import any
@@ -70,17 +69,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
@@ -109,14 +108,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
@@ -137,11 +137,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/optimizers/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.optimizers import legacy
-from keras.optimizers import schedules
+from keras.api.optimizers import legacy
+from keras.api.optimizers import schedules
 from keras.src.optimizers import deserialize
 from keras.src.optimizers import get
 from keras.src.optimizers import serialize
 from keras.src.optimizers.adadelta import Adadelta
 from keras.src.optimizers.adafactor import Adafactor
 from keras.src.optimizers.adagrad import Adagrad
 from keras.src.optimizers.adam import Adam
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers import LegacyOptimizerWarning as Adagrad
 from keras.src.optimizers import LegacyOptimizerWarning as Adam
 from keras.src.optimizers import LegacyOptimizerWarning as Ftrl
 from keras.src.optimizers import LegacyOptimizerWarning as Optimizer
 from keras.src.optimizers import LegacyOptimizerWarning as RMSprop
 from keras.src.optimizers import LegacyOptimizerWarning as SGD
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecayRestarts
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
-from keras.src.optimizers.schedules.learning_rate_schedule import PiecewiseConstantDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    CosineDecayRestarts,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    LearningRateSchedule,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PiecewiseConstantDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import deserialize
 from keras.src.optimizers.schedules.learning_rate_schedule import serialize
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/preprocessing/image/__init__.py` & `keras-3.3.0/keras/src/utils/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
+from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
+from keras.src.utils.dataset_utils import split_dataset
+from keras.src.utils.file_utils import get_file
+from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
 from keras.src.utils.image_utils import save_img
-from keras.src.utils.image_utils import smart_resize
-
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.legacy.preprocessing.image import DirectoryIterator
-from keras.src.legacy.preprocessing.image import ImageDataGenerator
-from keras.src.legacy.preprocessing.image import Iterator
-from keras.src.legacy.preprocessing.image import NumpyArrayIterator
-from keras.src.legacy.preprocessing.image import apply_affine_transform
-from keras.src.legacy.preprocessing.image import apply_brightness_shift
-from keras.src.legacy.preprocessing.image import apply_channel_shift
-from keras.src.legacy.preprocessing.image import random_brightness
-from keras.src.legacy.preprocessing.image import random_channel_shift
-from keras.src.legacy.preprocessing.image import random_rotation
-from keras.src.legacy.preprocessing.image import random_shear
-from keras.src.legacy.preprocessing.image import random_shift
-from keras.src.legacy.preprocessing.image import random_zoom
+from keras.src.utils.io_utils import disable_interactive_logging
+from keras.src.utils.io_utils import enable_interactive_logging
+from keras.src.utils.io_utils import is_interactive_logging_enabled
+from keras.src.utils.model_visualization import model_to_dot
+from keras.src.utils.model_visualization import plot_model
+from keras.src.utils.numerical_utils import normalize
+from keras.src.utils.numerical_utils import to_categorical
+from keras.src.utils.progbar import Progbar
+from keras.src.utils.python_utils import default
+from keras.src.utils.python_utils import is_default
+from keras.src.utils.python_utils import removeprefix
+from keras.src.utils.python_utils import removesuffix
+from keras.src.utils.rng_utils import set_random_seed
+from keras.src.utils.sequence_utils import pad_sequences
+from keras.src.utils.text_dataset_utils import text_dataset_from_directory
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/random/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/random/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.random.random import beta
 from keras.src.random.random import binomial
 from keras.src.random.random import categorical
 from keras.src.random.random import dropout
 from keras.src.random.random import gamma
 from keras.src.random.random import normal
 from keras.src.random.random import randint
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/regularizers/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/regularizers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.regularizers import deserialize
 from keras.src.regularizers import get
 from keras.src.regularizers import serialize
 from keras.src.regularizers.regularizers import L1
 from keras.src.regularizers.regularizers import L1 as l1
 from keras.src.regularizers.regularizers import L1L2
 from keras.src.regularizers.regularizers import L1L2 as l1_l2
 from keras.src.regularizers.regularizers import L2
 from keras.src.regularizers.regularizers import L2 as l2
 from keras.src.regularizers.regularizers import OrthogonalRegularizer
-from keras.src.regularizers.regularizers import OrthogonalRegularizer as orthogonal_regularizer
+from keras.src.regularizers.regularizers import (
+    OrthogonalRegularizer as orthogonal_regularizer,
+)
 from keras.src.regularizers.regularizers import Regularizer
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/saving/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/saving/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
```

### Comparing `keras-3.2.1/keras/_tf_keras/keras/utils/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
+from keras.api.utils import legacy
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.layers.preprocessing.feature_space import FeatureSpace
 from keras.src.ops.operation_utils import get_source_inputs
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-from keras.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
-from keras.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    pack_x_y_sample_weight,
+)
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    unpack_x_y_sample_weight,
+)
 from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset
-from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
+from keras.src.trainers.data_adapters.py_dataset_adapter import (
+    PyDataset as Sequence,
+)
 from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras.src.utils.dataset_utils import split_dataset
 from keras.src.utils.file_utils import get_file
 from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
@@ -37,9 +45,10 @@
 from keras.src.utils.model_visualization import plot_model
 from keras.src.utils.numerical_utils import normalize
 from keras.src.utils.numerical_utils import to_categorical
 from keras.src.utils.progbar import Progbar
 from keras.src.utils.rng_utils import set_random_seed
 from keras.src.utils.sequence_utils import pad_sequences
 from keras.src.utils.text_dataset_utils import text_dataset_from_directory
-from keras.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
-from keras.utils import legacy
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras-3.2.1/keras/activations/__init__.py` & `keras-3.3.0/keras/api/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.activations import deserialize
 from keras.src.activations import get
 from keras.src.activations import serialize
 from keras.src.activations.activations import elu
 from keras.src.activations.activations import exponential
 from keras.src.activations.activations import gelu
 from keras.src.activations.activations import hard_sigmoid
```

### Comparing `keras-3.2.1/keras/applications/__init__.py` & `keras-3.3.0/keras/api/applications/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.applications import convnext
-from keras.applications import densenet
-from keras.applications import efficientnet
-from keras.applications import efficientnet_v2
-from keras.applications import imagenet_utils
-from keras.applications import inception_resnet_v2
-from keras.applications import inception_v3
-from keras.applications import mobilenet
-from keras.applications import mobilenet_v2
-from keras.applications import mobilenet_v3
-from keras.applications import nasnet
-from keras.applications import resnet
-from keras.applications import resnet50
-from keras.applications import resnet_v2
-from keras.applications import vgg16
-from keras.applications import vgg19
-from keras.applications import xception
+from keras.api.applications import convnext
+from keras.api.applications import densenet
+from keras.api.applications import efficientnet
+from keras.api.applications import efficientnet_v2
+from keras.api.applications import imagenet_utils
+from keras.api.applications import inception_resnet_v2
+from keras.api.applications import inception_v3
+from keras.api.applications import mobilenet
+from keras.api.applications import mobilenet_v2
+from keras.api.applications import mobilenet_v3
+from keras.api.applications import nasnet
+from keras.api.applications import resnet
+from keras.api.applications import resnet50
+from keras.api.applications import resnet_v2
+from keras.api.applications import vgg16
+from keras.api.applications import vgg19
+from keras.api.applications import xception
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.densenet import DenseNet121
 from keras.src.applications.densenet import DenseNet169
@@ -49,16 +48,16 @@
 from keras.src.applications.inception_v3 import InceptionV3
 from keras.src.applications.mobilenet import MobileNet
 from keras.src.applications.mobilenet_v2 import MobileNetV2
 from keras.src.applications.mobilenet_v3 import MobileNetV3Large
 from keras.src.applications.mobilenet_v3 import MobileNetV3Small
 from keras.src.applications.nasnet import NASNetLarge
 from keras.src.applications.nasnet import NASNetMobile
+from keras.src.applications.resnet import ResNet50
 from keras.src.applications.resnet import ResNet101
 from keras.src.applications.resnet import ResNet152
-from keras.src.applications.resnet import ResNet50
+from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.resnet_v2 import ResNet101V2
 from keras.src.applications.resnet_v2 import ResNet152V2
-from keras.src.applications.resnet_v2 import ResNet50V2
 from keras.src.applications.vgg16 import VGG16
 from keras.src.applications.vgg19 import VGG19
 from keras.src.applications.xception import Xception
```

### Comparing `keras-3.2.1/keras/applications/convnext/__init__.py` & `keras-3.3.0/keras/api/applications/convnext/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.convnext import ConvNeXtBase
 from keras.src.applications.convnext import ConvNeXtLarge
 from keras.src.applications.convnext import ConvNeXtSmall
 from keras.src.applications.convnext import ConvNeXtTiny
 from keras.src.applications.convnext import ConvNeXtXLarge
 from keras.src.applications.convnext import decode_predictions
 from keras.src.applications.convnext import preprocess_input
```

### Comparing `keras-3.2.1/keras/applications/efficientnet/__init__.py` & `keras-3.3.0/keras/api/applications/efficientnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet import EfficientNetB0
 from keras.src.applications.efficientnet import EfficientNetB1
 from keras.src.applications.efficientnet import EfficientNetB2
 from keras.src.applications.efficientnet import EfficientNetB3
 from keras.src.applications.efficientnet import EfficientNetB4
 from keras.src.applications.efficientnet import EfficientNetB5
 from keras.src.applications.efficientnet import EfficientNetB6
```

### Comparing `keras-3.2.1/keras/applications/efficientnet_v2/__init__.py` & `keras-3.3.0/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B0
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B1
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B2
 from keras.src.applications.efficientnet_v2 import EfficientNetV2B3
 from keras.src.applications.efficientnet_v2 import EfficientNetV2L
 from keras.src.applications.efficientnet_v2 import EfficientNetV2M
 from keras.src.applications.efficientnet_v2 import EfficientNetV2S
```

### Comparing `keras-3.2.1/keras/backend/__init__.py` & `keras-3.3.0/keras/api/_tf_keras/keras/backend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import is_float_dtype
 from keras.src.backend.common.variables import is_int_dtype
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.config import backend
```

### Comparing `keras-3.2.1/keras/callbacks/__init__.py` & `keras-3.3.0/keras/api/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.callbacks.backup_and_restore import BackupAndRestore
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.callback_list import CallbackList
 from keras.src.callbacks.csv_logger import CSVLogger
 from keras.src.callbacks.early_stopping import EarlyStopping
 from keras.src.callbacks.history import History
 from keras.src.callbacks.lambda_callback import LambdaCallback
```

### Comparing `keras-3.2.1/keras/config/__init__.py` & `keras-3.3.0/keras/api/config/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.backend.config import backend
 from keras.src.backend.config import epsilon
 from keras.src.backend.config import floatx
 from keras.src.backend.config import image_data_format
 from keras.src.backend.config import set_epsilon
 from keras.src.backend.config import set_floatx
 from keras.src.backend.config import set_image_data_format
```

### Comparing `keras-3.2.1/keras/constraints/__init__.py` & `keras-3.3.0/keras/api/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.constraints import deserialize
 from keras.src.constraints import get
 from keras.src.constraints import serialize
 from keras.src.constraints.constraints import Constraint
 from keras.src.constraints.constraints import MaxNorm
 from keras.src.constraints.constraints import MaxNorm as max_norm
 from keras.src.constraints.constraints import MinMaxNorm
```

### Comparing `keras-3.2.1/keras/distribution/__init__.py` & `keras-3.3.0/keras/api/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.distribution.distribution_lib import DataParallel
 from keras.src.distribution.distribution_lib import DeviceMesh
 from keras.src.distribution.distribution_lib import LayoutMap
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
```

### Comparing `keras-3.2.1/keras/initializers/__init__.py` & `keras-3.3.0/keras/api/initializers/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,64 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.initializers import deserialize
 from keras.src.initializers import get
 from keras.src.initializers import serialize
 from keras.src.initializers.constant_initializers import Constant
 from keras.src.initializers.constant_initializers import Constant as constant
 from keras.src.initializers.constant_initializers import Identity
-from keras.src.initializers.constant_initializers import Identity as IdentityInitializer
+from keras.src.initializers.constant_initializers import (
+    Identity as IdentityInitializer,
+)
 from keras.src.initializers.constant_initializers import Identity as identity
 from keras.src.initializers.constant_initializers import Ones
 from keras.src.initializers.constant_initializers import Ones as ones
 from keras.src.initializers.constant_initializers import Zeros
 from keras.src.initializers.constant_initializers import Zeros as zeros
 from keras.src.initializers.initializer import Initializer
 from keras.src.initializers.random_initializers import GlorotNormal
-from keras.src.initializers.random_initializers import GlorotNormal as glorot_normal
+from keras.src.initializers.random_initializers import (
+    GlorotNormal as glorot_normal,
+)
 from keras.src.initializers.random_initializers import GlorotUniform
-from keras.src.initializers.random_initializers import GlorotUniform as glorot_uniform
+from keras.src.initializers.random_initializers import (
+    GlorotUniform as glorot_uniform,
+)
 from keras.src.initializers.random_initializers import HeNormal
 from keras.src.initializers.random_initializers import HeNormal as he_normal
 from keras.src.initializers.random_initializers import HeUniform
 from keras.src.initializers.random_initializers import HeUniform as he_uniform
 from keras.src.initializers.random_initializers import LecunNormal
-from keras.src.initializers.random_initializers import LecunNormal as lecun_normal
+from keras.src.initializers.random_initializers import (
+    LecunNormal as lecun_normal,
+)
 from keras.src.initializers.random_initializers import LecunUniform
-from keras.src.initializers.random_initializers import LecunUniform as lecun_uniform
+from keras.src.initializers.random_initializers import (
+    LecunUniform as lecun_uniform,
+)
 from keras.src.initializers.random_initializers import OrthogonalInitializer
-from keras.src.initializers.random_initializers import OrthogonalInitializer as Orthogonal
-from keras.src.initializers.random_initializers import OrthogonalInitializer as orthogonal
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as Orthogonal,
+)
+from keras.src.initializers.random_initializers import (
+    OrthogonalInitializer as orthogonal,
+)
 from keras.src.initializers.random_initializers import RandomNormal
-from keras.src.initializers.random_initializers import RandomNormal as random_normal
+from keras.src.initializers.random_initializers import (
+    RandomNormal as random_normal,
+)
 from keras.src.initializers.random_initializers import RandomUniform
-from keras.src.initializers.random_initializers import RandomUniform as random_uniform
+from keras.src.initializers.random_initializers import (
+    RandomUniform as random_uniform,
+)
 from keras.src.initializers.random_initializers import TruncatedNormal
-from keras.src.initializers.random_initializers import TruncatedNormal as truncated_normal
+from keras.src.initializers.random_initializers import (
+    TruncatedNormal as truncated_normal,
+)
 from keras.src.initializers.random_initializers import VarianceScaling
-from keras.src.initializers.random_initializers import VarianceScaling as variance_scaling
+from keras.src.initializers.random_initializers import (
+    VarianceScaling as variance_scaling,
+)
```

### Comparing `keras-3.2.1/keras/layers/__init__.py` & `keras-3.3.0/keras/src/layers/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,39 @@
-"""DO NOT EDIT.
-
-This file was autogenerated. Do not edit it by hand,
-since your modifications would be overwritten.
-"""
-
-
-from keras.src.export.export_lib import TFSMLayer
-from keras.src.layers import deserialize
-from keras.src.layers import serialize
+from keras.src.api_export import keras_export
 from keras.src.layers.activations.activation import Activation
 from keras.src.layers.activations.elu import ELU
 from keras.src.layers.activations.leaky_relu import LeakyReLU
 from keras.src.layers.activations.prelu import PReLU
 from keras.src.layers.activations.relu import ReLU
 from keras.src.layers.activations.softmax import Softmax
 from keras.src.layers.attention.additive_attention import AdditiveAttention
 from keras.src.layers.attention.attention import Attention
-from keras.src.layers.attention.grouped_query_attention import GroupedQueryAttention as GroupQueryAttention
+from keras.src.layers.attention.grouped_query_attention import (
+    GroupedQueryAttention,
+)
 from keras.src.layers.attention.multi_head_attention import MultiHeadAttention
 from keras.src.layers.convolutional.conv1d import Conv1D
-from keras.src.layers.convolutional.conv1d import Conv1D as Convolution1D
 from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose
-from keras.src.layers.convolutional.conv1d_transpose import Conv1DTranspose as Convolution1DTranspose
 from keras.src.layers.convolutional.conv2d import Conv2D
-from keras.src.layers.convolutional.conv2d import Conv2D as Convolution2D
 from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose
-from keras.src.layers.convolutional.conv2d_transpose import Conv2DTranspose as Convolution2DTranspose
 from keras.src.layers.convolutional.conv3d import Conv3D
-from keras.src.layers.convolutional.conv3d import Conv3D as Convolution3D
 from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose
-from keras.src.layers.convolutional.conv3d_transpose import Conv3DTranspose as Convolution3DTranspose
 from keras.src.layers.convolutional.depthwise_conv1d import DepthwiseConv1D
 from keras.src.layers.convolutional.depthwise_conv2d import DepthwiseConv2D
 from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D
-from keras.src.layers.convolutional.separable_conv1d import SeparableConv1D as SeparableConvolution1D
 from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D
-from keras.src.layers.convolutional.separable_conv2d import SeparableConv2D as SeparableConvolution2D
 from keras.src.layers.core.dense import Dense
 from keras.src.layers.core.einsum_dense import EinsumDense
 from keras.src.layers.core.embedding import Embedding
 from keras.src.layers.core.identity import Identity
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.core.lambda_layer import Lambda
 from keras.src.layers.core.masking import Masking
 from keras.src.layers.core.wrapper import Wrapper
-from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.merging.add import Add
 from keras.src.layers.merging.add import add
 from keras.src.layers.merging.average import Average
 from keras.src.layers.merging.average import average
 from keras.src.layers.merging.concatenate import Concatenate
 from keras.src.layers.merging.concatenate import concatenate
@@ -59,63 +43,68 @@
 from keras.src.layers.merging.maximum import maximum
 from keras.src.layers.merging.minimum import Minimum
 from keras.src.layers.merging.minimum import minimum
 from keras.src.layers.merging.multiply import Multiply
 from keras.src.layers.merging.multiply import multiply
 from keras.src.layers.merging.subtract import Subtract
 from keras.src.layers.merging.subtract import subtract
-from keras.src.layers.normalization.batch_normalization import BatchNormalization
-from keras.src.layers.normalization.group_normalization import GroupNormalization
-from keras.src.layers.normalization.layer_normalization import LayerNormalization
-from keras.src.layers.normalization.spectral_normalization import SpectralNormalization
+from keras.src.layers.normalization.batch_normalization import (
+    BatchNormalization,
+)
+from keras.src.layers.normalization.group_normalization import (
+    GroupNormalization,
+)
+from keras.src.layers.normalization.layer_normalization import (
+    LayerNormalization,
+)
+from keras.src.layers.normalization.spectral_normalization import (
+    SpectralNormalization,
+)
 from keras.src.layers.normalization.unit_normalization import UnitNormalization
 from keras.src.layers.pooling.average_pooling1d import AveragePooling1D
-from keras.src.layers.pooling.average_pooling1d import AveragePooling1D as AvgPool1D
 from keras.src.layers.pooling.average_pooling2d import AveragePooling2D
-from keras.src.layers.pooling.average_pooling2d import AveragePooling2D as AvgPool2D
 from keras.src.layers.pooling.average_pooling3d import AveragePooling3D
-from keras.src.layers.pooling.average_pooling3d import AveragePooling3D as AvgPool3D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D
-from keras.src.layers.pooling.global_average_pooling1d import GlobalAveragePooling1D as GlobalAvgPool1D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D
-from keras.src.layers.pooling.global_average_pooling2d import GlobalAveragePooling2D as GlobalAvgPool2D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D
-from keras.src.layers.pooling.global_average_pooling3d import GlobalAveragePooling3D as GlobalAvgPool3D
+from keras.src.layers.pooling.global_average_pooling1d import (
+    GlobalAveragePooling1D,
+)
+from keras.src.layers.pooling.global_average_pooling2d import (
+    GlobalAveragePooling2D,
+)
+from keras.src.layers.pooling.global_average_pooling3d import (
+    GlobalAveragePooling3D,
+)
 from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D
-from keras.src.layers.pooling.global_max_pooling1d import GlobalMaxPooling1D as GlobalMaxPool1D
 from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D
-from keras.src.layers.pooling.global_max_pooling2d import GlobalMaxPooling2D as GlobalMaxPool2D
 from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D
-from keras.src.layers.pooling.global_max_pooling3d import GlobalMaxPooling3D as GlobalMaxPool3D
 from keras.src.layers.pooling.max_pooling1d import MaxPooling1D
-from keras.src.layers.pooling.max_pooling1d import MaxPooling1D as MaxPool1D
 from keras.src.layers.pooling.max_pooling2d import MaxPooling2D
-from keras.src.layers.pooling.max_pooling2d import MaxPooling2D as MaxPool2D
 from keras.src.layers.pooling.max_pooling3d import MaxPooling3D
-from keras.src.layers.pooling.max_pooling3d import MaxPooling3D as MaxPool3D
 from keras.src.layers.preprocessing.audio_preprocessing import MelSpectrogram
 from keras.src.layers.preprocessing.category_encoding import CategoryEncoding
 from keras.src.layers.preprocessing.center_crop import CenterCrop
 from keras.src.layers.preprocessing.discretization import Discretization
 from keras.src.layers.preprocessing.hashed_crossing import HashedCrossing
 from keras.src.layers.preprocessing.hashing import Hashing
+from keras.src.layers.preprocessing.index_lookup import IndexLookup
 from keras.src.layers.preprocessing.integer_lookup import IntegerLookup
 from keras.src.layers.preprocessing.normalization import Normalization
 from keras.src.layers.preprocessing.random_brightness import RandomBrightness
 from keras.src.layers.preprocessing.random_contrast import RandomContrast
 from keras.src.layers.preprocessing.random_crop import RandomCrop
 from keras.src.layers.preprocessing.random_flip import RandomFlip
 from keras.src.layers.preprocessing.random_rotation import RandomRotation
 from keras.src.layers.preprocessing.random_translation import RandomTranslation
 from keras.src.layers.preprocessing.random_zoom import RandomZoom
 from keras.src.layers.preprocessing.rescaling import Rescaling
 from keras.src.layers.preprocessing.resizing import Resizing
 from keras.src.layers.preprocessing.string_lookup import StringLookup
 from keras.src.layers.preprocessing.text_vectorization import TextVectorization
-from keras.src.layers.regularization.activity_regularization import ActivityRegularization
+from keras.src.layers.regularization.activity_regularization import (
+    ActivityRegularization,
+)
 from keras.src.layers.regularization.alpha_dropout import AlphaDropout
 from keras.src.layers.regularization.dropout import Dropout
 from keras.src.layers.regularization.gaussian_dropout import GaussianDropout
 from keras.src.layers.regularization.gaussian_noise import GaussianNoise
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout1D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout2D
 from keras.src.layers.regularization.spatial_dropout import SpatialDropout3D
@@ -141,10 +130,46 @@
 from keras.src.layers.rnn.lstm import LSTM
 from keras.src.layers.rnn.lstm import LSTMCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNN
 from keras.src.layers.rnn.simple_rnn import SimpleRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.layers.rnn.time_distributed import TimeDistributed
-from keras.src.utils.jax_layer import FlaxLayer
-from keras.src.utils.jax_layer import JaxLayer
-from keras.src.utils.torch_utils import TorchModuleWrapper
+from keras.src.saving import serialization_lib
+
+
+@keras_export("keras.layers.serialize")
+def serialize(layer):
+    """Returns the layer configuration as a Python dict.
+
+    Args:
+        layer: A `keras.layers.Layer` instance to serialize.
+
+    Returns:
+        Python dict which contains the configuration of the layer.
+    """
+    return serialization_lib.serialize_keras_object(layer)
+
+
+@keras_export("keras.layers.deserialize")
+def deserialize(config, custom_objects=None):
+    """Returns a Keras layer object via its configuration.
+
+    Args:
+        config: A python dict containing a serialized layer configuration.
+        custom_objects: Optional dictionary mapping names (strings) to custom
+            objects (classes and functions) to be considered during
+            deserialization.
+
+    Returns:
+        A Keras layer instance.
+    """
+    obj = serialization_lib.deserialize_keras_object(
+        config,
+        custom_objects=custom_objects,
+    )
+    if not isinstance(obj, Layer):
+        raise ValueError(
+            "`keras.layers.deserialize` was passed a `config` object that is "
+            f"not a `keras.layers.Layer`. Received: {config}"
+        )
+    return obj
```

### Comparing `keras-3.2.1/keras/losses/__init__.py` & `keras-3.3.0/keras/api/losses/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses import deserialize
 from keras.src.losses import get
 from keras.src.losses import serialize
 from keras.src.losses.loss import Loss
+from keras.src.losses.losses import CTC
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
-from keras.src.losses.losses import CTC
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
 from keras.src.losses.losses import CosineSimilarity
 from keras.src.losses.losses import Dice
 from keras.src.losses.losses import Hinge
 from keras.src.losses.losses import Huber
@@ -24,14 +23,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -43,7 +43,8 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
```

### Comparing `keras-3.2.1/keras/metrics/__init__.py` & `keras-3.3.0/keras/api/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import hinge
 from keras.src.losses.losses import huber
@@ -57,15 +56,17 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
```

### Comparing `keras-3.2.1/keras/mixed_precision/__init__.py` & `keras-3.3.0/keras/api/mixed_precision/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.dtype_policies.dtype_policy import DTypePolicy
 from keras.src.dtype_policies.dtype_policy import DTypePolicy as Policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy
 from keras.src.dtype_policies.dtype_policy import dtype_policy as global_policy
 from keras.src.dtype_policies.dtype_policy import set_dtype_policy
-from keras.src.dtype_policies.dtype_policy import set_dtype_policy as set_global_policy
+from keras.src.dtype_policies.dtype_policy import (
+    set_dtype_policy as set_global_policy,
+)
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
```

### Comparing `keras-3.2.1/keras/ops/__init__.py` & `keras-3.3.0/keras/api/ops/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.ops import image
-from keras.ops import linalg
-from keras.ops import nn
-from keras.ops import numpy
+from keras.api.ops import image
+from keras.api.ops import linalg
+from keras.api.ops import nn
+from keras.api.ops import numpy
 from keras.src.ops.core import cast
 from keras.src.ops.core import cond
 from keras.src.ops.core import convert_to_numpy
 from keras.src.ops.core import convert_to_tensor
 from keras.src.ops.core import custom_gradient
 from keras.src.ops.core import fori_loop
 from keras.src.ops.core import is_tensor
@@ -24,14 +23,15 @@
 from keras.src.ops.core import stop_gradient
 from keras.src.ops.core import unstack
 from keras.src.ops.core import vectorized_map
 from keras.src.ops.core import while_loop
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
@@ -52,14 +52,15 @@
 from keras.src.ops.math import top_k
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
@@ -147,17 +148,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
@@ -186,14 +187,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
@@ -214,11 +216,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras-3.2.1/keras/ops/linalg/__init__.py` & `keras-3.3.0/keras/api/ops/linalg/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.linalg import cholesky
 from keras.src.ops.linalg import det
 from keras.src.ops.linalg import eig
+from keras.src.ops.linalg import eigh
 from keras.src.ops.linalg import inv
 from keras.src.ops.linalg import lu_factor
 from keras.src.ops.linalg import norm
 from keras.src.ops.linalg import qr
 from keras.src.ops.linalg import solve
 from keras.src.ops.linalg import solve_triangular
 from keras.src.ops.linalg import svd
```

### Comparing `keras-3.2.1/keras/ops/nn/__init__.py` & `keras-3.3.0/keras/api/ops/nn/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.nn import average_pool
 from keras.src.ops.nn import batch_normalization
 from keras.src.ops.nn import binary_crossentropy
 from keras.src.ops.nn import categorical_crossentropy
 from keras.src.ops.nn import conv
 from keras.src.ops.nn import conv_transpose
+from keras.src.ops.nn import ctc_decode
 from keras.src.ops.nn import ctc_loss
 from keras.src.ops.nn import depthwise_conv
 from keras.src.ops.nn import elu
 from keras.src.ops.nn import gelu
 from keras.src.ops.nn import hard_sigmoid
 from keras.src.ops.nn import hard_silu
 from keras.src.ops.nn import hard_silu as hard_swish
```

### Comparing `keras-3.2.1/keras/ops/numpy/__init__.py` & `keras-3.3.0/keras/api/ops/numpy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.ops.numpy import abs
 from keras.src.ops.numpy import absolute
 from keras.src.ops.numpy import add
 from keras.src.ops.numpy import all
 from keras.src.ops.numpy import amax
 from keras.src.ops.numpy import amin
 from keras.src.ops.numpy import any
@@ -70,17 +69,17 @@
 from keras.src.ops.numpy import isfinite
 from keras.src.ops.numpy import isinf
 from keras.src.ops.numpy import isnan
 from keras.src.ops.numpy import less
 from keras.src.ops.numpy import less_equal
 from keras.src.ops.numpy import linspace
 from keras.src.ops.numpy import log
-from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import log1p
 from keras.src.ops.numpy import log2
+from keras.src.ops.numpy import log10
 from keras.src.ops.numpy import logaddexp
 from keras.src.ops.numpy import logical_and
 from keras.src.ops.numpy import logical_not
 from keras.src.ops.numpy import logical_or
 from keras.src.ops.numpy import logical_xor
 from keras.src.ops.numpy import logspace
 from keras.src.ops.numpy import matmul
@@ -109,14 +108,15 @@
 from keras.src.ops.numpy import ravel
 from keras.src.ops.numpy import real
 from keras.src.ops.numpy import reciprocal
 from keras.src.ops.numpy import repeat
 from keras.src.ops.numpy import reshape
 from keras.src.ops.numpy import roll
 from keras.src.ops.numpy import round
+from keras.src.ops.numpy import select
 from keras.src.ops.numpy import sign
 from keras.src.ops.numpy import sin
 from keras.src.ops.numpy import sinh
 from keras.src.ops.numpy import size
 from keras.src.ops.numpy import sort
 from keras.src.ops.numpy import split
 from keras.src.ops.numpy import sqrt
@@ -137,11 +137,12 @@
 from keras.src.ops.numpy import transpose
 from keras.src.ops.numpy import tri
 from keras.src.ops.numpy import tril
 from keras.src.ops.numpy import triu
 from keras.src.ops.numpy import true_divide
 from keras.src.ops.numpy import var
 from keras.src.ops.numpy import vdot
+from keras.src.ops.numpy import vectorize
 from keras.src.ops.numpy import vstack
 from keras.src.ops.numpy import where
 from keras.src.ops.numpy import zeros
 from keras.src.ops.numpy import zeros_like
```

### Comparing `keras-3.2.1/keras/optimizers/__init__.py` & `keras-3.3.0/keras/api/optimizers/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
-from keras.optimizers import legacy
-from keras.optimizers import schedules
+from keras.api.optimizers import legacy
+from keras.api.optimizers import schedules
 from keras.src.optimizers import deserialize
 from keras.src.optimizers import get
 from keras.src.optimizers import serialize
 from keras.src.optimizers.adadelta import Adadelta
 from keras.src.optimizers.adafactor import Adafactor
 from keras.src.optimizers.adagrad import Adagrad
 from keras.src.optimizers.adam import Adam
```

### Comparing `keras-3.2.1/keras/optimizers/legacy/__init__.py` & `keras-3.3.0/keras/api/optimizers/legacy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers import LegacyOptimizerWarning as Adagrad
 from keras.src.optimizers import LegacyOptimizerWarning as Adam
 from keras.src.optimizers import LegacyOptimizerWarning as Ftrl
 from keras.src.optimizers import LegacyOptimizerWarning as Optimizer
 from keras.src.optimizers import LegacyOptimizerWarning as RMSprop
 from keras.src.optimizers import LegacyOptimizerWarning as SGD
```

### Comparing `keras-3.2.1/keras/optimizers/schedules/__init__.py` & `keras-3.3.0/keras/api/optimizers/schedules/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecayRestarts
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import LearningRateSchedule
-from keras.src.optimizers.schedules.learning_rate_schedule import PiecewiseConstantDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    CosineDecayRestarts,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    LearningRateSchedule,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PiecewiseConstantDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import deserialize
 from keras.src.optimizers.schedules.learning_rate_schedule import serialize
```

### Comparing `keras-3.2.1/keras/random/__init__.py` & `keras-3.3.0/keras/api/random/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.random.random import beta
 from keras.src.random.random import binomial
 from keras.src.random.random import categorical
 from keras.src.random.random import dropout
 from keras.src.random.random import gamma
 from keras.src.random.random import normal
 from keras.src.random.random import randint
```

### Comparing `keras-3.2.1/keras/regularizers/__init__.py` & `keras-3.3.0/keras/api/regularizers/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.regularizers import deserialize
 from keras.src.regularizers import get
 from keras.src.regularizers import serialize
 from keras.src.regularizers.regularizers import L1
 from keras.src.regularizers.regularizers import L1 as l1
 from keras.src.regularizers.regularizers import L1L2
 from keras.src.regularizers.regularizers import L1L2 as l1_l2
 from keras.src.regularizers.regularizers import L2
 from keras.src.regularizers.regularizers import L2 as l2
 from keras.src.regularizers.regularizers import OrthogonalRegularizer
-from keras.src.regularizers.regularizers import OrthogonalRegularizer as orthogonal_regularizer
+from keras.src.regularizers.regularizers import (
+    OrthogonalRegularizer as orthogonal_regularizer,
+)
 from keras.src.regularizers.regularizers import Regularizer
```

### Comparing `keras-3.2.1/keras/saving/__init__.py` & `keras-3.3.0/keras/api/saving/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.saving_api import load_weights
 from keras.src.saving.saving_api import save_model
```

### Comparing `keras-3.2.1/keras/src/__init__.py` & `keras-3.3.0/keras/src/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 from keras.src.backend import KerasTensor
 from keras.src.layers import Input
 from keras.src.layers import Layer
 from keras.src.models import Functional
 from keras.src.models import Model
 from keras.src.models import Sequential
 from keras.src.version import __version__
-
```

### Comparing `keras-3.2.1/keras/src/activations/__init__.py` & `keras-3.3.0/keras/src/activations/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,8 +100,7 @@
     else:
         obj = identifier
     if callable(obj):
         return obj
     raise ValueError(
         f"Could not interpret activation function identifier: {identifier}"
     )
-
```

### Comparing `keras-3.2.1/keras/src/activations/activations.py` & `keras-3.3.0/keras/src/activations/activations.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,8 +454,7 @@
     is applied along.
 
     Args:
         x: Input tensor.
         axis: Integer, axis along which the softmax is applied.
     """
     return ops.log_softmax(x, axis=axis)
-
```

### Comparing `keras-3.2.1/keras/src/api_export.py` & `keras-3.3.0/keras/src/api_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
     class keras_export:
         def __init__(self, path):
             self.path = path
 
         def __call__(self, symbol):
             register_internal_serializable(self.path, symbol)
             return symbol
-
```

### Comparing `keras-3.2.1/keras/src/applications/convnext.py` & `keras-3.3.0/keras/src/applications/convnext.py`

 * *Files 0% similar despite different names*

```diff
@@ -751,8 +751,7 @@
 
 @keras_export("keras.applications.convnext.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/densenet.py` & `keras-3.3.0/keras/src/applications/densenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -480,8 +480,7 @@
 Returns:
     A Keras model instance.
 """
 
 setattr(DenseNet121, "__doc__", DenseNet121.__doc__ + DOC)
 setattr(DenseNet169, "__doc__", DenseNet169.__doc__ + DOC)
 setattr(DenseNet201, "__doc__", DenseNet201.__doc__ + DOC)
-
```

### Comparing `keras-3.2.1/keras/src/applications/efficientnet.py` & `keras-3.3.0/keras/src/applications/efficientnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -847,8 +847,7 @@
 
 @keras_export("keras.applications.efficientnet.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/efficientnet_v2.py` & `keras-3.3.0/keras/src/applications/efficientnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1338,8 +1338,7 @@
 
 @keras_export("keras.applications.efficientnet_v2.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/imagenet_utils.py` & `keras-3.3.0/keras/src/applications/imagenet_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -456,8 +456,7 @@
     }:
         raise ValueError(
             "Only `None` and `softmax` activations are allowed "
             "for the `classifier_activation` argument when using "
             "pretrained weights, with `include_top=True`; Received: "
             f"classifier_activation={classifier_activation}"
         )
-
```

### Comparing `keras-3.2.1/keras/src/applications/inception_resnet_v2.py` & `keras-3.3.0/keras/src/applications/inception_resnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/inception_v3.py` & `keras-3.3.0/keras/src/applications/inception_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,8 +434,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/mobilenet.py` & `keras-3.3.0/keras/src/applications/mobilenet.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,8 +425,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/mobilenet_v2.py` & `keras-3.3.0/keras/src/applications/mobilenet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,8 +494,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/mobilenet_v3.py` & `keras-3.3.0/keras/src/applications/mobilenet_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,8 +674,7 @@
 
 @keras_export("keras.applications.mobilenet_v3.decode_predictions")
 def decode_predictions(preds, top=5):
     return imagenet_utils.decode_predictions(preds, top=top)
 
 
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/nasnet.py` & `keras-3.3.0/keras/src/applications/nasnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -856,8 +856,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/resnet.py` & `keras-3.3.0/keras/src/applications/resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -576,8 +576,7 @@
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50, "__doc__", ResNet50.__doc__ + DOC)
 setattr(ResNet101, "__doc__", ResNet101.__doc__ + DOC)
 setattr(ResNet152, "__doc__", ResNet152.__doc__ + DOC)
-
```

### Comparing `keras-3.2.1/keras/src/applications/resnet_v2.py` & `keras-3.3.0/keras/src/applications/resnet_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,8 +195,7 @@
 Returns:
     A Model instance.
 """
 
 setattr(ResNet50V2, "__doc__", ResNet50V2.__doc__ + DOC)
 setattr(ResNet101V2, "__doc__", ResNet101V2.__doc__ + DOC)
 setattr(ResNet152V2, "__doc__", ResNet152V2.__doc__ + DOC)
-
```

### Comparing `keras-3.2.1/keras/src/applications/vgg16.py` & `keras-3.3.0/keras/src/applications/vgg16.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,8 +240,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_CAFFE,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/vgg19.py` & `keras-3.3.0/keras/src/applications/vgg19.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,8 +248,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_CAFFE,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/applications/xception.py` & `keras-3.3.0/keras/src/applications/xception.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,8 +347,7 @@
 
 preprocess_input.__doc__ = imagenet_utils.PREPROCESS_INPUT_DOC.format(
     mode="",
     ret=imagenet_utils.PREPROCESS_INPUT_RET_DOC_TF,
     error=imagenet_utils.PREPROCESS_INPUT_ERROR_DOC,
 )
 decode_predictions.__doc__ = imagenet_utils.decode_predictions.__doc__
-
```

### Comparing `keras-3.2.1/keras/src/backend/__init__.py` & `keras-3.3.0/keras/src/backend/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,7 @@
     distribution_lib = None
 elif backend() == "numpy":
     from keras.src.backend.numpy import *  # noqa: F403
 
     distribution_lib = None
 else:
     raise ValueError(f"Unable to import backend : {backend()}")
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/__init__.py` & `keras-3.3.0/keras/src/backend/common/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,8 +4,7 @@
 from keras.src.backend.common.variables import KerasVariable
 from keras.src.backend.common.variables import get_autocast_scope
 from keras.src.backend.common.variables import is_float_dtype
 from keras.src.backend.common.variables import is_int_dtype
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.common.variables import standardize_shape
 from keras.src.random import random
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/dtypes.py` & `keras-3.3.0/keras/src/backend/common/dtypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,8 +305,7 @@
             raise ValueError(
                 "There is no implicit conversions from float8 dtypes to others."
                 f" You must cast it internally. Received: {dtypes}"
             )
     return _lattice_result_type(
         *(config.floatx() if arg is None else arg for arg in dtypes),
     )
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/global_state.py` & `keras-3.3.0/keras/src/backend/common/global_state.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,25 +18,33 @@
         attr = default
         if set_to_default:
             set_global_attribute(name, attr)
     return attr
 
 
 @keras_export(["keras.utils.clear_session", "keras.backend.clear_session"])
-def clear_session():
+def clear_session(free_memory=True):
     """Resets all state generated by Keras.
 
     Keras manages a global state, which it uses to implement the Functional
     model-building API and to uniquify autogenerated layer names.
 
     If you are creating many models in a loop, this global state will consume
     an increasing amount of memory over time, and you may want to clear it.
     Calling `clear_session()` releases the global state: this helps avoid
     clutter from old models and layers, especially when memory is limited.
 
+    Args:
+        free_memory: Whether to call Python garbage collection.
+            It's usually a good practice to call it to make sure
+            memory used by deleted objects is immediately freed.
+            However, it may take a few seconds to execute, so
+            when using `clear_session()` in a short loop,
+            you may want to skip it.
+
     Example 1: calling `clear_session()` when creating models in a loop
 
     ```python
     for _ in range(100):
       # Without `clear_session()`, each iteration of this loop will
       # slightly increase the size of the global state managed by Keras
       model = keras.Sequential([
@@ -81,10 +89,10 @@
     elif backend.backend() == "torch":
         import torch._dynamo as dynamo
 
         # reset's torchdynamo's cache so that  cached guards, compiled fn, etc
         # do not persist between clear_session() calls
         dynamo.reset()
 
-    # Manually trigger garbage collection.
-    gc.collect()
-
+    if free_memory:
+        # Manually trigger garbage collection.
+        gc.collect()
```

### Comparing `keras-3.2.1/keras/src/backend/common/keras_tensor.py` & `keras-3.3.0/keras/src/backend/common/keras_tensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export("keras.KerasTensor")
 class KerasTensor:
     """Symbolic tensor -- encapsulates a shape and a dtype.
 
@@ -307,8 +307,7 @@
     that was created via `Input()`. A "symbolic tensor"
     can be understood as a placeholder -- it does not
     contain any actual numerical data, only a shape and dtype.
     It can be used for building Functional models, but it
     cannot be used in actual computations.
     """
     return isinstance(x, KerasTensor)
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/name_scope.py` & `keras-3.3.0/keras/src/backend/common/name_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
         return ""
     parts = []
     for entry in name_scope_stack:
         if entry.override_parent is not None:
             parts = [p for p in entry.override_parent.split("/") if p]
         parts.append(entry.name)
     return "/".join(parts)
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/stateless_scope.py` & `keras-3.3.0/keras/src/backend/common/stateless_scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,19 +86,20 @@
         global_state.set_global_attribute(
             "stateless_scope", self.original_scope
         )
         if self.original_scope is None and self.initialize_variables:
             # We're back in eager scope;
             # if any variables were created within the stateless
             # scope, we initialize them here.
-            from keras.src.backend.common.variables import initialize_all_variables
+            from keras.src.backend.common.variables import (
+                initialize_all_variables,
+            )
 
             initialize_all_variables()
 
 
 def in_stateless_scope():
     return global_state.get_global_attribute("stateless_scope") is not None
 
 
 def get_stateless_scope():
     return global_state.get_global_attribute("stateless_scope")
-
```

### Comparing `keras-3.2.1/keras/src/backend/common/variables.py` & `keras-3.3.0/keras/src/backend/common/variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
     initial_array = np.ones((3, 3))
     variable_from_array = keras.Variable(initializer=initial_array)
     ```
 
     **Using a Keras initializer to create a `Variable`:**
 
     ```python
-    from keras.initializers import Ones
+    from keras.src.initializers import Ones
     variable_from_initializer = keras.Variable(
         initializer=Ones(), shape=(3, 3), dtype="float32"
     )
     ```
 
     **Updating the value of a `Variable`:**
 
@@ -111,14 +111,18 @@
         self._shape = None
         self._initializer = None
         self._regularizer = None
         self._constraint = None
         self._trainable = trainable
         self._autocast = autocast
         self._aggregation = aggregation
+        # `self._overwrite_with_gradient` is an internal property to determine
+        # whether this variable should be overwritten by the computed gradient.
+        # Ref: https://github.com/google/flax/blob/main/flax/linen/fp8_ops.py
+        self._overwrite_with_gradient = False
         if isinstance(initializer, str):
             from keras.src import initializers
 
             initializer = initializers.get(initializer)
         if callable(initializer):
             if shape is None:
                 raise ValueError(
@@ -263,14 +267,36 @@
         return self._trainable
 
     @trainable.setter
     def trainable(self, value):
         self._trainable = value
 
     @property
+    def overwrite_with_gradient(self):
+        """Whether this variable should be overwritten by the gradient.
+
+        This property is designed for a special case where we want to overwrite
+        the variable directly with its computed gradient. For example, in float8
+        training, new `scale` and `amax_history` are computed as gradients, and
+        we want to overwrite them directly instead of following the typical
+        procedure such as gradient descent with a learning rate, gradient
+        clipping and weight decaying.
+        """
+        return self._overwrite_with_gradient
+
+    @overwrite_with_gradient.setter
+    def overwrite_with_gradient(self, value):
+        if not isinstance(value, bool):
+            raise TypeError(
+                "`overwrite_with_gradient` must be a boolean. "
+                f"Received: {value}"
+            )
+        self._overwrite_with_gradient = value
+
+    @property
     def regularizer(self):
         return self._regularizer
 
     @regularizer.setter
     def regularizer(self, value):
         from keras.src.regularizers import Regularizer
 
@@ -587,8 +613,7 @@
 
     def __enter__(self):
         self.original_scope = get_autocast_scope()
         global_state.set_global_attribute("autocast_scope", self)
 
     def __exit__(self, *args, **kwargs):
         global_state.set_global_attribute("autocast_scope", self.original_scope)
-
```

### Comparing `keras-3.2.1/keras/src/backend/config.py` & `keras-3.3.0/keras/src/backend/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -270,8 +270,7 @@
     Example:
 
     >>> keras.config.backend()
     'tensorflow'
 
     """
     return _BACKEND
-
```

### Comparing `keras-3.2.1/keras/src/backend/exports.py` & `keras-3.3.0/keras/src/backend/exports.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,8 +28,7 @@
 class name_scope(backend_name_scope):
     pass
 
 
 @keras_export("keras.device")
 def device(device_name):
     return backend.device_scope(device_name)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/__init__.py` & `keras-3.3.0/keras/src/backend/jax/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,7 @@
 from keras.src.backend.jax.core import shape
 from keras.src.backend.jax.core import stop_gradient
 from keras.src.backend.jax.core import vectorized_map
 from keras.src.backend.jax.rnn import cudnn_ok
 from keras.src.backend.jax.rnn import gru
 from keras.src.backend.jax.rnn import lstm
 from keras.src.backend.jax.rnn import rnn
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/core.py` & `keras-3.3.0/keras/src/backend/jax/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import jax
 import jax.experimental.sparse as jax_sparse
 import jax.numpy as jnp
 import ml_dtypes
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.jax import distribution_lib
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = True
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         value = jnp.array(value, dtype=self._dtype)
@@ -363,8 +363,7 @@
             "Invalid value for argument `device_name`. "
             "Expected a string like 'gpu:0' or a `jax.Device` instance. "
             f"Received: device_name='{device_name}'"
         )
     else:
         jax_device = device_name
     return jax.default_device(jax_device)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/distribution_lib.py` & `keras-3.3.0/keras/src/backend/jax/distribution_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,8 +260,7 @@
         raise ValueError(
             "Cannot create sharding when device mesh is not set "
             "for TensorLayout."
         )
     partition_spec = jax.sharding.PartitionSpec(*tensor_layout.axes)
     jax_mesh = _to_jax_mesh(tensor_layout.device_mesh)
     return jax.sharding.NamedSharding(jax_mesh, partition_spec)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/linalg.py` & `keras-3.3.0/keras/src/backend/jax/linalg.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,18 @@
     return jnp.linalg.det(a)
 
 
 def eig(x):
     return jnp.linalg.eig(x)
 
 
+def eigh(x):
+    return jnp.linalg.eigh(x)
+
+
 def inv(a):
     return jnp.linalg.inv(a)
 
 
 def lu_factor(x):
     lu_factor_fn = jsp.linalg.lu_factor
     if x.ndim > 2:
@@ -66,8 +70,7 @@
 
 def solve_triangular(a, b, lower=False):
     return jsp.linalg.solve_triangular(a, b, lower=lower)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return jnp.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/math.py` & `keras-3.3.0/keras/src/backend/jax/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,8 +271,7 @@
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return jnp.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/nn.py` & `keras-3.3.0/keras/src/backend/numpy/nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,102 +1,134 @@
 import jax
-import jax.experimental.sparse as jax_sparse
-import jax.numpy as jnp
 import numpy as np
 from jax import lax
-from jax import nn as jnn
+from jax import numpy as jnp
 
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
     compute_conv_transpose_padding_args_for_jax,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.jax.core import cast
-from keras.src.backend.jax.core import convert_to_tensor
+from keras.src.backend.numpy.core import cast
+from keras.src.backend.numpy.core import convert_to_tensor
+from keras.src.backend.numpy.core import is_tensor
+from keras.src.utils.module_utils import scipy
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return jnn.relu(x)
+    return np.maximum(x, np.array(0.0, x.dtype))
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    return jnn.relu6(x)
+    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
+    # np.minimum and np.maximum here
+    return np.minimum(
+        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
+    )
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return jnn.sigmoid(x)
+    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
 
 
 def tanh(x):
-    x = convert_to_tensor(x)
-    return jnn.tanh(x)
+    return np.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return jnn.softplus(x)
+    return np.logaddexp(x, np.array(0.0, x.dtype))
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return jnn.soft_sign(x)
+    return x / (np.array(1.0, x.dtype) + np.abs(x))
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return jnn.silu(x)
+    return x * sigmoid(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return jnn.log_sigmoid(x)
+    return -softplus(-x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return jnn.leaky_relu(x, negative_slope=negative_slope)
+    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
 
 
 def hard_sigmoid(x):
-    x = convert_to_tensor(x)
-    return jnn.hard_sigmoid(x)
+    # python numbers will be promoted to float64 by np, so it's necessary to
+    # first convert the python numbers to np scalars
+    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
+    return np.where(
+        x <= 0.0,
+        np.array(0.0, x.dtype),
+        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
+    )
 
 
 def hard_silu(x):
-    x = convert_to_tensor(x)
-    return jnn.hard_silu(x)
+    return x * hard_sigmoid(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return jnn.elu(x, alpha=alpha)
+    return np.where(
+        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
+    )
 
 
-def selu(x):
+def selu(
+    x,
+    alpha=1.6732632423543772848170429916717,
+    scale=1.0507009873554804934193349852946,
+):
     x = convert_to_tensor(x)
-    return jnn.selu(x)
+    return np.array(scale, x.dtype) * elu(x, alpha)
 
 
 def gelu(x, approximate=True):
     x = convert_to_tensor(x)
-    return jnn.gelu(x, approximate)
+    # followed by JAX's implementation
+    if approximate:
+        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
+        cdf = np.array(0.5, x.dtype) * (
+            np.array(1.0, x.dtype)
+            + np.tanh(
+                sqrt_2_over_pi
+                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
+            )
+        )
+        return x * cdf
+    else:
+        sqrt_2 = np.sqrt(2).astype(x.dtype)
+        return (
+            x
+            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
+            / np.array(2, x.dtype)
+        )
 
 
-def softmax(x, axis=-1):
-    x = convert_to_tensor(x)
-    return jnn.softmax(x, axis=axis)
+def softmax(x, axis=None):
+    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
+    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
 
 
-def log_softmax(x, axis=-1):
-    x = convert_to_tensor(x)
-    return jnn.log_softmax(x, axis=axis)
+def log_softmax(x, axis=None):
+    max_x = np.max(x, axis=axis, keepdims=True)
+    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
+    return x - max_x - logsumexp
 
 
 def _convert_to_spatial_operand(
     x,
     num_spatial_dims,
     data_format="channels_last",
     include_batch_and_channels=True,
@@ -136,21 +168,23 @@
         The output of the reduction for each window slice.
     """
     if padding not in ("same", "valid"):
         raise ValueError(
             f"Invalid padding '{padding}', must be 'same' or 'valid'."
         )
     padding = padding.upper()
-    return lax.reduce_window(
-        inputs,
-        initial_value,
-        reduce_fn,
-        pool_size,
-        strides,
-        padding,
+    return np.array(
+        lax.reduce_window(
+            inputs,
+            initial_value,
+            reduce_fn,
+            pool_size,
+            strides,
+            padding,
+        )
     )
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
@@ -269,22 +303,24 @@
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
             f"kernel's in_channels. Received input channels {channels} and "
             f"kernel in_channels {kernel_in_channels}. "
         )
     feature_group_count = channels // kernel_in_channels
-    return jax.lax.conv_general_dilated(
-        convert_to_tensor(inputs),
-        convert_to_tensor(kernel),
-        strides,
-        padding,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        feature_group_count=feature_group_count,
+    return np.array(
+        jax.lax.conv_general_dilated(
+            inputs,
+            kernel if is_tensor(kernel) else kernel.numpy(),
+            strides,
+            padding,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            feature_group_count=feature_group_count,
+        )
     )
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
@@ -311,25 +347,27 @@
         data_format,
         include_batch_and_channels=False,
     )
     feature_group_count = (
         inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
     )
     kernel = jnp.reshape(
-        kernel,
+        kernel if is_tensor(kernel) else kernel.numpy(),
         kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
     )
-    return jax.lax.conv_general_dilated(
-        inputs,
-        kernel,
-        strides,
-        padding,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        feature_group_count=feature_group_count,
+    return np.array(
+        jax.lax.conv_general_dilated(
+            inputs,
+            kernel,
+            strides,
+            padding,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            feature_group_count=feature_group_count,
+        )
     )
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
@@ -390,79 +428,72 @@
     dilation_rate = _convert_to_spatial_operand(
         dilation_rate,
         num_spatial_dims,
         data_format,
         include_batch_and_channels=False,
     )
 
-    return jax.lax.conv_transpose(
-        inputs,
-        kernel,
-        strides,
-        padding=padding_values,
-        rhs_dilation=dilation_rate,
-        dimension_numbers=dimension_numbers,
-        transpose_kernel=True,
+    return np.array(
+        jax.lax.conv_transpose(
+            inputs,
+            kernel if is_tensor(kernel) else kernel.numpy(),
+            strides,
+            padding=padding_values,
+            rhs_dilation=dilation_rate,
+            dimension_numbers=dimension_numbers,
+            transpose_kernel=True,
+        )
     )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    x = convert_to_tensor(x)
     if sparse:
-        if axis < 0:
-            axis = axis + len(x.shape) + 1
-        if dtype is None:
-            dtype = "float32"
-        # We deal with negative inputs by having zeros in the output although
-        # it's useless. It makes shapes static.
-        values = jnp.greater_equal(jnp.ravel(x), 0).astype(dtype)
-        values_count = values.shape[0]
-        indices = [jnp.arange(dim) for dim in x.shape]
-        indices = jnp.meshgrid(*indices, indexing="ij")
-        indices.insert(axis, jnp.maximum(x, 0))  # Deal with negative indices
-        indices = [a.reshape(values_count, 1).astype("int32") for a in indices]
-        indices = jnp.concatenate(indices, axis=1)
-        shape = list(x.shape)
-        shape.insert(axis, num_classes)
-        shape = tuple(shape)
-        return jax_sparse.BCOO(
-            (values, indices),
-            shape=shape,
-            indices_sorted=True,
-            unique_indices=True,
-        )
-    return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
+    x = convert_to_tensor(x)
+    input_shape = x.shape
+
+    # Shrink the last dimension if the shape is (..., 1).
+    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
+        input_shape = tuple(input_shape[:-1])
+
+    x = x.reshape(-1)
+    if not num_classes:
+        num_classes = np.max(x) + 1
+
+    batch_size = x.shape[0]
+    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
+    valid_indices = x >= 0
+    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
+
+    # First, reshape the array with the extra dimension at the end
+    output_shape = input_shape + (num_classes,)
+    categorical = np.reshape(categorical, output_shape)
+
+    # Then, move this new dimension to the right place (according to axis)
+    if axis != -1:
+        categorical = np.moveaxis(categorical, -1, axis)
+
+    return categorical
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    if sparse:
+        raise ValueError("Unsupported value `sparse=True` with numpy backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    if sparse:
-        result = one_hot(
-            x, num_classes, axis=axis, dtype="int32", sparse=sparse
-        )
-        # JAX's BCOO does not support max reduction, use sum and compare with 0.
-        result = jax_sparse.bcoo_reduce_sum(result, axes=(reduction_axis,))
-        result = jax_sparse.bcoo_sum_duplicates(result)
-        values = jnp.greater_equal(result.data, 0).astype(dtype)
-        return jax_sparse.BCOO(
-            (values, result.indices),
-            shape=result.shape,
-            indices_sorted=True,
-            unique_indices=True,
-        )
-    return jnp.max(
+    outputs = np.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
         axis=reduction_axis,
     )
+    return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = jnp.array(target)
-    output = jnp.array(output)
+    target = np.array(target)
+    output = np.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -470,193 +501,131 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = jax.nn.log_softmax(output, axis=axis)
+        log_prob = log_softmax(output, axis=axis)
     else:
-        output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = jnp.log(output)
-    return -jnp.sum(target * log_prob, axis=axis)
+        output = output / np.sum(output, axis, keepdims=True)
+        output = np.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = np.log(output)
+    return -np.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = jnp.array(target, dtype="int32")
-    output = jnp.array(output)
+    target = np.array(target, dtype="int32")
+    output = np.array(output)
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = jnp.squeeze(target, axis=-1)
+        target = np.squeeze(target, axis=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = jax.nn.log_softmax(output, axis=axis)
+        log_prob = log_softmax(output, axis=axis)
     else:
-        output = output / jnp.sum(output, axis, keepdims=True)
-        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = jnp.log(output)
-    target = jnn.one_hot(target, output.shape[axis], axis=axis)
-    return -jnp.sum(target * log_prob, axis=axis)
+        output = output / np.sum(output, axis, keepdims=True)
+        output = np.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = np.log(output)
+    target = one_hot(target, output.shape[axis], axis=axis)
+    return -np.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = jnp.array(target)
-    output = jnp.array(output)
+    target = np.array(target)
+    output = np.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_logits = jax.nn.log_sigmoid(output)
-        log_neg_logits = jax.nn.log_sigmoid(-output)
-        return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
-
-    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * jnp.log(output)
-    bce += (1.0 - target) * jnp.log(1.0 - output)
+        output = sigmoid(output)
+
+    output = np.clip(output, epsilon(), 1.0 - epsilon())
+    bce = target * np.log(output)
+    bce += (1.0 - target) * np.log(1.0 - output)
     return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with JAX."
+            "Argument synchronized=True is not supported with NumPy."
         )
+    axes = tuple(axes) if isinstance(axes, list) else axes
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype in ("float16", "bfloat16"):
+    if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
-    mean = jnp.mean(x, axes, keepdims=True)
-    variance = jnp.var(x, axis=axes, keepdims=True)
+    mean = np.mean(x, axes, keepdims=True)
+
+    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
+    # but less numerically stable.
+    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
 
     if not keepdims:
-        mean = jnp.squeeze(mean, axes)
-        variance = jnp.squeeze(variance, axes)
+        mean = np.squeeze(mean, axes)
+        variance = np.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = jnp.clip(
-            mean, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
-        )
-        variance = jnp.clip(
-            variance, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
+        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
+        variance = np.clip(
+            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = jnp.reshape(mean, shape)
-    variance = jnp.reshape(variance, shape)
+    mean = np.reshape(mean, shape)
+    variance = np.reshape(variance, shape)
 
-    inv = jax.lax.rsqrt(variance + epsilon)
+    inv = 1.0 / np.sqrt(variance + epsilon)
     if scale is not None:
-        scale = jnp.reshape(scale, shape)
+        scale = np.reshape(scale, shape)
         inv = inv * scale
 
     res = -mean * inv
     if offset is not None:
-        offset = jnp.reshape(offset, shape)
+        offset = np.reshape(offset, shape)
         res = res + offset
 
     return x * inv + res
 
 
-def ctc_loss(
-    target,
-    output,
-    target_length,
-    output_length,
-    mask_index=0,
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
 ):
-    batch_size, _, _ = output.shape
-    batch_size, max_target_length = target.shape
-
-    output = output.transpose((1, 0, 2))
-    target = target.transpose((1, 0)).astype("int32")
-
-    logits = jnn.log_softmax(output)
-    mgrid_t, mgrid_b = jnp.meshgrid(
-        jnp.arange(max_target_length), jnp.arange(batch_size)
-    )
-    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
-    logprobs_mask = logits[:, :, mask_index]
-
-    logit_paddings = jnp.array(
-        jnp.arange(max_target_length) < output_length[:, None],
-        dtype=jnp.float32,
+    raise NotImplementedError(
+        "NumPy backend does not yet support CTC decoding."
     )
-
-    repeat = jnp.array(target[1:] == target[:-1])
-    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
-
-    _logepsilon = -100000.0
-
-    def _iterate(prev, x):
-        prev_mask, prev_emit = prev
-        logprob_mask, logprob_emit, pad = x
-
-        prev_mask_orig = prev_mask
-        prev_mask = prev_mask.at[:, 1:].set(
-            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
-        )
-        emit = jnp.logaddexp(
-            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
-        )
-
-        mask = prev_mask + logprob_mask[:, None]
-        mask = mask.at[:, 1:].set(
-            jnp.logaddexp(
-                mask[:, 1:],
-                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
-            )
-        )
-
-        pad = pad[:, None]
-        emit = emit * pad + prev_emit * (1 - pad)
-        mask = mask * pad + prev_mask_orig * (1 - pad)
-
-        return (mask, emit), (mask, emit)
-
-    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
-    mask_init = mask_init.at[:, 0].set(0.0)
-    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
-
-    _, (alphas_mask, alphas_emit) = lax.scan(
-        _iterate,
-        (mask_init, emit_init),
-        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
-    )
-
-    last_alpha_mask = (
-        alphas_mask[-1]
-        .at[:, 1:]
-        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
-    )
-
-    return -last_alpha_mask[jnp.arange(batch_size), target_length]
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/numpy.py` & `keras-3.3.0/keras/src/backend/jax/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,26 +19,35 @@
 def add(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.add(x1, x2)
 
 
 def bincount(x, weights=None, minlength=0, sparse=False):
-    if sparse:
+    # Note: bincount is never tracable / jittable because the output shape
+    # depends on the values in x.
+    if sparse or isinstance(x, jax_sparse.BCOO):
+        if isinstance(x, jax_sparse.BCOO):
+            if weights is not None:
+                if not isinstance(weights, jax_sparse.BCOO):
+                    raise ValueError("`x` and `weights` must both be BCOOs")
+                if x.indices is not weights.indices:
+                    # This test works in eager mode only
+                    if not jnp.all(jnp.equal(x.indices, weights.indices)):
+                        raise ValueError(
+                            "`x` and `weights` BCOOs must have the same indices"
+                        )
+                weights = weights.data
+            x = x.data
         reduction_axis = 1 if len(x.shape) > 1 else 0
         maxlength = jnp.maximum(jnp.max(x) + 1, minlength)
-        one_hot_encoding = nn.one_hot(x, maxlength, sparse=sparse)
+        one_hot_encoding = nn.one_hot(x, maxlength, sparse=True)
         if weights is not None:
-            split_weights = split(
-                weights,
-                weights.shape[reduction_axis],
-                reduction_axis,
-            )
-            stacked_weights = stack(split_weights, axis=reduction_axis)
-            one_hot_encoding = one_hot_encoding * stacked_weights
+            expanded_weights = jnp.expand_dims(weights, reduction_axis + 1)
+            one_hot_encoding = one_hot_encoding * expanded_weights
 
         outputs = jax_sparse.bcoo_reduce_sum(
             one_hot_encoding,
             axes=(reduction_axis,),
         )
         return outputs
     if len(x.shape) == 2:
@@ -210,18 +219,16 @@
 
 @sparse.elementwise_unary(linear=False)
 def absolute(x):
     x = convert_to_tensor(x)
     return jnp.absolute(x)
 
 
-@sparse.elementwise_unary(linear=False)
 def abs(x):
-    x = convert_to_tensor(x)
-    return jnp.absolute(x)
+    return absolute(x)
 
 
 def all(x, axis=None, keepdims=False):
     return jnp.all(x, axis=axis, keepdims=keepdims)
 
 
 def any(x, axis=None, keepdims=False):
@@ -326,20 +333,20 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return jnp.arctanh(x)
 
 
-def argmax(x, axis=None):
-    return jnp.argmax(x, axis=axis)
+def argmax(x, axis=None, keepdims=False):
+    return jnp.argmax(x, axis=axis, keepdims=keepdims)
 
 
-def argmin(x, axis=None):
-    return jnp.argmin(x, axis=axis)
+def argmin(x, axis=None, keepdims=False):
+    return jnp.argmin(x, axis=axis, keepdims=keepdims)
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
     if x.ndim == 0:
         return jnp.argsort(x, axis=None)
     return jnp.argsort(x, axis=axis)
@@ -481,14 +488,15 @@
 
 
 def diff(a, n=1, axis=-1):
     a = convert_to_tensor(a)
     return jnp.diff(a, n=n, axis=axis)
 
 
+@sparse.elementwise_unary(linear=False)
 def digitize(x, bins):
     x = convert_to_tensor(x)
     bins = convert_to_tensor(bins)
     return jnp.digitize(x, bins)
 
 
 def dot(x, y):
@@ -756,17 +764,17 @@
     return jnp.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
     return jnp.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
-    return jnp.nan_to_num(x)
+    return jnp.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     return jnp.ndim(x)
 
 
 def nonzero(x):
@@ -960,15 +968,26 @@
     x2 = convert_to_tensor(x2)
     return jnp.tensordot(x1, x2, axes=axes)
 
 
 @sparse.elementwise_unary(linear=False)
 def round(x, decimals=0):
     x = convert_to_tensor(x)
-    return jnp.round(x, decimals=decimals)
+
+    # jnp.round doesn't support decimals < 0 for integers
+    x_dtype = standardize_dtype(x.dtype)
+    if "int" in x_dtype and decimals < 0:
+        factor = cast(math.pow(10, decimals), config.floatx())
+        x = cast(x, config.floatx())
+        x = jnp.multiply(x, factor)
+        x = jnp.round(x)
+        x = jnp.divide(x, factor)
+        return cast(x, x_dtype)
+    else:
+        return jnp.round(x, decimals=decimals)
 
 
 def tile(x, repeats):
     return jnp.tile(x, repeats)
 
 
 def trace(x, offset=0, axis1=0, axis2=1):
@@ -1000,14 +1019,20 @@
     return jnp.vdot(x1, x2)
 
 
 def vstack(xs):
     return jnp.vstack(xs)
 
 
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    if excluded is None:
+        excluded = set()
+    return jnp.vectorize(pyfunc, excluded=excluded, signature=signature)
+
+
 def where(condition, x1, x2):
     return jnp.where(condition, x1, x2)
 
 
 @sparse.elementwise_division
 def divide(x1, x2):
     x1 = convert_to_tensor(x1)
@@ -1130,7 +1155,10 @@
 
 
 def correlate(x1, x2, mode="valid"):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.correlate(x1, x2, mode)
 
+
+def select(condlist, choicelist, default=0):
+    return jnp.select(condlist, choicelist, default=default)
```

### Comparing `keras-3.2.1/keras/src/backend/jax/optimizer.py` & `keras-3.3.0/keras/src/backend/jax/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,31 +21,32 @@
             steps = self.gradient_accumulation_steps
 
             current_trainable_vars_value = [
                 v.value for v in trainable_variables
             ]
             current_optimizer_vars_value = [v.value for v in self.variables]
 
+            # `trainable_variables` might have been filtered in previous
+            # processing steps, so we need to ensure the correct mapping between
+            # `self._accumulated_gradients` and `trainable_variables`
+            acc_grads = [
+                self._accumulated_gradients[self._get_variable_index(v)]
+                for v in trainable_variables
+            ]
+
             new_g_accs = jax.lax.cond(
                 is_update_step,
-                lambda: [
-                    jnp.zeros(x.shape, dtype=x.dtype)
-                    for x in self._accumulated_gradients
-                ],
-                lambda: [
-                    grads[i] + self._accumulated_gradients[i]
-                    for i in range(len(grads))
-                ],
+                lambda: [jnp.zeros(g.shape, dtype=g.dtype) for g in acc_grads],
+                lambda: [g + acc_g for g, acc_g in zip(grads, acc_grads)],
             )
 
             grads = jax.lax.cond(
                 is_update_step,
                 lambda: [
-                    (grads[i] + self._accumulated_gradients[i]) / steps
-                    for i in range(len(grads))
+                    (g + acc_g) / steps for g, acc_g in zip(grads, acc_grads)
                 ],
                 lambda: list(grads),
             )
 
             self._backend_update_step(
                 grads, trainable_variables, self.learning_rate
             )
@@ -62,15 +63,15 @@
 
             for value, v in zip(new_trainable_vars, trainable_variables):
                 v.assign(value)
 
             for value, v in zip(new_opt_vars, self.variables):
                 v.assign(value)
 
-            for n_g_acc, g_acc in zip(new_g_accs, self._accumulated_gradients):
+            for n_g_acc, g_acc in zip(new_g_accs, acc_grads):
                 g_acc.assign(n_g_acc)
 
         else:
             self._backend_update_step(
                 grads, trainable_variables, self.learning_rate
             )
 
@@ -97,8 +98,7 @@
                 ):
                     var.assign(
                         average_var * should_overwrite_model_vars_int
                         + var.value * should_not_overwrite_model_vars_int
                     )
 
         self.iterations.assign_add(1)
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/random.py` & `keras-3.3.0/keras/src/backend/jax/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,8 +110,7 @@
     # jax doesn't accept python lists as arguments
     alpha = jax.numpy.array(alpha)
     beta = jax.numpy.array(beta)
     sample = jax.random.beta(
         key=seed, a=alpha, b=beta, shape=shape, dtype=dtype
     )
     return sample
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/rnn.py` & `keras-3.3.0/keras/src/backend/jax/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import contextlib
 
 from jax import lax
 from jax import numpy as jnp
 
+from keras.src import tree
 from keras.src.backend.common import stateless_scope
-from keras.src.utils import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -220,8 +220,7 @@
 
 
 def unstack(x, axis=0):
     return [
         lax.index_in_dim(x, i, axis, keepdims=False)
         for i in range(x.shape[axis])
     ]
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/sparse.py` & `keras-3.3.0/keras/src/backend/jax/sparse.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,8 +322,7 @@
                 raise ValueError(f"Unsupported sparse format: {x1.__class__}")
         elif isinstance(x2, jax_sparse.JAXSparse):
             # x1 is dense, x2 is sparse, densify x2
             x2 = x2.todense()
         return func(x1, x2)
 
     return sparse_wrapper
-
```

### Comparing `keras-3.2.1/keras/src/backend/jax/trainer.py` & `keras-3.3.0/keras/src/backend/jax/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import jax
 import numpy as np
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.backend import distribution_lib as jax_distribution_lib
 from keras.src.distribution import distribution_lib
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class JAXTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
@@ -433,29 +433,30 @@
                     "trainable_variables": trainable_variables,
                     "non_trainable_variables": non_trainable_variables,
                     "optimizer_variables": optimizer_variables,
                     "metrics_variables": metrics_variables,
                 }
 
                 # Callbacks
-                callbacks.on_train_batch_end(step, self._pythonify_logs(logs))
+                logs = self._pythonify_logs(logs)
+                callbacks.on_train_batch_end(step, logs)
                 if self.stop_training:
                     break
 
             # Reattach state to the model (if not already done by a callback).
             # NOTE: doing this after each step would be a big performance
             # bottleneck.
             self.jax_state_sync()
 
-            # Override with model metrics instead of last step logs
+            # Override with model metrics instead of last step logs if needed.
             # The jax spmd_mode is need for multi-process context, since the
             # metrics values are replicated, and we don't want to do a all
             # gather, and only need the local copy of the value.
             with jax.spmd_mode("allow_all"):
-                epoch_logs = self.get_metrics_result()
+                epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
             ):
                 # Create JAXEpochIterator for evaluation and cache it.
                 if getattr(self, "_eval_epoch_iterator", None) is None:
@@ -581,26 +582,27 @@
             self._jax_state = {
                 # I wouldn't recommend modifying non-trainable model state
                 # during evaluate(), but it's allowed.
                 "trainable_variables": trainable_variables,
                 "non_trainable_variables": non_trainable_variables,
                 "metrics_variables": metrics_variables,
             }
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
 
         # Reattach state back to model (if not already done by a callback).
         self.jax_state_sync()
 
         # The jax spmd_mode is need for multi-process context, since the
         # metrics values are replicated, and we don't want to do a all
         # gather, and only need the local copy of the value.
         with jax.spmd_mode("allow_all"):
-            logs = self.get_metrics_result()
+            logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
         self._jax_state = None
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
@@ -1003,8 +1005,7 @@
             for data in itertools.islice(numpy_iterator, n):
                 queue.append(_distribute_data(data))
 
         enqueue(n=2)  # TODO: should we make `n` configurable?
         while queue:
             yield queue.popleft()
             enqueue(1)
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/__init__.py` & `keras-3.3.0/keras/src/backend/numpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 from keras.src.backend.numpy.core import is_tensor
 from keras.src.backend.numpy.core import shape
 from keras.src.backend.numpy.core import vectorized_map
 from keras.src.backend.numpy.rnn import cudnn_ok
 from keras.src.backend.numpy.rnn import gru
 from keras.src.backend.numpy.rnn import lstm
 from keras.src.backend.numpy.rnn import rnn
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/core.py` & `keras-3.3.0/keras/src/backend/numpy/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = False
 
 
 class Variable(KerasVariable):
     def _initialize(self, value):
         self._value = np.array(value, dtype=self._dtype)
@@ -230,8 +230,7 @@
     return [x[i] for i in range(x.shape[0])]
 
 
 def custom_gradient(fun):
     raise NotImplementedError(
         "`custom_gradient` is not supported with numpy backend"
     )
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/linalg.py` & `keras-3.3.0/keras/src/backend/numpy/linalg.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,18 @@
     return np.linalg.det(a)
 
 
 def eig(a):
     return np.linalg.eig(a)
 
 
+def eigh(a):
+    return np.linalg.eigh(a)
+
+
 def inv(a):
     return np.linalg.inv(a)
 
 
 def lu_factor(a):
     if a.ndim == 2:
         return sl.lu_factor(a)
@@ -72,8 +76,7 @@
         b = np.expand_dims(b, axis=-1)
         return _vectorized_solve_triangular(a, b).squeeze(axis=-1)
     return _vectorized_solve_triangular(a, b)
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     return np.linalg.svd(x, full_matrices=full_matrices, compute_uv=compute_uv)
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/math.py` & `keras-3.3.0/keras/src/backend/numpy/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -323,8 +323,7 @@
     x = convert_to_tensor(x)
     dtype = standardize_dtype(x.dtype)
     if "int" in dtype or dtype == "bool":
         dtype = dtypes.result_type(x.dtype, "float32")
     return np.linalg.norm(x, ord=ord, axis=axis, keepdims=keepdims).astype(
         dtype
     )
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/nn.py` & `keras-3.3.0/keras/src/backend/torch/nn.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,386 +1,471 @@
-import jax
-import numpy as np
-from jax import lax
-from jax import numpy as jnp
+import torch
+import torch.nn.functional as tnn
 
+from keras.src import tree
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_jax,
+    compute_conv_transpose_padding_args_for_torch,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.numpy.core import cast
-from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.backend.numpy.core import is_tensor
-from keras.src.utils.module_utils import scipy
+from keras.src.backend.torch.core import cast
+from keras.src.backend.torch.core import convert_to_tensor
+from keras.src.backend.torch.core import get_device
+from keras.src.backend.torch.numpy import expand_dims
+from keras.src.backend.torch.numpy import maximum
+from keras.src.backend.torch.numpy import where
+from keras.src.utils.argument_validation import standardize_tuple
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return np.maximum(x, np.array(0.0, x.dtype))
+    return tnn.relu(x)
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    # np.clip incorrectly promote bfloat16 to float32, so we replace it with
-    # np.minimum and np.maximum here
-    return np.minimum(
-        np.maximum(x, np.array(0.0, x.dtype)), np.array(6.0, x.dtype)
-    )
+    return tnn.relu6(x)
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return np.array(1.0, x.dtype) / (np.array(1.0, x.dtype) + np.exp(-x))
+    return tnn.sigmoid(x)
 
 
 def tanh(x):
-    return np.tanh(x)
+    x = convert_to_tensor(x)
+    return tnn.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return np.logaddexp(x, np.array(0.0, x.dtype))
+    return tnn.softplus(x)
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return x / (np.array(1.0, x.dtype) + np.abs(x))
+    return tnn.softsign(x)
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return x * sigmoid(x)
+    return tnn.silu(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return -softplus(-x)
+    return tnn.logsigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return np.maximum(x, np.array(negative_slope, x.dtype) * x)
+    return tnn.leaky_relu(x, negative_slope=negative_slope)
 
 
 def hard_sigmoid(x):
-    # python numbers will be promoted to float64 by np, so it's necessary to
-    # first convert the python numbers to np scalars
-    x = x / np.array(6.0, x.dtype) + np.array(0.5, x.dtype)
-    return np.where(
-        x <= 0.0,
-        np.array(0.0, x.dtype),
-        np.where(x >= 1.0, np.array(1.0, x.dtype), x),
-    )
+    x = convert_to_tensor(x)
+    return tnn.hardsigmoid(x)
 
 
 def hard_silu(x):
-    return x * hard_sigmoid(x)
+    x = convert_to_tensor(x)
+    return tnn.hardswish(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return np.where(
-        x >= np.array(0.0, x.dtype), x, np.array(alpha, x.dtype) * np.expm1(x)
-    )
+    return tnn.elu(x, alpha)
 
 
-def selu(
-    x,
-    alpha=1.6732632423543772848170429916717,
-    scale=1.0507009873554804934193349852946,
-):
+def selu(x):
     x = convert_to_tensor(x)
-    return np.array(scale, x.dtype) * elu(x, alpha)
+    return tnn.selu(x)
 
 
 def gelu(x, approximate=True):
+    # TODO: torch.nn.gelu expects string approximate of `"none"` or `"tanh"`
     x = convert_to_tensor(x)
-    # followed by JAX's implementation
     if approximate:
-        sqrt_2_over_pi = np.sqrt(2 / np.pi).astype(x.dtype)
-        cdf = np.array(0.5, x.dtype) * (
-            np.array(1.0, x.dtype)
-            + np.tanh(
-                sqrt_2_over_pi
-                * (x + np.array(0.044715, x.dtype) * (x**3).astype(x.dtype))
-            )
-        )
-        return x * cdf
-    else:
-        sqrt_2 = np.sqrt(2).astype(x.dtype)
-        return (
-            x
-            * (scipy.special.erf(x / sqrt_2) + 1).astype(x.dtype)
-            / np.array(2, x.dtype)
-        )
+        return tnn.gelu(x, approximate="tanh")
+    return tnn.gelu(x)
 
 
-def softmax(x, axis=None):
-    exp_x = np.exp(x - np.max(x, axis=axis, keepdims=True))
-    return exp_x / np.sum(exp_x, axis=axis, keepdims=True)
+def softmax(x, axis=-1):
+    x = convert_to_tensor(x)
+    dtype = standardize_dtype(x.dtype)
+    # TODO: tnn.softmax doesn't support float16 using cpu
+    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+        x = cast(x, "float32")
+    if axis is None:
+        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
+        # We need this workaround for the reduction on every dim.
+        output = torch.reshape(x, [-1])
+        output = tnn.softmax(output, dim=-1)
+        output = torch.reshape(output, x.shape)
+    else:
+        output = tnn.softmax(x, dim=axis)
+    return cast(output, dtype)
 
 
-def log_softmax(x, axis=None):
-    max_x = np.max(x, axis=axis, keepdims=True)
-    logsumexp = np.log(np.exp(x - max_x).sum(axis=axis, keepdims=True))
-    return x - max_x - logsumexp
+def log_softmax(x, axis=-1):
+    x = convert_to_tensor(x)
+    dtype = standardize_dtype(x.dtype)
+    # TODO: tnn.log_softmax doesn't support float16 using cpu
+    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
+        x = cast(x, "float32")
+    if axis is None:
+        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
+        # We need this workaround for the reduction on every dim.
+        output = torch.reshape(x, [-1])
+        output = tnn.log_softmax(output, dim=-1)
+        output = torch.reshape(output, x.shape)
+    else:
+        output = tnn.log_softmax(x, dim=axis)
+    return cast(output, dtype)
 
 
-def _convert_to_spatial_operand(
-    x,
-    num_spatial_dims,
-    data_format="channels_last",
-    include_batch_and_channels=True,
+def _compute_padding_length(
+    input_length, kernel_length, stride, dilation_rate=1
 ):
-    # Helper function that converts an operand to a spatial operand.
-    x = (x,) * num_spatial_dims if isinstance(x, int) else x
-    if not include_batch_and_channels:
-        return x
-    if data_format == "channels_last":
-        x = (1,) + x + (1,)
-    else:
-        x = (1,) + (1,) + x
-    return x
+    """Compute padding length along one dimension."""
+    total_padding_length = (
+        dilation_rate * (kernel_length - 1) - (input_length - 1) % stride
+    )
+    left_padding = total_padding_length // 2
+    right_padding = (total_padding_length + 1) // 2
+    return (left_padding, right_padding)
 
 
-def _pool(
-    inputs,
-    initial_value,
-    reduce_fn,
-    pool_size,
-    strides=None,
-    padding="valid",
+def _apply_same_padding(
+    inputs, kernel_size, strides, operation_type, dilation_rate=1
 ):
-    """Helper function to define pooling functions.
+    """Apply same padding to the input tensor.
 
-    Args:
-        inputs: input data of shape `N+2`.
-        initial_value: the initial value for the reduction.
-        reduce_fn: a reduce function of the form `(T, T) -> T`.
-        pool_size: a sequence of `N` integers, representing the window size to
-            reduce over.
-        strides: a sequence of `N` integers, representing the inter-window
-            strides (default: `(1, ..., 1)`).
-        padding: either the string `same` or `valid`.
+    This function will evaluate if the padding value is compatible with torch
+    functions. To avoid calling `pad()` as much as possible, which may cause
+    performance or memory issues, when compatible, it does not apply the padding
+    to the tensor, but returns the input tensor and the padding value to pass to
+    the torch functions. If not compatible, it returns the padded tensor and 0
+    as the padding value.
 
     Returns:
-        The output of the reduction for each window slice.
+        tensor: A padded tensor or the inputs.
+        padding: The padding value, ready to pass to the torch functions.
     """
-    if padding not in ("same", "valid"):
-        raise ValueError(
-            f"Invalid padding '{padding}', must be 'same' or 'valid'."
-        )
-    padding = padding.upper()
-    return np.array(
-        lax.reduce_window(
-            inputs,
-            initial_value,
-            reduce_fn,
-            pool_size,
-            strides,
-            padding,
-        )
+    spatial_shape = inputs.shape[2:]
+    num_spatial_dims = len(spatial_shape)
+    padding = ()
+
+    for i in range(num_spatial_dims):
+        if operation_type == "pooling":
+            padding_size = _compute_padding_length(
+                spatial_shape[i], kernel_size[i], strides[i]
+            )
+            mode = "replicate"
+        else:
+            dilation_rate = standardize_tuple(
+                dilation_rate, num_spatial_dims, "dilation_rate"
+            )
+            padding_size = _compute_padding_length(
+                spatial_shape[i], kernel_size[i], strides[i], dilation_rate[i]
+            )
+            mode = "constant"
+        padding = (padding_size,) + padding
+
+    if all([left == right for left, right in padding]):
+        return inputs, [left for left, _ in padding]
+
+    flattened_padding = tuple(
+        value for left_and_right in padding for value in left_and_right
     )
+    return tnn.pad(inputs, pad=flattened_padding, mode=mode), 0
+
+
+def _transpose_spatial_inputs(inputs):
+    num_spatial_dims = inputs.ndim - 2
+    # Torch pooling does not support `channels_last` format, so
+    # we need to transpose to `channels_first` format.
+    if num_spatial_dims == 1:
+        inputs = torch.permute(inputs, (0, 2, 1))
+    elif num_spatial_dims == 2:
+        inputs = torch.permute(inputs, (0, 3, 1, 2))
+    elif num_spatial_dims == 3:
+        inputs = torch.permute(inputs, (0, 4, 1, 2, 3))
+    else:
+        raise ValueError(
+            "Inputs must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+    return inputs
+
+
+def _transpose_spatial_outputs(outputs):
+    # Undo the transpose in `_transpose_spatial_inputs`.
+    num_spatial_dims = len(outputs.shape) - 2
+    if num_spatial_dims == 1:
+        outputs = torch.permute(outputs, (0, 2, 1))
+    elif num_spatial_dims == 2:
+        outputs = torch.permute(outputs, (0, 2, 3, 1))
+    elif num_spatial_dims == 3:
+        outputs = torch.permute(outputs, (0, 2, 3, 4, 1))
+    return outputs
+
+
+def _transpose_conv_kernel(kernel):
+    # Torch requires conv kernel of format
+    # `(out_channels, in_channels, spatial_dims)`, we need to transpose.
+    num_spatial_dims = len(kernel.shape) - 2
+    if num_spatial_dims == 1:
+        kernel = torch.permute(kernel, (2, 1, 0))
+    elif num_spatial_dims == 2:
+        kernel = torch.permute(kernel, (3, 2, 0, 1))
+    elif num_spatial_dims == 3:
+        kernel = torch.permute(kernel, (4, 3, 0, 1, 2))
+    return kernel
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
+    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
+    if strides is None:
+        strides = pool_size
+    else:
+        strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
+    if data_format == "channels_last":
+        inputs = _transpose_spatial_inputs(inputs)
+
+    if padding == "same":
+        # Torch does not natively support `"same"` padding, we need to manually
+        # apply the right amount of padding to `inputs`.
+        inputs, padding = _apply_same_padding(
+            inputs, pool_size, strides, operation_type="pooling"
+        )
+    else:
+        padding = 0
+
+    device = get_device()
+    # Torch max pooling ops do not support symbolic tensors.
+    # Create a real tensor to execute the ops.
+    if device == "meta":
+        inputs = torch.empty(
+            size=inputs.shape, dtype=inputs.dtype, device="cpu"
+        )
+
+    if num_spatial_dims == 1:
+        outputs = tnn.max_pool1d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    elif num_spatial_dims == 2:
+        outputs = tnn.max_pool2d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.max_pool3d(
+            inputs, kernel_size=pool_size, stride=strides, padding=padding
+        )
+    else:
+        raise ValueError(
+            "Inputs to pooling op must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+
+    outputs = outputs.to(device)
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def average_pool(
     inputs,
     pool_size,
-    strides,
-    padding,
+    strides=None,
+    padding="valid",
     data_format=None,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = _convert_to_spatial_operand(
-        pool_size, num_spatial_dims, data_format
-    )
-    strides = pool_size if strides is None else strides
-    strides = _convert_to_spatial_operand(
-        strides, num_spatial_dims, data_format
-    )
-
-    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
-    if padding == "valid":
-        # Avoid the extra reduce_window.
-        return pooled / np.prod(pool_size)
-    else:
-        # Count the number of valid entries at each input point, then use that
-        # for computing average. Assumes that any two arrays of same shape will
-        # be padded the same. Avoid broadcasting on axis where pooling is
-        # skipped.
-        shape = [
-            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
-        ]
-        window_counts = _pool(
-            jnp.ones(shape, inputs.dtype),
-            0.0,
-            lax.add,
-            pool_size,
-            strides,
-            padding,
-        )
-        return pooled / window_counts
-
-
-def _convert_to_lax_conv_dimension_numbers(
-    num_spatial_dims,
-    data_format="channels_last",
-    transpose=False,
-):
-    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
-    num_dims = num_spatial_dims + 2
+    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
+    if strides is None:
+        strides = pool_size
+    else:
+        strides = standardize_tuple(strides, num_spatial_dims, "strides")
 
+    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        spatial_dims = tuple(range(1, num_dims - 1))
-        inputs_dn = (0, num_dims - 1) + spatial_dims
-    else:
-        spatial_dims = tuple(range(2, num_dims))
-        inputs_dn = (0, 1) + spatial_dims
+        inputs = _transpose_spatial_inputs(inputs)
+    padding_value = 0
+    if padding == "same":
+        spatial_shape = inputs.shape[2:]
+        num_spatial_dims = len(spatial_shape)
+        padding_value = []
+        uneven_padding = []
+
+        for i in range(num_spatial_dims):
+            padding_size = _compute_padding_length(
+                spatial_shape[i], pool_size[i], strides[i]
+            )
+            # Torch only supports even padding on each dim, to replicate the
+            # behavior of "same" padding of `tf.keras` as much as possible,
+            # we need to pad evenly using the shorter padding.
+            padding_value.append(padding_size[0])
+            if padding_size[0] != padding_size[1]:
+                # Handle unequal padding.
+                # `torch.nn.pad` sets padding value in the reverse order.
+                uneven_padding = [0, 1] + uneven_padding
+        # Only call tnn.pad when needed.
+        if len(uneven_padding) > 0:
+            inputs = tnn.pad(inputs, uneven_padding)
 
-    if transpose:
-        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
+    if num_spatial_dims == 1:
+        outputs = tnn.avg_pool1d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
+    elif num_spatial_dims == 2:
+        outputs = tnn.avg_pool2d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.avg_pool3d(
+            inputs,
+            kernel_size=pool_size,
+            stride=strides,
+            padding=padding_value,
+            count_include_pad=False,
+        )
     else:
-        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
-
-    return lax.ConvDimensionNumbers(
-        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
-    )
+        raise ValueError(
+            "Inputs to pooling op must have ndim=3, 4 or 5, "
+            "corresponding to 1D, 2D and 3D inputs. "
+            f"Received input shape: {inputs.shape}."
+        )
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
+    kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
+    strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        channels = inputs.shape[-1]
-    else:
-        channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[-2]
+        inputs = _transpose_spatial_inputs(inputs)
+    # Transpose kernel from keras format to torch format.
+    kernel = _transpose_conv_kernel(kernel)
+    if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
+        # Torch does not support this case in conv2d().
+        # Manually pad the tensor.
+        inputs, padding = _apply_same_padding(
+            inputs,
+            kernel.shape[2:],
+            strides,
+            operation_type="conv",
+            dilation_rate=dilation_rate,
+        )
+    channels = inputs.shape[1]
+    kernel_in_channels = kernel.shape[1]
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
-            f"kernel's in_channels. Received input channels {channels} and "
-            f"kernel in_channels {kernel_in_channels}. "
+            f"kernel.shape[1]. Received: inputs.shape={inputs.shape}, "
+            f"kernel.shape={kernel.shape}"
         )
-    feature_group_count = channels // kernel_in_channels
-    return np.array(
-        jax.lax.conv_general_dilated(
+    groups = channels // kernel_in_channels
+    if num_spatial_dims == 1:
+        outputs = tnn.conv1d(
             inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
         )
-    )
+    elif num_spatial_dims == 2:
+        outputs = tnn.conv2d(
+            inputs,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.conv3d(
+            inputs,
+            kernel,
+            stride=strides,
+            dilation=dilation_rate,
+            groups=groups,
+            padding=padding,
+        )
+    else:
+        raise ValueError(
+            "Inputs to conv operation should have ndim=3, 4, or 5,"
+            "corresponding to 1D, 2D and 3D inputs. Received input "
+            f"shape: {inputs.shape}."
+        )
+
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
-    num_spatial_dims = inputs.ndim - 2
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    feature_group_count = (
-        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
-    )
-    kernel = jnp.reshape(
-        kernel if is_tensor(kernel) else kernel.numpy(),
-        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
-    )
-    return np.array(
-        jax.lax.conv_general_dilated(
-            inputs,
-            kernel,
-            strides,
-            padding,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            feature_group_count=feature_group_count,
-        )
+    kernel = convert_to_tensor(kernel)
+    kernel = torch.reshape(
+        kernel, kernel.shape[:-2] + (1, kernel.shape[-2] * kernel.shape[-1])
     )
+    return conv(inputs, kernel, strides, padding, data_format, dilation_rate)
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -400,100 +485,117 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    data_format = standardize_data_format(data_format)
+    inputs = convert_to_tensor(inputs)
+    kernel = convert_to_tensor(kernel)
     num_spatial_dims = inputs.ndim - 2
-    padding_values = compute_conv_transpose_padding_args_for_jax(
+    strides = standardize_tuple(strides, num_spatial_dims, "strides")
+
+    data_format = standardize_data_format(data_format)
+    (
+        torch_padding,
+        torch_output_padding,
+    ) = compute_conv_transpose_padding_args_for_torch(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
         dilation_rate=dilation_rate,
     )
-    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
-        num_spatial_dims,
-        data_format,
-        transpose=False,
-    )
-    strides = _convert_to_spatial_operand(
-        strides,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
-    dilation_rate = _convert_to_spatial_operand(
-        dilation_rate,
-        num_spatial_dims,
-        data_format,
-        include_batch_and_channels=False,
-    )
+    if data_format == "channels_last":
+        inputs = _transpose_spatial_inputs(inputs)
+    # Transpose kernel from keras format to torch format.
+    kernel = _transpose_conv_kernel(kernel)
+    kernel_spatial_shape = kernel.shape[2:]
+    if isinstance(dilation_rate, int):
+        dilation_rate = [dilation_rate] * len(kernel_spatial_shape)
 
-    return np.array(
-        jax.lax.conv_transpose(
+    if num_spatial_dims == 1:
+        outputs = tnn.conv_transpose1d(
             inputs,
-            kernel if is_tensor(kernel) else kernel.numpy(),
-            strides,
-            padding=padding_values,
-            rhs_dilation=dilation_rate,
-            dimension_numbers=dimension_numbers,
-            transpose_kernel=True,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
         )
-    )
+    elif num_spatial_dims == 2:
+        outputs = tnn.conv_transpose2d(
+            inputs,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
+        )
+    elif num_spatial_dims == 3:
+        outputs = tnn.conv_transpose3d(
+            inputs,
+            kernel,
+            stride=strides,
+            padding=torch_padding,
+            output_padding=torch_output_padding,
+            dilation=dilation_rate,
+        )
+    else:
+        raise ValueError(
+            "Inputs to conv transpose operation should have ndim=3, 4, or 5,"
+            "corresponding to 1D, 2D and 3D inputs. Received input "
+            f"shape: {inputs.shape}."
+        )
+    if data_format == "channels_last":
+        outputs = _transpose_spatial_outputs(outputs)
+    return outputs
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
-    x = convert_to_tensor(x)
-    input_shape = x.shape
-
-    # Shrink the last dimension if the shape is (..., 1).
-    if input_shape and input_shape[-1] == 1 and len(input_shape) > 1:
-        input_shape = tuple(input_shape[:-1])
-
-    x = x.reshape(-1)
-    if not num_classes:
-        num_classes = np.max(x) + 1
-
-    batch_size = x.shape[0]
-    categorical = np.zeros((batch_size, num_classes), dtype=dtype)
-    valid_indices = x >= 0
-    categorical[np.arange(batch_size)[valid_indices], x[valid_indices]] = 1
-
-    # First, reshape the array with the extra dimension at the end
-    output_shape = input_shape + (num_classes,)
-    categorical = np.reshape(categorical, output_shape)
-
-    # Then, move this new dimension to the right place (according to axis)
-    if axis != -1:
-        categorical = np.moveaxis(categorical, -1, axis)
-
-    return categorical
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
+    # Axis is the output axis. By default, PyTorch, outputs to last axis.
+    # If axis is not last, change output to axis and shift remaining elements.
+    x = convert_to_tensor(x, dtype=torch.long)
+
+    # Torch one_hot does not natively handle negative values, so we add some
+    # manual handling for negatives in the input to one_hot by using max(x, 0).
+    # The output will have some invalid results, so we set them back to 0 using
+    # `where` afterwards.
+    output = tnn.one_hot(maximum(x, 0), num_classes)
+    output = where(expand_dims(x, axis=-1) >= 0, output, 0)
+    output = convert_to_tensor(output, dtype=dtype)
+    dims = output.dim()
+    if axis != -1 and axis != dims:
+        new_axes_order = list(range(dims))
+        new_axes_order[axis] = -1  # Shifts output to axis position
+        # Shift remaining axes with offset by 1 since output moved to `axis`.
+        for ax in range(axis + 1, dims):
+            new_axes_order[ax] -= 1
+        output = output.permute(new_axes_order)
+    return output
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with numpy backend")
+        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = np.max(
+    outputs = torch.amax(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        axis=reduction_axis,
+        dim=reduction_axis,
     )
     return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target)
-    output = np.array(output)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -501,118 +603,177 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = log_softmax(output, axis=axis)
+        log_prob = tnn.log_softmax(output, dim=axis)
     else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
-    return -np.sum(target * log_prob, axis=axis)
+        output = output / torch.sum(output, dim=axis, keepdim=True)
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = torch.log(output)
+    return -torch.sum(target * log_prob, dim=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = np.array(target, dtype="int32")
-    output = np.array(output)
+    target = convert_to_tensor(target, dtype=torch.long)
+    output = convert_to_tensor(output)
+
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = np.squeeze(target, axis=-1)
+        target = torch.squeeze(target, dim=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = log_softmax(output, axis=axis)
+        log_prob = tnn.log_softmax(output, dim=axis)
     else:
-        output = output / np.sum(output, axis, keepdims=True)
-        output = np.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = np.log(output)
+        output = output / torch.sum(output, dim=axis, keepdim=True)
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = torch.log(output)
     target = one_hot(target, output.shape[axis], axis=axis)
-    return -np.sum(target * log_prob, axis=axis)
+    return -torch.sum(target * log_prob, dim=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = np.array(target)
-    output = np.array(output)
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
-
+    # By default, PyTorch, does reduction of `sum` over all rows,
+    # change reduction to `none` to keep dim
     if from_logits:
-        output = sigmoid(output)
-
-    output = np.clip(output, epsilon(), 1.0 - epsilon())
-    bce = target * np.log(output)
-    bce += (1.0 - target) * np.log(1.0 - output)
-    return -bce
+        return tnn.binary_cross_entropy_with_logits(
+            output, target, reduction="none"
+        )
+    else:
+        output = torch.clip(output, epsilon(), 1.0 - epsilon())
+        return tnn.binary_cross_entropy(output, target, reduction="none")
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with NumPy."
+            "Argument synchronized=True is not supported with PyTorch."
         )
-    axes = tuple(axes) if isinstance(axes, list) else axes
+    x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
     if ori_dtype == "float16":
         need_cast = True
         x = cast(x, "float32")
 
-    mean = np.mean(x, axes, keepdims=True)
+    mean = torch.mean(x, dim=axes, keepdim=True)
 
     # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
     # but less numerically stable.
-    variance = np.mean(np.square(x), axis=axes, keepdims=True) - np.square(mean)
+    # Note: stop_gradient does not change the gradient to the mean, because that
+    # gradient is zero.
+    variance = torch.mean(
+        torch.square(x), dim=axes, keepdim=True
+    ) - torch.square(mean)
 
     if not keepdims:
-        mean = np.squeeze(mean, axes)
-        variance = np.squeeze(variance, axes)
+        mean = torch.squeeze(mean, axes)
+        variance = torch.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = np.clip(mean, np.finfo(np.float16).min, np.finfo(np.float16).max)
-        variance = np.clip(
-            variance, np.finfo(np.float16).min, np.finfo(np.float16).max
+        mean = torch.clip(
+            mean,
+            torch.finfo(torch.float16).min,
+            torch.finfo(torch.float16).max,
+        )
+        variance = torch.clip(
+            variance,
+            torch.finfo(torch.float16).min,
+            torch.finfo(torch.float16).max,
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
+    x = convert_to_tensor(x)
+    mean = convert_to_tensor(mean)
+    variance = convert_to_tensor(variance)
+
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = np.reshape(mean, shape)
-    variance = np.reshape(variance, shape)
+    mean = torch.reshape(mean, shape)
+    variance = torch.reshape(variance, shape)
 
-    inv = 1.0 / np.sqrt(variance + epsilon)
+    if offset is not None:
+        offset = convert_to_tensor(offset)
+        offset = torch.reshape(offset, shape)
+    else:
+        offset = torch.zeros_like(mean)
     if scale is not None:
-        scale = np.reshape(scale, shape)
-        inv = inv * scale
+        scale = convert_to_tensor(scale)
+        scale = torch.reshape(scale, shape)
+    else:
+        scale = torch.ones_like(variance)
+
+    return (
+        x.subtract(mean)
+        .mul_(variance.add(epsilon).rsqrt_().mul(scale))
+        .add_(offset)
+    )
 
-    res = -mean * inv
-    if offset is not None:
-        offset = np.reshape(offset, shape)
-        res = res + offset
 
-    return x * inv + res
+def ctc_loss(
+    target,
+    output,
+    target_length,
+    output_length,
+    mask_index=0,
+):
+    target = convert_to_tensor(target)
+    output = convert_to_tensor(output)
+    target_length = convert_to_tensor(target_length)
+    output_length = convert_to_tensor(output_length)
+
+    output = torch.transpose(output, 1, 0)
+    logits = tnn.log_softmax(output, dim=-1)
 
+    return tnn.ctc_loss(
+        logits,
+        target,
+        output_length,
+        target_length,
+        blank=mask_index,
+        reduction="none",
+    )
+
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    raise NotImplementedError(
+        "Torch backend does not yet support CTC decoding."
+    )
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/numpy.py` & `keras-3.3.0/keras/src/backend/numpy/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import numpy as np
 
+from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import standardize_axis_for_numpy
 from keras.src.backend.numpy.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 def add(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
         x2 = convert_to_tensor(x2)
@@ -223,22 +223,22 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = x.astype(dtype)
     return np.arctanh(x)
 
 
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     axis = standardize_axis_for_numpy(axis)
-    return np.argmax(x, axis=axis).astype("int32")
+    return np.argmax(x, axis=axis, keepdims=keepdims).astype("int32")
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     axis = standardize_axis_for_numpy(axis)
-    return np.argmin(x, axis=axis).astype("int32")
+    return np.argmin(x, axis=axis, keepdims=keepdims).astype("int32")
 
 
 def argsort(x, axis=-1):
     axis = standardize_axis_for_numpy(axis)
     return np.argsort(x, axis=axis).astype("int32")
 
 
@@ -684,16 +684,16 @@
     return np.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
     return np.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
-    return np.nan_to_num(x)
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
+    return np.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     return np.ndim(x)
 
 
 def nonzero(x):
@@ -933,14 +933,18 @@
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(
             lambda x: convert_to_tensor(x).astype(dtype), xs
         )
     return np.vstack(xs)
 
 
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return np.vectorize(pyfunc, excluded=excluded, signature=signature)
+
+
 def where(condition, x1, x2):
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
             x2 = convert_to_tensor(x2)
         dtype = dtypes.result_type(
@@ -1087,7 +1091,10 @@
     elif dtype not in ["bfloat16", "float16", "float64"]:
         dtype = "float32"
 
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return np.correlate(x1, x2, mode)
 
+
+def select(condlist, choicelist, default=0):
+    return np.select(condlist, choicelist, default=default)
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/random.py` & `keras-3.3.0/keras/src/backend/numpy/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,7 @@
 
 def beta(shape, alpha, beta, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = draw_seed(seed)
     rng = np.random.default_rng(seed)
     sample = rng.beta(a=alpha, b=beta, size=shape).astype(dtype)
     return sample
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/rnn.py` & `keras-3.3.0/keras/src/backend/numpy/rnn.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import numpy as np
 
-from keras.src.utils import tree
+from keras.src import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -233,8 +233,7 @@
         outputs = np.flip(outputs, axis=0)
 
     return states, outputs
 
 
 def cudnn_ok(*args, **kwargs):
     return False
-
```

### Comparing `keras-3.2.1/keras/src/backend/numpy/trainer.py` & `keras-3.3.0/keras/src/backend/numpy/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import numpy as np
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
+from keras.src import tree
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.numpy.core import is_tensor
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class NumpyTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.test_function = None
         self.predict_function = None
@@ -265,18 +265,19 @@
         self.stop_evaluating = False
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         for step, data in epoch_iterator.enumerate_epoch():
             callbacks.on_test_batch_begin(step)
             logs = self.test_function(data)
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     def train_on_batch(
@@ -315,8 +316,7 @@
     def predict_on_batch(self, x):
         self.make_predict_function()
         batch_outputs = self.predict_function([(x,)])
         batch_outputs = tree.map_structure(
             backend.convert_to_numpy, batch_outputs
         )
         return batch_outputs
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/__init__.py` & `keras-3.3.0/keras/src/backend/tensorflow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,8 +21,7 @@
 from keras.src.backend.tensorflow.core import shape
 from keras.src.backend.tensorflow.core import stop_gradient
 from keras.src.backend.tensorflow.core import vectorized_map
 from keras.src.backend.tensorflow.rnn import cudnn_ok
 from keras.src.backend.tensorflow.rnn import gru
 from keras.src.backend.tensorflow.rnn import lstm
 from keras.src.backend.tensorflow.rnn import rnn
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/core.py` & `keras-3.3.0/keras/src/backend/tensorflow/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import numpy as np
 import tensorflow as tf
 from tensorflow.compiler.tf2xla.python.xla import dynamic_update_slice
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.name_scope import name_scope as base_name_scope
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.common.stateless_scope import in_stateless_scope
-from keras.src.utils import tree
+from keras.src.backend.tensorflow.sparse import sparse_to_dense
 from keras.src.utils.naming import auto_name
 
 SUPPORTS_SPARSE_TENSORS = True
 
 
 class Variable(
     KerasVariable,
@@ -96,17 +97,15 @@
 
     def _write_object_proto(self, proto, options):
         return self.value._write_object_proto(proto, options)
 
 
 def convert_to_tensor(x, dtype=None, sparse=None):
     if isinstance(x, tf.SparseTensor) and sparse is not None and not sparse:
-        x_shape = x.shape
-        x = tf.sparse.to_dense(x)
-        x.set_shape(x_shape)
+        x = sparse_to_dense(x)
     if dtype is not None:
         dtype = standardize_dtype(dtype)
     if not tf.is_tensor(x):
         if dtype == "bool":
             # TensorFlow boolean conversion is stricter than other backends.
             # It does not allow ints. We convert without dtype and cast instead.
             x = tf.convert_to_tensor(x)
@@ -120,17 +119,15 @@
             return x
         return tf.cast(x, dtype=dtype)
     return x
 
 
 def convert_to_numpy(x):
     if isinstance(x, tf.SparseTensor):
-        x_shape = x.shape
-        x = tf.sparse.to_dense(x)
-        x.set_shape(x_shape)
+        x = sparse_to_dense(x)
     elif isinstance(x, tf.IndexedSlices):
         x = tf.convert_to_tensor(x)
     elif isinstance(x, tf.RaggedTensor):
         x = x.to_tensor()
     return np.asarray(x)
 
 
@@ -298,8 +295,7 @@
         super().__exit__(*args, **kwargs)
         if self._pop_on_exit:
             self._tf_name_scope.__exit__(*args, **kwargs)
 
 
 def device_scope(device_name):
     return tf.device(device_name)
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/distribution_lib.py` & `keras-3.3.0/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,21 +19,30 @@
         device_type: string of `"cpu"`, `"gpu"` or `"tpu"`. Default to `gpu` or
         `tpu` if available when device_type is not provided. Otherwise will
         return the `cpu` devices.
 
     Return:
         List of devices that are available for distribute computation.
     """
-    device_type = device_type.upper() if device_type else "CPU"
+    device_type = device_type.upper() if device_type else None
 
     # DTensor doesn't support getting global devices, even when knowing the
     # Mesh. Use TF API instead to get global devices. Coordinator service is
     # enabled by default with DTensor, so that list_logical_devices() returns
     # a list of global devices. More context can be found in b/254911601.
     tf_devices = tf.config.list_logical_devices(device_type=device_type)
+    cpu_devices = []
+    other_devices = []
+    for device in tf_devices:
+        if device.device_type.lower() == "cpu":
+            cpu_devices.append(device)
+        else:
+            other_devices.append(device)
+    if device_type is None:
+        tf_devices = other_devices if len(other_devices) > 0 else cpu_devices
     return [
         f"{device.device_type.lower()}:{device.name.split(':')[-1]}"
         for device in tf_devices
     ]
 
 
 def distribute_value(value, tensor_layout):
@@ -72,8 +81,7 @@
         )
 
     sharding_specs = [
         axis if axis else dtensor.UNSHARDED for axis in tensor_layout.axes
     ]
     dtensor_mesh = _to_dtensor_mesh(tensor_layout.device_mesh)
     return dtensor.Layout(sharding_specs=sharding_specs, mesh=dtensor_mesh)
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/layer.py` & `keras-3.3.0/keras/src/backend/tensorflow/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tensorflow as tf
 
+from keras.src import tree
 from keras.src.backend.tensorflow.trackable import KerasAutoTrackable
 from keras.src.utils import tf_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class TFLayer(KerasAutoTrackable):
     def __init__(self, *args, **kwargs):
         # Export-related attributes
         self._saved_model_inputs_spec = None
         self._saved_model_arg_spec = None
@@ -116,8 +116,7 @@
                 ]
 
         @tf.function(input_signature=input_signature)
         def serving_default(inputs):
             return self(inputs)
 
         return serving_default
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/linalg.py` & `keras-3.3.0/keras/src/backend/tensorflow/linalg.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
@@ -18,24 +17,30 @@
     return tf.linalg.det(a)
 
 
 def eig(a):
     return tf.linalg.eig(a)
 
 
+def eigh(a):
+    return tf.linalg.eigh(a)
+
+
 def inv(a):
     return tf.linalg.inv(a)
 
 
 def lu_factor(a):
     lu, p = tf.linalg.lu(a)
     return lu, tf.math.invert_permutation(p)
 
 
 def norm(x, ord=None, axis=None, keepdims=False):
+    from keras.src.backend.tensorflow.numpy import moveaxis
+
     x = convert_to_tensor(x)
     x_shape = x.shape
     ndim = x_shape.rank
 
     if axis is None:
         axis = tuple(range(ndim))
     elif isinstance(axis, int):
@@ -121,15 +126,15 @@
                 row_axis -= 1
             x = tf.math.reduce_min(
                 tf.reduce_sum(tf.math.abs(x), axis=col_axis, keepdims=keepdims),
                 axis=row_axis,
                 keepdims=keepdims,
             )
         elif ord in ("nuc", 2, -2):
-            x = tfnp.moveaxis(x, axis, (-2, -1))
+            x = moveaxis(x, axis, (-2, -1))
             if ord == -2:
                 x = tf.math.reduce_min(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
                 )
             elif ord == 2:
                 x = tf.math.reduce_max(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
@@ -180,8 +185,7 @@
 
 
 def svd(x, full_matrices=True, compute_uv=True):
     s, u, v = tf.linalg.svd(
         x, full_matrices=full_matrices, compute_uv=compute_uv
     )
     return u, s, tf.linalg.adjoint(v)
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/math.py` & `keras-3.3.0/keras/src/backend/tensorflow/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
 
@@ -256,14 +255,16 @@
 def solve(a, b):
     a = convert_to_tensor(a)
     b = convert_to_tensor(b)
     return tf.linalg.solve(a, b)
 
 
 def norm(x, ord=None, axis=None, keepdims=False):
+    from keras.src.backend.tensorflow.numpy import moveaxis
+
     x = convert_to_tensor(x)
     x_shape = x.shape
     ndim = x_shape.rank
 
     if axis is None:
         axis = tuple(range(ndim))
     elif isinstance(axis, int):
@@ -324,15 +325,15 @@
                 col_axis -= 1
             x = tf.math.reduce_min(
                 tf.reduce_sum(tf.math.abs(x), axis=row_axis, keepdims=keepdims),
                 axis=col_axis,
                 keepdims=keepdims,
             )
         else:
-            x = tfnp.moveaxis(x, axis, (-2, -1))
+            x = moveaxis(x, axis, (-2, -1))
             if ord == -2:
                 x = tf.math.reduce_min(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
                 )
             else:
                 x = tf.math.reduce_sum(
                     tf.linalg.svd(x, compute_uv=False), axis=-1
@@ -348,8 +349,7 @@
         )
     elif num_axes == 2:
         raise ValueError(
             f"Invalid `ord` argument for matrix norm. Received: ord={ord}"
         )
     else:
         raise ValueError(f"Invalid axis values. Received: axis={axis}")
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/nn.py` & `keras-3.3.0/keras/src/backend/tensorflow/nn.py`

 * *Files 3% similar despite different names*

```diff
@@ -442,15 +442,15 @@
         padding=padding.upper(),
         data_format=tf_data_format,
         dilations=dilation_rate,
     )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    x = convert_to_tensor(x)
+    x = convert_to_tensor(x, dtype="int64")
     if dtype is None:
         dtype = "float32"
     if sparse:
         # We don't use `tf.sparse.bincount`, it doesn't handle negative indices
         # and only support rank 1 and 2 tensors (`one_hot` adds a dimension).
         if axis < 0:
             axis = axis + len(x.shape) + 1
@@ -793,39 +793,53 @@
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    """Runs CTC (Connectionist Temporal Classification) loss on each
-    batch element.
-
-    Arguments:
-        target: Tensor `(batch_size, max_length)` containing the
-            target sequences in integer format.
-        output: Tensor `(batch_size, max_length, num_classes)`
-            containing the output of the softmax.
-        target_length: Tensor `(batch_size,)` containing the sequence length
-            for each target sequence in the batch.
-        output_length: Tensor `(batch_size,)` containing the sequence length
-            for each output sequence in the batch.
-        mask_index: The value in `target` and `output` that represents the
-            blank label.
-
-    Returns:
-        A tensor of shape `(batch_size,)` containing the CTC loss for each
-        sample in the batch.
-    """
     target = tf.convert_to_tensor(target)
     target = tf.cast(target, dtype="int32")
     output = tf.convert_to_tensor(output)
     output = tf.cast(output, dtype="float32")
     return tf.nn.ctc_loss(
         labels=target,
         logits=output,
         label_length=target_length,
         logit_length=output_length,
         blank_index=mask_index,
         logits_time_major=False,
     )
 
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = tf.convert_to_tensor(inputs)
+    inputs = tf.transpose(inputs, (1, 0, 2))
+
+    sequence_length = tf.convert_to_tensor(sequence_length, dtype="int32")
+    if strategy == "greedy":
+        return tf.nn.ctc_greedy_decoder(
+            inputs=inputs,
+            sequence_length=sequence_length,
+            merge_repeated=merge_repeated,
+            blank_index=mask_index,
+        )
+    elif strategy == "beam_search":
+        return tf.nn.ctc_beam_search_decoder(
+            inputs=inputs,
+            sequence_length=sequence_length,
+            beam_width=beam_width,
+            top_paths=top_paths,
+        )
+    else:
+        raise ValueError(
+            f"Invalid strategy {strategy}. Supported values are "
+            "'greedy' and 'beam_search'."
+        )
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/numpy.py` & `keras-3.3.0/keras/src/backend/tensorflow/numpy.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 import functools
 import math
 import string
 import warnings
 
 import numpy as np
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 from tensorflow.python.ops.linalg.sparse import sparse_csr_matrix_ops
 
+from keras.src import tree
 from keras.src.backend import config
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
+from keras.src.backend.common.backend_utils import vectorize_impl
 from keras.src.backend.tensorflow import sparse
 from keras.src.backend.tensorflow.core import cast
 from keras.src.backend.tensorflow.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 @sparse.elementwise_binary_union(tf.sparse.add)
 def add(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
@@ -571,54 +571,63 @@
     output = tf.reduce_mean(
         tf.cast(x, compute_dtype), axis=axis, keepdims=keepdims
     )
     return tf.cast(output, result_dtype)
 
 
 def max(x, axis=None, keepdims=False, initial=None):
+    x = convert_to_tensor(x)
+
     # The TensorFlow numpy API implementation doesn't support `initial` so we
     # handle it manually here.
     if initial is not None:
-        return tf.math.maximum(
-            tfnp.max(x, axis=axis, keepdims=keepdims), initial
-        )
+        if standardize_dtype(x.dtype) == "bool":
+            x = tf.reduce_any(x, axis=axis, keepdims=keepdims)
+            x = tf.math.maximum(tf.cast(x, "int32"), tf.cast(initial, "int32"))
+            return tf.cast(x, "bool")
+        else:
+            x = tf.reduce_max(x, axis=axis, keepdims=keepdims)
+            return tf.math.maximum(x, initial)
 
     # TensorFlow returns -inf by default for an empty list, but for consistency
     # with other backends and the numpy API we want to throw in this case.
     if tf.executing_eagerly():
         size_x = size(x)
         tf.assert_greater(
             size_x,
             tf.constant(0, dtype=size_x.dtype),
             message="Cannot compute the max of an empty tensor.",
         )
 
-    return tfnp.max(x, axis=axis, keepdims=keepdims)
+    if standardize_dtype(x.dtype) == "bool":
+        return tf.reduce_any(x, axis=axis, keepdims=keepdims)
+    else:
+        return tf.reduce_max(x, axis=axis, keepdims=keepdims)
 
 
 def ones(shape, dtype=None):
     dtype = dtype or config.floatx()
     return tf.ones(shape, dtype=dtype)
 
 
 def zeros(shape, dtype=None):
     dtype = dtype or config.floatx()
     return tf.zeros(shape, dtype=dtype)
 
 
 @sparse.elementwise_unary
 def absolute(x):
+    x = convert_to_tensor(x)
     # uintx and bool are always non-negative
     dtype = standardize_dtype(x.dtype)
     if "uint" in dtype or dtype == "bool":
         return x
     return tf.abs(x)
 
 
-@sparse.elementwise_unary
 def abs(x):
     return absolute(x)
 
 
 def all(x, axis=None, keepdims=False):
     x = tf.cast(x, "bool")
     return tf.reduce_all(x, axis=axis, keepdims=keepdims)
@@ -646,16 +655,14 @@
     if axis is None:
         return tf.concat([tf.reshape(x1, [-1]), tf.reshape(x2, [-1])], axis=0)
     else:
         return tf.concat([x1, x2], axis=axis)
 
 
 def arange(start, stop=None, step=1, dtype=None):
-    # tfnp.arange has trouble with dynamic Tensors in compiled function.
-    # tf.range does not.
     if dtype is None:
         dtypes_to_resolve = [
             getattr(start, "dtype", type(start)),
             getattr(step, "dtype", type(step)),
         ]
         if stop is not None:
             dtypes_to_resolve.append(getattr(stop, "dtype", type(stop)))
@@ -741,24 +748,43 @@
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = tf.cast(x, dtype)
     return tf.math.atanh(x)
 
 
-def argmax(x, axis=None):
+def _keepdims(x, y, axis):
+    if axis is None:
+        shape = [1 for _ in range(len(x.shape))]
+    else:
+        shape = [tf.shape[i] for i in range(len(x.shape))]
+        for axis in tree.flatten(axis):
+            shape[axis] = 1
+    y = tf.reshape(y, shape)
+    return y
+
+
+def argmax(x, axis=None, keepdims=False):
+    _x = x
     if axis is None:
         x = tf.reshape(x, [-1])
-    return tf.cast(tf.argmax(x, axis=axis), dtype="int32")
+    y = tf.cast(tf.argmax(x, axis=axis), dtype="int32")
+    if keepdims:
+        y = _keepdims(_x, y, axis)
+    return y
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
+    _x = x
     if axis is None:
         x = tf.reshape(x, [-1])
-    return tf.cast(tf.argmin(x, axis=axis), dtype="int32")
+    y = tf.cast(tf.argmin(x, axis=axis), dtype="int32")
+    if keepdims:
+        y = _keepdims(_x, y, axis)
+    return y
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "bool":
         x = tf.cast(x, "uint8")
 
@@ -774,35 +800,47 @@
 
 def array(x, dtype=None):
     return convert_to_tensor(x, dtype=dtype)
 
 
 def average(x, axis=None, weights=None):
     x = convert_to_tensor(x)
-    axis = to_tuple_or_list(axis)
-    dtypes_to_resolve = [x.dtype, float]
-    if weights is not None:
+
+    if weights is None:  # Treat all weights as 1
+        dtype = dtypes.result_type(x.dtype, float)
+        x = tf.cast(x, dtype)
+        avg = tf.reduce_mean(x, axis=axis)
+    else:
         weights = convert_to_tensor(weights)
-        dtypes_to_resolve.append(weights.dtype)
-    result_dtype = dtypes.result_type(*dtypes_to_resolve)
-    compute_dtype = result_dtype
-    # TODO: since tfnp.average incorrectly promote bfloat16 to float64, we
-    # need to cast to float32 first and then cast back to bfloat16
-    if compute_dtype == "bfloat16":
-        compute_dtype = "float32"
-    x = tf.cast(x, compute_dtype)
-    if weights is not None:
-        weights = tf.cast(weights, compute_dtype)
-    if axis is None:
-        x = tfnp.average(x, weights=weights, axis=None)
-        return tf.cast(x, result_dtype)
-    for a in axis:
-        # `tfnp.average` does not handle multiple axes.
-        x = tfnp.average(x, weights=weights, axis=a)
-    return tf.cast(x, result_dtype)
+        dtype = dtypes.result_type(x.dtype, weights.dtype, float)
+        x = tf.cast(x, dtype)
+        weights = tf.cast(weights, dtype)
+
+        def _rank_equal_case():
+            weights_sum = tf.reduce_sum(weights, axis=axis)
+            return tf.reduce_sum(x * weights, axis=axis) / weights_sum
+
+        def _rank_not_equal_case():
+            weights_sum = tf.reduce_sum(weights)
+            axes = tf.convert_to_tensor([[axis], [0]])
+            return tf.tensordot(x, weights, axes) / weights_sum
+
+        if axis is None:
+            avg = _rank_equal_case()
+        else:
+            # We condition on rank rather than shape equality, because if we do
+            # the latter, when the shapes are partially unknown but the ranks
+            # are known and different, np_utils.cond will run shape checking on
+            # the true branch, which will raise a shape-checking error.
+            avg = tf.cond(
+                tf.equal(tf.rank(x), tf.rank(weights)),
+                _rank_equal_case,
+                _rank_not_equal_case,
+            )
+    return avg
 
 
 def broadcast_to(x, shape):
     return tf.broadcast_to(x, shape)
 
 
 @sparse.elementwise_unary
@@ -853,15 +891,16 @@
 @sparse.elementwise_unary
 def conj(x):
     return tf.math.conj(x)
 
 
 @sparse.elementwise_unary
 def copy(x):
-    return tfnp.copy(x)
+    x = convert_to_tensor(x)
+    return tf.identity(x)
 
 
 @sparse.densifying_unary(1)
 def cos(x):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
@@ -885,25 +924,60 @@
 def count_nonzero(x, axis=None):
     return tf.math.count_nonzero(x, axis=axis, dtype="int32")
 
 
 def cross(x1, x2, axisa=-1, axisb=-1, axisc=-1, axis=None):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
+    if axis is not None:
+        axisa = axis
+        axisb = axis
+        axisc = axis
+    x1 = moveaxis(x1, axisa, -1)
+    x2 = moveaxis(x2, axisb, -1)
+
     dtype = dtypes.result_type(x1.dtype, x2.dtype)
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
-    return tfnp.cross(
-        x1,
-        x2,
-        axisa=axisa,
-        axisb=axisb,
-        axisc=axisc,
-        axis=axis,
+
+    def maybe_pad_zeros(x, size_of_last_dim):
+        def pad_zeros(x):
+            return tf.pad(
+                x,
+                tf.concat(
+                    [
+                        tf.zeros([tf.rank(x) - 1, 2], "int32"),
+                        tf.constant([[0, 1]], "int32"),
+                    ],
+                    axis=0,
+                ),
+            )
+
+        return tf.cond(
+            tf.equal(size_of_last_dim, 2), lambda: pad_zeros(x), lambda: x
+        )
+
+    x1_dim = tf.shape(x1)[-1]
+    x2_dim = tf.shape(x2)[-1]
+    x1 = maybe_pad_zeros(x1, x1_dim)
+    x2 = maybe_pad_zeros(x2, x2_dim)
+
+    # Broadcast each other
+    shape = tf.shape(x1)
+    shape = tf.broadcast_dynamic_shape(shape, tf.shape(x2))
+    x1 = tf.broadcast_to(x1, shape)
+    x2 = tf.broadcast_to(x2, shape)
+
+    c = tf.linalg.cross(x1, x2)
+    c = tf.cond(
+        (x1_dim == 2) & (x2_dim == 2),
+        lambda: c[..., 2],
+        lambda: moveaxis(c, -1, axisc),
     )
+    return c
 
 
 def cumprod(x, axis=None, dtype=None):
     x = convert_to_tensor(x, dtype=dtype)
     # tf.math.cumprod doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = tf.cast(x, "int32")
@@ -921,28 +995,78 @@
     if axis is None:
         x = tf.reshape(x, [-1])
         axis = 0
     return tf.math.cumsum(x, axis=axis)
 
 
 def diag(x, k=0):
-    return tfnp.diag(x, k=k)
+    x = convert_to_tensor(x)
+    if len(x.shape) == 1:
+        return tf.cond(
+            tf.equal(tf.size(x), 0),
+            lambda: tf.zeros([builtins.abs(k), builtins.abs(k)], dtype=x.dtype),
+            lambda: tf.linalg.diag(x, k=k),
+        )
+    elif len(x.shape) == 2:
+        return diagonal(x, offset=k)
+    else:
+        raise ValueError(f"`x` must be 1d or 2d. Received: x.shape={x.shape}")
 
 
 def diagonal(x, offset=0, axis1=0, axis2=1):
-    return tfnp.diagonal(
-        x,
-        offset=offset,
-        axis1=axis1,
-        axis2=axis2,
+    x = convert_to_tensor(x)
+    x_rank = x.ndim
+    if (
+        offset == 0
+        and (axis1 == x_rank - 2 or axis1 == -2)
+        and (axis2 == x_rank - 1 or axis2 == -1)
+    ):
+        return tf.linalg.diag_part(x)
+
+    x = moveaxis(x, (axis1, axis2), (-2, -1))
+    x_shape = tf.shape(x)
+
+    def _zeros():
+        return tf.zeros(tf.concat([x_shape[:-1], [0]], 0), dtype=x.dtype)
+
+    x, offset = tf.cond(
+        tf.logical_or(
+            tf.less_equal(offset, -1 * x_shape[-2]),
+            tf.greater_equal(offset, x_shape[-1]),
+        ),
+        _zeros,
+        lambda: (x, offset),
     )
+    return tf.linalg.diag_part(x, k=offset)
 
 
 def diff(a, n=1, axis=-1):
-    return tfnp.diff(a, n=n, axis=axis)
+    a = convert_to_tensor(a)
+    if n == 0:
+        return a
+    elif n < 0:
+        raise ValueError(f"Order `n` must be non-negative. Received n={n}")
+    elif a.ndim == 0:
+        raise ValueError(
+            "`diff` requires input that is at least one dimensional. "
+            f"Received: a={a}"
+        )
+    axis = canonicalize_axis(axis, a.ndim)
+    slice1 = [slice(None)] * a.ndim
+    slice2 = [slice(None)] * a.ndim
+    slice1[axis] = slice(1, None)
+    slice2[axis] = slice(None, -1)
+    slice1_tuple = tuple(slice1)
+    slice2_tuple = tuple(slice2)
+    for _ in range(n):
+        if standardize_dtype(a.dtype) == "bool":
+            a = tf.not_equal(a[slice1_tuple], a[slice2_tuple])
+        else:
+            a = tf.subtract(a[slice1_tuple], a[slice2_tuple])
+    return a
 
 
 def digitize(x, bins):
     x = convert_to_tensor(x)
     bins = list(bins)
 
     # bins must be float type
@@ -1018,15 +1142,17 @@
 
 def expand_dims(x, axis):
     x = convert_to_tensor(x)
     axis = to_tuple_or_list(axis)
     out_ndim = len(x.shape) + len(axis)
     axis = sorted([canonicalize_axis(a, out_ndim) for a in axis])
     if isinstance(x, tf.SparseTensor):
-        from keras.src.ops.operation_utils import compute_expand_dims_output_shape
+        from keras.src.ops.operation_utils import (
+            compute_expand_dims_output_shape,
+        )
 
         output_shape = compute_expand_dims_output_shape(x.shape, axis)
         for a in axis:
             x = tf.sparse.expand_dims(x, a)
         x.set_shape(output_shape)
         return x
     for a in axis:
@@ -1127,33 +1253,30 @@
         return tf.abs(x1 - x2) <= (1e-08 + 1e-05 * tf.abs(x2))
     else:
         return tf.equal(x1, x2)
 
 
 @sparse.densifying_unary(True)
 def isfinite(x):
-    # `tfnp.isfinite` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.ones(x.shape, tf.bool)
     return tf.math.is_finite(x)
 
 
 def isinf(x):
-    # `tfnp.isinf` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.zeros(x.shape, tf.bool)
     return tf.math.is_inf(x)
 
 
 def isnan(x):
-    # `tfnp.isnan` requires `enable_numpy_behavior`, so we reimplement it.
     x = convert_to_tensor(x)
     dtype_as_dtype = tf.as_dtype(x.dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return tf.zeros(x.shape, tf.bool)
     return tf.math.is_nan(x)
 
 
@@ -1181,23 +1304,45 @@
     if dtype is None:
         dtypes_to_resolve = [
             getattr(start, "dtype", type(start)),
             getattr(stop, "dtype", type(stop)),
             float,
         ]
         dtype = dtypes.result_type(*dtypes_to_resolve)
-    return tfnp.linspace(
-        start,
-        stop,
-        num=num,
-        endpoint=endpoint,
-        retstep=retstep,
-        dtype=dtype,
-        axis=axis,
-    )
+    else:
+        dtype = standardize_dtype(dtype)
+    start = convert_to_tensor(start, dtype=dtype)
+    stop = convert_to_tensor(stop, dtype=dtype)
+    if num < 0:
+        raise ValueError(
+            f"`num` must be a non-negative integer. Received: num={num}"
+        )
+    step = tf.convert_to_tensor(np.nan)
+    if endpoint:
+        result = tf.linspace(start, stop, num, axis=axis)
+        if num > 1:
+            step = (stop - start) / (num - 1)
+    else:
+        # tf.linspace doesn't support endpoint=False, so we manually handle it
+        if num > 0:
+            step = (stop - start) / num
+        if num > 1:
+            new_stop = tf.cast(stop, step.dtype) - step
+            start = tf.cast(start, new_stop.dtype)
+            result = tf.linspace(start, new_stop, num, axis=axis)
+        else:
+            result = tf.linspace(start, stop, num, axis=axis)
+    if dtype is not None:
+        if "int" in dtype:
+            result = tf.floor(result)
+        result = tf.cast(result, dtype)
+    if retstep:
+        return (result, step)
+    else:
+        return result
 
 
 @sparse.densifying_unary(-np.inf)
 def log(x):
     x = convert_to_tensor(x)
     dtype = (
         config.floatx()
@@ -1246,17 +1391,14 @@
 
 def logaddexp(x1, x2):
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     dtype = dtypes.result_type(x1.dtype, x2.dtype, float)
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
-
-    # Below is the same implementation as tfnp.logaddexp using all native
-    # ops to prevent incorrect promotion of bfloat16.
     delta = x1 - x2
     return tf.where(
         tf.math.is_nan(delta),
         x1 + x2,
         tf.maximum(x1, x2) + tf.math.log1p(tf.math.exp(-tf.abs(delta))),
     )
 
@@ -1275,32 +1417,23 @@
 def logical_or(x1, x2):
     x1 = tf.cast(x1, "bool")
     x2 = tf.cast(x2, "bool")
     return tf.logical_or(x1, x2)
 
 
 def logspace(start, stop, num=50, endpoint=True, base=10, dtype=None, axis=0):
-    if dtype is None:
-        dtypes_to_resolve = [
-            getattr(start, "dtype", type(start)),
-            getattr(stop, "dtype", type(stop)),
-            float,
-        ]
-        dtype = dtypes.result_type(*dtypes_to_resolve)
-    start = tf.cast(start, dtype)
-    stop = tf.cast(stop, dtype)
-    return tfnp.logspace(
-        start,
-        stop,
+    result = linspace(
+        start=start,
+        stop=stop,
         num=num,
         endpoint=endpoint,
-        base=base,
         dtype=dtype,
         axis=axis,
     )
+    return tf.pow(tf.cast(base, result.dtype), result)
 
 
 @sparse.elementwise_binary_union(tf.sparse.maximum, densify_mixed=True)
 def maximum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
@@ -1320,32 +1453,40 @@
 
 def meshgrid(*x, indexing="xy"):
     return tf.meshgrid(*x, indexing=indexing)
 
 
 def min(x, axis=None, keepdims=False, initial=None):
     x = convert_to_tensor(x)
+
     # The TensorFlow numpy API implementation doesn't support `initial` so we
     # handle it manually here.
     if initial is not None:
-        return tf.math.minimum(
-            tfnp.min(x, axis=axis, keepdims=keepdims), initial
-        )
+        if standardize_dtype(x.dtype) == "bool":
+            x = tf.reduce_all(x, axis=axis, keepdims=keepdims)
+            x = tf.math.minimum(tf.cast(x, "int32"), tf.cast(initial, "int32"))
+            return tf.cast(x, "bool")
+        else:
+            x = tf.reduce_min(x, axis=axis, keepdims=keepdims)
+        return tf.math.minimum(x, initial)
 
     # TensorFlow returns inf by default for an empty list, but for consistency
     # with other backends and the numpy API we want to throw in this case.
     if tf.executing_eagerly():
         size_x = size(x)
         tf.assert_greater(
             size_x,
             tf.constant(0, dtype=size_x.dtype),
             message="Cannot compute the min of an empty tensor.",
         )
 
-    return tfnp.min(x, axis=axis, keepdims=keepdims)
+    if standardize_dtype(x.dtype) == "bool":
+        return tf.reduce_all(x, axis=axis, keepdims=keepdims)
+    else:
+        return tf.reduce_min(x, axis=axis, keepdims=keepdims)
 
 
 @sparse.elementwise_binary_union(tf.sparse.minimum, densify_mixed=True)
 def minimum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
@@ -1367,33 +1508,54 @@
         dtype = "int32"
     x1 = tf.cast(x1, dtype)
     x2 = tf.cast(x2, dtype)
     return tf.math.mod(x1, x2)
 
 
 def moveaxis(x, source, destination):
-    return tfnp.moveaxis(x, source=source, destination=destination)
+    x = convert_to_tensor(x)
+
+    _source = to_tuple_or_list(source)
+    _destination = to_tuple_or_list(destination)
+    _source = tuple(canonicalize_axis(i, x.ndim) for i in _source)
+    _destination = tuple(canonicalize_axis(i, x.ndim) for i in _destination)
+    if len(_source) != len(_destination):
+        raise ValueError(
+            "Inconsistent number of `source` and `destination`. "
+            f"Received: source={source}, destination={destination}"
+        )
+    # Directly return x if no movement is required
+    if _source == _destination:
+        return x
+    perm = [i for i in range(x.ndim) if i not in _source]
+    for dest, src in sorted(zip(_destination, _source)):
+        perm.insert(dest, src)
+    return tf.transpose(x, perm)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
 
     dtype = x.dtype
     dtype_as_dtype = tf.as_dtype(dtype)
     if dtype_as_dtype.is_integer or not dtype_as_dtype.is_numeric:
         return x
 
-    # Replace NaN with 0
-    x = tf.where(tf.math.is_nan(x), tf.constant(0, dtype), x)
+    # Replace NaN with `nan`
+    x = tf.where(tf.math.is_nan(x), tf.constant(nan, dtype), x)
 
-    # Replace positive infinity with dtype.max
-    x = tf.where(tf.math.is_inf(x) & (x > 0), tf.constant(dtype.max, dtype), x)
-
-    # Replace negative infinity with dtype.min
-    x = tf.where(tf.math.is_inf(x) & (x < 0), tf.constant(dtype.min, dtype), x)
+    # Replace positive infinity with `posinf` or `dtype.max`
+    if posinf is None:
+        posinf = dtype.max
+    x = tf.where(tf.math.is_inf(x) & (x > 0), tf.constant(posinf, dtype), x)
+
+    # Replace negative infinity with `neginf` or `dtype.min`
+    if neginf is None:
+        neginf = dtype.min
+    x = tf.where(tf.math.is_inf(x) & (x < 0), tf.constant(neginf, dtype), x)
 
     return x
 
 
 def ndim(x):
     x = convert_to_tensor(x)
     return x.ndim
@@ -1590,16 +1752,14 @@
 @sparse.densifying_unary(np.inf)
 def reciprocal(x):
     x = convert_to_tensor(x)
     return tf.math.reciprocal(x)
 
 
 def repeat(x, repeats, axis=None):
-    # tfnp.repeat has trouble with dynamic Tensors in compiled function.
-    # tf.repeat does not.
     x = convert_to_tensor(x)
     # TODO: tf.repeat doesn't support uint16
     if standardize_dtype(x.dtype) == "uint16":
         x = tf.cast(x, "uint32")
         return tf.cast(tf.repeat(x, repeats, axis=axis), "uint16")
     return tf.repeat(x, repeats, axis=axis)
 
@@ -1615,15 +1775,22 @@
         output = tf.sparse.reshape(x, newshape)
         output.set_shape(output_shape)
         return output
     return tf.reshape(x, newshape)
 
 
 def roll(x, shift, axis=None):
-    return tfnp.roll(x, shift, axis=axis)
+    x = convert_to_tensor(x)
+    if axis is not None:
+        return tf.roll(x, shift=shift, axis=axis)
+
+    # If axis is None, the roll happens as a 1-d tensor.
+    original_shape = tf.shape(x)
+    x = tf.roll(tf.reshape(x, [-1]), shift, 0)
+    return tf.reshape(x, original_shape)
 
 
 @sparse.elementwise_unary
 def sign(x):
     x = convert_to_tensor(x)
     ori_dtype = standardize_dtype(x.dtype)
     # TODO: tf.sign doesn't support uint8, uint16, uint32
@@ -1670,22 +1837,20 @@
     return tf.sort(x, axis=axis)
 
 
 def split(x, indices_or_sections, axis=0):
     if not isinstance(indices_or_sections, int):
         # `tf.split` requires `num_or_size_splits`, so we need to convert
         # `indices_or_sections` to the appropriate format.
-        # The following implementation offers better compatibility for the
-        # tensor argument `indices_or_sections` than original `tfnp.split`.
         total_size = x.shape[axis]
         indices_or_sections = convert_to_tensor(indices_or_sections)
         start_size = indices_or_sections[0:1]
         end_size = total_size - indices_or_sections[-1:]
         num_or_size_splits = tf.concat(
-            [start_size, tfnp.diff(indices_or_sections), end_size], axis=0
+            [start_size, diff(indices_or_sections), end_size], axis=0
         )
     else:
         num_or_size_splits = indices_or_sections
     return tf.split(x, num_or_size_splits, axis=axis)
 
 
 def stack(x, axis=0):
@@ -1701,51 +1866,135 @@
     ori_dtype = standardize_dtype(x.dtype)
     if "int" in ori_dtype or ori_dtype == "bool":
         x = tf.cast(x, config.floatx())
     return tf.math.reduce_std(x, axis=axis, keepdims=keepdims)
 
 
 def swapaxes(x, axis1, axis2):
-    return tfnp.swapaxes(x, axis1=axis1, axis2=axis2)
+    x = convert_to_tensor(x)
+
+    if (
+        x.shape.rank is not None
+        and isinstance(axis1, int)
+        and isinstance(axis2, int)
+    ):
+        # This branch makes sure `perm` is statically known, to avoid a
+        # not-compile-time-constant XLA error.
+        axis1 = canonicalize_axis(axis1, x.ndim)
+        axis2 = canonicalize_axis(axis2, x.ndim)
+
+        # Directly return x if no movement is required
+        if axis1 == axis2:
+            return x
+
+        perm = list(range(x.ndim))
+        perm[axis1] = axis2
+        perm[axis2] = axis1
+    else:
+        x_rank = tf.rank(x)
+        axis1 = tf.where(axis1 < 0, tf.add(axis1, x_rank), axis1)
+        axis2 = tf.where(axis2 < 0, tf.add(axis2, x_rank), axis2)
+        perm = tf.range(x_rank)
+        perm = tf.tensor_scatter_nd_update(
+            perm, [[axis1], [axis2]], [axis2, axis1]
+        )
+    return tf.transpose(x, perm)
 
 
 def take(x, indices, axis=None):
     if isinstance(indices, tf.SparseTensor):
         if x.dtype not in (tf.float16, tf.float32, tf.float64, tf.bfloat16):
             warnings.warn(
                 "`take` with the TensorFlow backend does not support "
                 f"`x.dtype={x.dtype}` when `indices` is a sparse tensor; "
                 "densifying `indices`."
             )
-            return tfnp.take(
-                x, convert_to_tensor(indices, sparse=False), axis=axis
-            )
+            return take(x, convert_to_tensor(indices, sparse=False), axis=axis)
         if axis is None:
             x = tf.reshape(x, (-1,))
         elif axis != 0:
             warnings.warn(
                 "`take` with the TensorFlow backend does not support "
                 f"`axis={axis}` when `indices` is a sparse tensor; "
                 "densifying `indices`."
             )
-            return tfnp.take(
-                x, convert_to_tensor(indices, sparse=False), axis=axis
-            )
+            return take(x, convert_to_tensor(indices, sparse=False), axis=axis)
         output = tf.nn.safe_embedding_lookup_sparse(
             embedding_weights=tf.convert_to_tensor(x),
             sparse_ids=tf.sparse.expand_dims(indices, axis=-1),
             default_id=0,
         )
         output.set_shape(indices.shape + output.shape[len(indices.shape) :])
         return output
-    return tfnp.take(x, indices, axis=axis)
+
+    x = convert_to_tensor(x)
+    indices = convert_to_tensor(indices)
+    if axis is None:
+        x = tf.reshape(x, [-1])
+        axis = 0
+    # Correct the indices using "fill" mode which is the same as in jax
+    indices = tf.where(
+        indices < 0,
+        indices + tf.cast(tf.shape(x)[axis], indices.dtype),
+        indices,
+    )
+    return tf.gather(x, indices, axis=axis)
 
 
 def take_along_axis(x, indices, axis=None):
-    return tfnp.take_along_axis(x, indices, axis=axis)
+    x = convert_to_tensor(x)
+    indices = convert_to_tensor(indices, "int64")
+    if axis is None:
+        if indices.ndim != 1:
+            raise ValueError(
+                "`indices` must be 1D if axis=None. "
+                f"Received: indices.shape={indices.shape}"
+            )
+        return take_along_axis(tf.reshape(x, [-1]), indices, 0)
+    rank = tf.rank(x)
+    static_axis = axis
+    axis = axis + rank if axis < 0 else axis
+
+    # Broadcast shapes to match, ensure that the axis of interest is not
+    # broadcast.
+    x_shape_original = tf.shape(x, out_type=indices.dtype)
+    indices_shape_original = tf.shape(indices, out_type=indices.dtype)
+    x_shape = tf.tensor_scatter_nd_update(x_shape_original, [[axis]], [1])
+    indices_shape = tf.tensor_scatter_nd_update(
+        indices_shape_original, [[axis]], [1]
+    )
+    broadcasted_shape = tf.broadcast_dynamic_shape(x_shape, indices_shape)
+    x_shape = tf.tensor_scatter_nd_update(
+        broadcasted_shape, [[axis]], [x_shape_original[axis]]
+    )
+    indices_shape = tf.tensor_scatter_nd_update(
+        broadcasted_shape, [[axis]], [indices_shape_original[axis]]
+    )
+    x = tf.broadcast_to(x, x_shape)
+    indices = tf.broadcast_to(indices, indices_shape)
+
+    # Save indices shape so we can restore it later.
+    possible_result_shape = indices.shape
+
+    # Correct the indices using "fill" mode which is the same as in jax
+    indices = tf.where(indices < 0, indices + x_shape[static_axis], indices)
+
+    x = swapaxes(x, static_axis, -1)
+    indices = swapaxes(indices, static_axis, -1)
+
+    x_shape = tf.shape(x)
+    x = tf.reshape(x, [-1, x_shape[-1]])
+    indices_shape = tf.shape(indices)
+    indices = tf.reshape(indices, [-1, indices_shape[-1]])
+
+    result = tf.gather(x, indices, batch_dims=1)
+    result = tf.reshape(result, indices_shape)
+    result = swapaxes(result, static_axis, -1)
+    result.set_shape(possible_result_shape)
+    return result
 
 
 @sparse.elementwise_unary
 def tan(x):
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
@@ -1775,15 +2024,14 @@
     x1 = tf.cast(x1, compute_dtype)
     x2 = tf.cast(x2, compute_dtype)
     return tf.cast(tf.tensordot(x1, x2, axes=axes), dtype=result_dtype)
 
 
 @sparse.elementwise_unary
 def round(x, decimals=0):
-    # `tfnp.round` requires `enable_numpy_behavior`, so we reimplement it.
     if decimals == 0:
         return tf.round(x)
     x_dtype = x.dtype
     if tf.as_dtype(x_dtype).is_integer:
         # int
         if decimals > 0:
             return x
@@ -1796,15 +2044,14 @@
     x = tf.multiply(x, factor)
     x = tf.round(x)
     x = tf.divide(x, factor)
     return tf.cast(x, x_dtype)
 
 
 def tile(x, repeats):
-    # The TFNP implementation is buggy, we roll our own.
     x = convert_to_tensor(x)
     repeats = tf.reshape(convert_to_tensor(repeats, dtype="int32"), [-1])
     repeats_size = tf.size(repeats)
     repeats = tf.pad(
         repeats,
         [[tf.maximum(x.shape.rank - repeats_size, 0), 0]],
         constant_values=1,
@@ -1819,20 +2066,47 @@
 
 
 def trace(x, offset=0, axis1=0, axis2=1):
     x = convert_to_tensor(x)
     dtype = standardize_dtype(x.dtype)
     if dtype not in ("int64", "uint32", "uint64"):
         dtype = dtypes.result_type(dtype, "int32")
-    return tfnp.trace(x, offset=offset, axis1=axis1, axis2=axis2, dtype=dtype)
+    x_shape = tf.shape(x)
+    x = moveaxis(x, (axis1, axis2), (-2, -1))
+    # Mask out the diagonal and reduce.
+    x = tf.where(
+        eye(x_shape[axis1], x_shape[axis2], k=offset, dtype="bool"),
+        x,
+        tf.zeros_like(x),
+    )
+    # The output dtype is set to "int32" if the input dtype is "bool"
+    if standardize_dtype(x.dtype) == "bool":
+        x = tf.cast(x, "int32")
+    return tf.cast(tf.reduce_sum(x, axis=(-2, -1)), dtype)
 
 
 def tri(N, M=None, k=0, dtype=None):
-    dtype = dtype or config.floatx()
-    return tfnp.tri(N, M=M, k=k, dtype=dtype)
+    M = M if M is not None else N
+    dtype = standardize_dtype(dtype or config.floatx())
+    if k < 0:
+        lower = -k - 1
+        if lower > N:
+            r = tf.zeros([N, M], dtype=dtype)
+        else:
+            o = tf.ones([N, M], dtype="bool")
+            r = tf.cast(
+                tf.logical_not(tf.linalg.band_part(o, lower, -1)), dtype=dtype
+            )
+    else:
+        o = tf.ones([N, M], dtype=dtype)
+        if k > M:
+            r = o
+        else:
+            r = tf.linalg.band_part(o, -1, k)
+    return r
 
 
 def tril(x, k=0):
     x = convert_to_tensor(x)
 
     if k >= 0:
         return tf.linalg.band_part(x, -1, k)
@@ -1879,14 +2153,33 @@
     dtype_set = set([getattr(x, "dtype", type(x)) for x in xs])
     if len(dtype_set) > 1:
         dtype = dtypes.result_type(*dtype_set)
         xs = tree.map_structure(lambda x: convert_to_tensor(x, dtype), xs)
     return tf.concat(xs, axis=0)
 
 
+def _vmap_fn(fn, in_axes=0):
+    if in_axes != 0:
+        raise ValueError(
+            "Not supported with `vectorize()` with the TensorFlow backend."
+        )
+
+    @functools.wraps(fn)
+    def wrapped(x):
+        return tf.vectorized_map(fn, x)
+
+    return wrapped
+
+
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return vectorize_impl(
+        pyfunc, _vmap_fn, excluded=excluded, signature=signature
+    )
+
+
 def where(condition, x1, x2):
     condition = tf.cast(condition, "bool")
     if x1 is not None and x2 is not None:
         if not isinstance(x1, (int, float)):
             x1 = convert_to_tensor(x1)
         if not isinstance(x2, (int, float)):
             x2 = convert_to_tensor(x2)
@@ -2044,15 +2337,37 @@
             x, axis=axis, keepdims=keepdims, output_is_sparse=True
         )
     return tf.reduce_sum(x, axis=axis, keepdims=keepdims)
 
 
 def eye(N, M=None, k=0, dtype=None):
     dtype = dtype or config.floatx()
-    return tfnp.eye(N, M=M, k=k, dtype=dtype)
+    if not M:
+        M = N
+    # Making sure N, M and k are `int`
+    N, M, k = int(N), int(M), int(k)
+    if k >= M or -k >= N:
+        # tf.linalg.diag will raise an error in this case
+        return zeros([N, M], dtype=dtype)
+    if k == 0:
+        return tf.eye(N, M, dtype=dtype)
+    # We need the precise length, otherwise tf.linalg.diag will raise an error
+    diag_len = builtins.min(N, M)
+    if k > 0:
+        if N >= M:
+            diag_len -= k
+        elif N + k > M:
+            diag_len = M - k
+    elif k <= 0:
+        if M >= N:
+            diag_len += k
+        elif M - k > N:
+            diag_len = N + k
+    diagonal_ = tf.ones([diag_len], dtype=dtype)
+    return tf.linalg.diag(diagonal=diagonal_, num_rows=N, num_cols=M, k=k)
 
 
 def floor_divide(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
     if not isinstance(x2, (int, float)):
         x2 = convert_to_tensor(x2)
@@ -2108,7 +2423,10 @@
         return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding="SAME"))
 
     x1 = tf.reshape(x1, (1, x1_len, 1))
     x2 = tf.reshape(x2, (x2_len, 1, 1))
 
     return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
 
+
+def select(condlist, choicelist, default=0):
+    return tf.experimental.numpy.select(condlist, choicelist, default=default)
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/optimizer.py` & `keras-3.3.0/keras/src/backend/tensorflow/optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,20 +124,23 @@
         )
 
     def _distributed_tf_update_step(
         self, distribution, grads_and_vars, learning_rate
     ):
         grads_and_vars = self._all_reduce_sum_gradients(grads_and_vars)
 
-        def apply_grad_to_update_var(var, grad):
+        def apply_grad_to_update_var(var, grad, learning_rate):
             return self.update_step(grad, var, learning_rate)
 
         for grad, var in grads_and_vars:
             distribution.extended.update(
-                var, apply_grad_to_update_var, args=(grad,), group=False
+                var,
+                apply_grad_to_update_var,
+                args=(grad, learning_rate),
+                group=False,
             )
 
     def _all_reduce_sum_gradients(self, grads_and_vars):
         """Returns all-reduced gradients aggregated via summation.
 
         Args:
             grads_and_vars: List of (gradient, variable) pairs.
@@ -189,19 +192,19 @@
         for var, average_var in zip(
             trainable_variables, self._model_variables_moving_average
         ):
             self._distribution_strategy.extended.update(
                 var, lambda a, b: a.assign(b), args=(average_var,)
             )
 
-    def _backend_increment_gradient_accumulators(self, grads):
+    def _backend_increment_gradient_accumulators(self, grads, acc_grads):
         def update_accumulator(var, grad):
             var.assign(var + grad)
 
-        accumulators = [v.value for v in self._accumulated_gradients]
+        accumulators = [v.value for v in acc_grads]
 
         def _distributed_tf_increment_grad_acc(
             distribution, grads, accumulators
         ):
             for grad, var in zip(grads, accumulators):
                 distribution.extended.update(
                     var, update_accumulator, args=(grad,), group=False
@@ -245,8 +248,7 @@
         warnings.warn(
             "Gradients do not exist for variables %s when minimizing the "
             "loss. If you're using `model.compile()`, did you forget to "
             "provide a `loss` argument?",
             ([v.name for v in vars_with_empty_grads]),
         )
     return filtered
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/random.py` & `keras-3.3.0/keras/src/backend/tensorflow/random.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import tensorflow as tf
-from tensorflow.experimental import numpy as tfnp
 
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.config import floatx
 from keras.src.random.seed_generator import SeedGenerator
 from keras.src.random.seed_generator import draw_seed
 from keras.src.random.seed_generator import make_default_seed
 
@@ -83,20 +82,22 @@
         rate=rate,
         noise_shape=noise_shape,
         seed=seed,
     )
 
 
 def shuffle(x, axis=0, seed=None):
+    from keras.src.backend.tensorflow.numpy import swapaxes
+
     seed = tf_draw_seed(seed)
     if axis == 0:
         return tf.random.experimental.stateless_shuffle(x, seed=seed)
-    x = tfnp.swapaxes(x, axis1=0, axis2=axis)
+    x = swapaxes(x, axis1=0, axis2=axis)
     x = tf.random.experimental.stateless_shuffle(x, seed=seed)
-    x = tfnp.swapaxes(x, axis1=0, axis2=axis)
+    x = swapaxes(x, axis1=0, axis2=axis)
     return x
 
 
 def gamma(shape, alpha, dtype=None, seed=None):
     dtype = dtype or floatx()
     seed = tf_draw_seed(seed)
     # TODO: `tf.random.stateless_gamma` doesn't support bfloat16
@@ -181,8 +182,7 @@
         tf.random.stateless_gamma(
             shape=shape, seed=seed_2, alpha=beta, dtype=intemediate_dtype
         ),
         dtype,
     )
     sample = gamma_a / (gamma_a + gamma_b)
     return sample
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/rnn.py` & `keras-3.3.0/keras/src/backend/tensorflow/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import tensorflow as tf
 
-from keras.src.utils import tree
+from keras.src import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -965,8 +965,7 @@
         last_output = h
 
     # Match CPU return format
     if not return_sequences:
         outputs = tf.expand_dims(last_output, axis=0 if time_major else 1)
 
     return (last_output, outputs, [h, c])
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/sparse.py` & `keras-3.3.0/keras/src/backend/tensorflow/sparse.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 ones_bool = functools.partial(tf.ones, dtype=tf.bool)
 ones_int8 = functools.partial(tf.ones, dtype=tf.int8)
 zeros_int8 = functools.partial(tf.zeros, dtype=tf.int8)
 ones_like_int8 = functools.partial(tf.ones_like, dtype=tf.int8)
 zeros_like_int8 = functools.partial(tf.zeros_like, dtype=tf.int8)
 
 
-def empty_tensor(shape, dtype):
-    return tf.reshape(tf.convert_to_tensor((), dtype=dtype), shape=shape)
-
-
 def sparse_to_dense(x, default_value=None):
     x_shape = x.shape
+    if x_shape.rank == 0:
+        # Workaround for bug on GPU when sparse tensor represents a scalar.
+        if x.values.shape[0] == 0:
+            return tf.constant(default_value, dtype=x.dtype)
+        else:
+            return tf.reshape(x.values, ())
     x = tf.sparse.to_dense(x, default_value=default_value)
     x.set_shape(x_shape)
     return x
 
 
 def sparse_with_values(x, values):
     x_shape = x.shape
@@ -180,17 +182,17 @@
     intersection_extra_dim = tf.sets.intersection(
         tf.sparse.expand_dims(ones1, axis=-1),
         tf.sparse.expand_dims(ones2, axis=-1),
     )
 
     def empty_intersection():
         return (
-            empty_tensor((0, x1.shape.rank), dtype=tf.int64),
-            empty_tensor((0,), dtype=x1.values.dtype),
-            empty_tensor((0,), dtype=x2.values.dtype),
+            tf.zeros((0, x1.shape.rank), dtype=tf.int64),
+            tf.zeros((0,), dtype=x1.values.dtype),
+            tf.zeros((0,), dtype=x2.values.dtype),
         )
 
     def non_empty_intersection():
         intersection = tf.sparse.reshape(intersection_extra_dim, x1.dense_shape)
 
         # Compute the masks to remove indices in x1 and x2 that are not
         # in the intersection, then trim x1 and x2.
@@ -245,16 +247,16 @@
         axis=-1,
     )
     intersection_indices_count = tf.shape(intersection_indices)[0]
 
     def empty_intersection():
         return (
             intersection_indices,
-            empty_tensor((0,) + x1.values.shape[1:], x1.dtype),
-            empty_tensor((0,) + x2.values.shape[1:], x2.dtype),
+            tf.zeros((0,) + x1.values.shape[1:], x1.dtype),
+            tf.zeros((0,) + x2.values.shape[1:], x2.dtype),
         )
 
     def non_empty_intersection():
         # Re-gather sub parts of the values that are part of the intersection.
         def values_for_intersection(indices_expanded, indices_count, values):
             indices_indices = tf.scatter_nd(
                 indices_expanded,
@@ -774,8 +776,7 @@
             # x2 is a IndexedSlices.
             # Divisor is slices, densify to do the divisions by zero correctly.
             x2 = tf.convert_to_tensor(x2)
         # Default case, no SparseTensor and no IndexedSlices.
         return func(x1, x2)
 
     return sparse_wrapper
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/trackable.py` & `keras-3.3.0/keras/src/backend/tensorflow/trackable.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,7 @@
             name=name,
             # Allow the user to switch the Trackable which is tracked by this
             # name, since assigning a new variable to an attribute has
             # historically been fine (e.g. Adam did this).
             overwrite=True,
         )
     return value
-
```

### Comparing `keras-3.2.1/keras/src/backend/tensorflow/trainer.py` & `keras-3.3.0/keras/src/backend/tensorflow/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import contextlib
 import warnings
 
 import numpy as np
 import tensorflow as tf
-from packaging.version import Version
 from tensorflow.python.eager import context as tf_context
 
 from keras.src import callbacks as callbacks_module
 from keras.src import metrics as metrics_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TensorFlowTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
@@ -27,19 +26,14 @@
         # Model must be created under scope of DistStrat it will be trained
         # with.
         if tf.distribute.has_strategy():
             self._distribute_strategy = tf.distribute.get_strategy()
         else:
             self._distribute_strategy = None
 
-        self._distribute_reduction_method = None
-        self._supports_reduce_retracing = Version(tf.__version__) >= Version(
-            "2.9.0"
-        )
-
     @property
     def distribute_strategy(self):
         return self._distribute_strategy or tf.distribute.get_strategy()
 
     @property
     def distribute_reduction_method(self):
         return self._distribute_reduction_method or "auto"
@@ -106,30 +100,31 @@
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a single training step on a batch of data."""
             return self.train_step(data)
 
         if not self.run_eagerly:
-            kwargs = {"jit_compile": self.jit_compile}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data,
+                reduce_retracing=True,
+                jit_compile=self.jit_compile,
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_iterator(iterator):
             """Runs a single training step given a Dataset iterator."""
             data = next(iterator)
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="auto",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_iterator(iterator):
             for _ in range(self.steps_per_execution):
                 outputs = one_step_on_iterator(iterator)
@@ -137,47 +132,43 @@
 
         if self.steps_per_execution > 1:
             train_function = multi_step_on_iterator
         else:
             train_function = one_step_on_iterator
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            train_function = tf.function(train_function, **kwargs)
+            train_function = tf.function(train_function, reduce_retracing=True)
 
         self.train_function = train_function
 
     def make_test_function(self, force=False):
         if self.test_function is not None and not force:
             return self.test_function
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a single test step on a batch of data."""
             return self.test_step(data)
 
         if not self.run_eagerly and self.jit_compile:
-            kwargs = {"jit_compile": True}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data, reduce_retracing=True, jit_compile=True
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_iterator(iterator):
             """Runs a single test step given a Dataset iterator."""
             data = next(iterator)
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="auto",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_iterator(iterator):
             for _ in range(self.steps_per_execution):
                 outputs = one_step_on_iterator(iterator)
@@ -185,46 +176,42 @@
 
         if self.steps_per_execution > 1:
             test_function = multi_step_on_iterator
         else:
             test_function = one_step_on_iterator
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            test_function = tf.function(test_function, **kwargs)
+            test_function = tf.function(test_function, reduce_retracing=True)
 
         self.test_function = test_function
 
     def make_predict_function(self, force=False):
         if self.predict_function is not None and not force:
             return self.predict_function
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data(data):
             """Runs a predict test step on a batch of data."""
             return self.predict_step(data)
 
         if not self.run_eagerly and self.jit_compile:
-            kwargs = {"jit_compile": True}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-            one_step_on_data = tf.function(one_step_on_data, **kwargs)
+            one_step_on_data = tf.function(
+                one_step_on_data, reduce_retracing=True, jit_compile=True
+            )
 
         @tf.autograph.experimental.do_not_convert
         def one_step_on_data_distributed(data):
             data = data[0]
             outputs = self.distribute_strategy.run(
                 one_step_on_data, args=(data,)
             )
             outputs = reduce_per_replica(
                 outputs,
                 self.distribute_strategy,
-                reduction=self.distribute_reduction_method,
+                reduction="concat",
             )
             return outputs
 
         @tf.autograph.experimental.do_not_convert
         def multi_step_on_data(data):
             outputs = one_step_on_data_distributed(data[:1])
             for single_step_data in data[1:]:
@@ -236,19 +223,17 @@
 
         if self.steps_per_execution > 1:
             predict_function = multi_step_on_data
         else:
             predict_function = one_step_on_data_distributed
 
         if not self.run_eagerly:
-            kwargs = {}
-            if self._supports_reduce_retracing:
-                kwargs.update({"reduce_retracing": True})
-
-            predict_function = tf.function(predict_function, **kwargs)
+            predict_function = tf.function(
+                predict_function, reduce_retracing=True
+            )
 
         self.predict_function = predict_function
 
     @traceback_utils.filter_traceback
     def fit(
         self,
         x=None,
@@ -323,22 +308,21 @@
         for epoch in range(initial_epoch, epochs):
             self.reset_metrics()
             callbacks.on_epoch_begin(epoch)
             with epoch_iterator.catch_stop_iteration():
                 for step, iterator in epoch_iterator.enumerate_epoch():
                     callbacks.on_train_batch_begin(step)
                     logs = self.train_function(iterator)
-                    callbacks.on_train_batch_end(
-                        step, self._pythonify_logs(logs)
-                    )
+                    logs = self._pythonify_logs(logs)
+                    callbacks.on_train_batch_end(step, logs)
                     if self.stop_training:
                         break
 
-            # Override with model metrics instead of last step logs
-            epoch_logs = self.get_metrics_result()
+            # Override with model metrics instead of last step logs if needed.
+            epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
             ):
                 # Create EpochIterator for evaluation and cache it.
                 if getattr(self, "_eval_epoch_iterator", None) is None:
@@ -435,18 +419,19 @@
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         with epoch_iterator.catch_stop_iteration():
             for step, iterator in epoch_iterator.enumerate_epoch():
                 callbacks.on_test_batch_begin(step)
                 logs = self.test_function(iterator)
-                callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+                logs = self._pythonify_logs(logs)
+                callbacks.on_test_batch_end(step, logs)
                 if self.stop_evaluating:
                     break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
@@ -702,15 +687,15 @@
     which represents the values across all the replicas, `reduce_per_replica`
     attempts to "reduce" those values and returns the corresponding structure
     that represents only single values.
 
     Currently, `reduce_per_replica` is only used for reducing the metric results
     from `tf.distribute.Strategy.run()`. Depending on the underlying
     `Strategy` implementation, `values` may be a `PerReplica` object,
-     which can be thought of as a collection of values across the replicas,
+    which can be thought of as a collection of values across the replicas,
     or a `tf.Tensor`, if the strategy has already conducted the reduction
     for the downstream library.
 
     There are five possible outcomes of reduction:
 
     1) if the `values` is a structure of simple `tf.Tensor`s, meaning that
        reduction is not actually needed, `reduce_per_replica` returns the
@@ -729,53 +714,60 @@
        case, where each replica contain different values which are not
        synchronized.
     5) else, if `reduction="concat"`, then `reduce_per_replica`
        returns the concatenation of the values across the replicas, along the
        axis of dimension 0. This is used in the inference case (`predict()`).
 
     Args:
-      values: Structure of `PerReplica` objects or `tf.Tensor`s. `tf.Tensor`s
-        are returned as-is.
-      strategy: `tf.distribute.Strategy` object.
-      reduction: One of `"auto"`, `"first"`, `"concat"`, or `"sum"`.
-        `"auto"` will select `"first"` when used under a TPUStrategy, or
-        `"sum"` otherwise.
+        values: Structure of `PerReplica` objects or `tf.Tensor`s.
+            `tf.Tensor`s are returned as-is.
+        strategy: `tf.distribute.Strategy` object.
+        reduction: One of `"auto"`, `"first"`, `"concat"`, `"mean"`, or `"sum"`.
+            `"auto"` will select `"first"` when used under a TPUStrategy, or
+            `"mean"` otherwise.
 
     Returns:
-      Structure of `Tensor`s, representing the result of reduction.
-
-    Raises:
-      ValueError: if the reduction method is not supported.
+        Structure of `Tensor`s, representing the result of reduction.
     """
 
     if reduction == "auto":
-        reduction = "sum"  # Ignore TPU strategy which should default to "first"
+        if isinstance(strategy, tf.distribute.TPUStrategy):
+            reduction = "first"
+        else:
+            reduction = "mean"
 
     def _reduce(v):
         """Reduce a single `PerReplica` object."""
         if _collective_all_reduce_multi_worker(strategy):
             if reduction == "concat":
                 return _multi_worker_concat(v, strategy)
             elif reduction == "sum":
-                return strategy.reduce("SUM", v, axis=None)
+                return strategy.reduce("SUM", v)
+            elif reduction == "mean":
+                return strategy.reduce("MEAN", v, axis=0)
 
         if not _is_per_replica_instance(v):
             return v
         elif reduction == "first":
             return strategy.experimental_local_results(v)[0]
         elif reduction == "concat":
             if _is_tpu_multi_host(strategy):
                 return _tpu_multi_host_concat(v, strategy)
             else:
                 return concat(strategy.experimental_local_results(v))
         elif reduction == "sum":
             return tf.reduce_sum(strategy.experimental_local_results(v))
+        elif reduction == "mean":
+            return tf.reduce_mean(
+                strategy.experimental_local_results(v), axis=0
+            )
         else:
             raise ValueError(
-                '`reduction` must be "first", "concat", "sum", or "auto". '
+                "`reduction` must be one of "
+                '"first", "concat", "mean", "sum", or "auto". '
                 f"Received: reduction={reduction}."
             )
 
     return tree.map_structure(_reduce, values)
 
 
 def _multi_worker_concat(v, strategy):
@@ -910,8 +902,7 @@
     if constant_inner_dimensions == 0:
         constant_inner_shape = None
     else:
         constant_inner_shape = tensors[0].shape[-constant_inner_dimensions:]
     return tf.ragged.constant(
         [tensor.numpy() for tensor in tensors], inner_shape=constant_inner_shape
     ).merge_dims(0, 1)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/__init__.py` & `keras-3.3.0/keras/src/backend/torch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,8 +35,7 @@
 from keras.src.backend.torch.core import stop_gradient
 from keras.src.backend.torch.core import to_torch_dtype
 from keras.src.backend.torch.core import vectorized_map
 from keras.src.backend.torch.rnn import cudnn_ok
 from keras.src.backend.torch.rnn import gru
 from keras.src.backend.torch.rnn import lstm
 from keras.src.backend.torch.rnn import rnn
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/core.py` & `keras-3.3.0/keras/src/backend/torch/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import contextlib
 import os
 
 import ml_dtypes
 import numpy as np
 import torch
 
+from keras.src import tree
 from keras.src.backend.common import KerasVariable
 from keras.src.backend.common import global_state
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.dtypes import result_type
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.backend.config import floatx
-from keras.src.utils import tree
 
 SUPPORTS_SPARSE_TENSORS = False
 
 # Some operators such as 'aten::_foreach_mul_.Scalar'
 # are not currently implemented for the MPS device.
 # check https://github.com/pytorch/pytorch/issues/77764.
 if (
@@ -486,8 +486,7 @@
         grad_fn = ctx.grad_fn
         if grad_fn is None:
             raise ValueError("grad_fn must be provided for custom gradient")
         grads = grad_fn(*args, upstream=grad_output)
         if not isinstance(grads, tuple):
             grads = (grads,)
         return (None,) + grads
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/layer.py` & `keras-3.3.0/keras/src/backend/torch/layer.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,16 +9,17 @@
         # Do not track variables when in a stateless scope.
         # The variables are not initialized.
         if in_stateless_scope():
             return
         self._track_variables()
 
     def _track_variables(self):
-        self.torch_params = torch.nn.ParameterList(
-            [variable.value for variable in self.variables]
+        # Index given to ParameterDict must be a string
+        self.torch_params = torch.nn.ParameterDict(
+            {str(id(variable)): variable.value for variable in self.variables}
         )
 
     def parameters(self, recurse=True):
         if not hasattr(self, "torch_params"):
             self._track_variables()
         return torch.nn.Module.parameters(self, recurse=recurse)
 
@@ -35,7 +36,19 @@
         ):
             from keras.src.utils.torch_utils import TorchModuleWrapper
 
             if not isinstance(self, TorchModuleWrapper):
                 value = TorchModuleWrapper(value)
         return name, value
 
+    def _post_track_variable(self, variable):
+        if hasattr(self, "torch_params"):
+            # Index given to ParameterDict must be a string
+            key = str(id(variable))
+            if key not in self.torch_params:
+                self.torch_params[key] = variable.value
+
+    def _post_untrack_variable(self, variable):
+        if hasattr(self, "torch_params"):
+            # Index given to ParameterDict must be a string
+            key = str(id(variable))
+            self.torch_params.pop(key)
```

### Comparing `keras-3.2.1/keras/src/backend/torch/linalg.py` & `keras-3.3.0/keras/src/backend/torch/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,18 @@
     return torch.det(x)
 
 
 def eig(x):
     return torch.linalg.eig(x)
 
 
+def eigh(x):
+    return torch.linalg.eigh(x)
+
+
 def inv(x):
     return torch.linalg.inv(x)
 
 
 def lu_factor(x):
     LU, pivots = torch.linalg.lu_factor(x)
     # torch retuns pivots with 1-based indexing
@@ -64,8 +68,7 @@
 
 def svd(x, full_matrices=True, compute_uv=True):
     if not compute_uv:
         raise NotImplementedError(
             "`compute_uv=False` is not supported for torch backend."
         )
     return torch.linalg.svd(x, full_matrices=full_matrices)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/math.py` & `keras-3.3.0/keras/src/backend/torch/math.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,8 +433,7 @@
     x = convert_to_tensor(x)
     if standardize_dtype(x.dtype) == "int64":
         dtype = config.floatx()
     else:
         dtype = dtypes.result_type(x.dtype, float)
     x = cast(x, dtype)
     return torch.linalg.norm(x, ord=ord, dim=axis, keepdim=keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/nn.py` & `keras-3.3.0/keras/src/backend/jax/nn.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,471 +1,348 @@
-import torch
-import torch.nn.functional as tnn
+import jax
+import jax.experimental.sparse as jax_sparse
+import jax.numpy as jnp
+import numpy as np
+from jax import lax
+from jax import nn as jnn
 
 from keras.src.backend import standardize_data_format
 from keras.src.backend import standardize_dtype
 from keras.src.backend.common.backend_utils import (
-    compute_conv_transpose_padding_args_for_torch,
+    compute_conv_transpose_padding_args_for_jax,
 )
 from keras.src.backend.config import epsilon
-from keras.src.backend.torch.core import cast
-from keras.src.backend.torch.core import convert_to_tensor
-from keras.src.backend.torch.core import get_device
-from keras.src.backend.torch.numpy import expand_dims
-from keras.src.backend.torch.numpy import maximum
-from keras.src.backend.torch.numpy import where
-from keras.src.utils import tree
-from keras.src.utils.argument_validation import standardize_tuple
+from keras.src.backend.jax.core import cast
+from keras.src.backend.jax.core import convert_to_tensor
 
 
 def relu(x):
     x = convert_to_tensor(x)
-    return tnn.relu(x)
+    return jnn.relu(x)
 
 
 def relu6(x):
     x = convert_to_tensor(x)
-    return tnn.relu6(x)
+    return jnn.relu6(x)
 
 
 def sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.sigmoid(x)
+    return jnn.sigmoid(x)
 
 
 def tanh(x):
     x = convert_to_tensor(x)
-    return tnn.tanh(x)
+    return jnn.tanh(x)
 
 
 def softplus(x):
     x = convert_to_tensor(x)
-    return tnn.softplus(x)
+    return jnn.softplus(x)
 
 
 def softsign(x):
     x = convert_to_tensor(x)
-    return tnn.softsign(x)
+    return jnn.soft_sign(x)
 
 
 def silu(x):
     x = convert_to_tensor(x)
-    return tnn.silu(x)
+    return jnn.silu(x)
 
 
 def log_sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.logsigmoid(x)
+    return jnn.log_sigmoid(x)
 
 
 def leaky_relu(x, negative_slope=0.2):
     x = convert_to_tensor(x)
-    return tnn.leaky_relu(x, negative_slope=negative_slope)
+    return jnn.leaky_relu(x, negative_slope=negative_slope)
 
 
 def hard_sigmoid(x):
     x = convert_to_tensor(x)
-    return tnn.hardsigmoid(x)
+    return jnn.hard_sigmoid(x)
 
 
 def hard_silu(x):
     x = convert_to_tensor(x)
-    return tnn.hardswish(x)
+    return jnn.hard_silu(x)
 
 
 def elu(x, alpha=1.0):
     x = convert_to_tensor(x)
-    return tnn.elu(x, alpha)
+    return jnn.elu(x, alpha=alpha)
 
 
 def selu(x):
     x = convert_to_tensor(x)
-    return tnn.selu(x)
+    return jnn.selu(x)
 
 
 def gelu(x, approximate=True):
-    # TODO: torch.nn.gelu expects string approximate of `"none"` or `"tanh"`
     x = convert_to_tensor(x)
-    if approximate:
-        return tnn.gelu(x, approximate="tanh")
-    return tnn.gelu(x)
+    return jnn.gelu(x, approximate)
 
 
 def softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
-    # TODO: tnn.softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
-        x = cast(x, "float32")
-    if axis is None:
-        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
-        # We need this workaround for the reduction on every dim.
-        output = torch.reshape(x, [-1])
-        output = tnn.softmax(output, dim=-1)
-        output = torch.reshape(output, x.shape)
-    else:
-        output = tnn.softmax(x, dim=axis)
-    return cast(output, dtype)
+    return jnn.softmax(x, axis=axis)
 
 
 def log_softmax(x, axis=-1):
     x = convert_to_tensor(x)
-    dtype = standardize_dtype(x.dtype)
-    # TODO: tnn.log_softmax doesn't support float16 using cpu
-    if get_device() == "cpu" and standardize_dtype(x.dtype) == "float16":
-        x = cast(x, "float32")
-    if axis is None:
-        # Unlike numpy, PyTorch will handle axis=None as axis=-1.
-        # We need this workaround for the reduction on every dim.
-        output = torch.reshape(x, [-1])
-        output = tnn.log_softmax(output, dim=-1)
-        output = torch.reshape(output, x.shape)
-    else:
-        output = tnn.log_softmax(x, dim=axis)
-    return cast(output, dtype)
+    return jnn.log_softmax(x, axis=axis)
 
 
-def _compute_padding_length(
-    input_length, kernel_length, stride, dilation_rate=1
+def _convert_to_spatial_operand(
+    x,
+    num_spatial_dims,
+    data_format="channels_last",
+    include_batch_and_channels=True,
 ):
-    """Compute padding length along one dimension."""
-    total_padding_length = (
-        dilation_rate * (kernel_length - 1) - (input_length - 1) % stride
-    )
-    left_padding = total_padding_length // 2
-    right_padding = (total_padding_length + 1) // 2
-    return (left_padding, right_padding)
+    # Helper function that converts an operand to a spatial operand.
+    x = (x,) * num_spatial_dims if isinstance(x, int) else x
+    if not include_batch_and_channels:
+        return x
+    if data_format == "channels_last":
+        x = (1,) + x + (1,)
+    else:
+        x = (1,) + (1,) + x
+    return x
 
 
-def _apply_same_padding(
-    inputs, kernel_size, strides, operation_type, dilation_rate=1
+def _pool(
+    inputs,
+    initial_value,
+    reduce_fn,
+    pool_size,
+    strides=None,
+    padding="valid",
 ):
-    """Apply same padding to the input tensor.
+    """Helper function to define pooling functions.
 
-    This function will evaluate if the padding value is compatible with torch
-    functions. To avoid calling `pad()` as much as possible, which may cause
-    performance or memory issues, when compatible, it does not apply the padding
-    to the tensor, but returns the input tensor and the padding value to pass to
-    the torch functions. If not compatible, it returns the padded tensor and 0
-    as the padding value.
+    Args:
+        inputs: input data of shape `N+2`.
+        initial_value: the initial value for the reduction.
+        reduce_fn: a reduce function of the form `(T, T) -> T`.
+        pool_size: a sequence of `N` integers, representing the window size to
+            reduce over.
+        strides: a sequence of `N` integers, representing the inter-window
+            strides (default: `(1, ..., 1)`).
+        padding: either the string `same` or `valid`.
 
     Returns:
-        tensor: A padded tensor or the inputs.
-        padding: The padding value, ready to pass to the torch functions.
+        The output of the reduction for each window slice.
     """
-    spatial_shape = inputs.shape[2:]
-    num_spatial_dims = len(spatial_shape)
-    padding = ()
-
-    for i in range(num_spatial_dims):
-        if operation_type == "pooling":
-            padding_size = _compute_padding_length(
-                spatial_shape[i], kernel_size[i], strides[i]
-            )
-            mode = "replicate"
-        else:
-            dilation_rate = standardize_tuple(
-                dilation_rate, num_spatial_dims, "dilation_rate"
-            )
-            padding_size = _compute_padding_length(
-                spatial_shape[i], kernel_size[i], strides[i], dilation_rate[i]
-            )
-            mode = "constant"
-        padding = (padding_size,) + padding
-
-    if all([left == right for left, right in padding]):
-        return inputs, [left for left, _ in padding]
-
-    flattened_padding = tuple(
-        value for left_and_right in padding for value in left_and_right
-    )
-    return tnn.pad(inputs, pad=flattened_padding, mode=mode), 0
-
-
-def _transpose_spatial_inputs(inputs):
-    num_spatial_dims = inputs.ndim - 2
-    # Torch pooling does not support `channels_last` format, so
-    # we need to transpose to `channels_first` format.
-    if num_spatial_dims == 1:
-        inputs = torch.permute(inputs, (0, 2, 1))
-    elif num_spatial_dims == 2:
-        inputs = torch.permute(inputs, (0, 3, 1, 2))
-    elif num_spatial_dims == 3:
-        inputs = torch.permute(inputs, (0, 4, 1, 2, 3))
-    else:
+    if padding not in ("same", "valid"):
         raise ValueError(
-            "Inputs must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-    return inputs
-
-
-def _transpose_spatial_outputs(outputs):
-    # Undo the transpose in `_transpose_spatial_inputs`.
-    num_spatial_dims = len(outputs.shape) - 2
-    if num_spatial_dims == 1:
-        outputs = torch.permute(outputs, (0, 2, 1))
-    elif num_spatial_dims == 2:
-        outputs = torch.permute(outputs, (0, 2, 3, 1))
-    elif num_spatial_dims == 3:
-        outputs = torch.permute(outputs, (0, 2, 3, 4, 1))
-    return outputs
-
-
-def _transpose_conv_kernel(kernel):
-    # Torch requires conv kernel of format
-    # `(out_channels, in_channels, spatial_dims)`, we need to transpose.
-    num_spatial_dims = len(kernel.shape) - 2
-    if num_spatial_dims == 1:
-        kernel = torch.permute(kernel, (2, 1, 0))
-    elif num_spatial_dims == 2:
-        kernel = torch.permute(kernel, (3, 2, 0, 1))
-    elif num_spatial_dims == 3:
-        kernel = torch.permute(kernel, (4, 3, 0, 1, 2))
-    return kernel
+            f"Invalid padding '{padding}', must be 'same' or 'valid'."
+        )
+    padding = padding.upper()
+    return lax.reduce_window(
+        inputs,
+        initial_value,
+        reduce_fn,
+        pool_size,
+        strides,
+        padding,
+    )
 
 
 def max_pool(
     inputs,
     pool_size,
     strides=None,
     padding="valid",
     data_format=None,
 ):
-    inputs = convert_to_tensor(inputs)
-    num_spatial_dims = inputs.ndim - 2
-    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
-    if strides is None:
-        strides = pool_size
-    else:
-        strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
-    if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-
-    if padding == "same":
-        # Torch does not natively support `"same"` padding, we need to manually
-        # apply the right amount of padding to `inputs`.
-        inputs, padding = _apply_same_padding(
-            inputs, pool_size, strides, operation_type="pooling"
-        )
-    else:
-        padding = 0
-
-    device = get_device()
-    # Torch max pooling ops do not support symbolic tensors.
-    # Create a real tensor to execute the ops.
-    if device == "meta":
-        inputs = torch.empty(
-            size=inputs.shape, dtype=inputs.dtype, device="cpu"
-        )
-
-    if num_spatial_dims == 1:
-        outputs = tnn.max_pool1d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.max_pool2d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.max_pool3d(
-            inputs, kernel_size=pool_size, stride=strides, padding=padding
-        )
-    else:
-        raise ValueError(
-            "Inputs to pooling op must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-
-    outputs = outputs.to(device)
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    num_spatial_dims = inputs.ndim - 2
+    pool_size = _convert_to_spatial_operand(
+        pool_size, num_spatial_dims, data_format
+    )
+    strides = pool_size if strides is None else strides
+    strides = _convert_to_spatial_operand(
+        strides, num_spatial_dims, data_format
+    )
+    return _pool(inputs, -jnp.inf, lax.max, pool_size, strides, padding)
 
 
 def average_pool(
     inputs,
     pool_size,
-    strides=None,
-    padding="valid",
+    strides,
+    padding,
     data_format=None,
 ):
-    inputs = convert_to_tensor(inputs)
+    data_format = standardize_data_format(data_format)
     num_spatial_dims = inputs.ndim - 2
-    pool_size = standardize_tuple(pool_size, num_spatial_dims, "pool_size")
-    if strides is None:
-        strides = pool_size
-    else:
-        strides = standardize_tuple(strides, num_spatial_dims, "strides")
+    pool_size = _convert_to_spatial_operand(
+        pool_size, num_spatial_dims, data_format
+    )
+    strides = pool_size if strides is None else strides
+    strides = _convert_to_spatial_operand(
+        strides, num_spatial_dims, data_format
+    )
+
+    pooled = _pool(inputs, 0.0, lax.add, pool_size, strides, padding)
+    if padding == "valid":
+        # Avoid the extra reduce_window.
+        return pooled / np.prod(pool_size)
+    else:
+        # Count the number of valid entries at each input point, then use that
+        # for computing average. Assumes that any two arrays of same shape will
+        # be padded the same. Avoid broadcasting on axis where pooling is
+        # skipped.
+        shape = [
+            (a if b != 1 else 1) for (a, b) in zip(inputs.shape, pool_size)
+        ]
+        window_counts = _pool(
+            jnp.ones(shape, inputs.dtype),
+            0.0,
+            lax.add,
+            pool_size,
+            strides,
+            padding,
+        )
+        return pooled / window_counts
+
+
+def _convert_to_lax_conv_dimension_numbers(
+    num_spatial_dims,
+    data_format="channels_last",
+    transpose=False,
+):
+    """Create a `lax.ConvDimensionNumbers` for the given inputs."""
+    num_dims = num_spatial_dims + 2
 
-    data_format = standardize_data_format(data_format)
     if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    padding_value = 0
-    if padding == "same":
-        spatial_shape = inputs.shape[2:]
-        num_spatial_dims = len(spatial_shape)
-        padding_value = []
-        uneven_padding = []
-
-        for i in range(num_spatial_dims):
-            padding_size = _compute_padding_length(
-                spatial_shape[i], pool_size[i], strides[i]
-            )
-            # Torch only supports even padding on each dim, to replicate the
-            # behavior of "same" padding of `tf.keras` as much as possible,
-            # we need to pad evenly using the shorter padding.
-            padding_value.append(padding_size[0])
-            if padding_size[0] != padding_size[1]:
-                # Handle unequal padding.
-                # `torch.nn.pad` sets padding value in the reverse order.
-                uneven_padding = [0, 1] + uneven_padding
-        # Only call tnn.pad when needed.
-        if len(uneven_padding) > 0:
-            inputs = tnn.pad(inputs, uneven_padding)
+        spatial_dims = tuple(range(1, num_dims - 1))
+        inputs_dn = (0, num_dims - 1) + spatial_dims
+    else:
+        spatial_dims = tuple(range(2, num_dims))
+        inputs_dn = (0, 1) + spatial_dims
 
-    if num_spatial_dims == 1:
-        outputs = tnn.avg_pool1d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.avg_pool2d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.avg_pool3d(
-            inputs,
-            kernel_size=pool_size,
-            stride=strides,
-            padding=padding_value,
-            count_include_pad=False,
-        )
+    if transpose:
+        kernel_dn = (num_dims - 2, num_dims - 1) + tuple(range(num_dims - 2))
     else:
-        raise ValueError(
-            "Inputs to pooling op must have ndim=3, 4 or 5, "
-            "corresponding to 1D, 2D and 3D inputs. "
-            f"Received input shape: {inputs.shape}."
-        )
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+        kernel_dn = (num_dims - 1, num_dims - 2) + tuple(range(num_dims - 2))
+
+    return lax.ConvDimensionNumbers(
+        lhs_spec=inputs_dn, rhs_spec=kernel_dn, out_spec=inputs_dn
+    )
 
 
 def conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    inputs = convert_to_tensor(inputs)
-    kernel = convert_to_tensor(kernel)
-    num_spatial_dims = inputs.ndim - 2
-    strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
+    num_spatial_dims = inputs.ndim - 2
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
     if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    # Transpose kernel from keras format to torch format.
-    kernel = _transpose_conv_kernel(kernel)
-    if padding == "same" and any(d != 1 for d in tree.flatten(strides)):
-        # Torch does not support this case in conv2d().
-        # Manually pad the tensor.
-        inputs, padding = _apply_same_padding(
-            inputs,
-            kernel.shape[2:],
-            strides,
-            operation_type="conv",
-            dilation_rate=dilation_rate,
-        )
-    channels = inputs.shape[1]
-    kernel_in_channels = kernel.shape[1]
+        channels = inputs.shape[-1]
+    else:
+        channels = inputs.shape[1]
+    kernel_in_channels = kernel.shape[-2]
     if channels % kernel_in_channels > 0:
         raise ValueError(
             "The number of input channels must be evenly divisible by "
-            f"kernel.shape[1]. Received: inputs.shape={inputs.shape}, "
-            f"kernel.shape={kernel.shape}"
+            f"kernel's in_channels. Received input channels {channels} and "
+            f"kernel in_channels {kernel_in_channels}. "
         )
-    groups = channels // kernel_in_channels
-    if num_spatial_dims == 1:
-        outputs = tnn.conv1d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.conv2d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.conv3d(
-            inputs,
-            kernel,
-            stride=strides,
-            dilation=dilation_rate,
-            groups=groups,
-            padding=padding,
-        )
-    else:
-        raise ValueError(
-            "Inputs to conv operation should have ndim=3, 4, or 5,"
-            "corresponding to 1D, 2D and 3D inputs. Received input "
-            f"shape: {inputs.shape}."
-        )
-
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    feature_group_count = channels // kernel_in_channels
+    return jax.lax.conv_general_dilated(
+        convert_to_tensor(inputs),
+        convert_to_tensor(kernel),
+        strides,
+        padding,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        feature_group_count=feature_group_count,
+    )
 
 
 def depthwise_conv(
     inputs,
     kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
-    kernel = convert_to_tensor(kernel)
-    kernel = torch.reshape(
-        kernel, kernel.shape[:-2] + (1, kernel.shape[-2] * kernel.shape[-1])
+    data_format = standardize_data_format(data_format)
+    num_spatial_dims = inputs.ndim - 2
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    feature_group_count = (
+        inputs.shape[-1] if data_format == "channels_last" else inputs.shape[1]
+    )
+    kernel = jnp.reshape(
+        kernel,
+        kernel.shape[:-2] + (1, feature_group_count * kernel.shape[-1]),
+    )
+    return jax.lax.conv_general_dilated(
+        inputs,
+        kernel,
+        strides,
+        padding,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        feature_group_count=feature_group_count,
     )
-    return conv(inputs, kernel, strides, padding, data_format, dilation_rate)
 
 
 def separable_conv(
     inputs,
     depthwise_kernel,
     pointwise_kernel,
     strides=1,
     padding="valid",
     data_format=None,
     dilation_rate=1,
 ):
+    data_format = standardize_data_format(data_format)
     depthwise_conv_output = depthwise_conv(
         inputs,
         depthwise_kernel,
         strides,
         padding,
         data_format,
         dilation_rate,
@@ -485,117 +362,107 @@
     kernel,
     strides=1,
     padding="valid",
     output_padding=None,
     data_format=None,
     dilation_rate=1,
 ):
-    inputs = convert_to_tensor(inputs)
-    kernel = convert_to_tensor(kernel)
-    num_spatial_dims = inputs.ndim - 2
-    strides = standardize_tuple(strides, num_spatial_dims, "strides")
-
     data_format = standardize_data_format(data_format)
-    (
-        torch_padding,
-        torch_output_padding,
-    ) = compute_conv_transpose_padding_args_for_torch(
+    num_spatial_dims = inputs.ndim - 2
+    padding_values = compute_conv_transpose_padding_args_for_jax(
         input_shape=inputs.shape,
         kernel_shape=kernel.shape,
         strides=strides,
         padding=padding,
         output_padding=output_padding,
         dilation_rate=dilation_rate,
     )
-    if data_format == "channels_last":
-        inputs = _transpose_spatial_inputs(inputs)
-    # Transpose kernel from keras format to torch format.
-    kernel = _transpose_conv_kernel(kernel)
-    kernel_spatial_shape = kernel.shape[2:]
-    if isinstance(dilation_rate, int):
-        dilation_rate = [dilation_rate] * len(kernel_spatial_shape)
+    dimension_numbers = _convert_to_lax_conv_dimension_numbers(
+        num_spatial_dims,
+        data_format,
+        transpose=False,
+    )
+    strides = _convert_to_spatial_operand(
+        strides,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
+    dilation_rate = _convert_to_spatial_operand(
+        dilation_rate,
+        num_spatial_dims,
+        data_format,
+        include_batch_and_channels=False,
+    )
 
-    if num_spatial_dims == 1:
-        outputs = tnn.conv_transpose1d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    elif num_spatial_dims == 2:
-        outputs = tnn.conv_transpose2d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    elif num_spatial_dims == 3:
-        outputs = tnn.conv_transpose3d(
-            inputs,
-            kernel,
-            stride=strides,
-            padding=torch_padding,
-            output_padding=torch_output_padding,
-            dilation=dilation_rate,
-        )
-    else:
-        raise ValueError(
-            "Inputs to conv transpose operation should have ndim=3, 4, or 5,"
-            "corresponding to 1D, 2D and 3D inputs. Received input "
-            f"shape: {inputs.shape}."
-        )
-    if data_format == "channels_last":
-        outputs = _transpose_spatial_outputs(outputs)
-    return outputs
+    return jax.lax.conv_transpose(
+        inputs,
+        kernel,
+        strides,
+        padding=padding_values,
+        rhs_dilation=dilation_rate,
+        dimension_numbers=dimension_numbers,
+        transpose_kernel=True,
+    )
 
 
 def one_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
+    x = convert_to_tensor(x)
     if sparse:
-        raise ValueError("Unsupported value `sparse=True` with torch backend")
-    # Axis is the output axis. By default, PyTorch, outputs to last axis.
-    # If axis is not last, change output to axis and shift remaining elements.
-    x = convert_to_tensor(x, dtype=torch.long)
-
-    # Torch one_hot does not natively handle negative values, so we add some
-    # manual handling for negatives in the input to one_hot by using max(x, 0).
-    # The output will have some invalid results, so we set them back to 0 using
-    # `where` afterwards.
-    output = tnn.one_hot(maximum(x, 0), num_classes)
-    output = where(expand_dims(x, axis=-1) >= 0, output, 0)
-    output = convert_to_tensor(output, dtype=dtype)
-    dims = output.dim()
-    if axis != -1 and axis != dims:
-        new_axes_order = list(range(dims))
-        new_axes_order[axis] = -1  # Shifts output to axis position
-        # Shift remaining axes with offset by 1 since output moved to `axis`.
-        for ax in range(axis + 1, dims):
-            new_axes_order[ax] -= 1
-        output = output.permute(new_axes_order)
-    return output
+        if axis < 0:
+            axis = axis + len(x.shape) + 1
+        if dtype is None:
+            dtype = "float32"
+        # We deal with negative inputs by having zeros in the output although
+        # it's useless. It makes shapes static.
+        values = jnp.greater_equal(jnp.ravel(x), 0).astype(dtype)
+        values_count = values.shape[0]
+        indices = [jnp.arange(dim) for dim in x.shape]
+        indices = jnp.meshgrid(*indices, indexing="ij")
+        indices.insert(axis, jnp.maximum(x, 0))  # Deal with negative indices
+        indices = [a.reshape(values_count, 1).astype("int32") for a in indices]
+        indices = jnp.concatenate(indices, axis=1)
+        shape = list(x.shape)
+        shape.insert(axis, num_classes)
+        shape = tuple(shape)
+        return jax_sparse.BCOO(
+            (values, indices),
+            shape=shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
+    return jnn.one_hot(x, num_classes, axis=axis, dtype=dtype)
 
 
 def multi_hot(x, num_classes, axis=-1, dtype="float32", sparse=False):
-    if sparse:
-        raise ValueError("Unsupported value `sparse=True` with torch backend")
     x = convert_to_tensor(x)
     reduction_axis = 1 if len(x.shape) > 1 else 0
-    outputs = torch.amax(
+    if sparse:
+        result = one_hot(
+            x, num_classes, axis=axis, dtype="int32", sparse=sparse
+        )
+        # JAX's BCOO does not support max reduction, use sum and compare with 0.
+        result = jax_sparse.bcoo_reduce_sum(result, axes=(reduction_axis,))
+        result = jax_sparse.bcoo_sum_duplicates(result)
+        values = jnp.greater_equal(result.data, 0).astype(dtype)
+        return jax_sparse.BCOO(
+            (values, result.indices),
+            shape=result.shape,
+            indices_sorted=True,
+            unique_indices=True,
+        )
+    return jnp.max(
         one_hot(cast(x, "int32"), num_classes, axis=axis, dtype=dtype),
-        dim=reduction_axis,
+        axis=reduction_axis,
     )
-    return outputs
 
 
 def categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
+    target = jnp.array(target)
+    output = jnp.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
@@ -603,164 +470,427 @@
         raise ValueError(
             "Arguments `target` and `output` must be at least rank 1. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
 
     if from_logits:
-        log_prob = tnn.log_softmax(output, dim=axis)
+        log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
-        output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = torch.log(output)
-    return -torch.sum(target * log_prob, dim=axis)
+        output = output / jnp.sum(output, axis, keepdims=True)
+        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = jnp.log(output)
+    return -jnp.sum(target * log_prob, axis=axis)
 
 
 def sparse_categorical_crossentropy(target, output, from_logits=False, axis=-1):
-    target = convert_to_tensor(target, dtype=torch.long)
-    output = convert_to_tensor(output)
-
+    target = jnp.array(target, dtype="int32")
+    output = jnp.array(output)
     if len(target.shape) == len(output.shape) and target.shape[-1] == 1:
-        target = torch.squeeze(target, dim=-1)
+        target = jnp.squeeze(target, axis=-1)
 
     if len(output.shape) < 1:
         raise ValueError(
             "Argument `output` must be at least rank 1. "
             "Received: "
             f"output.shape={output.shape}"
         )
     if target.shape != output.shape[:-1]:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape "
             "up until the last dimension: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
     if from_logits:
-        log_prob = tnn.log_softmax(output, dim=axis)
+        log_prob = jax.nn.log_softmax(output, axis=axis)
     else:
-        output = output / torch.sum(output, dim=axis, keepdim=True)
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        log_prob = torch.log(output)
-    target = one_hot(target, output.shape[axis], axis=axis)
-    return -torch.sum(target * log_prob, dim=axis)
+        output = output / jnp.sum(output, axis, keepdims=True)
+        output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+        log_prob = jnp.log(output)
+    target = jnn.one_hot(target, output.shape[axis], axis=axis)
+    return -jnp.sum(target * log_prob, axis=axis)
 
 
 def binary_crossentropy(target, output, from_logits=False):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
+    target = jnp.array(target)
+    output = jnp.array(output)
 
     if target.shape != output.shape:
         raise ValueError(
             "Arguments `target` and `output` must have the same shape. "
             "Received: "
             f"target.shape={target.shape}, output.shape={output.shape}"
         )
-    # By default, PyTorch, does reduction of `sum` over all rows,
-    # change reduction to `none` to keep dim
+
     if from_logits:
-        return tnn.binary_cross_entropy_with_logits(
-            output, target, reduction="none"
-        )
-    else:
-        output = torch.clip(output, epsilon(), 1.0 - epsilon())
-        return tnn.binary_cross_entropy(output, target, reduction="none")
+        log_logits = jax.nn.log_sigmoid(output)
+        log_neg_logits = jax.nn.log_sigmoid(-output)
+        return -1.0 * target * log_logits - (1.0 - target) * log_neg_logits
+
+    output = jnp.clip(output, epsilon(), 1.0 - epsilon())
+    bce = target * jnp.log(output)
+    bce += (1.0 - target) * jnp.log(1.0 - output)
+    return -bce
 
 
 def moments(x, axes, keepdims=False, synchronized=False):
     if synchronized:
         raise NotImplementedError(
-            "Argument synchronized=True is not supported with PyTorch."
+            "Argument synchronized=True is not supported with JAX."
         )
-    x = convert_to_tensor(x)
     # The dynamic range of float16 is too limited for statistics. As a
     # workaround, we simply perform the operations on float32 and convert back
     # to float16
     need_cast = False
     ori_dtype = standardize_dtype(x.dtype)
-    if ori_dtype == "float16":
+    if ori_dtype in ("float16", "bfloat16"):
         need_cast = True
         x = cast(x, "float32")
 
-    mean = torch.mean(x, dim=axes, keepdim=True)
-
-    # The variance is computed using $Var = E[|x|^2] - |E[x]|^2$, It is faster
-    # but less numerically stable.
-    # Note: stop_gradient does not change the gradient to the mean, because that
-    # gradient is zero.
-    variance = torch.mean(
-        torch.square(x), dim=axes, keepdim=True
-    ) - torch.square(mean)
+    mean = jnp.mean(x, axes, keepdims=True)
+    variance = jnp.var(x, axis=axes, keepdims=True)
 
     if not keepdims:
-        mean = torch.squeeze(mean, axes)
-        variance = torch.squeeze(variance, axes)
+        mean = jnp.squeeze(mean, axes)
+        variance = jnp.squeeze(variance, axes)
     if need_cast:
         # avoid overflow and underflow when casting from float16 to float32
-        mean = torch.clip(
-            mean,
-            torch.finfo(torch.float16).min,
-            torch.finfo(torch.float16).max,
-        )
-        variance = torch.clip(
-            variance,
-            torch.finfo(torch.float16).min,
-            torch.finfo(torch.float16).max,
+        mean = jnp.clip(
+            mean, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
+        )
+        variance = jnp.clip(
+            variance, jnp.finfo(jnp.float16).min, jnp.finfo(jnp.float16).max
         )
         mean = cast(mean, ori_dtype)
         variance = cast(variance, ori_dtype)
     return mean, variance
 
 
 def batch_normalization(
     x, mean, variance, axis, offset=None, scale=None, epsilon=1e-3
 ):
-    x = convert_to_tensor(x)
-    mean = convert_to_tensor(mean)
-    variance = convert_to_tensor(variance)
-
     shape = [1] * len(x.shape)
     shape[axis] = mean.shape[0]
-    mean = torch.reshape(mean, shape)
-    variance = torch.reshape(variance, shape)
+    mean = jnp.reshape(mean, shape)
+    variance = jnp.reshape(variance, shape)
 
-    if offset is not None:
-        offset = convert_to_tensor(offset)
-        offset = torch.reshape(offset, shape)
-    else:
-        offset = torch.zeros_like(mean)
+    inv = jax.lax.rsqrt(variance + epsilon)
     if scale is not None:
-        scale = convert_to_tensor(scale)
-        scale = torch.reshape(scale, shape)
-    else:
-        scale = torch.ones_like(variance)
+        scale = jnp.reshape(scale, shape)
+        inv = inv * scale
 
-    return (
-        x.subtract(mean)
-        .mul_(variance.add(epsilon).rsqrt_().mul(scale))
-        .add_(offset)
-    )
+    res = -mean * inv
+    if offset is not None:
+        offset = jnp.reshape(offset, shape)
+        res = res + offset
+
+    return jnp.add(x * inv, res)
 
 
 def ctc_loss(
     target,
     output,
     target_length,
     output_length,
     mask_index=0,
 ):
-    target = convert_to_tensor(target)
-    output = convert_to_tensor(output)
-    target_length = convert_to_tensor(target_length)
-    output_length = convert_to_tensor(output_length)
-
-    output = torch.transpose(output, 1, 0)
-    logits = tnn.log_softmax(output, dim=-1)
-
-    return tnn.ctc_loss(
-        logits,
-        target,
-        output_length,
-        target_length,
-        blank=mask_index,
-        reduction="none",
+    batch_size, _, _ = output.shape
+    batch_size, max_target_length = target.shape
+
+    output = output.transpose((1, 0, 2))
+    target = target.transpose((1, 0)).astype("int32")
+
+    logits = jnn.log_softmax(output)
+    mgrid_t, mgrid_b = jnp.meshgrid(
+        jnp.arange(max_target_length), jnp.arange(batch_size)
+    )
+    logprobs_emit = logits[mgrid_t, mgrid_b, target[:, :, None]]
+    logprobs_mask = logits[:, :, mask_index]
+
+    logit_paddings = jnp.array(
+        jnp.arange(max_target_length) < output_length[:, None],
+        dtype=jnp.float32,
+    )
+
+    repeat = jnp.array(target[1:] == target[:-1])
+    repeat = jnp.pad(repeat, ((0, 1), (0, 0))).transpose((1, 0))
+
+    _logepsilon = -100000.0
+
+    def _iterate(prev, x):
+        prev_mask, prev_emit = prev
+        logprob_mask, logprob_emit, pad = x
+
+        prev_mask_orig = prev_mask
+        prev_mask = prev_mask.at[:, 1:].set(
+            jnp.logaddexp(prev_mask[:, 1:], prev_emit + _logepsilon * repeat),
+        )
+        emit = jnp.logaddexp(
+            prev_mask[:, :-1] + logprob_emit, prev_emit + logprob_emit
+        )
+
+        mask = prev_mask + logprob_mask[:, None]
+        mask = mask.at[:, 1:].set(
+            jnp.logaddexp(
+                mask[:, 1:],
+                prev_emit + logprob_mask[:, None] + _logepsilon * (1 - repeat),
+            )
+        )
+
+        pad = pad[:, None]
+        emit = emit * pad + prev_emit * (1 - pad)
+        mask = mask * pad + prev_mask_orig * (1 - pad)
+
+        return (mask, emit), (mask, emit)
+
+    mask_init = jnp.full((batch_size, max_target_length + 1), _logepsilon)
+    mask_init = mask_init.at[:, 0].set(0.0)
+    emit_init = jnp.full((batch_size, max_target_length), _logepsilon)
+
+    _, (alphas_mask, alphas_emit) = lax.scan(
+        _iterate,
+        (mask_init, emit_init),
+        (logprobs_mask, logprobs_emit, logit_paddings.transpose()),
+    )
+
+    last_alpha_mask = (
+        alphas_mask[-1]
+        .at[:, 1:]
+        .set(jnp.logaddexp(alphas_mask[-1, :, 1:], alphas_emit[-1]))
+    )
+
+    return -last_alpha_mask[jnp.arange(batch_size), target_length]
+
+
+def ctc_greedy_decode(
+    inputs,
+    sequence_length,
+    merge_repeated=True,
+    mask_index=None,
+):
+    inputs = jnp.array(inputs)
+    sequence_length = jnp.array(sequence_length, dtype=jnp.int32)
+
+    if mask_index is None:
+        mask_index = inputs.shape[-1] - 1
+
+    indices = jnp.argmax(inputs, axis=-1)
+    scores = jnp.max(inputs, axis=-1)
+
+    seqlen_mask = jnp.arange(inputs.shape[1])[None, :]
+    seqlen_mask = seqlen_mask >= sequence_length[:, None]
+
+    if merge_repeated:
+        repeat = indices[:, 1:] == indices[:, :-1]
+        repeat = jnp.pad(repeat, ((0, 0), (1, 0)))
+
+        indices = jnp.where(repeat, mask_index, indices)
+    else:
+        repeat = jnp.zeros_like(indices, dtype=bool)
+
+    indices = jnp.where(seqlen_mask, mask_index, indices)
+    indices = [batch[batch != mask_index] for batch in indices]
+    max_len = max(len(batch) for batch in indices)
+    indices = jnp.array(
+        [jnp.pad(batch, (0, max_len - len(batch))) for batch in indices]
     )
 
+    scores = jnp.where(seqlen_mask, 0.0, scores)
+    scores = -jnp.sum(scores, axis=1)[:, None]
+
+    return [indices], scores
+
+
+def ctc_beam_search_decode(
+    inputs,
+    sequence_length,
+    beam_width=100,
+    top_paths=1,
+    mask_index=None,
+):
+    inputs = jnp.array(inputs)
+    sequence_length = jnp.array(sequence_length)
+
+    batch_size, max_seq_len, num_classes = inputs.shape
+    inputs = jnn.log_softmax(inputs)
+    seqlen_mask = jnp.arange(max_seq_len)[None, :] >= sequence_length[:, None]
+
+    if mask_index is None:
+        mask_index = num_classes - 1
+
+    # This is a workaround for the fact that jnp.argsort does not support
+    # the order parameter which is used to break ties when scores are equal.
+    # For compatibility with the tensorflow implementation, we flip the inputs
+    # and the mask_index, and then flip the classes back to the correct indices
+    inputs = jnp.flip(inputs, axis=2)
+    mask_index = num_classes - mask_index - 1
+
+    _pad = -1
+
+    init_paths = jnp.full(
+        (batch_size, 2 * beam_width, max_seq_len), _pad, dtype=jnp.int32
+    )
+
+    num_init_paths = jnp.min(jnp.array([num_classes, beam_width]))
+    max_classes = jnp.argsort(inputs[:, 0], axis=1)[:, -num_init_paths:]
+    init_classes = jnp.where(max_classes == mask_index, _pad, max_classes)
+    init_paths = init_paths.at[:, :num_init_paths, 0].set(init_classes)
+
+    init_scores = (
+        jnp.full((batch_size, 2 * beam_width), -jnp.inf)
+        .at[:, :num_init_paths]
+        .set(jnp.take_along_axis(inputs[:, 0], max_classes, axis=1))
+    )
+    init_masked = init_paths[:, :, 0] == _pad
+
+    def _extend_paths(paths, scores, masked, x):
+        paths = jnp.repeat(paths, num_classes, axis=0)
+        scores = jnp.repeat(scores, num_classes)
+        masked = jnp.repeat(masked, num_classes)
+
+        path_tail_index = jnp.argmax(paths == _pad, axis=1)
+        paths_arange = jnp.arange(2 * beam_width * num_classes)
+        path_tails = paths[paths_arange, path_tail_index - 1]
+        path_tails = jnp.where(path_tail_index == 0, _pad, path_tails)
+
+        classes = jnp.arange(num_classes).at[mask_index].set(_pad)
+        classes = jnp.tile(classes, 2 * beam_width)
+
+        prev_masked = masked
+        masked = classes == _pad
+
+        masked_repeat = ~prev_masked & (path_tails == classes)
+        classes = jnp.where(masked_repeat, _pad, classes)
+        paths = paths.at[paths_arange, path_tail_index].set(classes)
+
+        x = jnp.tile(x, 2 * beam_width)
+        scores = scores + x
+
+        return paths, scores, masked
+
+    def _merge_scores(unique_inverse, scores):
+        scores_max = jnp.max(scores)
+        scores_exp = jnp.exp(scores - scores_max)
+        scores = jnp.zeros_like(scores).at[unique_inverse].add(scores_exp)
+        scores = jnp.log(scores) + scores_max
+        return scores
+
+    def _prune_paths(paths, scores, masked):
+        paths, unique_inverse = jnp.unique(
+            paths,
+            return_inverse=True,
+            size=2 * num_classes * beam_width,
+            axis=0,
+            fill_value=_pad,
+        )
+        if len(unique_inverse.shape) >= 2:
+            unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+
+        emit_scores = jnp.where(masked, -jnp.inf, scores)
+        mask_scores = jnp.where(masked, scores, -jnp.inf)
+
+        emit_scores = _merge_scores(unique_inverse, emit_scores)
+        mask_scores = _merge_scores(unique_inverse, mask_scores)
+
+        total_scores = jnp.logaddexp(emit_scores, mask_scores)
+        top_indices = jnp.argsort(total_scores)[-beam_width:]
+
+        paths = paths[top_indices]
+        emit_scores = emit_scores[top_indices]
+        mask_scores = mask_scores[top_indices]
+
+        paths = jnp.tile(paths, (2, 1))
+        scores = jnp.concatenate([emit_scores, mask_scores])
+        masked = jnp.concatenate(
+            [jnp.zeros(beam_width, bool), jnp.ones(beam_width, bool)]
+        )
+
+        return paths, scores, masked
+
+    def _decode_step(paths, scores, masked, x):
+        paths, scores, masked = _extend_paths(paths, scores, masked, x)
+        paths, scores, masked = _prune_paths(paths, scores, masked)
+        return paths, scores, masked
+
+    def _step(prev, x):
+        paths, scores, masked = prev
+        x, seqlen_mask = x
+
+        paths, scores, masked = lax.cond(
+            seqlen_mask,
+            lambda paths, scores, masked, x: (paths, scores, masked),
+            _decode_step,
+            paths,
+            scores,
+            masked,
+            x,
+        )
+
+        return (paths, scores, masked), None
+
+    def _decode_batch(
+        init_paths, init_scores, init_masked, inputs, seqlen_mask
+    ):
+        (paths, scores, masked), _ = lax.scan(
+            _step,
+            (init_paths, init_scores, init_masked),
+            (inputs[1:], seqlen_mask[1:]),
+        )
+
+        paths, unique_inverse = jnp.unique(
+            paths,
+            return_inverse=True,
+            size=2 * num_classes * beam_width,
+            axis=0,
+            fill_value=_pad,
+        )
+        if len(unique_inverse.shape) >= 2:
+            unique_inverse = jnp.squeeze(unique_inverse, axis=1)
+        scores = _merge_scores(unique_inverse, scores)
+
+        top_indices = jnp.argsort(scores)[-top_paths:][::-1]
+        paths = paths[top_indices]
+        scores = scores[top_indices]
+
+        return paths, scores
+
+    paths, scores = jax.vmap(_decode_batch)(
+        init_paths, init_scores, init_masked, inputs, seqlen_mask
+    )
+
+    # convert classes back to the correct indices
+    paths = jnp.where(paths == _pad, _pad, num_classes - paths - 1)
+
+    lengths = jnp.argmax(paths == _pad, axis=2)
+    lengths = jnp.max(lengths, axis=0)
+    paths = jnp.where(paths == _pad, 0, paths)
+
+    paths = paths.transpose((1, 0, 2))
+    paths = [path[:, :length] for path, length in zip(paths, lengths)]
+
+    return paths, scores
+
+
+def ctc_decode(
+    inputs,
+    sequence_length,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    if strategy == "greedy":
+        return ctc_greedy_decode(
+            inputs,
+            sequence_length,
+            merge_repeated=merge_repeated,
+            mask_index=mask_index,
+        )
+    else:
+        return ctc_beam_search_decode(
+            inputs,
+            sequence_length,
+            beam_width=beam_width,
+            top_paths=top_paths,
+            mask_index=mask_index,
+        )
```

### Comparing `keras-3.2.1/keras/src/backend/torch/numpy.py` & `keras-3.3.0/keras/src/backend/torch/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import torch
 
 from keras.src.backend import KerasTensor
 from keras.src.backend import config
 from keras.src.backend.common import dtypes
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
+from keras.src.backend.common.backend_utils import vectorize_impl
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.backend.torch.core import cast
 from keras.src.backend.torch.core import convert_to_tensor
 from keras.src.backend.torch.core import get_device
 from keras.src.backend.torch.core import is_tensor
 from keras.src.backend.torch.core import to_torch_dtype
 
@@ -168,16 +169,19 @@
         result = torch.max(x)
     else:
         result = amax(x, axis=axis, keepdims=keepdims)
     if isinstance(getattr(result, "values", None), torch.Tensor):
         result = result.values
 
     if initial is not None:
-        initial = convert_to_tensor(initial)
-        return torch.maximum(result, torch.full(result.shape, initial))
+        dtype = to_torch_dtype(result.dtype)
+        initial = convert_to_tensor(initial, dtype=dtype)
+        return torch.maximum(
+            result, torch.full(result.shape, initial, dtype=dtype)
+        )
     return result
 
 
 def ones(shape, dtype=None):
     dtype = to_torch_dtype(dtype or config.floatx())
     if isinstance(shape, int):
         shape = (shape,)
@@ -194,25 +198,25 @@
 def zeros_like(x, dtype=None):
     x = convert_to_tensor(x)
     dtype = to_torch_dtype(dtype or x.dtype)
     return torch.zeros_like(x, dtype=dtype)
 
 
 def absolute(x):
-    return abs(x)
-
-
-def abs(x):
     x = convert_to_tensor(x)
     # bool are always non-negative
     if standardize_dtype(x.dtype) == "bool":
         return x
     return torch.abs(x)
 
 
+def abs(x):
+    return absolute(x)
+
+
 def all(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
     if axis is None:
         return cast(torch.all(x), "bool")
     axis = to_tuple_or_list(axis)
     for a in axis:
         # `torch.all` does not handle multiple axes.
@@ -314,32 +318,32 @@
 
 
 def arctanh(x):
     x = convert_to_tensor(x)
     return torch.arctanh(x)
 
 
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
 
     # TODO: torch.argmax doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = cast(x, "uint8")
 
-    return cast(torch.argmax(x, dim=axis), dtype="int32")
+    return cast(torch.argmax(x, dim=axis, keepdim=keepdims), dtype="int32")
 
 
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     x = convert_to_tensor(x)
 
     # TODO: torch.argmin doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
         x = cast(x, "uint8")
 
-    return cast(torch.argmin(x, dim=axis), dtype="int32")
+    return cast(torch.argmin(x, dim=axis, keepdim=keepdims), dtype="int32")
 
 
 def argsort(x, axis=-1):
     x = convert_to_tensor(x)
 
     # TODO: torch.argsort doesn't support bool
     if standardize_dtype(x.dtype) == "bool":
@@ -740,16 +744,23 @@
             getattr(start, "dtype", type(start)),
             getattr(stop, "dtype", type(stop)),
             float,
         ]
         dtype = dtypes.result_type(*dtypes_to_resolve)
     dtype = to_torch_dtype(dtype)
 
-    if endpoint is False:
-        stop = stop - ((stop - start) / num)
+    step = convert_to_tensor(torch.nan)
+    if endpoint:
+        if num > 1:
+            step = (stop - start) / (num - 1)
+    else:
+        if num > 0:
+            step = (stop - start) / num
+        if num > 1:
+            stop = stop - ((stop - start) / num)
     if hasattr(start, "__len__") and hasattr(stop, "__len__"):
         start = convert_to_tensor(start, dtype=dtype)
         stop = convert_to_tensor(stop, dtype=dtype)
         steps = torch.arange(num, dtype=dtype, device=get_device()) / (num - 1)
 
         # reshape `steps` to allow for broadcasting
         for i in range(start.ndim):
@@ -762,15 +773,15 @@
             start=start,
             end=stop,
             steps=num,
             dtype=dtype,
             device=get_device(),
         )
     if retstep is True:
-        return (linspace, num)
+        return (linspace, step)
     return linspace
 
 
 def log(x):
     x = convert_to_tensor(x)
     return torch.log(x)
 
@@ -945,15 +956,16 @@
     else:
         result = amin(x, axis=axis, keepdims=keepdims)
 
     if isinstance(getattr(result, "values", None), torch.Tensor):
         result = result.values
 
     if initial is not None:
-        initial = convert_to_tensor(initial)
+        dtype = to_torch_dtype(result.dtype)
+        initial = convert_to_tensor(initial, dtype=dtype)
         return torch.minimum(result, initial)
     return result
 
 
 def minimum(x1, x2):
     if not isinstance(x1, (int, float)):
         x1 = convert_to_tensor(x1)
@@ -979,17 +991,17 @@
 
 
 def moveaxis(x, source, destination):
     x = convert_to_tensor(x)
     return torch.moveaxis(x, source=source, destination=destination)
 
 
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     x = convert_to_tensor(x)
-    return torch.nan_to_num(x)
+    return torch.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 def ndim(x):
     x = convert_to_tensor(x)
     return x.ndim
 
 
@@ -1261,14 +1273,21 @@
     x = convert_to_tensor(x)
     return torch.swapaxes(x, axis0=axis1, axis1=axis2)
 
 
 def take(x, indices, axis=None):
     x = convert_to_tensor(x)
     indices = convert_to_tensor(indices).long()
+    # Correct the indices using "fill" mode which is the same as in jax
+    x_dim = x.shape[axis] if axis is not None else x.shape[0]
+    indices = torch.where(
+        indices < 0,
+        indices + x_dim,
+        indices,
+    )
     if x.ndim == 2 and axis == 0:
         # This case is equivalent to embedding lookup.
         return torch.nn.functional.embedding(indices, x)
     if axis is None:
         x = torch.reshape(x, (-1,))
         axis = 0
     if axis is not None:
@@ -1281,14 +1300,21 @@
         return out.reshape(shape)
     return torch.take(x, index=indices)
 
 
 def take_along_axis(x, indices, axis=None):
     x = convert_to_tensor(x)
     indices = convert_to_tensor(indices).long()
+    # Correct the indices using "fill" mode which is the same as in jax
+    x_dim = x.shape[axis] if axis is not None else x.shape[0]
+    indices = torch.where(
+        indices < 0,
+        indices + x_dim,
+        indices,
+    )
     return torch.take_along_dim(x, indices, dim=axis)
 
 
 def tan(x):
     x = convert_to_tensor(x)
     return torch.tan(x)
 
@@ -1383,14 +1409,20 @@
 
 
 def vstack(xs):
     xs = [convert_to_tensor(x) for x in xs]
     return torch.vstack(xs)
 
 
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    return vectorize_impl(
+        pyfunc, torch.vmap, excluded=excluded, signature=signature
+    )
+
+
 def where(condition, x1, x2):
     condition = convert_to_tensor(condition, dtype=bool)
     if x1 is not None and x2 is not None:
         x1 = convert_to_tensor(x1)
         x2 = convert_to_tensor(x2)
         return torch.where(condition, x1, x2)
     else:
@@ -1564,7 +1596,15 @@
 
     if mode == "same":
         start_idx = (result.size(-1) - x1_len) // 2
         result = result[..., start_idx : start_idx + x1_len]
 
     return torch.squeeze(result)
 
+
+def select(condlist, choicelist, default=0):
+    condlist = [convert_to_tensor(c) for c in condlist]
+    choicelist = [convert_to_tensor(c) for c in choicelist]
+    out = convert_to_tensor(default)
+    for c, v in reversed(list(zip(condlist, choicelist))):
+        out = torch.where(c, v, out)
+    return out
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,7 @@
         torch._foreach_add_(
             accumulated_delta_vars,
             torch._foreach_mul(delta_vars, delta_vars),
             alpha=1 - rho,
         )
 
         torch._foreach_add_(variables, delta_vars, alpha=lr)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
                 torch._foreach_mul(grads, lr),
                 torch._foreach_sqrt(
                     torch._foreach_add(accumulators, self.epsilon)
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,8 +52,7 @@
             variables,
             torch._foreach_div(
                 torch._foreach_mul(m_list, alpha),
                 torch._foreach_add(torch._foreach_sqrt(v_list), self.epsilon),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,8 +46,7 @@
                 torch._foreach_mul(
                     torch._foreach_add(u_list, self.epsilon),
                     1 - beta_1_power,
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,8 +31,7 @@
             variables,
             torch._foreach_mul(c_t, lr),
             alpha=-1,
         )
 
         torch._foreach_mul_(m_list, self.beta_2)
         torch._foreach_add_(m_list, grads, alpha=1 - self.beta_2)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,8 +68,7 @@
                 torch._foreach_mul(m_hat_list, lr),
                 torch._foreach_add(
                     torch._foreach_sqrt(v_hat_list), self.epsilon
                 ),
             ),
             alpha=-1,
         )
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,8 +39,7 @@
         if self.weight_decay is None:
             return
 
         torch._foreach_mul_(
             [v.value for v in variables if self._use_weight_decay(v)],
             1 - self.weight_decay * self._get_current_learning_rate(),
         )
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,11 +15,10 @@
 
     @torch_utils.no_grad
     def _backend_reset_gradient_accumulators(self):
         acc_list = [v.value for v in self._accumulated_gradients]
         torch._foreach_mul_(acc_list, 0.0)
 
     @torch_utils.no_grad
-    def _backend_increment_gradient_accumulators(self, grads):
-        acc_list = [v.value for v in self._accumulated_gradients]
+    def _backend_increment_gradient_accumulators(self, grads, acc_grads):
+        acc_list = [v.value for v in acc_grads]
         torch._foreach_add_(acc_list, grads, alpha=1.0)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
                 for variable in keras_variables
             ]
             torch._foreach_mul_(momentum_list, self.momentum)
             torch._foreach_add_(momentum_list, increments)
             torch._foreach_add_(variables, momentum_list, alpha=-1)
         else:
             torch._foreach_add_(variables, increments, alpha=-1)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-3.3.0/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,7 @@
                 torch._foreach_add_(variables, grads, alpha=-learning_rate)
                 torch._foreach_add_(variables, bufs, alpha=self.momentum)
             else:
                 torch._foreach_add_(variables, bufs)
 
         else:
             torch._foreach_add_(variables, grads, alpha=-learning_rate)
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/random.py` & `keras-3.3.0/keras/src/backend/torch/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -238,8 +238,7 @@
         torch.manual_seed(first_seed + second_seed)
     beta_distribution = torch.distributions.beta.Beta(
         concentration1=alpha, concentration0=beta
     )
     sample = beta_distribution.sample().type(dtype)
     torch.random.set_rng_state(prev_rng_state)
     return sample
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/rnn.py` & `keras-3.3.0/keras/src/backend/torch/rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import torch
 
+from keras.src import tree
 from keras.src.backend.torch.core import convert_to_tensor
-from keras.src.utils import tree
 
 
 def rnn(
     step_function,
     inputs,
     initial_states,
     go_backwards=False,
@@ -377,8 +377,7 @@
 
 def lstm(*args, **kwargs):
     raise NotImplementedError
 
 
 def gru(*args, **kwargs):
     raise NotImplementedError
-
```

### Comparing `keras-3.2.1/keras/src/backend/torch/trainer.py` & `keras-3.3.0/keras/src/backend/torch/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import numpy as np
 import torch
 from packaging.version import parse
 
 from keras.src import backend
 from keras.src import callbacks as callbacks_module
 from keras.src import optimizers as optimizers_module
+from keras.src import tree
 from keras.src.trainers import trainer as base_trainer
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.epoch_iterator import EpochIterator
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TorchTrainer(base_trainer.Trainer):
     def __init__(self):
         super().__init__()
         self.train_function = None
         self.test_function = None
@@ -248,22 +248,23 @@
             # when implementing a custom layer with torch layers.
             self.train()
             for step, data in epoch_iterator.enumerate_epoch():
                 # Callbacks
                 callbacks.on_train_batch_begin(step)
 
                 logs = self.train_function(data)
+                logs = self._pythonify_logs(logs)
 
                 # Callbacks
-                callbacks.on_train_batch_end(step, self._pythonify_logs(logs))
+                callbacks.on_train_batch_end(step, logs)
                 if self.stop_training:
                     break
 
-            # Override with model metrics instead of last step logs
-            epoch_logs = self.get_metrics_result()
+            # Override with model metrics instead of last step logs if needed.
+            epoch_logs = dict(self._get_metrics_result_or_logs(logs))
 
             # Switch the torch Module back to testing mode.
             self.eval()
 
             # Run validation.
             if validation_data is not None and self._should_eval(
                 epoch, validation_freq
@@ -364,18 +365,19 @@
         self.stop_evaluating = False
         callbacks.on_test_begin()
         logs = None
         self.reset_metrics()
         for step, data in epoch_iterator.enumerate_epoch():
             callbacks.on_test_batch_begin(step)
             logs = self.test_function(data)
-            callbacks.on_test_batch_end(step, self._pythonify_logs(logs))
+            logs = self._pythonify_logs(logs)
+            callbacks.on_test_batch_end(step, logs)
             if self.stop_evaluating:
                 break
-        logs = self.get_metrics_result()
+        logs = self._get_metrics_result_or_logs(logs)
         callbacks.on_test_end(logs)
 
         if return_dict:
             return logs
         return self._flatten_metrics_in_order(logs)
 
     @traceback_utils.filter_traceback
@@ -498,8 +500,7 @@
         )
         return batch_outputs
 
 
 class TorchEpochIterator(EpochIterator):
     def _get_iterator(self):
         return self.data_adapter.get_torch_dataloader()
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/__init__.py` & `keras-3.3.0/keras/src/callbacks/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,8 +9,7 @@
 from keras.src.callbacks.model_checkpoint import ModelCheckpoint
 from keras.src.callbacks.progbar_logger import ProgbarLogger
 from keras.src.callbacks.reduce_lr_on_plateau import ReduceLROnPlateau
 from keras.src.callbacks.remote_monitor import RemoteMonitor
 from keras.src.callbacks.swap_ema_weights import SwapEMAWeights
 from keras.src.callbacks.tensorboard import TensorBoard
 from keras.src.callbacks.terminate_on_nan import TerminateOnNaN
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/backup_and_restore.py` & `keras-3.3.0/keras/src/callbacks/backup_and_restore.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,16 +95,30 @@
                 "Invalid value for argument `save_freq`. "
                 f"Received: save_freq={save_freq}. "
                 "Expected either 'epoch' or an integer value."
             )
 
     def on_train_begin(self, logs=None):
         """Get training state from temporary file and restore it."""
+        if not self.model.built:
+            raise ValueError(
+                "To use the BackupAndRestore callback, "
+                "you model must be built before you call `fit()`. "
+                f"Model {self.model} is unbuilt. You can build it "
+                "beforehand by calling it on a batch of data."
+            )
         if file_utils.exists(self._weights_path):
+            if (
+                self.model.optimizer is not None
+                and not self.model.optimizer.built
+            ):
+                # Make sure optimizer weights exist before loading.
+                self.model.optimizer.build(self.model.trainable_variables)
             self.model.load_weights(self._weights_path)
+
         if file_utils.exists(self._training_metadata_path):
             with file_utils.File(self._training_metadata_path, "r") as f:
                 training_metadata = json.loads(f.read())
             epoch = training_metadata["epoch"]
             self.model._initial_epoch = epoch
 
     def on_epoch_end(self, epoch, logs=None):
@@ -152,8 +166,7 @@
             self._batches_seen_since_last_saving = 0
             return True
         return False
 
     def on_train_end(self, logs=None):
         if self.delete_checkpoint and file_utils.exists(self.backup_dir):
             file_utils.rmtree(self.backup_dir)
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/callback.py` & `keras-3.3.0/keras/src/callbacks/callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,8 +272,7 @@
 
         Subclasses should override for any actions to run.
 
         Args:
             logs: Dict. Currently no data is passed to this argument for this
               method but that may change in the future.
         """
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/callback_list.py` & `keras-3.3.0/keras/src/callbacks/callback_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.callbacks.callback import Callback
 from keras.src.callbacks.history import History
 from keras.src.callbacks.progbar_logger import ProgbarLogger
-from keras.src.utils import tree
 
 
 @keras_export("keras.callbacks.CallbackList")
 class CallbackList(Callback):
     """Container abstracting a list of callbacks."""
 
     def __init__(
@@ -150,8 +150,7 @@
         for callback in self.callbacks:
             callback.on_predict_begin(logs)
 
     def on_predict_end(self, logs=None):
         logs = logs or {}
         for callback in self.callbacks:
             callback.on_predict_end(logs)
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/csv_logger.py` & `keras-3.3.0/keras/src/callbacks/csv_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,7 @@
         )
         self.writer.writerow(row_dict)
         self.csv_file.flush()
 
     def on_train_end(self, logs=None):
         self.csv_file.close()
         self.writer = None
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/early_stopping.py` & `keras-3.3.0/keras/src/callbacks/early_stopping.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,8 +208,7 @@
                 ),
                 stacklevel=2,
             )
         return monitor_value
 
     def _is_improvement(self, monitor_value, reference_value):
         return self.monitor_op(monitor_value - self.min_delta, reference_value)
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/history.py` & `keras-3.3.0/keras/src/callbacks/history.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,8 +36,7 @@
         self.epoch.append(epoch)
         for k, v in logs.items():
             self.history.setdefault(k, []).append(v)
 
         # Set the history attribute on the model after the epoch ends. This will
         # make sure that the state which is set is the latest one.
         self.model.history = self
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/lambda_callback.py` & `keras-3.3.0/keras/src/callbacks/lambda_callback.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,7 @@
             self.on_train_begin = on_train_begin
         if on_train_end is not None:
             self.on_train_end = on_train_end
         if on_train_batch_begin is not None:
             self.on_train_batch_begin = on_train_batch_begin
         if on_train_batch_end is not None:
             self.on_train_batch_end = on_train_batch_end
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/learning_rate_scheduler.py` & `keras-3.3.0/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,8 +75,7 @@
             )
 
     def on_epoch_end(self, epoch, logs=None):
         logs = logs or {}
         logs["learning_rate"] = float(
             backend.convert_to_numpy(self.model.optimizer.learning_rate)
         )
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/model_checkpoint.py` & `keras-3.3.0/keras/src/callbacks/model_checkpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -410,8 +410,7 @@
         if n_file_with_latest_mod_time == 1:
             # Return the sole file that has most recent modified time.
             return file_path_with_latest_mod_time
         else:
             # If there are more than one file having latest modified time,
             # return the file path with the largest file name.
             return file_path_with_largest_file_name
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/progbar_logger.py` & `keras-3.3.0/keras/src/callbacks/progbar_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,8 +96,7 @@
 
     def _finalize_progbar(self, logs):
         logs = logs or {}
         if self.target is None:
             self.target = self.seen
             self.progbar.target = self.target
         self.progbar.update(self.target, list(logs.items()), finalize=True)
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,8 +143,7 @@
                                 f"learning rate to {new_lr}."
                             )
                         self.cooldown_counter = self.cooldown
                         self.wait = 0
 
     def in_cooldown(self):
         return self.cooldown_counter > 0
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/remote_monitor.py` & `keras-3.3.0/keras/src/callbacks/remote_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
                     headers=self.headers,
                 )
         except requests.exceptions.RequestException:
             warnings.warn(
                 f"Could not reach RemoteMonitor root server at {self.root}",
                 stacklevel=2,
             )
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/swap_ema_weights.py` & `keras-3.3.0/keras/src/callbacks/swap_ema_weights.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,8 +174,7 @@
             self._swap_variables()
             self._ema_weights_in_model = True
 
     def on_predict_end(self, logs=None):
         if not self._ema_weights_in_model:
             self._swap_variables()
             self._ema_weights_in_model = False
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/tensorboard.py` & `keras-3.3.0/keras/src/callbacks/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 import os
 import sys
 import time
 import warnings
 
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.callbacks.callback import Callback
 from keras.src.layers import Embedding
 from keras.src.optimizers import Optimizer
 from keras.src.utils import file_utils
-from keras.src.utils import tree
 
 
 @keras_export("keras.callbacks.TensorBoard")
 class TensorBoard(Callback):
     """Enable visualizations for TensorBoard.
 
     TensorBoard is a visualization tool provided with TensorFlow. A TensorFlow
@@ -670,8 +670,7 @@
 
     with summary.experimental.summary_scope(
         name, "graph_keras_model", [data, step]
     ) as (tag, _):
         return summary.write(
             tag=tag, tensor=json_string, step=step, metadata=summary_metadata
         )
-
```

### Comparing `keras-3.2.1/keras/src/callbacks/terminate_on_nan.py` & `keras-3.3.0/keras/src/callbacks/terminate_on_nan.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
         loss = logs.get("loss")
         if loss is not None:
             if np.isnan(loss) or np.isinf(loss):
                 io_utils.print_msg(
                     f"Batch {batch}: Invalid loss, terminating training"
                 )
                 self.model.stop_training = True
-
```

### Comparing `keras-3.2.1/keras/src/constraints/__init__.py` & `keras-3.3.0/keras/src/constraints/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret constraint identifier: {identifier}"
         )
-
```

### Comparing `keras-3.2.1/keras/src/constraints/constraints.py` & `keras-3.3.0/keras/src/constraints/constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,8 +207,7 @@
     def get_config(self):
         return {
             "min_value": self.min_value,
             "max_value": self.max_value,
             "rate": self.rate,
             "axis": self.axis,
         }
-
```

### Comparing `keras-3.2.1/keras/src/datasets/boston_housing.py` & `keras-3.3.0/keras/src/datasets/boston_housing.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     y = y[indices]
 
     x_train = np.array(x[: int(len(x) * (1 - test_split))])
     y_train = np.array(y[: int(len(x) * (1 - test_split))])
     x_test = np.array(x[int(len(x) * (1 - test_split)) :])
     y_test = np.array(y[int(len(x) * (1 - test_split)) :])
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/california_housing.py` & `keras-3.3.0/keras/src/datasets/california_housing.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,8 +98,7 @@
     y = y[indices]
 
     x_train = np.array(x[: int(len(x) * (1 - test_split))])
     y_train = np.array(y[: int(len(x) * (1 - test_split))])
     x_test = np.array(x[int(len(x) * (1 - test_split)) :])
     y_test = np.array(y[int(len(x) * (1 - test_split)) :])
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/cifar.py` & `keras-3.3.0/keras/src/datasets/cifar.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,8 +22,7 @@
             d_decoded[k.decode("utf8")] = v
         d = d_decoded
     data = d["data"]
     labels = d[label_key]
 
     data = data.reshape(data.shape[0], 3, 32, 32)
     return data, labels
-
```

### Comparing `keras-3.2.1/keras/src/datasets/cifar10.py` & `keras-3.3.0/keras/src/datasets/cifar10.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,7 @@
         x_train = x_train.transpose(0, 2, 3, 1)
         x_test = x_test.transpose(0, 2, 3, 1)
 
     x_test = x_test.astype(x_train.dtype)
     y_test = y_test.astype(y_train.dtype)
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/cifar100.py` & `keras-3.3.0/keras/src/datasets/cifar100.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,7 @@
     y_test = np.reshape(y_test, (len(y_test), 1))
 
     if backend.image_data_format() == "channels_last":
         x_train = x_train.transpose(0, 2, 3, 1)
         x_test = x_test.transpose(0, 2, 3, 1)
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/fashion_mnist.py` & `keras-3.3.0/keras/src/datasets/fashion_mnist.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,8 +90,7 @@
 
     with gzip.open(paths[3], "rb") as imgpath:
         x_test = np.frombuffer(imgpath.read(), np.uint8, offset=16).reshape(
             len(y_test), 28, 28
         )
 
     return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/imdb.py` & `keras-3.3.0/keras/src/datasets/imdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,8 +182,7 @@
     path = get_file(
         fname=path,
         origin=origin_folder + "imdb_word_index.json",
         file_hash="bfafd718b763782e994055a2d397834f",
     )
     with open(path) as f:
         return json.load(f)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/mnist.py` & `keras-3.3.0/keras/src/datasets/mnist.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,8 +65,7 @@
         ),
     )
     with np.load(path, allow_pickle=True) as f:
         x_train, y_train = f["x_train"], f["y_train"]
         x_test, y_test = f["x_test"], f["y_test"]
 
         return (x_train, y_train), (x_test, y_test)
-
```

### Comparing `keras-3.2.1/keras/src/datasets/reuters.py` & `keras-3.3.0/keras/src/datasets/reuters.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,8 +214,7 @@
         "dlr",
         "gas",
         "silver",
         "wpi",
         "hog",
         "lead",
     )
-
```

### Comparing `keras-3.2.1/keras/src/distribution/__init__.py` & `keras-3.3.0/keras/src/distribution/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,8 +5,7 @@
 from keras.src.distribution.distribution_lib import ModelParallel
 from keras.src.distribution.distribution_lib import TensorLayout
 from keras.src.distribution.distribution_lib import distribute_tensor
 from keras.src.distribution.distribution_lib import distribution
 from keras.src.distribution.distribution_lib import initialize
 from keras.src.distribution.distribution_lib import list_devices
 from keras.src.distribution.distribution_lib import set_distribution
-
```

### Comparing `keras-3.2.1/keras/src/distribution/distribution_lib.py` & `keras-3.3.0/keras/src/distribution/distribution_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -824,8 +824,7 @@
 def set_distribution(value):
     """Set the distribution as the global distribution setting.
 
     Args:
         value: a `Distribution` instance.
     """
     global_state.set_global_attribute(GLOBAL_ATTRIBUTE_NAME, value)
-
```

### Comparing `keras-3.2.1/keras/src/dtype_policies/dtype_policy.py` & `keras-3.3.0/keras/src/dtype_policies/dtype_policy.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from keras.src import backend
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
 
+QUANTIZATION_MODES = ("int8", "float8")
+
 
 @keras_export(
     [
         "keras.DTypePolicy",
         "keras.dtype_policies.DTypePolicy",
         "keras.mixed_precision.DTypePolicy",  # Legacy
         "keras.mixed_precision.Policy",  # Legacy
@@ -51,25 +53,25 @@
     equivalent to passing
     `dtype=keras.config.DTypePolicy("float32")`.
     In general, passing a dtype policy name to a layer is equivalent
     to passing the corresponding policy, so it is never necessary
     to explicitly construct a `DTypePolicy` object.
     """
 
-    def __new__(cls, name):
+    def __new__(cls, name, *args, **kwargs):
         if not isinstance(name, str):
             raise TypeError(
                 "'name' must be a string, such as 'mixed_float16'. "
                 f"Received: name={name} (of type {type(name)})"
             )
         # For backwards compatibility
         # TODO: We should consider deprecating this behavior
         if cls is __class__:
-            if name.startswith("int8"):
-                return QuantizedDTypePolicy(name)
+            if name.startswith(QUANTIZATION_MODES):
+                return _get_quantized_dtype_policy_by_str(name)
             return FloatDTypePolicy(name)
         return super().__new__(cls)
 
     def __getnewargs__(self):
         # To support `copy`, `deepcopy` and `pickle`
         return (self._name,)
 
@@ -188,43 +190,41 @@
                 "'float32'."
             )
 
     def __repr__(self):
         return f'<FloatDTypePolicy "{self._name}">'
 
 
-@keras_export(
-    ["keras.QuantizedDTypePolicy", "keras.dtype_policies.QuantizedDTypePolicy"]
-)
+@keras_export("keras.dtype_policies.QuantizedDTypePolicy")
 class QuantizedDTypePolicy(DTypePolicy):
     def __init__(self, name):
         super().__init__(name)
         self._quantization_mode, self._compute_dtype, self._variable_dtype = (
             self._parse_name(name)
         )
 
     def _parse_name(self, name):
         error_msg = (
-            f"Cannot convert '{name}' to a QuantizedDTypePolicy. "
-            "Valid policies include "
-            "'int8_from_float32', 'int8_from_float16', 'int8_from_bfloat16', "
-            "'int8_from_mixed_float16', 'int8_from_mixed_bfloat16'."
+            f"Cannot convert '{name}' to a {self.__class__.__name__}. "
+            f"Valid policies are: {self._get_all_valid_policies()}."
         )
         split_name = name.split("_from_")
         if len(split_name) != 2:
             raise ValueError(error_msg)
         mode, from_name = split_name
-        if mode not in ("int8",):
+        if mode not in QUANTIZATION_MODES:
             raise ValueError(error_msg)
-        if from_name == "mixed_float16":
+        if from_name == "mixed_float16" and mode != "int8":
             return mode, "float16", "float32"
         elif from_name == "mixed_bfloat16":
             return mode, "bfloat16", "float32"
         try:
             dtype = backend.standardize_dtype(from_name)
+            if dtype == "float16" and mode == "int8":
+                raise ValueError
             return mode, dtype, dtype
         except ValueError:
             raise ValueError(error_msg)
 
     @property
     def quantization_mode(self):
         """The quantization mode of this policy.
@@ -233,14 +233,75 @@
             The quantization mode of this policy, as a string.
         """
         return self._quantization_mode
 
     def __repr__(self):
         return f'<QuantizedDTypePolicy "{self._name}">'
 
+    def _get_all_valid_policies(self):
+        valid_float_policies = [
+            "float32",
+            "float16",
+            "bfloat16",
+            "mixed_float16",
+            "mixed_bfloat16",
+        ]
+        valid_policies = [
+            f"{mode}_from_{policy}"
+            for mode in ("int8",)
+            for policy in valid_float_policies
+        ]
+        # Remove invalid policies
+        valid_policies.remove("int8_from_float16")
+        valid_policies.remove("int8_from_mixed_float16")
+        return valid_policies
+
+
+@keras_export("keras.dtype_policies.QuantizedFloat8DTypePolicy")
+class QuantizedFloat8DTypePolicy(QuantizedDTypePolicy):
+    def __init__(self, name, amax_history_length=1024):
+        super().__init__(name)
+        if not isinstance(amax_history_length, int):
+            raise TypeError(
+                "`amax_history_length` must be an integer. "
+                f"Received: amax_history_length={amax_history_length}"
+            )
+        self._amax_history_length = amax_history_length
+
+    @property
+    def amax_history_length(self):
+        """The length of the amax history window.
+
+        This property is used for scaling factor computation in float8 training.
+        """
+        return self._amax_history_length
+
+    def __repr__(self):
+        return f'<QuantizedFloat8DTypePolicy "{self._name}">'
+
+    def _get_all_valid_policies(self):
+        valid_float_policies = [
+            "float32",
+            "float16",
+            "bfloat16",
+            "mixed_float16",
+            "mixed_bfloat16",
+        ]
+        valid_policies = [
+            f"{mode}_from_{policy}"
+            for mode in ("float8")
+            for policy in valid_float_policies
+        ]
+        return valid_policies
+
+    def get_config(self):
+        config = super().get_config()
+        config.update({"amax_history_length": self.amax_history_length})
+        return config
+
 
 @keras_export(
     [
         "keras.config.set_dtype_policy",
         "keras.mixed_precision.set_dtype_policy",  # Legacy
         "keras.mixed_precision.set_global_policy",  # Legacy
     ]
@@ -250,16 +311,16 @@
 
     Example:
 
     >>> keras.config.set_dtype_policy("mixed_float16")
     """
     if not isinstance(policy, DTypePolicy):
         if isinstance(policy, str):
-            if policy.startswith("int8"):
-                policy = QuantizedDTypePolicy(policy)
+            if policy.startswith(QUANTIZATION_MODES):
+                policy = _get_quantized_dtype_policy_by_str(policy)
             else:
                 policy = FloatDTypePolicy(policy)
         else:
             raise ValueError(
                 "Invalid `policy` argument. "
                 "Expected the string name of a policy "
                 "(such as 'mixed_float16') or a `DTypePolicy` "
@@ -280,7 +341,21 @@
     """Returns the current default dtype policy object."""
     policy = global_state.get_global_attribute("dtype_policy", None)
     if policy is None:
         policy = FloatDTypePolicy(backend.floatx())
         set_dtype_policy(policy)
     return policy
 
+
+def _get_quantized_dtype_policy_by_str(policy):
+    if not isinstance(policy, str):
+        raise TypeError(f"`policy` must be a string. Received: policy={policy}")
+    if not policy.startswith(QUANTIZATION_MODES):
+        raise ValueError(
+            "`policy` is incompatible with the current supported quantization."
+        )
+    if policy.startswith("int8"):
+        return QuantizedDTypePolicy(policy)
+    elif policy.startswith("float8"):
+        return QuantizedFloat8DTypePolicy(policy)
+    else:
+        raise NotImplementedError
```

### Comparing `keras-3.2.1/keras/src/export/export_lib.py` & `keras-3.3.0/keras/src/export/export_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 import inspect
 import itertools
 import string
 
 from absl import logging
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.stateless_scope import StatelessScope
 from keras.src.layers import Layer
 from keras.src.models import Functional
 from keras.src.models import Sequential
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 from keras.src.utils.module_utils import tensorflow as tf
 
 
 @keras_export("keras.export.ExportArchive")
 class ExportArchive:
     """ExportArchive is used to write SavedModel artifacts (e.g. for inference).
 
@@ -819,8 +819,7 @@
                 if (
                     id(v) not in trainable_variables_ids
                     and id(v) not in non_trainable_variables_ids
                 ):
                     non_trainable_variables.append(v)
                     non_trainable_variables_ids.add(id(v))
     return trainable_variables, non_trainable_variables
-
```

### Comparing `keras-3.2.1/keras/src/initializers/__init__.py` & `keras-3.3.0/keras/src/initializers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,8 +114,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret initializer identifier: {identifier}"
         )
-
```

### Comparing `keras-3.2.1/keras/src/initializers/constant_initializers.py` & `keras-3.3.0/keras/src/initializers/constant_initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,8 +147,7 @@
         if len(shape) != 2:
             raise ValueError(
                 "Identity matrix initializer can only be used for 2D matrices. "
                 f"Received: shape={shape} of rank {len(shape)}."
             )
         dtype = standardize_dtype(dtype)
         return self.gain * ops.eye(*shape, dtype=dtype)
-
```

### Comparing `keras-3.2.1/keras/src/initializers/initializer.py` & `keras-3.3.0/keras/src/initializers/initializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,8 +78,7 @@
         Returns:
             An `Initializer` instance.
         """
         return cls(**config)
 
     def clone(self):
         return self.__class__.from_config(self.get_config())
-
```

### Comparing `keras-3.2.1/keras/src/initializers/random_initializers.py` & `keras-3.3.0/keras/src/initializers/random_initializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -697,8 +697,7 @@
         if num_rows < num_cols:
             q = ops.transpose(q)
         return self.gain * ops.reshape(q, shape)
 
     def get_config(self):
         seed_config = serialization_lib.serialize_keras_object(self._init_seed)
         return {"gain": self.gain, "seed": seed_config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/activation.py` & `keras-3.3.0/keras/src/layers/activations/activation.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = {"activation": activations.serialize(self.activation)}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/elu.py` & `keras-3.3.0/keras/src/layers/activations/elu.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,8 +25,7 @@
         self.supports_masking = True
 
     def call(self, inputs):
         return activations.elu(inputs, alpha=self.alpha)
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/leaky_relu.py` & `keras-3.3.0/keras/src/layers/activations/leaky_relu.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,7 @@
     def get_config(self):
         config = super().get_config()
         config.update({"negative_slope": self.negative_slope})
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/prelu.py` & `keras-3.3.0/keras/src/layers/activations/prelu.py`

 * *Files 0% similar despite different names*

```diff
@@ -93,8 +93,7 @@
                 "shared_axes": self.shared_axes,
             }
         )
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/relu.py` & `keras-3.3.0/keras/src/layers/activations/relu.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,8 +79,7 @@
                 "threshold": self.threshold,
             }
         )
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/layers/activations/softmax.py` & `keras-3.3.0/keras/src/layers/activations/softmax.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,8 +69,7 @@
     def get_config(self):
         config = super().get_config()
         config.update({"axis": self.axis})
         return config
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/layers/attention/additive_attention.py` & `keras-3.3.0/keras/src/layers/attention/additive_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,8 +97,7 @@
         scale = self.scale if self.use_scale else 1.0
         return ops.sum(scale * ops.tanh(q_reshaped + k_reshaped), axis=-1)
 
     def get_config(self):
         base_config = super().get_config()
         del base_config["score_mode"]
         return base_config
-
```

### Comparing `keras-3.2.1/keras/src/layers/attention/attention.py` & `keras-3.3.0/keras/src/layers/attention/attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,8 +276,7 @@
         base_config = super().get_config()
         config = {
             "use_scale": self.use_scale,
             "score_mode": self.score_mode,
             "dropout": self.dropout,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/attention/grouped_query_attention.py` & `keras-3.3.0/keras/src/layers/attention/grouped_query_attention.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,8 +427,7 @@
                 self.activity_regularizer
             ),
             "kernel_constraint": constraints.serialize(self.kernel_constraint),
             "bias_constraint": constraints.serialize(self.bias_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/attention/multi_head_attention.py` & `keras-3.3.0/keras/src/layers/attention/multi_head_attention.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import collections
 import math
 import string
 
 import numpy as np
 
+from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
 from keras.src.api_export import keras_export
 from keras.src.layers.activations.softmax import Softmax
 from keras.src.layers.core.einsum_dense import EinsumDense
@@ -599,14 +600,45 @@
             )
 
         if self._output_shape:
             return query_shape[:-1] + self._output_shape
 
         return query_shape
 
+    def compute_output_spec(
+        self,
+        query,
+        value,
+        key=None,
+        query_mask=None,
+        value_mask=None,
+        key_mask=None,
+        attention_mask=None,
+        return_attention_scores=False,
+        training=None,
+        use_causal_mask=False,
+    ):
+        if key is not None:
+            key_shape = key.shape
+        else:
+            key_shape = None
+        output_shape = self.compute_output_shape(
+            query.shape, value.shape, key_shape
+        )
+        output_spec = backend.KerasTensor(
+            output_shape, dtype=self.compute_dtype
+        )
+        if return_attention_scores:
+            length = query.shape[1]
+            attention_shape = (query.shape[0], self.num_heads, length, length)
+            return output_spec, backend.KerasTensor(
+                attention_shape, dtype=self.compute_dtype
+            )
+        return output_spec
+
 
 def _index_to_einsum_variable(i):
     """Coverts an index to a einsum variable name.
 
     We simply map indices to lowercase characters, e.g. 0 -> 'a', 1 -> 'b'.
     """
     return string.ascii_lowercase[i]
@@ -697,8 +729,7 @@
     equation = f"{input_str},{kernel_str}->{output_str}"
 
     return equation, bias_axes, len(output_str)
 
 
 def _get_output_shape(output_rank, known_last_dims):
     return [None] * (output_rank - len(known_last_dims)) + list(known_last_dims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/base_conv.py` & `keras-3.3.0/keras/src/layers/convolutional/base_conv.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,14 +67,23 @@
             kernel after being updated by an `Optimizer` (e.g. used to implement
             norm constraints or value constraints for layer weights). The
             function must take as input the unprojected variable and must return
             the projected variable (which must have the same shape). Constraints
             are not safe to use when doing asynchronous distributed training.
         bias_constraint: Optional projection function to be applied to the
             bias after being updated by an `Optimizer`.
+        lora_rank: Optional integer. If set, the layer's forward pass
+            will implement LoRA (Low-Rank Adaptation)
+            with the provided rank. LoRA sets the layer's kernel
+            to non-trainable and replaces it with a delta over the
+            original kernel, obtained via multiplying two lower-rank
+            trainable matrices. This can be useful to reduce the
+            computation cost of fine-tuning large dense layers.
+            You can also enable LoRA on an existing layer by calling
+            `layer.enable_lora(rank)`.
     """
 
     def __init__(
         self,
         rank,
         filters,
         kernel_size,
@@ -88,24 +97,18 @@
         kernel_initializer="glorot_uniform",
         bias_initializer="zeros",
         kernel_regularizer=None,
         bias_regularizer=None,
         activity_regularizer=None,
         kernel_constraint=None,
         bias_constraint=None,
-        trainable=True,
-        name=None,
+        lora_rank=None,
         **kwargs,
     ):
-        super().__init__(
-            trainable=trainable,
-            name=name,
-            activity_regularizer=activity_regularizer,
-            **kwargs,
-        )
+        super().__init__(activity_regularizer=activity_regularizer, **kwargs)
         self.rank = rank
         self.filters = filters
         self.groups = groups
         self.kernel_size = standardize_tuple(kernel_size, rank, "kernel_size")
         self.strides = standardize_tuple(strides, rank, "strides")
         self.dilation_rate = standardize_tuple(
             dilation_rate, rank, "dilation_rate"
@@ -116,14 +119,16 @@
         self.use_bias = use_bias
         self.kernel_initializer = initializers.get(kernel_initializer)
         self.bias_initializer = initializers.get(bias_initializer)
         self.kernel_regularizer = regularizers.get(kernel_regularizer)
         self.bias_regularizer = regularizers.get(bias_regularizer)
         self.kernel_constraint = constraints.get(kernel_constraint)
         self.bias_constraint = constraints.get(bias_constraint)
+        self.lora_rank = lora_rank
+        self.lora_enabled = False
         self.input_spec = InputSpec(min_ndim=self.rank + 2)
         self.data_format = self.data_format
 
         if self.filters is not None and self.filters <= 0:
             raise ValueError(
                 "Invalid value for argument `filters`. Expected a strictly "
                 f"positive value. Received filters={self.filters}."
@@ -183,15 +188,15 @@
             self.filters,
         )
 
         # compute_output_shape contains some validation logic for the input
         # shape, and make sure the output shape has all positive dimensions.
         self.compute_output_shape(input_shape)
 
-        self.kernel = self.add_weight(
+        self._kernel = self.add_weight(
             name="kernel",
             shape=kernel_shape,
             initializer=self.kernel_initializer,
             regularizer=self.kernel_regularizer,
             constraint=self.kernel_constraint,
             trainable=True,
             dtype=self.dtype,
@@ -205,14 +210,28 @@
                 constraint=self.bias_constraint,
                 trainable=True,
                 dtype=self.dtype,
             )
         else:
             self.bias = None
         self.built = True
+        if self.lora_rank:
+            self.enable_lora(self.lora_rank)
+
+    @property
+    def kernel(self):
+        if not self.built:
+            raise AttributeError(
+                "You must build the layer before accessing `kernel`."
+            )
+        if self.lora_enabled:
+            return self._kernel + ops.matmul(
+                self.lora_kernel_a, self.lora_kernel_b
+            )
+        return self._kernel
 
     def convolution_op(self, inputs, kernel):
         return ops.conv(
             inputs,
             kernel,
             strides=list(self.strides),
             padding=self.padding,
@@ -244,14 +263,75 @@
             self.kernel_size,
             strides=self.strides,
             padding=self.padding,
             data_format=self.data_format,
             dilation_rate=self.dilation_rate,
         )
 
+    def enable_lora(
+        self, rank, a_initializer="he_uniform", b_initializer="zeros"
+    ):
+        if self.kernel_constraint:
+            raise ValueError(
+                "Lora is incompatible with kernel constraints. "
+                "In order to enable lora on this layer, remove the "
+                "`kernel_constraint` argument."
+            )
+        if not self.built:
+            raise ValueError(
+                "Cannot enable lora on a layer that isn't yet built."
+            )
+        if self.lora_enabled:
+            raise ValueError(
+                "lora is already enabled. "
+                "This can only be done once per layer."
+            )
+        self._tracker.unlock()
+        self.lora_kernel_a = self.add_weight(
+            name="lora_kernel_a",
+            shape=self._kernel.shape[:-1] + (rank,),
+            initializer=initializers.get(a_initializer),
+            regularizer=self.kernel_regularizer,
+        )
+        self.lora_kernel_b = self.add_weight(
+            name="lora_kernel_b",
+            shape=(rank, self.filters),
+            initializer=initializers.get(b_initializer),
+            regularizer=self.kernel_regularizer,
+        )
+        self._kernel.trainable = False
+        self._tracker.lock()
+        self.lora_enabled = True
+        self.lora_rank = rank
+
+    def save_own_variables(self, store):
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        target_variables = [self.kernel]
+        if self.use_bias:
+            target_variables.append(self.bias)
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
+
+    def load_own_variables(self, store):
+        if not self.lora_enabled:
+            self._check_load_own_variables(store)
+        # Do nothing if the layer isn't yet built
+        if not self.built:
+            return
+        target_variables = [self._kernel]
+        if self.use_bias:
+            target_variables.append(self.bias)
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
+        if self.lora_enabled:
+            self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
+            self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
+
     def get_config(self):
         config = super().get_config()
         config.update(
             {
                 "filters": self.filters,
                 "kernel_size": self.kernel_size,
                 "strides": self.strides,
@@ -278,9 +358,44 @@
                 ),
                 "kernel_constraint": constraints.serialize(
                     self.kernel_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
+        if self.lora_rank:
+            config["lora_rank"] = self.lora_rank
         return config
 
+    def _check_load_own_variables(self, store):
+        all_vars = self._trainable_variables + self._non_trainable_variables
+        if len(store.keys()) != len(all_vars):
+            if len(all_vars) == 0 and not self.built:
+                raise ValueError(
+                    f"Layer '{self.name}' was never built "
+                    "and thus it doesn't have any variables. "
+                    f"However the weights file lists {len(store.keys())} "
+                    "variables for this layer.\n"
+                    "In most cases, this error indicates that either:\n\n"
+                    "1. The layer is owned by a parent layer that "
+                    "implements a `build()` method, but calling the "
+                    "parent's `build()` method did NOT create the state of "
+                    f"the child layer '{self.name}'. A `build()` method "
+                    "must create ALL state for the layer, including "
+                    "the state of any children layers.\n\n"
+                    "2. You need to implement "
+                    "the `def build_from_config(self, config)` method "
+                    f"on layer '{self.name}', to specify how to rebuild "
+                    "it during loading. "
+                    "In this case, you might also want to implement the "
+                    "method that generates the build config at saving time, "
+                    "`def get_build_config(self)`. "
+                    "The method `build_from_config()` is meant "
+                    "to create the state "
+                    "of the layer (i.e. its variables) upon deserialization.",
+                )
+            raise ValueError(
+                f"Layer '{self.name}' expected {len(all_vars)} variables, "
+                "but received "
+                f"{len(store.keys())} variables during loading. "
+                f"Expected: {[v.name for v in all_vars]}"
+            )
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-3.3.0/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,8 +253,7 @@
                 "kernel_constraint": constraints.serialize(
                     self.kernel_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-3.3.0/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -268,8 +268,7 @@
                 "depthwise_constraint": constraints.serialize(
                     self.depthwise_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/base_separable_conv.py` & `keras-3.3.0/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -289,8 +289,7 @@
                 "pointwise_constraint": constraints.serialize(
                     self.pointwise_constraint
                 ),
                 "bias_constraint": constraints.serialize(self.bias_constraint),
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv1d.py` & `keras-3.3.0/keras/src/layers/convolutional/conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,8 +162,7 @@
                 bias_shape = (1, self.filters) + (1,) * self.rank
             bias = ops.reshape(self.bias, bias_shape)
             outputs += bias
 
         if self.activation is not None:
             return self.activation(outputs)
         return outputs
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-3.3.0/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,8 +123,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv2d.py` & `keras-3.3.0/keras/src/layers/convolutional/conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,8 +120,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-3.3.0/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,8 +125,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv3d.py` & `keras-3.3.0/keras/src/layers/convolutional/conv3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,8 +126,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-3.3.0/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,7 @@
             kernel_regularizer=kernel_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             kernel_constraint=kernel_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-3.3.0/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,8 +129,7 @@
             depthwise_regularizer=depthwise_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-3.3.0/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,8 +130,7 @@
             depthwise_regularizer=depthwise_regularizer,
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/separable_conv1d.py` & `keras-3.3.0/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,7 @@
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             pointwise_constraint=pointwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/convolutional/separable_conv2d.py` & `keras-3.3.0/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,7 @@
             bias_regularizer=bias_regularizer,
             activity_regularizer=activity_regularizer,
             depthwise_constraint=depthwise_constraint,
             pointwise_constraint=pointwise_constraint,
             bias_constraint=bias_constraint,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/dense.py` & `keras-3.3.0/keras/src/layers/core/embedding.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,243 +1,265 @@
-from keras.src import activations
+import warnings
+
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
 from keras.src import regularizers
 from keras.src.api_export import keras_export
-from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 
 
-@keras_export("keras.layers.Dense")
-class Dense(Layer):
-    """Just your regular densely-connected NN layer.
-
-    `Dense` implements the operation:
-    `output = activation(dot(input, kernel) + bias)`
-    where `activation` is the element-wise activation function
-    passed as the `activation` argument, `kernel` is a weights matrix
-    created by the layer, and `bias` is a bias vector created by the layer
-    (only applicable if `use_bias` is `True`).
-
-    Note: If the input to the layer has a rank greater than 2, `Dense`
-    computes the dot product between the `inputs` and the `kernel` along the
-    last axis of the `inputs` and axis 0 of the `kernel` (using `tf.tensordot`).
-    For example, if input has dimensions `(batch_size, d0, d1)`, then we create
-    a `kernel` with shape `(d1, units)`, and the `kernel` operates along axis 2
-    of the `input`, on every sub-tensor of shape `(1, 1, d1)` (there are
-    `batch_size * d0` such sub-tensors). The output in this case will have
-    shape `(batch_size, d0, units)`.
+@keras_export("keras.layers.Embedding")
+class Embedding(Layer):
+    """Turns positive integers (indexes) into dense vectors of fixed size.
+
+    e.g. `[[4], [20]] -> [[0.25, 0.1], [0.6, -0.2]]`
+
+    This layer can only be used on positive integer inputs of a fixed range.
+
+    Example:
+
+    >>> model = keras.Sequential()
+    >>> model.add(keras.layers.Embedding(1000, 64))
+    >>> # The model will take as input an integer matrix of size (batch,
+    >>> # input_length), and the largest integer (i.e. word index) in the input
+    >>> # should be no larger than 999 (vocabulary size).
+    >>> # Now model.output_shape is (None, 10, 64), where `None` is the batch
+    >>> # dimension.
+    >>> input_array = np.random.randint(1000, size=(32, 10))
+    >>> model.compile('rmsprop', 'mse')
+    >>> output_array = model.predict(input_array)
+    >>> print(output_array.shape)
+    (32, 10, 64)
 
     Args:
-        units: Positive integer, dimensionality of the output space.
-        activation: Activation function to use.
-            If you don't specify anything, no activation is applied
-            (ie. "linear" activation: `a(x) = x`).
-        use_bias: Boolean, whether the layer uses a bias vector.
-        kernel_initializer: Initializer for the `kernel` weights matrix.
-        bias_initializer: Initializer for the bias vector.
-        kernel_regularizer: Regularizer function applied to
-            the `kernel` weights matrix.
-        bias_regularizer: Regularizer function applied to the bias vector.
-        activity_regularizer: Regularizer function applied to
-            the output of the layer (its "activation").
-        kernel_constraint: Constraint function applied to
-            the `kernel` weights matrix.
-        bias_constraint: Constraint function applied to the bias vector.
+        input_dim: Integer. Size of the vocabulary,
+            i.e. maximum integer index + 1.
+        output_dim: Integer. Dimension of the dense embedding.
+        embeddings_initializer: Initializer for the `embeddings`
+            matrix (see `keras.initializers`).
+        embeddings_regularizer: Regularizer function applied to
+            the `embeddings` matrix (see `keras.regularizers`).
+        embeddings_constraint: Constraint function applied to
+            the `embeddings` matrix (see `keras.constraints`).
+        mask_zero: Boolean, whether or not the input value 0 is a special
+            "padding" value that should be masked out.
+            This is useful when using recurrent layers which
+            may take variable length input. If this is `True`,
+            then all subsequent layers in the model need
+            to support masking or an exception will be raised.
+            If `mask_zero` is set to `True`, as a consequence,
+            index 0 cannot be used in the vocabulary (`input_dim` should
+            equal size of vocabulary + 1).
+        weights: Optional floating-point matrix of size
+            `(input_dim, output_dim)`. The initial embeddings values
+            to use.
         lora_rank: Optional integer. If set, the layer's forward pass
             will implement LoRA (Low-Rank Adaptation)
-            with the provided rank. LoRA sets the layer's kernel
-            to non-trainable and replaces it with a delta over the
-            original kernel, obtained via multiplying two lower-rank
+            with the provided rank. LoRA sets the layer's embeddings
+            matrix to non-trainable and replaces it with a delta over the
+            original matrix, obtained via multiplying two lower-rank
             trainable matrices. This can be useful to reduce the
-            computation cost of fine-tuning large dense layers.
+            computation cost of fine-tuning large embedding layers.
             You can also enable LoRA on an existing
-            `Dense` layer by calling `layer.enable_lora(rank)`.
+            `Embedding` layer by calling `layer.enable_lora(rank)`.
 
     Input shape:
-        N-D tensor with shape: `(batch_size, ..., input_dim)`.
-        The most common situation would be
-        a 2D input with shape `(batch_size, input_dim)`.
+        2D tensor with shape: `(batch_size, input_length)`.
 
     Output shape:
-        N-D tensor with shape: `(batch_size, ..., units)`.
-        For instance, for a 2D input with shape `(batch_size, input_dim)`,
-        the output would have shape `(batch_size, units)`.
+        3D tensor with shape: `(batch_size, input_length, output_dim)`.
     """
 
     def __init__(
         self,
-        units,
-        activation=None,
-        use_bias=True,
-        kernel_initializer="glorot_uniform",
-        bias_initializer="zeros",
-        kernel_regularizer=None,
-        bias_regularizer=None,
-        activity_regularizer=None,
-        kernel_constraint=None,
-        bias_constraint=None,
+        input_dim,
+        output_dim,
+        embeddings_initializer="uniform",
+        embeddings_regularizer=None,
+        embeddings_constraint=None,
+        mask_zero=False,
+        weights=None,
         lora_rank=None,
         **kwargs,
     ):
-        super().__init__(activity_regularizer=activity_regularizer, **kwargs)
-        self.units = units
-        self.activation = activations.get(activation)
-        self.use_bias = use_bias
-        self.kernel_initializer = initializers.get(kernel_initializer)
-        self.bias_initializer = initializers.get(bias_initializer)
-        self.kernel_regularizer = regularizers.get(kernel_regularizer)
-        self.bias_regularizer = regularizers.get(bias_regularizer)
-        self.kernel_constraint = constraints.get(kernel_constraint)
-        self.bias_constraint = constraints.get(bias_constraint)
+        input_length = kwargs.pop("input_length", None)
+        if input_length is not None:
+            warnings.warn(
+                "Argument `input_length` is deprecated. Just remove it."
+            )
+        super().__init__(**kwargs)
+        self.input_dim = input_dim
+        self.output_dim = output_dim
+        self.embeddings_initializer = initializers.get(embeddings_initializer)
+        self.embeddings_regularizer = regularizers.get(embeddings_regularizer)
+        self.embeddings_constraint = constraints.get(embeddings_constraint)
+        self.mask_zero = mask_zero
+        self.supports_masking = mask_zero
+        self.autocast = False
         self.lora_rank = lora_rank
         self.lora_enabled = False
-        self.input_spec = InputSpec(min_ndim=2)
-        self.supports_masking = True
 
-    def build(self, input_shape):
-        input_dim = input_shape[-1]
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        if weights is not None:
+            self.build()
+            if not (isinstance(weights, list) and len(weights) == 1):
+                weights = [weights]
+            self.set_weights(weights)
+
+    def build(self, input_shape=None):
+        if self.built:
+            return
+        # We use `self._dtype_policy` to check to avoid issues in torch dynamo
+        is_quantized = isinstance(
+            self._dtype_policy, dtype_policies.QuantizedDTypePolicy
+        )
+        if is_quantized:
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
-        else:
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=(input_dim, self.units),
-                initializer=self.kernel_initializer,
-                regularizer=self.kernel_regularizer,
-                constraint=self.kernel_constraint,
-            )
-        if self.use_bias:
-            self.bias = self.add_weight(
-                name="bias",
-                shape=(self.units,),
-                initializer=self.bias_initializer,
-                regularizer=self.bias_regularizer,
-                constraint=self.bias_constraint,
+        if not is_quantized or self.dtype_policy.quantization_mode != "int8":
+            self._embeddings = self.add_weight(
+                shape=(self.input_dim, self.output_dim),
+                initializer=self.embeddings_initializer,
+                name="embeddings",
+                regularizer=self.embeddings_regularizer,
+                constraint=self.embeddings_constraint,
+                trainable=True,
             )
-        else:
-            self.bias = None
-        self.input_spec = InputSpec(min_ndim=2, axes={-1: input_dim})
         self.built = True
         if self.lora_rank:
             self.enable_lora(self.lora_rank)
 
     @property
-    def kernel(self):
-        if not self.built:
-            raise AttributeError(
-                "You must build the layer before accessing `kernel`."
-            )
+    def embeddings(self):
         if self.lora_enabled:
-            return self._kernel + ops.matmul(
-                self.lora_kernel_a, self.lora_kernel_b
+            return self._embeddings + ops.matmul(
+                self.lora_embeddings_a, self.lora_embeddings_b
             )
-        return self._kernel
+        return self._embeddings
 
     def call(self, inputs):
-        x = ops.matmul(inputs, self.kernel)
-        if self.bias is not None:
-            x = ops.add(x, self.bias)
-        if self.activation is not None:
-            x = self.activation(x)
-        return x
+        if inputs.dtype != "int32" and inputs.dtype != "int64":
+            inputs = ops.cast(inputs, "int32")
+        outputs = ops.take(self.embeddings, inputs, axis=0)
+        return ops.cast(outputs, dtype=self.compute_dtype)
+
+    def compute_mask(self, inputs, mask=None):
+        if not self.mask_zero:
+            return None
+        return ops.not_equal(inputs, 0)
 
     def compute_output_shape(self, input_shape):
-        output_shape = list(input_shape)
-        output_shape[-1] = self.units
-        return tuple(output_shape)
+        return input_shape + (self.output_dim,)
 
     def enable_lora(
         self, rank, a_initializer="he_uniform", b_initializer="zeros"
     ):
-        if self.kernel_constraint:
+        if self.embeddings_constraint:
             raise ValueError(
-                "Lora is incompatible with kernel constraints. "
+                "Lora is incompatible with embedding constraints. "
                 "In order to enable lora on this layer, remove the "
-                "`kernel_constraint` argument."
+                "`embeddings_constraint` argument."
             )
         if not self.built:
             raise ValueError(
                 "Cannot enable lora on a layer that isn't yet built."
             )
         if self.lora_enabled:
             raise ValueError(
                 "lora is already enabled. "
                 "This can only be done once per layer."
             )
         self._tracker.unlock()
-        self.lora_kernel_a = self.add_weight(
-            name="lora_kernel_a",
-            shape=(self.kernel.shape[0], rank),
+        self.lora_embeddings_a = self.add_weight(
+            name="lora_embeddings_a",
+            shape=(self.embeddings.shape[0], rank),
             initializer=initializers.get(a_initializer),
-            regularizer=self.kernel_regularizer,
+            regularizer=self.embeddings_regularizer,
         )
-        self.lora_kernel_b = self.add_weight(
-            name="lora_kernel_b",
-            shape=(rank, self.kernel.shape[1]),
+        self.lora_embeddings_b = self.add_weight(
+            name="lora_embeddings_b",
+            shape=(rank, self.embeddings.shape[1]),
             initializer=initializers.get(b_initializer),
-            regularizer=self.kernel_regularizer,
+            regularizer=self.embeddings_regularizer,
         )
-        self._kernel.trainable = False
+        self.embeddings.trainable = False
         self._tracker.lock()
         self.lora_enabled = True
         self.lora_rank = rank
 
     def save_own_variables(self, store):
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
-        store["0"] = kernel_value
-        if self.use_bias:
-            store["1"] = self.bias
+        embeddings_value, embeddings_scale = (
+            self._get_embeddings_with_merged_lora()
+        )
+        target_variables = [embeddings_value]
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            store["2"] = kernel_scale
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                target_variables.append(embeddings_scale)
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        self._kernel.assign(store["0"])
-        if self.use_bias:
-            self.bias.assign(store["1"])
+        target_variables = [self._embeddings]
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.kernel_scale.assign(store["2"])
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                target_variables.append(self.embeddings_scale)
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
-            self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
-            self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
+            self.lora_embeddings_a.assign(
+                ops.zeros(self.lora_embeddings_a.shape)
+            )
+            self.lora_embeddings_b.assign(
+                ops.zeros(self.lora_embeddings_b.shape)
+            )
 
     def get_config(self):
         base_config = super().get_config()
         config = {
-            "units": self.units,
-            "activation": activations.serialize(self.activation),
-            "use_bias": self.use_bias,
-            "kernel_initializer": initializers.serialize(
-                self.kernel_initializer
+            "input_dim": self.input_dim,
+            "output_dim": self.output_dim,
+            "embeddings_initializer": initializers.serialize(
+                self.embeddings_initializer
+            ),
+            "embeddings_regularizer": regularizers.serialize(
+                self.embeddings_regularizer
             ),
-            "bias_initializer": initializers.serialize(self.bias_initializer),
-            "kernel_regularizer": regularizers.serialize(
-                self.kernel_regularizer
+            "activity_regularizer": regularizers.serialize(
+                self.activity_regularizer
             ),
-            "bias_regularizer": regularizers.serialize(self.bias_regularizer),
-            "kernel_constraint": constraints.serialize(self.kernel_constraint),
-            "bias_constraint": constraints.serialize(self.bias_constraint),
+            "embeddings_constraint": constraints.serialize(
+                self.embeddings_constraint
+            ),
+            "mask_zero": self.mask_zero,
         }
         if self.lora_rank:
             config["lora_rank"] = self.lora_rank
         return {**base_config, **config}
 
     def _check_load_own_variables(self, store):
         all_vars = self._trainable_variables + self._non_trainable_variables
@@ -269,137 +291,136 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related methods"""
+    """Quantization-related (int8) methods"""
+
+    QUANTIZATION_MODE_ERROR_TEMPLATE = (
+        "Invalid quantization mode. Expected 'int8'. "
+        "Received: quantization_mode={mode}"
+    )
 
     def quantized_build(self, input_shape, mode):
-        input_dim = input_shape[-1]
         if mode == "int8":
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=(input_dim, self.units),
-                initializer="zeros",
-                dtype="int8",
-                trainable=False,
-            )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=(self.units,),
-                initializer="ones",
-                trainable=False,
+            self._int8_build()
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
+    def _int8_build(
+        self,
+        embeddings_initializer="zeros",
+        embeddings_scale_initializer="ones",
+    ):
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+        self._embeddings = self.add_weight(
+            name="embeddings",
+            shape=(self.input_dim, self.output_dim),
+            initializer=embeddings_initializer,
+            dtype="int8",
+            trainable=False,
+        )
+        self.embeddings_scale = self.add_weight(
+            name="embeddings_scale",
+            shape=(self.output_dim,),
+            initializer=embeddings_scale_initializer,
+            trainable=False,
+        )
+        self._is_quantized = True
+
     def quantized_call(self, inputs):
-        @ops.custom_gradient
-        def matmul_with_inputs_gradient(inputs, kernel, kernel_scale):
-            def grad_fn(*args, upstream=None):
-                if upstream is None:
-                    (upstream,) = args
-                float_kernel = ops.divide(
-                    ops.cast(kernel, dtype=self.compute_dtype),
-                    kernel_scale,
-                )
-                inputs_grad = ops.matmul(upstream, ops.transpose(float_kernel))
-                return (inputs_grad, None, None)
+        if self.dtype_policy.quantization_mode == "int8":
+            return self._int8_call(inputs)
+        else:
+            mode = self.dtype_policy.quantization_mode
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
 
-            inputs, inputs_scale = self.inputs_quantizer(inputs)
-            x = ops.matmul(inputs, kernel)
-            # De-scale outputs
-            x = ops.cast(x, self.compute_dtype)
-            x = ops.divide(x, ops.multiply(inputs_scale, kernel_scale))
-            return x, grad_fn
-
-        x = matmul_with_inputs_gradient(
-            inputs,
-            ops.convert_to_tensor(self._kernel),
-            ops.convert_to_tensor(self.kernel_scale),
+    def _int8_call(self, inputs):
+        # We cannot update quantized self._embeddings, so the custom gradient is
+        # not needed
+        if backend.standardize_dtype(inputs.dtype) not in ("int32", "int64"):
+            inputs = ops.cast(inputs, "int32")
+        outputs = ops.take(self._embeddings, inputs, axis=0)
+        # De-scale outputs
+        outputs = ops.cast(outputs, self.compute_dtype)
+        outputs = ops.divide(
+            outputs, ops.expand_dims(self.embeddings_scale, axis=0)
         )
         if self.lora_enabled:
-            lora_x = ops.matmul(inputs, self.lora_kernel_a)
-            lora_x = ops.matmul(lora_x, self.lora_kernel_b)
-            x = ops.add(x, lora_x)
-        if self.bias is not None:
-            x = ops.add(x, self.bias)
-        if self.activation is not None:
-            x = self.activation(x)
-        return x
+            lora_outputs = ops.take(self.lora_embeddings_a, inputs, axis=0)
+            lora_outputs = ops.matmul(lora_outputs, self.lora_embeddings_b)
+            outputs = ops.add(outputs, lora_outputs)
+        return outputs
 
     def quantize(self, mode):
         import gc
 
         # Prevent quantization of the subclasses
-        if type(self) is not Dense:
+        if type(self) is not Embedding:
             raise NotImplementedError(
                 f"Layer {self.__class__.__name__} does not have a `quantize()` "
                 "method implemented."
             )
         self._check_quantize_args(mode, self.compute_dtype)
-        if mode == "int8":
-            if backend.standardize_dtype(self._kernel.dtype) == "int8":
-                raise ValueError("`quantize` can only be done once per layer.")
-            # Configure `self.inputs_quantizer`
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            # Quantize `self._kernel` to int8 and compute corresponding scale
-            kernel_value, kernel_scale = quantizers.abs_max_quantize(
-                self._kernel, axis=0
-            )
-            kernel_scale = ops.squeeze(kernel_scale, axis=0)
-            self._tracker.unlock()
-            self._untrack_variable(self._kernel)
-            kernel_shape = self._kernel.shape
-            del self._kernel
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_value,
-                dtype="int8",
-                trainable=False,
-            )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=(self.units,),
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_scale,
-                trainable=False,
-            )
-            self._tracker.lock()
-        else:
-            NotImplementedError(
-                "Invalid quantization mode. Expected 'int8'. "
-                f"Received: mode={mode}"
-            )
 
         # Set new dtype policy
         if not isinstance(
             self.dtype_policy, dtype_policies.QuantizedDTypePolicy
         ):
             quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
-            self.dtype_policy = dtype_policies.get(quantized_dtype)
+            # We set the internal `self._dtype_policy` instead of using the
+            # setter to avoid double `quantize` call
+            self._dtype_policy = dtype_policies.get(quantized_dtype)
+
+        self._tracker.unlock()
+        if mode == "int8":
+            # Configure `self.inputs_quantizer`
+            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
+            # Quantize `self._embeddings` to int8 and compute corresponding
+            # scale
+            embeddings_value, embeddings_scale = quantizers.abs_max_quantize(
+                self._embeddings, axis=0
+            )
+            embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+            self._untrack_variable(self._embeddings)
+            del self._embeddings
+            # Utilize a lambda expression as an initializer to prevent adding a
+            # large constant to the computation graph.
+            self._int8_build(
+                lambda shape, dtype: embeddings_value,
+                lambda shape, dtype: embeddings_scale,
+            )
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+        self._tracker.lock()
 
         # Release memory manually because sometimes the backend doesn't
         gc.collect()
 
-    def _get_kernel_with_merged_lora(self):
+    def _get_embeddings_with_merged_lora(self):
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            kernel_value = self._kernel
-            kernel_scale = self.kernel_scale
+            embeddings_value = self._embeddings
+            embeddings_scale = self.embeddings_scale
             if self.lora_enabled:
-                # Dequantize & quantize to merge lora weights into int8 kernel
+                # Dequantize & quantize to merge lora weights into embeddings
                 # Note that this is a lossy compression
-                kernel_value = ops.divide(kernel_value, kernel_scale)
-                kernel_value = ops.add(
-                    kernel_value,
-                    ops.matmul(self.lora_kernel_a, self.lora_kernel_b),
+                embeddings_value = ops.divide(
+                    embeddings_value, embeddings_scale
                 )
-                kernel_value, kernel_scale = quantizers.abs_max_quantize(
-                    kernel_value, axis=0
+                embeddings_value = ops.add(
+                    embeddings_value,
+                    ops.matmul(self.lora_embeddings_a, self.lora_embeddings_b),
                 )
-                kernel_scale = ops.squeeze(kernel_scale, axis=0)
-            return kernel_value, kernel_scale
-        return self.kernel, None
-
+                embeddings_value, embeddings_scale = (
+                    quantizers.abs_max_quantize(embeddings_value, axis=0)
+                )
+                embeddings_scale = ops.squeeze(embeddings_scale, axis=0)
+            return embeddings_value, embeddings_scale
+        return self.embeddings, None
```

### Comparing `keras-3.2.1/keras/src/layers/core/einsum_dense.py` & `keras-3.3.0/keras/src/layers/core/einsum_dense.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import re
 import string
 
+import ml_dtypes
 import numpy as np
 
 from keras.src import activations
-from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import ops
 from keras.src import quantizers
 from keras.src import regularizers
 from keras.src.api_export import keras_export
@@ -149,21 +149,27 @@
             self.equation,
             self.bias_axes,
             input_shape,
             self.partial_output_shape,
         )
         kernel_shape, bias_shape, full_output_shape = shape_data
         self.full_output_shape = tuple(full_output_shape)
-        # `quantized_build` needs `self.input_spec`
+        # `self._int8_build` needs `self.input_spec`
         self.input_spec = InputSpec(ndim=len(input_shape))
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        # We use `self._dtype_policy` to check to avoid issues in torch dynamo
+        is_quantized = isinstance(
+            self._dtype_policy, dtype_policies.QuantizedDTypePolicy
+        )
+        if is_quantized:
             self.quantized_build(
                 input_shape, mode=self.dtype_policy.quantization_mode
             )
-        else:
+        if not is_quantized or self.dtype_policy.quantization_mode != "int8":
+            # If the layer is quantized to int8, `self._kernel` will be added
+            # in `self._int8_build`. Therefore, we skip it here.
             self._kernel = self.add_weight(
                 name="kernel",
                 shape=tuple(kernel_shape),
                 initializer=self.kernel_initializer,
                 regularizer=self.kernel_regularizer,
                 constraint=self.kernel_constraint,
                 dtype=self.dtype,
@@ -247,33 +253,63 @@
     def save_own_variables(self, store):
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
         kernel_value, kernel_scale = self._get_kernel_with_merged_lora()
-        store["0"] = kernel_value
+        target_variables = [kernel_value]
         if self.bias is not None:
-            store["1"] = self.bias
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            store["2"] = kernel_scale
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                target_variables.append(kernel_scale)
+            elif mode == "float8":
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
+        for i, variable in enumerate(target_variables):
+            store[str(i)] = variable
 
     def load_own_variables(self, store):
         if not self.lora_enabled:
             self._check_load_own_variables(store)
         # Do nothing if the layer isn't yet built
         if not self.built:
             return
         # The keys of the `store` will be saved as determined because the
         # default ordering will change after quantization
-        self._kernel.assign(store["0"])
+        target_variables = [self._kernel]
         if self.bias is not None:
-            self.bias.assign(store["1"])
+            target_variables.append(self.bias)
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
-            self.kernel_scale.assign(store["2"])
+            mode = self.dtype_policy.quantization_mode
+            if mode == "int8":
+                target_variables.append(self.kernel_scale)
+            elif mode == "float8":
+                target_variables.append(self.inputs_scale)
+                target_variables.append(self.inputs_amax_history)
+                target_variables.append(self.kernel_scale)
+                target_variables.append(self.kernel_amax_history)
+                target_variables.append(self.outputs_grad_scale)
+                target_variables.append(self.outputs_grad_amax_history)
+            else:
+                raise NotImplementedError(
+                    self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+                )
+        for i, variable in enumerate(target_variables):
+            variable.assign(store[str(i)])
         if self.lora_enabled:
             self.lora_kernel_a.assign(ops.zeros(self.lora_kernel_a.shape))
             self.lora_kernel_b.assign(ops.zeros(self.lora_kernel_b.shape))
 
     def get_config(self):
         base_config = super().get_config()
         config = {
@@ -329,61 +365,145 @@
             raise ValueError(
                 f"Layer '{self.name}' expected {len(all_vars)} variables, "
                 "but received "
                 f"{len(store.keys())} variables during loading. "
                 f"Expected: {[v.name for v in all_vars]}"
             )
 
-    """Quantization-related methods"""
+    """Quantization-related (int8 and float8) methods"""
+
+    QUANTIZATION_MODE_ERROR_TEMPLATE = (
+        f"Invalid quantization mode. Expected one of "
+        f"{dtype_policies.QUANTIZATION_MODES}. "
+        "Received: quantization_mode={mode}"
+    )
 
     def quantized_build(self, input_shape, mode):
-        shape_data = _analyze_einsum_string(
-            self.equation,
-            self.bias_axes,
-            input_shape,
-            self.partial_output_shape,
-        )
-        kernel_shape, _, _ = shape_data
         if mode == "int8":
-            (
-                self._input_reduced_axes,
-                self._kernel_reduced_axes,
-                self._input_transpose_axes,
-                self._kernel_transpose_axes,
-                self._input_expand_axes,
-                self._kernel_expand_axes,
-                self._input_squeeze_axes,
-                self._kernel_squeeze_axes,
-                self._custom_gradient_equation,
-                self._kernel_reverse_transpose_axes,
-            ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
-            self.inputs_quantizer = quantizers.AbsMaxQuantizer(axis=-1)
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                initializer="zeros",
-                dtype="int8",
-                trainable=False,
-            )
-            kernel_scale_shape = np.array(kernel_shape)
-            kernel_scale_shape[self._kernel_reduced_axes] = 1
-            kernel_scale_shape = kernel_scale_shape[self._kernel_transpose_axes]
-            kernel_scale_shape = kernel_scale_shape.tolist()
-            for a in sorted(self._kernel_expand_axes):
-                kernel_scale_shape.insert(a, 1)
-            for a in sorted(self._kernel_squeeze_axes, reverse=True):
-                kernel_scale_shape.pop(a)
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=kernel_scale_shape,
-                initializer="ones",
-                trainable=False,
+            shape_data = _analyze_einsum_string(
+                self.equation,
+                self.bias_axes,
+                input_shape,
+                self.partial_output_shape,
+            )
+            kernel_shape, _, _ = shape_data
+            self._int8_build(kernel_shape)
+        elif mode == "float8":
+            self._float8_build()
+        else:
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
             )
 
+    def _int8_build(
+        self,
+        kernel_shape,
+        kernel_initializer="zeros",
+        kernel_scale_initializer="ones",
+    ):
+        (
+            self._input_reduced_axes,
+            self._kernel_reduced_axes,
+            self._input_transpose_axes,
+            self._kernel_transpose_axes,
+            self._input_expand_axes,
+            self._kernel_expand_axes,
+            self._input_squeeze_axes,
+            self._kernel_squeeze_axes,
+            self._custom_gradient_equation,
+            self._kernel_reverse_transpose_axes,
+        ) = _analyze_quantization_info(self.equation, self.input_spec.ndim)
+        self.inputs_quantizer = quantizers.AbsMaxQuantizer(
+            axis=self._input_reduced_axes
+        )
+        self._kernel = self.add_weight(
+            name="kernel",
+            shape=kernel_shape,
+            initializer=kernel_initializer,
+            dtype="int8",
+            trainable=False,
+        )
+        kernel_scale_shape = np.array(kernel_shape)
+        kernel_scale_shape[self._kernel_reduced_axes] = 1
+        kernel_scale_shape = kernel_scale_shape[self._kernel_transpose_axes]
+        kernel_scale_shape = kernel_scale_shape.tolist()
+        for a in sorted(self._kernel_expand_axes):
+            kernel_scale_shape.insert(a, 1)
+        for a in sorted(self._kernel_squeeze_axes, reverse=True):
+            kernel_scale_shape.pop(a)
+        self.kernel_scale = self.add_weight(
+            name="kernel_scale",
+            shape=kernel_scale_shape,
+            initializer=kernel_scale_initializer,
+            trainable=False,
+        )
+        self._is_quantized = True
+
+    def _float8_build(self):
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedFloat8DTypePolicy
+        ):
+            raise TypeError(
+                "`self.dtype_policy` must be the type of "
+                f"QuantizedFloat8DTypePolicy. Received {self.dtype_policy}"
+            )
+        amax_history_length = self.dtype_policy.amax_history_length
+        # We set `trainable=True` because we will use the gradients to overwrite
+        # these variables
+        scale_kwargs = {
+            "shape": (),
+            "initializer": "ones",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        amax_history_kwargs = {
+            "shape": (amax_history_length,),
+            "initializer": "zeros",
+            "dtype": "float32",  # Always be float32
+            "trainable": True,
+            "autocast": False,
+        }
+        self.inputs_scale = self.add_weight(name="inputs_scale", **scale_kwargs)
+        self.inputs_amax_history = self.add_weight(
+            name="inputs_amax_history", **amax_history_kwargs
+        )
+        self.kernel_scale = self.add_weight(name="kernel_scale", **scale_kwargs)
+        self.kernel_amax_history = self.add_weight(
+            name="kernel_amax_history", **amax_history_kwargs
+        )
+        self.outputs_grad_scale = self.add_weight(
+            name="outputs_grad_scale", **scale_kwargs
+        )
+        self.outputs_grad_amax_history = self.add_weight(
+            name="outputs_grad_amax_history", **amax_history_kwargs
+        )
+        # We need to set `overwrite_with_gradient=True` to instruct the
+        # optimizer to directly overwrite these variables with their computed
+        # gradients during training
+        self.inputs_scale.overwrite_with_gradient = True
+        self.inputs_amax_history.overwrite_with_gradient = True
+        self.kernel_scale.overwrite_with_gradient = True
+        self.kernel_amax_history.overwrite_with_gradient = True
+        self.outputs_grad_scale.overwrite_with_gradient = True
+        self.outputs_grad_amax_history.overwrite_with_gradient = True
+        self._is_quantized = True
+
     def quantized_call(self, inputs):
+        if self.dtype_policy.quantization_mode == "int8":
+            return self._int8_call(inputs)
+        elif self.dtype_policy.quantization_mode == "float8":
+            return self._float8_call(inputs)
+        else:
+            mode = self.dtype_policy.quantization_mode
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+
+    def _int8_call(self, inputs):
         @ops.custom_gradient
         def einsum_with_inputs_gradient(inputs, kernel, kernel_scale):
             def grad_fn(*args, upstream=None):
                 if upstream is None:
                     (upstream,) = args
                 # De-scale kernel
                 _kernel_scale = kernel_scale  # Overcome UnboundLocalError
@@ -438,27 +558,124 @@
             x = ops.add(x, lora_x)
         if self.bias is not None:
             x += self.bias
         if self.activation is not None:
             x = self.activation(x)
         return x
 
+    def _float8_call(self, inputs):
+        if self.lora_enabled:
+            raise NotImplementedError(
+                "Currently, `_float8_call` doesn't support LoRA"
+            )
+
+        @ops.custom_gradient
+        def quantized_dequantize_inputs(inputs, scale, amax_history):
+            new_scale = quantizers.compute_float8_scale(
+                ops.max(amax_history, axis=0),
+                scale,
+                ops.cast(
+                    float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
+                ),
+            )
+            qdq_inputs = quantizers.quantize_and_dequantize(
+                inputs, scale, "float8_e4m3fn", self.compute_dtype
+            )
+            new_amax_history = quantizers.compute_float8_amax_history(
+                inputs, amax_history
+            )
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                return upstream, new_scale, new_amax_history
+
+            return qdq_inputs, grad
+
+        @ops.custom_gradient
+        def quantized_dequantize_outputs(outputs, scale, amax_history):
+            """Quantize-dequantize the output gradient but not the output."""
+
+            def grad(*args, upstream=None, variables=None):
+                if upstream is None:
+                    (upstream,) = args
+                new_scale = quantizers.compute_float8_scale(
+                    ops.max(amax_history, axis=0),
+                    scale,
+                    ops.cast(
+                        float(ml_dtypes.finfo("float8_e5m2").max), "float32"
+                    ),
+                )
+                qdq_upstream = quantizers.quantize_and_dequantize(
+                    upstream, scale, "float8_e5m2", self.compute_dtype
+                )
+                new_amax_history = quantizers.compute_float8_amax_history(
+                    upstream, amax_history
+                )
+                return qdq_upstream, new_scale, new_amax_history
+
+            return outputs, grad
+
+        x = ops.einsum(
+            self.equation,
+            quantized_dequantize_inputs(
+                inputs,
+                ops.convert_to_tensor(self.inputs_scale),
+                ops.convert_to_tensor(self.inputs_amax_history),
+            ),
+            quantized_dequantize_inputs(
+                ops.convert_to_tensor(self._kernel),
+                ops.convert_to_tensor(self.kernel_scale),
+                ops.convert_to_tensor(self.kernel_amax_history),
+            ),
+        )
+        # `quantized_dequantize_outputs` is placed immediately after
+        # `ops.einsum` for the sake of pattern matching in gemm_rewrite. That
+        # way, the qdq will be adjacent to the corresponding einsum_bprop in the
+        # bprop.
+        x = quantized_dequantize_outputs(
+            x,
+            ops.convert_to_tensor(self.outputs_grad_scale),
+            ops.convert_to_tensor(self.outputs_grad_amax_history),
+        )
+        if self.bias is not None:
+            # Under non-mixed precision cases, F32 bias has to be converted to
+            # BF16 first to get the biasAdd fusion support. ref. PR
+            # https://github.com/tensorflow/tensorflow/pull/60306
+            bias = self.bias
+            if self.dtype_policy.compute_dtype == "float32":
+                bias_bf16 = ops.cast(bias, "bfloat16")
+                bias = ops.cast(bias_bf16, bias.dtype)
+            x = ops.add(x, bias)
+        if self.activation is not None:
+            x = self.activation(x)
+        return x
+
     def quantize(self, mode):
         import gc
 
         # Prevent quantization of the subclasses
         if type(self) is not EinsumDense:
             raise NotImplementedError(
                 f"Layer {self.__class__.__name__} does not have a `quantize()` "
                 "method implemented."
             )
         self._check_quantize_args(mode, self.compute_dtype)
+
+        # Set new dtype policy
+        if not isinstance(
+            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+        ):
+            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
+            # We set the internal `self._dtype_policy` instead of using the
+            # setter to avoid double `quantize` call
+            self._dtype_policy = dtype_policies.get(quantized_dtype)
+
+        self._tracker.unlock()
         if mode == "int8":
-            if backend.standardize_dtype(self._kernel.dtype) == "int8":
-                raise ValueError("`quantize` can only be done once per layer.")
             (
                 self._input_reduced_axes,
                 self._kernel_reduced_axes,
                 self._input_transpose_axes,
                 self._kernel_transpose_axes,
                 self._input_expand_axes,
                 self._kernel_expand_axes,
@@ -482,43 +699,31 @@
                 kernel_scale = ops.expand_dims(
                     kernel_scale, axis=self._kernel_expand_axes
                 )
             if self._kernel_squeeze_axes:
                 kernel_scale = ops.squeeze(
                     kernel_scale, axis=self._kernel_squeeze_axes
                 )
-            self._tracker.unlock()
             self._untrack_variable(self._kernel)
             kernel_shape = self._kernel.shape
             del self._kernel
-            self._kernel = self.add_weight(
-                name="kernel",
-                shape=kernel_shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_value,
-                dtype="int8",
-                trainable=False,
-            )
-            self.kernel_scale = self.add_weight(
-                name="kernel_scale",
-                shape=kernel_scale.shape,
-                # Prevent adding a large constant to the computation graph
-                initializer=lambda shape, dtype: kernel_scale,
-                trainable=False,
+            # Utilize a lambda expression as an initializer to prevent adding a
+            # large constant to the computation graph.
+            self._int8_build(
+                kernel_shape,
+                lambda shape, dtype: kernel_value,
+                lambda shape, dtype: kernel_scale,
             )
-            self._tracker.lock()
+        elif mode == "float8":
+            self._float8_build()
         else:
-            NotImplementedError()
-
-        # Set new dtype policy
-        if not isinstance(
-            self.dtype_policy, dtype_policies.QuantizedDTypePolicy
-        ):
-            quantized_dtype = f"{mode}_from_{self.dtype_policy.name}"
-            self.dtype_policy = dtype_policies.get(quantized_dtype)
+            raise NotImplementedError(
+                self.QUANTIZATION_MODE_ERROR_TEMPLATE.format(mode)
+            )
+        self._tracker.lock()
 
         # Release memory manually because sometimes the backend doesn't
         gc.collect()
 
     def _get_kernel_with_merged_lora(self):
         if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
             kernel_value = self._kernel
@@ -831,8 +1036,7 @@
         input_expand_axes,
         weight_expand_axes,
         input_squeeze_axes,
         weight_squeeze_axes,
         custom_gradient_equation,
         weight_reverse_transpose_axes,
     )
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/identity.py` & `keras-3.3.0/keras/src/layers/core/identity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.layers.layer import Layer
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.Identity")
 class Identity(Layer):
     """Identity layer.
 
     This layer should be used as a placeholder when no operation is to be
@@ -23,8 +23,7 @@
         return input_shape
 
     def compute_output_spec(self, inputs):
         return tree.map_structure(
             lambda x: KerasTensor(x.shape, dtype=x.dtype, sparse=x.sparse),
             inputs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/input_layer.py` & `keras-3.3.0/keras/src/layers/core/input_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,8 +146,7 @@
         dtype=dtype,
         sparse=sparse,
         batch_shape=batch_shape,
         name=name,
         input_tensor=tensor,
     )
     return layer.output
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/lambda_layer.py` & `keras-3.3.0/keras/src/layers/core/lambda_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import inspect
 import types
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 from keras.src.utils import python_utils
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.Lambda")
 class Lambda(Layer):
     """Wraps arbitrary expressions as a `Layer` object.
 
     The `Lambda` layer exists so that arbitrary expressions can be used
@@ -221,8 +221,7 @@
                     )
                 )
         if "arguments" in config:
             config["arguments"] = serialization_lib.deserialize_keras_object(
                 config["arguments"], custom_objects=custom_objects
             )
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/masking.py` & `keras-3.3.0/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

```diff
@@ -68,8 +68,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {"mask_value": self.mask_value}
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/core/wrapper.py` & `keras-3.3.0/keras/src/layers/core/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,8 +41,7 @@
     @classmethod
     def from_config(cls, config, custom_objects=None):
         layer = serialization_lib.deserialize_keras_object(
             config.pop("layer"),
             custom_objects=custom_objects,
         )
         return cls(layer, **config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/input_spec.py` & `keras-3.3.0/keras/src/layers/input_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 
 
 @keras_export(["keras.InputSpec", "keras.layers.InputSpec"])
 class InputSpec:
     """Specifies the rank, dtype and shape of every input to a layer.
 
     Layers can expose (if appropriate) an `input_spec` attribute:
@@ -244,8 +244,7 @@
                     if spec_dim != dim:
                         raise ValueError(
                             f'Input {input_index} of layer "{layer_name}" is '
                             "incompatible with the layer: "
                             f"expected shape={spec.shape}, "
                             f"found shape={shape}"
                         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/layer.py` & `keras-3.3.0/keras/src/layers/layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,28 @@
 from functools import wraps
 
 from keras.src import backend
 from keras.src import constraints
 from keras.src import dtype_policies
 from keras.src import initializers
 from keras.src import regularizers
+from keras.src import tree
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend.common import global_state
 from keras.src.backend.common.name_scope import current_path
 from keras.src.distribution import distribution_lib
 from keras.src.layers import input_spec
 from keras.src.metrics.metric import Metric
 from keras.src.ops.operation import Operation
 from keras.src.utils import python_utils
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 if backend.backend() == "tensorflow":
     from keras.src.backend.tensorflow.layer import TFLayer as BackendLayer
 elif backend.backend() == "jax":
     from keras.src.backend.jax.layer import JaxLayer as BackendLayer
 elif backend.backend() == "torch":
     from keras.src.backend.torch.layer import TorchLayer as BackendLayer
@@ -632,22 +632,27 @@
         state and random seeds.
         """
         if not self.trainable:
             return self.weights
         return [v for v in self.weights if not v.trainable]
 
     @property
+    def metrics(self):
+        """List of all metrics."""
+        metrics = list(self._metrics)
+        for layer in self._layers:
+            metrics.extend(layer.metrics)
+        return metrics
+
+    @property
     def metrics_variables(self):
         """List of all metric variables."""
         vars = []
-        for metric in self._metrics:
+        for metric in self.metrics:
             vars.extend(metric.variables)
-        for layer in self._layers:
-            for metric in layer._metrics:
-                vars.extend(metric.variables)
         return vars
 
     def get_weights(self):
         """Return the values of `layer.weights` as a list of NumPy arrays."""
         return [v.numpy() for v in self.weights]
 
     def set_weights(self, weights):
@@ -665,14 +670,25 @@
                     f"Layer {self.name} weight shape {variable.shape} "
                     "is not compatible with provided weight "
                     f"shape {value.shape}."
                 )
             variable.assign(value)
 
     @property
+    def dtype_policy(self):
+        return self._dtype_policy
+
+    @dtype_policy.setter
+    def dtype_policy(self, value):
+        self._dtype_policy = dtype_policies.get(value)
+        if isinstance(self._dtype_policy, dtype_policies.QuantizedDTypePolicy):
+            if self.built:
+                self.quantize(self._dtype_policy.quantization_mode)
+
+    @property
     def dtype(self):
         """Alias of `layer.variable_dtype`."""
         return self.variable_dtype
 
     @property
     def compute_dtype(self):
         """The dtype of the computations performed by the layer."""
@@ -1123,17 +1139,25 @@
     def _check_quantize_args(self, mode, compute_dtype):
         if not self.built:
             raise ValueError(
                 "Cannot quantize a layer that isn't yet built. "
                 f"Layer '{self.name}' (of type '{self.__class__.__name__}') "
                 "is not built yet."
             )
-        if mode not in ("int8",):
+        if getattr(self, "_is_quantized", False):
             raise ValueError(
-                f"`quantize` must be one of ('int8'). Received: mode={mode}"
+                f"Layer '{self.name}' is already quantized with "
+                f"dtype_policy='{self.dtype_policy.name}'. "
+                f"Received: mode={mode}"
+            )
+        if mode not in dtype_policies.QUANTIZATION_MODES:
+            raise ValueError(
+                "Invalid quantization mode. "
+                f"Expected one of {dtype_policies.QUANTIZATION_MODES}. "
+                f"Received: mode={mode}"
             )
         if mode == "int8" and compute_dtype == "float16":
             raise ValueError(
                 f"Quantization mode='{mode}' doesn't work well with "
                 "compute_dtype='float16'. Consider loading model/layer with "
                 "another dtype policy such as 'mixed_bfloat16' or "
                 "'mixed_float16' before calling `quantize()`."
@@ -1199,21 +1223,23 @@
     def _track_variable(self, variable):
         if variable.trainable:
             self._tracker.add_to_store("trainable_variables", variable)
         else:
             self._tracker.add_to_store("non_trainable_variables", variable)
         if not self.trainable:
             variable.trainable = False
+        self._post_track_variable(variable)
 
     def _untrack_variable(self, variable):
         previous_lock_state = self._tracker.locked
         self._tracker.unlock()
         self._tracker.untrack(variable)
         if previous_lock_state is True:
             self._tracker.lock()
+        self._post_untrack_variable(variable)
 
     def add_metric(self):
         # Permanently disabled
         raise NotImplementedError
 
     def count_params(self):
         """Count the total number of scalars composing the weights.
@@ -1602,8 +1628,7 @@
     return isinstance(s, (list, tuple)) and all(
         d is None or isinstance(d, int) for d in s
     )
 
 
 def might_have_unbuilt_state(layer):
     return any(not lr.built for lr in layer._layers)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/add.py` & `keras-3.3.0/keras/src/layers/merging/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> added = keras.layers.add([x1, x2])
     >>> out = keras.layers.Dense(4)(added)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Add(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/average.py` & `keras-3.3.0/keras/src/layers/merging/average.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.average([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Average(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/base_merge.py` & `keras-3.3.0/keras/src/layers/merging/base_merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,8 +234,7 @@
         if all(m is None for m in mask):
             return None
         masks = [ops.expand_dims(m, axis=0) for m in mask if m is not None]
         return ops.all(ops.concatenate(masks, axis=0), axis=0, keepdims=False)
 
     def get_config(self):
         return super().get_config()
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/concatenate.py` & `keras-3.3.0/keras/src/layers/merging/concatenate.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,8 +166,7 @@
         axis: Concatenation axis.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
         A tensor, the concatenation of the inputs alongside axis `axis`.
     """
     return Concatenate(axis=axis, **kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/dot.py` & `keras-3.3.0/keras/src/layers/merging/dot.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,8 +370,7 @@
             is the cosine proximity between the two samples.
         **kwargs: Standard layer keyword arguments.
 
     Returns:
         A tensor, the dot product of the samples from the inputs.
     """
     return Dot(axes=axes, **kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/maximum.py` & `keras-3.3.0/keras/src/layers/merging/maximum.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.maximum([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Maximum(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/minimum.py` & `keras-3.3.0/keras/src/layers/merging/minimum.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.minimum([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Minimum(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/multiply.py` & `keras-3.3.0/keras/src/layers/merging/multiply.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,8 +64,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> y = keras.layers.multiply([x1, x2])
     >>> out = keras.layers.Dense(4)(y)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Multiply(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/merging/subtract.py` & `keras-3.3.0/keras/src/layers/merging/subtract.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
     >>> x2 = keras.layers.Dense(8, activation='relu')(input2)
     >>> subtracted = keras.layers.subtract([x1, x2])
     >>> out = keras.layers.Dense(4)(subtracted)
     >>> model = keras.models.Model(inputs=[input1, input2], outputs=out)
 
     """
     return Subtract(**kwargs)(inputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/normalization/batch_normalization.py` & `keras-3.3.0/keras/src/layers/normalization/batch_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -320,8 +320,7 @@
             mask_weights_broadcasted * squared_difference,
             self._reduction_axes,
             keepdims=True,
         )
         variance = weighted_distsq / (sum_of_weights + backend.config.epsilon())
 
         return ops.squeeze(mean), ops.squeeze(variance)
-
```

### Comparing `keras-3.2.1/keras/src/layers/normalization/group_normalization.py` & `keras-3.3.0/keras/src/layers/normalization/group_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,8 +213,7 @@
             "beta_regularizer": regularizers.serialize(self.beta_regularizer),
             "gamma_regularizer": regularizers.serialize(self.gamma_regularizer),
             "beta_constraint": constraints.serialize(self.beta_constraint),
             "gamma_constraint": constraints.serialize(self.gamma_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/normalization/layer_normalization.py` & `keras-3.3.0/keras/src/layers/normalization/layer_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -246,8 +246,7 @@
             "beta_regularizer": regularizers.serialize(self.beta_regularizer),
             "gamma_regularizer": regularizers.serialize(self.gamma_regularizer),
             "beta_constraint": constraints.serialize(self.beta_constraint),
             "gamma_constraint": constraints.serialize(self.gamma_constraint),
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/normalization/spectral_normalization.py` & `keras-3.3.0/keras/src/layers/normalization/spectral_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,7 @@
             kernel, self.kernel.dtype
         )
 
     def get_config(self):
         config = {"power_iterations": self.power_iterations}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/normalization/unit_normalization.py` & `keras-3.3.0/keras/src/layers/normalization/unit_normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,8 +51,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = super().get_config()
         config.update({"axis": self.axis})
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/average_pooling1d.py` & `keras-3.3.0/keras/src/layers/pooling/average_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -84,8 +84,7 @@
             pool_dimensions=1,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/average_pooling2d.py` & `keras-3.3.0/keras/src/layers/pooling/average_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,7 @@
             pool_dimensions=2,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/average_pooling3d.py` & `keras-3.3.0/keras/src/layers/pooling/average_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
             pool_dimensions=3,
             pool_mode="average",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/base_global_pooling.py` & `keras-3.3.0/keras/src/layers/pooling/base_global_pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
         config.update(
             {
                 "data_format": self.data_format,
                 "keepdims": self.keepdims,
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/base_pooling.py` & `keras-3.3.0/keras/src/layers/pooling/base_pooling.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,7 @@
                 "pool_size": self.pool_size,
                 "padding": self.padding,
                 "strides": self.strides,
                 "data_format": self.data_format,
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-3.3.0/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,7 @@
                 inputs, axis=steps_axis, keepdims=self.keepdims
             ) / ops.sum(mask, axis=steps_axis, keepdims=self.keepdims)
         else:
             return ops.mean(inputs, axis=steps_axis, keepdims=self.keepdims)
 
     def compute_mask(self, inputs, mask=None):
         return None
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-3.3.0/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,8 +62,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.mean(inputs, axis=[1, 2], keepdims=self.keepdims)
         return ops.mean(inputs, axis=[2, 3], keepdims=self.keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-3.3.0/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.mean(inputs, axis=[1, 2, 3], keepdims=self.keepdims)
         return ops.mean(inputs, axis=[2, 3, 4], keepdims=self.keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-3.3.0/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,8 +60,7 @@
             keepdims=keepdims,
             **kwargs,
         )
 
     def call(self, inputs):
         steps_axis = 1 if self.data_format == "channels_last" else 2
         return ops.max(inputs, axis=steps_axis, keepdims=self.keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-3.3.0/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,8 +62,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.max(inputs, axis=[1, 2], keepdims=self.keepdims)
         return ops.max(inputs, axis=[2, 3], keepdims=self.keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-3.3.0/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,8 +63,7 @@
             **kwargs,
         )
 
     def call(self, inputs):
         if self.data_format == "channels_last":
             return ops.max(inputs, axis=[1, 2, 3], keepdims=self.keepdims)
         return ops.max(inputs, axis=[2, 3, 4], keepdims=self.keepdims)
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/max_pooling1d.py` & `keras-3.3.0/keras/src/layers/pooling/max_pooling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,8 +85,7 @@
             pool_dimensions=1,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/max_pooling2d.py` & `keras-3.3.0/keras/src/layers/pooling/max_pooling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,8 +101,7 @@
             pool_dimensions=2,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/pooling/max_pooling3d.py` & `keras-3.3.0/keras/src/layers/pooling/max_pooling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,8 +77,7 @@
             pool_dimensions=3,
             pool_mode="max",
             padding=padding,
             data_format=data_format,
             name=name,
             **kwargs,
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -364,8 +364,7 @@
                 "top_db": self.top_db,
                 "mag_exp": self.mag_exp,
                 "min_power": self.min_power,
                 "ref_power": self.ref_power,
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/category_encoding.py` & `keras-3.3.0/keras/src/layers/preprocessing/category_encoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,8 +200,7 @@
                     "`'count'`. Received `count_weights={count_weights}`."
                 )
             count_weights = self.backend.convert_to_tensor(
                 count_weights, dtype=self.compute_dtype
             )
         outputs = self._encode(inputs, count_weights)
         return backend_utils.convert_tf_tensor(outputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/center_crop.py` & `keras-3.3.0/keras/src/layers/preprocessing/center_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,8 +138,7 @@
         base_config = super().get_config()
         config = {
             "height": self.height,
             "width": self.width,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/discretization.py` & `keras-3.3.0/keras/src/layers/preprocessing/discretization.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,14 @@
         )
         self.num_bins = num_bins
         self.epsilon = epsilon
         self.output_mode = output_mode
         self.sparse = sparse
 
         if self.bin_boundaries:
-            self.built = True
             self.summary = None
         else:
             self.summary = np.array([[], []], dtype="float32")
 
     def build(self, input_shape=None):
         self.built = True
 
@@ -334,8 +333,7 @@
     new_bins = np.interp(percents, cum_weight_percents, summary[0])
     cum_weights = np.interp(percents, cum_weight_percents, cum_weights)
     new_weights = cum_weights - np.concatenate(
         (np.array([0]), cum_weights[:-1])
     )
     summary = np.stack((new_bins, new_weights))
     return summary.astype("float32")
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/feature_space.py` & `keras-3.3.0/keras/src/layers/preprocessing/feature_space.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from keras.src import backend
 from keras.src import layers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import saving_lib
 from keras.src.saving import serialization_lib
 from keras.src.utils import backend_utils
-from keras.src.utils import tree
 from keras.src.utils.module_utils import tensorflow as tf
 from keras.src.utils.naming import auto_name
 
 
 class Cross:
     def __init__(self, feature_names, crossing_dim, output_mode="one_hot"):
         if output_mode not in {"int", "one_hot"}:
@@ -792,8 +792,7 @@
         saving_lib.save_model(self, filepath)
 
     def save_own_variables(self, store):
         return
 
     def load_own_variables(self, store):
         return
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files 0% similar despite different names*

```diff
@@ -217,8 +217,7 @@
             tf.as_dtype(x.dtype).is_integer or x.dtype == tf.string
             for x in inputs
         ):
             raise ValueError(
                 "All `HashedCrossing` inputs should have an integer or "
                 f"string dtype. Received: inputs={inputs}"
             )
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/hashing.py` & `keras-3.3.0/keras/src/layers/preprocessing/hashing.py`

 * *Files 0% similar despite different names*

```diff
@@ -275,8 +275,7 @@
                 "salt": self.salt,
                 "mask_value": self.mask_value,
                 "output_mode": self.output_mode,
                 "sparse": self.sparse,
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/index_lookup.py` & `keras-3.3.0/keras/src/layers/preprocessing/index_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -991,8 +991,7 @@
 def listify_tensors(x):
     """Convert any tensors or numpy arrays to lists for config serialization."""
     if tf.is_tensor(x):
         x = x.numpy()
     if isinstance(x, np.ndarray):
         x = x.tolist()
     return x
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/integer_lookup.py` & `keras-3.3.0/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,7 @@
     def call(self, inputs):
         if not isinstance(
             inputs, (tf.Tensor, tf.RaggedTensor, np.ndarray, list, tuple)
         ):
             inputs = tf.convert_to_tensor(backend.convert_to_numpy(inputs))
         outputs = super().call(inputs)
         return backend_utils.convert_tf_tensor(outputs)
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/normalization.py` & `keras-3.3.0/keras/src/layers/preprocessing/normalization.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,8 +330,7 @@
     def get_build_config(self):
         if self._build_input_shape:
             return {"input_shape": self._build_input_shape}
 
     def build_from_config(self, config):
         if config:
             self.build(config["input_shape"])
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_brightness.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_brightness.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,20 +76,20 @@
         self._set_value_range(value_range)
         self.seed = seed
         self.generator = SeedGenerator(seed)
 
     def _set_value_range(self, value_range):
         if not isinstance(value_range, (tuple, list)):
             raise ValueError(
-                self.value_range_VALIDATION_ERROR
+                self._VALUE_RANGE_VALIDATION_ERROR
                 + f"Received: value_range={value_range}"
             )
         if len(value_range) != 2:
             raise ValueError(
-                self.value_range_VALIDATION_ERROR
+                self._VALUE_RANGE_VALIDATION_ERROR
                 + f"Received: value_range={value_range}"
             )
         self.value_range = sorted(value_range)
 
     def _set_factor(self, factor):
         if isinstance(factor, (tuple, list)):
             if len(factor) != 2:
@@ -158,8 +158,7 @@
         config = {
             "factor": self._factor,
             "value_range": self.value_range,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_contrast.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_contrast.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,8 +92,7 @@
     def get_config(self):
         config = {
             "factor": self.factor,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_crop.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_crop.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,8 +167,7 @@
                 "height": self.height,
                 "width": self.width,
                 "seed": self.seed,
                 "data_format": self.data_format,
             }
         )
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_flip.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_flip.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         config = super().get_config()
         config.update({"seed": self.seed, "mode": self.mode})
         return config
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_rotation.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_rotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,8 +248,7 @@
             "fill_mode": self.fill_mode,
             "fill_value": self.fill_value,
             "interpolation": self.interpolation,
             "seed": self.seed,
         }
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_translation.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_translation.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,8 +245,7 @@
             "fill_mode": self.fill_mode,
             "interpolation": self.interpolation,
             "seed": self.seed,
             "fill_value": self.fill_value,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/random_zoom.py` & `keras-3.3.0/keras/src/layers/preprocessing/random_zoom.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             Note that when using torch backend, `"reflect"` is redirected to
             `"mirror"` `(c d c b | a b c d | c b a b)` because torch does not
             support `"reflect"`.
             Note that torch backend does not support `"wrap"`.
         interpolation: Interpolation mode. Supported values: `"nearest"`,
             `"bilinear"`.
         seed: Integer. Used to create a random seed.
-        fill_value: a float represents the value to be filled outside
+        fill_value: a float that represents the value to be filled outside
             the boundaries when `fill_mode="constant"`.
         data_format: string, either `"channels_last"` or `"channels_first"`.
             The ordering of the dimensions in the inputs. `"channels_last"`
             corresponds to inputs with shape `(batch, height, width, channels)`
             while `"channels_first"` corresponds to inputs with shape
             `(batch, channels, height, width)`. It defaults to the
             `image_data_format` value found in your Keras config file at
@@ -257,8 +257,7 @@
             "fill_mode": self.fill_mode,
             "interpolation": self.interpolation,
             "seed": self.seed,
             "fill_value": self.fill_value,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/rescaling.py` & `keras-3.3.0/keras/src/layers/preprocessing/rescaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,8 +57,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "scale": self.scale,
             "offset": self.offset,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/resizing.py` & `keras-3.3.0/keras/src/layers/preprocessing/resizing.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.layers.preprocessing.tf_data_layer import TFDataLayer
-from keras.src.utils import image_utils
 
 
 @keras_export("keras.layers.Resizing")
 class Resizing(TFDataLayer):
     """A preprocessing layer which resizes images.
 
     This layer resizes an image input to a target height and width. The input
@@ -36,14 +35,23 @@
         crop_to_aspect_ratio: If `True`, resize the images without aspect
             ratio distortion. When the original aspect ratio differs
             from the target aspect ratio, the output image will be
             cropped so as to return the
             largest possible window in the image (of size `(height, width)`)
             that matches the target aspect ratio. By default
             (`crop_to_aspect_ratio=False`), aspect ratio may not be preserved.
+        pad_to_aspect_ratio: If `True`, pad the images without aspect
+            ratio distortion. When the original aspect ratio differs
+            from the target aspect ratio, the output image will be
+            evenly padded on the short side.
+        fill_mode: When using `pad_to_aspect_ratio=True`, padded areas
+            are filled according to the given mode. Only `"constant"` is
+            supported at this time
+            (fill with constant value, equal to `fill_value`).
+        fill_value: Float. Padding value to use when `pad_to_aspect_ratio=True`.
         data_format: string, either `"channels_last"` or `"channels_first"`.
             The ordering of the dimensions in the inputs. `"channels_last"`
             corresponds to inputs with shape `(batch, height, width, channels)`
             while `"channels_first"` corresponds to inputs with shape
             `(batch, channels, height, width)`. It defaults to the
             `image_data_format` value found in your Keras config file at
             `~/.keras/keras.json`. If you never set it, then it will be
@@ -53,42 +61,42 @@
 
     def __init__(
         self,
         height,
         width,
         interpolation="bilinear",
         crop_to_aspect_ratio=False,
+        pad_to_aspect_ratio=False,
+        fill_mode="constant",
+        fill_value=0.0,
         data_format=None,
         **kwargs,
     ):
         super().__init__(**kwargs)
         self.height = height
         self.width = width
         self.interpolation = interpolation
         self.data_format = backend.standardize_data_format(data_format)
         self.crop_to_aspect_ratio = crop_to_aspect_ratio
+        self.pad_to_aspect_ratio = pad_to_aspect_ratio
+        self.fill_mode = fill_mode
+        self.fill_value = fill_value
 
     def call(self, inputs):
         size = (self.height, self.width)
-        if self.crop_to_aspect_ratio:
-            outputs = image_utils.smart_resize(
-                inputs,
-                size=size,
-                interpolation=self.interpolation,
-                data_format=self.data_format,
-                backend_module=self.backend,
-            )
-        else:
-            outputs = self.backend.image.resize(
-                inputs,
-                size=size,
-                interpolation=self.interpolation,
-                data_format=self.data_format,
-            )
-        return outputs
+        return self.backend.image.resize(
+            inputs,
+            size=size,
+            interpolation=self.interpolation,
+            data_format=self.data_format,
+            crop_to_aspect_ratio=self.crop_to_aspect_ratio,
+            pad_to_aspect_ratio=self.pad_to_aspect_ratio,
+            fill_mode=self.fill_mode,
+            fill_value=self.fill_value,
+        )
 
     def compute_output_shape(self, input_shape):
         input_shape = list(input_shape)
         if len(input_shape) == 4:
             if self.data_format == "channels_last":
                 input_shape[1] = self.height
                 input_shape[2] = self.width
@@ -107,11 +115,13 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "height": self.height,
             "width": self.width,
             "interpolation": self.interpolation,
             "crop_to_aspect_ratio": self.crop_to_aspect_ratio,
+            "pad_to_aspect_ratio": self.pad_to_aspect_ratio,
+            "fill_mode": self.fill_mode,
+            "fill_value": self.fill_value,
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/string_lookup.py` & `keras-3.3.0/keras/src/layers/preprocessing/string_lookup.py`

 * *Files 0% similar despite different names*

```diff
@@ -388,8 +388,7 @@
             tf_inputs = False
             if not isinstance(inputs, (np.ndarray, list, tuple)):
                 inputs = tf.convert_to_tensor(backend.convert_to_numpy(inputs))
         outputs = super().call(inputs)
         if not tf_inputs:
             outputs = backend_utils.convert_tf_tensor(outputs)
         return outputs
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/text_vectorization.py` & `keras-3.3.0/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files 0% similar despite different names*

```diff
@@ -620,8 +620,7 @@
         self._lookup_layer.load_own_variables(store)
 
     def save_assets(self, dir_path):
         self._lookup_layer.save_assets(dir_path)
 
     def load_assets(self, dir_path):
         self._lookup_layer.load_assets(dir_path)
-
```

### Comparing `keras-3.2.1/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-3.3.0/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import keras.src.backend
+from keras.src import tree
 from keras.src.layers.layer import Layer
 from keras.src.random.seed_generator import SeedGenerator
 from keras.src.utils import backend_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class TFDataLayer(Layer):
     """Layer that can safely used in a tf.data pipeline.
 
     The `call()` method must solely rely on `self.backend` ops.
 
@@ -51,8 +51,7 @@
         if not hasattr(self, "_backend_generators"):
             self._backend_generators = {}
         if backend in self._backend_generators:
             return self._backend_generators[backend]
         seed_generator = SeedGenerator(self.seed, backend=self.backend)
         self._backend_generators[backend] = seed_generator
         return seed_generator
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/activity_regularization.py` & `keras-3.3.0/keras/src/layers/regularization/activity_regularization.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,7 @@
     def compute_output_shape(self, input_shape):
         return input_shape
 
     def get_config(self):
         base_config = super().get_config()
         config = {"l1": self.l1, "l2": self.l2}
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/alpha_dropout.py` & `keras-3.3.0/keras/src/layers/regularization/alpha_dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
                 f"Invalid value received for argument "
                 "`rate`. Expected a float value between 0 and 1. "
                 f"Received: rate={rate}"
             )
         self.rate = rate
         self.seed = seed
         self.noise_shape = noise_shape
-        self.seed_generator = backend.random.SeedGenerator(seed)
+        if rate > 0:
+            self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
-        self.built = True
 
     def call(self, inputs, training=False):
         if training and self.rate > 0:
             noise_shape = self._get_concrete_noise_shape(
                 inputs, self.noise_shape
             )
             alpha = 1.6732632423543772848170429916717
@@ -91,8 +91,7 @@
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
             "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/dropout.py` & `keras-3.3.0/keras/src/layers/regularization/dropout.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,14 @@
             )
         self.rate = rate
         self.seed = seed
         self.noise_shape = noise_shape
         if rate > 0:
             self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
-        self.built = True
 
     def call(self, inputs, training=False):
         if training and self.rate > 0:
             return backend.random.dropout(
                 inputs,
                 self.rate,
                 noise_shape=self.noise_shape,
@@ -71,8 +70,7 @@
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
             "noise_shape": self.noise_shape,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/gaussian_dropout.py` & `keras-3.3.0/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
             raise ValueError(
                 f"Invalid value received for argument "
                 "`rate`. Expected a float value between 0 and 1. "
                 f"Received: rate={rate}"
             )
         self.rate = rate
         self.seed = seed
-        self.seed_generator = backend.random.SeedGenerator(seed)
+        if rate > 0:
+            self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
 
     def call(self, inputs, training=False):
         if training and self.rate > 0:
             stddev = math.sqrt(self.rate / (1.0 - self.rate))
             return inputs * backend.random.normal(
                 shape=ops.shape(inputs),
@@ -55,8 +56,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "rate": self.rate,
             "seed": self.seed,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/gaussian_noise.py` & `keras-3.3.0/keras/src/layers/regularization/gaussian_noise.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,16 @@
             raise ValueError(
                 f"Invalid value received for argument "
                 "`stddev`. Expected a float value between 0 and 1. "
                 f"Received: stddev={stddev}"
             )
         self.stddev = stddev
         self.seed = seed
-        self.seed_generator = backend.random.SeedGenerator(seed)
+        if stddev > 0:
+            self.seed_generator = backend.random.SeedGenerator(seed)
         self.supports_masking = True
 
     def call(self, inputs, training=False):
         if training and self.stddev > 0:
             return inputs + backend.random.normal(
                 shape=ops.shape(inputs),
                 mean=0.0,
@@ -55,8 +56,7 @@
     def get_config(self):
         base_config = super().get_config()
         config = {
             "stddev": self.stddev,
             "seed": self.seed,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/regularization/spatial_dropout.py` & `keras-3.3.0/keras/src/layers/regularization/spatial_dropout.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,8 +186,7 @@
 
     def get_config(self):
         base_config = super().get_config()
         config = {
             "data_format": self.data_format,
         }
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/cropping1d.py` & `keras-3.3.0/keras/src/layers/reshaping/cropping1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,8 +76,7 @@
         else:
             return inputs[:, self.cropping[0] : -self.cropping[1], :]
 
     def get_config(self):
         config = {"cropping": self.cropping}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/cropping2d.py` & `keras-3.3.0/keras/src/layers/reshaping/cropping2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,8 +218,7 @@
                 :,
             ]
 
     def get_config(self):
         config = {"cropping": self.cropping, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/cropping3d.py` & `keras-3.3.0/keras/src/layers/reshaping/cropping3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,8 +278,7 @@
                 :,
             ]
 
     def get_config(self):
         config = {"cropping": self.cropping, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/flatten.py` & `keras-3.3.0/keras/src/layers/reshaping/flatten.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,8 +74,7 @@
             shape=output_shape, dtype=inputs.dtype, sparse=inputs.sparse
         )
 
     def get_config(self):
         config = {"data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/permute.py` & `keras-3.3.0/keras/src/layers/reshaping/permute.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,8 +58,7 @@
     def call(self, inputs):
         return ops.transpose(inputs, axes=(0,) + self.dims)
 
     def get_config(self):
         config = {"dims": self.dims}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/repeat_vector.py` & `keras-3.3.0/keras/src/layers/reshaping/repeat_vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,8 +42,7 @@
         reshaped = ops.reshape(inputs, (input_shape[0], 1, input_shape[1]))
         return ops.repeat(reshaped, self.n, axis=1)
 
     def get_config(self):
         config = {"n": self.n}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/reshape.py` & `keras-3.3.0/keras/src/layers/reshaping/reshape.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
             inputs, (ops.shape(inputs)[0],) + self._resolved_target_shape
         )
 
     def get_config(self):
         config = {"target_shape": self.target_shape}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/up_sampling1d.py` & `keras-3.3.0/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,8 +55,7 @@
     def call(self, inputs):
         return ops.repeat(x=inputs, repeats=self.size, axis=1)
 
     def get_config(self):
         config = {"size": self.size}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/up_sampling2d.py` & `keras-3.3.0/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,8 +163,7 @@
                 x.shape[2] * width_factor,
             )
             x = ops.image.resize(x, new_shape, interpolation=interpolation)
         if data_format == "channels_first":
             x = ops.transpose(x, [0, 3, 1, 2])
 
         return x
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/up_sampling3d.py` & `keras-3.3.0/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,8 +128,7 @@
         elif data_format == "channels_last":
             output = ops.repeat(x, depth_factor, axis=1)
             output = ops.repeat(output, height_factor, axis=2)
             output = ops.repeat(output, width_factor, axis=3)
             return output
         else:
             raise ValueError(f"Invalid data_format: {data_format}")
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/zero_padding1d.py` & `keras-3.3.0/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,8 +64,7 @@
         all_dims_padding = ((0, 0), self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/zero_padding2d.py` & `keras-3.3.0/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,8 +113,7 @@
             all_dims_padding = ((0, 0), *self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/reshaping/zero_padding3d.py` & `keras-3.3.0/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,8 +112,7 @@
             all_dims_padding = ((0, 0), *self.padding, (0, 0))
         return ops.pad(inputs, all_dims_padding)
 
     def get_config(self):
         config = {"padding": self.padding, "data_format": self.data_format}
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/bidirectional.py` & `keras-3.3.0/keras/src/layers/rnn/bidirectional.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,8 +319,7 @@
             backward_layer = serialization_lib.deserialize_keras_object(
                 backward_layer_config, custom_objects=custom_objects
             )
             config["backward_layer"] = backward_layer
         # Instantiate the wrapper, adjust it and return it.
         layer = cls(**config)
         return layer
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/conv_lstm.py` & `keras-3.3.0/keras/src/layers/rnn/conv_lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
 from keras.src.ops import operation_utils
 from keras.src.utils import argument_validation
-from keras.src.utils import tree
 
 
 class ConvLSTMCell(Layer, DropoutRNNCell):
     """Cell class for the ConvLSTM layer.
 
     Args:
         rank: Integer, rank of the convolution, e.g. "2" for 2D convolutions.
@@ -683,8 +683,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/conv_lstm1d.py` & `keras-3.3.0/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,8 +178,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/conv_lstm2d.py` & `keras-3.3.0/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,8 +178,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/conv_lstm3d.py` & `keras-3.3.0/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,8 +177,7 @@
             go_backwards=go_backwards,
             stateful=stateful,
             dropout=dropout,
             recurrent_dropout=recurrent_dropout,
             seed=seed,
             **kwargs
         )
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,8 +47,7 @@
         mask should be cached across all timestep within the same batch, but
         shouldn't be cached between batches.
         """
         self._dropout_mask = None
 
     def reset_recurrent_dropout_mask(self):
         self._recurrent_dropout_mask = None
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/gru.py` & `keras-3.3.0/keras/src/layers/rnn/gru.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.GRUCell")
 class GRUCell(Layer, DropoutRNNCell):
     """Cell class for the GRU layer.
 
     This class processes one step within the whole time sequence input, whereas
@@ -683,8 +683,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/lstm.py` & `keras-3.3.0/keras/src/layers/rnn/lstm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from keras.src import activations
 from keras.src import backend
 from keras.src import constraints
 from keras.src import initializers
 from keras.src import ops
 from keras.src import regularizers
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.rnn import RNN
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.LSTMCell")
 class LSTMCell(Layer, DropoutRNNCell):
     """Cell class for the LSTM layer.
 
     This class processes one step within the whole time sequence input, whereas
@@ -663,8 +663,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/rnn.py` & `keras-3.3.0/keras/src/layers/rnn/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.layers.rnn.dropout_rnn_cell import DropoutRNNCell
 from keras.src.layers.rnn.stacked_rnn_cells import StackedRNNCells
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.RNN")
 class RNN(Layer):
     """Base class for recurrent layers.
 
     Args:
@@ -129,16 +129,16 @@
     calling `reset_states` with the keyword argument `states`. The value of
     `states` should be a numpy array or list of numpy arrays representing
     the initial state of the RNN layer.
 
     Examples:
 
     ```python
-    from keras.layers import RNN
-    from keras import ops
+    from keras.src.layers import RNN
+    from keras.src import ops
 
     # First, let's define a RNN Cell, as a layer subclass.
     class MinimalRNNCell(keras.layers.Layer):
 
         def __init__(self, units, **kwargs):
             super().__init__(**kwargs)
             self.units = units
@@ -232,26 +232,34 @@
             self.state_size = [state_size]
             self.single_state = True
         else:
             self.state_size = list(state_size)
             self.single_state = False
 
     def compute_output_shape(self, sequences_shape, initial_state_shape=None):
-        state_shape = [(sequences_shape[0], d) for d in self.state_size]
+        batch_size = sequences_shape[0]
+        length = sequences_shape[1]
+        states_shape = []
+        for state_size in self.state_size:
+            if isinstance(state_size, int):
+                states_shape.append((batch_size, state_size))
+            elif isinstance(state_size, (list, tuple)):
+                states_shape.append([(batch_size, s) for s in state_size])
+
         output_size = getattr(self.cell, "output_size", None)
         if output_size is None:
             output_size = self.state_size[0]
         if not isinstance(output_size, int):
             raise ValueError("output_size must be an integer.")
         if self.return_sequences:
-            output_shape = (sequences_shape[0], sequences_shape[1], output_size)
+            output_shape = (batch_size, length, output_size)
         else:
-            output_shape = (sequences_shape[0], output_size)
+            output_shape = (batch_size, output_size)
         if self.return_state:
-            return output_shape, *state_shape
+            return output_shape, *states_shape
         return output_shape
 
     def compute_mask(self, _, mask):
         # Time step masks must be the same for each input.
         # This is because the mask for an RNN is of size [batch, time_steps, 1],
         # and specifies which time steps should be skipped, and a time step
         # must be skipped for all inputs.
@@ -468,8 +476,7 @@
     @classmethod
     def from_config(cls, config, custom_objects=None):
         cell = serialization_lib.deserialize_keras_object(
             config.pop("cell"), custom_objects=custom_objects
         )
         layer = cls(cell, **config)
         return layer
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/simple_rnn.py` & `keras-3.3.0/keras/src/layers/rnn/simple_rnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,8 +444,7 @@
         base_config = super().get_config()
         del base_config["cell"]
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export("keras.layers.StackedRNNCells")
 class StackedRNNCells(Layer):
     """Wrapper allowing a stack of RNN cells to behave as a single cell.
 
     Used to implement efficient stacked RNNs.
@@ -133,8 +133,7 @@
         for cell_config in config.pop("cells"):
             cells.append(
                 serialization_lib.deserialize_keras_object(
                     cell_config, custom_objects=custom_objects
                 )
             )
         return cls(cells, **config)
-
```

### Comparing `keras-3.2.1/keras/src/layers/rnn/time_distributed.py` & `keras-3.3.0/keras/src/layers/rnn/time_distributed.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,8 +109,7 @@
             )
             return time_distributed_transpose(outputs)
 
         # Implementation #2: use backend.vectorized_map.
 
         outputs = backend.vectorized_map(step_function, ops.arange(timesteps))
         return time_distributed_transpose(outputs)
-
```

### Comparing `keras-3.2.1/keras/src/legacy/backend.py` & `keras-3.3.0/keras/src/legacy/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -2283,8 +2283,7 @@
         return v
 
 
 @keras_export("keras._legacy.backend.zeros_like")
 def zeros_like(x, dtype=None, name=None):
     """DEPRECATED."""
     return tf.zeros_like(x, dtype=dtype, name=name)
-
```

### Comparing `keras-3.2.1/keras/src/legacy/layers.py` & `keras-3.3.0/keras/src/legacy/layers.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,8 +239,7 @@
     def get_config(self):
         config = {"theta": float(self.theta)}
         base_config = super().get_config()
         return {**base_config, **config}
 
     def compute_output_shape(self, input_shape):
         return input_shape
-
```

### Comparing `keras-3.2.1/keras/src/legacy/losses.py` & `keras-3.3.0/keras/src/legacy/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,7 @@
 
     @classmethod
     def validate(cls, key):
         if key not in cls.all():
             raise ValueError(
                 f'Invalid Reduction Key: {key}. Expected keys are "{cls.all()}"'
             )
-
```

### Comparing `keras-3.2.1/keras/src/legacy/preprocessing/image.py` & `keras-3.3.0/keras/src/legacy/preprocessing/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -1886,8 +1886,7 @@
                 cval=cval,
             )
             for x_channel in x
         ]
         x = np.stack(channel_images, axis=0)
         x = np.rollaxis(x, 0, channel_axis + 1)
     return x
-
```

### Comparing `keras-3.2.1/keras/src/legacy/preprocessing/sequence.py` & `keras-3.3.0/keras/src/legacy/preprocessing/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,8 +314,7 @@
             seed = random.randint(0, 10e6)
         random.seed(seed)
         random.shuffle(couples)
         random.seed(seed)
         random.shuffle(labels)
 
     return couples, labels
-
```

### Comparing `keras-3.2.1/keras/src/legacy/preprocessing/text.py` & `keras-3.3.0/keras/src/legacy/preprocessing/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,8 +330,7 @@
     tokenizer = Tokenizer(**config)
     tokenizer.word_counts = word_counts
     tokenizer.word_docs = word_docs
     tokenizer.index_docs = index_docs
     tokenizer.word_index = word_index
     tokenizer.index_word = index_word
     return tokenizer
-
```

### Comparing `keras-3.2.1/keras/src/legacy/saving/json_utils.py` & `keras-3.3.0/keras/src/legacy/saving/json_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,8 +214,7 @@
 
     if isinstance(obj, bytes):
         return {"class_name": "__bytes__", "value": obj.decode("utf-8")}
 
     raise TypeError(
         f"Unable to serialize {obj} to JSON. Unrecognized type {type(obj)}."
     )
-
```

### Comparing `keras-3.2.1/keras/src/legacy/saving/legacy_h5_format.py` & `keras-3.3.0/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     """Save top-level weights of a model to a HDF5 group.
 
     Args:
         f: HDF5 group.
         weights: List of weight variables.
     """
     weight_values = [backend.convert_to_numpy(w) for w in weights]
-    weight_names = [w.name.encode("utf8") for w in weights]
+    weight_names = [str(w.path).encode("utf8") for w in weights]
     save_attributes_to_hdf5_group(f, "weight_names", weight_names)
     for name, val in zip(weight_names, weight_values):
         param_dset = f.create_dataset(name, val.shape, dtype=val.dtype)
         if not val.shape:
             # scalar
             param_dset[()] = val
         else:
@@ -251,15 +251,15 @@
     """
     if isinstance(optimizer, optimizers.Optimizer):
         symbolic_weights = optimizer.variables
     else:
         symbolic_weights = getattr(optimizer, "weights")
     if symbolic_weights:
         weights_group = hdf5_group.create_group("optimizer_weights")
-        weight_names = [str(w.name).encode("utf8") for w in symbolic_weights]
+        weight_names = [str(w.path).encode("utf8") for w in symbolic_weights]
         save_attributes_to_hdf5_group(
             weights_group, "weight_names", weight_names
         )
         weight_values = [backend.convert_to_numpy(w) for w in symbolic_weights]
         for name, val in zip(weight_names, weight_values):
             param_dset = weights_group.create_dataset(
                 name, val.shape, dtype=val.dtype
@@ -460,24 +460,24 @@
                 expected_shape = symbolic_weights[i].shape
                 received_shape = weight_values[i].shape
                 if expected_shape != received_shape:
                     if skip_mismatch:
                         warnings.warn(
                             f"Skipping loading weights for layer #{k} (named "
                             f"{layer.name}) due to mismatch in shape for "
-                            f"weight {symbolic_weights[i].name}. "
+                            f"weight {symbolic_weights[i].path}. "
                             f"Weight expects shape {expected_shape}. "
                             "Received saved weight "
                             f"with shape {received_shape}",
                             stacklevel=2,
                         )
                         continue
                     raise ValueError(
                         f"Shape mismatch in layer #{k} (named {layer.name}) "
-                        f"for weight {symbolic_weights[i].name}. "
+                        f"for weight {symbolic_weights[i].path}. "
                         f"Weight expects shape {expected_shape}. "
                         "Received saved weight "
                         f"with shape {received_shape}"
                     )
                 else:
                     symbolic_weights[i].assign(weight_values[i])
 
@@ -509,24 +509,24 @@
                 expected_shape = symbolic_weights[i].shape
                 received_shape = weight_values[i].shape
                 if expected_shape != received_shape:
                     if skip_mismatch:
                         warnings.warn(
                             "Skipping loading top-level weight for model due "
                             "to mismatch in shape for "
-                            f"weight {symbolic_weights[i].name}. "
+                            f"weight {symbolic_weights[i].path}. "
                             f"Weight expects shape {expected_shape}. "
                             "Received saved weight "
                             f"with shape {received_shape}",
                             stacklevel=2,
                         )
                     else:
                         raise ValueError(
                             "Shape mismatch in model for top-level weight "
-                            f"{symbolic_weights[i].name}. "
+                            f"{symbolic_weights[i].path}. "
                             f"Weight expects shape {expected_shape}. "
                             "Received saved weight "
                             f"with shape {received_shape}"
                         )
                 else:
                     symbolic_weights[i].assign(weight_values[i])
 
@@ -612,8 +612,7 @@
     Args:
         layer: a `Model` or `Layer` instance.
 
     Returns:
         A list of variables with the legacy weight order.
     """
     return layer.trainable_weights + layer.non_trainable_weights
-
```

### Comparing `keras-3.2.1/keras/src/legacy/saving/saving_utils.py` & `keras-3.3.0/keras/src/legacy/saving/saving_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from keras.src import backend
 from keras.src import layers
 from keras.src import losses
 from keras.src import metrics as metrics_module
 from keras.src import models
 from keras.src import optimizers
+from keras.src import tree
 from keras.src.legacy.saving import serialization
 from keras.src.saving import object_registration
-from keras.src.utils import tree
 
 MODULE_OBJECTS = threading.local()
 
 # Legacy lambda arguments not found in Keras 3
 LAMBDA_DEP_ARGS = (
     "module",
     "function_type",
@@ -254,8 +254,7 @@
             model.compiled_metrics.build(model.outputs, model.outputs)
     except:
         logging.warning(
             "Compiled the loaded model, but the compiled metrics have "
             "yet to be built. `model.compile_metrics` will be empty "
             "until you train or evaluate the model."
         )
-
```

### Comparing `keras-3.2.1/keras/src/legacy/saving/serialization.py` & `keras-3.3.0/keras/src/legacy/saving/serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -568,8 +568,7 @@
 
 
 def _find_replace_nested_dict(config, find, replace):
     dict_str = json.dumps(config)
     dict_str = dict_str.replace(find, replace)
     config = json.loads(dict_str)
     return config
-
```

### Comparing `keras-3.2.1/keras/src/losses/__init__.py` & `keras-3.3.0/keras/src/losses/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import inspect
+
 from keras.src.api_export import keras_export
 from keras.src.losses.loss import Loss
 from keras.src.losses.losses import BinaryCrossentropy
 from keras.src.losses.losses import BinaryFocalCrossentropy
 from keras.src.losses.losses import CategoricalCrossentropy
 from keras.src.losses.losses import CategoricalFocalCrossentropy
 from keras.src.losses.losses import CategoricalHinge
@@ -15,14 +17,15 @@
 from keras.src.losses.losses import MeanAbsoluteError
 from keras.src.losses.losses import MeanAbsolutePercentageError
 from keras.src.losses.losses import MeanSquaredError
 from keras.src.losses.losses import MeanSquaredLogarithmicError
 from keras.src.losses.losses import Poisson
 from keras.src.losses.losses import SparseCategoricalCrossentropy
 from keras.src.losses.losses import SquaredHinge
+from keras.src.losses.losses import Tversky
 from keras.src.losses.losses import binary_crossentropy
 from keras.src.losses.losses import binary_focal_crossentropy
 from keras.src.losses.losses import categorical_crossentropy
 from keras.src.losses.losses import categorical_focal_crossentropy
 from keras.src.losses.losses import categorical_hinge
 from keras.src.losses.losses import cosine_similarity
 from keras.src.losses.losses import ctc
@@ -34,14 +37,15 @@
 from keras.src.losses.losses import mean_absolute_error
 from keras.src.losses.losses import mean_absolute_percentage_error
 from keras.src.losses.losses import mean_squared_error
 from keras.src.losses.losses import mean_squared_logarithmic_error
 from keras.src.losses.losses import poisson
 from keras.src.losses.losses import sparse_categorical_crossentropy
 from keras.src.losses.losses import squared_hinge
+from keras.src.losses.losses import tversky
 from keras.src.saving import serialization_lib
 
 ALL_OBJECTS = {
     # Base
     Loss,
     LossFunctionWrapper,
     # Probabilistic
@@ -62,14 +66,15 @@
     Huber,
     # Hinge
     Hinge,
     SquaredHinge,
     CategoricalHinge,
     # Image segmentation
     Dice,
+    Tversky,
     # Probabilistic
     kl_divergence,
     poisson,
     binary_crossentropy,
     binary_focal_crossentropy,
     categorical_crossentropy,
     categorical_focal_crossentropy,
@@ -84,14 +89,15 @@
     huber,
     # Hinge
     hinge,
     squared_hinge,
     categorical_hinge,
     # Image segmentation
     dice,
+    tversky,
 }
 
 ALL_OBJECTS_DICT = {cls.__name__: cls for cls in ALL_OBJECTS}
 ALL_OBJECTS_DICT.update(
     {
         "bce": binary_crossentropy,
         "BCE": binary_crossentropy,
@@ -125,16 +131,16 @@
 @keras_export("keras.losses.deserialize")
 def deserialize(name, custom_objects=None):
     """Deserializes a serialized loss class/function instance.
 
     Args:
         name: Loss configuration.
         custom_objects: Optional dictionary mapping names (strings) to custom
-          objects (classes and functions) to be considered during
-          deserialization.
+            objects (classes and functions) to be considered during
+            deserialization.
 
     Returns:
         A Keras `Loss` instance or a loss function.
     """
     return serialization_lib.deserialize_keras_object(
         name,
         module_objects=ALL_OBJECTS_DICT,
@@ -179,11 +185,12 @@
         obj = deserialize(identifier)
     elif isinstance(identifier, str):
         obj = ALL_OBJECTS_DICT.get(identifier, None)
     else:
         obj = identifier
 
     if callable(obj):
+        if inspect.isclass(obj):
+            obj = obj()
         return obj
     else:
         raise ValueError(f"Could not interpret loss identifier: {identifier}")
-
```

### Comparing `keras-3.2.1/keras/src/losses/loss.py` & `keras-3.3.0/keras/src/losses/loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export(["keras.Loss", "keras.losses.Loss"])
 class Loss:
     """Loss base class.
 
@@ -176,8 +176,7 @@
             mask, sample_weight = squeeze_or_expand_to_same_rank(
                 mask, sample_weight
             )
             sample_weight *= mask
         else:
             sample_weight = mask
     return sample_weight
-
```

### Comparing `keras-3.2.1/keras/src/losses/losses.py` & `keras-3.3.0/keras/src/losses/losses.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,14 +338,18 @@
 
     Formula:
 
     ```python
     loss = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         reduction: Type of reduction to apply to the loss. In almost all cases
             this should be `"sum_over_batch_size"`.
             Supported options are `"sum"`, `"sum_over_batch_size"` or `None`.
         name: Optional name for the loss instance.
     """
 
@@ -1439,14 +1443,18 @@
 
     Formula:
 
     ```python
     loss = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         y_true: Tensor of true targets.
         y_pred: Tensor of predicted targets.
 
     Returns:
         KL Divergence loss values with shape = `[batch_size, d0, .. dN-1]`.
 
@@ -1997,7 +2005,96 @@
     dice = ops.divide(
         2.0 * intersection,
         ops.sum(y_true) + ops.sum(y_pred) + backend.epsilon(),
     )
 
     return 1 - dice
 
+
+@keras_export("keras.losses.Tversky")
+class Tversky(LossFunctionWrapper):
+    """Computes the Tversky loss value between `y_true` and `y_pred`.
+
+    This loss function is weighted by the alpha and beta coefficients
+    that penalize false positives and false negatives.
+
+    With `alpha=0.5` and `beta=0.5`, the loss value becomes equivalent to
+    Dice Loss.
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+        alpha: coefficient controlling incidence of false positives.
+        beta: coefficient controlling incidence of false negatives.
+
+    Returns:
+        Tversky loss value.
+
+    Reference:
+
+    - [Salehi et al., 2017](https://arxiv.org/abs/1706.05721)
+    """
+
+    def __init__(
+        self,
+        alpha=0.5,
+        beta=0.5,
+        reduction="sum_over_batch_size",
+        name="tversky",
+    ):
+        super().__init__(
+            tversky,
+            alpha=alpha,
+            beta=beta,
+            name=name,
+            reduction=reduction,
+        )
+        self.alpha = alpha
+        self.beta = beta
+
+    def get_config(self):
+        return {
+            "name": self.name,
+            "alpha": self.alpha,
+            "beta": self.beta,
+            "reduction": self.reduction,
+        }
+
+
+@keras_export("keras.losses.tversky")
+def tversky(y_true, y_pred, alpha=0.5, beta=0.5):
+    """Computes the Tversky loss value between `y_true` and `y_pred`.
+
+    This loss function is weighted by the alpha and beta coefficients
+    that penalize false positives and false negatives.
+
+    With `alpha=0.5` and `beta=0.5`, the loss value becomes equivalent to
+    Dice Loss.
+
+    Args:
+        y_true: tensor of true targets.
+        y_pred: tensor of predicted targets.
+        alpha: coefficient controlling incidence of false positives.
+        beta: coefficient controlling incidence of false negatives.
+
+    Returns:
+        Tversky loss value.
+
+    Reference:
+
+    - [Salehi et al., 2017](https://arxiv.org/abs/1706.05721)
+    """
+    y_pred = ops.convert_to_tensor(y_pred)
+    y_true = ops.cast(y_true, y_pred.dtype)
+
+    inputs = ops.reshape(y_true, [-1])
+    targets = ops.reshape(y_pred, [-1])
+
+    intersection = ops.sum(inputs * targets)
+    fp = ops.sum((1 - targets) * inputs)
+    fn = ops.sum(targets * (1 - inputs))
+    tversky = ops.divide(
+        intersection,
+        intersection + fp * alpha + fn * beta + backend.epsilon(),
+    )
+
+    return 1 - tversky
```

### Comparing `keras-3.2.1/keras/src/metrics/__init__.py` & `keras-3.3.0/keras/src/metrics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 from keras.src.metrics.iou_metrics import OneHotIoU
 from keras.src.metrics.iou_metrics import OneHotMeanIoU
 from keras.src.metrics.metric import Metric
 from keras.src.metrics.probabilistic_metrics import BinaryCrossentropy
 from keras.src.metrics.probabilistic_metrics import CategoricalCrossentropy
 from keras.src.metrics.probabilistic_metrics import KLDivergence
 from keras.src.metrics.probabilistic_metrics import Poisson
-from keras.src.metrics.probabilistic_metrics import SparseCategoricalCrossentropy
+from keras.src.metrics.probabilistic_metrics import (
+    SparseCategoricalCrossentropy,
+)
 from keras.src.metrics.reduction_metrics import Mean
 from keras.src.metrics.reduction_metrics import MeanMetricWrapper
 from keras.src.metrics.reduction_metrics import Sum
 from keras.src.metrics.regression_metrics import CosineSimilarity
 from keras.src.metrics.regression_metrics import LogCoshError
 from keras.src.metrics.regression_metrics import MeanAbsoluteError
 from keras.src.metrics.regression_metrics import MeanAbsolutePercentageError
@@ -198,8 +200,7 @@
         obj = identifier
     if callable(obj):
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(f"Could not interpret metric identifier: {identifier}")
-
```

### Comparing `keras-3.2.1/keras/src/metrics/accuracy_metrics.py` & `keras-3.3.0/keras/src/metrics/accuracy_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -463,8 +463,7 @@
         )
         self.k = k
         # Metric should be maximized during optimization.
         self._direction = "up"
 
     def get_config(self):
         return {"name": self.name, "dtype": self.dtype, "k": self.k}
-
```

### Comparing `keras-3.2.1/keras/src/metrics/confusion_metrics.py` & `keras-3.3.0/keras/src/metrics/confusion_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1573,8 +1573,7 @@
         if self._init_from_thresholds:
             # We remove the endpoint thresholds as an inverse of how the
             # thresholds were initialized. This ensures that a metric
             # initialized from this config has the same thresholds.
             config["thresholds"] = self.thresholds[1:-1]
         base_config = super().get_config()
         return {**base_config, **config}
-
```

### Comparing `keras-3.2.1/keras/src/metrics/f_score_metrics.py` & `keras-3.3.0/keras/src/metrics/f_score_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,8 +314,7 @@
             dtype=dtype,
         )
 
     def get_config(self):
         base_config = super().get_config()
         del base_config["beta"]
         return base_config
-
```

### Comparing `keras-3.2.1/keras/src/metrics/hinge_metrics.py` & `keras-3.3.0/keras/src/metrics/hinge_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,7 @@
     def __init__(self, name="categorical_hinge", dtype=None):
         super().__init__(fn=categorical_hinge, name=name, dtype=dtype)
         # Metric should be minimized during optimization.
         self._direction = "down"
 
     def get_config(self):
         return {"name": self.name, "dtype": self.dtype}
-
```

### Comparing `keras-3.2.1/keras/src/metrics/iou_metrics.py` & `keras-3.3.0/keras/src/metrics/iou_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,18 +111,20 @@
         sample_weight = ops.broadcast_to(sample_weight, ops.shape(y_true))
 
         if self.ignore_class is not None:
             ignore_class = ops.convert_to_tensor(
                 self.ignore_class, y_true.dtype
             )
             valid_mask = ops.not_equal(y_true, ignore_class)
-            y_true = y_true[valid_mask]
-            y_pred = y_pred[valid_mask]
+            y_true = y_true * ops.cast(valid_mask, y_true.dtype)
+            y_pred = y_pred * ops.cast(valid_mask, y_pred.dtype)
             if sample_weight is not None:
-                sample_weight = sample_weight[valid_mask]
+                sample_weight = sample_weight * ops.cast(
+                    valid_mask, sample_weight.dtype
+                )
 
         y_pred = ops.cast(y_pred, dtype=self.dtype)
         y_true = ops.cast(y_true, dtype=self.dtype)
         sample_weight = ops.cast(sample_weight, dtype=self.dtype)
 
         current_cm = confusion_matrix(
             y_true,
@@ -741,8 +743,7 @@
             "num_classes": self.num_classes,
             "name": self.name,
             "dtype": self._dtype,
             "ignore_class": self.ignore_class,
             "sparse_y_pred": self.sparse_y_pred,
             "axis": self.axis,
         }
-
```

### Comparing `keras-3.2.1/keras/src/metrics/metric.py` & `keras-3.3.0/keras/src/metrics/metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,8 +237,7 @@
             )
 
     def __repr__(self):
         return f"<{self.__class__.__name__} " f"name={self.name}>"
 
     def __str__(self):
         return self.__repr__()
-
```

### Comparing `keras-3.2.1/keras/src/metrics/metrics_utils.py` & `keras-3.3.0/keras/src/metrics/metrics_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -677,8 +677,7 @@
     indices = ops.stack([labels, predictions], axis=1)
     values = ops.ones_like(predictions, dtype) if weights is None else weights
     indices = ops.cast(indices, dtype="int64")
     values = ops.cast(values, dtype=dtype)
     num_classes = int(num_classes)
     confusion_matrix = ops.scatter(indices, values, (num_classes, num_classes))
     return confusion_matrix
-
```

### Comparing `keras-3.2.1/keras/src/metrics/probabilistic_metrics.py` & `keras-3.3.0/keras/src/metrics/probabilistic_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,18 @@
 
     Formula:
 
     ```python
     metric = y_true * log(y_true / y_pred)
     ```
 
+    `y_true` and `y_pred` are expected to be probability
+    distributions, with values between 0 and 1. They will get
+    clipped to the `[0, 1]` range.
+
     Args:
         name: (Optional) string name of the metric instance.
         dtype: (Optional) data type of the metric result.
 
     Examples:
 
     >>> m = keras.metrics.KLDivergence()
@@ -337,8 +341,7 @@
     def get_config(self):
         return {
             "name": self.name,
             "dtype": self.dtype,
             "from_logits": self.from_logits,
             "axis": self.axis,
         }
-
```

### Comparing `keras-3.2.1/keras/src/metrics/reduction_metrics.py` & `keras-3.3.0/keras/src/metrics/reduction_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,8 +213,7 @@
         return {**base_config, **config}
 
     @classmethod
     def from_config(cls, config):
         if "fn" in config:
             config = serialization_lib.deserialize_keras_object(config)
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/metrics/regression_metrics.py` & `keras-3.3.0/keras/src/metrics/regression_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -609,8 +609,7 @@
     """
     y_pred = ops.convert_to_tensor(y_pred)
     y_true = ops.convert_to_tensor(y_true, dtype=y_pred.dtype)
     y_true, y_pred = squeeze_or_expand_to_same_rank(y_true, y_pred)
     y_pred = normalize(y_pred, axis=axis)
     y_true = normalize(y_true, axis=axis)
     return ops.sum(y_true * y_pred, axis=axis)
-
```

### Comparing `keras-3.2.1/keras/src/models/cloning.py` & `keras-3.3.0/keras/src/models/cloning.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from keras.src import backend
+from keras.src import tree
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers import Input
 from keras.src.layers import InputLayer
 from keras.src.models.functional import Functional
 from keras.src.models.functional import functional_like_constructor
 from keras.src.models.sequential import Sequential
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export("keras.models.clone_model")
 def clone_model(model, input_tensors=None, clone_function=None):
     """Clone a Functional or Sequential `Model` instance.
 
     Model cloning is similar to calling a model on new inputs,
@@ -286,8 +286,7 @@
     else:
         # This may be incorrect: the new model will end up having a different
         # class than the original. However various existing models rely
         # on this behavior, so we keep it.
         new_model = Functional(input_tensors, output_tensors, name=model.name)
 
     return new_model
-
```

### Comparing `keras-3.2.1/keras/src/models/functional.py` & `keras-3.3.0/keras/src/models/functional.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import copy
 import inspect
 import typing
 import warnings
 
 from keras.src import backend
 from keras.src import ops
+from keras.src import tree
 from keras.src.backend.common import global_state
 from keras.src.layers.core.input_layer import Input
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.input_spec import InputSpec
 from keras.src.layers.layer import Layer
 from keras.src.legacy.saving import saving_utils
 from keras.src.legacy.saving import serialization as legacy_serialization
@@ -16,15 +17,14 @@
 from keras.src.ops.function import Function
 from keras.src.ops.function import _build_map
 from keras.src.ops.function import make_node_key
 from keras.src.ops.node import KerasHistory
 from keras.src.ops.node import Node
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class Functional(Function, Model):
     """A `Functional` model is a `Model` defined as a directed graph of layers.
 
     Three types of `Model` exist: subclassed `Model`, `Functional` model,
     and `Sequential` (a special case of `Functional`).
@@ -476,15 +476,15 @@
         """
         args, kwargs = deserialize_node(node_data, created_layers)
         # Call layer on its inputs, thus creating the node
         # and building the layer if needed.
         layer(*args, **kwargs)
 
     def process_layer(layer_data):
-        """Deserializes a layer, then call it on appropriate inputs.
+        """Deserializes a layer and index its inbound nodes.
 
         Args:
             layer_data: layer config dict.
         """
         layer_name = layer_data["name"]
 
         # Instantiate layer.
@@ -549,22 +549,28 @@
     # Create lits of input and output tensors and return new class
     name = config.get("name")
     trainable = config.get("trainable")
 
     def get_tensor(layer_name, node_index, tensor_index):
         assert layer_name in created_layers
         layer = created_layers[layer_name]
+        if isinstance(layer, Functional):
+            # Functional models start out with a built-in node.
+            node_index -= 1
         layer_output_tensors = layer._inbound_nodes[node_index].output_tensors
         return layer_output_tensors[tensor_index]
 
     def map_tensors(tensors):
         if isinstance(tensors, dict):
             return {k: get_tensor(*v) for k, v in tensors.items()}
         else:
-            return [get_tensor(*v) for v in tensors]
+            tensor_list = [get_tensor(*v) for v in tensors]
+            if len(tensor_list) == 1:
+                return tensor_list[0]
+            return tensor_list
 
     input_tensors = map_tensors(config["input_layers"])
     output_tensors = map_tensors(config["output_layers"])
     return cls(
         inputs=input_tensors,
         outputs=output_tensors,
         name=name,
@@ -606,16 +612,17 @@
 
     def serialize_keras_tensor(x):
         # Serialize KerasTensor while converting
         # node indices to only include nodes relevant to `own_nodes`.
         if isinstance(x, backend.KerasTensor):
             operation, node_index, tensor_index = x._keras_history
             irrelevant_node_count = 0
-            for node in operation._inbound_nodes[:node_index]:
-                if node not in own_nodes:
+            for i, node in enumerate(operation._inbound_nodes[:node_index]):
+                node_key = make_node_key(operation, i)
+                if node_key not in own_nodes:
                     irrelevant_node_count += 1
             x._keras_history = KerasHistory(
                 operation, node_index - irrelevant_node_count, tensor_index
             )
             serialized = serialization_lib.serialize_keras_object(x)
             x._keras_history = KerasHistory(operation, node_index, tensor_index)
             return serialized
@@ -761,15 +768,15 @@
     # cloned The key is the string ID of the original keras tensor, and value is
     # the cloned Keras tensor instance.
     kt_id_mapping = {}
     op_id_mapping = {}
 
     for kt_input in tree.flatten(inputs):
         if is_input_keras_tensor(kt_input):
-            # For any existing Keras tensor from keras.src.Input, leave them as is.
+            # For any existing Keras tensor from keras.Input, leave them as is.
             cloned_inputs.append(kt_input)
             kt_id_mapping[id(kt_input)] = kt_input
         else:
             # We need to create a new Keras tensor for any intermediate tensor
             cloned_input = Input(
                 batch_shape=kt_input.shape,
                 dtype=kt_input.dtype,
@@ -817,8 +824,7 @@
         Node(
             operation,
             call_args=call_args_copy,
             call_kwargs=call_kwargs_copy,
             outputs=output_copy,
         )
     return cloned_inputs, cloned_outputs
-
```

### Comparing `keras-3.2.1/keras/src/models/model.py` & `keras-3.3.0/keras/src/models/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import inspect
+import io
 import json
 import typing
 import warnings
 
+import keras.src.saving.saving_lib as saving_lib
 from keras.src import backend
 from keras.src import utils
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.models.variable_mapping import map_trackable_variables
 from keras.src.saving import saving_api
 from keras.src.trainers import trainer as base_trainer
 from keras.src.utils import summary_utils
 from keras.src.utils import traceback_utils
 
 if backend.backend() == "tensorflow":
-    from keras.src.backend.tensorflow.trainer import TensorFlowTrainer as Trainer
+    from keras.src.backend.tensorflow.trainer import (
+        TensorFlowTrainer as Trainer,
+    )
 elif backend.backend() == "jax":
     from keras.src.backend.jax.trainer import JAXTrainer as Trainer
 elif backend.backend() == "torch":
     from keras.src.backend.torch.trainer import TorchTrainer as Trainer
 elif backend.backend() == "numpy":
     from keras.src.backend.numpy.trainer import NumpyTrainer as Trainer
 else:
@@ -309,15 +313,15 @@
         Args:
             filepath: `str` or `pathlib.Path` object.
                 Path where to save the model. Must end in `.weights.h5`.
             overwrite: Whether we should overwrite any existing model
                 at the target location, or instead ask the user
                 via an interactive prompt.
         """
-        return saving_api.save_weights(self, filepath, overwrite=True)
+        return saving_api.save_weights(self, filepath, overwrite=overwrite)
 
     @traceback_utils.filter_traceback
     def load_weights(self, filepath, skip_mismatch=False, **kwargs):
         """Load weights from a file saved via `save_weights()`.
 
         Weights are loaded based on the network's
         topology. This means the architecture should be the same as when the
@@ -342,33 +346,59 @@
                 there is a mismatch in the number of weights, or a mismatch in
                 the shape of the weights.
         """
         saving_api.load_weights(
             self, filepath, skip_mismatch=skip_mismatch, **kwargs
         )
 
+    # Note: renaming this function will cause old pickles to be broken.
+    # This is probably not a huge deal, as pickle should not be a recommended
+    # saving format -- it should only be supported for use with distributed
+    # computing frameworks.
+    @classmethod
+    def _unpickle_model(cls, bytesio):
+        # pickle is not safe regardless of what you do.
+        return saving_lib._load_model_from_fileobj(
+            bytesio, custom_objects=None, compile=True, safe_mode=False
+        )
+
+    def __reduce__(self):
+        """__reduce__ is used to customize the behavior of `pickle.pickle()`.
+
+        The method returns a tuple of two elements: a function, and a list of
+        arguments to pass to that function.  In this case we just leverage the
+        keras saving library."""
+        buf = io.BytesIO()
+        saving_lib._save_model_to_fileobj(self, buf, "h5")
+        return (
+            self._unpickle_model,
+            (buf,),
+        )
+
     def quantize(self, mode):
         """Quantize the weights of the model.
 
         Note that the model must be built first before calling this method.
         `quantize` will recursively call `quantize(mode)` in all layers and
         will be skipped if the layer doesn't implement the function.
 
         Args:
             mode: The mode of the quantization. Only 'int8' is supported at this
                 time.
         """
+        from keras.src.dtype_policies import QUANTIZATION_MODES
+
         if not self.built:
             raise ValueError(
                 "The model must be built first before calling `quantize()`."
             )
-        if mode not in ("int8",):
+        if mode not in QUANTIZATION_MODES:
             raise ValueError(
-                "Invalid quantization mode. Expected 'int8'. "
-                f"Received: mode={mode}"
+                "Invalid quantization mode. "
+                f"Expected one of {QUANTIZATION_MODES}. Received: mode={mode}"
             )
         mode_changed = False
         for layer in self._flatten_layers():
             list_of_sublayers = list(layer._flatten_layers())
             if len(list_of_sublayers) == 1:  # leaves of the model
                 try:
                     layer.quantize(mode)
@@ -596,8 +626,7 @@
         inject_functional_model_class(base) for base in cls.__bases__
     )
     # Trigger any `__new__` class swapping that needed to happen on `Functional`
     # but did not because functional was not in the class hierarchy.
     cls.__new__(cls)
 
     return cls
-
```

### Comparing `keras-3.2.1/keras/src/models/sequential.py` & `keras-3.3.0/keras/src/models/sequential.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import copy
 import inspect
 import typing
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
 from keras.src.layers.core.input_layer import InputLayer
 from keras.src.layers.layer import Layer
 from keras.src.legacy.saving import saving_utils
 from keras.src.legacy.saving import serialization as legacy_serialization
 from keras.src.models.functional import Functional
 from keras.src.models.model import Model
 from keras.src.saving import serialization_lib
-from keras.src.utils import tree
 
 
 @keras_export(["keras.Sequential", "keras.models.Sequential"])
 class Sequential(Model):
     """`Sequential` groups a linear stack of layers into a `Model`.
 
     Examples:
@@ -340,8 +340,7 @@
         if (
             not model._functional
             and build_input_shape
             and isinstance(build_input_shape, (tuple, list))
         ):
             model.build(build_input_shape)
         return model
-
```

### Comparing `keras-3.2.1/keras/src/models/variable_mapping.py` & `keras-3.3.0/keras/src/models/variable_mapping.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
     for trackable in container:
         if saving_lib._is_keras_trackable(trackable):
             map_trackable_variables(
                 trackable,
                 store,
                 visited_trackables=visited_trackables,
             )
-
```

### Comparing `keras-3.2.1/keras/src/ops/__init__.py` & `keras-3.3.0/keras/src/ops/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,8 +10,7 @@
 from keras.src.ops import image
 from keras.src.ops import operation_utils
 from keras.src.ops.core import *  # noqa: F403
 from keras.src.ops.linalg import *  # noqa: F403
 from keras.src.ops.math import *  # noqa: F403
 from keras.src.ops.nn import *  # noqa: F403
 from keras.src.ops.numpy import *  # noqa: F403
-
```

### Comparing `keras-3.2.1/keras/src/ops/core.py` & `keras-3.3.0/keras/src/ops/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,20 +13,20 @@
 is_tensor
 custom_gradient
 """
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend import any_symbolic_tensors
 from keras.src.ops.operation import Operation
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class Scatter(Operation):
     def call(self, indices, values, shape):
         return backend.core.scatter(indices, values, shape)
 
     def compute_output_spec(self, indices, values, shape):
@@ -704,8 +704,7 @@
         e = ops.exp(x)
         def grad(*args, upstream):
             return ops.multiply(upstream, 1.0 - 1.0 / ops.add(1, e))
         return ops.log(1 + e), grad
     ```
     """
     return backend.core.custom_gradient(f)
-
```

### Comparing `keras-3.2.1/keras/src/ops/function.py` & `keras-3.3.0/keras/src/ops/function.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend.config import backend
 from keras.src.ops.operation import Operation
-from keras.src.utils import tree
 
 
 @keras_export("keras.Function")
 class Function(Operation):
     """Class that encapsulates a computation graph of Keras operations.
 
     You can use a `Function` to capture the computation graph linking
@@ -399,8 +399,7 @@
                 nodes_in_decreasing_depth,
                 operation_indices,
             )
 
     finished_nodes.add(node)
     nodes_in_progress.remove(node)
     nodes_in_decreasing_depth.append(node)
-
```

### Comparing `keras-3.2.1/keras/src/ops/image.py` & `keras-3.3.0/keras/src/ops/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,35 +3,144 @@
 from keras.src.api_export import keras_export
 from keras.src.backend import KerasTensor
 from keras.src.backend import any_symbolic_tensors
 from keras.src.ops.operation import Operation
 from keras.src.ops.operation_utils import compute_conv_output_shape
 
 
+class RGBToGrayscale(Operation):
+    def __init__(
+        self,
+        data_format="channels_last",
+    ):
+        super().__init__()
+        self.data_format = data_format
+
+    def call(self, image):
+        return backend.image.rgb_to_grayscale(
+            image,
+            data_format=self.data_format,
+        )
+
+    def compute_output_spec(self, image):
+        if len(image.shape) not in (3, 4):
+            raise ValueError(
+                "Invalid image rank: expected rank 3 (single image) "
+                "or rank 4 (batch of images). Received input with shape: "
+                f"image.shape={image.shape}"
+            )
+
+        if len(image.shape) == 3:
+            if self.data_format == "channels_last":
+                return KerasTensor(image.shape[:-1] + (1,), dtype=image.dtype)
+            else:
+                return KerasTensor((1,) + image.shape[1:], dtype=image.dtype)
+        elif len(image.shape) == 4:
+            if self.data_format == "channels_last":
+                return KerasTensor(
+                    (image.shape[0],) + image.shape[1:-1] + (1,),
+                    dtype=image.dtype,
+                )
+            else:
+                return KerasTensor(
+                    (
+                        image.shape[0],
+                        1,
+                    )
+                    + image.shape[2:],
+                    dtype=image.dtype,
+                )
+
+
+@keras_export("keras.ops.image.rgb_to_grayscale")
+def rgb_to_grayscale(
+    image,
+    data_format="channels_last",
+):
+    """Convert RGB images to grayscale.
+
+    This function converts RGB images to grayscale images. It supports both
+    3D and 4D tensors, where the last dimension represents channels.
+
+    Args:
+        image: Input RGB image or batch of RGB images. Must be a 3D tensor
+            with shape `(height, width, channels)` or a 4D tensor with shape
+            `(batch, height, width, channels)`.
+        data_format: A string specifying the data format of the input tensor.
+            It can be either `"channels_last"` or `"channels_first"`.
+            `"channels_last"` corresponds to inputs with shape
+            `(batch, height, width, channels)`, while `"channels_first"`
+            corresponds to inputs with shape `(batch, channels, height, width)`.
+            Defaults to `"channels_last"`.
+
+    Returns:
+        Grayscale image or batch of grayscale images.
+
+    Examples:
+
+    >>> import numpy as np
+    >>> from keras.src import ops
+    >>> x = np.random.random((2, 4, 4, 3))
+    >>> y = ops.image.rgb_to_grayscale(x)
+    >>> y.shape
+    (2, 4, 4, 1)
+
+    >>> x = np.random.random((4, 4, 3)) # Single RGB image
+    >>> y = ops.image.rgb_to_grayscale(x)
+    >>> y.shape
+    (4, 4, 1)
+
+    >>> x = np.random.random((2, 3, 4, 4))
+    >>> y = ops.image.rgb_to_grayscale(x, data_format="channels_first")
+    >>> y.shape
+    (2, 1, 4, 4)
+    """
+    if any_symbolic_tensors((image,)):
+        return RGBToGrayscale(
+            data_format=data_format,
+        ).symbolic_call(image)
+    return backend.image.rgb_to_grayscale(
+        image,
+        data_format=data_format,
+    )
+
+
 class Resize(Operation):
     def __init__(
         self,
         size,
         interpolation="bilinear",
         antialias=False,
+        crop_to_aspect_ratio=False,
+        pad_to_aspect_ratio=False,
+        fill_mode="constant",
+        fill_value=0.0,
         data_format="channels_last",
     ):
         super().__init__()
         self.size = tuple(size)
         self.interpolation = interpolation
         self.antialias = antialias
         self.data_format = data_format
+        self.crop_to_aspect_ratio = crop_to_aspect_ratio
+        self.pad_to_aspect_ratio = pad_to_aspect_ratio
+        self.fill_mode = fill_mode
+        self.fill_value = fill_value
 
     def call(self, image):
         return backend.image.resize(
             image,
             self.size,
             interpolation=self.interpolation,
             antialias=self.antialias,
             data_format=self.data_format,
+            crop_to_aspect_ratio=self.crop_to_aspect_ratio,
+            pad_to_aspect_ratio=self.pad_to_aspect_ratio,
+            fill_mode=self.fill_mode,
+            fill_value=self.fill_value,
         )
 
     def compute_output_spec(self, image):
         if len(image.shape) == 3:
             return KerasTensor(
                 self.size + (image.shape[-1],), dtype=image.dtype
             )
@@ -55,25 +164,45 @@
 
 @keras_export("keras.ops.image.resize")
 def resize(
     image,
     size,
     interpolation="bilinear",
     antialias=False,
+    crop_to_aspect_ratio=False,
+    pad_to_aspect_ratio=False,
+    fill_mode="constant",
+    fill_value=0.0,
     data_format="channels_last",
 ):
     """Resize images to size using the specified interpolation method.
 
     Args:
         image: Input image or batch of images. Must be 3D or 4D.
         size: Size of output image in `(height, width)` format.
         interpolation: Interpolation method. Available methods are `"nearest"`,
             `"bilinear"`, and `"bicubic"`. Defaults to `"bilinear"`.
         antialias: Whether to use an antialiasing filter when downsampling an
             image. Defaults to `False`.
+        crop_to_aspect_ratio: If `True`, resize the images without aspect
+            ratio distortion. When the original aspect ratio differs
+            from the target aspect ratio, the output image will be
+            cropped so as to return the
+            largest possible window in the image (of size `(height, width)`)
+            that matches the target aspect ratio. By default
+            (`crop_to_aspect_ratio=False`), aspect ratio may not be preserved.
+        pad_to_aspect_ratio: If `True`, pad the images without aspect
+            ratio distortion. When the original aspect ratio differs
+            from the target aspect ratio, the output image will be
+            evenly padded on the short side.
+        fill_mode: When using `pad_to_aspect_ratio=True`, padded areas
+            are filled according to the given mode. Only `"constant"` is
+            supported at this time
+            (fill with constant value, equal to `fill_value`).
+        fill_value: Float. Padding value to use when `pad_to_aspect_ratio=True`.
         data_format: string, either `"channels_last"` or `"channels_first"`.
             The ordering of the dimensions in the inputs. `"channels_last"`
             corresponds to inputs with shape `(batch, height, width, channels)`
             while `"channels_first"` corresponds to inputs with shape
             `(batch, channels, height, weight)`. It defaults to the
             `image_data_format` value found in your Keras config file at
             `~/.keras/keras.json`. If you never set it, then it will be
@@ -96,28 +225,51 @@
 
     >>> x = np.random.random((2, 3, 4, 4)) # batch of 2 RGB images
     >>> y = keras.ops.image.resize(x, (2, 2),
     ...     data_format="channels_first")
     >>> y.shape
     (2, 3, 2, 2)
     """
-
+    if len(size) != 2:
+        raise ValueError(
+            "Expected `size` to be a tuple of 2 integers. "
+            f"Received: size={size}"
+        )
+    if len(image.shape) < 3 or len(image.shape) > 4:
+        raise ValueError(
+            "Expected an image array with shape `(height, width, "
+            "channels)`, or `(batch_size, height, width, channels)`, but "
+            f"got input with incorrect rank, of shape {image.shape}."
+        )
+    if pad_to_aspect_ratio and crop_to_aspect_ratio:
+        raise ValueError(
+            "Only one of `pad_to_aspect_ratio` & `crop_to_aspect_ratio` "
+            "can be `True`."
+        )
     if any_symbolic_tensors((image,)):
         return Resize(
             size,
             interpolation=interpolation,
             antialias=antialias,
             data_format=data_format,
+            crop_to_aspect_ratio=crop_to_aspect_ratio,
+            pad_to_aspect_ratio=pad_to_aspect_ratio,
+            fill_mode=fill_mode,
+            fill_value=fill_value,
         ).symbolic_call(image)
     return backend.image.resize(
         image,
         size,
         interpolation=interpolation,
         antialias=antialias,
+        crop_to_aspect_ratio=crop_to_aspect_ratio,
         data_format=data_format,
+        pad_to_aspect_ratio=pad_to_aspect_ratio,
+        fill_mode=fill_mode,
+        fill_value=fill_value,
     )
 
 
 class AffineTransform(Operation):
     def __init__(
         self,
         interpolation="bilinear",
@@ -414,15 +566,15 @@
     )
     if _unbatched:
         patches = backend.numpy.squeeze(patches, axis=0)
     return patches
 
 
 class MapCoordinates(Operation):
-    def __init__(self, order, fill_mode="constant", fill_value=0):
+    def __init__(self, order=1, fill_mode="constant", fill_value=0):
         super().__init__()
         self.order = order
         self.fill_mode = fill_mode
         self.fill_value = fill_value
 
     def call(self, image, coordinates):
         return backend.image.map_coordinates(
@@ -932,8 +1084,7 @@
 
     cropped_shape = [batch, target_height, target_width, depth]
     cropped = backend.numpy.reshape(cropped, cropped_shape)
 
     if not is_batch:
         cropped = backend.numpy.squeeze(cropped, axis=[0])
     return cropped
-
```

### Comparing `keras-3.2.1/keras/src/ops/linalg.py` & `keras-3.3.0/keras/src/ops/linalg.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,16 @@
     def __init__(self):
         super().__init__()
 
     def call(self, x):
         return _eig(x)
 
     def compute_output_spec(self, x):
-        _assert_2d(x)
         _assert_square(x)
+        _assert_2d(x)
         return (
             KerasTensor(x.shape[:-1], x.dtype),
             KerasTensor(x.shape, x.dtype),
         )
 
 
 @keras_export(["keras.ops.eig", "keras.ops.linalg.eig"])
@@ -106,28 +106,68 @@
 
     Args:
         x: Input tensor of shape `(..., M, M)`.
 
     Returns:
         A tuple of two tensors: a tensor of shape `(..., M)` containing
         eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
-
     """
     if any_symbolic_tensors((x,)):
         return Eig().symbolic_call(x)
     return _eig(x)
 
 
 def _eig(x):
     x = backend.convert_to_tensor(x)
-    _assert_2d(x)
     _assert_square(x)
+    _assert_2d(x)
     return backend.linalg.eig(x)
 
 
+class Eigh(Operation):
+
+    def __init__(self):
+        super().__init__()
+
+    def call(self, x):
+        return _eigh(x)
+
+    def compute_output_spec(self, x):
+        _assert_square(x)
+        _assert_2d(x)
+        return (
+            KerasTensor(x.shape[:-1], x.dtype),
+            KerasTensor(x.shape, x.dtype),
+        )
+
+
+@keras_export(["keras.ops.eigh", "keras.ops.linalg.eigh"])
+def eigh(x):
+    """Computes the eigenvalues and eigenvectors of a complex Hermitian.
+
+    Args:
+        x: Input tensor of shape `(..., M, M)`.
+
+    Returns:
+        A tuple of two tensors: a tensor of shape `(..., M)` containing
+        eigenvalues and a tensor of shape `(..., M, M)` containing eigenvectors.
+
+    """
+    if any_symbolic_tensors((x,)):
+        return Eigh().symbolic_call(x)
+    return _eigh(x)
+
+
+def _eigh(x):
+    x = backend.convert_to_tensor(x)
+    _assert_square(x)
+    _assert_2d(x)
+    return backend.linalg.eigh(x)
+
+
 class Inv(Operation):
 
     def __init__(self):
         super().__init__()
 
     def call(self, x):
         return _inv(x)
@@ -592,8 +632,7 @@
     elif a.ndim == b.ndim - 1:
         if a.shape[-1] != b.shape[-1]:
             raise ValueError(
                 "Incompatible shapes between `a` and `b`. "
                 "Expected `a.shape[-1] == b.shape[-1]`. "
                 f"Received: a.shape={a.shape}, b.shape={b.shape}"
             )
-
```

### Comparing `keras-3.2.1/keras/src/ops/math.py` & `keras-3.3.0/keras/src/ops/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -920,8 +920,7 @@
     >>> keras.ops.erfinv(x)
     array([-0.47694, -0.17914, -0.08886,  0. ,  0.27246], dtype=float32)
     """
     if any_symbolic_tensors((x,)):
         return Erfinv().symbolic_call(x)
     x = backend.convert_to_tensor(x)
     return backend.math.erfinv(x)
-
```

### Comparing `keras-3.2.1/keras/src/ops/nn.py` & `keras-3.3.0/keras/src/ops/nn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1869,14 +1869,74 @@
             target, output, target_length, output_length
         )
     return backend.nn.ctc_loss(
         target, output, target_length, output_length, mask_index
     )
 
 
+@keras_export(
+    [
+        "keras.ops.ctc_decode",
+        "keras.ops.nn.ctc_decode",
+    ]
+)
+def ctc_decode(
+    inputs,
+    sequence_lengths,
+    strategy,
+    beam_width=100,
+    top_paths=1,
+    merge_repeated=True,
+    mask_index=None,
+):
+    """Decodes the output of a CTC model.
+
+    Args:
+        inputs: A tensor of shape `(batch_size, max_length, num_classes)`
+            containing the logits (output of the model).
+        sequence_lengths: A tensor of shape `(batch_size,)` containing the
+            sequence lengths for the batch.
+        strategy: A string for the decoding strategy. Supported values are
+            `"greedy"` and `"beam_search"`.
+        beam_width: An integer scalar beam width used in beam search.
+            Defaults to 100.
+        top_paths: An integer scalar, the number of top paths to return.
+            Defaults to 1.
+        merge_repeated: A boolean scalar, whether to merge repeated
+            labels in the output. Defaults to `True`.
+        mask_index: An integer scalar, the index of the mask character in
+            the vocabulary. Defaults to `None`.
+
+    Returns:
+        A tuple containing:
+
+        - A list of decoded sequences.
+        - A list of the negative of the sum of the probability logits
+        (if strategy is `"greedy"`) or the log probability (if strategy is
+        `"beam_search"`) for each sequence.
+    """
+
+    if any_symbolic_tensors((inputs, sequence_lengths)):
+        raise NotImplementedError(
+            "CTC decoding is not supported with KerasTensors. Use it "
+            "inside the call() method of a Layer or the predict_step "
+            "method of a model."
+        )
+
+    return backend.nn.ctc_decode(
+        inputs=inputs,
+        sequence_length=sequence_lengths,
+        strategy=strategy,
+        beam_width=beam_width,
+        top_paths=top_paths,
+        merge_repeated=merge_repeated,
+        mask_index=mask_index,
+    )
+
+
 class Normalize(Operation):
     def __init__(self, axis=-1, order=2):
         super().__init__()
         self.axis = axis
         self.order = order
 
     def compute_output_spec(self, x):
@@ -1929,8 +1989,7 @@
     x = backend.convert_to_tensor(x)
     if len(x.shape) == 0:
         x = backend.numpy.expand_dims(x, axis=0)
     epsilon = backend.epsilon()
     norm = backend.linalg.norm(x, ord=order, axis=axis, keepdims=True)
     denom = backend.numpy.maximum(norm, epsilon)
     return backend.numpy.divide(x, denom)
-
```

### Comparing `keras-3.2.1/keras/src/ops/node.py` & `keras-3.3.0/keras/src/ops/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import collections
 
+from keras.src import tree
 from keras.src.backend import KerasTensor
 from keras.src.ops.symbolic_arguments import SymbolicArguments
-from keras.src.utils import tree
 
 
 class Node:
     """A `Node` describes an operation `__call__()` event.
 
     A Keras Function is a DAG with `Node` instances as nodes, and
     `KerasTensor` instances as edges. Nodes aren't `Operation` instances,
@@ -78,15 +78,15 @@
                     operation=operation, node_index=node_index, tensor_index=i
                 )
 
         # Whether this is a root node.
         self.is_input = not self.arguments.keras_tensors
 
     def __repr__(self):
-        return f"<Node operation={self.operation}, id={id(self)}>"
+        return f"<Node operation={self.operation.name}, id={id(self)}>"
 
     @property
     def input_tensors(self):
         return self.arguments.keras_tensors
 
     @property
     def output_tensors(self):
@@ -137,8 +137,7 @@
     # Added to maintain memory and performance characteristics of `namedtuple`
     # while subclassing.
     __slots__ = ()
 
 
 def is_keras_tensor(obj):
     return hasattr(obj, "_keras_history")
-
```

### Comparing `keras-3.2.1/keras/src/ops/numpy.py` & `keras-3.3.0/keras/src/ops/numpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         axis: An integer or tuple of integers that represent the axis along
             which a logical AND reduction is performed. The default
             (`axis=None`) is to perform a logical AND over all the dimensions
             of the input array. `axis` may be negative, in which case it counts
             for the last to the first axis.
         keepdims: If `True`, axes which are reduced are left in the result as
             dimensions with size one. With this option, the result will
-            broadcast correctly against the input array. Defaults to`False`.
+            broadcast correctly against the input array. Defaults to `False`.
 
     Returns:
         The tensor containing the logical AND reduction over the `axis`.
 
     Examples:
     >>> x = keras.ops.convert_to_tensor([True, False])
     >>> keras.ops.all(x)
@@ -412,15 +412,15 @@
         axis: An integer or tuple of integers that represent the axis along
             which a logical OR reduction is performed. The default
             (`axis=None`) is to perform a logical OR over all the dimensions
             of the input array. `axis` may be negative, in which case it counts
             for the last to the first axis.
         keepdims: If `True`, axes which are reduced are left in the result as
             dimensions with size one. With this option, the result will
-            broadcast correctly against the input array. Defaults to`False`.
+            broadcast correctly against the input array. Defaults to `False`.
 
     Returns:
         The tensor containing the logical OR reduction over the `axis`.
 
     Examples:
     >>> x = keras.ops.convert_to_tensor([True, False])
     >>> keras.ops.any(x)
@@ -959,37 +959,42 @@
     """
     if any_symbolic_tensors((x,)):
         return Arctanh().symbolic_call(x)
     return backend.numpy.arctanh(x)
 
 
 class Argmax(Operation):
-    def __init__(self, axis=None):
+    def __init__(self, axis=None, keepdims=False):
         super().__init__()
         self.axis = axis
+        self.keepdims = keepdims
 
     def call(self, x):
-        return backend.numpy.argmax(x, axis=self.axis)
+        return backend.numpy.argmax(x, axis=self.axis, keepdims=self.keepdims)
 
     def compute_output_spec(self, x):
+        if self.keepdims:
+            return KerasTensor(x.shape, dtype="int32")
         if self.axis is None:
             return KerasTensor([], dtype="int32")
         return KerasTensor(
             reduce_shape(x.shape, axis=[self.axis]), dtype="int32"
         )
 
 
 @keras_export(["keras.ops.argmax", "keras.ops.numpy.argmax"])
-def argmax(x, axis=None):
+def argmax(x, axis=None, keepdims=False):
     """Returns the indices of the maximum values along an axis.
 
     Args:
         x: Input tensor.
         axis: By default, the index is into the flattened tensor, otherwise
             along the specified axis.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one. Defaults to `False`.
 
     Returns:
         Tensor of indices. It has the same shape as `x`, with the dimension
         along `axis` removed.
 
     Example:
     >>> x = keras.ops.arange(6).reshape(2, 3) + 10
@@ -1000,42 +1005,47 @@
     array(5, dtype=int32)
     >>> keras.ops.argmax(x, axis=0)
     array([1, 1, 1], dtype=int32)
     >>> keras.ops.argmax(x, axis=1)
     array([2, 2], dtype=int32)
     """
     if any_symbolic_tensors((x,)):
-        return Argmax(axis=axis).symbolic_call(x)
-    return backend.numpy.argmax(x, axis=axis)
+        return Argmax(axis=axis, keepdims=keepdims).symbolic_call(x)
+    return backend.numpy.argmax(x, axis=axis, keepdims=keepdims)
 
 
 class Argmin(Operation):
-    def __init__(self, axis=None):
+    def __init__(self, axis=None, keepdims=False):
         super().__init__()
         self.axis = axis
+        self.keepdims = keepdims
 
     def call(self, x):
-        return backend.numpy.argmin(x, axis=self.axis)
+        return backend.numpy.argmin(x, axis=self.axis, keepdims=self.keepdims)
 
     def compute_output_spec(self, x):
+        if self.keepdims:
+            return KerasTensor(x.shape, dtype="int32")
         if self.axis is None:
             return KerasTensor([], dtype="int32")
         return KerasTensor(
             reduce_shape(x.shape, axis=[self.axis]), dtype="int32"
         )
 
 
 @keras_export(["keras.ops.argmin", "keras.ops.numpy.argmin"])
-def argmin(x, axis=None):
+def argmin(x, axis=None, keepdims=False):
     """Returns the indices of the minium values along an axis.
 
     Args:
         x: Input tensor.
         axis: By default, the index is into the flattened tensor, otherwise
             along the specified axis.
+        keepdims: If this is set to `True`, the axes which are reduced are left
+            in the result as dimensions with size one. Defaults to `False`.
 
     Returns:
         Tensor of indices. It has the same shape as `x`, with the dimension
         along `axis` removed.
 
     Example:
     >>> x = keras.ops.arange(6).reshape(2, 3) + 10
@@ -1046,16 +1056,16 @@
     array(0, dtype=int32)
     >>> keras.ops.argmin(x, axis=0)
     array([0, 0, 0], dtype=int32)
     >>> keras.ops.argmin(x, axis=1)
     array([0, 0], dtype=int32)
     """
     if any_symbolic_tensors((x,)):
-        return Argmin(axis=axis).symbolic_call(x)
-    return backend.numpy.argmin(x, axis=axis)
+        return Argmin(axis=axis, keepdims=keepdims).symbolic_call(x)
+    return backend.numpy.argmin(x, axis=axis, keepdims=keepdims)
 
 
 class Argsort(Operation):
     def __init__(self, axis=-1):
         super().__init__()
         self.axis = axis
 
@@ -1259,16 +1269,19 @@
         dtypes_to_resolve = [x.dtype]
         if self.weights is not None:
             weights = backend.convert_to_tensor(self.weights)
             dtypes_to_resolve.append(weights.dtype)
             dtype = dtypes.result_type(*dtypes_to_resolve)
         else:
             dtype = "int32"
+        x_sparse = getattr(x, "sparse", False)
         return KerasTensor(
-            list(x.shape[:-1]) + [None], dtype=dtype, sparse=self.sparse
+            list(x.shape[:-1]) + [None],
+            dtype=dtype,
+            sparse=x_sparse or self.sparse,
         )
 
 
 @keras_export(["keras.ops.bincount", "keras.ops.numpy.bincount"])
 def bincount(x, weights=None, minlength=0, sparse=False):
     """Count the number of occurrences of each value in a tensor of integers.
 
@@ -1877,15 +1890,15 @@
             above the main diagonal, and `k < 0` for diagonals below
             the main diagonal.
 
     Returns:
         The extracted diagonal or constructed diagonal tensor.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.arange(9).reshape((3, 3))
     >>> x
     array([[0, 1, 2],
            [3, 4, 5],
            [6, 7, 8]])
 
     >>> ops.diag(x)
@@ -1971,15 +1984,15 @@
         axis2: Axis to be used as the second axis of the 2-D sub-arrays.
             Defaults to `1` (second axis).
 
     Returns:
         Tensor of diagonals.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.arange(4).reshape((2, 2))
     >>> x
     array([[0, 1],
            [2, 3]])
     >>> x.diagonal()
     array([0, 3])
     >>> x.diagonal(1)
@@ -2040,15 +2053,15 @@
         axis: Axis to compute discrete difference(s) along.
             Defaults to `-1`.(last axis).
 
     Returns:
         Tensor of diagonals.
 
     Examples:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.convert_to_tensor([1, 2, 4, 7, 0])
     >>> ops.diff(x)
     array([ 1,  2,  3, -7])
     >>> ops.diff(x, n=2)
     array([  1,   1, -10])
 
     >>> x = ops.convert_to_tensor([[1, 3, 6, 10], [0, 5, 6, 8]])
@@ -2068,15 +2081,16 @@
     def compute_output_spec(self, x, bins):
         bins_shape = bins.shape
         if len(bins_shape) > 1:
             raise ValueError(
                 f"`bins` must be a 1D array. Received: bins={bins} "
                 f"with shape bins.shape={bins_shape}"
             )
-        return KerasTensor(x.shape, dtype="int32")
+        sparse = getattr(x, "sparse", False)
+        return KerasTensor(x.shape, dtype="int32", sparse=sparse)
 
 
 @keras_export(["keras.ops.digitize", "keras.ops.numpy.digitize"])
 def digitize(x, bins):
     """Returns the indices of the bins to which each value in `x` belongs.
 
     Args:
@@ -2358,15 +2372,15 @@
             output form.
         operands: The operands to compute the Einstein sum of.
 
     Returns:
         The calculation based on the Einstein summation convention.
 
     Example:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> a = ops.arange(25).reshape(5, 5)
     >>> b = ops.arange(5)
     >>> c = ops.arange(6).reshape(2, 3)
 
     Trace of a matrix:
 
     >>> ops.einsum("ii", a)
@@ -3157,15 +3171,15 @@
         stop: The end value of the sequence, unless `endpoint` is set to
             `False`. In that case, the sequence consists of all but the last
             of `num + 1` evenly spaced samples, so that `stop` is excluded.
             Note that the step size changes when `endpoint` is `False`.
         num: Number of samples to generate. Defaults to `50`. Must be
             non-negative.
         endpoint: If `True`, `stop` is the last sample. Otherwise, it is
-            not included. Defaults to`True`.
+            not included. Defaults to `True`.
         retstep: If `True`, return `(samples, step)`, where `step` is the
             spacing between samples.
         dtype: The type of the output tensor.
         axis: The axis in the result to store the samples. Relevant only if
             start or stop are array-like. Defaults to `0`.
 
     Note:
@@ -3494,15 +3508,15 @@
         start: The starting value of the sequence.
         stop: The final value of the sequence, unless `endpoint` is `False`.
             In that case, `num + 1` values are spaced over the interval in
             log-space, of which all but the last (a sequence of length `num`)
             are returned.
         num: Number of samples to generate. Defaults to `50`.
         endpoint: If `True`, `stop` is the last sample. Otherwise, it is not
-            included. Defaults to`True`.
+            included. Defaults to `True`.
         base: The base of the log space. Defaults to `10`.
         dtype: The type of the output tensor.
         axis: The axis in the result to store the samples. Relevant only
             if start or stop are array-like.
 
     Note:
         Torch backend does not support `axis` argument.
@@ -3597,16 +3611,16 @@
     """Return the maximum of a tensor or maximum along an axis.
 
     Args:
         x: Input tensor.
         axis: Axis or axes along which to operate. By default, flattened input
             is used.
         keepdims: If this is set to `True`, the axes which are reduced are left
-            in the result as dimensions with size one. Defaults to`False`.
-        initial: The minimum value of an output element. Defaults to`None`.
+            in the result as dimensions with size one. Defaults to `False`.
+        initial: The minimum value of an output element. Defaults to `None`.
 
     Returns:
         Maximum of `x`.
     """
     if any_symbolic_tensors((x,)):
         return Max(axis=axis, keepdims=keepdims, initial=initial).symbolic_call(
             x
@@ -3740,15 +3754,15 @@
         indexing: `"xy"` or `"ij"`. "xy" is cartesian; `"ij"` is matrix
             indexing of output. Defaults to `"xy"`.
 
     Returns:
         Sequence of N tensors.
 
     Example:
-    >>> from keras import ops
+    >>> from keras.src import ops
     >>> x = ops.array([1, 2, 3])
     >>> y = ops.array([4, 5, 6])
 
     >>> grid_x, grid_y = ops.meshgrid(x, y, indexing="ij")
     >>> grid_x
     array([[1, 1, 1],
            [2, 2, 2],
@@ -3790,16 +3804,16 @@
     """Return the minimum of a tensor or minimum along an axis.
 
     Args:
         x: Input tensor.
         axis: Axis or axes along which to operate. By default, flattened input
             is used.
         keepdims: If this is set to `True`, the axes which are reduced are left
-            in the result as dimensions with size one. Defaults to`False`.
-        initial: The maximum value of an output element. Defaults to`None`.
+            in the result as dimensions with size one. Defaults to `False`.
+        initial: The maximum value of an output element. Defaults to `None`.
 
     Returns:
         Minimum of `x`.
     """
     if any_symbolic_tensors((x,)):
         return Min(axis=axis, keepdims=keepdims, initial=initial).symbolic_call(
             x
@@ -3937,34 +3951,52 @@
     """
     if any_symbolic_tensors((x,)):
         return Moveaxis(source, destination).symbolic_call(x)
     return backend.numpy.moveaxis(x, source=source, destination=destination)
 
 
 class NanToNum(Operation):
+    def __init__(self, nan=0.0, posinf=None, neginf=None):
+        super().__init__()
+        self.nan = nan
+        self.posinf = posinf
+        self.neginf = neginf
+
     def call(self, x):
-        return backend.numpy.nan_to_num(x)
+        return backend.numpy.nan_to_num(
+            x, nan=self.nan, posinf=self.posinf, neginf=self.neginf
+        )
+
+    def compute_output_spec(self, x):
+        return KerasTensor(x.shape, dtype=x.dtype)
 
 
 @keras_export(
     [
         "keras.ops.nan_to_num",
         "keras.ops.numpy.nan_to_num",
     ]
 )
-def nan_to_num(x):
+def nan_to_num(x, nan=0.0, posinf=None, neginf=None):
     """Replace NaN with zero and infinity with large finite numbers.
 
     Args:
         x: Input data.
+        nan: Optional float or int. Value to replace `NaN` entries with.
+        posinf: Optional float or int.
+            Value to replace positive infinity with.
+        neginf: Optional float or int.
+            Value to replace negative infinity with.
 
     Returns:
         `x`, with non-finite values replaced.
     """
-    return backend.numpy.nan_to_num(x)
+    if any_symbolic_tensors((x,)):
+        return NanToNum(nan=nan, posinf=posinf, neginf=neginf).symbolic_call(x)
+    return backend.numpy.nan_to_num(x, nan=nan, posinf=posinf, neginf=neginf)
 
 
 class Ndim(Operation):
     def call(self, x):
         return backend.numpy.ndim(
             x,
         )
@@ -5248,22 +5280,26 @@
     """
     if any_symbolic_tensors((x,)):
         return Trace(offset, axis1, axis2).symbolic_call(x)
     return backend.numpy.trace(x, offset=offset, axis1=axis1, axis2=axis2)
 
 
 class Tri(Operation):
-    def call(self, N, M=None, k=0, dtype=None):
-        return backend.numpy.tri(N, M=M, k=k, dtype=dtype)
+    def __init__(self, k=0, dtype=None):
+        super().__init__()
+        self.k = k
+        self.dtype = dtype or backend.floatx()
+
+    def call(self, N, M=None):
+        return backend.numpy.tri(N=N, M=M, k=self.k, dtype=self.dtype)
 
-    def compute_output_spec(self, N, M=None, k=0, dtype=None):
+    def compute_output_spec(self, N, M=None):
         if M is None:
             M = N
-        dtype = dtype or backend.floatx()
-        return KerasTensor((N, M), dtype=dtype)
+        return KerasTensor((N, M), dtype=self.dtype)
 
 
 @keras_export(["keras.ops.tri", "keras.ops.numpy.tri"])
 def tri(N, M=None, k=0, dtype=None):
     """Return a tensor with ones at and below a diagonal and zeros elsewhere.
 
     Args:
@@ -5375,14 +5411,56 @@
         Output tensor.
     """
     if any_symbolic_tensors((x1, x2)):
         return Vdot().symbolic_call(x1, x2)
     return backend.numpy.vdot(x1, x2)
 
 
+@keras_export(["keras.ops.vectorize", "keras.ops.numpy.vectorize"])
+def vectorize(pyfunc, *, excluded=None, signature=None):
+    """Turn a function into a vectorized function.
+
+    Example:
+
+    ```python
+    def myfunc(a, b):
+        return a + b
+
+    vfunc = np.vectorize(myfunc)
+    y = vfunc([1, 2, 3, 4], 2)  # Returns Tensor([3, 4, 5, 6])
+    ```
+
+    Args:
+        pyfunc: Callable of a single tensor argument.
+        excluded: Optional set of integers representing
+            positional arguments for which the function
+            will not be vectorized.
+            These will be passed directly to `pyfunc` unmodified.
+        signature: Optional generalized universal function signature,
+            e.g., `"(m,n),(n)->(m)"` for vectorized
+            matrix-vector multiplication. If provided,
+            `pyfunc` will be called with (and expected to return)
+            arrays with shapes given by the size of corresponding
+            core dimensions. By default, `pyfunc` is assumed
+            to take scalars tensors as input and output.
+
+    Returns:
+        A new function that applies `pyfunc` to every element
+        of its input along axis 0 (the batch axis).
+    """
+    if not callable(pyfunc):
+        raise ValueError(
+            "Expected argument `pyfunc` to be a callable. "
+            f"Received: pyfunc={pyfunc}"
+        )
+    return backend.numpy.vectorize(
+        pyfunc, excluded=excluded, signature=signature
+    )
+
+
 class Vstack(Operation):
     def call(self, xs):
         return backend.numpy.vstack(xs)
 
     def compute_output_spec(self, xs):
         first_shape = xs[0].shape
         total_size_on_axis = 0
@@ -6003,22 +6081,26 @@
     Returns:
         Tensor of ones with the given shape and dtype.
     """
     return backend.numpy.ones(shape, dtype=dtype)
 
 
 class Eye(Operation):
-    def call(self, N, M=None, k=0, dtype=None):
-        return backend.numpy.eye(N, M=M, k=k, dtype=dtype)
+    def __init__(self, k=0, dtype=None):
+        super().__init__()
+        self.k = k
+        self.dtype = dtype or backend.floatx()
+
+    def call(self, N, M=None):
+        return backend.numpy.eye(N, M=M, k=self.k, dtype=self.dtype)
 
-    def compute_output_spec(self, N, M=None, k=0, dtype=None):
+    def compute_output_spec(self, N, M=None):
         if M is None:
             M = N
-        dtype = dtype or backend.floatx()
-        return KerasTensor((N, M), dtype=dtype)
+        return KerasTensor((N, M), dtype=self.dtype)
 
 
 @keras_export(["keras.ops.eye", "keras.ops.numpy.eye"])
 def eye(N, M=None, k=0, dtype=None):
     """Return a 2-D tensor with ones on the diagonal and zeros elsewhere.
 
     Args:
@@ -6155,7 +6237,69 @@
     Returns:
         Output tensor, cross-correlation of `x1` and `x2`.
     """
     if any_symbolic_tensors((x1, x2)):
         return Correlate(mode=mode).symbolic_call(x1, x2)
     return backend.numpy.correlate(x1, x2, mode=mode)
 
+
+class Select(Operation):
+    def __init__(self):
+        super().__init__()
+
+    def call(self, condlist, choicelist, default=0):
+        return backend.numpy.correlate(condlist, choicelist, default)
+
+    def compute_output_spec(self, condlist, choicelist, default=0):
+        first_element = choicelist[0]
+        return KerasTensor(first_element.shape, dtype=first_element.dtype)
+
+
+@keras_export(["keras.ops.select", "keras.ops.numpy.select"])
+def select(condlist, choicelist, default=0):
+    """Return elements from `choicelist`, based on conditions in `condlist`.
+
+    Args:
+        condlist: List of boolean tensors.
+            The list of conditions which determine from which array
+            in choicelist the output elements are taken.
+            When multiple conditions are satisfied,
+            the first one encountered in condlist is used.
+        choicelist: List of tensors.
+            The list of tensors from which the output elements are taken.
+            This list has to be of the same length as `condlist`.
+        defaults: Optional scalar value.
+            The element inserted in the output
+            when all conditions evaluate to `False`.
+
+    Returns:
+        Tensor where the output at position `m` is the `m`-th element
+        of the tensor in `choicelist` where the `m`-th element of the
+        corresponding tensor in `condlist` is `True`.
+
+    Example:
+
+    ```python
+    from keras import ops
+
+    x = ops.arange(6)
+    condlist = [x<3, x>3]
+    choicelist = [x, x**2]
+    ops.select(condlist, choicelist, 42)
+    # Returns: tensor([0,  1,  2, 42, 16, 25])
+    ```
+    """
+    if not isinstance(condlist, list) or not isinstance(choicelist, list):
+        raise ValueError(
+            "condlist and choicelist must be lists. Received: "
+            f"type(condlist) = {type(condlist)}, "
+            f"type(choicelist) = {type(choicelist)}"
+        )
+    if not condlist or not choicelist:
+        raise ValueError(
+            "condlist and choicelist must not be empty. Received: "
+            f"condlist = {condlist}, "
+            f"choicelist = {choicelist}"
+        )
+    if any_symbolic_tensors(condlist + choicelist + [default]):
+        return Select().symbolic_call(condlist, choicelist, default)
+    return backend.numpy.select(condlist, choicelist, default)
```

### Comparing `keras-3.2.1/keras/src/ops/operation.py` & `keras-3.3.0/keras/src/ops/operation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 import inspect
 import textwrap
 
 from keras.src import backend
 from keras.src import dtype_policies
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.keras_tensor import any_symbolic_tensors
 from keras.src.ops.node import Node
 from keras.src.utils import python_utils
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 from keras.src.utils.naming import auto_name
 
 
 @keras_export("keras.Operation")
 class Operation:
     def __init__(self, dtype=None, name=None):
         if name is None:
             name = auto_name(self.__class__.__name__)
         if not isinstance(name, str) or "/" in name:
             raise ValueError(
                 "Argument `name` must be a string and "
                 "cannot contain character `/`. "
                 f"Received: name={name} (of type {type(name)})"
             )
-        self.dtype_policy = dtype_policies.get(dtype)
+        self._dtype_policy = dtype_policies.get(dtype)
         self.name = name
         self._inbound_nodes = []
         self._outbound_nodes = []
 
     @traceback_utils.filter_traceback
     def __call__(self, *args, **kwargs):
         if traceback_utils.is_traceback_filtering_enabled():
             # Wrap self.call to provide helpful info in case of exception
             if any_symbolic_tensors(args, kwargs):
                 call_fn = self.symbolic_call
             else:
                 if isinstance(
-                    self.dtype_policy, dtype_policies.QuantizedDTypePolicy
+                    self._dtype_policy, dtype_policies.QuantizedDTypePolicy
                 ):
                     call_fn = self.quantized_call
                 else:
                     call_fn = self.call
             call_fn = traceback_utils.inject_argument_info_in_traceback(
                 call_fn,
                 object_name=(f"{self.__class__.__name__}.call()"),
             )
             return call_fn(*args, **kwargs)
 
         # Plain flow.
         if any_symbolic_tensors(args, kwargs):
             return self.symbolic_call(*args, **kwargs)
-        if isinstance(self.dtype_policy, dtype_policies.QuantizedDTypePolicy):
+        if isinstance(self._dtype_policy, dtype_policies.QuantizedDTypePolicy):
             return self.quantized_call(*args, **kwargs)
         else:
             return self.call(*args, **kwargs)
 
     def symbolic_call(self, *args, **kwargs):
         # Perform shape/dtype inference.
         outputs = self.compute_output_spec(*args, **kwargs)
@@ -277,7 +277,14 @@
         """Can be overridden for per backend post build actions."""
         pass
 
     def _setattr_hook(self, name, value):
         """Can be overridden for per backend post build actions."""
         return name, value
 
+    def _post_track_variable(self, variable):
+        """Can be overridden for per backend post track actions."""
+        pass
+
+    def _post_untrack_variable(self, variable):
+        """Can be overridden for per backend post untrack actions."""
+        pass
```

### Comparing `keras-3.2.1/keras/src/ops/operation_utils.py` & `keras-3.3.0/keras/src/ops/operation_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import math
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common.backend_utils import canonicalize_axis
 from keras.src.backend.common.backend_utils import to_tuple_or_list
-from keras.src.utils import tree
 
 
 def broadcast_shapes(shape1, shape2):
     """Broadcast input shapes to a unified shape.
 
     Convert to list for mutability.
 
@@ -396,8 +396,7 @@
             for tensor in node.input_tensors:
                 previous_sources = get_source_inputs(tensor)
                 # Avoid input redundancy.
                 for x in previous_sources:
                     if all(x is not t for t in source_tensors):
                         source_tensors.append(x)
             return source_tensors
-
```

### Comparing `keras-3.2.1/keras/src/ops/symbolic_arguments.py` & `keras-3.3.0/keras/src/ops/symbolic_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
+from keras.src import tree
 from keras.src.backend import KerasTensor
-from keras.src.utils import tree
 
 
 class SymbolicArguments:
     def __init__(self, *args, **kwargs):
         self.args = tree.map_structure(lambda x: x, args)
         self.kwargs = tree.map_structure(lambda x: x, kwargs)
         self._flat_arguments = tree.flatten((self.args, self.kwargs))
@@ -42,8 +42,7 @@
             if isinstance(x, KerasTensor):
                 val = tensor_dict.get(id(x), None)
                 if val is not None:
                     return val
             return x
 
         return self.convert(switch_fn)
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/__init__.py` & `keras-3.3.0/keras/src/optimizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,8 +115,7 @@
         raise ImportError(
             "`keras.optimizers.legacy` is not supported in Keras 3. When using "
             "`tf.keras`, to continue using a `tf.keras.optimizers.legacy` "
             "optimizer, you can install the `tf_keras` package (Keras 2) and "
             "set the environment variable `TF_USE_LEGACY_KERAS=True` to "
             "configure TensorFlow to use `tf_keras` when accessing `tf.keras`."
         )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adadelta.py` & `keras-3.3.0/keras/src/optimizers/adadelta.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,26 +45,30 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adadelta",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             name=name,
             **kwargs,
         )
         self.rho = rho
         self.epsilon = epsilon
 
     def build(self, var_list):
@@ -129,8 +133,7 @@
         )
         return config
 
 
 Adadelta.__doc__ = Adadelta.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adafactor.py` & `keras-3.3.0/keras/src/optimizers/adafactor.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,27 +52,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adafactor",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_2_decay = beta_2_decay
         self.epsilon_1 = epsilon_1
         self.epsilon_2 = epsilon_2
         self.clip_threshold = clip_threshold
         self.relative_step = relative_step
@@ -198,8 +202,7 @@
         )
         return config
 
 
 Adafactor.__doc__ = Adafactor.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adagrad.py` & `keras-3.3.0/keras/src/optimizers/adagrad.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,26 +40,30 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adagrad",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             name=name,
             **kwargs,
         )
         self.initial_accumulator_value = initial_accumulator_value
         self.epsilon = epsilon
 
     def build(self, var_list):
@@ -105,8 +109,7 @@
         )
         return config
 
 
 Adagrad.__doc__ = Adagrad.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adam.py` & `keras-3.3.0/keras/src/optimizers/adam.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,27 +50,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adam",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
         self.amsgrad = amsgrad
 
@@ -157,8 +161,7 @@
         )
         return config
 
 
 Adam.__doc__ = Adam.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adamax.py` & `keras-3.3.0/keras/src/optimizers/adamax.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,27 +59,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adamax",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
 
     def build(self, var_list):
@@ -146,8 +150,7 @@
         )
         return config
 
 
 Adamax.__doc__ = Adamax.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/adamw.py` & `keras-3.3.0/keras/src/optimizers/adamw.py`

 * *Files 4% similar despite different names*

```diff
@@ -60,14 +60,16 @@
         amsgrad=False,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="adamw",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             beta_1=beta_1,
             beta_2=beta_2,
@@ -77,21 +79,22 @@
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
 
         if self.weight_decay is None:
             raise ValueError(
                 "Argument `weight_decay` must be a float. Received: "
                 "weight_decay=None"
             )
 
 
 AdamW.__doc__ = AdamW.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/base_optimizer.py` & `keras-3.3.0/keras/src/optimizers/base_optimizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import re
 import warnings
 
-import numpy as np
-
 from keras.src import backend
 from keras.src import initializers
 from keras.src import ops
 from keras.src.optimizers.schedules import learning_rate_schedule
 from keras.src.saving import serialization_lib
 from keras.src.utils import tracking
 from keras.src.utils.naming import auto_name
@@ -207,15 +205,19 @@
         """Add an all-zeros variable with the shape and dtype of a reference
         variable.
         """
         name = name or "var"
         if hasattr(reference_variable, "path"):
             name = reference_variable.path.replace("/", "_") + "_" + name
         else:
-            name = str(reference_variable.name).replace(":", "_") + "_" + name
+            name = (
+                str(reference_variable.name).replace("/", "_").replace(":", "_")
+                + "_"
+                + name
+            )
         return self.add_variable(
             shape=reference_variable.shape,
             initializer=initializer,
             dtype=reference_variable.dtype,
             name=name,
         )
 
@@ -316,14 +318,22 @@
             if not self.built:
                 with backend.name_scope(self.name, caller=self):
                     self.build(trainable_variables)
                 self.built = True
             self._check_variables_are_known(trainable_variables)
 
         with backend.name_scope(self.name, caller=self):
+            # Overwrite targeted variables directly with their gradients if
+            # their `overwrite_with_gradient` is set.
+            grads, trainable_variables = (
+                self._overwrite_variables_directly_with_gradients(
+                    grads, trainable_variables
+                )
+            )
+
             # Filter empty gradients.
             grads, trainable_variables = self._filter_empty_gradients(
                 grads, trainable_variables
             )
             if len(list(grads)) == 0:
                 return
 
@@ -359,35 +369,39 @@
         - Update gradient accumulators, if gradient accumulation is configured.
         - Update the iteration counter.
         """
         if self.gradient_accumulation_steps:
             is_update_step = (
                 self.iterations + 1
             ) % self.gradient_accumulation_steps == 0
+            # `trainable_variables` might have been filtered in previous
+            # processing steps, so we need to ensure the correct mapping between
+            # `self._accumulated_gradients` and `trainable_variables`
+            acc_grads = [
+                self._accumulated_gradients[self._get_variable_index(v)]
+                for v in trainable_variables
+            ]
 
-            def _update_step_fn(self, grads, trainable_variables):
+            def _update_step_fn(grads, trainable_variables):
                 # Run update step with accumulated grads + reset accumulators
                 steps = self.gradient_accumulation_steps
                 grads = [
-                    (grads[i] + self._accumulated_gradients[i]) / steps
-                    for i in range(len(grads))
+                    (g + acc_g) / steps for g, acc_g in zip(grads, acc_grads)
                 ]
                 self._backend_update_step(
                     grads, trainable_variables, self.learning_rate
                 )
                 self._backend_reset_gradient_accumulators()
 
-            def _grad_accumulation_fn(self, grads):
-                # Update gradient accumulators
-                self._backend_increment_gradient_accumulators(grads)
-
             ops.cond(
                 is_update_step,
-                lambda: _update_step_fn(self, grads, trainable_variables),
-                lambda: _grad_accumulation_fn(self, grads),
+                lambda: _update_step_fn(grads, trainable_variables),
+                lambda: self._backend_increment_gradient_accumulators(
+                    grads, acc_grads
+                ),
             )
         else:
             # Run udpate step.
             self._backend_update_step(
                 grads, trainable_variables, self.learning_rate
             )
 
@@ -418,22 +432,19 @@
         by TF to support tf.distribute.
         """
         for grad, var in zip(grads, trainable_variables):
             self.update_step(grad, var, learning_rate)
 
     def _backend_reset_gradient_accumulators(self):
         for g_acc in self._accumulated_gradients:
-            g_acc.assign(np.zeros(g_acc.shape, dtype=g_acc.dtype))
+            g_acc.assign(ops.zeros(g_acc.shape, dtype=g_acc.dtype))
 
-    def _backend_increment_gradient_accumulators(self, grads):
-        new_g_accs = [
-            (grads[i] + self._accumulated_gradients[i])
-            for i in range(len(grads))
-        ]
-        for n_g_acc, g_acc in zip(new_g_accs, self._accumulated_gradients):
+    def _backend_increment_gradient_accumulators(self, grads, acc_grads):
+        new_g_accs = [(g + acc_g) for g, acc_g in zip(grads, acc_grads)]
+        for n_g_acc, g_acc in zip(new_g_accs, acc_grads):
             g_acc.assign(n_g_acc)
 
     def stateless_apply(self, optimizer_variables, grads, trainable_variables):
         self._check_super_called()
 
         if not self.built:
             raise ValueError(
@@ -497,14 +508,18 @@
 
     @property
     def learning_rate(self):
         return self._get_current_learning_rate()
 
     @learning_rate.setter
     def learning_rate(self, learning_rate):
+        if isinstance(self._learning_rate, backend.Variable):
+            prev_lr_var = self._learning_rate
+        else:
+            prev_lr_var = None
         if isinstance(
             learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             self._learning_rate = learning_rate
         elif callable(learning_rate):
             self._learning_rate = learning_rate
         else:
@@ -515,14 +530,19 @@
                     "This optimizer was created with a `LearningRateSchedule`"
                     " object as its `learning_rate` constructor argument, "
                     "hence its learning rate is not settable. If you need the"
                     " learning rate to be settable, you should instantiate "
                     "the optimizer with a float `learning_rate` argument."
                 )
             self._learning_rate.assign(learning_rate)
+        if prev_lr_var is not None and not isinstance(
+            self._learning_rate, backend.Variable
+        ):
+            # Untrack learning rate variable
+            self._untrack_variable(prev_lr_var)
 
     def set_weights(self, weights):
         """Set the weights of the optimizer."""
         if not self.built:
             raise ValueError(
                 "You are calling `set_weights()` on an optimizer that has not "
                 "yet been built. Please call "
@@ -563,17 +583,72 @@
 
     def _get_current_learning_rate(self):
         if isinstance(
             self._learning_rate, learning_rate_schedule.LearningRateSchedule
         ):
             return self._learning_rate(self.iterations)
         elif callable(self._learning_rate):
-            return self._learning_rate(self.iterations)
+            return self._learning_rate()
         return self._learning_rate
 
+    def _overwrite_variables_directly_with_gradients(self, grads, vars):
+        """Overwrite the variables directly by their gradients.
+
+        This method is designed for a special case where we want to overwrite
+        the variable directly with its computed gradient. For example, in float8
+        training, new `scale` and `amax_history` are computed as gradients, and
+        we want to overwrite them directly instead of following the typical
+        procedure such as gradient descent with a learning rate, gradient
+        clipping and weight decaying.
+
+        After the update, the processed pairs will be filtered out.
+        """
+        # Shortcut for `tf.Variable` because it doesn't have a
+        # `overwrite_with_gradient` attr
+        if not hasattr(vars[0], "overwrite_with_gradient"):
+            return grads, vars
+
+        # Shallow copies
+        filtered_grads = list(grads)
+        filtered_vars = list(vars)
+
+        # Iterate from right to left for safe popping
+        for i in range(len(filtered_grads) - 1, -1, -1):
+            g, v = filtered_grads[i], filtered_vars[i]
+            if v.overwrite_with_gradient:
+                if self.gradient_accumulation_steps:
+                    # Utilize a stateless manner for JAX compatibility
+                    steps = self.gradient_accumulation_steps
+                    is_update_step = (self.iterations + 1) % steps == 0
+                    acc_g = self._accumulated_gradients[
+                        self._get_variable_index(v)
+                    ]
+                    # `ops.maximum` is utilized for gradient accumulation for
+                    # `overwrite_with_gradient=True` variables
+                    new_g_acc = ops.cond(
+                        is_update_step,
+                        lambda: ops.zeros(g.shape, dtype=g.dtype),
+                        lambda: ops.maximum(g, acc_g),
+                    )
+                    new_g = ops.cond(
+                        is_update_step,
+                        lambda: ops.maximum(g, acc_g),
+                        lambda: g,
+                    )
+                    new_v = ops.cond(
+                        is_update_step, lambda: new_g, lambda: v.value
+                    )
+                    v.assign(new_v)
+                    acc_g.assign(new_g_acc)
+                else:
+                    v.assign(g)
+                filtered_grads.pop(i)
+                filtered_vars.pop(i)
+        return filtered_grads, filtered_vars
+
     def _filter_empty_gradients(self, grads, vars):
         filtered_grads = list(grads)
         filtered_vars = list(vars)
         missing_grad_vars = []
 
         # Iterate from right to left for safe popping
         for i in range(len(filtered_grads) - 1, -1, -1):
@@ -828,14 +903,21 @@
         l2norm = ops.where(pred, ops.sqrt(l2sum_safe), l2sum)
         intermediate = ops.multiply(values, self.clipnorm)
         values_clip = ops.convert_to_tensor(intermediate) / ops.maximum(
             l2norm, self.clipnorm
         )
         return values_clip
 
+    def _untrack_variable(self, variable):
+        previous_lock_state = self._tracker.locked
+        self._tracker.unlock()
+        self._tracker.untrack(variable)
+        if previous_lock_state is True:
+            self._tracker.lock()
+
 
 base_optimizer_keyword_args = """name: String. The name to use
             for momentum accumulator weights created by
             the optimizer.
         weight_decay: Float. If set, weight decay is applied.
         clipnorm: Float. If set, the gradient of each weight is individually
             clipped so that its norm is no higher than this value.
@@ -895,8 +977,7 @@
     use_norm = global_norm(value_list)
     # Calculate L2-norm, clip elements by ratio of clip_norm to L2-norm
     scale_for_finite = clip_norm * ops.minimum(1.0 / use_norm, 1.0 / clip_norm)
     # If use_norm is any finite number, this is a no-op. For inf/-inf/NaN,
     # this will make scale NaN.
     scale = scale_for_finite + (use_norm - use_norm)
     return [v * scale if v is not None else v for v in value_list]
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/ftrl.py` & `keras-3.3.0/keras/src/optimizers/ftrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,27 +87,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="ftrl",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
 
         if initial_accumulator_value < 0.0:
             raise ValueError(
                 "`initial_accumulator_value` needs to be positive or zero. "
                 "Received: initial_accumulator_value="
@@ -239,8 +243,7 @@
         )
         return config
 
 
 Ftrl.__doc__ = Ftrl.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/lion.py` & `keras-3.3.0/keras/src/optimizers/lion.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,27 +49,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="lion",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         if beta_1 <= 0 or beta_1 > 1:
             raise ValueError(
                 "Argument `beta_1` must be in the [0, 1] range. Otherwise, the "
@@ -132,8 +136,7 @@
         )
         return config
 
 
 Lion.__doc__ = Lion.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/loss_scale_optimizer.py` & `keras-3.3.0/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,8 +290,7 @@
         )
         return cls(inner_optimizer, **config)
 
 
 LossScaleOptimizer.__doc__ = LossScaleOptimizer.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/nadam.py` & `keras-3.3.0/keras/src/optimizers/nadam.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="nadam",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
         self.epsilon = epsilon
 
     def build(self, var_list):
@@ -164,8 +168,7 @@
         )
         return config
 
 
 Nadam.__doc__ = Nadam.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/optimizer.py` & `keras-3.3.0/keras/src/optimizers/optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,7 @@
 
 @keras_export(["keras.Optimizer", "keras.optimizers.Optimizer"])
 class Optimizer(BackendOptimizer, base_optimizer.BaseOptimizer):
     pass
 
 
 base_optimizer_keyword_args = base_optimizer.base_optimizer_keyword_args
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/rmsprop.py` & `keras-3.3.0/keras/src/optimizers/rmsprop.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,27 +59,31 @@
         centered=False,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
-        ema_overwrite_frequency=100,
+        ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="rmsprop",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             name=name,
             **kwargs,
         )
         self.rho = rho
         self.momentum = momentum
         self.epsilon = epsilon
         self.centered = centered
@@ -170,8 +174,7 @@
         )
         return config
 
 
 RMSprop.__doc__ = RMSprop.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/schedules/__init__.py` & `keras-3.3.0/keras/src/optimizers/schedules/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 from keras.src.optimizers.schedules.learning_rate_schedule import CosineDecay
 from keras.src.optimizers.schedules.learning_rate_schedule import (
     CosineDecayRestarts,
 )
-from keras.src.optimizers.schedules.learning_rate_schedule import ExponentialDecay
-from keras.src.optimizers.schedules.learning_rate_schedule import InverseTimeDecay
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    ExponentialDecay,
+)
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    InverseTimeDecay,
+)
 from keras.src.optimizers.schedules.learning_rate_schedule import (
     PiecewiseConstantDecay,
 )
-from keras.src.optimizers.schedules.learning_rate_schedule import PolynomialDecay
-
+from keras.src.optimizers.schedules.learning_rate_schedule import (
+    PolynomialDecay,
+)
```

### Comparing `keras-3.2.1/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files 0% similar despite different names*

```diff
@@ -963,8 +963,7 @@
     """
     return serialization_lib.deserialize_keras_object(
         config,
         module_objects=globals(),
         custom_objects=custom_objects,
         printable_module_name="decay",
     )
-
```

### Comparing `keras-3.2.1/keras/src/optimizers/sgd.py` & `keras-3.3.0/keras/src/optimizers/sgd.py`

 * *Files 10% similar despite different names*

```diff
@@ -48,27 +48,31 @@
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
         name="SGD",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         if not isinstance(momentum, float) or momentum < 0 or momentum > 1:
             raise ValueError("`momentum` must be a float between [0, 1].")
         self.momentum = momentum
         self.nesterov = nesterov
 
@@ -133,8 +137,7 @@
         )
         return config
 
 
 SGD.__doc__ = SGD.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
-
```

### Comparing `keras-3.2.1/keras/src/quantizers/__init__.py` & `keras-3.3.0/keras/src/quantizers/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import inspect
 
 from keras.src.api_export import keras_export
 from keras.src.quantizers.quantizers import AbsMaxQuantizer
 from keras.src.quantizers.quantizers import Quantizer
 from keras.src.quantizers.quantizers import abs_max_quantize
+from keras.src.quantizers.quantizers import compute_float8_amax_history
+from keras.src.quantizers.quantizers import compute_float8_scale
+from keras.src.quantizers.quantizers import quantize_and_dequantize
 from keras.src.saving import serialization_lib
 from keras.src.utils.naming import to_snake_case
 
 ALL_OBJECTS = {Quantizer, AbsMaxQuantizer}
 ALL_OBJECTS_DICT = {cls.__name__: cls for cls in ALL_OBJECTS}
 ALL_OBJECTS_DICT.update(
     {to_snake_case(cls.__name__): cls for cls in ALL_OBJECTS}
@@ -45,8 +48,7 @@
         if inspect.isclass(obj):
             obj = obj(kwargs)
         return obj
     else:
         raise ValueError(
             f"Could not interpret quantizer identifier: {identifier}"
         )
-
```

### Comparing `keras-3.2.1/keras/src/random/random.py` & `keras-3.3.0/keras/src/random/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,8 +294,7 @@
             across multiple calls. To get different random values
             across multiple calls, use as seed an instance
             of `keras.random.SeedGenerator`.
     """
     return backend.random.beta(
         shape=shape, alpha=alpha, beta=beta, dtype=dtype, seed=seed
     )
-
```

### Comparing `keras-3.2.1/keras/src/random/seed_generator.py` & `keras-3.3.0/keras/src/random/seed_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import numpy as np
 
 from keras.src import backend
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
 from keras.src.utils import jax_utils
+from keras.src.utils.naming import auto_name
 
 
 @keras_export("keras.random.SeedGenerator")
 class SeedGenerator:
     """Generates variable seeds upon each call to a RNG-using function.
 
     In Keras, all RNG-using methods (such as `keras.random.normal()`)
@@ -40,15 +41,19 @@
                 return keras.random.dropout(
                     x, rate=0.5, seed=self.seed_generator
                 )
             return x
     ```
     """
 
-    def __init__(self, seed=None, **kwargs):
+    def __init__(self, seed=None, name=None, **kwargs):
+        if name is None:
+            name = auto_name(self.__class__.__name__)
+        self.name = name
+
         custom_backend = kwargs.pop("backend", None)
         if kwargs:
             raise ValueError(f"Unrecognized keyword arguments: {kwargs}")
         if custom_backend is not None:
             self.backend = custom_backend
         else:
             self.backend = backend
@@ -62,21 +67,22 @@
                 "Argument `seed` must be an integer. " f"Received: seed={seed}"
             )
 
         def seed_initializer(*args, **kwargs):
             dtype = kwargs.get("dtype", None)
             return self.backend.convert_to_tensor([seed, 0], dtype=dtype)
 
-        self.state = self.backend.Variable(
-            seed_initializer,
-            shape=(2,),
-            dtype="uint32",
-            trainable=False,
-            name="seed_generator_state",
-        )
+        with backend.name_scope(self.name, caller=self):
+            self.state = self.backend.Variable(
+                seed_initializer,
+                shape=(2,),
+                dtype="uint32",
+                trainable=False,
+                name="seed_generator_state",
+            )
 
     def next(self, ordered=True):
         seed_state = self.state
         # Use * 1 to create a copy
         new_seed_value = seed_state.value * 1
         if ordered:
             increment = self.backend.convert_to_tensor(
@@ -135,8 +141,7 @@
     elif seed is None:
         return global_seed_generator().next(ordered=False)
     raise ValueError(
         "Argument `seed` must be either an integer "
         "or an instance of `SeedGenerator`. "
         f"Received: seed={seed} (of type {type(seed)})"
     )
-
```

### Comparing `keras-3.2.1/keras/src/regularizers/__init__.py` & `keras-3.3.0/keras/src/regularizers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,7 @@
         if inspect.isclass(obj):
             obj = obj()
         return obj
     else:
         raise ValueError(
             f"Could not interpret regularizer identifier: {identifier}"
         )
-
```

### Comparing `keras-3.2.1/keras/src/regularizers/regularizers.py` & `keras-3.3.0/keras/src/regularizers/regularizers.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,8 +346,7 @@
         or value < 0
     ):
         raise ValueError(
             f"Invalid value for argument {name}: expected a non-negative float."
             f"Received: {name}={value}"
         )
     return float(value)
-
```

### Comparing `keras-3.2.1/keras/src/saving/__init__.py` & `keras-3.3.0/keras/src/saving/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,8 +3,7 @@
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.saving_api import load_model
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-
```

### Comparing `keras-3.2.1/keras/src/saving/object_registration.py` & `keras-3.3.0/keras/src/saving/object_registration.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,8 +224,7 @@
     elif name in GLOBAL_CUSTOM_OBJECTS:
         return GLOBAL_CUSTOM_OBJECTS[name]
     elif custom_objects and name in custom_objects:
         return custom_objects[name]
     elif module_objects and name in module_objects:
         return module_objects[name]
     return None
-
```

### Comparing `keras-3.2.1/keras/src/saving/saving_api.py` & `keras-3.3.0/keras/src/saving/saving_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,17 @@
         return saving_lib.load_model(
             filepath,
             custom_objects=custom_objects,
             compile=compile,
             safe_mode=safe_mode,
         )
     if str(filepath).endswith((".h5", ".hdf5")):
-        return legacy_h5_format.load_model_from_hdf5(filepath)
+        return legacy_h5_format.load_model_from_hdf5(
+            filepath, custom_objects=custom_objects, compile=compile
+        )
     elif str(filepath).endswith(".keras"):
         raise ValueError(
             f"File not found: filepath={filepath}. "
             "Please ensure the file is an accessible `.keras` "
             "zip file."
         )
     else:
@@ -258,8 +260,7 @@
                 legacy_h5_format.load_weights_from_hdf5_group(f, model)
     else:
         raise ValueError(
             f"File format not supported: filepath={filepath}. "
             "Keras 3 only supports V3 `.keras` and `.weights.h5` "
             "files, or legacy V1/V2 `.h5` files."
         )
-
```

### Comparing `keras-3.2.1/keras/src/saving/saving_lib.py` & `keras-3.3.0/keras/src/saving/saving_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -806,8 +806,7 @@
         (
             Layer,
             Optimizer,
             Metric,
             Loss,
         ),
     )
-
```

### Comparing `keras-3.2.1/keras/src/saving/serialization_lib.py` & `keras-3.3.0/keras/src/saving/serialization_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,19 @@
             "class_name": "__slice__",
             "config": {
                 "start": serialize_keras_object(obj.start),
                 "stop": serialize_keras_object(obj.stop),
                 "step": serialize_keras_object(obj.step),
             },
         }
+    # Ellipsis is an instance, and ellipsis class is not in global scope.
+    # checking equality also fails elsewhere in the library, so we have
+    # to dynamically get the type.
+    if isinstance(obj, type(Ellipsis)):
+        return {"class_name": "__ellipsis__", "config": {}}
     if isinstance(obj, backend.KerasTensor):
         history = getattr(obj, "_keras_history", None)
         if history:
             history = list(history)
             history[0] = history[0].name
         return {
             "class_name": "__keras_tensor__",
@@ -609,14 +614,16 @@
         return backend.convert_to_tensor(
             inner_config["value"], dtype=inner_config["dtype"]
         )
     if class_name == "__numpy__":
         return np.array(inner_config["value"], dtype=inner_config["dtype"])
     if config["class_name"] == "__bytes__":
         return inner_config["value"].encode("utf-8")
+    if config["class_name"] == "__ellipsis__":
+        return Ellipsis
     if config["class_name"] == "__slice__":
         return slice(
             deserialize_keras_object(
                 inner_config["start"],
                 custom_objects=custom_objects,
                 safe_mode=safe_mode,
             ),
@@ -804,8 +811,7 @@
 
     raise TypeError(
         f"Could not locate {obj_type} '{name}'. "
         "Make sure custom classes are decorated with "
         "`@keras.saving.register_keras_serializable()`. "
         f"Full object config: {full_config}"
     )
-
```

### Comparing `keras-3.2.1/keras/src/testing/test_case.py` & `keras-3.3.0/keras/src/testing/test_case.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 import unittest
 
 import numpy as np
 
 from keras.src import backend
 from keras.src import distribution
 from keras.src import ops
+from keras.src import tree
 from keras.src import utils
 from keras.src.backend.common import is_float_dtype
 from keras.src.backend.common import standardize_dtype
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import KerasTensor
 from keras.src.models import Model
 from keras.src.utils import traceback_utils
-from keras.src.utils import tree
 
 
 class TestCase(unittest.TestCase):
     maxDiff = None
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def setUp(self):
         # clear global state so that test cases are independent
         # required for the jit enabled torch tests since dynamo has
         # a global cache for guards, compiled fn, etc
-        clear_session()
+        clear_session(free_memory=False)
         if traceback_utils.is_traceback_filtering_enabled():
             traceback_utils.disable_traceback_filtering()
 
     def get_temp_dir(self):
         temp_dir = tempfile.mkdtemp()
         self.addCleanup(lambda: shutil.rmtree(temp_dir))
         return temp_dir
@@ -287,17 +287,30 @@
                 self.assertLen(
                     layer.non_trainable_variables,
                     expected_num_non_trainable_variables,
                     msg="Unexpected number of non_trainable_variables",
                 )
             if expected_num_seed_generators is not None:
                 self.assertLen(
-                    layer._seed_generators,
+                    get_seed_generators(layer),
                     expected_num_seed_generators,
-                    msg="Unexpected number of _seed_generators",
+                    msg="Unexpected number of seed_generators",
+                )
+            if (
+                backend.backend() == "torch"
+                and expected_num_trainable_weights is not None
+                and expected_num_non_trainable_weights is not None
+                and expected_num_seed_generators is not None
+            ):
+                self.assertLen(
+                    layer.torch_params,
+                    expected_num_trainable_weights
+                    + expected_num_non_trainable_weights
+                    + expected_num_seed_generators,
+                    msg="Unexpected number of torch_params",
                 )
 
         def run_output_asserts(layer, output, eager=False):
             if expected_output_shape is not None:
                 if isinstance(expected_output_shape, tuple) and is_shape_tuple(
                     expected_output_shape[0]
                 ):
@@ -659,7 +672,18 @@
             for k, v in shape.items()
         }
     else:
         raise ValueError(
             f"Cannot map function to unknown objects {shape} and {dtype}"
         )
 
+
+def get_seed_generators(layer):
+    """Get a List of all seed generators in the layer recursively."""
+    seed_generators = []
+    seen_ids = set()
+    for sublayer in layer._flatten_layers(True, True):
+        for sg in sublayer._seed_generators:
+            if id(sg) not in seen_ids:
+                seed_generators.append(sg)
+                seen_ids.add(id(sg))
+    return seed_generators
```

### Comparing `keras-3.2.1/keras/src/testing/test_utils.py` & `keras-3.3.0/keras/src/testing/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,8 +157,7 @@
                 new_test.update(test_dict)
                 new_test["testcase_name"] = testcase_name
                 new_tests.append(new_test)
         # Overwrite the list of tests with the product obtained so far
         tests = new_tests
 
     return tests
-
```

### Comparing `keras-3.2.1/keras/src/trainers/compile_utils.py` & `keras-3.3.0/keras/src/trainers/compile_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from keras.src import backend
 from keras.src import losses as losses_module
 from keras.src import metrics as metrics_module
 from keras.src import ops
-from keras.src.utils import tree
+from keras.src import tree
 from keras.src.utils.naming import get_object_name
 
 
 class MetricsList(metrics_module.Metric):
     def __init__(self, metrics, name="metrics_list", output_name=None):
         super().__init__(name=name)
         self.metrics = metrics
@@ -409,18 +409,22 @@
     def __init__(
         self,
         loss,
         loss_weights=None,
         reduction="sum_over_batch_size",
         output_names=None,
     ):
-        if loss_weights and not isinstance(loss_weights, (list, tuple, dict)):
+        if loss_weights and not isinstance(
+            loss_weights, (list, tuple, dict, float)
+        ):
             raise ValueError(
-                "Expected `loss_weights` argument to be a list, tuple, or "
-                f"dict. Received instead: loss_weights={loss_weights} "
+                "Expected `loss_weights` argument to be a float "
+                "(single output case) or a list, tuple, or "
+                "dict (multiple output case). "
+                f"Received instead: loss_weights={loss_weights} "
                 f"of type {type(loss_weights)}"
             )
         self._user_loss = loss
         self._user_loss_weights = loss_weights
         self.built = False
         self.output_names = output_names
         super().__init__(name="compile_loss", reduction=reduction)
@@ -648,8 +652,7 @@
 
     def get_config(self):
         raise NotImplementedError
 
     @classmethod
     def from_config(cls, config):
         raise NotImplementedError
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/__init__.py` & `keras-3.3.0/keras/src/trainers/data_adapters/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,8 +136,7 @@
     if hasattr(x, "__class__"):
         for parent in x.__class__.__mro__:
             if parent.__name__ == "DataLoader" and "torch.utils.data" in str(
                 parent.__module__
             ):
                 return True
     return False
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import functools
 import math
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import array_slicing
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class ArrayDataAdapter(DataAdapter):
     """Adapter for array-like objects, e.g. TF/JAX Tensors, NumPy arrays."""
 
     def __init__(
         self,
@@ -370,8 +370,7 @@
         `True` if `arrays` can be handled by `ArrayDataAdapter`, `False`
         otherwise.
     """
 
     return all(
         tree.flatten(tree.map_structure(array_slicing.can_slice_array, arrays))
     )
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/array_slicing.py` & `keras-3.3.0/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import collections
 import math
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
-from keras.src.utils import tree
 
 try:
     import pandas
 except ImportError:
     pandas = None
 
 
@@ -171,17 +171,17 @@
 
     @classmethod
     def convert_to_jax_compatible(cls, x):
         return data_adapter_utils.tf_sparse_to_jax_sparse(x)
 
     @classmethod
     def convert_to_torch_compatible(cls, x):
-        from keras.src.utils.module_utils import tensorflow as tf
+        from keras.src.backend.tensorflow import sparse as tf_sparse
 
-        return tf.sparse.to_dense(x)
+        return tf_sparse.sparse_to_dense(x)
 
 
 class JaxSliceable(Sliceable):
     def __getitem__(self, indices):
         return self.array[indices, ...]
 
     @classmethod
@@ -506,8 +506,7 @@
     train_arrays = tree.map_structure(
         lambda x: _split(x, start=0, end=split_at), sliceables
     )
     val_arrays = tree.map_structure(
         lambda x: _split(x, start=split_at, end=batch_dim), sliceables
     )
     return train_arrays, val_arrays
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/data_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,7 @@
         Will return None if has_partial_batch is False or batch_size is None.
         """
         raise NotImplementedError
 
     def on_epoch_end(self):
         """A hook called after each epoch."""
         pass
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-3.3.0/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
-from keras.src.utils import tree
 
 NUM_BATCHES_FOR_TENSOR_SPEC = 2
 
 
 @keras_export("keras.utils.unpack_x_y_sample_weight")
 def unpack_x_y_sample_weight(data):
     """Unpacks user-provided data tuple.
@@ -302,8 +302,7 @@
     return jax_sparse.BCOO((values, indices), shape=x.shape)
 
 
 def jax_sparse_to_tf_sparse(x):
     from keras.src.utils.module_utils import tensorflow as tf
 
     return tf.SparseTensor(x.indices, x.data, x.shape)
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import itertools
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class GeneratorDataAdapter(DataAdapter):
     """Adapter for Python generators."""
 
     def __init__(self, generator):
         first_batches, generator = peek_and_restore(generator)
@@ -79,8 +79,7 @@
 def peek_and_restore(generator):
     batches = list(
         itertools.islice(
             generator, data_adapter_utils.NUM_BATCHES_FOR_TENSOR_SPEC
         )
     )
     return batches, itertools.chain(batches, generator)
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -591,8 +591,7 @@
 
     if random_seed is not None:
         np.random.seed(random_seed + worker_proc.ident)
 
     if id_queue is not None:
         # If a worker dies during init, the pool will just create a replacement.
         id_queue.put(worker_proc.ident, block=True, timeout=0.1)
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class TFDatasetAdapter(DataAdapter):
     """Adapter that handles `tf.data.Dataset`."""
 
     def __init__(self, dataset, class_weight=None, distribution=None):
         """Iniitialize the TFDatasetAdapter.
@@ -140,8 +140,7 @@
             # Special casing for rank 1, where we can guarantee sparse encoding.
             y_classes = tf.cast(tf.round(y), tf.int32)
 
         cw = tf.gather(class_weight_tensor, y_classes)
         return x, y, cw
 
     return class_weights_map_fn
-
```

### Comparing `keras-3.2.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import itertools
 
 import numpy as np
 
+from keras.src import tree
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.trainers.data_adapters.data_adapter import DataAdapter
-from keras.src.utils import tree
 
 
 class TorchDataLoaderAdapter(DataAdapter):
     """Adapter that handles `torch.utils.data.DataLoader`."""
 
     def __init__(self, dataloader):
         import torch
@@ -78,8 +78,7 @@
             return self._partial_batch_size > 0
         else:
             return None
 
     @property
     def partial_batch_size(self):
         return self._partial_batch_size
-
```

### Comparing `keras-3.2.1/keras/src/trainers/epoch_iterator.py` & `keras-3.3.0/keras/src/trainers/epoch_iterator.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,8 +122,7 @@
     @property
     def num_batches(self):
         if self.steps_per_epoch:
             return self.steps_per_epoch
         # Either copied from the data_adapter, or
         # inferred at the end of an iteration.
         return self._num_batches
-
```

### Comparing `keras-3.2.1/keras/src/trainers/trainer.py` & `keras-3.3.0/keras/src/trainers/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import platform
 import warnings
 
 from keras.src import backend
 from keras.src import metrics as metrics_module
 from keras.src import ops
 from keras.src import optimizers
+from keras.src import tree
 from keras.src.optimizers.loss_scale_optimizer import LossScaleOptimizer
 from keras.src.saving import serialization_lib
 from keras.src.trainers.compile_utils import CompileLoss
 from keras.src.trainers.compile_utils import CompileMetrics
 from keras.src.trainers.data_adapters import data_adapter_utils
 from keras.src.utils import traceback_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 
 
 class Trainer:
     def __init__(self):
         self._lock = False
         self._run_eagerly = False
         self._jit_compile = None
@@ -238,30 +238,23 @@
     @run_eagerly.setter
     def run_eagerly(self, value):
         self._run_eagerly = value
 
     @property
     def metrics(self):
         metrics = [self._loss_tracker] if self.compiled else []
-        metrics.extend(self._metrics[:])
+        metrics.extend(super().metrics)
         if self.compiled and self._compile_metrics is not None:
             metrics += [self._compile_metrics]
         return metrics
 
     @property
     def metrics_names(self):
         return [m.name for m in self.metrics]
 
-    @property
-    def metrics_variables(self):
-        vars = []
-        for metric in self.metrics:
-            vars.extend(metric.variables)
-        return vars
-
     def reset_metrics(self):
         for m in self.metrics:
             m.reset_state()
 
     def compute_loss(
         self,
         x=None,
@@ -320,15 +313,15 @@
         del x  # The default implementation does not use `x`.
         losses = []
         if self._compile_loss is not None:
             loss = self._compile_loss(y, y_pred, sample_weight)
             if loss is not None:
                 losses.append(loss)
         for loss in self.losses:
-            losses.append(ops.cast(loss, dtype=backend.floatx()))
+            losses.append(ops.sum(ops.cast(loss, dtype=backend.floatx())))
         if backend.backend() != "jax" and len(losses) == 0:
             raise ValueError(
                 "No loss to compute. Provide a `loss` argument in `compile()`."
             )
         if len(losses) == 1:
             total_loss = losses[0]
         elif len(losses) == 0:
@@ -902,14 +895,45 @@
                 try:
                     value = float(value)
                 except:
                     pass
                 result[key] = value
         return result
 
+    def _get_metrics_result_or_logs(self, logs):
+        """Returns model metrics as a dict if the keys match with input logs.
+
+        When the training / evalution is performed with an asynchronous steps,
+        the last scheduled `train / test_step` may not give the latest metrics
+        because it is not guaranteed to be executed the last. This method gets
+        metrics from the model directly instead of relying on the return from
+        last step function.
+
+        When the user has custom train / test step functions, the metrics
+        returned may be different from `Model.metrics`. In those instances,
+        this function will be no-op and return the logs passed in.
+
+        Args:
+            logs: A `dict` of metrics returned by train / test step function.
+
+        Returns:
+            A `dict` containing values of the metrics listed in `self.metrics`
+            when logs and model metrics keys match. Otherwise it returns input
+            `logs`.
+        """
+        metric_logs = self.get_metrics_result()
+        # Verify that train / test step logs passed and metric logs have
+        # matching keys. It could be different when using custom step functions,
+        # in which case we return the logs from the last step.
+        if isinstance(logs, dict) and set(logs.keys()) == set(
+            metric_logs.keys()
+        ):
+            return metric_logs
+        return logs
+
     def _flatten_metrics_in_order(self, logs):
         """Turns `logs` dict into a list as per key order of `metrics_names`."""
         metric_names = []
         for metric in self.metrics:
             if isinstance(metric, CompileMetrics):
                 metric_names += [
                     sub_metric.name for sub_metric in metric.metrics
@@ -1006,8 +1030,7 @@
 
             if tf.config.list_physical_devices("GPU"):
                 return False
     # XLA not supported by some layers
     if all(x.supports_jit for x in model._flatten_layers()):
         return True
     return False
-
```

### Comparing `keras-3.2.1/keras/src/utils/argument_validation.py` & `keras-3.3.0/keras/src/utils/argument_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,7 @@
     elif isinstance(value, str) and value in allowable_strings:
         return
     raise ValueError(
         f"Unknown value for `{arg_name}` argument of {caller_name}. "
         f"Allowed values are: {allowable_strings}. Received: "
         f"{arg_name}={value}"
     )
-
```

### Comparing `keras-3.2.1/keras/src/utils/audio_dataset_utils.py` & `keras-3.3.0/keras/src/utils/audio_dataset_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,14 +170,18 @@
 
     dataset_utils.check_validation_split_arg(
         validation_split, subset, shuffle, seed
     )
 
     if seed is None:
         seed = np.random.randint(1e6)
+    if batch_size is not None:
+        shuffle_buffer_size = batch_size * 8
+    else:
+        shuffle_buffer_size = 1024
 
     file_paths, labels, class_names = dataset_utils.index_directory(
         directory,
         labels,
         formats=ALLOWED_FORMATS,
         class_names=class_names,
         shuffle=shuffle,
@@ -199,29 +203,28 @@
             validation_split=validation_split,
             directory=directory,
             label_mode=label_mode,
             class_names=class_names,
             sampling_rate=sampling_rate,
             output_sequence_length=output_sequence_length,
             ragged=ragged,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
         train_dataset = prepare_dataset(
             dataset=train_dataset,
             batch_size=batch_size,
-            shuffle=shuffle,
-            seed=seed,
             class_names=class_names,
             output_sequence_length=output_sequence_length,
             ragged=ragged,
         )
         val_dataset = prepare_dataset(
             dataset=val_dataset,
             batch_size=batch_size,
-            shuffle=False,
-            seed=seed,
             class_names=class_names,
             output_sequence_length=output_sequence_length,
             ragged=ragged,
         )
         return train_dataset, val_dataset
 
     else:
@@ -232,50 +235,43 @@
             validation_split=validation_split,
             subset=subset,
             label_mode=label_mode,
             class_names=class_names,
             sampling_rate=sampling_rate,
             output_sequence_length=output_sequence_length,
             ragged=ragged,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
         dataset = prepare_dataset(
             dataset=dataset,
             batch_size=batch_size,
-            shuffle=shuffle,
-            seed=seed,
             class_names=class_names,
             output_sequence_length=output_sequence_length,
             ragged=ragged,
         )
         return dataset
 
 
 def prepare_dataset(
     dataset,
     batch_size,
-    shuffle,
-    seed,
     class_names,
     output_sequence_length,
     ragged,
 ):
     dataset = dataset.prefetch(tf.data.AUTOTUNE)
     if batch_size is not None:
-        if shuffle:
-            dataset = dataset.shuffle(buffer_size=batch_size * 8, seed=seed)
-
         if output_sequence_length is None and not ragged:
             dataset = dataset.padded_batch(
                 batch_size, padded_shapes=([None, None], [])
             )
         else:
             dataset = dataset.batch(batch_size)
-    else:
-        if shuffle:
-            dataset = dataset.shuffle(buffer_size=1024, seed=seed)
 
     # Users may need to reference `class_names`.
     dataset.class_names = class_names
     return dataset
 
 
 def get_training_and_validation_dataset(
@@ -284,14 +280,17 @@
     validation_split,
     directory,
     label_mode,
     class_names,
     sampling_rate,
     output_sequence_length,
     ragged,
+    shuffle=False,
+    shuffle_buffer_size=None,
+    seed=None,
 ):
     (
         file_paths_train,
         labels_train,
     ) = dataset_utils.get_training_or_validation_split(
         file_paths, labels, validation_split, "training"
     )
@@ -314,24 +313,28 @@
         file_paths=file_paths_train,
         labels=labels_train,
         label_mode=label_mode,
         num_classes=len(class_names) if class_names else 0,
         sampling_rate=sampling_rate,
         output_sequence_length=output_sequence_length,
         ragged=ragged,
+        shuffle=shuffle,
+        shuffle_buffer_size=shuffle_buffer_size,
+        seed=seed,
     )
 
     val_dataset = paths_and_labels_to_dataset(
         file_paths=file_paths_val,
         labels=labels_val,
         label_mode=label_mode,
         num_classes=len(class_names) if class_names else 0,
         sampling_rate=sampling_rate,
         output_sequence_length=output_sequence_length,
         ragged=ragged,
+        shuffle=False,
     )
 
     return train_dataset, val_dataset
 
 
 def get_dataset(
     file_paths,
@@ -340,36 +343,40 @@
     validation_split,
     subset,
     label_mode,
     class_names,
     sampling_rate,
     output_sequence_length,
     ragged,
+    shuffle=False,
+    shuffle_buffer_size=None,
+    seed=None,
 ):
     file_paths, labels = dataset_utils.get_training_or_validation_split(
         file_paths, labels, validation_split, subset
     )
     if not file_paths:
         raise ValueError(
             f"No audio files found in directory {directory}. "
             f"Allowed format(s): {ALLOWED_FORMATS}"
         )
 
-    dataset = paths_and_labels_to_dataset(
+    return paths_and_labels_to_dataset(
         file_paths=file_paths,
         labels=labels,
         label_mode=label_mode,
         num_classes=len(class_names) if class_names else 0,
         sampling_rate=sampling_rate,
         output_sequence_length=output_sequence_length,
         ragged=ragged,
+        shuffle=shuffle,
+        shuffle_buffer_size=shuffle_buffer_size,
+        seed=seed,
     )
 
-    return dataset
-
 
 def read_and_decode_audio(
     path, sampling_rate=None, output_sequence_length=None
 ):
     """Reads and decodes audio file."""
     audio = tf.io.read_file(path)
 
@@ -392,17 +399,25 @@
     file_paths,
     labels,
     label_mode,
     num_classes,
     sampling_rate,
     output_sequence_length,
     ragged,
+    shuffle=False,
+    shuffle_buffer_size=None,
+    seed=None,
 ):
     """Constructs a fixed-size dataset of audio and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
+    if shuffle:
+        path_ds = path_ds.shuffle(
+            buffer_size=shuffle_buffer_size or 1024, seed=seed
+        )
+
     audio_ds = path_ds.map(
         lambda x: read_and_decode_audio(
             x, sampling_rate, output_sequence_length
         ),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
 
@@ -414,8 +429,7 @@
 
     if label_mode:
         label_ds = dataset_utils.labels_to_dataset(
             labels, label_mode, num_classes
         )
         audio_ds = tf.data.Dataset.zip((audio_ds, label_ds))
     return audio_ds
-
```

### Comparing `keras-3.2.1/keras/src/utils/backend_utils.py` & `keras-3.3.0/keras/src/utils/backend_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,19 +114,18 @@
     # Clear module cache.
     loaded_modules = [
         key for key in sys.modules.keys() if key.startswith("keras")
     ]
     for key in loaded_modules:
         del sys.modules[key]
     # Reimport Keras with the new backend (set via KERAS_BACKEND).
-    import keras.src as keras
+    import keras
 
     # Finally: refresh all imported Keras submodules.
     globs = copy.copy(globals())
     for key, value in globs.items():
         if value.__class__ == keras.__class__:
             if str(value).startswith("<module 'keras."):
                 module_name = str(value)
                 module_name = module_name[module_name.find("'") + 1 :]
                 module_name = module_name[: module_name.find("'")]
                 globals()[key] = importlib.import_module(module_name)
-
```

### Comparing `keras-3.2.1/keras/src/utils/code_stats.py` & `keras-3.3.0/keras/src/utils/code_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
                     else:
                         if not line.endswith('"""'):
                             string_open = True
                 else:
                     if line.startswith('"""'):
                         string_open = False
     return loc
-
```

### Comparing `keras-3.2.1/keras/src/utils/dataset_utils.py` & `keras-3.3.0/keras/src/utils/dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -244,15 +244,17 @@
             Defaults to `True`.
         start_time (float): the start time of the dataset iteration. this is
             used only if `data_size_warning_flag` is set to true.
 
     Yields:
         data_sample: The next sample.
     """
-    from keras.src.trainers.data_adapters.data_adapter_utils import is_torch_tensor
+    from keras.src.trainers.data_adapters.data_adapter_utils import (
+        is_torch_tensor,
+    )
 
     try:
         dataset_iterator = iter(dataset_iterator)
         first_sample = next(dataset_iterator)
         if isinstance(first_sample, (tf.Tensor, np.ndarray)) or is_torch_tensor(
             first_sample
         ):
@@ -764,8 +766,7 @@
         )
     if validation_split and shuffle and seed is None:
         raise ValueError(
             "If using `validation_split` and shuffling the data, you must "
             "provide a `seed` argument, to make sure that there is no "
             "overlap between the training and validation subset."
         )
-
```

### Comparing `keras-3.2.1/keras/src/utils/dtype_utils.py` & `keras-3.3.0/keras/src/utils/dtype_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,8 +45,7 @@
                 highest_float_size = dtype_size(dtype)
             elif dtype == "float16" and highest_float == "bfloat16":
                 highest_float = "float32"
                 highest_float_size = dtype_size(highest_float)
     if highest_float:
         tensors = [ops.cast(x, highest_float) for x in tensors]
     return tensors
-
```

### Comparing `keras-3.2.1/keras/src/utils/file_utils.py` & `keras-3.3.0/keras/src/utils/file_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -484,8 +484,7 @@
 def makedirs(path):
     if is_remote_path(path):
         if gfile.available:
             return gfile.makedirs(path)
         else:
             _raise_if_no_gfile(path)
     return os.makedirs(path)
-
```

### Comparing `keras-3.2.1/keras/src/utils/image_dataset_utils.py` & `keras-3.3.0/keras/src/utils/image_dataset_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -234,14 +234,18 @@
     if label_mode == "binary" and len(class_names) != 2:
         raise ValueError(
             'When passing `label_mode="binary"`, there must be exactly 2 '
             f"class_names. Received: class_names={class_names}"
         )
 
     data_format = standardize_data_format(data_format=data_format)
+    if batch_size is not None:
+        shuffle_buffer_size = batch_size * 8
+    else:
+        shuffle_buffer_size = 1024
 
     if subset == "both":
         (
             image_paths_train,
             labels_train,
         ) = dataset_utils.get_training_or_validation_split(
             image_paths, labels, validation_split, "training"
@@ -269,42 +273,36 @@
             labels=labels_train,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             interpolation=interpolation,
             crop_to_aspect_ratio=crop_to_aspect_ratio,
             pad_to_aspect_ratio=pad_to_aspect_ratio,
             data_format=data_format,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
 
         val_dataset = paths_and_labels_to_dataset(
             image_paths=image_paths_val,
             image_size=image_size,
             num_channels=num_channels,
             labels=labels_val,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             interpolation=interpolation,
             crop_to_aspect_ratio=crop_to_aspect_ratio,
             pad_to_aspect_ratio=pad_to_aspect_ratio,
             data_format=data_format,
+            shuffle=False,
         )
 
         if batch_size is not None:
-            if shuffle:
-                # Shuffle locally at each iteration
-                train_dataset = train_dataset.shuffle(
-                    buffer_size=batch_size * 8, seed=seed
-                )
             train_dataset = train_dataset.batch(batch_size)
             val_dataset = val_dataset.batch(batch_size)
-        else:
-            if shuffle:
-                train_dataset = train_dataset.shuffle(
-                    buffer_size=1024, seed=seed
-                )
 
         train_dataset = train_dataset.prefetch(tf.data.AUTOTUNE)
         val_dataset = val_dataset.prefetch(tf.data.AUTOTUNE)
 
         # Users may need to reference `class_names`.
         train_dataset.class_names = class_names
         val_dataset.class_names = class_names
@@ -331,24 +329,21 @@
             labels=labels,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             interpolation=interpolation,
             crop_to_aspect_ratio=crop_to_aspect_ratio,
             pad_to_aspect_ratio=pad_to_aspect_ratio,
             data_format=data_format,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
 
         if batch_size is not None:
-            if shuffle:
-                # Shuffle locally at each iteration
-                dataset = dataset.shuffle(buffer_size=batch_size * 8, seed=seed)
             dataset = dataset.batch(batch_size)
-        else:
-            if shuffle:
-                dataset = dataset.shuffle(buffer_size=1024, seed=seed)
 
         dataset = dataset.prefetch(tf.data.AUTOTUNE)
         # Users may need to reference `class_names`.
         dataset.class_names = class_names
 
         # Include file paths for images as attribute.
         dataset.file_paths = image_paths
@@ -363,18 +358,26 @@
     labels,
     label_mode,
     num_classes,
     interpolation,
     data_format,
     crop_to_aspect_ratio=False,
     pad_to_aspect_ratio=False,
+    shuffle=False,
+    shuffle_buffer_size=None,
+    seed=None,
 ):
     """Constructs a dataset of images and labels."""
     # TODO(fchollet): consider making num_parallel_calls settable
     path_ds = tf.data.Dataset.from_tensor_slices(image_paths)
+    if shuffle:
+        path_ds = path_ds.shuffle(
+            buffer_size=shuffle_buffer_size or 1024, seed=seed
+        )
+
     args = (
         image_size,
         num_channels,
         interpolation,
         data_format,
         crop_to_aspect_ratio,
         pad_to_aspect_ratio,
@@ -435,8 +438,7 @@
             img = tf.transpose(img, (2, 0, 1))
 
     if data_format == "channels_last":
         img.set_shape((image_size[0], image_size[1], num_channels))
     else:
         img.set_shape((num_channels, image_size[0], image_size[1]))
     return img
-
```

### Comparing `keras-3.2.1/keras/src/utils/image_utils.py` & `keras-3.3.0/keras/src/utils/image_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,8 +448,7 @@
     img = backend_module.image.resize(
         img, size=size, interpolation=interpolation, data_format=data_format
     )
 
     if isinstance(x, np.ndarray):
         return np.array(img)
     return img
-
```

### Comparing `keras-3.2.1/keras/src/utils/io_utils.py` & `keras-3.3.0/keras/src/utils/io_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,8 +119,7 @@
         overwrite = (
             input('Enter "y" (overwrite) or "n" (cancel).').strip().lower()
         )
     if overwrite == "n":
         return False
     print_msg("[TIP] Next time specify overwrite=True!")
     return True
-
```

### Comparing `keras-3.2.1/keras/src/utils/jax_layer.py` & `keras-3.3.0/keras/src/utils/jax_layer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import inspect
 
 import numpy as np
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.layers.layer import Layer
 from keras.src.saving import serialization_lib
 from keras.src.utils import jax_utils
 from keras.src.utils import tracking
-from keras.src.utils import tree
 from keras.src.utils.module_utils import jax
 
 
 @keras_export("keras.layers.JaxLayer")
 class JaxLayer(Layer):
     """Keras Layer that wraps a JAX model.
 
@@ -671,8 +671,7 @@
         method = serialization_lib.deserialize_keras_object(config["method"])
         if isinstance(config["method"], str):
             # Deserialize bound method from the module.
             method = getattr(module, method)
         config["module"] = module
         config["method"] = method
         return cls(**config)
-
```

### Comparing `keras-3.2.1/keras/src/utils/model_visualization.py` & `keras-3.3.0/keras/src/utils/model_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Utilities related to model visualization."""
 
 import os
 import sys
 
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 
 try:
     # pydot-ng is a fork of pydot that is better maintained.
     import pydot_ng as pydot
 except ImportError:
     # pydotplus is an improved version of pydot
     try:
@@ -68,17 +68,18 @@
     if kwargs:
         raise ValueError(f"Invalid kwargs: {kwargs}")
 
     table = (
         '<<table border="0" cellborder="1" bgcolor="black" cellpadding="10">'
     )
 
-    colspan = max(
-        1, sum(int(x) for x in (show_dtype, show_shapes, show_trainable))
-    )
+    colspan_max = sum(int(x) for x in (show_dtype, show_trainable))
+    if show_shapes:
+        colspan_max += 2
+    colspan = max(1, colspan_max)
 
     if show_layer_names:
         table += (
             f'<tr><td colspan="{colspan}" bgcolor="black">'
             '<font point-size="16" color="white">'
             f"<b>{layer.name}</b> ({class_name})"
             "</font></td></tr>"
@@ -100,23 +101,33 @@
             '<font point-size="14">'
             f"Activation: <b>{get_layer_activation_name(layer)}</b>"
             "</font></td></tr>"
         )
 
     cols = []
     if show_shapes:
-        shape = None
+        input_shape = None
+        output_shape = None
         try:
-            shape = tree.map_structure(lambda x: x.shape, layer.output)
+            input_shape = tree.map_structure(lambda x: x.shape, layer.input)
+            output_shape = tree.map_structure(lambda x: x.shape, layer.output)
         except (ValueError, AttributeError):
             pass
+        if class_name != "InputLayer":
+            cols.append(
+                (
+                    '<td bgcolor="white"><font point-size="14">'
+                    f'Input shape: <b>{input_shape or "?"}</b>'
+                    "</font></td>"
+                )
+            )
         cols.append(
             (
                 '<td bgcolor="white"><font point-size="14">'
-                f'Output shape: <b>{shape or "?"}</b>'
+                f'Output shape: <b>{output_shape or "?"}</b>'
                 "</font></td>"
             )
         )
     if show_dtype:
         dtype = None
         try:
             dtype = tree.map_structure(lambda x: x.dtype, layer.output)
@@ -244,15 +255,14 @@
         "show_layer_activations": show_layer_activations,
         "show_dtype": show_dtype,
         "show_shapes": show_shapes,
         "show_trainable": show_trainable,
     }
 
     if isinstance(model, sequential.Sequential):
-        # TODO
         layers = model.layers
     elif not isinstance(model, functional.Functional):
         # We treat subclassed models as a single node.
         node = make_node(model, **kwargs)
         dot.add_node(node)
         return dot
     else:
@@ -449,8 +459,7 @@
     if extension != "pdf":
         try:
             from IPython import display
 
             return display.Image(filename=to_file)
         except ImportError:
             pass
-
```

### Comparing `keras-3.2.1/keras/src/utils/module_utils.py` & `keras-3.3.0/keras/src/utils/module_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -37,8 +37,9 @@
 
 
 tensorflow = LazyModule("tensorflow")
 gfile = LazyModule("tensorflow.io.gfile", pip_name="tensorflow")
 tensorflow_io = LazyModule("tensorflow_io")
 scipy = LazyModule("scipy")
 jax = LazyModule("jax")
-
+optree = LazyModule("optree")
+dmtree = LazyModule("tree")
```

### Comparing `keras-3.2.1/keras/src/utils/naming.py` & `keras-3.3.0/keras/src/utils/naming.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,7 @@
     if hasattr(obj, "name"):  # Most Keras objects.
         return obj.name
     elif hasattr(obj, "__name__"):  # Function.
         return to_snake_case(obj.__name__)
     elif hasattr(obj, "__class__"):  # Class instance.
         return to_snake_case(obj.__class__.__name__)
     return to_snake_case(str(obj))
-
```

### Comparing `keras-3.2.1/keras/src/utils/numerical_utils.py` & `keras-3.3.0/keras/src/utils/numerical_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,8 +137,7 @@
     else:
         bincounts = backend_module.numpy.bincount(
             inputs,
             minlength=depth,
         )
     bincounts = backend_module.cast(bincounts, dtype)
     return bincounts
-
```

### Comparing `keras-3.2.1/keras/src/utils/progbar.py` & `keras-3.3.0/keras/src/utils/progbar.py`

 * *Files 0% similar despite different names*

```diff
@@ -263,8 +263,7 @@
                 time_per_unit = (now - self._start) / current
 
             if current == 1:
                 self._time_after_first_step = now
             return time_per_unit
         else:
             return 0
-
```

### Comparing `keras-3.2.1/keras/src/utils/python_utils.py` & `keras-3.3.0/keras/src/utils/python_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,8 +144,7 @@
 
 def remove_by_id(lst, value):
     """Remove a value from a list by id."""
     for i, v in enumerate(lst):
         if id(v) == id(value):
             del lst[i]
             return
-
```

### Comparing `keras-3.2.1/keras/src/utils/rng_utils.py` & `keras-3.3.0/keras/src/utils/rng_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,8 +50,7 @@
     np.random.seed(seed)
     if tf.available:
         tf.random.set_seed(seed)
     if backend.backend() == "torch":
         import torch
 
         torch.manual_seed(seed)
-
```

### Comparing `keras-3.2.1/keras/src/utils/sequence_utils.py` & `keras-3.3.0/keras/src/utils/sequence_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,8 +133,7 @@
         if padding == "post":
             x[idx, : len(trunc)] = trunc
         elif padding == "pre":
             x[idx, -len(trunc) :] = trunc
         else:
             raise ValueError(f'Padding type "{padding}" not understood')
     return x
-
```

### Comparing `keras-3.2.1/keras/src/utils/summary_utils.py` & `keras-3.3.0/keras/src/utils/summary_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 import rich.markup
 
 # See https://github.com/keras-team/keras/issues/448
 # for below imports
 import rich.table
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.utils import dtype_utils
 from keras.src.utils import io_utils
-from keras.src.utils import tree
 
 
 def count_params(weights):
     shapes = [v.shape for v in weights]
     return int(sum(math.prod(p) for p in shapes))
 
 
@@ -414,8 +414,7 @@
             "Passed layer_names do not match the layer names in the model. "
             f"Received: {layer_range}"
         )
 
     if min(lower_index) > max(upper_index):
         return [min(upper_index), max(lower_index) + 1]
     return [min(lower_index), max(upper_index) + 1]
-
```

### Comparing `keras-3.2.1/keras/src/utils/text_dataset_utils.py` & `keras-3.3.0/keras/src/utils/text_dataset_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,14 +156,18 @@
     )
 
     if label_mode == "binary" and len(class_names) != 2:
         raise ValueError(
             'When passing `label_mode="binary"`, there must be exactly 2 '
             f"class_names. Received: class_names={class_names}"
         )
+    if batch_size is not None:
+        shuffle_buffer_size = batch_size * 8
+    else:
+        shuffle_buffer_size = 1024
 
     if subset == "both":
         (
             file_paths_train,
             labels_train,
         ) = dataset_utils.get_training_or_validation_split(
             file_paths, labels, validation_split, "training"
@@ -186,38 +190,34 @@
             )
         train_dataset = paths_and_labels_to_dataset(
             file_paths=file_paths_train,
             labels=labels_train,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             max_length=max_length,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
         val_dataset = paths_and_labels_to_dataset(
             file_paths=file_paths_val,
             labels=labels_val,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             max_length=max_length,
+            shuffle=False,
         )
 
-        train_dataset = train_dataset.prefetch(tf.data.AUTOTUNE)
-        val_dataset = val_dataset.prefetch(tf.data.AUTOTUNE)
         if batch_size is not None:
-            if shuffle:
-                # Shuffle locally at each iteration
-                train_dataset = train_dataset.shuffle(
-                    buffer_size=batch_size * 8, seed=seed
-                )
             train_dataset = train_dataset.batch(batch_size)
             val_dataset = val_dataset.batch(batch_size)
-        else:
-            if shuffle:
-                train_dataset = train_dataset.shuffle(
-                    buffer_size=1024, seed=seed
-                )
+
+        train_dataset = train_dataset.prefetch(tf.data.AUTOTUNE)
+        val_dataset = val_dataset.prefetch(tf.data.AUTOTUNE)
+
         # Users may need to reference `class_names`.
         train_dataset.class_names = class_names
         val_dataset.class_names = class_names
         dataset = [train_dataset, val_dataset]
     else:
         file_paths, labels = dataset_utils.get_training_or_validation_split(
             file_paths, labels, validation_split, subset
@@ -229,34 +229,44 @@
             )
         dataset = paths_and_labels_to_dataset(
             file_paths=file_paths,
             labels=labels,
             label_mode=label_mode,
             num_classes=len(class_names) if class_names else 0,
             max_length=max_length,
+            shuffle=shuffle,
+            shuffle_buffer_size=shuffle_buffer_size,
+            seed=seed,
         )
-        dataset = dataset.prefetch(tf.data.AUTOTUNE)
         if batch_size is not None:
-            if shuffle:
-                # Shuffle locally at each iteration
-                dataset = dataset.shuffle(buffer_size=batch_size * 8, seed=seed)
             dataset = dataset.batch(batch_size)
-        else:
-            if shuffle:
-                dataset = dataset.shuffle(buffer_size=1024, seed=seed)
+        dataset = dataset.prefetch(tf.data.AUTOTUNE)
+
         # Users may need to reference `class_names`.
         dataset.class_names = class_names
     return dataset
 
 
 def paths_and_labels_to_dataset(
-    file_paths, labels, label_mode, num_classes, max_length
+    file_paths,
+    labels,
+    label_mode,
+    num_classes,
+    max_length,
+    shuffle=False,
+    shuffle_buffer_size=None,
+    seed=None,
 ):
     """Constructs a dataset of text strings and labels."""
     path_ds = tf.data.Dataset.from_tensor_slices(file_paths)
+    if shuffle:
+        path_ds = path_ds.shuffle(
+            buffer_size=shuffle_buffer_size or 1024, seed=seed
+        )
+
     string_ds = path_ds.map(
         lambda x: path_to_string_content(x, max_length),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     if label_mode:
         label_ds = dataset_utils.labels_to_dataset(
             labels, label_mode, num_classes
@@ -266,8 +276,7 @@
 
 
 def path_to_string_content(path, max_length):
     txt = tf.io.read_file(path)
     if max_length is not None:
         txt = tf.strings.substr(txt, 0, max_length)
     return txt
-
```

### Comparing `keras-3.2.1/keras/src/utils/tf_utils.py` & `keras-3.3.0/keras/src/utils/tf_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -140,8 +140,7 @@
 def ensure_tensor(inputs, dtype=None):
     """Ensures the input is a Tensor, SparseTensor or RaggedTensor."""
     if not isinstance(inputs, (tf.Tensor, tf.SparseTensor, tf.RaggedTensor)):
         inputs = tf.convert_to_tensor(inputs, dtype)
     if dtype is not None and inputs.dtype != dtype:
         inputs = tf.cast(inputs, dtype)
     return inputs
-
```

### Comparing `keras-3.2.1/keras/src/utils/timeseries_dataset_utils.py` & `keras-3.3.0/keras/src/utils/timeseries_dataset_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,8 +255,7 @@
 def sequences_from_indices(array, indices_ds, start_index, end_index):
     dataset = tf.data.Dataset.from_tensors(array[start_index:end_index])
     dataset = tf.data.Dataset.zip((dataset.repeat(), indices_ds)).map(
         lambda steps, inds: tf.gather(steps, inds),
         num_parallel_calls=tf.data.AUTOTUNE,
     )
     return dataset
-
```

### Comparing `keras-3.2.1/keras/src/utils/torch_utils.py` & `keras-3.3.0/keras/src/utils/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     PyTorch modules.
 
     ```python
     import torch.nn as nn
     import torch.nn.functional as F
 
     import keras
-    from keras.layers import TorchModuleWrapper
+    from keras.src.layers import TorchModuleWrapper
 
     class Classifier(keras.Model):
         def __init__(self, **kwargs):
             super().__init__(**kwargs)
             # Wrap `torch.nn.Module`s with `TorchModuleWrapper`
             # if they contain parameters
             self.conv1 = TorchModuleWrapper(
@@ -153,8 +153,7 @@
 def no_grad(orig_func):
     import torch
 
     if parse(torch.__version__) >= parse("2.1.0"):
         return torch.no_grad(orig_func)
     else:
         return orig_func
-
```

### Comparing `keras-3.2.1/keras/src/utils/traceback_utils.py` & `keras-3.3.0/keras/src/utils/traceback_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import inspect
 import os
 import traceback
 import types
 from functools import wraps
 
 from keras.src import backend
+from keras.src import tree
 from keras.src.api_export import keras_export
 from keras.src.backend.common import global_state
-from keras.src.utils import tree
 
 _EXCLUDED_PATHS = (
     os.path.abspath(os.path.join(__file__, "..", "..")),
     os.path.join("tensorflow", "python"),
 )
 
 
@@ -235,8 +235,7 @@
             tensor_cls = "array"
 
         return (
             f"{tensor_cls}(shape={value.shape}, "
             f"dtype={backend.standardize_dtype(value.dtype)})"
         )
     return repr(value)
-
```

### Comparing `keras-3.2.1/keras/src/utils/tracking.py` & `keras-3.3.0/keras/src/utils/tracking.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from functools import wraps
 
-import optree
-import optree.utils
-
+from keras.src import tree
 from keras.src.backend.common.global_state import get_global_attribute
 from keras.src.backend.common.global_state import set_global_attribute
 from keras.src.utils import python_utils
 
 
 class DotNotTrackScope:
     def __enter__(self):
@@ -78,19 +76,24 @@
                 if store_name in self.exclusions:
                     for excl in self.exclusions[store_name]:
                         if self.is_in_store(excl, attr):
                             return attr
                 if not self.is_in_store(store_name, attr):
                     self.add_to_store(store_name, attr)
                 return attr
+        if isinstance(attr, tuple) and hasattr(attr, "_fields"):
+            # Named tuple case.
+            wrapped_attr = {}
+            for name, e in attr._asdict().items():
+                wrapped_attr[name] = self.track(e)
+            return attr.__class__(**wrapped_attr)
         if isinstance(attr, tuple):
             wrapped_attr = []
             for e in attr:
                 wrapped_attr.append(self.track(e))
-            # This should cover tuples and nametuples
             return attr.__class__(wrapped_attr)
         elif isinstance(attr, list):
             return TrackedList(attr, self)
         elif isinstance(attr, dict):
             # TODO: OrderedDict?
             return TrackedDict(attr, self)
         elif isinstance(attr, set):
@@ -116,32 +119,41 @@
             raise ValueError(self._lock_violation_msg)
         self.config[store_name][1].append(value)
         self.stored_ids[store_name].add(id(value))
 
     def is_in_store(self, store_name, value):
         return id(value) in self.stored_ids[store_name]
 
+    def replace_tracked_value(self, store_name, old_value, new_value):
+        if not self.is_in_store(store_name, old_value):
+            raise ValueError(f"Unknown value: {old_value}")
+        store_list = self.config[store_name][1]
+        index = store_list.index(old_value)
+        store_list[index] = new_value
+        self.stored_ids[store_name].remove(id(old_value))
+        self.stored_ids[store_name].add(id(new_value))
+
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedList(list):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = [tracker.track(v) for v in values]
         super().__init__(values or [])
 
     def append(self, value):
         if self.tracker:
             self.tracker.track(value)
         super().append(value)
 
-    def insert(self, value):
+    def insert(self, index, value):
         if self.tracker:
             self.tracker.track(value)
-        super().insert(value)
+        super().insert(index, value)
 
     def extend(self, values):
         if self.tracker:
             values = [self.tracker.track(v) for v in values]
         super().extend(values)
 
     def remove(self, value):
@@ -178,15 +190,15 @@
 
     @classmethod
     def tree_unflatten(cls, metadata, children):
         # For optree
         return cls(children)
 
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedDict(dict):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = {k: tracker.track(v) for k, v in values.items()}
         super().__init__(values or [])
 
@@ -218,27 +230,31 @@
     def clear(self):
         if self.tracker:
             for value in self.values():
                 self.tracker.untrack(value)
         super().clear()
 
     def tree_flatten(self):
+        from keras.src.utils.module_utils import optree
+
         # For optree
         keys, values = optree.utils.unzip2(
             optree.utils.total_order_sorted(self.items(), key=lambda kv: kv[0])
         )
         return values, list(keys), keys
 
     @classmethod
     def tree_unflatten(cls, keys, values):
+        from keras.src.utils.module_utils import optree
+
         # For optree
         return cls(optree.utils.safe_zip(keys, values))
 
 
-@optree.register_pytree_node_class(namespace="keras")
+@tree.register_tree_node_class
 class TrackedSet(set):
     def __init__(self, values=None, tracker=None):
         self.tracker = tracker
         if tracker and values:
             values = {tracker.track(v) for v in values}
         super().__init__(values or [])
 
@@ -273,8 +289,7 @@
         # For optree
         return (self, None)
 
     @classmethod
     def tree_unflatten(cls, metadata, children):
         # For optree
         return cls(children)
-
```

### Comparing `keras-3.2.1/keras/utils/__init__.py` & `keras-3.3.0/keras/api/utils/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,39 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-
+from keras.api.utils import legacy
 from keras.src.backend.common.global_state import clear_session
 from keras.src.backend.common.keras_tensor import is_keras_tensor
 from keras.src.backend.common.variables import standardize_dtype
 from keras.src.layers.preprocessing.feature_space import FeatureSpace
 from keras.src.ops.operation_utils import get_source_inputs
 from keras.src.saving.object_registration import CustomObjectScope
-from keras.src.saving.object_registration import CustomObjectScope as custom_object_scope
+from keras.src.saving.object_registration import (
+    CustomObjectScope as custom_object_scope,
+)
 from keras.src.saving.object_registration import get_custom_objects
 from keras.src.saving.object_registration import get_registered_name
 from keras.src.saving.object_registration import get_registered_object
 from keras.src.saving.object_registration import register_keras_serializable
 from keras.src.saving.serialization_lib import deserialize_keras_object
 from keras.src.saving.serialization_lib import serialize_keras_object
-from keras.src.trainers.data_adapters.data_adapter_utils import pack_x_y_sample_weight
-from keras.src.trainers.data_adapters.data_adapter_utils import unpack_x_y_sample_weight
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    pack_x_y_sample_weight,
+)
+from keras.src.trainers.data_adapters.data_adapter_utils import (
+    unpack_x_y_sample_weight,
+)
 from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset
-from keras.src.trainers.data_adapters.py_dataset_adapter import PyDataset as Sequence
+from keras.src.trainers.data_adapters.py_dataset_adapter import (
+    PyDataset as Sequence,
+)
 from keras.src.utils.audio_dataset_utils import audio_dataset_from_directory
 from keras.src.utils.dataset_utils import split_dataset
 from keras.src.utils.file_utils import get_file
 from keras.src.utils.image_dataset_utils import image_dataset_from_directory
 from keras.src.utils.image_utils import array_to_img
 from keras.src.utils.image_utils import img_to_array
 from keras.src.utils.image_utils import load_img
@@ -37,9 +45,10 @@
 from keras.src.utils.model_visualization import plot_model
 from keras.src.utils.numerical_utils import normalize
 from keras.src.utils.numerical_utils import to_categorical
 from keras.src.utils.progbar import Progbar
 from keras.src.utils.rng_utils import set_random_seed
 from keras.src.utils.sequence_utils import pad_sequences
 from keras.src.utils.text_dataset_utils import text_dataset_from_directory
-from keras.src.utils.timeseries_dataset_utils import timeseries_dataset_from_array
-from keras.utils import legacy
+from keras.src.utils.timeseries_dataset_utils import (
+    timeseries_dataset_from_array,
+)
```

### Comparing `keras-3.2.1/keras.egg-info/PKG-INFO` & `keras-3.3.0/keras.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.2.1
+Version: 3.3.0
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,14 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
@@ -75,14 +76,20 @@
 
 2. Run installation command from the root directory.
 
 ```
 python pip_build.py --install
 ```
 
+3. Run API generation script when creating PRs that update `keras_export` public APIs:
+
+```
+./shell/api_gen.sh
+```
+
 #### Adding GPU support
 
 The `requirements.txt` file will install a CPU-only version of TensorFlow, JAX, and PyTorch. For GPU support, we also
 provide a separate `requirements-{backend}-cuda.txt` for TensorFlow, JAX, and PyTorch. These install all CUDA
 dependencies via `pip` and expect a NVIDIA driver to be pre-installed. We recommend a clean python environment for each
 backend to avoid CUDA version mismatches. As an example, here is how to create a Jax GPU environment with `conda`:
```

### Comparing `keras-3.2.1/keras.egg-info/SOURCES.txt` & `keras-3.3.0/keras.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,148 +1,178 @@
+LICENSE
 README.md
+pyproject.toml
+setup.cfg
 setup.py
+benchmarks/__init__.py
+benchmarks/layer_benchmark/__init__.py
+benchmarks/layer_benchmark/activation_benchmark.py
+benchmarks/layer_benchmark/attention_benchmark.py
+benchmarks/layer_benchmark/base_benchmark.py
+benchmarks/layer_benchmark/conv_benchmark.py
+benchmarks/layer_benchmark/core_benchmark.py
+benchmarks/layer_benchmark/merge_benchmark.py
+benchmarks/layer_benchmark/normalization_benchmark.py
+benchmarks/layer_benchmark/pooling_benchmark.py
+benchmarks/layer_benchmark/regularization_benchmark.py
+benchmarks/layer_benchmark/reshaping_benchmark.py
+benchmarks/layer_benchmark/rnn_benchmark.py
+benchmarks/model_benchmark/__init__.py
+benchmarks/model_benchmark/benchmark_utils.py
+benchmarks/model_benchmark/bert_benchmark.py
+benchmarks/model_benchmark/image_classification_benchmark.py
+benchmarks/torch_ctl_benchmark/__init__.py
+benchmarks/torch_ctl_benchmark/benchmark_utils.py
+benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
+benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
 keras/__init__.py
 keras.egg-info/PKG-INFO
 keras.egg-info/SOURCES.txt
 keras.egg-info/dependency_links.txt
 keras.egg-info/requires.txt
 keras.egg-info/top_level.txt
-keras/_tf_keras/__init__.py
-keras/_tf_keras/keras/__init__.py
-keras/_tf_keras/keras/activations/__init__.py
-keras/_tf_keras/keras/applications/__init__.py
-keras/_tf_keras/keras/applications/convnext/__init__.py
-keras/_tf_keras/keras/applications/densenet/__init__.py
-keras/_tf_keras/keras/applications/efficientnet/__init__.py
-keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
-keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-keras/_tf_keras/keras/applications/inception_v3/__init__.py
-keras/_tf_keras/keras/applications/mobilenet/__init__.py
-keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-keras/_tf_keras/keras/applications/nasnet/__init__.py
-keras/_tf_keras/keras/applications/resnet/__init__.py
-keras/_tf_keras/keras/applications/resnet50/__init__.py
-keras/_tf_keras/keras/applications/resnet_v2/__init__.py
-keras/_tf_keras/keras/applications/vgg16/__init__.py
-keras/_tf_keras/keras/applications/vgg19/__init__.py
-keras/_tf_keras/keras/applications/xception/__init__.py
-keras/_tf_keras/keras/backend/__init__.py
-keras/_tf_keras/keras/callbacks/__init__.py
-keras/_tf_keras/keras/config/__init__.py
-keras/_tf_keras/keras/constraints/__init__.py
-keras/_tf_keras/keras/datasets/__init__.py
-keras/_tf_keras/keras/datasets/boston_housing/__init__.py
-keras/_tf_keras/keras/datasets/california_housing/__init__.py
-keras/_tf_keras/keras/datasets/cifar10/__init__.py
-keras/_tf_keras/keras/datasets/cifar100/__init__.py
-keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-keras/_tf_keras/keras/datasets/imdb/__init__.py
-keras/_tf_keras/keras/datasets/mnist/__init__.py
-keras/_tf_keras/keras/datasets/reuters/__init__.py
-keras/_tf_keras/keras/distribution/__init__.py
-keras/_tf_keras/keras/dtype_policies/__init__.py
-keras/_tf_keras/keras/export/__init__.py
-keras/_tf_keras/keras/initializers/__init__.py
-keras/_tf_keras/keras/layers/__init__.py
-keras/_tf_keras/keras/legacy/__init__.py
-keras/_tf_keras/keras/legacy/saving/__init__.py
-keras/_tf_keras/keras/losses/__init__.py
-keras/_tf_keras/keras/metrics/__init__.py
-keras/_tf_keras/keras/mixed_precision/__init__.py
-keras/_tf_keras/keras/models/__init__.py
-keras/_tf_keras/keras/ops/__init__.py
-keras/_tf_keras/keras/ops/image/__init__.py
-keras/_tf_keras/keras/ops/linalg/__init__.py
-keras/_tf_keras/keras/ops/nn/__init__.py
-keras/_tf_keras/keras/ops/numpy/__init__.py
-keras/_tf_keras/keras/optimizers/__init__.py
-keras/_tf_keras/keras/optimizers/legacy/__init__.py
-keras/_tf_keras/keras/optimizers/schedules/__init__.py
-keras/_tf_keras/keras/preprocessing/__init__.py
-keras/_tf_keras/keras/preprocessing/image/__init__.py
-keras/_tf_keras/keras/preprocessing/sequence/__init__.py
-keras/_tf_keras/keras/preprocessing/text/__init__.py
-keras/_tf_keras/keras/quantizers/__init__.py
-keras/_tf_keras/keras/random/__init__.py
-keras/_tf_keras/keras/regularizers/__init__.py
-keras/_tf_keras/keras/saving/__init__.py
-keras/_tf_keras/keras/tree/__init__.py
-keras/_tf_keras/keras/utils/__init__.py
-keras/_tf_keras/keras/utils/legacy/__init__.py
-keras/activations/__init__.py
-keras/applications/__init__.py
-keras/applications/convnext/__init__.py
-keras/applications/densenet/__init__.py
-keras/applications/efficientnet/__init__.py
-keras/applications/efficientnet_v2/__init__.py
-keras/applications/imagenet_utils/__init__.py
-keras/applications/inception_resnet_v2/__init__.py
-keras/applications/inception_v3/__init__.py
-keras/applications/mobilenet/__init__.py
-keras/applications/mobilenet_v2/__init__.py
-keras/applications/mobilenet_v3/__init__.py
-keras/applications/nasnet/__init__.py
-keras/applications/resnet/__init__.py
-keras/applications/resnet50/__init__.py
-keras/applications/resnet_v2/__init__.py
-keras/applications/vgg16/__init__.py
-keras/applications/vgg19/__init__.py
-keras/applications/xception/__init__.py
-keras/backend/__init__.py
-keras/callbacks/__init__.py
-keras/config/__init__.py
-keras/constraints/__init__.py
-keras/datasets/__init__.py
-keras/datasets/boston_housing/__init__.py
-keras/datasets/california_housing/__init__.py
-keras/datasets/cifar10/__init__.py
-keras/datasets/cifar100/__init__.py
-keras/datasets/fashion_mnist/__init__.py
-keras/datasets/imdb/__init__.py
-keras/datasets/mnist/__init__.py
-keras/datasets/reuters/__init__.py
-keras/distribution/__init__.py
-keras/dtype_policies/__init__.py
-keras/export/__init__.py
-keras/initializers/__init__.py
-keras/layers/__init__.py
-keras/legacy/__init__.py
-keras/legacy/saving/__init__.py
-keras/losses/__init__.py
-keras/metrics/__init__.py
-keras/mixed_precision/__init__.py
-keras/models/__init__.py
-keras/ops/__init__.py
-keras/ops/image/__init__.py
-keras/ops/linalg/__init__.py
-keras/ops/nn/__init__.py
-keras/ops/numpy/__init__.py
-keras/optimizers/__init__.py
-keras/optimizers/legacy/__init__.py
-keras/optimizers/schedules/__init__.py
-keras/preprocessing/__init__.py
-keras/preprocessing/image/__init__.py
-keras/preprocessing/sequence/__init__.py
-keras/quantizers/__init__.py
-keras/random/__init__.py
-keras/regularizers/__init__.py
-keras/saving/__init__.py
+keras/api/__init__.py
+keras/api/_tf_keras/__init__.py
+keras/api/_tf_keras/keras/__init__.py
+keras/api/_tf_keras/keras/activations/__init__.py
+keras/api/_tf_keras/keras/applications/__init__.py
+keras/api/_tf_keras/keras/applications/convnext/__init__.py
+keras/api/_tf_keras/keras/applications/densenet/__init__.py
+keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
+keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
+keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+keras/api/_tf_keras/keras/applications/nasnet/__init__.py
+keras/api/_tf_keras/keras/applications/resnet/__init__.py
+keras/api/_tf_keras/keras/applications/resnet50/__init__.py
+keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
+keras/api/_tf_keras/keras/applications/vgg16/__init__.py
+keras/api/_tf_keras/keras/applications/vgg19/__init__.py
+keras/api/_tf_keras/keras/applications/xception/__init__.py
+keras/api/_tf_keras/keras/backend/__init__.py
+keras/api/_tf_keras/keras/callbacks/__init__.py
+keras/api/_tf_keras/keras/config/__init__.py
+keras/api/_tf_keras/keras/constraints/__init__.py
+keras/api/_tf_keras/keras/datasets/__init__.py
+keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
+keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
+keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
+keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
+keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+keras/api/_tf_keras/keras/datasets/imdb/__init__.py
+keras/api/_tf_keras/keras/datasets/mnist/__init__.py
+keras/api/_tf_keras/keras/datasets/reuters/__init__.py
+keras/api/_tf_keras/keras/distribution/__init__.py
+keras/api/_tf_keras/keras/dtype_policies/__init__.py
+keras/api/_tf_keras/keras/export/__init__.py
+keras/api/_tf_keras/keras/initializers/__init__.py
+keras/api/_tf_keras/keras/layers/__init__.py
+keras/api/_tf_keras/keras/legacy/__init__.py
+keras/api/_tf_keras/keras/legacy/saving/__init__.py
+keras/api/_tf_keras/keras/losses/__init__.py
+keras/api/_tf_keras/keras/metrics/__init__.py
+keras/api/_tf_keras/keras/mixed_precision/__init__.py
+keras/api/_tf_keras/keras/models/__init__.py
+keras/api/_tf_keras/keras/ops/__init__.py
+keras/api/_tf_keras/keras/ops/image/__init__.py
+keras/api/_tf_keras/keras/ops/linalg/__init__.py
+keras/api/_tf_keras/keras/ops/nn/__init__.py
+keras/api/_tf_keras/keras/ops/numpy/__init__.py
+keras/api/_tf_keras/keras/optimizers/__init__.py
+keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
+keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
+keras/api/_tf_keras/keras/preprocessing/__init__.py
+keras/api/_tf_keras/keras/preprocessing/image/__init__.py
+keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
+keras/api/_tf_keras/keras/quantizers/__init__.py
+keras/api/_tf_keras/keras/random/__init__.py
+keras/api/_tf_keras/keras/regularizers/__init__.py
+keras/api/_tf_keras/keras/saving/__init__.py
+keras/api/_tf_keras/keras/tree/__init__.py
+keras/api/_tf_keras/keras/utils/__init__.py
+keras/api/_tf_keras/keras/utils/legacy/__init__.py
+keras/api/activations/__init__.py
+keras/api/applications/__init__.py
+keras/api/applications/convnext/__init__.py
+keras/api/applications/densenet/__init__.py
+keras/api/applications/efficientnet/__init__.py
+keras/api/applications/efficientnet_v2/__init__.py
+keras/api/applications/imagenet_utils/__init__.py
+keras/api/applications/inception_resnet_v2/__init__.py
+keras/api/applications/inception_v3/__init__.py
+keras/api/applications/mobilenet/__init__.py
+keras/api/applications/mobilenet_v2/__init__.py
+keras/api/applications/mobilenet_v3/__init__.py
+keras/api/applications/nasnet/__init__.py
+keras/api/applications/resnet/__init__.py
+keras/api/applications/resnet50/__init__.py
+keras/api/applications/resnet_v2/__init__.py
+keras/api/applications/vgg16/__init__.py
+keras/api/applications/vgg19/__init__.py
+keras/api/applications/xception/__init__.py
+keras/api/backend/__init__.py
+keras/api/callbacks/__init__.py
+keras/api/config/__init__.py
+keras/api/constraints/__init__.py
+keras/api/datasets/__init__.py
+keras/api/datasets/boston_housing/__init__.py
+keras/api/datasets/california_housing/__init__.py
+keras/api/datasets/cifar10/__init__.py
+keras/api/datasets/cifar100/__init__.py
+keras/api/datasets/fashion_mnist/__init__.py
+keras/api/datasets/imdb/__init__.py
+keras/api/datasets/mnist/__init__.py
+keras/api/datasets/reuters/__init__.py
+keras/api/distribution/__init__.py
+keras/api/dtype_policies/__init__.py
+keras/api/export/__init__.py
+keras/api/initializers/__init__.py
+keras/api/layers/__init__.py
+keras/api/legacy/__init__.py
+keras/api/legacy/saving/__init__.py
+keras/api/losses/__init__.py
+keras/api/metrics/__init__.py
+keras/api/mixed_precision/__init__.py
+keras/api/models/__init__.py
+keras/api/ops/__init__.py
+keras/api/ops/image/__init__.py
+keras/api/ops/linalg/__init__.py
+keras/api/ops/nn/__init__.py
+keras/api/ops/numpy/__init__.py
+keras/api/optimizers/__init__.py
+keras/api/optimizers/legacy/__init__.py
+keras/api/optimizers/schedules/__init__.py
+keras/api/preprocessing/__init__.py
+keras/api/preprocessing/image/__init__.py
+keras/api/preprocessing/sequence/__init__.py
+keras/api/quantizers/__init__.py
+keras/api/random/__init__.py
+keras/api/regularizers/__init__.py
+keras/api/saving/__init__.py
+keras/api/tree/__init__.py
+keras/api/utils/__init__.py
+keras/api/utils/legacy/__init__.py
 keras/src/__init__.py
 keras/src/api_export.py
 keras/src/version.py
 keras/src/activations/__init__.py
 keras/src/activations/activations.py
+keras/src/activations/activations_test.py
 keras/src/applications/__init__.py
+keras/src/applications/applications_test.py
 keras/src/applications/convnext.py
 keras/src/applications/densenet.py
 keras/src/applications/efficientnet.py
 keras/src/applications/efficientnet_v2.py
 keras/src/applications/imagenet_utils.py
+keras/src/applications/imagenet_utils_test.py
 keras/src/applications/inception_resnet_v2.py
 keras/src/applications/inception_v3.py
 keras/src/applications/mobilenet.py
 keras/src/applications/mobilenet_v2.py
 keras/src/applications/mobilenet_v3.py
 keras/src/applications/nasnet.py
 keras/src/applications/resnet.py
@@ -151,23 +181,32 @@
 keras/src/applications/vgg19.py
 keras/src/applications/xception.py
 keras/src/backend/__init__.py
 keras/src/backend/config.py
 keras/src/backend/exports.py
 keras/src/backend/common/__init__.py
 keras/src/backend/common/backend_utils.py
+keras/src/backend/common/backend_utils_test.py
+keras/src/backend/common/compute_output_spec_test.py
 keras/src/backend/common/dtypes.py
+keras/src/backend/common/dtypes_test.py
 keras/src/backend/common/global_state.py
+keras/src/backend/common/global_state_test.py
 keras/src/backend/common/keras_tensor.py
+keras/src/backend/common/keras_tensor_test.py
 keras/src/backend/common/name_scope.py
+keras/src/backend/common/name_scope_test.py
 keras/src/backend/common/stateless_scope.py
+keras/src/backend/common/stateless_scope_test.py
 keras/src/backend/common/variables.py
+keras/src/backend/common/variables_test.py
 keras/src/backend/jax/__init__.py
 keras/src/backend/jax/core.py
 keras/src/backend/jax/distribution_lib.py
+keras/src/backend/jax/distribution_lib_test.py
 keras/src/backend/jax/image.py
 keras/src/backend/jax/layer.py
 keras/src/backend/jax/linalg.py
 keras/src/backend/jax/math.py
 keras/src/backend/jax/nn.py
 keras/src/backend/jax/numpy.py
 keras/src/backend/jax/optimizer.py
@@ -184,24 +223,28 @@
 keras/src/backend/numpy/nn.py
 keras/src/backend/numpy/numpy.py
 keras/src/backend/numpy/random.py
 keras/src/backend/numpy/rnn.py
 keras/src/backend/numpy/trainer.py
 keras/src/backend/tensorflow/__init__.py
 keras/src/backend/tensorflow/core.py
+keras/src/backend/tensorflow/distribute_test.py
 keras/src/backend/tensorflow/distribution_lib.py
 keras/src/backend/tensorflow/image.py
 keras/src/backend/tensorflow/layer.py
 keras/src/backend/tensorflow/linalg.py
 keras/src/backend/tensorflow/math.py
+keras/src/backend/tensorflow/name_scope_test.py
 keras/src/backend/tensorflow/nn.py
 keras/src/backend/tensorflow/numpy.py
 keras/src/backend/tensorflow/optimizer.py
+keras/src/backend/tensorflow/optimizer_distribute_test.py
 keras/src/backend/tensorflow/random.py
 keras/src/backend/tensorflow/rnn.py
+keras/src/backend/tensorflow/saved_model_test.py
 keras/src/backend/tensorflow/sparse.py
 keras/src/backend/tensorflow/tensorboard.py
 keras/src/backend/tensorflow/trackable.py
 keras/src/backend/tensorflow/trainer.py
 keras/src/backend/torch/__init__.py
 keras/src/backend/torch/core.py
 keras/src/backend/torch/image.py
@@ -223,293 +266,476 @@
 keras/src/backend/torch/optimizers/torch_nadam.py
 keras/src/backend/torch/optimizers/torch_optimizer.py
 keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
 keras/src/backend/torch/optimizers/torch_rmsprop.py
 keras/src/backend/torch/optimizers/torch_sgd.py
 keras/src/callbacks/__init__.py
 keras/src/callbacks/backup_and_restore.py
+keras/src/callbacks/backup_and_restore_test.py
 keras/src/callbacks/callback.py
 keras/src/callbacks/callback_list.py
+keras/src/callbacks/callback_test.py
 keras/src/callbacks/csv_logger.py
+keras/src/callbacks/csv_logger_test.py
 keras/src/callbacks/early_stopping.py
+keras/src/callbacks/early_stopping_test.py
 keras/src/callbacks/history.py
 keras/src/callbacks/lambda_callback.py
+keras/src/callbacks/lambda_callback_test.py
 keras/src/callbacks/learning_rate_scheduler.py
+keras/src/callbacks/learning_rate_scheduler_test.py
 keras/src/callbacks/model_checkpoint.py
+keras/src/callbacks/model_checkpoint_test.py
 keras/src/callbacks/progbar_logger.py
 keras/src/callbacks/reduce_lr_on_plateau.py
+keras/src/callbacks/reduce_lr_on_plateau_test.py
 keras/src/callbacks/remote_monitor.py
+keras/src/callbacks/remote_monitor_test.py
 keras/src/callbacks/swap_ema_weights.py
+keras/src/callbacks/swap_ema_weights_test.py
 keras/src/callbacks/tensorboard.py
+keras/src/callbacks/tensorboard_test.py
 keras/src/callbacks/terminate_on_nan.py
+keras/src/callbacks/terminate_on_nan_test.py
 keras/src/constraints/__init__.py
 keras/src/constraints/constraints.py
+keras/src/constraints/constraints_test.py
 keras/src/datasets/__init__.py
 keras/src/datasets/boston_housing.py
 keras/src/datasets/california_housing.py
 keras/src/datasets/cifar.py
 keras/src/datasets/cifar10.py
 keras/src/datasets/cifar100.py
 keras/src/datasets/fashion_mnist.py
 keras/src/datasets/imdb.py
 keras/src/datasets/mnist.py
 keras/src/datasets/reuters.py
 keras/src/distribution/__init__.py
 keras/src/distribution/distribution_lib.py
+keras/src/distribution/distribution_lib_test.py
 keras/src/dtype_policies/__init__.py
 keras/src/dtype_policies/dtype_policy.py
+keras/src/dtype_policies/dtype_policy_test.py
 keras/src/export/__init__.py
 keras/src/export/export_lib.py
+keras/src/export/export_lib_test.py
 keras/src/initializers/__init__.py
 keras/src/initializers/constant_initializers.py
+keras/src/initializers/constant_initializers_test.py
 keras/src/initializers/initializer.py
 keras/src/initializers/random_initializers.py
+keras/src/initializers/random_initializers_test.py
 keras/src/layers/__init__.py
 keras/src/layers/input_spec.py
 keras/src/layers/layer.py
+keras/src/layers/layer_test.py
 keras/src/layers/activations/__init__.py
 keras/src/layers/activations/activation.py
+keras/src/layers/activations/activation_test.py
 keras/src/layers/activations/elu.py
+keras/src/layers/activations/elu_test.py
 keras/src/layers/activations/leaky_relu.py
+keras/src/layers/activations/leaky_relu_test.py
 keras/src/layers/activations/prelu.py
+keras/src/layers/activations/prelu_test.py
 keras/src/layers/activations/relu.py
+keras/src/layers/activations/relu_test.py
 keras/src/layers/activations/softmax.py
+keras/src/layers/activations/softmax_test.py
 keras/src/layers/attention/__init__.py
 keras/src/layers/attention/additive_attention.py
+keras/src/layers/attention/additive_attention_test.py
 keras/src/layers/attention/attention.py
+keras/src/layers/attention/attention_test.py
 keras/src/layers/attention/grouped_query_attention.py
+keras/src/layers/attention/grouped_query_attention_test.py
 keras/src/layers/attention/multi_head_attention.py
+keras/src/layers/attention/multi_head_attention_test.py
 keras/src/layers/convolutional/__init__.py
 keras/src/layers/convolutional/base_conv.py
 keras/src/layers/convolutional/base_conv_transpose.py
 keras/src/layers/convolutional/base_depthwise_conv.py
 keras/src/layers/convolutional/base_separable_conv.py
 keras/src/layers/convolutional/conv1d.py
 keras/src/layers/convolutional/conv1d_transpose.py
 keras/src/layers/convolutional/conv2d.py
 keras/src/layers/convolutional/conv2d_transpose.py
 keras/src/layers/convolutional/conv3d.py
 keras/src/layers/convolutional/conv3d_transpose.py
+keras/src/layers/convolutional/conv_test.py
+keras/src/layers/convolutional/conv_transpose_test.py
 keras/src/layers/convolutional/depthwise_conv1d.py
 keras/src/layers/convolutional/depthwise_conv2d.py
+keras/src/layers/convolutional/depthwise_conv_test.py
 keras/src/layers/convolutional/separable_conv1d.py
 keras/src/layers/convolutional/separable_conv2d.py
+keras/src/layers/convolutional/separable_conv_test.py
 keras/src/layers/core/__init__.py
 keras/src/layers/core/dense.py
+keras/src/layers/core/dense_test.py
 keras/src/layers/core/einsum_dense.py
+keras/src/layers/core/einsum_dense_test.py
 keras/src/layers/core/embedding.py
+keras/src/layers/core/embedding_test.py
 keras/src/layers/core/identity.py
+keras/src/layers/core/identity_test.py
 keras/src/layers/core/input_layer.py
+keras/src/layers/core/input_layer_test.py
 keras/src/layers/core/lambda_layer.py
+keras/src/layers/core/lambda_layer_test.py
 keras/src/layers/core/masking.py
+keras/src/layers/core/masking_test.py
 keras/src/layers/core/wrapper.py
+keras/src/layers/core/wrapper_test.py
 keras/src/layers/merging/__init__.py
 keras/src/layers/merging/add.py
 keras/src/layers/merging/average.py
 keras/src/layers/merging/base_merge.py
 keras/src/layers/merging/concatenate.py
 keras/src/layers/merging/dot.py
 keras/src/layers/merging/maximum.py
+keras/src/layers/merging/merging_test.py
 keras/src/layers/merging/minimum.py
 keras/src/layers/merging/multiply.py
 keras/src/layers/merging/subtract.py
 keras/src/layers/normalization/__init__.py
 keras/src/layers/normalization/batch_normalization.py
+keras/src/layers/normalization/batch_normalization_test.py
 keras/src/layers/normalization/group_normalization.py
+keras/src/layers/normalization/group_normalization_test.py
 keras/src/layers/normalization/layer_normalization.py
+keras/src/layers/normalization/layer_normalization_test.py
 keras/src/layers/normalization/spectral_normalization.py
+keras/src/layers/normalization/spectral_normalization_test.py
 keras/src/layers/normalization/unit_normalization.py
+keras/src/layers/normalization/unit_normalization_test.py
 keras/src/layers/pooling/__init__.py
 keras/src/layers/pooling/average_pooling1d.py
 keras/src/layers/pooling/average_pooling2d.py
 keras/src/layers/pooling/average_pooling3d.py
+keras/src/layers/pooling/average_pooling_test.py
 keras/src/layers/pooling/base_global_pooling.py
 keras/src/layers/pooling/base_pooling.py
 keras/src/layers/pooling/global_average_pooling1d.py
 keras/src/layers/pooling/global_average_pooling2d.py
 keras/src/layers/pooling/global_average_pooling3d.py
+keras/src/layers/pooling/global_average_pooling_test.py
 keras/src/layers/pooling/global_max_pooling1d.py
 keras/src/layers/pooling/global_max_pooling2d.py
 keras/src/layers/pooling/global_max_pooling3d.py
+keras/src/layers/pooling/global_max_pooling_test.py
 keras/src/layers/pooling/max_pooling1d.py
 keras/src/layers/pooling/max_pooling2d.py
 keras/src/layers/pooling/max_pooling3d.py
+keras/src/layers/pooling/max_pooling_test.py
 keras/src/layers/preprocessing/__init__.py
 keras/src/layers/preprocessing/audio_preprocessing.py
+keras/src/layers/preprocessing/audio_preprocessing_test.py
 keras/src/layers/preprocessing/category_encoding.py
+keras/src/layers/preprocessing/category_encoding_test.py
 keras/src/layers/preprocessing/center_crop.py
+keras/src/layers/preprocessing/center_crop_test.py
 keras/src/layers/preprocessing/discretization.py
+keras/src/layers/preprocessing/discretization_test.py
 keras/src/layers/preprocessing/feature_space.py
+keras/src/layers/preprocessing/feature_space_test.py
 keras/src/layers/preprocessing/hashed_crossing.py
+keras/src/layers/preprocessing/hashed_crossing_test.py
 keras/src/layers/preprocessing/hashing.py
+keras/src/layers/preprocessing/hashing_test.py
 keras/src/layers/preprocessing/index_lookup.py
+keras/src/layers/preprocessing/index_lookup_test.py
 keras/src/layers/preprocessing/integer_lookup.py
+keras/src/layers/preprocessing/integer_lookup_test.py
 keras/src/layers/preprocessing/normalization.py
+keras/src/layers/preprocessing/normalization_test.py
 keras/src/layers/preprocessing/random_brightness.py
+keras/src/layers/preprocessing/random_brightness_test.py
 keras/src/layers/preprocessing/random_contrast.py
+keras/src/layers/preprocessing/random_contrast_test.py
 keras/src/layers/preprocessing/random_crop.py
+keras/src/layers/preprocessing/random_crop_test.py
 keras/src/layers/preprocessing/random_flip.py
+keras/src/layers/preprocessing/random_flip_test.py
 keras/src/layers/preprocessing/random_rotation.py
+keras/src/layers/preprocessing/random_rotation_test.py
 keras/src/layers/preprocessing/random_translation.py
+keras/src/layers/preprocessing/random_translation_test.py
 keras/src/layers/preprocessing/random_zoom.py
+keras/src/layers/preprocessing/random_zoom_test.py
 keras/src/layers/preprocessing/rescaling.py
+keras/src/layers/preprocessing/rescaling_test.py
 keras/src/layers/preprocessing/resizing.py
+keras/src/layers/preprocessing/resizing_test.py
 keras/src/layers/preprocessing/string_lookup.py
+keras/src/layers/preprocessing/string_lookup_test.py
 keras/src/layers/preprocessing/text_vectorization.py
+keras/src/layers/preprocessing/text_vectorization_test.py
 keras/src/layers/preprocessing/tf_data_layer.py
 keras/src/layers/regularization/__init__.py
 keras/src/layers/regularization/activity_regularization.py
+keras/src/layers/regularization/activity_regularization_test.py
 keras/src/layers/regularization/alpha_dropout.py
+keras/src/layers/regularization/alpha_dropout_test.py
 keras/src/layers/regularization/dropout.py
+keras/src/layers/regularization/dropout_test.py
 keras/src/layers/regularization/gaussian_dropout.py
+keras/src/layers/regularization/gaussian_dropout_test.py
 keras/src/layers/regularization/gaussian_noise.py
+keras/src/layers/regularization/gaussian_noise_test.py
 keras/src/layers/regularization/spatial_dropout.py
+keras/src/layers/regularization/spatial_dropout_test.py
 keras/src/layers/reshaping/__init__.py
 keras/src/layers/reshaping/cropping1d.py
+keras/src/layers/reshaping/cropping1d_test.py
 keras/src/layers/reshaping/cropping2d.py
+keras/src/layers/reshaping/cropping2d_test.py
 keras/src/layers/reshaping/cropping3d.py
+keras/src/layers/reshaping/cropping3d_test.py
 keras/src/layers/reshaping/flatten.py
+keras/src/layers/reshaping/flatten_test.py
 keras/src/layers/reshaping/permute.py
+keras/src/layers/reshaping/permute_test.py
 keras/src/layers/reshaping/repeat_vector.py
+keras/src/layers/reshaping/repeat_vector_test.py
 keras/src/layers/reshaping/reshape.py
+keras/src/layers/reshaping/reshape_test.py
 keras/src/layers/reshaping/up_sampling1d.py
+keras/src/layers/reshaping/up_sampling1d_test.py
 keras/src/layers/reshaping/up_sampling2d.py
+keras/src/layers/reshaping/up_sampling2d_test.py
 keras/src/layers/reshaping/up_sampling3d.py
+keras/src/layers/reshaping/up_sampling3d_test.py
 keras/src/layers/reshaping/zero_padding1d.py
+keras/src/layers/reshaping/zero_padding1d_test.py
 keras/src/layers/reshaping/zero_padding2d.py
+keras/src/layers/reshaping/zero_padding2d_test.py
 keras/src/layers/reshaping/zero_padding3d.py
+keras/src/layers/reshaping/zero_padding3d_test.py
 keras/src/layers/rnn/__init__.py
 keras/src/layers/rnn/bidirectional.py
+keras/src/layers/rnn/bidirectional_test.py
 keras/src/layers/rnn/conv_lstm.py
 keras/src/layers/rnn/conv_lstm1d.py
+keras/src/layers/rnn/conv_lstm1d_test.py
 keras/src/layers/rnn/conv_lstm2d.py
+keras/src/layers/rnn/conv_lstm2d_test.py
 keras/src/layers/rnn/conv_lstm3d.py
+keras/src/layers/rnn/conv_lstm3d_test.py
+keras/src/layers/rnn/conv_lstm_test.py
 keras/src/layers/rnn/dropout_rnn_cell.py
+keras/src/layers/rnn/dropout_rnn_cell_test.py
 keras/src/layers/rnn/gru.py
+keras/src/layers/rnn/gru_test.py
 keras/src/layers/rnn/lstm.py
+keras/src/layers/rnn/lstm_test.py
 keras/src/layers/rnn/rnn.py
+keras/src/layers/rnn/rnn_test.py
 keras/src/layers/rnn/simple_rnn.py
+keras/src/layers/rnn/simple_rnn_test.py
 keras/src/layers/rnn/stacked_rnn_cells.py
+keras/src/layers/rnn/stacked_rnn_cells_test.py
 keras/src/layers/rnn/time_distributed.py
+keras/src/layers/rnn/time_distributed_test.py
 keras/src/legacy/__init__.py
 keras/src/legacy/backend.py
 keras/src/legacy/layers.py
 keras/src/legacy/losses.py
 keras/src/legacy/preprocessing/__init__.py
 keras/src/legacy/preprocessing/image.py
 keras/src/legacy/preprocessing/sequence.py
 keras/src/legacy/preprocessing/text.py
 keras/src/legacy/saving/__init__.py
 keras/src/legacy/saving/json_utils.py
+keras/src/legacy/saving/json_utils_test.py
 keras/src/legacy/saving/legacy_h5_format.py
+keras/src/legacy/saving/legacy_h5_format_test.py
 keras/src/legacy/saving/saving_options.py
 keras/src/legacy/saving/saving_utils.py
 keras/src/legacy/saving/serialization.py
 keras/src/losses/__init__.py
 keras/src/losses/loss.py
+keras/src/losses/loss_test.py
 keras/src/losses/losses.py
+keras/src/losses/losses_test.py
 keras/src/metrics/__init__.py
 keras/src/metrics/accuracy_metrics.py
+keras/src/metrics/accuracy_metrics_test.py
 keras/src/metrics/confusion_metrics.py
+keras/src/metrics/confusion_metrics_test.py
 keras/src/metrics/f_score_metrics.py
+keras/src/metrics/f_score_metrics_test.py
 keras/src/metrics/hinge_metrics.py
+keras/src/metrics/hinge_metrics_test.py
 keras/src/metrics/iou_metrics.py
+keras/src/metrics/iou_metrics_test.py
 keras/src/metrics/metric.py
+keras/src/metrics/metric_test.py
 keras/src/metrics/metrics_utils.py
 keras/src/metrics/probabilistic_metrics.py
+keras/src/metrics/probabilistic_metrics_test.py
 keras/src/metrics/reduction_metrics.py
+keras/src/metrics/reduction_metrics_test.py
 keras/src/metrics/regression_metrics.py
+keras/src/metrics/regression_metrics_test.py
 keras/src/models/__init__.py
 keras/src/models/cloning.py
+keras/src/models/cloning_test.py
 keras/src/models/functional.py
+keras/src/models/functional_test.py
 keras/src/models/model.py
+keras/src/models/model_test.py
 keras/src/models/sequential.py
+keras/src/models/sequential_test.py
 keras/src/models/variable_mapping.py
+keras/src/models/variable_mapping_test.py
 keras/src/ops/__init__.py
 keras/src/ops/core.py
+keras/src/ops/core_test.py
 keras/src/ops/function.py
+keras/src/ops/function_test.py
 keras/src/ops/image.py
+keras/src/ops/image_test.py
 keras/src/ops/linalg.py
+keras/src/ops/linalg_test.py
 keras/src/ops/math.py
+keras/src/ops/math_test.py
 keras/src/ops/nn.py
+keras/src/ops/nn_test.py
 keras/src/ops/node.py
+keras/src/ops/node_test.py
 keras/src/ops/numpy.py
+keras/src/ops/numpy_test.py
 keras/src/ops/operation.py
+keras/src/ops/operation_test.py
 keras/src/ops/operation_utils.py
+keras/src/ops/operation_utils_test.py
 keras/src/ops/symbolic_arguments.py
+keras/src/ops/symbolic_arguments_test.py
 keras/src/optimizers/__init__.py
 keras/src/optimizers/adadelta.py
+keras/src/optimizers/adadelta_test.py
 keras/src/optimizers/adafactor.py
+keras/src/optimizers/adafactor_test.py
 keras/src/optimizers/adagrad.py
+keras/src/optimizers/adagrad_test.py
 keras/src/optimizers/adam.py
+keras/src/optimizers/adam_test.py
 keras/src/optimizers/adamax.py
+keras/src/optimizers/adamax_test.py
 keras/src/optimizers/adamw.py
+keras/src/optimizers/adamw_test.py
 keras/src/optimizers/base_optimizer.py
 keras/src/optimizers/ftrl.py
+keras/src/optimizers/ftrl_test.py
 keras/src/optimizers/lion.py
+keras/src/optimizers/lion_test.py
 keras/src/optimizers/loss_scale_optimizer.py
+keras/src/optimizers/loss_scale_optimizer_test.py
 keras/src/optimizers/nadam.py
+keras/src/optimizers/nadam_test.py
 keras/src/optimizers/optimizer.py
+keras/src/optimizers/optimizer_sparse_test.py
+keras/src/optimizers/optimizer_test.py
 keras/src/optimizers/rmsprop.py
+keras/src/optimizers/rmsprop_test.py
 keras/src/optimizers/sgd.py
+keras/src/optimizers/sgd_test.py
 keras/src/optimizers/schedules/__init__.py
 keras/src/optimizers/schedules/learning_rate_schedule.py
+keras/src/optimizers/schedules/learning_rate_schedule_test.py
 keras/src/quantizers/__init__.py
 keras/src/quantizers/quantizers.py
+keras/src/quantizers/quantizers_test.py
 keras/src/random/__init__.py
 keras/src/random/random.py
+keras/src/random/random_test.py
 keras/src/random/seed_generator.py
+keras/src/random/seed_generator_test.py
 keras/src/regularizers/__init__.py
 keras/src/regularizers/regularizers.py
+keras/src/regularizers/regularizers_test.py
 keras/src/saving/__init__.py
 keras/src/saving/object_registration.py
+keras/src/saving/object_registration_test.py
 keras/src/saving/saving_api.py
+keras/src/saving/saving_api_test.py
 keras/src/saving/saving_lib.py
+keras/src/saving/saving_lib_test.py
 keras/src/saving/serialization_lib.py
+keras/src/saving/serialization_lib_test.py
 keras/src/testing/__init__.py
 keras/src/testing/test_case.py
 keras/src/testing/test_utils.py
+keras/src/testing/test_utils_test.py
 keras/src/trainers/__init__.py
 keras/src/trainers/compile_utils.py
+keras/src/trainers/compile_utils_test.py
 keras/src/trainers/epoch_iterator.py
+keras/src/trainers/epoch_iterator_test.py
 keras/src/trainers/trainer.py
+keras/src/trainers/trainer_test.py
 keras/src/trainers/data_adapters/__init__.py
 keras/src/trainers/data_adapters/array_data_adapter.py
+keras/src/trainers/data_adapters/array_data_adapter_test.py
 keras/src/trainers/data_adapters/array_slicing.py
 keras/src/trainers/data_adapters/data_adapter.py
 keras/src/trainers/data_adapters/data_adapter_utils.py
 keras/src/trainers/data_adapters/generator_data_adapter.py
+keras/src/trainers/data_adapters/generator_data_adapter_test.py
 keras/src/trainers/data_adapters/py_dataset_adapter.py
+keras/src/trainers/data_adapters/py_dataset_adapter_test.py
 keras/src/trainers/data_adapters/tf_dataset_adapter.py
+keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
 keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
+keras/src/tree/__init__.py
+keras/src/tree/dmtree_impl.py
+keras/src/tree/optree_impl.py
+keras/src/tree/tree_api.py
+keras/src/tree/tree_test.py
 keras/src/utils/__init__.py
 keras/src/utils/argument_validation.py
 keras/src/utils/audio_dataset_utils.py
+keras/src/utils/audio_dataset_utils_test.py
 keras/src/utils/backend_utils.py
 keras/src/utils/code_stats.py
+keras/src/utils/code_stats_test.py
 keras/src/utils/dataset_utils.py
+keras/src/utils/dataset_utils_test.py
 keras/src/utils/dtype_utils.py
+keras/src/utils/dtype_utils_test.py
 keras/src/utils/file_utils.py
+keras/src/utils/file_utils_test.py
 keras/src/utils/image_dataset_utils.py
+keras/src/utils/image_dataset_utils_test.py
 keras/src/utils/image_utils.py
 keras/src/utils/io_utils.py
+keras/src/utils/io_utils_test.py
 keras/src/utils/jax_layer.py
+keras/src/utils/jax_layer_test.py
 keras/src/utils/jax_utils.py
 keras/src/utils/model_visualization.py
 keras/src/utils/module_utils.py
 keras/src/utils/naming.py
+keras/src/utils/naming_test.py
 keras/src/utils/numerical_utils.py
+keras/src/utils/numerical_utils_test.py
 keras/src/utils/progbar.py
 keras/src/utils/python_utils.py
+keras/src/utils/python_utils_test.py
 keras/src/utils/rng_utils.py
+keras/src/utils/rng_utils_test.py
 keras/src/utils/sequence_utils.py
+keras/src/utils/sequence_utils_test.py
 keras/src/utils/summary_utils.py
+keras/src/utils/summary_utils_test.py
 keras/src/utils/text_dataset_utils.py
+keras/src/utils/text_dataset_utils_test.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
+keras/src/utils/timeseries_dataset_utils_test.py
 keras/src/utils/torch_utils.py
+keras/src/utils/torch_utils_test.py
 keras/src/utils/traceback_utils.py
 keras/src/utils/tracking.py
-keras/src/utils/tree.py
-keras/tree/__init__.py
-keras/utils/__init__.py
-keras/utils/legacy/__init__.py
+keras/src/utils/tracking_test.py
```

### Comparing `keras-3.2.1/setup.py` & `keras-3.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,18 +19,15 @@
             delim = '"' if '"' in line else "'"
             return line.split(delim)[1]
     raise RuntimeError("Unable to find version string.")
 
 
 HERE = pathlib.Path(__file__).parent
 README = (HERE / "README.md").read_text()
-if os.path.exists("keras/version.py"):
-    VERSION = get_version("keras/version.py")
-else:
-    VERSION = get_version("keras/__init__.py")
+VERSION = get_version("keras/src/version.py")
 
 setup(
     name="keras",
     description="Multi-backend Keras.",
     long_description_content_type="text/markdown",
     long_description=README,
     version=VERSION,
```

