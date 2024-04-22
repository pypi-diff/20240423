# Comparing `tmp/keras-3.3.0.tar.gz` & `tmp/keras-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keras-3.3.0.tar", last modified: Mon Apr 22 18:30:47 2024, max compression
+gzip compressed data, was "keras-3.3.1.tar", last modified: Mon Apr 22 22:42:13 2024, max compression
```

## Comparing `keras-3.3.0.tar` & `keras-3.3.1.tar`

### file list

```diff
@@ -1,921 +1,695 @@
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.593129 keras-3.3.0/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11356 2023-09-22 16:55:14.000000 keras-3.3.0/LICENSE
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5753 2024-04-22 18:30:47.593031 keras-3.3.0/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4789 2024-04-20 16:30:07.000000 keras-3.3.0/README.md
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.345190 keras-3.3.0/benchmarks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.349220 keras-3.3.0/benchmarks/layer_benchmark/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3754 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/activation_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3052 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/attention_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9434 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/base_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7246 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/conv_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3033 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/core_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5706 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/merge_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3507 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/normalization_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8179 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/pooling_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4668 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/regularization_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7154 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/reshaping_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6189 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/layer_benchmark/rnn_benchmark.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.350277 keras-3.3.0/benchmarks/model_benchmark/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      790 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/benchmark_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4661 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/bert_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4498 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/model_benchmark/image_classification_benchmark.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.351320 keras-3.3.0/benchmarks/torch_ctl_benchmark/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1087 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/benchmark_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2638 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2574 2024-04-15 18:21:08.000000 keras-3.3.0/benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.351581 keras-3.3.0/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      828 2024-04-20 19:17:05.000000 keras-3.3.0/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.353225 keras-3.3.0/keras/api/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.353607 keras-3.3.0/keras/api/_tf_keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-20 19:17:01.000000 keras-3.3.0/keras/api/_tf_keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.354274 keras-3.3.0/keras/api/_tf_keras/keras/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2057 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.354854 keras-3.3.0/keras/api/_tf_keras/keras/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355077 keras-3.3.0/keras/api/_tf_keras/keras/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355454 keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355676 keras-3.3.0/keras/api/_tf_keras/keras/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.355899 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356149 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356412 keras-3.3.0/keras/api/_tf_keras/keras/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356649 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.356880 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357093 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357324 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357545 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.357769 keras-3.3.0/keras/api/_tf_keras/keras/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358001 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358218 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358439 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358667 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.358913 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359138 keras-3.3.0/keras/api/_tf_keras/keras/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359339 keras-3.3.0/keras/api/_tf_keras/keras/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359530 keras-3.3.0/keras/api/_tf_keras/keras/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359775 keras-3.3.0/keras/api/_tf_keras/keras/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.359979 keras-3.3.0/keras/api/_tf_keras/keras/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360187 keras-3.3.0/keras/api/_tf_keras/keras/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360390 keras-3.3.0/keras/api/_tf_keras/keras/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360598 keras-3.3.0/keras/api/_tf_keras/keras/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.360806 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361009 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361304 keras-3.3.0/keras/api/_tf_keras/keras/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.361654 keras-3.3.0/keras/api/_tf_keras/keras/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.362807 keras-3.3.0/keras/api/_tf_keras/keras/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363008 keras-3.3.0/keras/api/_tf_keras/keras/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363194 keras-3.3.0/keras/api/_tf_keras/keras/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363379 keras-3.3.0/keras/api/_tf_keras/keras/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.0/keras/api/_tf_keras/keras/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363684 keras-3.3.0/keras/api/_tf_keras/keras/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.363871 keras-3.3.0/keras/api/_tf_keras/keras/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364064 keras-3.3.0/keras/api/_tf_keras/keras/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364395 keras-3.3.0/keras/api/_tf_keras/keras/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364580 keras-3.3.0/keras/api/_tf_keras/keras/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364757 keras-3.3.0/keras/api/_tf_keras/keras/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.364928 keras-3.3.0/keras/api/_tf_keras/keras/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365270 keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365438 keras-3.3.0/keras/api/_tf_keras/keras/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.365621 keras-3.3.0/keras/api/_tf_keras/keras/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366004 keras-3.3.0/keras/api/_tf_keras/keras/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366188 keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.366364 keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.373453 keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.373894 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374141 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374337 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374534 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374735 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.374932 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.375931 keras-3.3.0/keras/api/_tf_keras/keras/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376149 keras-3.3.0/keras/api/_tf_keras/keras/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376337 keras-3.3.0/keras/api/_tf_keras/keras/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376539 keras-3.3.0/keras/api/_tf_keras/keras/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376738 keras-3.3.0/keras/api/_tf_keras/keras/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.376935 keras-3.3.0/keras/api/_tf_keras/keras/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.377122 keras-3.3.0/keras/api/_tf_keras/keras/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/_tf_keras/keras/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.381399 keras-3.3.0/keras/api/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/activations/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.381699 keras-3.3.0/keras/api/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.382463 keras-3.3.0/keras/api/applications/convnext/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/convnext/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.382731 keras-3.3.0/keras/api/applications/densenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/densenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.383547 keras-3.3.0/keras/api/applications/efficientnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/efficientnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.384442 keras-3.3.0/keras/api/applications/efficientnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/efficientnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385250 keras-3.3.0/keras/api/applications/imagenet_utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/imagenet_utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385443 keras-3.3.0/keras/api/applications/inception_resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/inception_resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385647 keras-3.3.0/keras/api/applications/inception_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/inception_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.385873 keras-3.3.0/keras/api/applications/mobilenet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386084 keras-3.3.0/keras/api/applications/mobilenet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386281 keras-3.3.0/keras/api/applications/mobilenet_v3/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/mobilenet_v3/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386463 keras-3.3.0/keras/api/applications/nasnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/nasnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.386802 keras-3.3.0/keras/api/applications/resnet/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387013 keras-3.3.0/keras/api/applications/resnet50/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet50/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387202 keras-3.3.0/keras/api/applications/resnet_v2/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/resnet_v2/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387383 keras-3.3.0/keras/api/applications/vgg16/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/vgg16/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387599 keras-3.3.0/keras/api/applications/vgg19/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/vgg19/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387803 keras-3.3.0/keras/api/applications/xception/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/applications/xception/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.387986 keras-3.3.0/keras/api/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388185 keras-3.3.0/keras/api/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/callbacks/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388382 keras-3.3.0/keras/api/config/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/config/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388575 keras-3.3.0/keras/api/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/constraints/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388778 keras-3.3.0/keras/api/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.388952 keras-3.3.0/keras/api/datasets/boston_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/boston_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389148 keras-3.3.0/keras/api/datasets/california_housing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/california_housing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389370 keras-3.3.0/keras/api/datasets/cifar10/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/cifar10/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389570 keras-3.3.0/keras/api/datasets/cifar100/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/cifar100/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.389764 keras-3.3.0/keras/api/datasets/fashion_mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/fashion_mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390003 keras-3.3.0/keras/api/datasets/imdb/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/imdb/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390230 keras-3.3.0/keras/api/datasets/mnist/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/mnist/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390444 keras-3.3.0/keras/api/datasets/reuters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/datasets/reuters/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390641 keras-3.3.0/keras/api/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/distribution/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.390839 keras-3.3.0/keras/api/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.0/keras/api/dtype_policies/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391138 keras-3.3.0/keras/api/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/export/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391349 keras-3.3.0/keras/api/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/initializers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.391750 keras-3.3.0/keras/api/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392138 keras-3.3.0/keras/api/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392329 keras-3.3.0/keras/api/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/legacy/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392516 keras-3.3.0/keras/api/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/losses/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.392799 keras-3.3.0/keras/api/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/metrics/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393143 keras-3.3.0/keras/api/mixed_precision/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/mixed_precision/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393318 keras-3.3.0/keras/api/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/models/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393493 keras-3.3.0/keras/api/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393779 keras-3.3.0/keras/api/ops/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.393945 keras-3.3.0/keras/api/ops/linalg/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/linalg/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.394189 keras-3.3.0/keras/api/ops/nn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/nn/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.394496 keras-3.3.0/keras/api/ops/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/ops/numpy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395392 keras-3.3.0/keras/api/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395632 keras-3.3.0/keras/api/optimizers/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.395815 keras-3.3.0/keras/api/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/optimizers/schedules/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396005 keras-3.3.0/keras/api/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396175 keras-3.3.0/keras/api/preprocessing/image/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/image/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396357 keras-3.3.0/keras/api/preprocessing/sequence/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/preprocessing/sequence/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396578 keras-3.3.0/keras/api/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/quantizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.396802 keras-3.3.0/keras/api/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/random/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.397096 keras-3.3.0/keras/api/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/regularizers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.398296 keras-3.3.0/keras/api/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/saving/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.398577 keras-3.3.0/keras/api/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/tree/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.399719 keras-3.3.0/keras/api/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/utils/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.399911 keras-3.3.0/keras/api/utils/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.0/keras/api/utils/legacy/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.400700 keras-3.3.0/keras/src/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      648 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.401439 keras-3.3.0/keras/src/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3540 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12442 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/activations.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30862 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/activations/activations_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/api_export.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.408011 keras-3.3.0/keras/src/applications/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10394 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/applications_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24919 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/convnext.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16848 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/densenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25274 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/efficientnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40460 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/efficientnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16034 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/imagenet_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11284 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/imagenet_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/inception_resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15520 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/inception_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17168 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17934 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23521 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/mobilenet_v3.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/nasnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19006 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/resnet.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/resnet_v2.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9110 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/vgg16.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9433 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/vgg19.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12705 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/applications/xception.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.409246 keras-3.3.0/keras/src/backend/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1971 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.414887 keras-3.3.0/keras/src/backend/common/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      583 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17099 2024-04-21 17:37:40.000000 keras-3.3.0/keras/src/backend/common/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8151 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/backend_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2118 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/compute_output_spec_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9808 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/dtypes.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8548 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/dtypes_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/global_state.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      499 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/global_state_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8974 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/keras_tensor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15026 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/keras_tensor_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/name_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2101 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/name_scope_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3692 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/stateless_scope.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1990 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/stateless_scope_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21446 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/common/variables.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31785 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/common/variables_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7139 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/config.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1056 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/exports.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.421169 keras-3.3.0/keras/src/backend/jax/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12765 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9679 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13481 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/distribution_lib_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14746 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       25 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1800 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8757 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26214 2024-04-22 16:38:23.000000 keras-3.3.0/keras/src/backend/jax/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30833 2024-04-22 17:47:17.000000 keras-3.3.0/keras/src/backend/jax/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3856 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13804 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    36259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/jax/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.425361 keras-3.3.0/keras/src/backend/numpy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6855 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13086 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       27 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1964 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18006 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/numpy/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28098 2024-04-21 17:26:32.000000 keras-3.3.0/keras/src/backend/numpy/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3961 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7652 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10738 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/numpy/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.432774 keras-3.3.0/keras/src/backend/tensorflow/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1458 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9444 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4406 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/distribute_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2747 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14197 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4639 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6161 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11451 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1624 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/name_scope_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26595 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    77771 2024-04-21 17:37:08.000000 keras-3.3.0/keras/src/backend/tensorflow/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9334 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7667 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/optimizer_distribute_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/tensorflow/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34600 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13290 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/saved_model_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32268 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/sparse.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1993 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/trackable.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33111 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/tensorflow/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.437089 keras-3.3.0/keras/src/backend/torch/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1892 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16162 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14001 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1865 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15073 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24278 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/backend/torch/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    47434 2024-04-21 17:37:08.000000 keras-3.3.0/keras/src/backend/torch/numpy.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.439641 keras-3.3.0/keras/src/backend/torch/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       78 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1672 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2421 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1803 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      783 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2053 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/optimizers/torch_sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8292 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13704 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17577 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/backend/torch/trainer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.447451 keras-3.3.0/keras/src/callbacks/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      922 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/backup_and_restore.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6109 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/backup_and_restore_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9830 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5255 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback_list.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/callback_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3206 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/csv_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5831 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/csv_logger_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8933 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/early_stopping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9528 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/early_stopping_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1301 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/history.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3441 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/lambda_callback.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6061 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/lambda_callback_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2965 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/learning_rate_scheduler.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3806 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/learning_rate_scheduler_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18488 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/model_checkpoint.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18107 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/model_checkpoint_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3104 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/progbar_logger.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5339 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4313 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/remote_monitor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3766 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/remote_monitor_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6843 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/swap_ema_weights.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6707 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/swap_ema_weights_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26393 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/tensorboard.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27236 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/tensorboard_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/terminate_on_nan.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1717 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/callbacks/terminate_on_nan_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.448188 keras-3.3.0/keras/src/constraints/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1715 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7333 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/constraints.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3505 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/constraints/constraints_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.450084 keras-3.3.0/keras/src/datasets/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      383 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/boston_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3850 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/california_housing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      704 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3086 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar10.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2914 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/cifar100.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2929 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/fashion_mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7149 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/imdb.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2393 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/mnist.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/datasets/reuters.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.450753 keras-3.3.0/keras/src/distribution/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      718 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31207 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/distribution_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18510 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/distribution/distribution_lib_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.451868 keras-3.3.0/keras/src/dtype_policies/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3506 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12480 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/dtype_policy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19083 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/dtype_policies/dtype_policy_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.452870 keras-3.3.0/keras/src/export/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       54 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32830 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/export_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33240 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/export/export_lib_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.454896 keras-3.3.0/keras/src/initializers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3958 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4884 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/constant_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/constant_initializers_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2633 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/initializer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23462 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/random_initializers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6637 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/initializers/random_initializers_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.456649 keras-3.3.0/keras/src/layers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8848 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/__init__.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.459603 keras-3.3.0/keras/src/layers/activations/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      272 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1236 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/activation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1108 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/activation_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/elu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      844 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/elu_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1900 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/leaky_relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/leaky_relu_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3453 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/prelu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1167 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/prelu_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/relu.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2864 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/relu_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2258 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/softmax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1679 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/activations/softmax_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.462138 keras-3.3.0/keras/src/layers/attention/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4330 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/additive_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3030 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/additive_attention_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11889 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14343 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/attention_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17952 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/grouped_query_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7755 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/grouped_query_attention_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28353 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/multi_head_attention.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13745 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/attention/multi_head_attention_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.468561 keras-3.3.0/keras/src/layers/convolutional/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17263 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/convolutional/base_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10695 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_conv_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11617 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_depthwise_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12643 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/base_separable_conv.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5571 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv1d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5691 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv2d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5893 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5897 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv3d_transpose.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32424 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27575 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/conv_transpose_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5999 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6087 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/depthwise_conv_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6531 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11914 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/convolutional/separable_conv_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.476049 keras-3.3.0/keras/src/layers/core/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25345 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26286 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/dense_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    42181 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/einsum_dense.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31411 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/layers/core/einsum_dense_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17364 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/layers/core/embedding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15413 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/embedding_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      817 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/identity.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1098 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/identity_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5107 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/input_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4670 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/input_layer_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8989 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/lambda_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3259 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/lambda_layer_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2629 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/masking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1712 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/masking_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1535 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/wrapper.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2589 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/core/wrapper_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9827 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/input_spec.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    63788 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/layers/layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    34277 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/layer_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.478530 keras-3.3.0/keras/src/layers/merging/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/add.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/average.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9249 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/base_merge.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6586 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/concatenate.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12807 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/dot.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/maximum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9678 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/merging_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/minimum.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2211 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/multiply.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2684 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/merging/subtract.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.481170 keras-3.3.0/keras/src/layers/normalization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13440 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/batch_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8094 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/batch_normalization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8534 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/group_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5919 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/group_normalization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9836 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/layer_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4832 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/layer_normalization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4306 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/spectral_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3034 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/spectral_normalization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1831 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/unit_normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2062 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/normalization/unit_normalization_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.486574 keras-3.3.0/keras/src/layers/pooling/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4150 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3235 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12382 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/average_pooling_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1460 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/base_global_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2425 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/base_pooling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3131 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2469 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2603 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6009 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_average_pooling_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2357 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2451 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2585 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5370 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/global_max_pooling_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3343 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4125 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3225 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9863 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/pooling/max_pooling_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.501723 keras-3.3.0/keras/src/layers/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14572 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8705 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/category_encoding.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/category_encoding_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5489 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/center_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/center_crop_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13145 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/discretization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6031 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/discretization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29613 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/feature_space.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21053 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/feature_space_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8317 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6810 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10936 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20526 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/hashing_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    41399 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/index_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21777 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/index_lookup_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18458 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/integer_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3480 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/integer_lookup_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13920 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/normalization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5271 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/normalization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6463 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_brightness.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4199 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_brightness_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3814 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_contrast.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1553 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_contrast_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6315 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_crop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_crop_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3805 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_flip.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5398 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_flip_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9645 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_rotation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2685 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_rotation_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10614 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_translation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11944 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_translation_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10820 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_zoom.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5186 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/random_zoom_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2177 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/rescaling.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3007 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/rescaling_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5349 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/resizing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/resizing_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17734 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/string_lookup.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1940 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/string_lookup_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27820 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/text_vectorization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5959 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/text_vectorization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/preprocessing/tf_data_layer.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.504175 keras-3.3.0/keras/src/layers/regularization/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1198 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/activity_regularization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/activity_regularization_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/alpha_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2161 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/alpha_dropout_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2978 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2125 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/dropout_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2041 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1074 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_dropout_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_noise.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1020 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/gaussian_noise_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/spatial_dropout.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/regularization/spatial_dropout_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.512085 keras-3.3.0/keras/src/layers/reshaping/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2760 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2921 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping1d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9044 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5253 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping2d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11265 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7196 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/cropping3d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3059 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/flatten.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4368 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/flatten_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2087 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/permute.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2736 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/permute_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1335 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/repeat_vector.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1548 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/repeat_vector_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/reshape.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3956 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/reshape_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1592 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2244 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling1d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5992 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5096 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling2d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4862 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/up_sampling3d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1920 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding1d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3781 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding2d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4288 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/reshaping/zero_padding3d_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.520038 keras-3.3.0/keras/src/layers/rnn/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/bidirectional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9359 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/bidirectional_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27242 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8294 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm1d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2838 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm1d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8379 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm2d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3194 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm2d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8287 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm3d.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3832 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm3d_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2275 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/conv_lstm_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2132 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3299 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27701 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/gru.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9441 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/gru_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26544 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/lstm.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9743 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/lstm_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19159 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15320 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/rnn_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17537 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/simple_rnn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9276 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/simple_rnn_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4943 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9872 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4797 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/time_distributed.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2814 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/layers/rnn/time_distributed_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.521616 keras-3.3.0/keras/src/legacy/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    70241 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/backend.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/layers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      523 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/losses.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.523180 keras-3.3.0/keras/src/legacy/preprocessing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    65545 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11172 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/sequence.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11110 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/preprocessing/text.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.525815 keras-3.3.0/keras/src/legacy/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7296 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/json_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3318 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/json_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22750 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/legacy_h5_format.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19413 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/legacy_h5_format_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      485 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/saving_options.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9275 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/saving_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    21808 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/legacy/saving/serialization.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.527753 keras-3.3.0/keras/src/losses/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-22 16:35:02.000000 keras-3.3.0/keras/src/losses/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5892 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/loss.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9374 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/loss_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    69132 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/losses.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    54720 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/losses/losses_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.535845 keras-3.3.0/keras/src/metrics/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7198 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15604 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/accuracy_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17463 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/accuracy_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    61579 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/confusion_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    63267 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/confusion_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11743 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/f_score_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15184 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/f_score_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3255 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/hinge_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4801 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/hinge_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26976 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/iou_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17104 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/iou_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8186 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metric.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metric_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26611 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/metrics_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10692 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/probabilistic_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8939 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/probabilistic_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7212 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/reduction_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5044 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/reduction_metrics_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19818 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/regression_metrics.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14185 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/metrics/regression_metrics_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.539723 keras-3.3.0/keras/src/models/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      143 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11094 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/cloning.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4113 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/cloning_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    32453 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/functional.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14762 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/functional_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23789 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/models/model.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    24695 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/models/model_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13013 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/sequential.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8380 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/sequential_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2164 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/variable_mapping.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1350 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/models/variable_mapping_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.553292 keras-3.3.0/keras/src/ops/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      644 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    22866 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/core.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31327 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/core_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15334 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/function.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4890 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/function_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    37256 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/image.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    31485 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/image_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    18342 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/linalg.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19959 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/linalg_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30618 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/math.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    47868 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/math_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    64046 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/ops/nn.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    83662 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/ops/nn_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5583 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/node.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2206 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/node_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   195627 2024-04-21 17:37:09.000000 keras-3.3.0/keras/src/ops/numpy.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)   285133 2024-04-21 17:37:12.000000 keras-3.3.0/keras/src/ops/numpy_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10732 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5533 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13759 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7368 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/operation_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1694 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/symbolic_arguments.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3615 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/ops/symbolic_arguments_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.561781 keras-3.3.0/keras/src/optimizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3931 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4759 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adadelta.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2744 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adadelta_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7637 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adafactor.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3791 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adafactor_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3918 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adagrad.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3249 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adagrad_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5909 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3657 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adam_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5083 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamax.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3173 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamax_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3784 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamw.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3254 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/adamw_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    40410 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/base_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/ftrl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2634 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/ftrl_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4969 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/lion.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2985 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/lion_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11553 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/loss_scale_optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4203 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/loss_scale_optimizer_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5926 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/nadam.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3304 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/nadam_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      813 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11204 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer_sparse_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13009 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/optimizer_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6003 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/rmsprop.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2761 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/rmsprop_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.562476 keras-3.3.0/keras/src/optimizers/schedules/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      546 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    35507 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15392 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4556 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/sgd.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3392 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/optimizers/sgd_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.563294 keras-3.3.0/keras/src/quantizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1784 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4810 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/quantizers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3006 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/quantizers/quantizers_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.564882 keras-3.3.0/keras/src/random/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      420 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13438 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/random.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17949 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/random_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4905 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/seed_generator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2855 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/random/seed_generator_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.565811 keras-3.3.0/keras/src/regularizers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1731 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/regularizers.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5675 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/regularizers/regularizers_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.569527 keras-3.3.0/keras/src/saving/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      614 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7358 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/object_registration.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4701 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/object_registration_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9737 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9033 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_api_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27008 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    33448 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/saving/saving_lib_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    29052 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/saving/serialization_lib.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13761 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/saving/serialization_lib_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.570664 keras-3.3.0/keras/src/testing/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      266 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    27552 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_case.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6197 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10599 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/testing/test_utils_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.572732 keras-3.3.0/keras/src/trainers/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    25940 2024-04-22 17:46:41.000000 keras-3.3.0/keras/src/trainers/compile_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    13799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/compile_utils_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.577269 keras-3.3.0/keras/src/trainers/data_adapters/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5423 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14323 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9404 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    17071 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/array_slicing.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3101 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9717 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/data_adapter_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2863 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     6621 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    19412 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9799 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5224 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10998 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2643 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7146 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3923 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/epoch_iterator.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5843 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/trainers/epoch_iterator_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    46449 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/trainers/trainer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    54651 2024-04-22 17:46:42.000000 keras-3.3.0/keras/src/trainers/trainer_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.578657 keras-3.3.0/keras/src/tree/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      521 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4970 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/dmtree_impl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11138 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/optree_impl.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9397 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/tree_api.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10359 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/tree/tree_test.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.592112 keras-3.3.0/keras/src/utils/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/__init__.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2876 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/argument_validation.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14664 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/audio_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16561 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/audio_dataset_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4130 2024-04-20 18:16:39.000000 keras-3.3.0/keras/src/utils/backend_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1442 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/code_stats.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5709 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/code_stats_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28554 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    12500 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dataset_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dtype_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5986 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/dtype_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16371 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/file_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    28322 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/file_utils_test.py
--rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16538 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    20039 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_dataset_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    16544 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/image_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3491 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/io_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2361 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/io_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    26570 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_layer.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    23050 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_layer_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      263 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/jax_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/model_visualization.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1276 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/module_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1776 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/naming.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4269 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/naming_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/numerical_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2604 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/numerical_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10349 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/progbar.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4003 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/python_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     3512 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/python_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/rng_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/rng_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4714 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/sequence_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4558 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/sequence_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    14512 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/summary_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1675 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/summary_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    10509 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/text_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    11279 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/text_dataset_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4630 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/tf_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     9842 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/timeseries_dataset_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     7769 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/timeseries_dataset_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     4991 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/torch_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8232 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/torch_utils_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8997 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/traceback_utils.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     8980 2024-04-21 17:38:44.000000 keras-3.3.0/keras/src/utils/tracking.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     2907 2024-04-20 16:30:07.000000 keras-3.3.0/keras/src/utils/tracking_test.py
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      189 2024-04-22 18:30:45.000000 keras-3.3.0/keras/src/version.py
-drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 18:30:47.592605 keras-3.3.0/keras.egg-info/
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     5753 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/PKG-INFO
--rw-r--r--   0 fchollet (337002) primarygroup (89939)    30370 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/SOURCES.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/dependency_links.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/requires.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)       17 2024-04-22 18:30:47.000000 keras-3.3.0/keras.egg-info/top_level.txt
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1128 2023-09-22 16:55:14.000000 keras-3.3.0/pyproject.toml
--rw-r--r--   0 fchollet (337002) primarygroup (89939)      285 2024-04-22 18:30:47.593487 keras-3.3.0/setup.cfg
--rw-r--r--   0 fchollet (337002) primarygroup (89939)     1769 2024-04-20 16:30:07.000000 keras-3.3.0/setup.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.251859 keras-3.3.1/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-22 22:42:13.251578 keras-3.3.1/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4789 2024-04-22 22:42:06.000000 keras-3.3.1/README.md
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.157150 keras-3.3.1/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      828 2024-04-20 19:17:05.000000 keras-3.3.1/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158107 keras-3.3.1/keras/_tf_keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       34 2024-04-22 22:42:06.000000 keras-3.3.1/keras/_tf_keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158270 keras-3.3.1/keras/_tf_keras/keras/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2057 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158427 keras-3.3.1/keras/_tf_keras/keras/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158582 keras-3.3.1/keras/_tf_keras/keras/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158737 keras-3.3.1/keras/_tf_keras/keras/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.158891 keras-3.3.1/keras/_tf_keras/keras/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159050 keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159203 keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159356 keras-3.3.1/keras/_tf_keras/keras/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159502 keras-3.3.1/keras/_tf_keras/keras/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159642 keras-3.3.1/keras/_tf_keras/keras/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159789 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.159944 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.160114 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.160288 keras-3.3.1/keras/_tf_keras/keras/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.160459 keras-3.3.1/keras/_tf_keras/keras/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.160602 keras-3.3.1/keras/_tf_keras/keras/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.160883 keras-3.3.1/keras/_tf_keras/keras/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161069 keras-3.3.1/keras/_tf_keras/keras/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161242 keras-3.3.1/keras/_tf_keras/keras/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161406 keras-3.3.1/keras/_tf_keras/keras/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161569 keras-3.3.1/keras/_tf_keras/keras/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161726 keras-3.3.1/keras/_tf_keras/keras/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.161903 keras-3.3.1/keras/_tf_keras/keras/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162073 keras-3.3.1/keras/_tf_keras/keras/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162228 keras-3.3.1/keras/_tf_keras/keras/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162383 keras-3.3.1/keras/_tf_keras/keras/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162537 keras-3.3.1/keras/_tf_keras/keras/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162683 keras-3.3.1/keras/_tf_keras/keras/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162830 keras-3.3.1/keras/_tf_keras/keras/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.162981 keras-3.3.1/keras/_tf_keras/keras/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163129 keras-3.3.1/keras/_tf_keras/keras/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163277 keras-3.3.1/keras/_tf_keras/keras/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163427 keras-3.3.1/keras/_tf_keras/keras/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163590 keras-3.3.1/keras/_tf_keras/keras/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163747 keras-3.3.1/keras/_tf_keras/keras/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.1/keras/_tf_keras/keras/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.163895 keras-3.3.1/keras/_tf_keras/keras/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164058 keras-3.3.1/keras/_tf_keras/keras/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164215 keras-3.3.1/keras/_tf_keras/keras/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164395 keras-3.3.1/keras/_tf_keras/keras/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164536 keras-3.3.1/keras/_tf_keras/keras/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164686 keras-3.3.1/keras/_tf_keras/keras/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.164861 keras-3.3.1/keras/_tf_keras/keras/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165038 keras-3.3.1/keras/_tf_keras/keras/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165190 keras-3.3.1/keras/_tf_keras/keras/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165338 keras-3.3.1/keras/_tf_keras/keras/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165505 keras-3.3.1/keras/_tf_keras/keras/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165660 keras-3.3.1/keras/_tf_keras/keras/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165805 keras-3.3.1/keras/_tf_keras/keras/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.165947 keras-3.3.1/keras/_tf_keras/keras/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166103 keras-3.3.1/keras/_tf_keras/keras/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166258 keras-3.3.1/keras/_tf_keras/keras/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166413 keras-3.3.1/keras/_tf_keras/keras/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166566 keras-3.3.1/keras/_tf_keras/keras/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166742 keras-3.3.1/keras/_tf_keras/keras/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.166914 keras-3.3.1/keras/_tf_keras/keras/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167089 keras-3.3.1/keras/_tf_keras/keras/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167253 keras-3.3.1/keras/_tf_keras/keras/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167408 keras-3.3.1/keras/_tf_keras/keras/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167585 keras-3.3.1/keras/_tf_keras/keras/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167755 keras-3.3.1/keras/_tf_keras/keras/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.167925 keras-3.3.1/keras/_tf_keras/keras/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168096 keras-3.3.1/keras/_tf_keras/keras/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.1/keras/_tf_keras/keras/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168273 keras-3.3.1/keras/api/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2058 2024-04-22 22:42:06.000000 keras-3.3.1/keras/api/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168451 keras-3.3.1/keras/api/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1347 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/activations/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168616 keras-3.3.1/keras/api/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3295 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168769 keras-3.3.1/keras/api/applications/convnext/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      535 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/convnext/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.168945 keras-3.3.1/keras/api/applications/densenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      414 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/densenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169112 keras-3.3.1/keras/api/applications/efficientnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      758 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/efficientnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169279 keras-3.3.1/keras/api/applications/efficientnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      733 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/efficientnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169425 keras-3.3.1/keras/api/applications/imagenet_utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      258 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/imagenet_utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169580 keras-3.3.1/keras/api/applications/inception_resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      341 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/inception_resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169758 keras-3.3.1/keras/api/applications/inception_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/inception_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.169941 keras-3.3.1/keras/api/applications/mobilenet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      303 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/mobilenet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.170111 keras-3.3.1/keras/api/applications/mobilenet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      314 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/mobilenet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.170277 keras-3.3.1/keras/api/applications/mobilenet_v3/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      254 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/mobilenet_v3/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.170437 keras-3.3.1/keras/api/applications/nasnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      351 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/nasnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.170807 keras-3.3.1/keras/api/applications/resnet/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      397 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/resnet/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.170991 keras-3.3.1/keras/api/applications/resnet50/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      293 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/resnet50/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171167 keras-3.3.1/keras/api/applications/resnet_v2/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      418 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/resnet_v2/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171337 keras-3.3.1/keras/api/applications/vgg16/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/vgg16/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171501 keras-3.3.1/keras/api/applications/vgg19/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      287 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/vgg19/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171671 keras-3.3.1/keras/api/applications/xception/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      299 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/applications/xception/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171826 keras-3.3.1/keras/api/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      883 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.171980 keras-3.3.1/keras/api/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1044 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/callbacks/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172146 keras-3.3.1/keras/api/config/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1143 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/config/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172295 keras-3.3.1/keras/api/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      797 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/constraints/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172451 keras-3.3.1/keras/api/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      454 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172595 keras-3.3.1/keras/api/datasets/boston_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      178 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/boston_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172744 keras-3.3.1/keras/api/datasets/california_housing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      182 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/california_housing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.172885 keras-3.3.1/keras/api/datasets/cifar10/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      171 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/cifar10/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173037 keras-3.3.1/keras/api/datasets/cifar100/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      172 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/cifar100/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173189 keras-3.3.1/keras/api/datasets/fashion_mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      177 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/fashion_mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173345 keras-3.3.1/keras/api/datasets/imdb/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      219 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/imdb/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173482 keras-3.3.1/keras/api/datasets/mnist/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      169 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/mnist/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173637 keras-3.3.1/keras/api/datasets/reuters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      280 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/datasets/reuters/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173797 keras-3.3.1/keras/api/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      775 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/distribution/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.173946 keras-3.3.1/keras/api/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      536 2024-04-22 16:35:02.000000 keras-3.3.1/keras/api/dtype_policies/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174102 keras-3.3.1/keras/api/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      176 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/export/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174264 keras-3.3.1/keras/api/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2844 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/initializers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174411 keras-3.3.1/keras/api/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9963 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174575 keras-3.3.1/keras/api/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      158 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174715 keras-3.3.1/keras/api/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/legacy/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.174855 keras-3.3.1/keras/api/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2381 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/losses/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175005 keras-3.3.1/keras/api/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4239 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/metrics/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175169 keras-3.3.1/keras/api/mixed_precision/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      636 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/mixed_precision/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175330 keras-3.3.1/keras/api/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      416 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/models/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175476 keras-3.3.1/keras/api/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8842 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/ops/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175639 keras-3.3.1/keras/api/ops/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      442 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/ops/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175781 keras-3.3.1/keras/api/ops/linalg/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      556 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/ops/linalg/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.175930 keras-3.3.1/keras/api/ops/nn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1464 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/ops/nn/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176076 keras-3.3.1/keras/api/ops/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5687 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/ops/numpy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176244 keras-3.3.1/keras/api/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      965 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/optimizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176415 keras-3.3.1/keras/api/optimizers/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      516 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/optimizers/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176571 keras-3.3.1/keras/api/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      918 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/optimizers/schedules/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176716 keras-3.3.1/keras/api/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      453 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/preprocessing/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.176862 keras-3.3.1/keras/api/preprocessing/image/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      379 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/preprocessing/image/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177028 keras-3.3.1/keras/api/preprocessing/sequence/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      179 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/preprocessing/sequence/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177196 keras-3.3.1/keras/api/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      627 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/quantizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177353 keras-3.3.1/keras/api/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      628 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/random/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177502 keras-3.3.1/keras/api/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      819 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/regularizers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177666 keras-3.3.1/keras/api/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      923 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/saving/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177827 keras-3.3.1/keras/api/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      582 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/tree/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.177988 keras-3.3.1/keras/api/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2652 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/utils/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.178134 keras-3.3.1/keras/api/utils/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      270 2024-04-20 19:17:05.000000 keras-3.3.1/keras/api/utils/legacy/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.178574 keras-3.3.1/keras/src/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      648 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.178856 keras-3.3.1/keras/src/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3540 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12442 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/activations/activations.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/api_export.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.182462 keras-3.3.1/keras/src/applications/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24919 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/convnext.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16848 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/densenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25274 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/efficientnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40460 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/efficientnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16034 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/imagenet_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14509 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/inception_resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15520 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/inception_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17168 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/mobilenet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17934 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/mobilenet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23521 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/mobilenet_v3.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30694 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/nasnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19006 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/resnet.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/resnet_v2.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9110 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/vgg16.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9433 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/vgg19.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12705 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/applications/xception.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.182970 keras-3.3.1/keras/src/backend/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1971 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.184466 keras-3.3.1/keras/src/backend/common/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      583 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17099 2024-04-21 17:37:40.000000 keras-3.3.1/keras/src/backend/common/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9808 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/dtypes.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3412 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/global_state.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8974 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/keras_tensor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2545 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/name_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3692 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/common/stateless_scope.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21446 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/common/variables.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7139 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/config.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1056 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/exports.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.187129 keras-3.3.1/keras/src/backend/jax/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1173 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12765 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9679 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14746 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       25 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1800 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8757 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26214 2024-04-22 16:38:23.000000 keras-3.3.1/keras/src/backend/jax/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30912 2024-04-22 20:22:03.000000 keras-3.3.1/keras/src/backend/jax/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3856 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13804 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    36259 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/jax/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.189365 keras-3.3.1/keras/src/backend/numpy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1012 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6855 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13086 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       27 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1964 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10586 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18006 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/numpy/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28176 2024-04-22 20:22:03.000000 keras-3.3.1/keras/src/backend/numpy/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3961 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7652 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10738 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/numpy/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.192421 keras-3.3.1/keras/src/backend/tensorflow/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1458 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9444 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2747 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/distribution_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14197 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4639 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6161 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/tensorflow/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11451 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/tensorflow/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26595 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/tensorflow/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    78597 2024-04-22 22:26:57.000000 keras-3.3.1/keras/src/backend/tensorflow/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9334 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6211 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/tensorflow/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    34600 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32268 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/sparse.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      170 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1993 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/trackable.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    33111 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/tensorflow/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.194593 keras-3.3.1/keras/src/backend/torch/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1892 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16162 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14001 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1865 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1801 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15073 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    24278 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/backend/torch/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    47943 2024-04-22 20:22:03.000000 keras-3.3.1/keras/src/backend/torch/numpy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.196497 keras-3.3.1/keras/src/backend/torch/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       78 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1672 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1889 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      150 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1041 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2421 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1803 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      783 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2053 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_rmsprop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1175 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/optimizers/torch_sgd.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8292 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13704 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17577 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/backend/torch/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.198883 keras-3.3.1/keras/src/callbacks/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      922 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7552 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/backup_and_restore.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9830 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5255 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/callback_list.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3206 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/csv_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8933 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/early_stopping.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1301 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/history.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3441 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/lambda_callback.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2965 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/learning_rate_scheduler.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18488 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/model_checkpoint.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3104 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/progbar_logger.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5339 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/reduce_lr_on_plateau.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2727 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/remote_monitor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6843 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/swap_ema_weights.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26393 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/tensorboard.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      669 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/callbacks/terminate_on_nan.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.199159 keras-3.3.1/keras/src/constraints/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1715 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/constraints/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7333 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/constraints/constraints.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.200614 keras-3.3.1/keras/src/datasets/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      383 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2644 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/boston_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3850 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/california_housing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      704 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/cifar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3086 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/cifar10.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2914 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/cifar100.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2929 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/fashion_mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7149 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/imdb.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2393 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/mnist.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7203 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/datasets/reuters.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.200910 keras-3.3.1/keras/src/distribution/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      718 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/distribution/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    31207 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/distribution/distribution_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.201204 keras-3.3.1/keras/src/dtype_policies/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3506 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/dtype_policies/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12480 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/dtype_policies/dtype_policy.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.201812 keras-3.3.1/keras/src/export/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       54 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/export/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32830 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/export/export_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.202965 keras-3.3.1/keras/src/initializers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3958 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/initializers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4884 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/initializers/constant_initializers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2633 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/initializers/initializer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23462 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/initializers/random_initializers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.203498 keras-3.3.1/keras/src/layers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8848 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/__init__.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.204724 keras-3.3.1/keras/src/layers/activations/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      272 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1236 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/activation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      809 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/elu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1900 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/leaky_relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3453 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/prelu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2670 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/relu.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2258 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/activations/softmax.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.205518 keras-3.3.1/keras/src/layers/attention/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/attention/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4330 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/attention/additive_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11889 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/attention/attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17952 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/attention/grouped_query_attention.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28353 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/attention/multi_head_attention.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.207929 keras-3.3.1/keras/src/layers/convolutional/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17263 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/layers/convolutional/base_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10695 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/base_conv_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11617 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/base_depthwise_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12643 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/base_separable_conv.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5571 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv1d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5670 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5691 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv2d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5893 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5897 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/conv3d_transpose.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5999 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/depthwise_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6087 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/depthwise_conv2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6450 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/separable_conv1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6531 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/convolutional/separable_conv2d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.209325 keras-3.3.1/keras/src/layers/core/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25345 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/layers/core/dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    42181 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/layers/core/einsum_dense.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17364 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/layers/core/embedding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      817 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/identity.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5107 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/input_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8989 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/lambda_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2629 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/masking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1535 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/core/wrapper.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9827 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/input_spec.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    63788 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/layers/layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.210872 keras-3.3.1/keras/src/layers/merging/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2150 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/add.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/average.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9249 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/base_merge.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6586 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/concatenate.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    12807 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/dot.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2214 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/maximum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2212 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/minimum.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2211 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/multiply.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2684 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/merging/subtract.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.211955 keras-3.3.1/keras/src/layers/normalization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13440 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/batch_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8534 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/group_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9836 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/layer_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4306 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/spectral_normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1831 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/normalization/unit_normalization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.214174 keras-3.3.1/keras/src/layers/pooling/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3344 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4150 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3235 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1460 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/base_global_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2425 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/base_pooling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3131 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_average_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2469 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_average_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2603 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_average_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2357 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2451 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2585 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/global_max_pooling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3343 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/max_pooling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4125 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/max_pooling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3225 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/pooling/max_pooling3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.220304 keras-3.3.1/keras/src/layers/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14572 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/audio_preprocessing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8705 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/category_encoding.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5489 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/center_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13145 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/discretization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29613 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/feature_space.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8317 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/hashed_crossing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10936 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/hashing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    41399 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/index_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18458 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/integer_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13920 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/normalization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6463 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_brightness.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3814 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_contrast.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6315 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_crop.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3805 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_flip.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9645 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_rotation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10614 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_translation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10820 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/random_zoom.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2177 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/rescaling.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5349 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/resizing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17734 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/string_lookup.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27820 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/text_vectorization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2133 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/preprocessing/tf_data_layer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.221416 keras-3.3.1/keras/src/layers/regularization/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1198 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/activity_regularization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3594 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/alpha_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2978 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2041 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/gaussian_dropout.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2089 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/gaussian_noise.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7300 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/regularization/spatial_dropout.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.223554 keras-3.3.1/keras/src/layers/reshaping/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2760 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/cropping1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9044 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/cropping2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11265 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/cropping3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3059 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/flatten.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2087 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/permute.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1335 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/repeat_vector.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2322 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/reshape.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1592 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/up_sampling1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5992 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/up_sampling2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4910 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/up_sampling3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2106 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/zero_padding1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4646 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/zero_padding2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5060 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/reshaping/zero_padding3d.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.226357 keras-3.3.1/keras/src/layers/rnn/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13203 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/bidirectional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27242 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/conv_lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8294 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/conv_lstm1d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8379 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/conv_lstm2d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8287 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/conv_lstm3d.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2132 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/dropout_rnn_cell.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27701 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/gru.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26544 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/lstm.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19159 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17537 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/simple_rnn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4943 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/stacked_rnn_cells.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4797 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/layers/rnn/time_distributed.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.227056 keras-3.3.1/keras/src/legacy/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    70241 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/backend.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8412 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/layers.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      523 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.227713 keras-3.3.1/keras/src/legacy/preprocessing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/preprocessing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    65545 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/preprocessing/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11172 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/preprocessing/sequence.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11110 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/preprocessing/text.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.228779 keras-3.3.1/keras/src/legacy/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7296 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/json_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22750 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/legacy_h5_format.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      485 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/saving_options.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9275 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/saving_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    21808 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/legacy/saving/serialization.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.229307 keras-3.3.1/keras/src/losses/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6363 2024-04-22 16:35:02.000000 keras-3.3.1/keras/src/losses/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5892 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/losses/loss.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    69132 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/losses/losses.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.232063 keras-3.3.1/keras/src/metrics/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7198 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15604 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/accuracy_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    61579 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/confusion_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11743 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/f_score_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3255 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/hinge_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26976 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/iou_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8186 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/metric.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26611 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/metrics_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10692 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/probabilistic_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7212 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/reduction_metrics.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19818 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/metrics/regression_metrics.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.233178 keras-3.3.1/keras/src/models/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      143 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/models/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11094 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/models/cloning.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    32453 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/models/functional.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    23789 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/models/model.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13013 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/models/sequential.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2164 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/models/variable_mapping.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.237655 keras-3.3.1/keras/src/ops/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      644 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    22866 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/core.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15334 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/function.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    37256 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/image.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    18342 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/linalg.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    30618 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/math.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    64046 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/ops/nn.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5583 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/node.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)   197331 2024-04-22 20:22:03.000000 keras-3.3.1/keras/src/ops/numpy.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10732 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/operation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13759 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/operation_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1694 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/ops/symbolic_arguments.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.239962 keras-3.3.1/keras/src/optimizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3931 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4759 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adadelta.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7637 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adafactor.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3918 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adagrad.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5909 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5083 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adamax.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3784 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/adamw.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    40410 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/base_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9099 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/ftrl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4969 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/lion.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11553 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/loss_scale_optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5926 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/nadam.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      813 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/optimizer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6003 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/rmsprop.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.240259 keras-3.3.1/keras/src/optimizers/schedules/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      546 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/schedules/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    35507 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/schedules/learning_rate_schedule.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4556 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/optimizers/sgd.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.240568 keras-3.3.1/keras/src/quantizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1784 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/quantizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4810 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/quantizers/quantizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.241379 keras-3.3.1/keras/src/random/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      420 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/random/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    13438 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/random/random.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4905 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/random/seed_generator.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.241868 keras-3.3.1/keras/src/regularizers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1731 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/regularizers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11799 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/regularizers/regularizers.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.242676 keras-3.3.1/keras/src/saving/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      614 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/saving/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     7358 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/saving/object_registration.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9737 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/saving/saving_api.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27008 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/saving/saving_lib.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    29052 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/saving/serialization_lib.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.243154 keras-3.3.1/keras/src/testing/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      266 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/testing/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    27552 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/testing/test_case.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     6197 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/testing/test_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.243772 keras-3.3.1/keras/src/trainers/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        0 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    25940 2024-04-22 17:46:41.000000 keras-3.3.1/keras/src/trainers/compile_utils.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.245334 keras-3.3.1/keras/src/trainers/data_adapters/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5423 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14323 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/array_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    17071 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/array_slicing.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3101 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9717 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/data_adapter_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2863 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/generator_data_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    19412 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/py_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5224 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2643 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3923 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/trainers/epoch_iterator.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    46449 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/trainers/trainer.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.245969 keras-3.3.1/keras/src/tree/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      521 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/tree/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4970 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/tree/dmtree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    11138 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/tree/optree_impl.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9397 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/tree/tree_api.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.250881 keras-3.3.1/keras/src/utils/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1423 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/__init__.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     2876 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/argument_validation.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14664 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/audio_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4130 2024-04-20 18:16:39.000000 keras-3.3.1/keras/src/utils/backend_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1442 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/code_stats.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    28554 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1483 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/dtype_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16371 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/file_utils.py
+-rwxr-xr-x   0 fchollet (337002) primarygroup (89939)    16538 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/image_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    16544 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/image_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     3491 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/io_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    26570 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/jax_layer.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      263 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/jax_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    15635 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/model_visualization.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1276 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/module_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1776 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/naming.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4571 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/numerical_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10349 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/progbar.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4003 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/python_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1677 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/rng_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4714 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/sequence_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    14512 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/summary_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    10509 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/text_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4630 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/tf_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     9842 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/timeseries_dataset_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     4991 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/torch_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8997 2024-04-20 16:30:07.000000 keras-3.3.1/keras/src/utils/traceback_utils.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     8980 2024-04-21 17:38:44.000000 keras-3.3.1/keras/src/utils/tracking.py
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)      189 2024-04-22 22:42:10.000000 keras-3.3.1/keras/src/version.py
+drwxr-xr-x   0 fchollet (337002) primarygroup (89939)        0 2024-04-22 22:42:13.251194 keras-3.3.1/keras.egg-info/
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     5731 2024-04-22 22:42:13.000000 keras-3.3.1/keras.egg-info/PKG-INFO
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)    20291 2024-04-22 22:42:13.000000 keras-3.3.1/keras.egg-info/SOURCES.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        1 2024-04-22 22:42:13.000000 keras-3.3.1/keras.egg-info/dependency_links.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       47 2024-04-22 22:42:13.000000 keras-3.3.1/keras.egg-info/requires.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)        6 2024-04-22 22:42:13.000000 keras-3.3.1/keras.egg-info/top_level.txt
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)       38 2024-04-22 22:42:13.251909 keras-3.3.1/setup.cfg
+-rw-r--r--   0 fchollet (337002) primarygroup (89939)     1769 2024-04-22 22:42:06.000000 keras-3.3.1/setup.py
```

### Comparing `keras-3.3.0/PKG-INFO` & `keras-3.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.3.0
+Version: 3.3.1
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras-3.3.0/README.md` & `keras-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/__init__.py` & `keras-3.3.1/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
-from keras.api import _tf_keras
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
```

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/__init__.py` & `keras-3.3.1/keras/api/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """DO NOT EDIT.
 
 This file was autogenerated. Do not edit it by hand,
 since your modifications would be overwritten.
 """
 
+
 from keras.api import activations
 from keras.api import applications
 from keras.api import backend
 from keras.api import callbacks
 from keras.api import config
 from keras.api import constraints
 from keras.api import datasets
```

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/activations/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/applications/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/applications/convnext/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/backend/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/callbacks/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/config/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/constraints/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/distribution/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/dtype_policies/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/initializers/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/layers/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/losses/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/metrics/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/mixed_precision/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/ops/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/ops/linalg/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/ops/nn/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/ops/numpy/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/legacy/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/optimizers/schedules/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/quantizers/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/random/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/regularizers/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/saving/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/tree/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/_tf_keras/keras/utils/__init__.py` & `keras-3.3.1/keras/_tf_keras/keras/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/activations/__init__.py` & `keras-3.3.1/keras/api/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/applications/__init__.py` & `keras-3.3.1/keras/api/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/applications/convnext/__init__.py` & `keras-3.3.1/keras/api/applications/convnext/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/applications/efficientnet/__init__.py` & `keras-3.3.1/keras/api/applications/efficientnet/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/applications/efficientnet_v2/__init__.py` & `keras-3.3.1/keras/api/applications/efficientnet_v2/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/backend/__init__.py` & `keras-3.3.1/keras/api/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/callbacks/__init__.py` & `keras-3.3.1/keras/api/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/config/__init__.py` & `keras-3.3.1/keras/api/config/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/constraints/__init__.py` & `keras-3.3.1/keras/api/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/distribution/__init__.py` & `keras-3.3.1/keras/api/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/dtype_policies/__init__.py` & `keras-3.3.1/keras/api/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/initializers/__init__.py` & `keras-3.3.1/keras/api/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/layers/__init__.py` & `keras-3.3.1/keras/api/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/losses/__init__.py` & `keras-3.3.1/keras/api/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/metrics/__init__.py` & `keras-3.3.1/keras/api/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/mixed_precision/__init__.py` & `keras-3.3.1/keras/api/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/ops/__init__.py` & `keras-3.3.1/keras/api/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/ops/linalg/__init__.py` & `keras-3.3.1/keras/api/ops/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/ops/nn/__init__.py` & `keras-3.3.1/keras/api/ops/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/ops/numpy/__init__.py` & `keras-3.3.1/keras/api/ops/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/optimizers/__init__.py` & `keras-3.3.1/keras/api/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/optimizers/legacy/__init__.py` & `keras-3.3.1/keras/api/optimizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/optimizers/schedules/__init__.py` & `keras-3.3.1/keras/api/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/quantizers/__init__.py` & `keras-3.3.1/keras/api/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/random/__init__.py` & `keras-3.3.1/keras/api/random/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/regularizers/__init__.py` & `keras-3.3.1/keras/api/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/saving/__init__.py` & `keras-3.3.1/keras/api/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/tree/__init__.py` & `keras-3.3.1/keras/api/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/api/utils/__init__.py` & `keras-3.3.1/keras/api/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/__init__.py` & `keras-3.3.1/keras/src/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/activations/__init__.py` & `keras-3.3.1/keras/src/activations/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/activations/activations.py` & `keras-3.3.1/keras/src/activations/activations.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/api_export.py` & `keras-3.3.1/keras/src/api_export.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/convnext.py` & `keras-3.3.1/keras/src/applications/convnext.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/densenet.py` & `keras-3.3.1/keras/src/applications/densenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/efficientnet.py` & `keras-3.3.1/keras/src/applications/efficientnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/efficientnet_v2.py` & `keras-3.3.1/keras/src/applications/efficientnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/imagenet_utils.py` & `keras-3.3.1/keras/src/applications/imagenet_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/inception_resnet_v2.py` & `keras-3.3.1/keras/src/applications/inception_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/inception_v3.py` & `keras-3.3.1/keras/src/applications/inception_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/mobilenet.py` & `keras-3.3.1/keras/src/applications/mobilenet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/mobilenet_v2.py` & `keras-3.3.1/keras/src/applications/mobilenet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/mobilenet_v3.py` & `keras-3.3.1/keras/src/applications/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/nasnet.py` & `keras-3.3.1/keras/src/applications/nasnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/resnet.py` & `keras-3.3.1/keras/src/applications/resnet.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/resnet_v2.py` & `keras-3.3.1/keras/src/applications/resnet_v2.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/vgg16.py` & `keras-3.3.1/keras/src/applications/vgg16.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/vgg19.py` & `keras-3.3.1/keras/src/applications/vgg19.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/applications/xception.py` & `keras-3.3.1/keras/src/applications/xception.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/__init__.py` & `keras-3.3.1/keras/src/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/__init__.py` & `keras-3.3.1/keras/src/backend/common/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/backend_utils.py` & `keras-3.3.1/keras/src/backend/common/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/dtypes.py` & `keras-3.3.1/keras/src/backend/common/dtypes.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/global_state.py` & `keras-3.3.1/keras/src/backend/common/global_state.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/keras_tensor.py` & `keras-3.3.1/keras/src/backend/common/keras_tensor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/name_scope.py` & `keras-3.3.1/keras/src/backend/common/name_scope.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/stateless_scope.py` & `keras-3.3.1/keras/src/backend/common/stateless_scope.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/common/variables.py` & `keras-3.3.1/keras/src/backend/common/variables.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/config.py` & `keras-3.3.1/keras/src/backend/config.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/exports.py` & `keras-3.3.1/keras/src/backend/exports.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/__init__.py` & `keras-3.3.1/keras/src/backend/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/core.py` & `keras-3.3.1/keras/src/backend/jax/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/distribution_lib.py` & `keras-3.3.1/keras/src/backend/jax/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/image.py` & `keras-3.3.1/keras/src/backend/jax/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/linalg.py` & `keras-3.3.1/keras/src/backend/jax/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/math.py` & `keras-3.3.1/keras/src/backend/jax/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/nn.py` & `keras-3.3.1/keras/src/backend/jax/nn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/numpy.py` & `keras-3.3.1/keras/src/backend/jax/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1158,7 +1158,11 @@
     x1 = convert_to_tensor(x1)
     x2 = convert_to_tensor(x2)
     return jnp.correlate(x1, x2, mode)
 
 
 def select(condlist, choicelist, default=0):
     return jnp.select(condlist, choicelist, default=default)
+
+
+def argpartition(x, kth, axis=-1):
+    return jnp.argpartition(x, kth, axis)
```

### Comparing `keras-3.3.0/keras/src/backend/jax/optimizer.py` & `keras-3.3.1/keras/src/backend/jax/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/random.py` & `keras-3.3.1/keras/src/backend/jax/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/rnn.py` & `keras-3.3.1/keras/src/backend/jax/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/sparse.py` & `keras-3.3.1/keras/src/backend/jax/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/jax/trainer.py` & `keras-3.3.1/keras/src/backend/jax/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/__init__.py` & `keras-3.3.1/keras/src/backend/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/core.py` & `keras-3.3.1/keras/src/backend/numpy/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/image.py` & `keras-3.3.1/keras/src/backend/numpy/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/linalg.py` & `keras-3.3.1/keras/src/backend/numpy/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/math.py` & `keras-3.3.1/keras/src/backend/numpy/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/nn.py` & `keras-3.3.1/keras/src/backend/numpy/nn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/numpy.py` & `keras-3.3.1/keras/src/backend/numpy/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1094,7 +1094,11 @@
     x1 = convert_to_tensor(x1, dtype)
     x2 = convert_to_tensor(x2, dtype)
     return np.correlate(x1, x2, mode)
 
 
 def select(condlist, choicelist, default=0):
     return np.select(condlist, choicelist, default=default)
+
+
+def argpartition(x, kth, axis=-1):
+    return np.argpartition(x, kth, axis)
```

### Comparing `keras-3.3.0/keras/src/backend/numpy/random.py` & `keras-3.3.1/keras/src/backend/numpy/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/rnn.py` & `keras-3.3.1/keras/src/backend/numpy/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/numpy/trainer.py` & `keras-3.3.1/keras/src/backend/numpy/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/__init__.py` & `keras-3.3.1/keras/src/backend/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/core.py` & `keras-3.3.1/keras/src/backend/tensorflow/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/distribution_lib.py` & `keras-3.3.1/keras/src/backend/tensorflow/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/image.py` & `keras-3.3.1/keras/src/backend/tensorflow/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/layer.py` & `keras-3.3.1/keras/src/backend/tensorflow/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/linalg.py` & `keras-3.3.1/keras/src/backend/tensorflow/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/math.py` & `keras-3.3.1/keras/src/backend/tensorflow/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/nn.py` & `keras-3.3.1/keras/src/backend/tensorflow/nn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/numpy.py` & `keras-3.3.1/keras/src/backend/tensorflow/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -2426,7 +2426,33 @@
     x2 = tf.reshape(x2, (x2_len, 1, 1))
 
     return tf.squeeze(tf.nn.conv1d(x1, x2, stride=1, padding=mode.upper()))
 
 
 def select(condlist, choicelist, default=0):
     return tf.experimental.numpy.select(condlist, choicelist, default=default)
+
+
+def argpartition(x, kth, axis=-1):
+    x = convert_to_tensor(x)
+
+    if standardize_dtype(x.dtype) not in ["int32", "int64"]:
+        x = tf.cast(x, tf.int32)
+
+    x = tf.experimental.numpy.swapaxes(x, axis, -1)
+    bottom_ind = tf.math.top_k(-x, kth + 1)[1]
+
+    def set_to_zero(args):
+        a, i = args
+        updates = tf.reshape(tf.zeros_like(i, dtype=tf.float32), [-1])
+        return tf.tensor_scatter_nd_update(a, i, updates)
+
+    for _ in range(x.ndim - 1):
+        set_to_zero = tf.vectorized_map(
+            set_to_zero, (tf.ones(tf.shape(x)), bottom_ind)
+        )
+    proxy = set_to_zero((tf.ones(tf.shape(x)), bottom_ind))
+
+    top_ind = tf.math.top_k(proxy, tf.shape(x)[-1] - kth - 1)[1]
+
+    out = tf.concat([bottom_ind, top_ind], axis=x.ndim - 1)
+    return tf.experimental.numpy.swapaxes(out, -1, axis)
```

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/optimizer.py` & `keras-3.3.1/keras/src/backend/tensorflow/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/random.py` & `keras-3.3.1/keras/src/backend/tensorflow/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/rnn.py` & `keras-3.3.1/keras/src/backend/tensorflow/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/sparse.py` & `keras-3.3.1/keras/src/backend/tensorflow/sparse.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/trackable.py` & `keras-3.3.1/keras/src/backend/tensorflow/trackable.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/tensorflow/trainer.py` & `keras-3.3.1/keras/src/backend/tensorflow/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/__init__.py` & `keras-3.3.1/keras/src/backend/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/core.py` & `keras-3.3.1/keras/src/backend/torch/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/image.py` & `keras-3.3.1/keras/src/backend/torch/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/layer.py` & `keras-3.3.1/keras/src/backend/torch/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/linalg.py` & `keras-3.3.1/keras/src/backend/torch/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/math.py` & `keras-3.3.1/keras/src/backend/torch/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/nn.py` & `keras-3.3.1/keras/src/backend/torch/nn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/numpy.py` & `keras-3.3.1/keras/src/backend/torch/numpy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1604,7 +1604,27 @@
 def select(condlist, choicelist, default=0):
     condlist = [convert_to_tensor(c) for c in condlist]
     choicelist = [convert_to_tensor(c) for c in choicelist]
     out = convert_to_tensor(default)
     for c, v in reversed(list(zip(condlist, choicelist))):
         out = torch.where(c, v, out)
     return out
+
+
+def argpartition(x, kth, axis=-1):
+    x = convert_to_tensor(x)
+
+    x = torch.transpose(x, axis, -1)
+    bottom_ind = torch.topk(-x, kth + 1)[1]
+
+    def set_to_zero(a, i):
+        a[i] = 0
+        return a
+
+    for _ in range(x.dim() - 1):
+        set_to_zero = torch.vmap(set_to_zero)
+    proxy = set_to_zero(torch.ones(x.shape), bottom_ind)
+
+    top_ind = torch.topk(proxy, x.shape[-1] - kth - 1)[1]
+
+    out = torch.cat([bottom_ind, top_ind], dim=x.dim() - 1)
+    return torch.transpose(out, -1, axis)
```

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adadelta.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_adadelta.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adagrad.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adam.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_adamax.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_adamax.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_lion.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_lion.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_nadam.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_optimizer.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_parallel_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_rmsprop.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/optimizers/torch_sgd.py` & `keras-3.3.1/keras/src/backend/torch/optimizers/torch_sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/random.py` & `keras-3.3.1/keras/src/backend/torch/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/rnn.py` & `keras-3.3.1/keras/src/backend/torch/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/backend/torch/trainer.py` & `keras-3.3.1/keras/src/backend/torch/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/__init__.py` & `keras-3.3.1/keras/src/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/backup_and_restore.py` & `keras-3.3.1/keras/src/callbacks/backup_and_restore.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/callback.py` & `keras-3.3.1/keras/src/callbacks/callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/callback_list.py` & `keras-3.3.1/keras/src/callbacks/callback_list.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/csv_logger.py` & `keras-3.3.1/keras/src/callbacks/csv_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/early_stopping.py` & `keras-3.3.1/keras/src/callbacks/early_stopping.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/history.py` & `keras-3.3.1/keras/src/callbacks/history.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/lambda_callback.py` & `keras-3.3.1/keras/src/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/learning_rate_scheduler.py` & `keras-3.3.1/keras/src/callbacks/learning_rate_scheduler.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/model_checkpoint.py` & `keras-3.3.1/keras/src/callbacks/model_checkpoint.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/progbar_logger.py` & `keras-3.3.1/keras/src/callbacks/progbar_logger.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau.py` & `keras-3.3.1/keras/src/callbacks/reduce_lr_on_plateau.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/reduce_lr_on_plateau_test.py` & `keras-3.3.1/keras/src/optimizers/adadelta.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,139 +1,139 @@
-import pytest
-
-from keras.src import callbacks
-from keras.src import layers
-from keras.src import optimizers
-from keras.src import testing
-from keras.src.models import Sequential
-from keras.src.testing import test_utils
-from keras.src.utils import io_utils
-from keras.src.utils import numerical_utils
-
-
-class ReduceLROnPlateauTest(testing.TestCase):
-    def setUp(self):
-        (x_train, y_train), (x_test, y_test) = test_utils.get_test_data(
-            train_samples=10,
-            test_samples=10,
-            input_shape=(3,),
-            num_classes=2,
-        )
-        y_test = numerical_utils.to_categorical(y_test)
-        y_train = numerical_utils.to_categorical(y_train)
-
-        model = Sequential([layers.Dense(5), layers.Dense(2)])
-
-        model.compile(
-            loss="mse",
-            optimizer=optimizers.Adam(0.1),
-        )
-
-        self.model = model
-        self.x_train = x_train
-        self.x_test = x_test
-        self.y_train = y_train
-        self.y_test = y_test
-
-    @pytest.mark.requires_trainable_backend
-    def test_reduces_lr_with_model_fit(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100
-        )
-
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=2,
-        )
-
-        self.assertEqual(self.model.optimizer.learning_rate.value, 0.01)
-
-    @pytest.mark.requires_trainable_backend
-    def test_throws_when_optimizer_has_schedule(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100
-        )
+from keras.src import ops
+from keras.src.api_export import keras_export
+from keras.src.optimizers import optimizer
+
+
+@keras_export(["keras.optimizers.Adadelta"])
+class Adadelta(optimizer.Optimizer):
+    """Optimizer that implements the Adadelta algorithm.
+
+    Adadelta optimization is a stochastic gradient descent method that is based
+    on adaptive learning rate per dimension to address two drawbacks:
+
+    - The continual decay of learning rates throughout training.
+    - The need for a manually selected global learning rate.
+
+    Adadelta is a more robust extension of Adagrad that adapts learning rates
+    based on a moving window of gradient updates, instead of accumulating all
+    past gradients. This way, Adadelta continues learning even when many updates
+    have been done. Compared to Adagrad, in the original version of Adadelta you
+    don't have to set an initial learning rate. In this version, the initial
+    learning rate can be set, as in most other Keras optimizers.
+
+    Args:
+        learning_rate: A float, a
+            `keras.optimizers.schedules.LearningRateSchedule` instance, or
+            a callable that takes no arguments and returns the actual value to
+            use. The learning rate. Defaults to `0.001`. Note that `Adadelta`
+            tends to benefit from higher initial learning rate values compared
+            to other optimizers. To match the exact form in the original paper,
+            use 1.0.
+        rho: A floating point value. The decay rate. Defaults to `0.95`.
+        epsilon: Small floating point value for maintaining numerical stability.
+        {{base_optimizer_keyword_args}}
+
+    Reference:
+
+    - [Zeiler, 2012](http://arxiv.org/abs/1212.5701)
+    """
+
+    def __init__(
+        self,
+        learning_rate=0.001,
+        rho=0.95,
+        epsilon=1e-7,
+        weight_decay=None,
+        clipnorm=None,
+        clipvalue=None,
+        global_clipnorm=None,
+        use_ema=False,
+        ema_momentum=0.99,
+        ema_overwrite_frequency=None,
+        loss_scale_factor=None,
+        gradient_accumulation_steps=None,
+        name="adadelta",
+        **kwargs,
+    ):
+        super().__init__(
+            learning_rate=learning_rate,
+            weight_decay=weight_decay,
+            clipnorm=clipnorm,
+            clipvalue=clipvalue,
+            global_clipnorm=global_clipnorm,
+            use_ema=use_ema,
+            ema_momentum=ema_momentum,
+            ema_overwrite_frequency=ema_overwrite_frequency,
+            loss_scale_factor=loss_scale_factor,
+            gradient_accumulation_steps=gradient_accumulation_steps,
+            name=name,
+            **kwargs,
+        )
+        self.rho = rho
+        self.epsilon = epsilon
+
+    def build(self, var_list):
+        if self.built:
+            return
+        super().build(var_list)
+        self._accumulated_grads = []
+        self._accumulated_delta_vars = []
+        for var in var_list:
+            self._accumulated_grads.append(
+                self.add_variable_from_reference(var, "accumulated_grad")
+            )
+            self._accumulated_delta_vars.append(
+                self.add_variable_from_reference(var, "accumulated_delta_var")
+            )
 
-        self.model.compile(
-            loss="mse",
-            optimizer=optimizers.Adam(
-                optimizers.schedules.PolynomialDecay(
-                    initial_learning_rate=0.1, decay_steps=10
-                )
+    def update_step(self, grad, variable, learning_rate):
+        """Update step given gradient and the associated model variable."""
+        lr = ops.cast(learning_rate, variable.dtype)
+        grad = ops.cast(grad, variable.dtype)
+
+        rho = self.rho
+        accumulated_grad = self._accumulated_grads[
+            self._get_variable_index(variable)
+        ]
+        accumulated_delta_var = self._accumulated_delta_vars[
+            self._get_variable_index(variable)
+        ]
+
+        def rms(x):
+            return ops.sqrt(ops.add(x, self.epsilon))
+
+        self.assign(
+            accumulated_grad,
+            ops.add(
+                rho * accumulated_grad, ops.multiply(1 - rho, ops.square(grad))
             ),
         )
-
-        with self.assertRaisesRegex(
-            TypeError,
-            "This optimizer was created with a `LearningRateSchedule`",
-        ):
-            self.model.fit(
-                self.x_train,
-                self.y_train,
-                validation_data=(self.x_test, self.y_test),
-                callbacks=[reduce_lr],
-                epochs=2,
+        delta_var = ops.negative(
+            ops.divide(
+                ops.multiply(rms(accumulated_delta_var), grad),
+                rms(accumulated_grad),
             )
-
-    @pytest.mark.requires_trainable_backend
-    def test_verbose_logging(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1, factor=0.1, monitor="val_loss", min_delta=100, verbose=1
         )
-        io_utils.disable_interactive_logging()
-        io_utils.set_logging_verbosity("INFO")
-
-        with self.assertLogs() as logs:
-            self.model.fit(
-                self.x_train,
-                self.y_train,
-                validation_data=(self.x_test, self.y_test),
-                callbacks=[reduce_lr],
-                epochs=2,
-            )
-            expected_log = "ReduceLROnPlateau reducing learning rate to 0.01"
-            self.assertTrue(any(expected_log in log for log in logs.output))
-
-    @pytest.mark.requires_trainable_backend
-    def test_honors_min_lr(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1,
-            factor=0.1,
-            monitor="val_loss",
-            min_delta=10,
-            min_lr=0.005,
-        )
-
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=4,
+        self.assign(
+            accumulated_delta_var,
+            ops.add(
+                ops.multiply(rho, accumulated_delta_var),
+                ops.multiply(1 - rho, ops.square(delta_var)),
+            ),
         )
+        self.assign_add(variable, ops.multiply(lr, delta_var))
 
-        self.assertEqual(self.model.optimizer.learning_rate.value, 0.005)
+    def get_config(self):
+        config = super().get_config()
 
-    @pytest.mark.requires_trainable_backend
-    def test_cooldown(self):
-        reduce_lr = callbacks.ReduceLROnPlateau(
-            patience=1,
-            factor=0.1,
-            monitor="val_loss",
-            min_delta=100,
-            cooldown=2,
+        config.update(
+            {
+                "rho": self.rho,
+                "epsilon": self.epsilon,
+            }
         )
+        return config
 
-        self.model.fit(
-            self.x_train,
-            self.y_train,
-            validation_data=(self.x_test, self.y_test),
-            callbacks=[reduce_lr],
-            epochs=4,
-        )
 
-        # With a cooldown of 2 epochs, we should only reduce the LR every other
-        # epoch, so after 4 epochs we will have reduced 2 times.
-        self.assertAllClose(self.model.optimizer.learning_rate.value, 0.001)
+Adadelta.__doc__ = Adadelta.__doc__.replace(
+    "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
+)
```

### Comparing `keras-3.3.0/keras/src/callbacks/remote_monitor.py` & `keras-3.3.1/keras/src/callbacks/remote_monitor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/swap_ema_weights.py` & `keras-3.3.1/keras/src/callbacks/swap_ema_weights.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/tensorboard.py` & `keras-3.3.1/keras/src/callbacks/tensorboard.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/callbacks/terminate_on_nan.py` & `keras-3.3.1/keras/src/callbacks/terminate_on_nan.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/constraints/__init__.py` & `keras-3.3.1/keras/src/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/constraints/constraints.py` & `keras-3.3.1/keras/src/constraints/constraints.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/boston_housing.py` & `keras-3.3.1/keras/src/datasets/boston_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/california_housing.py` & `keras-3.3.1/keras/src/datasets/california_housing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/cifar.py` & `keras-3.3.1/keras/src/datasets/cifar.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/cifar10.py` & `keras-3.3.1/keras/src/datasets/cifar10.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/cifar100.py` & `keras-3.3.1/keras/src/datasets/cifar100.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/fashion_mnist.py` & `keras-3.3.1/keras/src/datasets/fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/imdb.py` & `keras-3.3.1/keras/src/datasets/imdb.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/mnist.py` & `keras-3.3.1/keras/src/datasets/mnist.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/datasets/reuters.py` & `keras-3.3.1/keras/src/datasets/reuters.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/distribution/__init__.py` & `keras-3.3.1/keras/src/distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/distribution/distribution_lib.py` & `keras-3.3.1/keras/src/distribution/distribution_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/dtype_policies/__init__.py` & `keras-3.3.1/keras/src/dtype_policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/dtype_policies/dtype_policy.py` & `keras-3.3.1/keras/src/dtype_policies/dtype_policy.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/export/export_lib.py` & `keras-3.3.1/keras/src/export/export_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/initializers/__init__.py` & `keras-3.3.1/keras/src/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/initializers/constant_initializers.py` & `keras-3.3.1/keras/src/initializers/constant_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/initializers/initializer.py` & `keras-3.3.1/keras/src/initializers/initializer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/initializers/random_initializers.py` & `keras-3.3.1/keras/src/initializers/random_initializers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/__init__.py` & `keras-3.3.1/keras/src/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/activation.py` & `keras-3.3.1/keras/src/layers/activations/activation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/elu.py` & `keras-3.3.1/keras/src/layers/activations/elu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/leaky_relu.py` & `keras-3.3.1/keras/src/layers/activations/leaky_relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/prelu.py` & `keras-3.3.1/keras/src/layers/activations/prelu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/relu.py` & `keras-3.3.1/keras/src/layers/activations/relu.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/activations/softmax.py` & `keras-3.3.1/keras/src/layers/activations/softmax.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/attention/additive_attention.py` & `keras-3.3.1/keras/src/layers/attention/additive_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/attention/attention.py` & `keras-3.3.1/keras/src/layers/attention/attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/attention/grouped_query_attention.py` & `keras-3.3.1/keras/src/layers/attention/grouped_query_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/attention/multi_head_attention.py` & `keras-3.3.1/keras/src/layers/attention/multi_head_attention.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/base_conv.py` & `keras-3.3.1/keras/src/layers/convolutional/base_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/base_conv_transpose.py` & `keras-3.3.1/keras/src/layers/convolutional/base_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/base_depthwise_conv.py` & `keras-3.3.1/keras/src/layers/convolutional/base_depthwise_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/base_separable_conv.py` & `keras-3.3.1/keras/src/layers/convolutional/base_separable_conv.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv1d.py` & `keras-3.3.1/keras/src/layers/convolutional/conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv1d_transpose.py` & `keras-3.3.1/keras/src/layers/convolutional/conv1d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv2d.py` & `keras-3.3.1/keras/src/layers/convolutional/conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv2d_transpose.py` & `keras-3.3.1/keras/src/layers/convolutional/conv2d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv3d.py` & `keras-3.3.1/keras/src/layers/convolutional/conv3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/conv3d_transpose.py` & `keras-3.3.1/keras/src/layers/convolutional/conv3d_transpose.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/depthwise_conv1d.py` & `keras-3.3.1/keras/src/layers/convolutional/depthwise_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/depthwise_conv2d.py` & `keras-3.3.1/keras/src/layers/convolutional/depthwise_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/separable_conv1d.py` & `keras-3.3.1/keras/src/layers/convolutional/separable_conv1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/convolutional/separable_conv2d.py` & `keras-3.3.1/keras/src/layers/convolutional/separable_conv2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/dense.py` & `keras-3.3.1/keras/src/layers/core/dense.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/dense_test.py` & `keras-3.3.1/keras/src/testing/test_case.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,734 +1,689 @@
-import os
+import json
+import shutil
+import tempfile
+import unittest
 
 import numpy as np
-import pytest
-from absl.testing import parameterized
 
 from keras.src import backend
-from keras.src import constraints
-from keras.src import layers
-from keras.src import models
+from keras.src import distribution
 from keras.src import ops
-from keras.src import optimizers
-from keras.src import random
-from keras.src import saving
-from keras.src import testing
-from keras.src.backend.common import keras_tensor
-from keras.src.export import export_lib
-
-
-class DenseTest(testing.TestCase, parameterized.TestCase):
-    @pytest.mark.requires_trainable_backend
-    def test_dense_basics(self):
-        # 2D case, no bias.
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 4,
-                "activation": "relu",
-                "kernel_initializer": "random_uniform",
-                "bias_initializer": "ones",
-                "use_bias": False,
-            },
-            input_shape=(2, 3),
-            expected_output_shape=(2, 4),
-            expected_num_trainable_weights=1,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
-        )
-        # 3D case, some regularizers.
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "activation": "sigmoid",
-                "kernel_regularizer": "l2",
-                "bias_regularizer": "l2",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=2,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=2,  # we have 2 regularizers.
-            supports_masking=True,
-        )
-
-    def test_dense_correctness(self):
-        # With bias and activation.
-        layer = layers.Dense(units=2, activation="relu")
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-                np.array([5.0, -6.0]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertAllClose(layer(inputs), [[10.0, 0.0]])
-
-        # Just a kernel matmul.
-        layer = layers.Dense(units=2, use_bias=False)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
-
-    def test_dense_errors(self):
-        with self.assertRaisesRegex(ValueError, "incompatible with the layer"):
-            layer = layers.Dense(units=2, activation="relu")
-            layer(keras_tensor.KerasTensor((1, 2)))
-            layer(keras_tensor.KerasTensor((1, 3)))
-
-    @pytest.mark.skipif(
-        not backend.SUPPORTS_SPARSE_TENSORS,
-        reason="Backend does not support sparse tensors.",
-    )
-    def test_dense_sparse(self):
-        import tensorflow as tf
-
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 4,
-            },
-            input_shape=(2, 3),
-            input_sparse=True,
-            expected_output_shape=(2, 4),
-            expected_num_trainable_weights=2,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-        )
-
-        inputs = 4 * backend.random.uniform((10, 10))
-        inputs = tf.sparse.from_dense(tf.nn.dropout(inputs, 0.8))
-
-        inputs = np.random.random((10, 10)).astype("float32")
-        inputs = np.multiply(inputs, inputs >= 0.8)
-
-        if backend.backend() == "tensorflow":
+from keras.src import tree
+from keras.src import utils
+from keras.src.backend.common import is_float_dtype
+from keras.src.backend.common import standardize_dtype
+from keras.src.backend.common.global_state import clear_session
+from keras.src.backend.common.keras_tensor import KerasTensor
+from keras.src.models import Model
+from keras.src.utils import traceback_utils
+
+
+class TestCase(unittest.TestCase):
+    maxDiff = None
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+    def setUp(self):
+        # clear global state so that test cases are independent
+        # required for the jit enabled torch tests since dynamo has
+        # a global cache for guards, compiled fn, etc
+        clear_session(free_memory=False)
+        if traceback_utils.is_traceback_filtering_enabled():
+            traceback_utils.disable_traceback_filtering()
+
+    def get_temp_dir(self):
+        temp_dir = tempfile.mkdtemp()
+        self.addCleanup(lambda: shutil.rmtree(temp_dir))
+        return temp_dir
+
+    def assertAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
+        if not isinstance(x1, np.ndarray):
+            x1 = backend.convert_to_numpy(x1)
+        if not isinstance(x2, np.ndarray):
+            x2 = backend.convert_to_numpy(x2)
+        np.testing.assert_allclose(x1, x2, atol=atol, rtol=rtol)
+
+    def assertNotAllClose(self, x1, x2, atol=1e-6, rtol=1e-6, msg=None):
+        try:
+            self.assertAllClose(x1, x2, atol=atol, rtol=rtol, msg=msg)
+        except AssertionError:
+            return
+        msg = msg or ""
+        raise AssertionError(
+            f"The two values are close at all elements. \n"
+            f"{msg}.\n"
+            f"Values: {x1}"
+        )
+
+    def assertAlmostEqual(self, x1, x2, decimal=3, msg=None):
+        if not isinstance(x1, np.ndarray):
+            x1 = backend.convert_to_numpy(x1)
+        if not isinstance(x2, np.ndarray):
+            x2 = backend.convert_to_numpy(x2)
+        np.testing.assert_almost_equal(x1, x2, decimal=decimal)
+
+    def assertAllEqual(self, x1, x2, msg=None):
+        self.assertEqual(len(x1), len(x2), msg=msg)
+        for e1, e2 in zip(x1, x2):
+            if isinstance(e1, (list, tuple)) or isinstance(e2, (list, tuple)):
+                self.assertAllEqual(e1, e2, msg=msg)
+            else:
+                e1 = backend.convert_to_numpy(e1)
+                e2 = backend.convert_to_numpy(e2)
+                self.assertEqual(e1, e2, msg=msg)
+
+    def assertLen(self, iterable, expected_len, msg=None):
+        self.assertEqual(len(iterable), expected_len, msg=msg)
+
+    def assertSparse(self, x, sparse=True):
+        if isinstance(x, KerasTensor):
+            self.assertEqual(x.sparse, sparse)
+        elif backend.backend() == "tensorflow":
             import tensorflow as tf
 
-            inputs = tf.sparse.from_dense(inputs)
+            if sparse:
+                self.assertIsInstance(x, tf.SparseTensor)
+            else:
+                self.assertNotIsInstance(x, tf.SparseTensor)
         elif backend.backend() == "jax":
             import jax.experimental.sparse as jax_sparse
 
-            inputs = jax_sparse.BCOO.fromdense(inputs)
+            if sparse:
+                self.assertIsInstance(x, jax_sparse.JAXSparse)
+            else:
+                self.assertNotIsInstance(x, jax_sparse.JAXSparse)
         else:
-            self.fail(f"Sparse is unsupported with backend {backend.backend()}")
-
-        layer = layers.Dense(units=10)
-        outputs = layer(inputs)
-
-        # Verify the computation is the same as if it had been a dense tensor
-        expected_outputs = ops.add(
-            ops.matmul(
-                backend.convert_to_tensor(inputs, sparse=False), layer.kernel
-            ),
-            layer.bias,
-        )
-        self.assertAllClose(outputs, expected_outputs)
+            self.assertFalse(
+                sparse,
+                f"Backend {backend.backend()} does not support sparse tensors",
+            )
+
+    def run_class_serialization_test(self, instance, custom_objects=None):
+        from keras.src.saving import custom_object_scope
+        from keras.src.saving import deserialize_keras_object
+        from keras.src.saving import serialize_keras_object
+
+        # get_config roundtrip
+        cls = instance.__class__
+        config = instance.get_config()
+        config_json = json.dumps(config, sort_keys=True, indent=4)
+        ref_dir = dir(instance)[:]
+        with custom_object_scope(custom_objects):
+            revived_instance = cls.from_config(config)
+        revived_config = revived_instance.get_config()
+        revived_config_json = json.dumps(
+            revived_config, sort_keys=True, indent=4
+        )
+        self.assertEqual(config_json, revived_config_json)
+        self.assertEqual(set(ref_dir), set(dir(revived_instance)))
+
+        # serialization roundtrip
+        serialized = serialize_keras_object(instance)
+        serialized_json = json.dumps(serialized, sort_keys=True, indent=4)
+        with custom_object_scope(custom_objects):
+            revived_instance = deserialize_keras_object(
+                json.loads(serialized_json)
+            )
+        revived_config = revived_instance.get_config()
+        revived_config_json = json.dumps(
+            revived_config, sort_keys=True, indent=4
+        )
+        self.assertEqual(config_json, revived_config_json)
+        new_dir = dir(revived_instance)[:]
+        for lst in [ref_dir, new_dir]:
+            if "__annotations__" in lst:
+                lst.remove("__annotations__")
+        self.assertEqual(set(ref_dir), set(new_dir))
+        return revived_instance
+
+    def run_layer_test(
+        self,
+        layer_cls,
+        init_kwargs,
+        input_shape=None,
+        input_dtype=None,
+        input_sparse=False,
+        input_data=None,
+        call_kwargs=None,
+        expected_output_shape=None,
+        expected_output_dtype=None,
+        expected_output_sparse=False,
+        expected_output=None,
+        expected_num_trainable_weights=None,
+        expected_num_non_trainable_weights=None,
+        expected_num_non_trainable_variables=None,
+        expected_num_seed_generators=None,
+        expected_num_losses=None,
+        supports_masking=None,
+        expected_mask_shape=None,
+        custom_objects=None,
+        run_training_check=True,
+        run_mixed_precision_check=True,
+    ):
+        """Run basic checks on a layer.
 
-        # Verify the gradient is sparse
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
+        Args:
+            layer_cls: The class of the layer to test.
+            init_kwargs: Dict of arguments to be used to
+                instantiate the layer.
+            input_shape: Shape tuple (or list/dict of shape tuples)
+                to call the layer on.
+            input_dtype: Corresponding input dtype.
+            input_sparse: Whether the input is a sparse tensor (this requires
+                the backend to support sparse tensors).
+            input_data: Tensor (or list/dict of tensors)
+                to call the layer on.
+            call_kwargs: Dict of arguments to use when calling the
+                layer (does not include the first input tensor argument)
+            expected_output_shape: Shape tuple
+                (or list/dict of shape tuples)
+                expected as output.
+            expected_output_dtype: dtype expected as output.
+            expected_output_sparse: Whether the output is expected to be sparse
+                (this requires the backend to support sparse tensors).
+            expected_output: Expected output tensor -- only
+                to be specified if input_data is provided.
+            expected_num_trainable_weights: Expected number
+                of trainable weights of the layer once built.
+            expected_num_non_trainable_weights: Expected number
+                of non-trainable weights of the layer once built.
+            expected_num_seed_generators: Expected number of
+                SeedGenerators objects of the layer once built.
+            expected_num_losses: Expected number of loss tensors
+                produced when calling the layer.
+            supports_masking: If True, will check that the layer
+                supports masking.
+            expected_mask_shape: Expected mask shape tuple
+                returned by compute_mask() (only supports 1 shape).
+            custom_objects: Dict of any custom objects to be
+                considered during deserialization.
+            run_training_check: Whether to attempt to train the layer
+                (if an input shape or input data was provided).
+            run_mixed_precision_check: Whether to test the layer with a mixed
+                precision dtype policy.
+        """
+        if input_shape is not None and input_data is not None:
+            raise ValueError(
+                "input_shape and input_data cannot be passed "
+                "at the same time."
+            )
+        if expected_output_shape is not None and expected_output is not None:
+            raise ValueError(
+                "expected_output_shape and expected_output cannot be passed "
+                "at the same time."
+            )
+        if expected_output is not None and input_data is None:
+            raise ValueError(
+                "In order to use expected_output, input_data must be provided."
+            )
+        if expected_mask_shape is not None and supports_masking is not True:
+            raise ValueError(
+                "In order to use expected_mask_shape, supports_masking "
+                "must be True."
+            )
+
+        init_kwargs = init_kwargs or {}
+        call_kwargs = call_kwargs or {}
+
+        if input_shape is not None and input_dtype is not None:
+            if isinstance(input_shape, tuple) and is_shape_tuple(
+                input_shape[0]
+            ):
+                self.assertIsInstance(input_dtype, tuple)
+                self.assertEqual(
+                    len(input_shape),
+                    len(input_dtype),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif isinstance(input_shape, dict):
+                self.assertIsInstance(input_dtype, dict)
+                self.assertEqual(
+                    set(input_shape.keys()),
+                    set(input_dtype.keys()),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif isinstance(input_shape, list):
+                self.assertIsInstance(input_dtype, list)
+                self.assertEqual(
+                    len(input_shape),
+                    len(input_dtype),
+                    msg="The number of input shapes and dtypes does not match",
+                )
+            elif not isinstance(input_shape, tuple):
+                raise ValueError("The type of input_shape is not supported")
+        if input_shape is not None and input_dtype is None:
+            input_dtype = tree.map_shape_structure(
+                lambda _: "float32", input_shape
+            )
+
+        # Serialization test.
+        layer = layer_cls(**init_kwargs)
+        self.run_class_serialization_test(layer, custom_objects)
+
+        # Basic masking test.
+        if supports_masking is not None:
+            self.assertEqual(
+                layer.supports_masking,
+                supports_masking,
+                msg="Unexpected supports_masking value",
+            )
+
+        def run_build_asserts(layer):
+            self.assertTrue(layer.built)
+            if expected_num_trainable_weights is not None:
+                self.assertLen(
+                    layer.trainable_weights,
+                    expected_num_trainable_weights,
+                    msg="Unexpected number of trainable_weights",
+                )
+            if expected_num_non_trainable_weights is not None:
+                self.assertLen(
+                    layer.non_trainable_weights,
+                    expected_num_non_trainable_weights,
+                    msg="Unexpected number of non_trainable_weights",
+                )
+            if expected_num_non_trainable_variables is not None:
+                self.assertLen(
+                    layer.non_trainable_variables,
+                    expected_num_non_trainable_variables,
+                    msg="Unexpected number of non_trainable_variables",
+                )
+            if expected_num_seed_generators is not None:
+                self.assertLen(
+                    get_seed_generators(layer),
+                    expected_num_seed_generators,
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
+                )
 
-            with tf.GradientTape() as g:
-                outputs = layer(inputs)
+        def run_output_asserts(layer, output, eager=False):
+            if expected_output_shape is not None:
+                if isinstance(expected_output_shape, tuple) and is_shape_tuple(
+                    expected_output_shape[0]
+                ):
+                    self.assertIsInstance(output, tuple)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_shape),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_shape = tuple(v.shape for v in output)
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, tuple):
+                    self.assertEqual(
+                        expected_output_shape,
+                        output.shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, dict):
+                    self.assertIsInstance(output, dict)
+                    self.assertEqual(
+                        set(output.keys()),
+                        set(expected_output_shape.keys()),
+                        msg="Unexpected output dict keys",
+                    )
+                    output_shape = {k: v.shape for k, v in output.items()}
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                elif isinstance(expected_output_shape, list):
+                    self.assertIsInstance(output, list)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_shape),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_shape = [v.shape for v in output]
+                    self.assertEqual(
+                        expected_output_shape,
+                        output_shape,
+                        msg="Unexpected output shape",
+                    )
+                else:
+                    raise ValueError(
+                        "The type of expected_output_shape is not supported"
+                    )
+            if expected_output_dtype is not None:
+                if isinstance(expected_output_dtype, tuple):
+                    self.assertIsInstance(output, tuple)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_dtype),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_dtype = tuple(
+                        backend.standardize_dtype(v.dtype) for v in output
+                    )
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                elif isinstance(expected_output_dtype, dict):
+                    self.assertIsInstance(output, dict)
+                    self.assertEqual(
+                        set(output.keys()),
+                        set(expected_output_dtype.keys()),
+                        msg="Unexpected output dict keys",
+                    )
+                    output_dtype = {
+                        k: backend.standardize_dtype(v.dtype)
+                        for k, v in output.items()
+                    }
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                elif isinstance(expected_output_dtype, list):
+                    self.assertIsInstance(output, list)
+                    self.assertEqual(
+                        len(output),
+                        len(expected_output_dtype),
+                        msg="Unexpected number of outputs",
+                    )
+                    output_dtype = [
+                        backend.standardize_dtype(v.dtype) for v in output
+                    ]
+                    self.assertEqual(
+                        expected_output_dtype,
+                        output_dtype,
+                        msg="Unexpected output dtype",
+                    )
+                else:
+                    output_dtype = tree.flatten(output)[0].dtype
+                    self.assertEqual(
+                        expected_output_dtype,
+                        backend.standardize_dtype(output_dtype),
+                        msg="Unexpected output dtype",
+                    )
+            if expected_output_sparse:
+                for x in tree.flatten(output):
+                    self.assertSparse(x)
+            if eager:
+                if expected_output is not None:
+                    self.assertEqual(type(expected_output), type(output))
+                    for ref_v, v in zip(
+                        tree.flatten(expected_output), tree.flatten(output)
+                    ):
+                        self.assertAllClose(
+                            ref_v, v, msg="Unexpected output value"
+                        )
+                if expected_num_losses is not None:
+                    self.assertLen(layer.losses, expected_num_losses)
+
+        def run_training_step(layer, input_data, output_data):
+            class TestModel(Model):
+                def __init__(self, layer):
+                    super().__init__()
+                    self.layer = layer
+
+                def call(self, x, training=False):
+                    return self.layer(x, training=training)
+
+            model = TestModel(layer)
+
+            data = (input_data, output_data)
+            if backend.backend() == "torch":
+                data = tree.map_structure(backend.convert_to_numpy, data)
+
+            def data_generator():
+                while True:
+                    yield data
+
+            # test the "default" path for each backend by setting
+            # jit_compile="auto".
+            # for tensorflow and jax backends auto is jitted
+            # Note that tensorflow cannot be jitted with sparse tensors
+            # for torch backend auto is eager
+            #
+            # NB: for torch, jit_compile=True turns on torchdynamo
+            #  which may not always succeed in tracing depending
+            #  on the model. Run your program with these env vars
+            #  to get debug traces of dynamo:
+            #    TORCH_LOGS="+dynamo"
+            #    TORCHDYNAMO_VERBOSE=1
+            #    TORCHDYNAMO_REPORT_GUARD_FAILURES=1
+            jit_compile = "auto"
+            if backend.backend() == "tensorflow" and input_sparse:
+                jit_compile = False
+            model.compile(optimizer="sgd", loss="mse", jit_compile=jit_compile)
+            model.fit(data_generator(), steps_per_epoch=1, verbose=0)
+
+        # Build test.
+        if input_data is not None or input_shape is not None:
+            if input_shape is None:
+                build_shape = tree.map_structure(
+                    lambda x: ops.shape(x), input_data
+                )
+            else:
+                build_shape = input_shape
+            layer = layer_cls(**init_kwargs)
+            if isinstance(build_shape, dict):
+                layer.build(**build_shape)
+            else:
+                layer.build(build_shape)
+            run_build_asserts(layer)
+
+            # Symbolic call test.
+            if input_shape is None:
+                keras_tensor_inputs = tree.map_structure(
+                    lambda x: create_keras_tensors(
+                        ops.shape(x), x.dtype, input_sparse
+                    ),
+                    input_data,
+                )
+            else:
+                keras_tensor_inputs = create_keras_tensors(
+                    input_shape, input_dtype, input_sparse
+                )
+            layer = layer_cls(**init_kwargs)
+            if isinstance(keras_tensor_inputs, dict):
+                keras_tensor_outputs = layer(
+                    **keras_tensor_inputs, **call_kwargs
+                )
+            else:
+                keras_tensor_outputs = layer(keras_tensor_inputs, **call_kwargs)
+            run_build_asserts(layer)
+            run_output_asserts(layer, keras_tensor_outputs, eager=False)
+
+            if expected_mask_shape is not None:
+                output_mask = layer.compute_mask(keras_tensor_inputs)
+                self.assertEqual(expected_mask_shape, output_mask.shape)
+
+        # Eager call test and compiled training test.
+        if input_data is not None or input_shape is not None:
+            if input_data is None:
+                input_data = create_eager_tensors(
+                    input_shape, input_dtype, input_sparse
+                )
+            layer = layer_cls(**init_kwargs)
+            if isinstance(input_data, dict):
+                output_data = layer(**input_data, **call_kwargs)
+            else:
+                output_data = layer(input_data, **call_kwargs)
+            run_output_asserts(layer, output_data, eager=True)
+
+            if run_training_check:
+                run_training_step(layer, input_data, output_data)
+
+            # Never test mixed precision on torch CPU. Torch lacks support.
+            if run_mixed_precision_check and backend.backend() == "torch":
+                import torch
+
+                run_mixed_precision_check = torch.cuda.is_available()
+
+            if run_mixed_precision_check:
+                layer = layer_cls(**{**init_kwargs, "dtype": "mixed_float16"})
+                input_spec = tree.map_structure(
+                    lambda spec: KerasTensor(
+                        spec.shape,
+                        dtype=(
+                            layer.compute_dtype
+                            if layer.autocast
+                            and backend.is_float_dtype(spec.dtype)
+                            else spec.dtype
+                        ),
+                    ),
+                    keras_tensor_inputs,
+                )
+                if isinstance(input_data, dict):
+                    output_data = layer(**input_data, **call_kwargs)
+                    output_spec = layer.compute_output_spec(**input_spec)
+                else:
+                    output_data = layer(input_data, **call_kwargs)
+                    output_spec = layer.compute_output_spec(input_spec)
+                for tensor, spec in zip(
+                    tree.flatten(output_data), tree.flatten(output_spec)
+                ):
+                    dtype = standardize_dtype(tensor.dtype)
+                    self.assertEqual(dtype, spec.dtype)
+                for weight in layer.weights:
+                    dtype = standardize_dtype(weight.dtype)
+                    if is_float_dtype(dtype):
+                        self.assertEqual(dtype, "float32")
 
-            self.assertIsInstance(
-                g.gradient(outputs, layer.kernel), tf.IndexedSlices
-            )
 
-    def test_dense_no_activation(self):
-        layer = layers.Dense(units=2, use_bias=False, activation=None)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
+def tensorflow_uses_gpu():
+    return backend.backend() == "tensorflow" and uses_gpu()
 
-    def test_dense_without_activation_set(self):
-        layer = layers.Dense(units=2, use_bias=False)
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
-        layer.activation = None
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        self.assertEqual(layer.bias, None)
-        self.assertAllClose(layer(inputs), [[5.0, -6.0]])
 
-    def test_dense_with_activation(self):
-        layer = layers.Dense(units=2, use_bias=False, activation="relu")
-        layer.build((1, 2))
-        layer.set_weights(
-            [
-                np.array([[1.0, -2.0], [3.0, -4.0]]),
-            ]
-        )
+def jax_uses_gpu():
+    return backend.backend() == "jax" and uses_gpu()
 
-        inputs = np.array(
-            [[-1.0, 2.0]],
-        )
-        output = layer(inputs)
-        expected_output = np.array([[5.0, 0.0]])
-        self.assertAllClose(output, expected_output)
-
-    def test_dense_constraints(self):
-        layer = layers.Dense(units=2, kernel_constraint="non_neg")
-        layer.build((None, 2))
-        self.assertIsInstance(layer.kernel.constraint, constraints.NonNeg)
-        layer = layers.Dense(units=2, bias_constraint="non_neg")
-        layer.build((None, 2))
-        self.assertIsInstance(layer.bias.constraint, constraints.NonNeg)
-
-    @pytest.mark.requires_trainable_backend
-    def test_enable_lora(self):
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        self.assertLen(layer.trainable_weights, 3)
-        self.assertLen(layer.non_trainable_weights, 1)
-        if backend.backend() == "torch":
-            self.assertLen(layer.torch_params, 4)
-        # Try eager call
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        _ = layer(x[:2])
-
-        init_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        init_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-
-        # Try calling fit()
-        model = models.Sequential(
-            [
-                layer,
-            ]
-        )
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y)
 
-        final_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        final_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        diff_a = np.max(
-            np.abs(init_lora_a_kernel_value - final_lora_a_kernel_value)
-        )
-        diff_b = np.max(
-            np.abs(init_lora_b_kernel_value - final_lora_b_kernel_value)
-        )
-        self.assertGreater(diff_a, 0.0)
-        self.assertGreater(diff_b, 0.0)
+def torch_uses_gpu():
+    return backend.backend() == "torch" and uses_gpu()
 
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(self.get_temp_dir(), "lora_model.keras")
-        model.save(temp_filepath)
-
-        new_model = saving.load_model(temp_filepath)
-        self.assertTrue(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "lora_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
 
-        # Load the file into a fresh, non-lora model
-        new_model = models.Sequential(
-            [
-                layers.Dense(units=16),
-            ]
-        )
-        new_model.build((None, 8))
-        new_model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try loading a normal checkpoint into a lora model
-        new_model.save_weights(temp_filepath)
-        model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-    @pytest.mark.requires_trainable_backend
-    def test_lora_weight_name(self):
-
-        class MyModel(models.Model):
-            def __init__(self):
-                super().__init__(name="mymodel")
-                self.dense = layers.Dense(16, name="dense")
-
-            def build(self, input_shape):
-                self.dense.build(input_shape)
-
-            def call(self, x):
-                return self.dense(x)
-
-        model = MyModel()
-        model.build((None, 8))
-        model.dense.enable_lora(4)
-        self.assertEqual(
-            model.dense.lora_kernel_a.path, "mymodel/dense/lora_kernel_a"
-        )
+def uses_gpu():
+    # Condition used to skip tests when using the GPU
+    devices = distribution.list_devices()
+    if any(d.startswith("gpu") for d in devices):
+        return True
+    return False
 
-    @pytest.mark.requires_trainable_backend
-    def test_lora_rank_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "activation": "sigmoid",
-                "kernel_regularizer": "l2",
-                "lora_rank": 2,
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=3,
-            expected_num_non_trainable_weights=1,
-            expected_num_seed_generators=0,
-            expected_num_losses=2,  # we have 2 regularizers.
-            supports_masking=True,
-        )
 
-    def test_enable_lora_with_kernel_constraint(self):
-        layer = layers.Dense(units=2, kernel_constraint="max_norm")
-        with self.assertRaisesRegex(
-            ValueError, "incompatible with kernel constraints"
-        ):
-            layer.enable_lora(rank=2)
-
-    def test_enable_lora_on_unbuilt_layer(self):
-        layer = layers.Dense(units=2)
-        with self.assertRaisesRegex(
-            ValueError, "Cannot enable lora on a layer that isn't yet built"
-        ):
-            layer.enable_lora(rank=2)
-
-    def test_enable_lora_when_already_enabled(self):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.enable_lora(rank=2)
-        with self.assertRaisesRegex(ValueError, "lora is already enabled"):
-            layer.enable_lora(rank=2)
-
-    """Test quantization-related (int8 and float8) methods"""
-
-    @pytest.mark.skipif(
-        backend.backend() == "numpy",
-        reason=f"{backend.backend()} does not support ops.custom_gradient.",
+def create_keras_tensors(input_shape, dtype, sparse):
+    if isinstance(input_shape, dict):
+        return {
+            utils.removesuffix(k, "_shape"): KerasTensor(
+                v, dtype=dtype[k], sparse=sparse
+            )
+            for k, v in input_shape.items()
+        }
+    return map_shape_dtype_structure(
+        lambda shape, dt: KerasTensor(shape, dtype=dt, sparse=sparse),
+        input_shape,
+        dtype,
     )
-    def test_quantize_int8(self):
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        x = np.random.random((2, 8))
-        y_float = layer(x)
-        layer.quantize("int8")
-
-        # Verify weights dtype
-        self.assertEqual(backend.standardize_dtype(layer._kernel.dtype), "int8")
-        self.assertEqual(
-            backend.standardize_dtype(layer.kernel_scale.dtype),
-            layer.variable_dtype,
-        )
-
-        # Try eager call and verify output correctness
-        y_quantized = layer(x)
-        mse = ops.mean(ops.square(y_float - y_quantized))
-        self.assertLess(mse, 1e-3)  # A weak correctness test
-
-        # Try saving and reloading the model
-        model = models.Sequential([layer])
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
-
-        # Try lora
-        layer = layers.Dense(units=16)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        layer.quantize("int8")
-        x = np.random.random((2, 8))
-        _ = layer(x)
-
-        # Try building with quantized dtype policy
-        layer = layers.Dense(units=16, dtype="int8_from_mixed_bfloat16")
-        layer.build((None, 8))
-        self.assertEqual(backend.standardize_dtype(layer._kernel.dtype), "int8")
-        self.assertEqual(
-            backend.standardize_dtype(layer.kernel_scale.dtype), "float32"
-        )
 
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_on_unbuilt_layer(self, mode):
-        layer = layers.Dense(units=2)
-        with self.assertRaisesRegex(
-            ValueError, "Cannot quantize a layer that isn't yet built."
-        ):
-            layer.quantize(mode)
-
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_on_subclass(self, mode):
-        class MyDense(layers.Dense):
-            pass
-
-        layer = MyDense(units=16)
-        layer.build((None, 8))
-        with self.assertRaises(NotImplementedError):
-            layer.quantize(mode)
-
-    @parameterized.named_parameters(
-        ("int8", "int8"),
-        ("float8", "float8"),
-    )
-    def test_quantize_when_already_quantized(self, mode):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.quantize(mode)
-        for m in ["int8", "float8"]:
-            with self.assertRaisesRegex(
-                ValueError, "is already quantized with dtype_policy="
-            ):
-                layer.quantize(m)
 
-    @parameterized.named_parameters(
-        ("int8", "int8_from_float32"),
-        ("float8", "float8_from_float32"),
-    )
-    def test_quantize_when_already_quantized_using_dtype_argument(self, mode):
-        layer = layers.Dense(units=2, dtype=mode)
-        layer.build((None, 2))
-        for m in ["int8", "float8"]:
-            with self.assertRaisesRegex(
-                ValueError, "is already quantized with dtype_policy="
-            ):
-                layer.quantize(m)
+def create_eager_tensors(input_shape, dtype, sparse):
+    from keras.src.backend import random
 
-    @parameterized.named_parameters(
-        ("int8", "int8_from_float32", 3),
-        ("float8", "float8_from_float32", 8),
-    )
-    def test_quantize_by_setting_dtype_policy(
-        self, policy, expected_num_variables
+    if set(tree.flatten(dtype)).difference(
+        ["float16", "float32", "float64", "int16", "int32", "int64"]
     ):
-        layer = layers.Dense(units=2)
-        layer.build((None, 2))
-        layer.dtype_policy = policy
-        self.assertLen(layer.variables, expected_num_variables)
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_int8_dtype_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "dtype": "int8_from_mixed_bfloat16",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=1,
-            expected_num_non_trainable_weights=2,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
+        raise ValueError(
+            "dtype must be a standard float or int dtype. "
+            f"Received: dtype={dtype}"
         )
 
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_int8_when_lora_enabled(self):
-        # Note that saving and loading with lora_enabled and quantized are
-        # lossy, so we use a weak correctness test for model outputs (atol=0.5).
-        config = dict(units=16)
-        layer = layers.Dense(**config)
-        layer.build((None, 8))
-        layer.enable_lora(4)
-        layer.quantize("int8")
-        self.assertLen(layer.trainable_weights, 3)
-        self.assertLen(layer.non_trainable_weights, 2)
-        if backend.backend() == "torch":
-            self.assertLen(layer.torch_params, 5)
-
-        # Try calling fit()
-        init_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        init_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        model = models.Sequential([layer])
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y, epochs=2)
-
-        final_lora_a_kernel_value = layer.lora_kernel_a.numpy()
-        final_lora_b_kernel_value = layer.lora_kernel_b.numpy()
-        diff_a = np.max(
-            np.abs(init_lora_a_kernel_value - final_lora_a_kernel_value)
-        )
-        diff_b = np.max(
-            np.abs(init_lora_b_kernel_value - final_lora_b_kernel_value)
-        )
-        self.assertGreater(diff_a, 0.0)
-        self.assertGreater(diff_b, 0.0)
-
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_lora_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertTrue(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_lora_model.weights.h5"
-        )
-        model.save_weights(temp_filepath)
-        new_model = models.Sequential([layers.Dense(**config)])
-        new_model.build((None, 8))
-        new_model.quantize("int8")
-        new_model.load_weights(temp_filepath)
-        self.assertFalse(new_model.layers[0].lora_enabled)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Try loading a normal checkpoint into a lora model
-        new_model.save_weights(temp_filepath)
-        model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x), atol=0.5)
-
-        # Test export and TFSMLayer reloading when using tensorflow backend
+    if sparse:
         if backend.backend() == "tensorflow":
             import tensorflow as tf
 
-            temp_filepath = os.path.join(self.get_temp_dir(), "exported_model")
-            ref_input = tf.random.normal((2, 8))
-            ref_output = model(ref_input)
-            export_lib.export_model(model, temp_filepath)
-            reloaded_layer = export_lib.TFSMLayer(temp_filepath)
-            self.assertAllClose(
-                reloaded_layer(ref_input), ref_output, atol=1e-7
-            )
-            self.assertLen(reloaded_layer.weights, len(model.weights))
-            self.assertLen(
-                reloaded_layer.trainable_weights, len(model.trainable_weights)
-            )
-            self.assertLen(
-                reloaded_layer.non_trainable_weights,
-                len(model.non_trainable_weights),
-            )
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8_dtype_argument(self):
-        self.run_layer_test(
-            layers.Dense,
-            init_kwargs={
-                "units": 5,
-                "dtype": "float8_from_mixed_bfloat16",
-            },
-            input_shape=(2, 3, 4),
-            expected_output_shape=(2, 3, 5),
-            expected_num_trainable_weights=8,
-            expected_num_non_trainable_weights=0,
-            expected_num_seed_generators=0,
-            expected_num_losses=0,
-            supports_masking=True,
-        )
+            def create_fn(shape, dt):
+                rng = np.random.default_rng(0)
+                x = (4 * rng.standard_normal(shape)).astype(dt)
+                x = np.multiply(x, rng.random(shape) < 0.7)
+                return tf.sparse.from_dense(x)
 
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8(self):
-        import ml_dtypes
-
-        from keras.src import quantizers
-
-        layer = layers.Dense(units=32)
-        layer.build((None, 16))
-        layer.quantize("float8")
-        optimizer = optimizers.AdamW(learning_rate=0.1)
-        optimizer.build(layer.trainable_variables)
-
-        def loss_fn(x, dy):
-            y = layer(x, training=True)
-            loss = y * ops.cast(dy, y.dtype)
-            return ops.sum(loss)
+        elif backend.backend() == "jax":
+            import jax.experimental.sparse as jax_sparse
 
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
+            def create_fn(shape, dt):
+                rng = np.random.default_rng(0)
+                x = (4 * rng.standard_normal(shape)).astype(dt)
+                x = np.multiply(x, rng.random(shape) < 0.7)
+                return jax_sparse.BCOO.fromdense(x, n_batch=1)
 
-            @tf.function(jit_compile=True)
-            def train_one_step(x, dy):
-                with tf.GradientTape() as tape:
-                    loss = loss_fn(x, dy)
-                grads = tape.gradient(loss, layer.trainable_variables)
-                optimizer.apply(grads, layer.trainable_variables)
+        else:
+            raise ValueError(
+                f"Sparse is unsupported with backend {backend.backend()}"
+            )
 
-        elif backend.backend() == "jax":
-            import jax
+    else:
 
-            def stateless_loss_fn(trainable_variables, x, dy):
-                y = layer.stateless_call(trainable_variables, [], x)[0]
-                loss = y * ops.cast(dy, y.dtype)
-                return ops.sum(loss)
-
-            grad_fn = jax.jit(jax.grad(stateless_loss_fn))
-
-            def train_one_step(x, dy):
-                trainable_variables = [
-                    v.value for v in layer.trainable_variables
-                ]
-                optimizer_variables = [v.value for v in optimizer.variables]
-                grads = grad_fn(trainable_variables, x, dy)
-                trainable_variables, optimizer_variables = (
-                    optimizer.stateless_apply(
-                        optimizer_variables, grads, trainable_variables
-                    )
-                )
-                for variable, value in zip(
-                    layer.trainable_variables, trainable_variables
-                ):
-                    variable.assign(value)
-                for variable, value in zip(
-                    optimizer.variables, optimizer_variables
-                ):
-                    variable.assign(value)
+        def create_fn(shape, dt):
+            return ops.cast(
+                random.uniform(shape, dtype="float32") * 3, dtype=dt
+            )
 
-        elif backend.backend() == "torch":
+    if isinstance(input_shape, dict):
+        return {
+            utils.removesuffix(k, "_shape"): create_fn(v, dtype[k])
+            for k, v in input_shape.items()
+        }
+    return map_shape_dtype_structure(create_fn, input_shape, dtype)
 
-            def train_one_step(x, dy):
-                layer.zero_grad()
-                loss = loss_fn(x, dy)
-                loss.backward()
-                grads = [v.value.grad for v in layer.trainable_variables]
-                optimizer.apply(grads, layer.trainable_variables)
-
-        scale_x, amax_history_x = ops.ones(()), ops.zeros((1024,))
-        scale_k, amax_history_k = ops.ones(()), ops.zeros((1024,))
-        scale_g, amax_history_g = ops.ones(()), ops.zeros((1024,))
-        e4m3_max = ops.cast(
-            float(ml_dtypes.finfo("float8_e4m3fn").max), "float32"
-        )
-        e5m2_max = ops.cast(
-            float(ml_dtypes.finfo("float8_e5m2").max), "float32"
-        )
 
-        for _ in range(3):
-            x = random.normal((16, 16), dtype="float32")
-            g = random.normal((16, 32), dtype="float32")
-            k = ops.convert_to_tensor(layer._kernel)
-
-            # Manually compute the expected amax history and scaling factors.
-            amax_from_history_x = ops.max(amax_history_x)
-            amax_from_history_k = ops.max(amax_history_k)
-            amax_from_history_g = ops.max(amax_history_g)
-            scale_x = quantizers.compute_float8_scale(
-                amax_from_history_x, scale_x, e4m3_max
-            )
-            scale_k = quantizers.compute_float8_scale(
-                amax_from_history_k, scale_k, e4m3_max
-            )
-            scale_g = quantizers.compute_float8_scale(
-                amax_from_history_g, scale_g, e5m2_max
-            )
-            amax_history_x = quantizers.compute_float8_amax_history(
-                x, amax_history_x
-            )
-            amax_history_k = quantizers.compute_float8_amax_history(
-                k, amax_history_k
-            )
-            amax_history_g = quantizers.compute_float8_amax_history(
-                g, amax_history_g
-            )
-
-            train_one_step(x, g)
-
-            self.assertAllClose(layer.inputs_amax_history, amax_history_x)
-            self.assertAllClose(layer.kernel_amax_history, amax_history_k)
-            self.assertAllClose(layer.outputs_grad_amax_history, amax_history_g)
-            self.assertAllClose(layer.inputs_scale, scale_x)
-            self.assertAllClose(layer.kernel_scale, scale_k)
-            self.assertAllClose(layer.outputs_grad_scale, scale_g)
-
-    @pytest.mark.requires_trainable_backend
-    def test_quantize_float8_fitting(self):
-        config = dict(units=16)
-        layer = layers.Dense(**config)
-        layer.build((None, 8))
-        layer.quantize("float8")
-        self.assertLen(layer.trainable_weights, 8)
-        self.assertLen(layer.non_trainable_weights, 0)
-
-        # Try calling fit()
-        x = np.random.random((64, 8))
-        y = np.random.random((64, 16))
-        model = models.Sequential([layer])
-        model.compile(optimizer="sgd", loss="mse")
-        model.fit(x, y, epochs=2)
-
-        # Try saving and reloading the model
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_float8_model.keras"
-        )
-        model.save(temp_filepath)
-        new_model = saving.load_model(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
-
-        # Try saving and reloading the model's weights only
-        temp_filepath = os.path.join(
-            self.get_temp_dir(), "quantized_float8_model.weights.h5"
+def is_shape_tuple(x):
+    return isinstance(x, (list, tuple)) and all(
+        isinstance(e, (int, type(None))) for e in x
+    )
+
+
+def map_shape_dtype_structure(fn, shape, dtype):
+    """Variant of tree.map_structure that operates on shape tuples."""
+    if is_shape_tuple(shape):
+        return fn(tuple(shape), dtype)
+    if isinstance(shape, list):
+        return [
+            map_shape_dtype_structure(fn, s, d) for s, d in zip(shape, dtype)
+        ]
+    if isinstance(shape, tuple):
+        return tuple(
+            map_shape_dtype_structure(fn, s, d) for s, d in zip(shape, dtype)
+        )
+    if isinstance(shape, dict):
+        return {
+            k: map_shape_dtype_structure(fn, v, dtype[k])
+            for k, v in shape.items()
+        }
+    else:
+        raise ValueError(
+            f"Cannot map function to unknown objects {shape} and {dtype}"
         )
-        model.save_weights(temp_filepath)
-        new_model = models.Sequential([layers.Dense(**config)])
-        new_model.build((None, 8))
-        new_model.quantize("float8")
-        new_model.load_weights(temp_filepath)
-        self.assertAllClose(model.predict(x), new_model.predict(x))
 
-        # Test export and TFSMLayer reloading when using tensorflow backend
-        if backend.backend() == "tensorflow":
-            import tensorflow as tf
 
-            temp_filepath = os.path.join(self.get_temp_dir(), "exported_model")
-            ref_input = tf.random.normal((2, 8))
-            ref_output = model(ref_input)
-            export_lib.export_model(model, temp_filepath)
-            reloaded_layer = export_lib.TFSMLayer(temp_filepath)
-            self.assertAllClose(reloaded_layer(ref_input), ref_output)
-            self.assertLen(reloaded_layer.weights, len(model.weights))
-            self.assertLen(
-                reloaded_layer.trainable_weights, len(model.trainable_weights)
-            )
-            self.assertLen(
-                reloaded_layer.non_trainable_weights,
-                len(model.non_trainable_weights),
-            )
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

### Comparing `keras-3.3.0/keras/src/layers/core/einsum_dense.py` & `keras-3.3.1/keras/src/layers/core/einsum_dense.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/embedding.py` & `keras-3.3.1/keras/src/layers/core/embedding.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/identity.py` & `keras-3.3.1/keras/src/layers/core/identity.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/input_layer.py` & `keras-3.3.1/keras/src/layers/core/input_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/lambda_layer.py` & `keras-3.3.1/keras/src/layers/core/lambda_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/masking.py` & `keras-3.3.1/keras/src/layers/core/masking.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/core/wrapper.py` & `keras-3.3.1/keras/src/layers/core/wrapper.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/input_spec.py` & `keras-3.3.1/keras/src/layers/input_spec.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/layer.py` & `keras-3.3.1/keras/src/layers/layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/add.py` & `keras-3.3.1/keras/src/layers/merging/add.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/average.py` & `keras-3.3.1/keras/src/layers/merging/average.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/base_merge.py` & `keras-3.3.1/keras/src/layers/merging/base_merge.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/concatenate.py` & `keras-3.3.1/keras/src/layers/merging/concatenate.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/dot.py` & `keras-3.3.1/keras/src/layers/merging/dot.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/maximum.py` & `keras-3.3.1/keras/src/layers/merging/maximum.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/minimum.py` & `keras-3.3.1/keras/src/layers/merging/minimum.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/multiply.py` & `keras-3.3.1/keras/src/layers/merging/multiply.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/merging/subtract.py` & `keras-3.3.1/keras/src/layers/merging/subtract.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/normalization/batch_normalization.py` & `keras-3.3.1/keras/src/layers/normalization/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/normalization/group_normalization.py` & `keras-3.3.1/keras/src/layers/normalization/group_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/normalization/layer_normalization.py` & `keras-3.3.1/keras/src/layers/normalization/layer_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/normalization/spectral_normalization.py` & `keras-3.3.1/keras/src/layers/normalization/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/normalization/unit_normalization.py` & `keras-3.3.1/keras/src/layers/normalization/unit_normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/average_pooling1d.py` & `keras-3.3.1/keras/src/layers/pooling/average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/average_pooling2d.py` & `keras-3.3.1/keras/src/layers/pooling/average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/average_pooling3d.py` & `keras-3.3.1/keras/src/layers/pooling/average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/base_global_pooling.py` & `keras-3.3.1/keras/src/layers/pooling/base_global_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/base_pooling.py` & `keras-3.3.1/keras/src/layers/pooling/base_pooling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_average_pooling1d.py` & `keras-3.3.1/keras/src/layers/pooling/global_average_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_average_pooling2d.py` & `keras-3.3.1/keras/src/layers/pooling/global_average_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_average_pooling3d.py` & `keras-3.3.1/keras/src/layers/pooling/global_average_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_max_pooling1d.py` & `keras-3.3.1/keras/src/layers/pooling/global_max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_max_pooling2d.py` & `keras-3.3.1/keras/src/layers/pooling/global_max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/global_max_pooling3d.py` & `keras-3.3.1/keras/src/layers/pooling/global_max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/max_pooling1d.py` & `keras-3.3.1/keras/src/layers/pooling/max_pooling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/max_pooling2d.py` & `keras-3.3.1/keras/src/layers/pooling/max_pooling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/pooling/max_pooling3d.py` & `keras-3.3.1/keras/src/layers/pooling/max_pooling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/audio_preprocessing.py` & `keras-3.3.1/keras/src/layers/preprocessing/audio_preprocessing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/category_encoding.py` & `keras-3.3.1/keras/src/layers/preprocessing/category_encoding.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/center_crop.py` & `keras-3.3.1/keras/src/layers/preprocessing/center_crop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/discretization.py` & `keras-3.3.1/keras/src/layers/preprocessing/discretization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/feature_space.py` & `keras-3.3.1/keras/src/layers/preprocessing/feature_space.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/hashed_crossing.py` & `keras-3.3.1/keras/src/layers/preprocessing/hashed_crossing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/hashing.py` & `keras-3.3.1/keras/src/layers/preprocessing/hashing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/index_lookup.py` & `keras-3.3.1/keras/src/layers/preprocessing/index_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/integer_lookup.py` & `keras-3.3.1/keras/src/layers/preprocessing/integer_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/normalization.py` & `keras-3.3.1/keras/src/layers/preprocessing/normalization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_brightness.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_brightness.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_contrast.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_contrast.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_crop.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_crop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_flip.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_flip.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_rotation.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_rotation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_translation.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_translation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/random_zoom.py` & `keras-3.3.1/keras/src/layers/preprocessing/random_zoom.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/rescaling.py` & `keras-3.3.1/keras/src/layers/preprocessing/rescaling.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/resizing.py` & `keras-3.3.1/keras/src/layers/preprocessing/resizing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/string_lookup.py` & `keras-3.3.1/keras/src/layers/preprocessing/string_lookup.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/text_vectorization.py` & `keras-3.3.1/keras/src/layers/preprocessing/text_vectorization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/preprocessing/tf_data_layer.py` & `keras-3.3.1/keras/src/layers/preprocessing/tf_data_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/activity_regularization.py` & `keras-3.3.1/keras/src/layers/regularization/activity_regularization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/alpha_dropout.py` & `keras-3.3.1/keras/src/layers/regularization/alpha_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/dropout.py` & `keras-3.3.1/keras/src/layers/regularization/dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/gaussian_dropout.py` & `keras-3.3.1/keras/src/layers/regularization/gaussian_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/gaussian_noise.py` & `keras-3.3.1/keras/src/layers/regularization/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/regularization/spatial_dropout.py` & `keras-3.3.1/keras/src/layers/regularization/spatial_dropout.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/cropping1d.py` & `keras-3.3.1/keras/src/layers/reshaping/cropping1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/cropping2d.py` & `keras-3.3.1/keras/src/layers/reshaping/cropping2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/cropping3d.py` & `keras-3.3.1/keras/src/layers/reshaping/cropping3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/flatten.py` & `keras-3.3.1/keras/src/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/permute.py` & `keras-3.3.1/keras/src/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/repeat_vector.py` & `keras-3.3.1/keras/src/layers/reshaping/repeat_vector.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/reshape.py` & `keras-3.3.1/keras/src/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/up_sampling1d.py` & `keras-3.3.1/keras/src/layers/reshaping/up_sampling1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/up_sampling2d.py` & `keras-3.3.1/keras/src/layers/reshaping/up_sampling2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/up_sampling3d.py` & `keras-3.3.1/keras/src/layers/reshaping/up_sampling3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/zero_padding1d.py` & `keras-3.3.1/keras/src/layers/reshaping/zero_padding1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/zero_padding2d.py` & `keras-3.3.1/keras/src/layers/reshaping/zero_padding2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/reshaping/zero_padding3d.py` & `keras-3.3.1/keras/src/layers/reshaping/zero_padding3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/bidirectional.py` & `keras-3.3.1/keras/src/layers/rnn/bidirectional.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/conv_lstm.py` & `keras-3.3.1/keras/src/layers/rnn/conv_lstm.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/conv_lstm1d.py` & `keras-3.3.1/keras/src/layers/rnn/conv_lstm1d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/conv_lstm2d.py` & `keras-3.3.1/keras/src/layers/rnn/conv_lstm2d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/conv_lstm3d.py` & `keras-3.3.1/keras/src/layers/rnn/conv_lstm3d.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/dropout_rnn_cell.py` & `keras-3.3.1/keras/src/layers/rnn/dropout_rnn_cell.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/gru.py` & `keras-3.3.1/keras/src/layers/rnn/gru.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/lstm.py` & `keras-3.3.1/keras/src/layers/rnn/lstm.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/rnn.py` & `keras-3.3.1/keras/src/layers/rnn/rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/simple_rnn.py` & `keras-3.3.1/keras/src/layers/rnn/simple_rnn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/stacked_rnn_cells.py` & `keras-3.3.1/keras/src/layers/rnn/stacked_rnn_cells.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/layers/rnn/time_distributed.py` & `keras-3.3.1/keras/src/layers/rnn/time_distributed.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/backend.py` & `keras-3.3.1/keras/src/legacy/backend.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/layers.py` & `keras-3.3.1/keras/src/legacy/layers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/losses.py` & `keras-3.3.1/keras/src/legacy/losses.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/preprocessing/image.py` & `keras-3.3.1/keras/src/legacy/preprocessing/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/preprocessing/sequence.py` & `keras-3.3.1/keras/src/legacy/preprocessing/sequence.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/preprocessing/text.py` & `keras-3.3.1/keras/src/legacy/preprocessing/text.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/saving/json_utils.py` & `keras-3.3.1/keras/src/legacy/saving/json_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/saving/legacy_h5_format.py` & `keras-3.3.1/keras/src/legacy/saving/legacy_h5_format.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/saving/saving_utils.py` & `keras-3.3.1/keras/src/legacy/saving/saving_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/legacy/saving/serialization.py` & `keras-3.3.1/keras/src/legacy/saving/serialization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/losses/__init__.py` & `keras-3.3.1/keras/src/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/losses/loss.py` & `keras-3.3.1/keras/src/losses/loss.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/losses/losses.py` & `keras-3.3.1/keras/src/losses/losses.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/__init__.py` & `keras-3.3.1/keras/src/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/accuracy_metrics.py` & `keras-3.3.1/keras/src/metrics/accuracy_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/confusion_metrics.py` & `keras-3.3.1/keras/src/metrics/confusion_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/f_score_metrics.py` & `keras-3.3.1/keras/src/metrics/f_score_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/hinge_metrics.py` & `keras-3.3.1/keras/src/metrics/hinge_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/iou_metrics.py` & `keras-3.3.1/keras/src/metrics/iou_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/metric.py` & `keras-3.3.1/keras/src/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/metrics_utils.py` & `keras-3.3.1/keras/src/metrics/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/probabilistic_metrics.py` & `keras-3.3.1/keras/src/metrics/probabilistic_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/reduction_metrics.py` & `keras-3.3.1/keras/src/metrics/reduction_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/metrics/regression_metrics.py` & `keras-3.3.1/keras/src/metrics/regression_metrics.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/models/cloning.py` & `keras-3.3.1/keras/src/models/cloning.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/models/functional.py` & `keras-3.3.1/keras/src/models/functional.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/models/model.py` & `keras-3.3.1/keras/src/models/model.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/models/sequential.py` & `keras-3.3.1/keras/src/models/sequential.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/models/variable_mapping.py` & `keras-3.3.1/keras/src/models/variable_mapping.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/__init__.py` & `keras-3.3.1/keras/src/ops/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/core.py` & `keras-3.3.1/keras/src/ops/core.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/function.py` & `keras-3.3.1/keras/src/ops/function.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/image.py` & `keras-3.3.1/keras/src/ops/image.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/linalg.py` & `keras-3.3.1/keras/src/ops/linalg.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/math.py` & `keras-3.3.1/keras/src/ops/math.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/nn.py` & `keras-3.3.1/keras/src/ops/nn.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/node.py` & `keras-3.3.1/keras/src/ops/node.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/numpy.py` & `keras-3.3.1/keras/src/ops/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 arcsin
 arcsinh
 arctan
 arctan2
 arctanh
 argmax
 argmin
+argpartition
 argsort
 array
 average
 bincount
 broadcast_to
 ceil
 clip
@@ -6299,7 +6300,53 @@
             "condlist and choicelist must not be empty. Received: "
             f"condlist = {condlist}, "
             f"choicelist = {choicelist}"
         )
     if any_symbolic_tensors(condlist + choicelist + [default]):
         return Select().symbolic_call(condlist, choicelist, default)
     return backend.numpy.select(condlist, choicelist, default)
+
+
+class Argpartition(Operation):
+    def __init__(self, kth, axis=-1):
+        super().__init__()
+        self.kth = kth
+        self.axis = axis
+
+    def call(self, x):
+        return backend.numpy.argpartition(x, kth=self.kth, axis=self.axis)
+
+    def compute_output_spec(self, x):
+        if not isinstance(self.kth, int):
+            raise ValueError(
+                "kth must be an integer. Received:" f"kth = {self.kth}"
+            )
+
+        dtype = "int32"
+        if backend.backend() in ("torch", "numpy"):
+            dtype = "int64"
+        return KerasTensor(x.shape, dtype=dtype)
+
+
+@keras_export(["keras.ops.argpartition", "keras.ops.numpy.argpartition"])
+def argpartition(x, kth, axis=-1):
+    """Performs an indirect partition along the given axis. It returns an array
+    of indices of the same shape as `x` that index data along the given axis
+    in partitioned order.
+
+    Args:
+        a: Array to sort.
+        kth: Element index to partition by.
+            The k-th element will be in its final sorted position and all
+            smaller elements will be moved before it and all larger elements
+            behind it. The order of all elements in the partitions is undefined.
+            If provided with a sequence of k-th it will partition all of them
+            into their sorted position at once.
+        axis: Axis along which to sort. The default is -1 (the last axis).
+            If None, the flattened array is used.
+
+    Returns:
+        Array of indices that partition `x` along the specified `axis`.
+    """
+    if any_symbolic_tensors((x,)):
+        return Argpartition(kth, axis).symbolic_call(x)
+    return backend.numpy.argpartition(x, kth, axis)
```

### Comparing `keras-3.3.0/keras/src/ops/operation.py` & `keras-3.3.1/keras/src/ops/operation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/operation_utils.py` & `keras-3.3.1/keras/src/ops/operation_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/ops/symbolic_arguments.py` & `keras-3.3.1/keras/src/ops/symbolic_arguments.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/__init__.py` & `keras-3.3.1/keras/src/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/adadelta.py` & `keras-3.3.1/keras/src/optimizers/adamax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,139 +1,156 @@
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.optimizers import optimizer
 
 
-@keras_export(["keras.optimizers.Adadelta"])
-class Adadelta(optimizer.Optimizer):
-    """Optimizer that implements the Adadelta algorithm.
-
-    Adadelta optimization is a stochastic gradient descent method that is based
-    on adaptive learning rate per dimension to address two drawbacks:
-
-    - The continual decay of learning rates throughout training.
-    - The need for a manually selected global learning rate.
-
-    Adadelta is a more robust extension of Adagrad that adapts learning rates
-    based on a moving window of gradient updates, instead of accumulating all
-    past gradients. This way, Adadelta continues learning even when many updates
-    have been done. Compared to Adagrad, in the original version of Adadelta you
-    don't have to set an initial learning rate. In this version, the initial
-    learning rate can be set, as in most other Keras optimizers.
+@keras_export(["keras.optimizers.Adamax"])
+class Adamax(optimizer.Optimizer):
+    """Optimizer that implements the Adamax algorithm.
+
+    Adamax, a variant of Adam based on the infinity norm, is a first-order
+    gradient-based optimization method. Due to its capability of adjusting the
+    learning rate based on data characteristics, it is suited to learn
+    time-variant process, e.g., speech data with dynamically changed noise
+    conditions. Default parameters follow those provided in the paper (see
+    references below).
+
+    Initialization:
+
+    ```python
+    m = 0  # Initialize initial 1st moment vector
+    u = 0  # Initialize the exponentially weighted infinity norm
+    t = 0  # Initialize timestep
+    ```
+
+    The update rule for parameter `w` with gradient `g` is described at the end
+    of section 7.1 of the paper (see the referenece section):
+
+    ```python
+    t += 1
+    m = beta1 * m + (1 - beta) * g
+    u = max(beta2 * u, abs(g))
+    current_lr = learning_rate / (1 - beta1 ** t)
+    w = w - current_lr * m / (u + epsilon)
+    ```
 
     Args:
         learning_rate: A float, a
             `keras.optimizers.schedules.LearningRateSchedule` instance, or
             a callable that takes no arguments and returns the actual value to
-            use. The learning rate. Defaults to `0.001`. Note that `Adadelta`
-            tends to benefit from higher initial learning rate values compared
-            to other optimizers. To match the exact form in the original paper,
-            use 1.0.
-        rho: A floating point value. The decay rate. Defaults to `0.95`.
-        epsilon: Small floating point value for maintaining numerical stability.
-        {{base_optimizer_keyword_args}}
+            use. The learning rate. Defaults to `0.001`.
+        beta_1: A float value or a constant float tensor. The exponential decay
+            rate for the 1st moment estimates.
+        beta_2: A float value or a constant float tensor. The exponential decay
+            rate for the exponentially weighted infinity norm.
+        epsilon: A small constant for numerical stability.
+            {{base_optimizer_keyword_args}}
 
     Reference:
 
-    - [Zeiler, 2012](http://arxiv.org/abs/1212.5701)
+    - [Kingma et al., 2014](http://arxiv.org/abs/1412.6980)
     """
 
     def __init__(
         self,
         learning_rate=0.001,
-        rho=0.95,
+        beta_1=0.9,
+        beta_2=0.999,
         epsilon=1e-7,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
         loss_scale_factor=None,
         gradient_accumulation_steps=None,
-        name="adadelta",
+        name="adamax",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
+            name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
             clipvalue=clipvalue,
             global_clipnorm=global_clipnorm,
             use_ema=use_ema,
             ema_momentum=ema_momentum,
             ema_overwrite_frequency=ema_overwrite_frequency,
             loss_scale_factor=loss_scale_factor,
             gradient_accumulation_steps=gradient_accumulation_steps,
-            name=name,
             **kwargs,
         )
-        self.rho = rho
+        self.beta_1 = beta_1
+        self.beta_2 = beta_2
         self.epsilon = epsilon
 
     def build(self, var_list):
+        """Initialize optimizer variables.
+
+        Adamax optimizer has 2 types of variables: momentums (denoted as m),
+        exponentially weighted infinity norm (denoted as u).
+
+        Args:
+            var_list: list of model variables to build Adamax variables on.
+        """
         if self.built:
             return
         super().build(var_list)
-        self._accumulated_grads = []
-        self._accumulated_delta_vars = []
+        self._m = []
+        self._u = []
         for var in var_list:
-            self._accumulated_grads.append(
-                self.add_variable_from_reference(var, "accumulated_grad")
+            self._m.append(
+                self.add_variable_from_reference(
+                    reference_variable=var, name="momentum"
+                )
             )
-            self._accumulated_delta_vars.append(
-                self.add_variable_from_reference(var, "accumulated_delta_var")
+            self._u.append(
+                self.add_variable_from_reference(
+                    reference_variable=var, name="norm"
+                )
             )
 
-    def update_step(self, grad, variable, learning_rate):
+    def update_step(self, gradient, variable, learning_rate):
         """Update step given gradient and the associated model variable."""
         lr = ops.cast(learning_rate, variable.dtype)
-        grad = ops.cast(grad, variable.dtype)
-
-        rho = self.rho
-        accumulated_grad = self._accumulated_grads[
-            self._get_variable_index(variable)
-        ]
-        accumulated_delta_var = self._accumulated_delta_vars[
-            self._get_variable_index(variable)
-        ]
+        gradient = ops.cast(gradient, variable.dtype)
+        local_step = ops.cast(self.iterations + 1, variable.dtype)
+        beta_1_power = ops.power(
+            ops.cast(self.beta_1, variable.dtype), local_step
+        )
 
-        def rms(x):
-            return ops.sqrt(ops.add(x, self.epsilon))
+        m = self._m[self._get_variable_index(variable)]
+        u = self._u[self._get_variable_index(variable)]
 
+        self.assign_add(
+            m, ops.multiply(ops.subtract(gradient, m), (1 - self.beta_1))
+        )
         self.assign(
-            accumulated_grad,
-            ops.add(
-                rho * accumulated_grad, ops.multiply(1 - rho, ops.square(grad))
-            ),
+            u, ops.maximum(ops.multiply(self.beta_2, u), ops.abs(gradient))
         )
-        delta_var = ops.negative(
+        self.assign_sub(
+            variable,
             ops.divide(
-                ops.multiply(rms(accumulated_delta_var), grad),
-                rms(accumulated_grad),
-            )
-        )
-        self.assign(
-            accumulated_delta_var,
-            ops.add(
-                ops.multiply(rho, accumulated_delta_var),
-                ops.multiply(1 - rho, ops.square(delta_var)),
+                ops.multiply(lr, m),
+                ops.multiply((1 - beta_1_power), ops.add(u, self.epsilon)),
             ),
         )
-        self.assign_add(variable, ops.multiply(lr, delta_var))
 
     def get_config(self):
         config = super().get_config()
 
         config.update(
             {
-                "rho": self.rho,
+                "beta_1": self.beta_1,
+                "beta_2": self.beta_2,
                 "epsilon": self.epsilon,
             }
         )
         return config
 
 
-Adadelta.__doc__ = Adadelta.__doc__.replace(
+Adamax.__doc__ = Adamax.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
```

### Comparing `keras-3.3.0/keras/src/optimizers/adafactor.py` & `keras-3.3.1/keras/src/optimizers/adafactor.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/adagrad.py` & `keras-3.3.1/keras/src/optimizers/adagrad.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/adam.py` & `keras-3.3.1/keras/src/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/adamax.py` & `keras-3.3.1/keras/src/optimizers/lion.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,75 +1,65 @@
 from keras.src import ops
 from keras.src.api_export import keras_export
 from keras.src.optimizers import optimizer
 
 
-@keras_export(["keras.optimizers.Adamax"])
-class Adamax(optimizer.Optimizer):
-    """Optimizer that implements the Adamax algorithm.
-
-    Adamax, a variant of Adam based on the infinity norm, is a first-order
-    gradient-based optimization method. Due to its capability of adjusting the
-    learning rate based on data characteristics, it is suited to learn
-    time-variant process, e.g., speech data with dynamically changed noise
-    conditions. Default parameters follow those provided in the paper (see
-    references below).
-
-    Initialization:
-
-    ```python
-    m = 0  # Initialize initial 1st moment vector
-    u = 0  # Initialize the exponentially weighted infinity norm
-    t = 0  # Initialize timestep
-    ```
-
-    The update rule for parameter `w` with gradient `g` is described at the end
-    of section 7.1 of the paper (see the referenece section):
-
-    ```python
-    t += 1
-    m = beta1 * m + (1 - beta) * g
-    u = max(beta2 * u, abs(g))
-    current_lr = learning_rate / (1 - beta1 ** t)
-    w = w - current_lr * m / (u + epsilon)
-    ```
+@keras_export(["keras.optimizers.Lion"])
+class Lion(optimizer.Optimizer):
+    """Optimizer that implements the Lion algorithm.
+
+    The Lion optimizer is a stochastic-gradient-descent method that uses the
+    sign operator to control the magnitude of the update, unlike other adaptive
+    optimizers such as Adam that rely on second-order moments. This make
+    Lion more memory-efficient as it only keeps track of the momentum. According
+    to the authors (see reference), its performance gain over Adam grows with
+    the batch size. Because the update of Lion is produced through the sign
+    operation, resulting in a larger norm, a suitable learning rate for Lion is
+    typically 3-10x smaller than that for AdamW. The weight decay for Lion
+    should be in turn 3-10x larger than that for AdamW to maintain a
+    similar strength (lr * wd).
 
     Args:
         learning_rate: A float, a
             `keras.optimizers.schedules.LearningRateSchedule` instance, or
             a callable that takes no arguments and returns the actual value to
             use. The learning rate. Defaults to `0.001`.
-        beta_1: A float value or a constant float tensor. The exponential decay
-            rate for the 1st moment estimates.
-        beta_2: A float value or a constant float tensor. The exponential decay
-            rate for the exponentially weighted infinity norm.
-        epsilon: A small constant for numerical stability.
-            {{base_optimizer_keyword_args}}
+        beta_1: A float value or a constant float tensor, or a callable
+            that takes no arguments and returns the actual value to use. The
+            rate to combine the current gradient and the 1st moment estimate.
+            Defaults to `0.9`.
+        beta_2: A float value or a constant float tensor, or a callable
+            that takes no arguments and returns the actual value to use. The
+            exponential decay rate for the 1st moment estimate. Defaults to
+            `0.99`.
+        {{base_optimizer_keyword_args}}
+
+    References:
+
+    - [Chen et al., 2023](http://arxiv.org/abs/2302.06675)
+    - [Authors' implementation](
+        http://github.com/google/automl/tree/master/lion)
 
-    Reference:
-
-    - [Kingma et al., 2014](http://arxiv.org/abs/1412.6980)
     """
 
     def __init__(
         self,
         learning_rate=0.001,
         beta_1=0.9,
-        beta_2=0.999,
-        epsilon=1e-7,
+        beta_2=0.99,
         weight_decay=None,
         clipnorm=None,
         clipvalue=None,
         global_clipnorm=None,
         use_ema=False,
         ema_momentum=0.99,
         ema_overwrite_frequency=None,
         loss_scale_factor=None,
         gradient_accumulation_steps=None,
-        name="adamax",
+        name="lion",
         **kwargs,
     ):
         super().__init__(
             learning_rate=learning_rate,
             name=name,
             weight_decay=weight_decay,
             clipnorm=clipnorm,
@@ -80,77 +70,73 @@
             ema_overwrite_frequency=ema_overwrite_frequency,
             loss_scale_factor=loss_scale_factor,
             gradient_accumulation_steps=gradient_accumulation_steps,
             **kwargs,
         )
         self.beta_1 = beta_1
         self.beta_2 = beta_2
-        self.epsilon = epsilon
+        if beta_1 <= 0 or beta_1 > 1:
+            raise ValueError(
+                "Argument `beta_1` must be in the [0, 1] range. Otherwise, the "
+                f"optimizer degenerates to SignSGD. Received: beta_1={beta_1}."
+            )
 
     def build(self, var_list):
         """Initialize optimizer variables.
 
-        Adamax optimizer has 2 types of variables: momentums (denoted as m),
-        exponentially weighted infinity norm (denoted as u).
+        Lion optimizer has one variable `momentums`.
 
         Args:
-            var_list: list of model variables to build Adamax variables on.
+            var_list: list of model variables to build Lion variables on.
         """
         if self.built:
             return
         super().build(var_list)
-        self._m = []
-        self._u = []
+        self._momentums = []
         for var in var_list:
-            self._m.append(
+            self._momentums.append(
                 self.add_variable_from_reference(
                     reference_variable=var, name="momentum"
                 )
             )
-            self._u.append(
-                self.add_variable_from_reference(
-                    reference_variable=var, name="norm"
-                )
-            )
 
     def update_step(self, gradient, variable, learning_rate):
         """Update step given gradient and the associated model variable."""
         lr = ops.cast(learning_rate, variable.dtype)
         gradient = ops.cast(gradient, variable.dtype)
-        local_step = ops.cast(self.iterations + 1, variable.dtype)
-        beta_1_power = ops.power(
-            ops.cast(self.beta_1, variable.dtype), local_step
-        )
-
-        m = self._m[self._get_variable_index(variable)]
-        u = self._u[self._get_variable_index(variable)]
+        beta_1 = ops.cast(self.beta_1, variable.dtype)
+        beta_2 = ops.cast(self.beta_2, variable.dtype)
+        m = self._momentums[self._get_variable_index(variable)]
 
-        self.assign_add(
-            m, ops.multiply(ops.subtract(gradient, m), (1 - self.beta_1))
-        )
-        self.assign(
-            u, ops.maximum(ops.multiply(self.beta_2, u), ops.abs(gradient))
-        )
         self.assign_sub(
             variable,
-            ops.divide(
-                ops.multiply(lr, m),
-                ops.multiply((1 - beta_1_power), ops.add(u, self.epsilon)),
+            ops.multiply(
+                lr,
+                ops.sign(
+                    ops.add(
+                        ops.multiply(m, beta_1),
+                        ops.multiply(gradient, (1.0 - beta_1)),
+                    )
+                ),
+            ),
+        )
+        self.assign(
+            m,
+            ops.add(
+                ops.multiply(m, beta_2), ops.multiply(gradient, (1.0 - beta_2))
             ),
         )
 
     def get_config(self):
         config = super().get_config()
-
         config.update(
             {
                 "beta_1": self.beta_1,
                 "beta_2": self.beta_2,
-                "epsilon": self.epsilon,
             }
         )
         return config
 
 
-Adamax.__doc__ = Adamax.__doc__.replace(
+Lion.__doc__ = Lion.__doc__.replace(
     "{{base_optimizer_keyword_args}}", optimizer.base_optimizer_keyword_args
 )
```

### Comparing `keras-3.3.0/keras/src/optimizers/adamw.py` & `keras-3.3.1/keras/src/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/base_optimizer.py` & `keras-3.3.1/keras/src/optimizers/base_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/ftrl.py` & `keras-3.3.1/keras/src/optimizers/ftrl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/loss_scale_optimizer.py` & `keras-3.3.1/keras/src/optimizers/loss_scale_optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/nadam.py` & `keras-3.3.1/keras/src/optimizers/nadam.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/optimizer.py` & `keras-3.3.1/keras/src/optimizers/optimizer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/rmsprop.py` & `keras-3.3.1/keras/src/optimizers/rmsprop.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/schedules/__init__.py` & `keras-3.3.1/keras/src/optimizers/schedules/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/schedules/learning_rate_schedule.py` & `keras-3.3.1/keras/src/optimizers/schedules/learning_rate_schedule.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/optimizers/sgd.py` & `keras-3.3.1/keras/src/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/quantizers/__init__.py` & `keras-3.3.1/keras/src/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/quantizers/quantizers.py` & `keras-3.3.1/keras/src/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/random/random.py` & `keras-3.3.1/keras/src/random/random.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/random/seed_generator.py` & `keras-3.3.1/keras/src/random/seed_generator.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/regularizers/__init__.py` & `keras-3.3.1/keras/src/regularizers/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/regularizers/regularizers.py` & `keras-3.3.1/keras/src/regularizers/regularizers.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/saving/__init__.py` & `keras-3.3.1/keras/src/saving/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/saving/object_registration.py` & `keras-3.3.1/keras/src/saving/object_registration.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/saving/saving_api.py` & `keras-3.3.1/keras/src/saving/saving_api.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/saving/saving_lib.py` & `keras-3.3.1/keras/src/saving/saving_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/saving/serialization_lib.py` & `keras-3.3.1/keras/src/saving/serialization_lib.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/testing/test_utils.py` & `keras-3.3.1/keras/src/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/compile_utils.py` & `keras-3.3.1/keras/src/trainers/compile_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/__init__.py` & `keras-3.3.1/keras/src/trainers/data_adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/array_data_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/array_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/array_slicing.py` & `keras-3.3.1/keras/src/trainers/data_adapters/array_slicing.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/data_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/data_adapter_utils.py` & `keras-3.3.1/keras/src/trainers/data_adapters/data_adapter_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/generator_data_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/generator_data_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/py_dataset_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/py_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/tf_dataset_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/tf_dataset_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/data_adapters/torch_data_loader_adapter.py` & `keras-3.3.1/keras/src/trainers/data_adapters/torch_data_loader_adapter.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/epoch_iterator.py` & `keras-3.3.1/keras/src/trainers/epoch_iterator.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/trainers/trainer.py` & `keras-3.3.1/keras/src/trainers/trainer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/tree/__init__.py` & `keras-3.3.1/keras/src/tree/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/tree/dmtree_impl.py` & `keras-3.3.1/keras/src/tree/dmtree_impl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/tree/optree_impl.py` & `keras-3.3.1/keras/src/tree/optree_impl.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/tree/tree_api.py` & `keras-3.3.1/keras/src/tree/tree_api.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/__init__.py` & `keras-3.3.1/keras/src/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/argument_validation.py` & `keras-3.3.1/keras/src/utils/argument_validation.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/audio_dataset_utils.py` & `keras-3.3.1/keras/src/utils/audio_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/backend_utils.py` & `keras-3.3.1/keras/src/utils/backend_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/code_stats.py` & `keras-3.3.1/keras/src/utils/code_stats.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/dataset_utils.py` & `keras-3.3.1/keras/src/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/dtype_utils.py` & `keras-3.3.1/keras/src/utils/dtype_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/file_utils.py` & `keras-3.3.1/keras/src/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/image_dataset_utils.py` & `keras-3.3.1/keras/src/utils/image_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/image_utils.py` & `keras-3.3.1/keras/src/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/io_utils.py` & `keras-3.3.1/keras/src/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/jax_layer.py` & `keras-3.3.1/keras/src/utils/jax_layer.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/model_visualization.py` & `keras-3.3.1/keras/src/utils/model_visualization.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/module_utils.py` & `keras-3.3.1/keras/src/utils/module_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/naming.py` & `keras-3.3.1/keras/src/utils/naming.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/numerical_utils.py` & `keras-3.3.1/keras/src/utils/numerical_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/progbar.py` & `keras-3.3.1/keras/src/utils/progbar.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/python_utils.py` & `keras-3.3.1/keras/src/utils/python_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/rng_utils.py` & `keras-3.3.1/keras/src/utils/rng_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/sequence_utils.py` & `keras-3.3.1/keras/src/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/summary_utils.py` & `keras-3.3.1/keras/src/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/text_dataset_utils.py` & `keras-3.3.1/keras/src/utils/text_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/tf_utils.py` & `keras-3.3.1/keras/src/utils/tf_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/timeseries_dataset_utils.py` & `keras-3.3.1/keras/src/utils/timeseries_dataset_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/torch_utils.py` & `keras-3.3.1/keras/src/utils/torch_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/traceback_utils.py` & `keras-3.3.1/keras/src/utils/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras/src/utils/tracking.py` & `keras-3.3.1/keras/src/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `keras-3.3.0/keras.egg-info/PKG-INFO` & `keras-3.3.1/keras.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keras
-Version: 3.3.0
+Version: 3.3.1
 Summary: Multi-backend Keras.
 Home-page: https://github.com/keras-team/keras
 Author: Keras team
 Author-email: keras-users@googlegroups.com
 License: Apache License 2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -15,15 +15,14 @@
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: absl-py
 Requires-Dist: numpy
 Requires-Dist: rich
 Requires-Dist: namex
 Requires-Dist: h5py
 Requires-Dist: optree
 Requires-Dist: ml-dtypes
```

### Comparing `keras-3.3.0/keras.egg-info/SOURCES.txt` & `keras-3.3.1/keras.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,103 +1,79 @@
-LICENSE
 README.md
-pyproject.toml
-setup.cfg
 setup.py
-benchmarks/__init__.py
-benchmarks/layer_benchmark/__init__.py
-benchmarks/layer_benchmark/activation_benchmark.py
-benchmarks/layer_benchmark/attention_benchmark.py
-benchmarks/layer_benchmark/base_benchmark.py
-benchmarks/layer_benchmark/conv_benchmark.py
-benchmarks/layer_benchmark/core_benchmark.py
-benchmarks/layer_benchmark/merge_benchmark.py
-benchmarks/layer_benchmark/normalization_benchmark.py
-benchmarks/layer_benchmark/pooling_benchmark.py
-benchmarks/layer_benchmark/regularization_benchmark.py
-benchmarks/layer_benchmark/reshaping_benchmark.py
-benchmarks/layer_benchmark/rnn_benchmark.py
-benchmarks/model_benchmark/__init__.py
-benchmarks/model_benchmark/benchmark_utils.py
-benchmarks/model_benchmark/bert_benchmark.py
-benchmarks/model_benchmark/image_classification_benchmark.py
-benchmarks/torch_ctl_benchmark/__init__.py
-benchmarks/torch_ctl_benchmark/benchmark_utils.py
-benchmarks/torch_ctl_benchmark/conv_model_benchmark.py
-benchmarks/torch_ctl_benchmark/dense_model_benchmark.py
 keras/__init__.py
 keras.egg-info/PKG-INFO
 keras.egg-info/SOURCES.txt
 keras.egg-info/dependency_links.txt
 keras.egg-info/requires.txt
 keras.egg-info/top_level.txt
+keras/_tf_keras/__init__.py
+keras/_tf_keras/keras/__init__.py
+keras/_tf_keras/keras/activations/__init__.py
+keras/_tf_keras/keras/applications/__init__.py
+keras/_tf_keras/keras/applications/convnext/__init__.py
+keras/_tf_keras/keras/applications/densenet/__init__.py
+keras/_tf_keras/keras/applications/efficientnet/__init__.py
+keras/_tf_keras/keras/applications/efficientnet_v2/__init__.py
+keras/_tf_keras/keras/applications/imagenet_utils/__init__.py
+keras/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
+keras/_tf_keras/keras/applications/inception_v3/__init__.py
+keras/_tf_keras/keras/applications/mobilenet/__init__.py
+keras/_tf_keras/keras/applications/mobilenet_v2/__init__.py
+keras/_tf_keras/keras/applications/mobilenet_v3/__init__.py
+keras/_tf_keras/keras/applications/nasnet/__init__.py
+keras/_tf_keras/keras/applications/resnet/__init__.py
+keras/_tf_keras/keras/applications/resnet50/__init__.py
+keras/_tf_keras/keras/applications/resnet_v2/__init__.py
+keras/_tf_keras/keras/applications/vgg16/__init__.py
+keras/_tf_keras/keras/applications/vgg19/__init__.py
+keras/_tf_keras/keras/applications/xception/__init__.py
+keras/_tf_keras/keras/backend/__init__.py
+keras/_tf_keras/keras/callbacks/__init__.py
+keras/_tf_keras/keras/config/__init__.py
+keras/_tf_keras/keras/constraints/__init__.py
+keras/_tf_keras/keras/datasets/__init__.py
+keras/_tf_keras/keras/datasets/boston_housing/__init__.py
+keras/_tf_keras/keras/datasets/california_housing/__init__.py
+keras/_tf_keras/keras/datasets/cifar10/__init__.py
+keras/_tf_keras/keras/datasets/cifar100/__init__.py
+keras/_tf_keras/keras/datasets/fashion_mnist/__init__.py
+keras/_tf_keras/keras/datasets/imdb/__init__.py
+keras/_tf_keras/keras/datasets/mnist/__init__.py
+keras/_tf_keras/keras/datasets/reuters/__init__.py
+keras/_tf_keras/keras/distribution/__init__.py
+keras/_tf_keras/keras/dtype_policies/__init__.py
+keras/_tf_keras/keras/export/__init__.py
+keras/_tf_keras/keras/initializers/__init__.py
+keras/_tf_keras/keras/layers/__init__.py
+keras/_tf_keras/keras/legacy/__init__.py
+keras/_tf_keras/keras/legacy/saving/__init__.py
+keras/_tf_keras/keras/losses/__init__.py
+keras/_tf_keras/keras/metrics/__init__.py
+keras/_tf_keras/keras/mixed_precision/__init__.py
+keras/_tf_keras/keras/models/__init__.py
+keras/_tf_keras/keras/ops/__init__.py
+keras/_tf_keras/keras/ops/image/__init__.py
+keras/_tf_keras/keras/ops/linalg/__init__.py
+keras/_tf_keras/keras/ops/nn/__init__.py
+keras/_tf_keras/keras/ops/numpy/__init__.py
+keras/_tf_keras/keras/optimizers/__init__.py
+keras/_tf_keras/keras/optimizers/legacy/__init__.py
+keras/_tf_keras/keras/optimizers/schedules/__init__.py
+keras/_tf_keras/keras/preprocessing/__init__.py
+keras/_tf_keras/keras/preprocessing/image/__init__.py
+keras/_tf_keras/keras/preprocessing/sequence/__init__.py
+keras/_tf_keras/keras/quantizers/__init__.py
+keras/_tf_keras/keras/random/__init__.py
+keras/_tf_keras/keras/regularizers/__init__.py
+keras/_tf_keras/keras/saving/__init__.py
+keras/_tf_keras/keras/tree/__init__.py
+keras/_tf_keras/keras/utils/__init__.py
+keras/_tf_keras/keras/utils/legacy/__init__.py
 keras/api/__init__.py
-keras/api/_tf_keras/__init__.py
-keras/api/_tf_keras/keras/__init__.py
-keras/api/_tf_keras/keras/activations/__init__.py
-keras/api/_tf_keras/keras/applications/__init__.py
-keras/api/_tf_keras/keras/applications/convnext/__init__.py
-keras/api/_tf_keras/keras/applications/densenet/__init__.py
-keras/api/_tf_keras/keras/applications/efficientnet/__init__.py
-keras/api/_tf_keras/keras/applications/efficientnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/imagenet_utils/__init__.py
-keras/api/_tf_keras/keras/applications/inception_resnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/inception_v3/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/mobilenet_v3/__init__.py
-keras/api/_tf_keras/keras/applications/nasnet/__init__.py
-keras/api/_tf_keras/keras/applications/resnet/__init__.py
-keras/api/_tf_keras/keras/applications/resnet50/__init__.py
-keras/api/_tf_keras/keras/applications/resnet_v2/__init__.py
-keras/api/_tf_keras/keras/applications/vgg16/__init__.py
-keras/api/_tf_keras/keras/applications/vgg19/__init__.py
-keras/api/_tf_keras/keras/applications/xception/__init__.py
-keras/api/_tf_keras/keras/backend/__init__.py
-keras/api/_tf_keras/keras/callbacks/__init__.py
-keras/api/_tf_keras/keras/config/__init__.py
-keras/api/_tf_keras/keras/constraints/__init__.py
-keras/api/_tf_keras/keras/datasets/__init__.py
-keras/api/_tf_keras/keras/datasets/boston_housing/__init__.py
-keras/api/_tf_keras/keras/datasets/california_housing/__init__.py
-keras/api/_tf_keras/keras/datasets/cifar10/__init__.py
-keras/api/_tf_keras/keras/datasets/cifar100/__init__.py
-keras/api/_tf_keras/keras/datasets/fashion_mnist/__init__.py
-keras/api/_tf_keras/keras/datasets/imdb/__init__.py
-keras/api/_tf_keras/keras/datasets/mnist/__init__.py
-keras/api/_tf_keras/keras/datasets/reuters/__init__.py
-keras/api/_tf_keras/keras/distribution/__init__.py
-keras/api/_tf_keras/keras/dtype_policies/__init__.py
-keras/api/_tf_keras/keras/export/__init__.py
-keras/api/_tf_keras/keras/initializers/__init__.py
-keras/api/_tf_keras/keras/layers/__init__.py
-keras/api/_tf_keras/keras/legacy/__init__.py
-keras/api/_tf_keras/keras/legacy/saving/__init__.py
-keras/api/_tf_keras/keras/losses/__init__.py
-keras/api/_tf_keras/keras/metrics/__init__.py
-keras/api/_tf_keras/keras/mixed_precision/__init__.py
-keras/api/_tf_keras/keras/models/__init__.py
-keras/api/_tf_keras/keras/ops/__init__.py
-keras/api/_tf_keras/keras/ops/image/__init__.py
-keras/api/_tf_keras/keras/ops/linalg/__init__.py
-keras/api/_tf_keras/keras/ops/nn/__init__.py
-keras/api/_tf_keras/keras/ops/numpy/__init__.py
-keras/api/_tf_keras/keras/optimizers/__init__.py
-keras/api/_tf_keras/keras/optimizers/legacy/__init__.py
-keras/api/_tf_keras/keras/optimizers/schedules/__init__.py
-keras/api/_tf_keras/keras/preprocessing/__init__.py
-keras/api/_tf_keras/keras/preprocessing/image/__init__.py
-keras/api/_tf_keras/keras/preprocessing/sequence/__init__.py
-keras/api/_tf_keras/keras/quantizers/__init__.py
-keras/api/_tf_keras/keras/random/__init__.py
-keras/api/_tf_keras/keras/regularizers/__init__.py
-keras/api/_tf_keras/keras/saving/__init__.py
-keras/api/_tf_keras/keras/tree/__init__.py
-keras/api/_tf_keras/keras/utils/__init__.py
-keras/api/_tf_keras/keras/utils/legacy/__init__.py
 keras/api/activations/__init__.py
 keras/api/applications/__init__.py
 keras/api/applications/convnext/__init__.py
 keras/api/applications/densenet/__init__.py
 keras/api/applications/efficientnet/__init__.py
 keras/api/applications/efficientnet_v2/__init__.py
 keras/api/applications/imagenet_utils/__init__.py
@@ -156,23 +132,20 @@
 keras/api/utils/__init__.py
 keras/api/utils/legacy/__init__.py
 keras/src/__init__.py
 keras/src/api_export.py
 keras/src/version.py
 keras/src/activations/__init__.py
 keras/src/activations/activations.py
-keras/src/activations/activations_test.py
 keras/src/applications/__init__.py
-keras/src/applications/applications_test.py
 keras/src/applications/convnext.py
 keras/src/applications/densenet.py
 keras/src/applications/efficientnet.py
 keras/src/applications/efficientnet_v2.py
 keras/src/applications/imagenet_utils.py
-keras/src/applications/imagenet_utils_test.py
 keras/src/applications/inception_resnet_v2.py
 keras/src/applications/inception_v3.py
 keras/src/applications/mobilenet.py
 keras/src/applications/mobilenet_v2.py
 keras/src/applications/mobilenet_v3.py
 keras/src/applications/nasnet.py
 keras/src/applications/resnet.py
@@ -181,32 +154,23 @@
 keras/src/applications/vgg19.py
 keras/src/applications/xception.py
 keras/src/backend/__init__.py
 keras/src/backend/config.py
 keras/src/backend/exports.py
 keras/src/backend/common/__init__.py
 keras/src/backend/common/backend_utils.py
-keras/src/backend/common/backend_utils_test.py
-keras/src/backend/common/compute_output_spec_test.py
 keras/src/backend/common/dtypes.py
-keras/src/backend/common/dtypes_test.py
 keras/src/backend/common/global_state.py
-keras/src/backend/common/global_state_test.py
 keras/src/backend/common/keras_tensor.py
-keras/src/backend/common/keras_tensor_test.py
 keras/src/backend/common/name_scope.py
-keras/src/backend/common/name_scope_test.py
 keras/src/backend/common/stateless_scope.py
-keras/src/backend/common/stateless_scope_test.py
 keras/src/backend/common/variables.py
-keras/src/backend/common/variables_test.py
 keras/src/backend/jax/__init__.py
 keras/src/backend/jax/core.py
 keras/src/backend/jax/distribution_lib.py
-keras/src/backend/jax/distribution_lib_test.py
 keras/src/backend/jax/image.py
 keras/src/backend/jax/layer.py
 keras/src/backend/jax/linalg.py
 keras/src/backend/jax/math.py
 keras/src/backend/jax/nn.py
 keras/src/backend/jax/numpy.py
 keras/src/backend/jax/optimizer.py
@@ -223,28 +187,24 @@
 keras/src/backend/numpy/nn.py
 keras/src/backend/numpy/numpy.py
 keras/src/backend/numpy/random.py
 keras/src/backend/numpy/rnn.py
 keras/src/backend/numpy/trainer.py
 keras/src/backend/tensorflow/__init__.py
 keras/src/backend/tensorflow/core.py
-keras/src/backend/tensorflow/distribute_test.py
 keras/src/backend/tensorflow/distribution_lib.py
 keras/src/backend/tensorflow/image.py
 keras/src/backend/tensorflow/layer.py
 keras/src/backend/tensorflow/linalg.py
 keras/src/backend/tensorflow/math.py
-keras/src/backend/tensorflow/name_scope_test.py
 keras/src/backend/tensorflow/nn.py
 keras/src/backend/tensorflow/numpy.py
 keras/src/backend/tensorflow/optimizer.py
-keras/src/backend/tensorflow/optimizer_distribute_test.py
 keras/src/backend/tensorflow/random.py
 keras/src/backend/tensorflow/rnn.py
-keras/src/backend/tensorflow/saved_model_test.py
 keras/src/backend/tensorflow/sparse.py
 keras/src/backend/tensorflow/tensorboard.py
 keras/src/backend/tensorflow/trackable.py
 keras/src/backend/tensorflow/trainer.py
 keras/src/backend/torch/__init__.py
 keras/src/backend/torch/core.py
 keras/src/backend/torch/image.py
@@ -266,476 +226,293 @@
 keras/src/backend/torch/optimizers/torch_nadam.py
 keras/src/backend/torch/optimizers/torch_optimizer.py
 keras/src/backend/torch/optimizers/torch_parallel_optimizer.py
 keras/src/backend/torch/optimizers/torch_rmsprop.py
 keras/src/backend/torch/optimizers/torch_sgd.py
 keras/src/callbacks/__init__.py
 keras/src/callbacks/backup_and_restore.py
-keras/src/callbacks/backup_and_restore_test.py
 keras/src/callbacks/callback.py
 keras/src/callbacks/callback_list.py
-keras/src/callbacks/callback_test.py
 keras/src/callbacks/csv_logger.py
-keras/src/callbacks/csv_logger_test.py
 keras/src/callbacks/early_stopping.py
-keras/src/callbacks/early_stopping_test.py
 keras/src/callbacks/history.py
 keras/src/callbacks/lambda_callback.py
-keras/src/callbacks/lambda_callback_test.py
 keras/src/callbacks/learning_rate_scheduler.py
-keras/src/callbacks/learning_rate_scheduler_test.py
 keras/src/callbacks/model_checkpoint.py
-keras/src/callbacks/model_checkpoint_test.py
 keras/src/callbacks/progbar_logger.py
 keras/src/callbacks/reduce_lr_on_plateau.py
-keras/src/callbacks/reduce_lr_on_plateau_test.py
 keras/src/callbacks/remote_monitor.py
-keras/src/callbacks/remote_monitor_test.py
 keras/src/callbacks/swap_ema_weights.py
-keras/src/callbacks/swap_ema_weights_test.py
 keras/src/callbacks/tensorboard.py
-keras/src/callbacks/tensorboard_test.py
 keras/src/callbacks/terminate_on_nan.py
-keras/src/callbacks/terminate_on_nan_test.py
 keras/src/constraints/__init__.py
 keras/src/constraints/constraints.py
-keras/src/constraints/constraints_test.py
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
-keras/src/distribution/distribution_lib_test.py
 keras/src/dtype_policies/__init__.py
 keras/src/dtype_policies/dtype_policy.py
-keras/src/dtype_policies/dtype_policy_test.py
 keras/src/export/__init__.py
 keras/src/export/export_lib.py
-keras/src/export/export_lib_test.py
 keras/src/initializers/__init__.py
 keras/src/initializers/constant_initializers.py
-keras/src/initializers/constant_initializers_test.py
 keras/src/initializers/initializer.py
 keras/src/initializers/random_initializers.py
-keras/src/initializers/random_initializers_test.py
 keras/src/layers/__init__.py
 keras/src/layers/input_spec.py
 keras/src/layers/layer.py
-keras/src/layers/layer_test.py
 keras/src/layers/activations/__init__.py
 keras/src/layers/activations/activation.py
-keras/src/layers/activations/activation_test.py
 keras/src/layers/activations/elu.py
-keras/src/layers/activations/elu_test.py
 keras/src/layers/activations/leaky_relu.py
-keras/src/layers/activations/leaky_relu_test.py
 keras/src/layers/activations/prelu.py
-keras/src/layers/activations/prelu_test.py
 keras/src/layers/activations/relu.py
-keras/src/layers/activations/relu_test.py
 keras/src/layers/activations/softmax.py
-keras/src/layers/activations/softmax_test.py
 keras/src/layers/attention/__init__.py
 keras/src/layers/attention/additive_attention.py
-keras/src/layers/attention/additive_attention_test.py
 keras/src/layers/attention/attention.py
-keras/src/layers/attention/attention_test.py
 keras/src/layers/attention/grouped_query_attention.py
-keras/src/layers/attention/grouped_query_attention_test.py
 keras/src/layers/attention/multi_head_attention.py
-keras/src/layers/attention/multi_head_attention_test.py
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
-keras/src/layers/convolutional/conv_test.py
-keras/src/layers/convolutional/conv_transpose_test.py
 keras/src/layers/convolutional/depthwise_conv1d.py
 keras/src/layers/convolutional/depthwise_conv2d.py
-keras/src/layers/convolutional/depthwise_conv_test.py
 keras/src/layers/convolutional/separable_conv1d.py
 keras/src/layers/convolutional/separable_conv2d.py
-keras/src/layers/convolutional/separable_conv_test.py
 keras/src/layers/core/__init__.py
 keras/src/layers/core/dense.py
-keras/src/layers/core/dense_test.py
 keras/src/layers/core/einsum_dense.py
-keras/src/layers/core/einsum_dense_test.py
 keras/src/layers/core/embedding.py
-keras/src/layers/core/embedding_test.py
 keras/src/layers/core/identity.py
-keras/src/layers/core/identity_test.py
 keras/src/layers/core/input_layer.py
-keras/src/layers/core/input_layer_test.py
 keras/src/layers/core/lambda_layer.py
-keras/src/layers/core/lambda_layer_test.py
 keras/src/layers/core/masking.py
-keras/src/layers/core/masking_test.py
 keras/src/layers/core/wrapper.py
-keras/src/layers/core/wrapper_test.py
 keras/src/layers/merging/__init__.py
 keras/src/layers/merging/add.py
 keras/src/layers/merging/average.py
 keras/src/layers/merging/base_merge.py
 keras/src/layers/merging/concatenate.py
 keras/src/layers/merging/dot.py
 keras/src/layers/merging/maximum.py
-keras/src/layers/merging/merging_test.py
 keras/src/layers/merging/minimum.py
 keras/src/layers/merging/multiply.py
 keras/src/layers/merging/subtract.py
 keras/src/layers/normalization/__init__.py
 keras/src/layers/normalization/batch_normalization.py
-keras/src/layers/normalization/batch_normalization_test.py
 keras/src/layers/normalization/group_normalization.py
-keras/src/layers/normalization/group_normalization_test.py
 keras/src/layers/normalization/layer_normalization.py
-keras/src/layers/normalization/layer_normalization_test.py
 keras/src/layers/normalization/spectral_normalization.py
-keras/src/layers/normalization/spectral_normalization_test.py
 keras/src/layers/normalization/unit_normalization.py
-keras/src/layers/normalization/unit_normalization_test.py
 keras/src/layers/pooling/__init__.py
 keras/src/layers/pooling/average_pooling1d.py
 keras/src/layers/pooling/average_pooling2d.py
 keras/src/layers/pooling/average_pooling3d.py
-keras/src/layers/pooling/average_pooling_test.py
 keras/src/layers/pooling/base_global_pooling.py
 keras/src/layers/pooling/base_pooling.py
 keras/src/layers/pooling/global_average_pooling1d.py
 keras/src/layers/pooling/global_average_pooling2d.py
 keras/src/layers/pooling/global_average_pooling3d.py
-keras/src/layers/pooling/global_average_pooling_test.py
 keras/src/layers/pooling/global_max_pooling1d.py
 keras/src/layers/pooling/global_max_pooling2d.py
 keras/src/layers/pooling/global_max_pooling3d.py
-keras/src/layers/pooling/global_max_pooling_test.py
 keras/src/layers/pooling/max_pooling1d.py
 keras/src/layers/pooling/max_pooling2d.py
 keras/src/layers/pooling/max_pooling3d.py
-keras/src/layers/pooling/max_pooling_test.py
 keras/src/layers/preprocessing/__init__.py
 keras/src/layers/preprocessing/audio_preprocessing.py
-keras/src/layers/preprocessing/audio_preprocessing_test.py
 keras/src/layers/preprocessing/category_encoding.py
-keras/src/layers/preprocessing/category_encoding_test.py
 keras/src/layers/preprocessing/center_crop.py
-keras/src/layers/preprocessing/center_crop_test.py
 keras/src/layers/preprocessing/discretization.py
-keras/src/layers/preprocessing/discretization_test.py
 keras/src/layers/preprocessing/feature_space.py
-keras/src/layers/preprocessing/feature_space_test.py
 keras/src/layers/preprocessing/hashed_crossing.py
-keras/src/layers/preprocessing/hashed_crossing_test.py
 keras/src/layers/preprocessing/hashing.py
-keras/src/layers/preprocessing/hashing_test.py
 keras/src/layers/preprocessing/index_lookup.py
-keras/src/layers/preprocessing/index_lookup_test.py
 keras/src/layers/preprocessing/integer_lookup.py
-keras/src/layers/preprocessing/integer_lookup_test.py
 keras/src/layers/preprocessing/normalization.py
-keras/src/layers/preprocessing/normalization_test.py
 keras/src/layers/preprocessing/random_brightness.py
-keras/src/layers/preprocessing/random_brightness_test.py
 keras/src/layers/preprocessing/random_contrast.py
-keras/src/layers/preprocessing/random_contrast_test.py
 keras/src/layers/preprocessing/random_crop.py
-keras/src/layers/preprocessing/random_crop_test.py
 keras/src/layers/preprocessing/random_flip.py
-keras/src/layers/preprocessing/random_flip_test.py
 keras/src/layers/preprocessing/random_rotation.py
-keras/src/layers/preprocessing/random_rotation_test.py
 keras/src/layers/preprocessing/random_translation.py
-keras/src/layers/preprocessing/random_translation_test.py
 keras/src/layers/preprocessing/random_zoom.py
-keras/src/layers/preprocessing/random_zoom_test.py
 keras/src/layers/preprocessing/rescaling.py
-keras/src/layers/preprocessing/rescaling_test.py
 keras/src/layers/preprocessing/resizing.py
-keras/src/layers/preprocessing/resizing_test.py
 keras/src/layers/preprocessing/string_lookup.py
-keras/src/layers/preprocessing/string_lookup_test.py
 keras/src/layers/preprocessing/text_vectorization.py
-keras/src/layers/preprocessing/text_vectorization_test.py
 keras/src/layers/preprocessing/tf_data_layer.py
 keras/src/layers/regularization/__init__.py
 keras/src/layers/regularization/activity_regularization.py
-keras/src/layers/regularization/activity_regularization_test.py
 keras/src/layers/regularization/alpha_dropout.py
-keras/src/layers/regularization/alpha_dropout_test.py
 keras/src/layers/regularization/dropout.py
-keras/src/layers/regularization/dropout_test.py
 keras/src/layers/regularization/gaussian_dropout.py
-keras/src/layers/regularization/gaussian_dropout_test.py
 keras/src/layers/regularization/gaussian_noise.py
-keras/src/layers/regularization/gaussian_noise_test.py
 keras/src/layers/regularization/spatial_dropout.py
-keras/src/layers/regularization/spatial_dropout_test.py
 keras/src/layers/reshaping/__init__.py
 keras/src/layers/reshaping/cropping1d.py
-keras/src/layers/reshaping/cropping1d_test.py
 keras/src/layers/reshaping/cropping2d.py
-keras/src/layers/reshaping/cropping2d_test.py
 keras/src/layers/reshaping/cropping3d.py
-keras/src/layers/reshaping/cropping3d_test.py
 keras/src/layers/reshaping/flatten.py
-keras/src/layers/reshaping/flatten_test.py
 keras/src/layers/reshaping/permute.py
-keras/src/layers/reshaping/permute_test.py
 keras/src/layers/reshaping/repeat_vector.py
-keras/src/layers/reshaping/repeat_vector_test.py
 keras/src/layers/reshaping/reshape.py
-keras/src/layers/reshaping/reshape_test.py
 keras/src/layers/reshaping/up_sampling1d.py
-keras/src/layers/reshaping/up_sampling1d_test.py
 keras/src/layers/reshaping/up_sampling2d.py
-keras/src/layers/reshaping/up_sampling2d_test.py
 keras/src/layers/reshaping/up_sampling3d.py
-keras/src/layers/reshaping/up_sampling3d_test.py
 keras/src/layers/reshaping/zero_padding1d.py
-keras/src/layers/reshaping/zero_padding1d_test.py
 keras/src/layers/reshaping/zero_padding2d.py
-keras/src/layers/reshaping/zero_padding2d_test.py
 keras/src/layers/reshaping/zero_padding3d.py
-keras/src/layers/reshaping/zero_padding3d_test.py
 keras/src/layers/rnn/__init__.py
 keras/src/layers/rnn/bidirectional.py
-keras/src/layers/rnn/bidirectional_test.py
 keras/src/layers/rnn/conv_lstm.py
 keras/src/layers/rnn/conv_lstm1d.py
-keras/src/layers/rnn/conv_lstm1d_test.py
 keras/src/layers/rnn/conv_lstm2d.py
-keras/src/layers/rnn/conv_lstm2d_test.py
 keras/src/layers/rnn/conv_lstm3d.py
-keras/src/layers/rnn/conv_lstm3d_test.py
-keras/src/layers/rnn/conv_lstm_test.py
 keras/src/layers/rnn/dropout_rnn_cell.py
-keras/src/layers/rnn/dropout_rnn_cell_test.py
 keras/src/layers/rnn/gru.py
-keras/src/layers/rnn/gru_test.py
 keras/src/layers/rnn/lstm.py
-keras/src/layers/rnn/lstm_test.py
 keras/src/layers/rnn/rnn.py
-keras/src/layers/rnn/rnn_test.py
 keras/src/layers/rnn/simple_rnn.py
-keras/src/layers/rnn/simple_rnn_test.py
 keras/src/layers/rnn/stacked_rnn_cells.py
-keras/src/layers/rnn/stacked_rnn_cells_test.py
 keras/src/layers/rnn/time_distributed.py
-keras/src/layers/rnn/time_distributed_test.py
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
-keras/src/legacy/saving/json_utils_test.py
 keras/src/legacy/saving/legacy_h5_format.py
-keras/src/legacy/saving/legacy_h5_format_test.py
 keras/src/legacy/saving/saving_options.py
 keras/src/legacy/saving/saving_utils.py
 keras/src/legacy/saving/serialization.py
 keras/src/losses/__init__.py
 keras/src/losses/loss.py
-keras/src/losses/loss_test.py
 keras/src/losses/losses.py
-keras/src/losses/losses_test.py
 keras/src/metrics/__init__.py
 keras/src/metrics/accuracy_metrics.py
-keras/src/metrics/accuracy_metrics_test.py
 keras/src/metrics/confusion_metrics.py
-keras/src/metrics/confusion_metrics_test.py
 keras/src/metrics/f_score_metrics.py
-keras/src/metrics/f_score_metrics_test.py
 keras/src/metrics/hinge_metrics.py
-keras/src/metrics/hinge_metrics_test.py
 keras/src/metrics/iou_metrics.py
-keras/src/metrics/iou_metrics_test.py
 keras/src/metrics/metric.py
-keras/src/metrics/metric_test.py
 keras/src/metrics/metrics_utils.py
 keras/src/metrics/probabilistic_metrics.py
-keras/src/metrics/probabilistic_metrics_test.py
 keras/src/metrics/reduction_metrics.py
-keras/src/metrics/reduction_metrics_test.py
 keras/src/metrics/regression_metrics.py
-keras/src/metrics/regression_metrics_test.py
 keras/src/models/__init__.py
 keras/src/models/cloning.py
-keras/src/models/cloning_test.py
 keras/src/models/functional.py
-keras/src/models/functional_test.py
 keras/src/models/model.py
-keras/src/models/model_test.py
 keras/src/models/sequential.py
-keras/src/models/sequential_test.py
 keras/src/models/variable_mapping.py
-keras/src/models/variable_mapping_test.py
 keras/src/ops/__init__.py
 keras/src/ops/core.py
-keras/src/ops/core_test.py
 keras/src/ops/function.py
-keras/src/ops/function_test.py
 keras/src/ops/image.py
-keras/src/ops/image_test.py
 keras/src/ops/linalg.py
-keras/src/ops/linalg_test.py
 keras/src/ops/math.py
-keras/src/ops/math_test.py
 keras/src/ops/nn.py
-keras/src/ops/nn_test.py
 keras/src/ops/node.py
-keras/src/ops/node_test.py
 keras/src/ops/numpy.py
-keras/src/ops/numpy_test.py
 keras/src/ops/operation.py
-keras/src/ops/operation_test.py
 keras/src/ops/operation_utils.py
-keras/src/ops/operation_utils_test.py
 keras/src/ops/symbolic_arguments.py
-keras/src/ops/symbolic_arguments_test.py
 keras/src/optimizers/__init__.py
 keras/src/optimizers/adadelta.py
-keras/src/optimizers/adadelta_test.py
 keras/src/optimizers/adafactor.py
-keras/src/optimizers/adafactor_test.py
 keras/src/optimizers/adagrad.py
-keras/src/optimizers/adagrad_test.py
 keras/src/optimizers/adam.py
-keras/src/optimizers/adam_test.py
 keras/src/optimizers/adamax.py
-keras/src/optimizers/adamax_test.py
 keras/src/optimizers/adamw.py
-keras/src/optimizers/adamw_test.py
 keras/src/optimizers/base_optimizer.py
 keras/src/optimizers/ftrl.py
-keras/src/optimizers/ftrl_test.py
 keras/src/optimizers/lion.py
-keras/src/optimizers/lion_test.py
 keras/src/optimizers/loss_scale_optimizer.py
-keras/src/optimizers/loss_scale_optimizer_test.py
 keras/src/optimizers/nadam.py
-keras/src/optimizers/nadam_test.py
 keras/src/optimizers/optimizer.py
-keras/src/optimizers/optimizer_sparse_test.py
-keras/src/optimizers/optimizer_test.py
 keras/src/optimizers/rmsprop.py
-keras/src/optimizers/rmsprop_test.py
 keras/src/optimizers/sgd.py
-keras/src/optimizers/sgd_test.py
 keras/src/optimizers/schedules/__init__.py
 keras/src/optimizers/schedules/learning_rate_schedule.py
-keras/src/optimizers/schedules/learning_rate_schedule_test.py
 keras/src/quantizers/__init__.py
 keras/src/quantizers/quantizers.py
-keras/src/quantizers/quantizers_test.py
 keras/src/random/__init__.py
 keras/src/random/random.py
-keras/src/random/random_test.py
 keras/src/random/seed_generator.py
-keras/src/random/seed_generator_test.py
 keras/src/regularizers/__init__.py
 keras/src/regularizers/regularizers.py
-keras/src/regularizers/regularizers_test.py
 keras/src/saving/__init__.py
 keras/src/saving/object_registration.py
-keras/src/saving/object_registration_test.py
 keras/src/saving/saving_api.py
-keras/src/saving/saving_api_test.py
 keras/src/saving/saving_lib.py
-keras/src/saving/saving_lib_test.py
 keras/src/saving/serialization_lib.py
-keras/src/saving/serialization_lib_test.py
 keras/src/testing/__init__.py
 keras/src/testing/test_case.py
 keras/src/testing/test_utils.py
-keras/src/testing/test_utils_test.py
 keras/src/trainers/__init__.py
 keras/src/trainers/compile_utils.py
-keras/src/trainers/compile_utils_test.py
 keras/src/trainers/epoch_iterator.py
-keras/src/trainers/epoch_iterator_test.py
 keras/src/trainers/trainer.py
-keras/src/trainers/trainer_test.py
 keras/src/trainers/data_adapters/__init__.py
 keras/src/trainers/data_adapters/array_data_adapter.py
-keras/src/trainers/data_adapters/array_data_adapter_test.py
 keras/src/trainers/data_adapters/array_slicing.py
 keras/src/trainers/data_adapters/data_adapter.py
 keras/src/trainers/data_adapters/data_adapter_utils.py
 keras/src/trainers/data_adapters/generator_data_adapter.py
-keras/src/trainers/data_adapters/generator_data_adapter_test.py
 keras/src/trainers/data_adapters/py_dataset_adapter.py
-keras/src/trainers/data_adapters/py_dataset_adapter_test.py
 keras/src/trainers/data_adapters/tf_dataset_adapter.py
-keras/src/trainers/data_adapters/tf_dataset_adapter_test.py
 keras/src/trainers/data_adapters/torch_data_loader_adapter.py
-keras/src/trainers/data_adapters/torch_data_loader_adapter_test.py
 keras/src/tree/__init__.py
 keras/src/tree/dmtree_impl.py
 keras/src/tree/optree_impl.py
 keras/src/tree/tree_api.py
-keras/src/tree/tree_test.py
 keras/src/utils/__init__.py
 keras/src/utils/argument_validation.py
 keras/src/utils/audio_dataset_utils.py
-keras/src/utils/audio_dataset_utils_test.py
 keras/src/utils/backend_utils.py
 keras/src/utils/code_stats.py
-keras/src/utils/code_stats_test.py
 keras/src/utils/dataset_utils.py
-keras/src/utils/dataset_utils_test.py
 keras/src/utils/dtype_utils.py
-keras/src/utils/dtype_utils_test.py
 keras/src/utils/file_utils.py
-keras/src/utils/file_utils_test.py
 keras/src/utils/image_dataset_utils.py
-keras/src/utils/image_dataset_utils_test.py
 keras/src/utils/image_utils.py
 keras/src/utils/io_utils.py
-keras/src/utils/io_utils_test.py
 keras/src/utils/jax_layer.py
-keras/src/utils/jax_layer_test.py
 keras/src/utils/jax_utils.py
 keras/src/utils/model_visualization.py
 keras/src/utils/module_utils.py
 keras/src/utils/naming.py
-keras/src/utils/naming_test.py
 keras/src/utils/numerical_utils.py
-keras/src/utils/numerical_utils_test.py
 keras/src/utils/progbar.py
 keras/src/utils/python_utils.py
-keras/src/utils/python_utils_test.py
 keras/src/utils/rng_utils.py
-keras/src/utils/rng_utils_test.py
 keras/src/utils/sequence_utils.py
-keras/src/utils/sequence_utils_test.py
 keras/src/utils/summary_utils.py
-keras/src/utils/summary_utils_test.py
 keras/src/utils/text_dataset_utils.py
-keras/src/utils/text_dataset_utils_test.py
 keras/src/utils/tf_utils.py
 keras/src/utils/timeseries_dataset_utils.py
-keras/src/utils/timeseries_dataset_utils_test.py
 keras/src/utils/torch_utils.py
-keras/src/utils/torch_utils_test.py
 keras/src/utils/traceback_utils.py
-keras/src/utils/tracking.py
-keras/src/utils/tracking_test.py
+keras/src/utils/tracking.py
```

### Comparing `keras-3.3.0/setup.py` & `keras-3.3.1/setup.py`

 * *Files identical despite different names*

