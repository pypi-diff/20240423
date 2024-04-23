# Comparing `tmp/aqtp-0.7.1.tar.gz` & `tmp/aqtp-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aqtp-0.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aqtp-0.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aqtp-0.7.1.tar` & `aqtp-0.7.2.tar`

### file list

```diff
@@ -1,268 +1,268 @@
--rw-r--r--   0        0        0       39 2024-04-10 00:47:50.574357 aqtp-0.7.1/.gitignore
--rw-r--r--   0        0        0      107 2024-04-10 00:47:50.574357 aqtp-0.7.1/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2024-04-10 00:47:50.574357 aqtp-0.7.1/LICENSE
--rw-r--r--   0        0        0    17310 2024-04-10 00:47:50.574357 aqtp-0.7.1/README.md
--rw-r--r--   0        0        0      641 2024-04-10 00:47:50.574357 aqtp-0.7.1/aqt/__init__.py
--rw-r--r--   0        0        0      576 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/__init__.py
--rw-r--r--   0        0        0     4354 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/aqt_common.py
--rw-r--r--   0        0        0    16011 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/aqt_config.py
--rw-r--r--   0        0        0    13928 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/aqt_config_schedule_test.py
--rw-r--r--   0        0        0     5177 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/aqt_config_utils.py
--rw-r--r--   0        0        0    15655 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/emulated_floating_points.py
--rw-r--r--   0        0        0     5730 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/common/emulation_utils.py
--rw-r--r--   0        0        0      576 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/__init__.py
--rw-r--r--   0        0        0    13641 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_conv_general.py
--rw-r--r--   0        0        0    12151 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_conv_general_test.py
--rw-r--r--   0        0        0     8861 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_dot_general.py
--rw-r--r--   0        0        0    14977 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_dot_general_test.py
--rw-r--r--   0        0        0     3693 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_matmul.py
--rw-r--r--   0        0        0     3293 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_matmul_test.py
--rw-r--r--   0        0        0     1083 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax/aqt_ops.py
--rw-r--r--   0        0        0    18180 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/aqt_tensor.py
--rw-r--r--   0        0        0     4751 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/aqt_tensor_test.py
--rw-r--r--   0        0        0     2705 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/aqt_utils.py
--rw-r--r--   0        0        0     4724 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_conv_general.py
--rw-r--r--   0        0        0    27174 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_dot_general.py
--rw-r--r--   0        0        0    36637 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_dot_general_test.py
--rw-r--r--   0        0        0     5166 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_quantizer.py
--rw-r--r--   0        0        0     9282 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_tensor.py
--rw-r--r--   0        0        0     2568 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/aqt_tensor_test.py
--rw-r--r--   0        0        0     2608 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/calibration.py
--rw-r--r--   0        0        0    20547 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/config.py
--rw-r--r--   0        0        0    37619 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/config_test.py
--rw-r--r--   0        0        0     5550 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/examples/examples.ipynb
--rw-r--r--   0        0        0    13343 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/examples/flax_e2e_model.py
--rw-r--r--   0        0        0    14269 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/examples/flax_e2e_model_test.py
--rw-r--r--   0        0        0    18962 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax.py
--rw-r--r--   0        0        0     2380 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax_calibration.py
--rw-r--r--   0        0        0     3835 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax_dg_core.py
--rw-r--r--   0        0        0     7540 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax_test.py
--rw-r--r--   0        0        0     3183 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/freezer.py
--rw-r--r--   0        0        0     7422 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/freezer_test.py
--rw-r--r--   0        0        0     1672 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax/v2/flax/intercept/README.md
--rw-r--r--   0        0        0     6896 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
--rw-r--r--   0        0        0     3997 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
--rw-r--r--   0        0        0     6087 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
--rw-r--r--   0        0        0     8989 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
--rw-r--r--   0        0        0     4731 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/numerics/fp8_numerics.py
--rw-r--r--   0        0        0     8739 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/numerics/fp8_numerics_test.py
--rw-r--r--   0        0        0     4451 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/numerics/int_numerics.py
--rw-r--r--   0        0        0     1426 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/numerics/no_numerics.py
--rw-r--r--   0        0        0     1338 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/numerics/numerics.py
--rw-r--r--   0        0        0     2526 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/pax/pax_base_ops.py
--rw-r--r--   0        0        0     2095 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/pax/pax_base_ops_test.py
--rw-r--r--   0        0        0     1846 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/stochastic_rounding.py
--rw-r--r--   0        0        0    15088 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/tiled_dot_general.py
--rw-r--r--   0        0        0     6972 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/tiled_dot_general_test.py
--rw-r--r--   0        0        0     4802 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/transpose.py
--rw-r--r--   0        0        0     4187 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/transpose_test.py
--rw-r--r--   0        0        0     4543 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax/v2/utils.py
--rw-r--r--   0        0        0     1590 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/__init__.py
--rw-r--r--   0        0        0    14397 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
--rw-r--r--   0        0        0     1921 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/__init__.py
--rw-r--r--   0        0        0    17225 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/compute_cost_utils.py
--rw-r--r--   0        0        0    24127 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/compute_cost_utils_test.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/flax/__init__.py
--rw-r--r--   0        0        0     5671 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/flax/struct.py
--rw-r--r--   0        0        0    35156 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/flax_attention.py
--rw-r--r--   0        0        0    25400 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/flax_attention_test.py
--rw-r--r--   0        0        0    43061 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/flax_layers.py
--rw-r--r--   0        0        0    75454 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/flax_layers_test.py
--rw-r--r--   0        0        0     6897 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/fp_cast.py
--rw-r--r--   0        0        0     7682 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/fp_cast_test.py
--rw-r--r--   0        0        0     9842 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/get_bounds.py
--rw-r--r--   0        0        0    11477 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/get_bounds_test.py
--rw-r--r--   0        0        0     3477 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/hlo_utils.py
--rw-r--r--   0        0        0     2570 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/hlo_utils_test.py
--rw-r--r--   0        0        0    10045 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/__init__.py
--rw-r--r--   0        0        0     1963 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/check_config_util.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/__init__.py
--rw-r--r--   0        0        0     7382 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/base_config.py
--rw-r--r--   0        0        0     1207 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
--rw-r--r--   0        0        0      853 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
--rw-r--r--   0        0        0     1230 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
--rw-r--r--   0        0        0     1439 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
--rw-r--r--   0        0        0     1231 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
--rw-r--r--   0        0        0     2000 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
--rw-r--r--   0        0        0     6443 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
--rw-r--r--   0        0        0     1647 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
--rw-r--r--   0        0        0     7476 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
--rw-r--r--   0        0        0      855 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
--rw-r--r--   0        0        0      855 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
--rw-r--r--   0        0        0      925 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
--rw-r--r--   0        0        0     1439 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
--rw-r--r--   0        0        0     1440 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
--rw-r--r--   0        0        0     1390 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
--rw-r--r--   0        0        0     1514 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
--rw-r--r--   0        0        0     1383 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
--rw-r--r--   0        0        0     1025 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
--rw-r--r--   0        0        0      925 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
--rw-r--r--   0        0        0     1232 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
--rw-r--r--   0        0        0     6856 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
--rw-r--r--   0        0        0     9732 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
--rw-r--r--   0        0        0     2423 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_test.py
--rw-r--r--   0        0        0     2130 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/hparams_config.py
--rw-r--r--   0        0        0   331485 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/imagenet.png
--rw-r--r--   0        0        0     8129 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/input_pipeline.py
--rw-r--r--   0        0        0     7345 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/models.py
--rw-r--r--   0        0        0     9773 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/models_test.py
--rw-r--r--   0        0        0    15474 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/pokebnn.py
--rw-r--r--   0        0        0     3119 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
--rw-r--r--   0        0        0       62 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/requirements.txt
--rw-r--r--   0        0        0     5749 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
--rw-r--r--   0        0        0    19735 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train.py
--rw-r--r--   0        0        0     2611 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_benchmark.py
--rw-r--r--   0        0        0     2547 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_test.py
--rw-r--r--   0        0        0     7991 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_utils.py
--rw-r--r--   0        0        0     5854 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/primitives.py
--rw-r--r--   0        0        0     6508 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/primitives_test.py
--rw-r--r--   0        0        0     3927 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/quant_config.py
--rw-r--r--   0        0        0    63283 2024-04-10 00:47:50.594357 aqtp-0.7.1/aqt/jax_legacy/jax/quantization.py
--rw-r--r--   0        0        0    45534 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/quantization_test.py
--rw-r--r--   0        0        0     1654 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/shape_utils.py
--rw-r--r--   0        0        0    22231 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
--rw-r--r--   0        0        0    23430 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
--rw-r--r--   0        0        0     9798 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/stats.py
--rw-r--r--   0        0        0     6060 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/stats_tag.py
--rw-r--r--   0        0        0     9777 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/stats_tag_test.py
--rw-r--r--   0        0        0    10461 2024-04-10 00:47:50.598357 aqtp-0.7.1/aqt/jax_legacy/jax/stats_test.py
--rw-r--r--   0        0        0     4637 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/test_utils.py
--rw-r--r--   0        0        0     5435 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/train_utils.py
--rw-r--r--   0        0        0     6454 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/train_utils_test.py
--rw-r--r--   0        0        0      995 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/utils.py
--rw-r--r--   0        0        0     2888 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
--rw-r--r--   0        0        0     7056 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
--rw-r--r--   0        0        0    15134 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/decode.py
--rw-r--r--   0        0        0    12107 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
--rw-r--r--   0        0        0    11082 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
--rw-r--r--   0        0        0    13257 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
--rw-r--r--   0        0        0     6573 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
--rw-r--r--   0        0        0     1069 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1069 2024-04-10 00:47:50.578357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
--rw-r--r--   0        0        0     1056 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1041 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
--rw-r--r--   0        0        0     1006 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1193 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
--rw-r--r--   0        0        0      954 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1101 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
--rw-r--r--   0        0        0     1002 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1000 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1042 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
--rw-r--r--   0        0        0     1002 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0      954 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
--rw-r--r--   0        0        0     1060 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
--rw-r--r--   0        0        0     1175 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
--rw-r--r--   0        0        0     1244 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
--rw-r--r--   0        0        0     1664 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
--rw-r--r--   0        0        0     1661 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
--rw-r--r--   0        0        0     1662 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
--rw-r--r--   0        0        0     1662 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
--rw-r--r--   0        0        0     2172 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
--rw-r--r--   0        0        0     1600 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1849 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1323 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1448 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1344 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
--rw-r--r--   0        0        0     1568 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
--rw-r--r--   0        0        0     1801 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
--rw-r--r--   0        0        0     1584 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
--rw-r--r--   0        0        0     1479 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
--rw-r--r--   0        0        0     1495 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
--rw-r--r--   0        0        0     1531 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
--rw-r--r--   0        0        0     1046 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
--rw-r--r--   0        0        0     1245 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
--rw-r--r--   0        0        0     1245 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
--rw-r--r--   0        0        0     1549 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1380 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1380 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2052 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
--rw-r--r--   0        0        0     1340 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
--rw-r--r--   0        0        0     1340 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     2032 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1757 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
--rw-r--r--   0        0        0     1729 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
--rw-r--r--   0        0        0     2133 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
--rw-r--r--   0        0        0     1238 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
--rw-r--r--   0        0        0     1238 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
--rw-r--r--   0        0        0     1587 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1379 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1379 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2123 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
--rw-r--r--   0        0        0     1213 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
--rw-r--r--   0        0        0     1213 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
--rw-r--r--   0        0        0     1554 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
--rw-r--r--   0        0        0     1375 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
--rw-r--r--   0        0        0     1375 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
--rw-r--r--   0        0        0     2063 2024-04-10 00:47:50.582357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
--rw-r--r--   0        0        0     2523 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
--rw-r--r--   0        0        0      995 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
--rw-r--r--   0        0        0     1672 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
--rw-r--r--   0        0        0     2392 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
--rw-r--r--   0        0        0     1222 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
--rw-r--r--   0        0        0     2101 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
--rw-r--r--   0        0        0     3356 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
--rw-r--r--   0        0        0     1531 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
--rw-r--r--   0        0        0     1965 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
--rw-r--r--   0        0        0      382 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
--rw-r--r--   0        0        0     1096 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1014 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
--rw-r--r--   0        0        0     1096 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
--rw-r--r--   0        0        0     1099 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
--rw-r--r--   0        0        0     1018 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
--rw-r--r--   0        0        0      995 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
--rw-r--r--   0        0        0     1925 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
--rw-r--r--   0        0        0    23300 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
--rw-r--r--   0        0        0    33382 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/models.py
--rw-r--r--   0        0        0    38051 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
--rw-r--r--   0        0        0     4055 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/predict.py
--rw-r--r--   0        0        0      160 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
--rw-r--r--   0        0        0    51590 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train.py
--rw-r--r--   0        0        0     5666 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
--rw-r--r--   0        0        0    10503 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
--rw-r--r--   0        0        0     3939 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
--rw-r--r--   0        0        0    25395 2024-04-10 00:47:50.586357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
--rw-r--r--   0        0        0     3284 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
--rw-r--r--   0        0        0      118 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/requirements.txt
--rw-r--r--   0        0        0    10519 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/README.md
--rw-r--r--   0        0        0      577 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/__init__.py
--rw-r--r--   0        0        0     4810 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/analysis_utils.py
--rw-r--r--   0        0        0     5109 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/analysis_utils_test.py
--rw-r--r--   0        0        0     1045 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/common.py
--rw-r--r--   0        0        0     8505 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/config_schema_utils.py
--rw-r--r--   0        0        0    11978 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/config_schema_utils_test.py
--rw-r--r--   0        0        0     6844 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/hparams_utils.py
--rw-r--r--   0        0        0    10185 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/pandas_utils.py
--rw-r--r--   0        0        0    10192 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/pandas_utils_test.py
--rw-r--r--   0        0        0    20428 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/report_utils.py
--rw-r--r--   0        0        0    23689 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/report_utils_test.py
--rw-r--r--   0        0        0     2538 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/summary_utils.py
--rw-r--r--   0        0        0     3451 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/summary_utils_test.py
--rw-r--r--   0        0        0     6640 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/tfevent_utils.py
--rw-r--r--   0        0        0     4307 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/jax_legacy/utils/tfevent_utils_test.py
--rw-r--r--   0        0        0    15648 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/test/aqt_conv_test_base.py
--rw-r--r--   0        0        0    11192 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/test/aqt_matmul_test_base.py
--rw-r--r--   0        0        0    12101 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/test/aqt_stats_test_base.py
--rw-r--r--   0        0        0    23072 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/test/aqt_tensor_test_base.py
--rw-r--r--   0        0        0     4694 2024-04-10 00:47:50.590357 aqtp-0.7.1/aqt/test/aqt_test_shared_base.py
--rw-r--r--   0        0        0   129585 2024-04-10 00:47:50.590357 aqtp-0.7.1/papers/aqt/aqt.pdf
--rw-r--r--   0        0        0     1303 2024-04-10 00:47:50.590357 aqtp-0.7.1/papers/aqt/aqt.tex
--rw-r--r--   0        0        0     1468 2024-04-10 00:47:50.590357 aqtp-0.7.1/papers/pokebnn/README.md
--rw-r--r--   0        0        0     2862 2024-04-10 00:47:50.594357 aqtp-0.7.1/papers/pokebnn/cloudtpu_train_pokebnn.sh
--rw-r--r--   0        0        0   117523 2024-04-10 00:47:50.594357 aqtp-0.7.1/papers/pokebnn/tensorboard.ipynb
--rw-r--r--   0        0        0      727 2024-04-10 00:47:50.594357 aqtp-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1852 2024-04-10 00:47:50.594357 aqtp-0.7.1/setup.py
--rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       39 2024-04-23 00:00:20.337048 aqtp-0.7.2/.gitignore
+-rw-r--r--   0        0        0      107 2024-04-23 00:00:20.341048 aqtp-0.7.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2024-04-23 00:00:20.341048 aqtp-0.7.2/LICENSE
+-rw-r--r--   0        0        0    17310 2024-04-23 00:00:20.341048 aqtp-0.7.2/README.md
+-rw-r--r--   0        0        0      641 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/__init__.py
+-rw-r--r--   0        0        0      576 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/__init__.py
+-rw-r--r--   0        0        0     4354 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_common.py
+-rw-r--r--   0        0        0    16011 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config.py
+-rw-r--r--   0        0        0    13928 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config_schedule_test.py
+-rw-r--r--   0        0        0     5177 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/aqt_config_utils.py
+-rw-r--r--   0        0        0    15655 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/emulated_floating_points.py
+-rw-r--r--   0        0        0     5730 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/common/emulation_utils.py
+-rw-r--r--   0        0        0      576 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/__init__.py
+-rw-r--r--   0        0        0    13641 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_conv_general.py
+-rw-r--r--   0        0        0    12151 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_conv_general_test.py
+-rw-r--r--   0        0        0     8861 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_dot_general.py
+-rw-r--r--   0        0        0    14977 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     3693 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_matmul.py
+-rw-r--r--   0        0        0     3293 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_matmul_test.py
+-rw-r--r--   0        0        0     1083 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax/aqt_ops.py
+-rw-r--r--   0        0        0    18180 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_tensor.py
+-rw-r--r--   0        0        0     4751 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2705 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/aqt_utils.py
+-rw-r--r--   0        0        0     4724 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_conv_general.py
+-rw-r--r--   0        0        0    29466 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_dot_general.py
+-rw-r--r--   0        0        0    36485 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_dot_general_test.py
+-rw-r--r--   0        0        0     5305 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_quantizer.py
+-rw-r--r--   0        0        0     9578 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_tensor.py
+-rw-r--r--   0        0        0     2568 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/aqt_tensor_test.py
+-rw-r--r--   0        0        0     2608 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/calibration.py
+-rw-r--r--   0        0        0    20942 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/config.py
+-rw-r--r--   0        0        0    37619 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/config_test.py
+-rw-r--r--   0        0        0     5550 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/examples.ipynb
+-rw-r--r--   0        0        0    15399 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model.py
+-rw-r--r--   0        0        0    25621 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model_test.py
+-rw-r--r--   0        0        0    20961 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax.py
+-rw-r--r--   0        0        0     7542 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_calibration.py
+-rw-r--r--   0        0        0     3835 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_dg_core.py
+-rw-r--r--   0        0        0     7540 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_test.py
+-rw-r--r--   0        0        0     3183 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax/v2/flax/freezer.py
+-rw-r--r--   0        0        0     7422 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/freezer_test.py
+-rw-r--r--   0        0        0     1672 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/README.md
+-rw-r--r--   0        0        0     6896 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py
+-rw-r--r--   0        0        0     3997 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py
+-rw-r--r--   0        0        0     6087 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py
+-rw-r--r--   0        0        0     8989 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py
+-rw-r--r--   0        0        0     4731 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics.py
+-rw-r--r--   0        0        0     8823 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics_test.py
+-rw-r--r--   0        0        0     4451 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/int_numerics.py
+-rw-r--r--   0        0        0     1426 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/no_numerics.py
+-rw-r--r--   0        0        0     1338 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/numerics/numerics.py
+-rw-r--r--   0        0        0     2539 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops.py
+-rw-r--r--   0        0        0     2095 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops_test.py
+-rw-r--r--   0        0        0     1846 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/stochastic_rounding.py
+-rw-r--r--   0        0        0    15088 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/tiled_dot_general.py
+-rw-r--r--   0        0        0     6972 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/tiled_dot_general_test.py
+-rw-r--r--   0        0        0     6727 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/transpose.py
+-rw-r--r--   0        0        0     4741 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/transpose_test.py
+-rw-r--r--   0        0        0     3680 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax/v2/utils.py
+-rw-r--r--   0        0        0     1590 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/__init__.py
+-rw-r--r--   0        0        0    14397 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb
+-rw-r--r--   0        0        0     1921 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/__init__.py
+-rw-r--r--   0        0        0    17225 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils.py
+-rw-r--r--   0        0        0    24127 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils_test.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax/__init__.py
+-rw-r--r--   0        0        0     5671 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax/struct.py
+-rw-r--r--   0        0        0    35156 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention.py
+-rw-r--r--   0        0        0    25400 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention_test.py
+-rw-r--r--   0        0        0    43061 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers.py
+-rw-r--r--   0        0        0    75454 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers_test.py
+-rw-r--r--   0        0        0     6897 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast.py
+-rw-r--r--   0        0        0     7682 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast_test.py
+-rw-r--r--   0        0        0     9842 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds.py
+-rw-r--r--   0        0        0    11477 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds_test.py
+-rw-r--r--   0        0        0     3477 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils.py
+-rw-r--r--   0        0        0     2570 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils_test.py
+-rw-r--r--   0        0        0    10045 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/__init__.py
+-rw-r--r--   0        0        0     1963 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/check_config_util.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py
+-rw-r--r--   0        0        0     7382 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py
+-rw-r--r--   0        0        0     1207 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py
+-rw-r--r--   0        0        0      853 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py
+-rw-r--r--   0        0        0     1230 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py
+-rw-r--r--   0        0        0     1439 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py
+-rw-r--r--   0        0        0     1231 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py
+-rw-r--r--   0        0        0     2000 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py
+-rw-r--r--   0        0        0     6443 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py
+-rw-r--r--   0        0        0     1647 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py
+-rw-r--r--   0        0        0     7476 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py
+-rw-r--r--   0        0        0      855 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py
+-rw-r--r--   0        0        0      855 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py
+-rw-r--r--   0        0        0      925 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py
+-rw-r--r--   0        0        0     1439 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py
+-rw-r--r--   0        0        0     1440 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py
+-rw-r--r--   0        0        0     1390 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py
+-rw-r--r--   0        0        0     1514 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py
+-rw-r--r--   0        0        0     1383 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py
+-rw-r--r--   0        0        0     1025 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py
+-rw-r--r--   0        0        0      925 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py
+-rw-r--r--   0        0        0     1232 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py
+-rw-r--r--   0        0        0     6856 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py
+-rw-r--r--   0        0        0     9732 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py
+-rw-r--r--   0        0        0     2423 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_test.py
+-rw-r--r--   0        0        0     2130 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/hparams_config.py
+-rw-r--r--   0        0        0   331485 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/imagenet.png
+-rw-r--r--   0        0        0     8129 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py
+-rw-r--r--   0        0        0     7345 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models.py
+-rw-r--r--   0        0        0     9773 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models_test.py
+-rw-r--r--   0        0        0    15474 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn.py
+-rw-r--r--   0        0        0     3119 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py
+-rw-r--r--   0        0        0       62 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/requirements.txt
+-rw-r--r--   0        0        0     5749 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py
+-rw-r--r--   0        0        0    19735 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train.py
+-rw-r--r--   0        0        0     2611 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py
+-rw-r--r--   0        0        0     2547 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_test.py
+-rw-r--r--   0        0        0     7991 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_utils.py
+-rw-r--r--   0        0        0     5854 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/primitives.py
+-rw-r--r--   0        0        0     6508 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/primitives_test.py
+-rw-r--r--   0        0        0     3927 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quant_config.py
+-rw-r--r--   0        0        0    63283 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quantization.py
+-rw-r--r--   0        0        0    45534 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/quantization_test.py
+-rw-r--r--   0        0        0     1654 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/shape_utils.py
+-rw-r--r--   0        0        0    22231 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py
+-rw-r--r--   0        0        0    23430 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py
+-rw-r--r--   0        0        0     9798 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats.py
+-rw-r--r--   0        0        0     6060 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag.py
+-rw-r--r--   0        0        0     9777 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag_test.py
+-rw-r--r--   0        0        0    10461 2024-04-23 00:00:20.357049 aqtp-0.7.2/aqt/jax_legacy/jax/stats_test.py
+-rw-r--r--   0        0        0     4637 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/test_utils.py
+-rw-r--r--   0        0        0     5435 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/train_utils.py
+-rw-r--r--   0        0        0     6454 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/train_utils_test.py
+-rw-r--r--   0        0        0      995 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/utils.py
+-rw-r--r--   0        0        0     2888 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py
+-rw-r--r--   0        0        0     7056 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py
+-rw-r--r--   0        0        0    15134 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py
+-rw-r--r--   0        0        0    12107 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py
+-rw-r--r--   0        0        0    11082 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py
+-rw-r--r--   0        0        0    13257 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py
+-rw-r--r--   0        0        0     6573 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py
+-rw-r--r--   0        0        0     1069 2024-04-23 00:00:20.341048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1069 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py
+-rw-r--r--   0        0        0     1056 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1041 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py
+-rw-r--r--   0        0        0     1006 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1193 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py
+-rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1101 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py
+-rw-r--r--   0        0        0     1002 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1000 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1042 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py
+-rw-r--r--   0        0        0     1002 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0      954 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py
+-rw-r--r--   0        0        0     1060 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py
+-rw-r--r--   0        0        0     1175 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py
+-rw-r--r--   0        0        0     1244 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py
+-rw-r--r--   0        0        0     1664 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py
+-rw-r--r--   0        0        0     1661 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py
+-rw-r--r--   0        0        0     1662 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py
+-rw-r--r--   0        0        0     1662 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py
+-rw-r--r--   0        0        0     2172 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py
+-rw-r--r--   0        0        0     1600 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1849 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1323 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1448 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1344 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py
+-rw-r--r--   0        0        0     1568 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py
+-rw-r--r--   0        0        0     1801 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py
+-rw-r--r--   0        0        0     1584 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py
+-rw-r--r--   0        0        0     1479 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py
+-rw-r--r--   0        0        0     1495 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py
+-rw-r--r--   0        0        0     1531 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py
+-rw-r--r--   0        0        0     1046 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py
+-rw-r--r--   0        0        0     1245 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py
+-rw-r--r--   0        0        0     1245 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py
+-rw-r--r--   0        0        0     1549 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1380 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1380 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2052 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py
+-rw-r--r--   0        0        0     1340 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py
+-rw-r--r--   0        0        0     1340 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     2032 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1757 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py
+-rw-r--r--   0        0        0     1729 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py
+-rw-r--r--   0        0        0     2133 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1238 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1238 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1587 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1379 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1379 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2123 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py
+-rw-r--r--   0        0        0     1213 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py
+-rw-r--r--   0        0        0     1213 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py
+-rw-r--r--   0        0        0     1554 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     1375 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py
+-rw-r--r--   0        0        0     1375 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py
+-rw-r--r--   0        0        0     2063 2024-04-23 00:00:20.345049 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py
+-rw-r--r--   0        0        0     2523 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py
+-rw-r--r--   0        0        0      995 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1672 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py
+-rw-r--r--   0        0        0     2392 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py
+-rw-r--r--   0        0        0     1222 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py
+-rw-r--r--   0        0        0     2101 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py
+-rw-r--r--   0        0        0     3356 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py
+-rw-r--r--   0        0        0     1531 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py
+-rw-r--r--   0        0        0     1965 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py
+-rw-r--r--   0        0        0      382 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py
+-rw-r--r--   0        0        0     1096 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1014 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py
+-rw-r--r--   0        0        0     1096 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py
+-rw-r--r--   0        0        0     1099 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py
+-rw-r--r--   0        0        0     1018 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py
+-rw-r--r--   0        0        0      995 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py
+-rw-r--r--   0        0        0     1925 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py
+-rw-r--r--   0        0        0    23300 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py
+-rw-r--r--   0        0        0    33382 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models.py
+-rw-r--r--   0        0        0    38051 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py
+-rw-r--r--   0        0        0     4055 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py
+-rw-r--r--   0        0        0      160 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/requirements.txt
+-rw-r--r--   0        0        0    51590 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train.py
+-rw-r--r--   0        0        0     5666 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py
+-rw-r--r--   0        0        0    10503 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py
+-rw-r--r--   0        0        0     3939 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py
+-rw-r--r--   0        0        0    25395 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py
+-rw-r--r--   0        0        0     3284 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py
+-rw-r--r--   0        0        0      118 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/requirements.txt
+-rw-r--r--   0        0        0    10519 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/README.md
+-rw-r--r--   0        0        0      577 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/__init__.py
+-rw-r--r--   0        0        0     4810 2024-04-23 00:00:20.349048 aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils.py
+-rw-r--r--   0        0        0     5109 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils_test.py
+-rw-r--r--   0        0        0     1045 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/common.py
+-rw-r--r--   0        0        0     8505 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils.py
+-rw-r--r--   0        0        0    11978 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils_test.py
+-rw-r--r--   0        0        0     6844 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/hparams_utils.py
+-rw-r--r--   0        0        0    10185 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils.py
+-rw-r--r--   0        0        0    10192 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils_test.py
+-rw-r--r--   0        0        0    20428 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/report_utils.py
+-rw-r--r--   0        0        0    23689 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/report_utils_test.py
+-rw-r--r--   0        0        0     2538 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils.py
+-rw-r--r--   0        0        0     3451 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils_test.py
+-rw-r--r--   0        0        0     6640 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils.py
+-rw-r--r--   0        0        0     4307 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils_test.py
+-rw-r--r--   0        0        0    15648 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_conv_test_base.py
+-rw-r--r--   0        0        0    11192 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_matmul_test_base.py
+-rw-r--r--   0        0        0    12101 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_stats_test_base.py
+-rw-r--r--   0        0        0    23072 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_tensor_test_base.py
+-rw-r--r--   0        0        0     4694 2024-04-23 00:00:20.353049 aqtp-0.7.2/aqt/test/aqt_test_shared_base.py
+-rw-r--r--   0        0        0   129585 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/aqt/aqt.pdf
+-rw-r--r--   0        0        0     1303 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/aqt/aqt.tex
+-rw-r--r--   0        0        0     1468 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/pokebnn/README.md
+-rw-r--r--   0        0        0     2862 2024-04-23 00:00:20.353049 aqtp-0.7.2/papers/pokebnn/cloudtpu_train_pokebnn.sh
+-rw-r--r--   0        0        0   117523 2024-04-23 00:00:20.357049 aqtp-0.7.2/papers/pokebnn/tensorboard.ipynb
+-rw-r--r--   0        0        0      727 2024-04-23 00:00:20.357049 aqtp-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1852 2024-04-23 00:00:20.357049 aqtp-0.7.2/setup.py
+-rw-r--r--   0        0        0    18058 1970-01-01 00:00:00.000000 aqtp-0.7.2/PKG-INFO
```

### Comparing `aqtp-0.7.1/LICENSE` & `aqtp-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/README.md` & `aqtp-0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/__init__.py` & `aqtp-0.7.2/aqt/common/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,10 +7,8 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""Accurate Quantized Training library."""
 
-__version__ = "0.7.1"
```

### Comparing `aqtp-0.7.1/aqt/common/__init__.py` & `aqtp-0.7.2/aqt/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/aqt_common.py` & `aqtp-0.7.2/aqt/common/aqt_common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/aqt_config.py` & `aqtp-0.7.2/aqt/common/aqt_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/aqt_config_schedule_test.py` & `aqtp-0.7.2/aqt/common/aqt_config_schedule_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/aqt_config_utils.py` & `aqtp-0.7.2/aqt/common/aqt_config_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/emulated_floating_points.py` & `aqtp-0.7.2/aqt/common/emulated_floating_points.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/common/emulation_utils.py` & `aqtp-0.7.2/aqt/common/emulation_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,7 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+
```

### Comparing `aqtp-0.7.1/aqt/jax/aqt_conv_general.py` & `aqtp-0.7.2/aqt/jax/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_conv_general_test.py` & `aqtp-0.7.2/aqt/jax/aqt_conv_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_dot_general.py` & `aqtp-0.7.2/aqt/jax/aqt_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_dot_general_test.py` & `aqtp-0.7.2/aqt/jax/aqt_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_matmul.py` & `aqtp-0.7.2/aqt/jax/aqt_matmul.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_matmul_test.py` & `aqtp-0.7.2/aqt/jax/aqt_matmul_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_ops.py` & `aqtp-0.7.2/aqt/jax/aqt_ops.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_tensor.py` & `aqtp-0.7.2/aqt/jax/aqt_tensor.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_tensor_test.py` & `aqtp-0.7.2/aqt/jax/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/aqt_utils.py` & `aqtp-0.7.2/aqt/jax/aqt_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_conv_general.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_conv_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_dot_general.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_dot_general.py`

 * *Files 6% similar despite different names*

```diff
@@ -232,23 +232,50 @@
   return qt.replace(scale_t=list_scale_t)
 
 
 @utils.flax_slots_dataclass
 class DotGeneralQuantizer(abc.ABC):
   """Abstract class for dot_general quantizer."""
 
-  @abc.abstractmethod
   def __call__(
       self,
       lhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
       rhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
   ) -> tuple[
       tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
       tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
   ]:
+    lhs, _ = lhs_quantization_info
+    rhs, _ = rhs_quantization_info
+    lhs_qt, rhs_qt = self.calibrate(
+        lhs_quantization_info, rhs_quantization_info
+    )
+    return self.calculate_qvalue(lhs, lhs_qt, rhs, rhs_qt)
+
+  @abc.abstractmethod
+  def calibrate(
+      self,
+      lhs_quantization_info: tuple[jax.Array, Sequence[int]],
+      rhs_quantization_info: tuple[jax.Array, Sequence[int]],
+  ) -> tuple[aqt_tensor.QTensor, aqt_tensor.QTensor]:
+    """Calculates incomplete QTensor from the given inputs."""
+    pass
+
+  @abc.abstractmethod
+  def calculate_qvalue(
+      self,
+      lhs: jax.Array,
+      lhs_qt: aqt_tensor.QTensor,
+      rhs: jax.Array,
+      rhs_qt: aqt_tensor.QTensor,
+  ) -> tuple[
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+      tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
+  ]:
+    """Calculates qvalues from the given inputs."""
     pass
 
   @abc.abstractmethod
   def swap_lhs_and_rhs(self) -> None:
     """Swaps lhs and rhs configuration."""
     pass
 
@@ -275,28 +302,40 @@
 @utils.flax_slots_dataclass
 class DefaultDotGeneralQuantizer(DotGeneralQuantizer):
   """Default dot_general quantizer."""
 
   lhs: aqt_quantizer.Quantizer
   rhs: aqt_quantizer.Quantizer
 
-  def __call__(
+  def calibrate(
       self,
-      lhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
-      rhs_quantization_info: tuple[jax.Array, Sequence[utils.AxisIdx]],
+      lhs_quantization_info: tuple[jax.Array, Sequence[int]],
+      rhs_quantization_info: tuple[jax.Array, Sequence[int]],
+  ) -> tuple[aqt_tensor.QTensor, aqt_tensor.QTensor]:
+    lhs_input, lhs_ca = lhs_quantization_info
+    rhs_input, rhs_ca = rhs_quantization_info
+    lhs_qt = self.lhs.calibrate(lhs_input, calibration_axes=lhs_ca)
+    rhs_qt = self.rhs.calibrate(rhs_input, calibration_axes=rhs_ca)
+    return (lhs_qt, rhs_qt)
+
+  def calculate_qvalue(
+      self,
+      lhs: jax.Array,
+      lhs_qt: aqt_tensor.QTensor,
+      rhs: jax.Array,
+      rhs_qt: aqt_tensor.QTensor,
   ) -> tuple[
       tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
       tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn],
   ]:
-    lhs_input, lhs_ca = lhs_quantization_info
-    rhs_input, rhs_ca = rhs_quantization_info
-    lhs_qt, lhs_quant_grad = self.lhs.quant(lhs_input, calibration_axes=lhs_ca)
-    rhs_qt, rhs_quant_grad = self.rhs.quant(rhs_input, calibration_axes=rhs_ca)
+    """Calculates qvalues from the given inputs."""
+    lhs_qt, lhs_grad = self.lhs.calculate_qvalue(lhs, lhs_qt)
+    rhs_qt, rhs_grad = self.rhs.calculate_qvalue(rhs, rhs_qt)
 
-    return (lhs_qt, lhs_quant_grad), (rhs_qt, rhs_quant_grad)
+    return (lhs_qt, lhs_grad), (rhs_qt, rhs_grad)
 
   def swap_lhs_and_rhs(self) -> None:
     self.lhs, self.rhs = self.rhs, self.lhs
 
   def assert_calib_shared_axes_value(
       self,
       lhs_val: Sequence[utils.AxisIdx] | None,
@@ -465,16 +504,29 @@
               rhs_shape=rhs.shape,
           )
         return output_qtensor, quant_grad
 
       lhs_calib_axes = _get_calibration_axes(self.lhs, lhs.ndim, lhs_ca, lhs_ba)
       rhs_calib_axes = _get_calibration_axes(self.rhs, rhs.ndim, rhs_ca, rhs_ba)
 
-      lhs_quantized, rhs_quantized = (
-          self.dg_quantizer((lhs, lhs_calib_axes), (rhs, rhs_calib_axes))
+      lhs_incomplete_qt, rhs_incomplete_qt = self.dg_quantizer.calibrate(
+          (lhs, lhs_calib_axes), (rhs, rhs_calib_axes)
+      )
+      if lhs_qt is not None and not lhs_qt.is_full():
+        # Incomplete QTensor is provided as lhs_qt.
+        lhs_incomplete_qt = lhs_qt
+        lhs_qt = None
+
+      if rhs_qt is not None and not rhs_qt.is_full():
+        # Incomplete QTensor is provided as rhs_qt.
+        rhs_incomplete_qt = rhs_qt
+        rhs_qt = None
+
+      lhs_quantized, rhs_quantized = self.dg_quantizer.calculate_qvalue(
+          lhs, lhs_incomplete_qt, rhs, rhs_incomplete_qt
       )
       lhs_qt_calculated, lhs_quant_grad = lhs_quantized
       rhs_qt_calculated, rhs_quant_grad = rhs_quantized
 
       lhs_qt, lhs_quant_grad = _postprocess_qtensor(
           lhs_qt,
           lhs_qt_calculated,
@@ -499,18 +551,15 @@
 
       out = _qtensor_dot_general(
           lhs_qt, rhs_qt, dimension_numbers, self, jnp.promote_types(lhs, rhs)
       )
 
       out = out.dequant()
 
-      res = DotGeneralRes(
-          lhs=lhs_res,
-          rhs=rhs_res,
-      )
+      res = DotGeneralRes(lhs=lhs_res, rhs=rhs_res)
       if self.local_aqt is not None:
         assert len(lhs_ca) == len(rhs_ca)
         if len(lhs_ca) > 0:
           out = jnp.sum(out, axis=0)
         # We are not supporting local AQT in fwd pass, so no res needed.
         res = None
       return out, res
@@ -565,14 +614,29 @@
     for scale in rhs_qt.scale:
       transposed_scale = transpose.rhs_scale_transpose_for_lhs_input(
           scale, dimension_numbers, lhs_qt.shape
       )
       assert isinstance(transposed_scale, jnp.ndarray)  # make pytype quiet
       lhs_qin = lhs_qin * transposed_scale.astype(lhs_qin.dtype)
 
+  if jax.local_devices()[0].platform == 'cpu':
+    # needed bet lax.dot_general(int4, int4) is illegal on cpu.
+    # TODO(aqt): Remove this platform check once
+    # https://github.com/google/jax/issues/19682 is fixed.
+    # TODO(yichizh): It's better to assert False here with the following msg
+    # msg = (
+    #     'lax.dot_general(int4, int4) is illegal on cpu:'
+    #     ' https://github.com/google/jax/issues/19682. The simple workaround'
+    #     ' is to upcast to int8, but in that case please directly set the'
+    #     ' numerics bits to int8. Please contact the AQT team if you believe'
+    #     ' the workaround is needed.'
+    # )
+    if lhs_qin.dtype == jnp.int4 and rhs_qin.dtype == jnp.int4:
+      lhs_qin = lhs_qin.astype(jnp.int8)
+      rhs_qin = rhs_qin.astype(jnp.int8)
   out = cfg.dot_general(
       lhs_qin,
       rhs_qin,
       dimension_numbers=dimension_numbers,
       preferred_element_type=cfg.dg_accumulator_dtype,
       precision=lax.Precision.DEFAULT,
   )
@@ -813,15 +877,7 @@
       cfg.drhs,
       True,
   )
   # fwd_dimension_numbers are marked as nondiff_argnums instead of returning
   # None as grad to it. This is because it is a tuple of Python integers
   # that cannot be traced by Jax.
   return (dlhs, drhs, None, None, None)
-
-
-def make_dot_general(dg: Optional[DotGeneral]):
-  # TODO(lew): call warnings.warn("Deprecated")
-  if dg is None:
-    return jax.lax.dot_general
-  else:
-    return dg
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_dot_general_test.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_dot_general_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 import flax.struct
 import jax
 import jax.numpy as jnp
 import numpy as np
 import scipy.stats
 
 
-def test_jaxpr_dtype(f, cfgs: list[aqt.DotGeneralRaw], float_dtype):
-  """Tests whether dot_generals in f conform to dtypes inside of cfgs."""
+def test_jaxpr_dtype(f, dg_raws: list[aqt.DotGeneralRaw], float_dtype):
+  """Tests whether dot_generals in f conform to dtypes inside of dg_raws."""
 
   def jaxpr_to_trityp(jaxpr):
     for eq in jaxpr.eqns:
       # This is where dot_generals hide when one uses custom vjp
       if "fun_jaxpr" in eq.params.keys():
         for rec in jaxpr_to_trityp(eq.params["fun_jaxpr"]):
           yield rec
@@ -51,27 +51,27 @@
         [lhs, rhs] = eq.invars
         [out] = eq.outvars
         trityp = (lhs.aval, rhs.aval, out.aval)
         yield trityp
 
   f_jaxpr = jax.make_jaxpr(f)()
   trityps = [trityp for trityp in jaxpr_to_trityp(f_jaxpr)]
-  assert len(trityps) == len(cfgs)
-  for (lhs_sa, rhs_sa, out_sa), cfg in zip(trityps, cfgs):
+  assert len(trityps) == len(dg_raws)
+  for (lhs_sa, rhs_sa, out_sa), dg_raw in zip(trityps, dg_raws):
     # If cfg has None, the type is inherited from the arguments' type.
     def assert_dtype_eq(dtype1, dtype2):
       assert dtype1 == dtype2, f"dtype1 != dtype2: {dtype1=} != {dtype2=}"
 
-    assert isinstance(cfg.dg_quantizer, aqt.DefaultDotGeneralQuantizer)
+    assert isinstance(dg_raw.dg_quantizer, aqt.DefaultDotGeneralQuantizer)
 
-    lhs_dtype = cfg.dg_quantizer.lhs.numerics.get_dtype()
-    rhs_dtype = cfg.dg_quantizer.rhs.numerics.get_dtype()
+    lhs_dtype = dg_raw.dg_quantizer.lhs.numerics.get_dtype()
+    rhs_dtype = dg_raw.dg_quantizer.rhs.numerics.get_dtype()
     assert_dtype_eq(lhs_sa.dtype, lhs_dtype or float_dtype)
     assert_dtype_eq(rhs_sa.dtype, rhs_dtype or float_dtype)
-    assert_dtype_eq(out_sa.dtype, cfg.dg_accumulator_dtype or float_dtype)
+    assert_dtype_eq(out_sa.dtype, dg_raw.dg_accumulator_dtype or float_dtype)
 
 
 def rand_unif(shape, maxval, seed, dtype=jnp.float32):
   key = jax.random.PRNGKey(seed)
   return jax.random.uniform(
       key=key, shape=shape, minval=-maxval, maxval=maxval, dtype=dtype
   )
@@ -138,15 +138,15 @@
     if options["test_gradient"]:
       test_eq(f"{name}: gl", good_gl, gl / gl_mult)  # backward pass  # pytype: disable=unsupported-operands
       test_eq(f"{name}: gr", good_gr, gr / gr_mult)  # backward pass  # pytype: disable=unsupported-operands
 
 
 def fqt_param_dict(s, use_fwd_quant, **kwargs):
   return dict(
-      cfg=config.fully_quantized(
+      dg=config.fully_quantized(
           use_fwd_quant=use_fwd_quant,
           use_stochastic_rounding=False,
           **kwargs,
       ),
       seed=s,
   )
 
@@ -171,31 +171,31 @@
 
   def vjp_bwd(self, res, grad):
     (x,) = res
     ret = grad * (x >= 0)
     return (ret, None)
 
 
-def _modify_cfg(
-    readonly_cfg: aqt.DotGeneral,
+def _modify_dg(
+    readonly_dg: aqt.DotGeneral,
     *,
     lhs_dequant_mode: aqt.DequantMode = aqt.DequantMode.OUTPUT,
     rhs_dequant_mode: aqt.DequantMode = aqt.DequantMode.OUTPUT,
     lhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     rhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     use_fwd_quant: bool | None = None,
     fwd_lhs_tricky_clip_and_round: bool = False,
     local_aqt: aqt.LocalAqt | None = None,
     clip_gradient: bool = False,
 ) -> aqt.DotGeneral:
-  cfg = copy.deepcopy(readonly_cfg)
+  dg = copy.deepcopy(readonly_dg)
   if fwd_lhs_tricky_clip_and_round:
     # Tricky means that we have zero gradient on x < 0
-    cfg.fwd.dg_quantizer.lhs.numerics = _TrickyNumerics()
-    cfg.fwd.dg_accumulator_dtype = None
+    dg.fwd.dg_quantizer.lhs.numerics = _TrickyNumerics()
+    dg.fwd.dg_accumulator_dtype = None
 
   # Setting po2_scale is ensuring that fake_quant and full dot_general
   # have the same numerics when scales are power of two (po2).
   # We are passing dims to config so that we can reuse it in fake_quant.
   # Power-of-2 scales allow FQ and AQT to be exactly the same.
   def _apply_po2_scale(c):
     c.dg_quantizer.lhs.po2_scale = True
@@ -219,15 +219,15 @@
           c.dg_quantizer.rhs.numerics.replace(dtype=None)
       )
     if on_lhs or on_rhs:
       c.dg_accumulator_dtype = None
 
   disable_lhs_quant = lhs_dequant_mode == aqt.DequantMode.THIS_INPUT
   disable_rhs_quant = rhs_dequant_mode == aqt.DequantMode.THIS_INPUT
-  for c in [cfg.fwd, cfg.dlhs, cfg.drhs]:
+  for c in [dg.fwd, dg.dlhs, dg.drhs]:
     _apply_po2_scale(c)
     _apply_dequant_mode(c, lhs_dequant_mode, rhs_dequant_mode)
     _apply_calibration_mode(
         c, lhs_calibration_mode, rhs_calibration_mode
     )
     _disable_quant_types(c, disable_lhs_quant, disable_rhs_quant)
 
@@ -242,133 +242,132 @@
             c.dg_quantizer.lhs.numerics.replace(round=False)
         )
       if isinstance(c.dg_quantizer.rhs.numerics, int_numerics.IntNumerics):
         c.dg_quantizer.rhs.numerics = (
             c.dg_quantizer.rhs.numerics.replace(round=False)
         )
 
-    disable_quant(cfg.fwd)
-    disable_quant(cfg.dlhs)
-    disable_quant(cfg.drhs)
+    disable_quant(dg.fwd)
+    disable_quant(dg.dlhs)
+    disable_quant(dg.drhs)
     lhs_quant = not isinstance(
-        cfg.fwd.dg_quantizer.lhs.numerics, no_numerics.NoNumerics
+        dg.fwd.dg_quantizer.lhs.numerics, no_numerics.NoNumerics
     )
     rhs_quant = not isinstance(
-        cfg.fwd.dg_quantizer.rhs.numerics, no_numerics.NoNumerics
+        dg.fwd.dg_quantizer.rhs.numerics, no_numerics.NoNumerics
     )
     if lhs_quant:
-      cfg.drhs.rhs.use_fwd_quant = use_fwd_quant
+      dg.drhs.rhs.use_fwd_quant = use_fwd_quant
     if rhs_quant:
-      cfg.dlhs.rhs.use_fwd_quant = use_fwd_quant
+      dg.dlhs.rhs.use_fwd_quant = use_fwd_quant
   if local_aqt is not None:
     # Currently we are not supporting local_aqt in fwd pass
-    # cfg.fwd.local_aqt = local_aqt
-    cfg.dlhs.local_aqt = local_aqt
-    cfg.drhs.local_aqt = local_aqt
+    # dg.fwd.local_aqt = local_aqt
+    dg.dlhs.local_aqt = local_aqt
+    dg.drhs.local_aqt = local_aqt
 
     # When using abs-max scaling, this should be a no-op.
-  if isinstance(cfg.fwd.dg_quantizer.lhs.numerics, int_numerics.IntNumerics):
-    cfg.fwd.dg_quantizer.lhs.numerics = (
-        cfg.fwd.dg_quantizer.lhs.numerics.replace(clip_gradient=clip_gradient)
+  if isinstance(dg.fwd.dg_quantizer.lhs.numerics, int_numerics.IntNumerics):
+    dg.fwd.dg_quantizer.lhs.numerics = (
+        dg.fwd.dg_quantizer.lhs.numerics.replace(clip_gradient=clip_gradient)
     )
-  if isinstance(cfg.fwd.dg_quantizer.rhs.numerics, int_numerics.IntNumerics):
-    cfg.fwd.dg_quantizer.rhs.numerics = (
-        cfg.fwd.dg_quantizer.rhs.numerics.replace(clip_gradient=clip_gradient)
+  if isinstance(dg.fwd.dg_quantizer.rhs.numerics, int_numerics.IntNumerics):
+    dg.fwd.dg_quantizer.rhs.numerics = (
+        dg.fwd.dg_quantizer.rhs.numerics.replace(clip_gradient=clip_gradient)
     )
 
-  return cfg
+  return dg
 
 
 def _aqt_dg_full_lr_diff(
     lhs_dequant_mode: aqt.DequantMode,
     rhs_dequant_mode: aqt.DequantMode,
     lhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     rhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     use_fwd_quant: bool | None = None,
     fwd_lhs_tricky_clip_and_round: bool = False,
     local_aqt: aqt.LocalAqt | None = None,
     *,
-    readonly_cfg: aqt.DotGeneral,
+    readonly_dg: aqt.DotGeneral,
     dims: jax.lax.DotDimensionNumbers,
     clip_gradient: bool = False,
 ) -> Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray]:
-  cfg = _modify_cfg(
-      readonly_cfg,
+  dg = _modify_dg(
+      readonly_dg,
       lhs_dequant_mode=lhs_dequant_mode,
       rhs_dequant_mode=rhs_dequant_mode,
       lhs_calibration_mode=lhs_calibration_mode,
       rhs_calibration_mode=rhs_calibration_mode,
       use_fwd_quant=use_fwd_quant,
       fwd_lhs_tricky_clip_and_round=fwd_lhs_tricky_clip_and_round,
       local_aqt=local_aqt,
       clip_gradient=clip_gradient,
   )
-  cfg = config.set_context(cfg, key=jax.random.PRNGKey(4), train_step=None)
-  dg = aqt.make_dot_general(cfg)
+  dg = config.set_context(dg, key=jax.random.PRNGKey(4), train_step=None)
   return lambda lhs, rhs: dg(lhs, rhs, dims)
 
 
 def _aqt_dg_full(
     dequant_mode: aqt.DequantMode,
     calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     use_fwd_quant: bool | None = None,
     fwd_lhs_tricky_clip_and_round: bool = False,
     local_aqt: aqt.LocalAqt | None = None,
     *,
-    readonly_cfg: aqt.DotGeneral,
+    readonly_dg: aqt.DotGeneral,
     dims: jax.lax.DotDimensionNumbers,
     clip_gradient: bool = False,
 ) -> Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray]:
   return _aqt_dg_full_lr_diff(
       dequant_mode,
       dequant_mode,
       calibration_mode,
       calibration_mode,
       use_fwd_quant,
       fwd_lhs_tricky_clip_and_round,
       local_aqt,
-      readonly_cfg=readonly_cfg,
+      readonly_dg=readonly_dg,
       dims=dims,
       clip_gradient=clip_gradient
   )
 
 
 def _aqt_dg_raw_lr_diff(
     lhs_dequant_mode: aqt.DequantMode,
     rhs_dequant_mode: aqt.DequantMode,
     lhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     rhs_calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     *,
-    readonly_cfg: aqt.DotGeneral,
+    readonly_dg: aqt.DotGeneral,
     dims: jax.lax.DotDimensionNumbers,
 ) -> Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray]:
-  cfg = _modify_cfg(
-      readonly_cfg,
+  dg = _modify_dg(
+      readonly_dg,
       lhs_dequant_mode=lhs_dequant_mode,
       rhs_dequant_mode=rhs_dequant_mode,
       lhs_calibration_mode=lhs_calibration_mode,
       rhs_calibration_mode=rhs_calibration_mode,
   )
-  cfg = config.set_context(cfg, key=jax.random.PRNGKey(4), train_step=None)
-  return lambda lhs, rhs: cfg.fwd(lhs, rhs, None, None, dims)[0]
+  dg = config.set_context(dg, key=jax.random.PRNGKey(4), train_step=None)
+  return lambda lhs, rhs: dg.fwd(lhs, rhs, None, None, dims)[0]
 
 
 def _aqt_dg_raw(
     dequant_mode: aqt.DequantMode,
     calibration_mode: aqt.CalibrationMode = aqt.CalibrationMode.CONTRACTING_AXIS,
     *,
-    readonly_cfg: aqt.DotGeneral,
+    readonly_dg: aqt.DotGeneral,
     dims: jax.lax.DotDimensionNumbers,
 ) -> Callable[[jnp.ndarray, jnp.ndarray], jnp.ndarray]:
   return _aqt_dg_raw_lr_diff(
       dequant_mode,
       dequant_mode,
       calibration_mode,
       calibration_mode,
-      readonly_cfg=readonly_cfg,
+      readonly_dg=readonly_dg,
       dims=dims,
   )
 
 
 class AqtDotGeneralResearchTest(parameterized.TestCase):
 
   def test_empty(self):
@@ -449,72 +448,72 @@
 
     # TODO(lew): test
 
   @parameterized.parameters([
       dict(
           # TODO(aqt): Change dlhs_bits to 4bit once
           # https://github.com/google/jax/issues/19682 is fixed.
-          cfg=config.config_v3(
+          dg=config.config_v3(
               fwd_bits=3,
               dlhs_bits=6,
               drhs_bits=5,
               drhs_accumulator_dtype=jnp.int32,  # overwriting the default None
           )
       ),
-      dict(cfg=config.dot_general_make(None, None)),
-      dict(cfg=config.dot_general_make(1, 1)),
-      dict(cfg=config.dot_general_make(1, 2)),
-      dict(cfg=config.dot_general_make(2, 1)),
-      dict(cfg=config.dot_general_make(2, 2)),
-      dict(cfg=config.dot_general_make(8, 8)),
-      dict(cfg=config.dot_general_make(8, 8), clip_gradient=True),
-      dict(cfg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(cfg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(None, None)),
+      dict(dg=config.dot_general_make(1, 1)),
+      dict(dg=config.dot_general_make(1, 2)),
+      dict(dg=config.dot_general_make(2, 1)),
+      dict(dg=config.dot_general_make(2, 2)),
+      dict(dg=config.dot_general_make(8, 8)),
+      dict(dg=config.dot_general_make(8, 8), clip_gradient=True),
+      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
-      dict(cfg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
-      dict(cfg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
-      dict(cfg=config.dot_general_make(None, 8)),
-      dict(cfg=config.dot_general_make(8, None)),
+      dict(dg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
+      dict(dg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
+      dict(dg=config.dot_general_make(None, 8)),
+      dict(dg=config.dot_general_make(8, None)),
       dict(
-          cfg=fqt_param_dict(s=10, use_fwd_quant=True)["cfg"],
+          dg=fqt_param_dict(s=10, use_fwd_quant=True)["dg"],
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       dict(
-          cfg=fqt_param_dict(
+          dg=fqt_param_dict(
               s=10,
               use_fwd_quant=True,
               dlhs_local_aqt=aqt.LocalAqt(2),
-          )["cfg"],
+          )["dg"],
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       dict(
-          cfg=config.dot_general_make(2, 2),
+          dg=config.dot_general_make(2, 2),
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       *[fqt_param_dict(s, use_fwd_quant=False) for s in range(10)],
       *[fqt_param_dict(s, use_fwd_quant=True) for s in range(10)],
   ])
   def test_dot_general_calibration_with_contracting_axis(
       self,
-      cfg: aqt.DotGeneral,
+      dg: aqt.DotGeneral,
       lhs_maxval=10.0,
       rhs_maxval=20.0,
       gra_maxval=30.0,
       dims=(((1,), (0,)), ((), ())),  # classical matmul
       # lhs_shape=(1, 1),
       # rhs_shape=(1, 2),
       # gra_shape=(1, 2),  # has to be the shape of the output
@@ -524,49 +523,49 @@
       lhs_shape=(10, 20),
       rhs_shape=(20, 30),
       gra_shape=(10, 30),  # has to be the shape of the output
       seed=0,
       dtype=jnp.float32,
       clip_gradient=False,
   ):
-    readonly_cfg = cfg
-    del cfg
+    readonly_dg = dg
+    del dg
 
     lhs = rand_unif(lhs_shape, lhs_maxval, seed, dtype)
     rhs = rand_unif(rhs_shape, rhs_maxval, seed + 1, dtype)
     gra = rand_unif(gra_shape, gra_maxval, seed + 2, dtype)
 
     # Prepare utility functions for test.
     aqt_dg_full = functools.partial(
         _aqt_dg_full,
-        readonly_cfg=readonly_cfg,
+        readonly_dg=readonly_dg,
         dims=dims,
         clip_gradient=clip_gradient,
     )
     aqt_dg_raw = functools.partial(
-        _aqt_dg_raw, readonly_cfg=readonly_cfg, dims=dims
+        _aqt_dg_raw, readonly_dg=readonly_dg, dims=dims
     )
-    modify_cfg = functools.partial(_modify_cfg, readonly_cfg=readonly_cfg)
+    modify_dg = functools.partial(_modify_dg, readonly_dg=readonly_dg)
     check = functools.partial(_check_result_eq, lhs=lhs, rhs=rhs, gra=gra)
 
     # Tests for dot_general.
     test_jaxpr_dtype(
         lambda: aqt_dg_full(aqt.DequantMode.OUTPUT)(lhs, rhs),
-        [modify_cfg().fwd],
+        [modify_dg().fwd],
         lhs.dtype,
     )
     test_jaxpr_dtype(
         lambda: jax.vjp(aqt_dg_full(aqt.DequantMode.OUTPUT), lhs, rhs),
-        [modify_cfg().fwd],
+        [modify_dg().fwd],
         lhs.dtype,
     )
     _, backprop = jax.vjp(aqt_dg_full(aqt.DequantMode.OUTPUT), lhs, rhs)
     test_jaxpr_dtype(
         lambda: backprop(gra),
-        [modify_cfg().dlhs, modify_cfg().drhs],
+        [modify_dg().dlhs, modify_dg().drhs],
         gra.dtype,
     )
 
     check([
         ("default    ", aqt_dg_full(aqt.DequantMode.OUTPUT), dict()),
         ("FQ         ", aqt_dg_full(aqt.DequantMode.THIS_INPUT), dict()),
         (
@@ -604,122 +603,122 @@
             "default    ",
             aqt_dg_full(aqt.DequantMode.THIS_INPUT, local_aqt=aqt.LocalAqt(2)),
             dict(),
         ),
     ])
 
     if isinstance(
-        readonly_cfg.fwd.dg_quantizer.lhs.numerics,
+        readonly_dg.fwd.dg_quantizer.lhs.numerics,
         int_numerics.IntNumerics,
     ):
       check([
           (
               "check_fwd_lhs_tricky_clip_and_round",
               aqt_dg_full(
                   aqt.DequantMode.OUTPUT, fwd_lhs_tricky_clip_and_round=True
               ),
               dict(check_fwd_lhs_tricky_clip_and_round=True),
           ),
       ])
 
     def unquant_aqt_dg(lhs, rhs):
-      dg = aqt.make_dot_general(config.default_unquantized_config())
+      dg = config.default_unquantized_config()
       return dg(lhs, rhs, dims)
 
     def lax_dg(lhs, rhs):
       return jax.lax.dot_general(lhs, rhs, dims)
 
     check([
         ("unquantized default:", unquant_aqt_dg, dict()),
         ("lax.dot_general:", lax_dg, dict()),
     ])
 
   @parameterized.parameters([
       dict(
-          cfg=lambda: config.config_v3(
+          dg=lambda: config.config_v3(
               fwd_bits=3,
               dlhs_bits=4,
               drhs_bits=5,
               drhs_accumulator_dtype=jnp.int32,  # overwriting the default None
           )
       ),
-      dict(cfg=config.dot_general_make(None, None)),
-      dict(cfg=config.dot_general_make(1, 1)),
-      dict(cfg=config.dot_general_make(1, 2)),
-      dict(cfg=config.dot_general_make(2, 1)),
-      dict(cfg=config.dot_general_make(2, 2)),
-      dict(cfg=config.dot_general_make(8, 8)),
-      dict(cfg=config.dot_general_make(8, 8), clip_gradient=True),
-      dict(cfg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(cfg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(None, None)),
+      dict(dg=config.dot_general_make(1, 1)),
+      dict(dg=config.dot_general_make(1, 2)),
+      dict(dg=config.dot_general_make(2, 1)),
+      dict(dg=config.dot_general_make(2, 2)),
+      dict(dg=config.dot_general_make(8, 8)),
+      dict(dg=config.dot_general_make(8, 8), clip_gradient=True),
+      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
       # That test could fail numerically because bf16
       # can't keep in the product of int8*int8 accurately.
       # It just so happens that this test does not fail but others do.
       # We do this test anyway, to catch jax-compilation-time errors.
-      dict(cfg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
-      dict(cfg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
-      dict(cfg=config.dot_general_make(None, 8)),
-      dict(cfg=config.dot_general_make(8, None)),
+      dict(dg=config.dot_general_make(2, 2), dtype=jnp.bfloat16),
+      dict(dg=config.dot_general_make(8, 8), dtype=jnp.bfloat16),
+      dict(dg=config.dot_general_make(None, 8)),
+      dict(dg=config.dot_general_make(8, None)),
       dict(
-          cfg=config.dot_general_make(2, 2),
+          dg=config.dot_general_make(2, 2),
           dims=(((0, 2), (1, 0)), ((3, 1), (2, 4))),
           # contraction: 2, 5; batch: 4, 3
           lhs_shape=(2, 3, 5, 4),  # non-contr: 3, 4
           rhs_shape=(5, 2, 4, 6, 3),  # non-contr: 4, 6, 3
           gra_shape=(4, 3, 6),
       ),
       *[fqt_param_dict(s, use_fwd_quant=None) for s in range(10)],
   ])
   def test_dot_general_calibration_with_remaining_axis(
       self,
-      cfg: config.DotGeneral | Callable[[], config.DotGeneral],
+      dg: config.DotGeneral | Callable[[], config.DotGeneral],
       lhs_maxval=10.0,
       rhs_maxval=20.0,
       gra_maxval=30.0,
       dims=(((1,), (0,)), ((), ())),  # classical matmul
       lhs_shape=(10, 20),
       rhs_shape=(20, 30),
       gra_shape=(10, 30),  # has to be the shape of the output
       seed=0,
       dtype=jnp.float32,
       clip_gradient=False,
   ):
     # Deferred evaluation of config function calls. 4-bit config initialization
     # triggers jax.local_devices(), which shouldn't be called before
     # absl.app.run() in some environments.
-    if not isinstance(cfg, config.DotGeneral):
-      cfg = cfg()
+    if not isinstance(dg, config.DotGeneral):
+      dg = dg()
     # Set use_fwd_quant to None.
-    cfg.drhs.rhs.use_fwd_quant = None
-    cfg.dlhs.rhs.use_fwd_quant = None
-    readonly_cfg = cfg
-    del cfg
+    dg.drhs.rhs.use_fwd_quant = None
+    dg.dlhs.rhs.use_fwd_quant = None
+    readonly_dg = dg
+    del dg
 
     lhs = rand_unif(lhs_shape, lhs_maxval, seed, dtype)
     rhs = rand_unif(rhs_shape, rhs_maxval, seed + 1, dtype)
     gra = rand_unif(gra_shape, gra_maxval, seed + 2, dtype)
 
     # Prepare utility functions for test.
     aqt_dg_full = functools.partial(
         _aqt_dg_full,
-        readonly_cfg=readonly_cfg,
+        readonly_dg=readonly_dg,
         dims=dims,
         clip_gradient=clip_gradient,
     )
     aqt_dg_full_lr_diff = functools.partial(
         _aqt_dg_full_lr_diff,
-        readonly_cfg=readonly_cfg,
+        readonly_dg=readonly_dg,
         dims=dims,
         clip_gradient=clip_gradient,
     )
     aqt_dg_raw = functools.partial(
-        _aqt_dg_raw, readonly_cfg=readonly_cfg, dims=dims
+        _aqt_dg_raw, readonly_dg=readonly_dg, dims=dims
     )
     aqt_dg_raw_lr_diff = functools.partial(
-        _aqt_dg_raw_lr_diff, readonly_cfg=readonly_cfg, dims=dims
+        _aqt_dg_raw_lr_diff, readonly_dg=readonly_dg, dims=dims
     )
     check = functools.partial(_check_result_eq, lhs=lhs, rhs=rhs, gra=gra)
 
     # test dot_general
     check([
         (
             "RA L       ",
@@ -810,103 +809,103 @@
                 local_aqt=aqt.LocalAqt(2),
             ),
             dict(),
         ),
     ])
 
   def test_dot_general_calibrate_dequant_mode_mismatch(self):
-    cfg = config.dot_general_make(8, 8, use_fwd_quant=None)
+    dg = config.dot_general_make(8, 8, use_fwd_quant=None)
     dims = (((1,), (0,)), ((), ()))
     lhs = rand_unif((10, 20), 10.0, 0, jnp.float32)
     rhs = rand_unif((20, 30), 20.0, 1, jnp.float32)
 
     # 1. Raise error when OTHER_INPUT + CONTRACTING_AXIS
     with self.assertRaisesRegex(
         AssertionError,
         ".*Unsupported calibration mode.*dequant mode combination.*",
     ):
       _aqt_dg_full_lr_diff(
           aqt.DequantMode.THIS_INPUT,
           aqt.DequantMode.OTHER_INPUT,
           aqt.CalibrationMode.CONTRACTING_AXIS,
           aqt.CalibrationMode.CONTRACTING_AXIS,
-          readonly_cfg=copy.deepcopy(cfg),
+          readonly_dg=copy.deepcopy(dg),
           dims=dims,
       )(lhs, rhs)
 
     # 2. Raise error when OUTPUT + REMAINING_AXIS
     with self.assertRaisesRegex(
         AssertionError,
         ".*Unsupported calibration mode.*dequant mode combination.*",
     ):
       _aqt_dg_full_lr_diff(
           aqt.DequantMode.THIS_INPUT,
           aqt.DequantMode.OUTPUT,
           aqt.CalibrationMode.CONTRACTING_AXIS,
           aqt.CalibrationMode.REMAINING_AXIS,
-          readonly_cfg=copy.deepcopy(cfg),
+          readonly_dg=copy.deepcopy(dg),
           dims=dims,
       )(lhs, rhs)
 
   @parameterized.parameters([False, True])
   def test_dot_general_prevent_fwd_quant_with_remaining_axis(
       self, use_fwd_quant
   ):
     """If calibration axis is remaining_axis, use_fwd_quant should be None."""
-    cfg = config.dot_general_make(8, 8, use_fwd_quant=use_fwd_quant)
+    dg = config.dot_general_make(8, 8, use_fwd_quant=use_fwd_quant)
     dims = (((1,), (0,)), ((), ()))
     lhs = rand_unif((10, 20), 10.0, 0, jnp.float32)
     rhs = rand_unif((20, 30), 20.0, 1, jnp.float32)
 
     with self.assertRaisesRegex(
         AssertionError,
         ".*use_fwd_quant should be set to None.*",
     ):
       _aqt_dg_full_lr_diff(
           aqt.DequantMode.THIS_INPUT,
           aqt.DequantMode.OTHER_INPUT,
           aqt.CalibrationMode.CONTRACTING_AXIS,
           aqt.CalibrationMode.REMAINING_AXIS,
-          readonly_cfg=copy.deepcopy(cfg),
+          readonly_dg=copy.deepcopy(dg),
           dims=dims,
       )(lhs, rhs)
 
   @parameterized.parameters([
-      dict(cfg=config.dot_general_make(8, 8)),
-      dict(cfg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
-      dict(cfg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(8, 8)),
+      dict(dg=config.dot_general_make(8, 8, dlhs_local_aqt=aqt.LocalAqt(2))),
+      dict(dg=config.dot_general_make(8, 8, drhs_local_aqt=aqt.LocalAqt(2))),
   ])
   def test_dot_general_equality_between_different_calibration_axes(
       self,
-      cfg: config.DotGeneral,
+      dg: config.DotGeneral,
   ):
     """Check equality between different calibration axes."""
     dims = (((1,), (0,)), ((), ()))
 
     # Set use_fwd_quant to None.
-    cfg.drhs.rhs.use_fwd_quant = None
-    cfg.dlhs.rhs.use_fwd_quant = None
-    readonly_cfg = cfg
-    del cfg
+    dg.drhs.rhs.use_fwd_quant = None
+    dg.dlhs.rhs.use_fwd_quant = None
+    readonly_dg = dg
+    del dg
 
     # Set the two arguments as powers of 2, to prevent it from having the
     # quantization loss.
     lhs = 2 ** jnp.floor(rand_unif((10, 20), 3.0, 1, jnp.float32) + 3.0)
     rhs = 2 ** jnp.floor(rand_unif((20, 30), 3.0, 2, jnp.float32) + 3.0)
     gra = 2 ** jnp.floor(rand_unif((10, 30), 3.0, 3, jnp.float32) + 3.0)
 
     # Prepare utility functions for test.
     aqt_dg_full = functools.partial(
         _aqt_dg_full,
-        readonly_cfg=readonly_cfg,
+        readonly_dg=readonly_dg,
         dims=dims
     )
     aqt_dg_full_lr_diff = functools.partial(
         _aqt_dg_full_lr_diff,
-        readonly_cfg=readonly_cfg,
+        readonly_dg=readonly_dg,
         dims=dims
     )
     check = functools.partial(_check_result_eq, lhs=lhs, rhs=rhs, gra=gra)
 
     # test dot_general
     check([
         (
@@ -948,40 +947,39 @@
             dict(),
         ),
     ])
 
   def test_dynamic_context(self):
     @jax.jit
     def f(lhs, rhs):
-      cfg = config.dot_general_make()
-      cfg = config.set_context(cfg, key=jax.random.PRNGKey(4), train_step=None)
-      dg = aqt.make_dot_general(cfg)
+      dg = config.dot_general_make()
+      dg = config.set_context(dg, key=jax.random.PRNGKey(4), train_step=None)
       return dg(lhs, rhs, (((0,), (0,)), ((), ())))
 
     lhs, rhs = jnp.array([3.0, 4.0]), jnp.array([4.0, 5.0])
     jax.value_and_grad(f)(lhs, rhs)
 
   def test_hardware_int8(self, seed=0):
-    cfg = config.dot_general_raw_make(8, 8)
+    dg_raw = config.dot_general_raw_make(8, 8)
 
     def dg(lhs, rhs):
-      ret, _ = cfg(
+      ret, _ = dg_raw(
           lhs,
           rhs,
           None,
           None,
           (((1,), (0,)), ((), ())),
       )
       return ret
 
     lhs = rand_unif((10, 20), 1.0, seed)
     rhs = rand_unif((20, 30), 1.0, seed + 1)
-    test_jaxpr_dtype(lambda: dg(lhs, rhs), [cfg], lhs.dtype)
-    assert cfg.dg_quantizer.lhs.numerics.get_dtype() == jnp.int8
-    assert cfg.dg_quantizer.rhs.numerics.get_dtype() == jnp.int8
+    test_jaxpr_dtype(lambda: dg(lhs, rhs), [dg_raw], lhs.dtype)
+    assert dg_raw.dg_quantizer.lhs.numerics.get_dtype() == jnp.int8
+    assert dg_raw.dg_quantizer.rhs.numerics.get_dtype() == jnp.int8
 
   @parameterized.parameters([
       (1, 1),
       (1, 2),
       (2, 1),
       (2, 2),
       (8, 8),
@@ -993,37 +991,37 @@
       self,
       lhs_bits,
       rhs_bits,
       lhs_maxval=10.0,
       rhs_maxval=20.0,
       seed=0,
   ):
-    cfg = config.conv_general_dilated_make(2, lhs_bits, rhs_bits)
+    dg_raw_conv = config.conv_general_dilated_make(2, lhs_bits, rhs_bits)
 
-    if cfg.lhs:
+    if dg_raw_conv.lhs:
       # Power-of-2 scales allow FQ and AQT to be exactly the same.
-      cfg.dg_quantizer.lhs.po2_scale = True
-    if cfg.rhs:
-      cfg.dg_quantizer.rhs.po2_scale = True
+      dg_raw_conv.dg_quantizer.lhs.po2_scale = True
+    if dg_raw_conv.rhs:
+      dg_raw_conv.dg_quantizer.rhs.po2_scale = True
 
     batch_n = 10
     contr_n = 20
     feature_n = 30
     lhs = rand_unif((batch_n, 4, 5, contr_n), lhs_maxval, seed)
     rhs = rand_unif((3, 3, contr_n, feature_n), rhs_maxval, seed + 1)
 
     lax_conv = jax.lax.conv_general_dilated
-    aqt_conv_fn = aqt_conv.make_conv_general_dilated(cfg)
+    aqt_conv_fn = aqt_conv.make_conv_general_dilated(dg_raw_conv)
     kwargs = {
         "window_strides": (1, 1),
         "padding": "SAME",
         "dimension_numbers": fl._conv_dimension_numbers(lhs.shape),
     }
-    lhs_fq = aqt_quantizer.make_fake_quant(cfg.dg_quantizer.lhs)(lhs)
-    rhs_fq = aqt_quantizer.make_fake_quant(cfg.dg_quantizer.rhs)(rhs)
+    lhs_fq = aqt_quantizer.make_fake_quant(dg_raw_conv.dg_quantizer.lhs)(lhs)
+    rhs_fq = aqt_quantizer.make_fake_quant(dg_raw_conv.dg_quantizer.rhs)(rhs)
     prod_fq = lax_conv(lhs_fq, rhs_fq, **kwargs)
     prod_aqt = aqt_conv_fn(lhs, rhs, **kwargs)
     assert (prod_aqt == prod_fq).all()
 
   @parameterized.parameters([
       dict(
           shard_count=2,
@@ -1035,40 +1033,40 @@
           lhs=[1270.0, 10.0, 1270000.0, 10000.0],
           expected_product=1280000.0,
       ),
   ])
   def test_local_aqt(self, shard_count, lhs, expected_product):
     # create a config that quantizes both forward and backward passes to int8
     # set the number of shards (local aqt) to 2
-    cfg = config.fully_quantized(
+    dg = config.fully_quantized(
         fwd_bits=8,
         bwd_bits=8,
         use_stochastic_rounding=False,
         drhs_local_aqt=aqt.LocalAqt(shard_count),
     )
-    cfg.fwd.dg_quantizer.lhs.numerics = (
-        cfg.fwd.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
+    dg.fwd.dg_quantizer.lhs.numerics = (
+        dg.fwd.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.fwd.dg_quantizer.rhs.numerics = (
-        cfg.fwd.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
+    dg.fwd.dg_quantizer.rhs.numerics = (
+        dg.fwd.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.drhs.dg_quantizer.lhs.numerics = (
-        cfg.drhs.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
+    dg.drhs.dg_quantizer.lhs.numerics = (
+        dg.drhs.dg_quantizer.lhs.numerics.replace(preserve_max_val=True)
     )
-    cfg.drhs.dg_quantizer.rhs.numerics = (
-        cfg.drhs.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
+    dg.drhs.dg_quantizer.rhs.numerics = (
+        dg.drhs.dg_quantizer.rhs.numerics.replace(preserve_max_val=True)
     )
-    dg = lambda lhs, rhs: aqt.make_dot_general(cfg)(
+    dg_f = lambda lhs, rhs: dg(
         lhs,
         rhs,
         dimension_numbers=(((), ()), ((), ())),
     )
     lhs = jnp.array(lhs)
     rhs = jnp.array([1.0])
-    output, bprop = jax.vjp(dg, lhs, rhs)
+    output, bprop = jax.vjp(dg_f, lhs, rhs)
     _, drhs = bprop(jnp.ones_like(output))
     assert drhs == expected_product
 
   def test_per_tensor(self):
     # TODO(lew): bits=8 started failing in VLP colab due x/x != 1.0 sometimes
     bits = 4
     my_numerics = int_numerics.IntNumerics(
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_quantizer.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,31 +49,26 @@
   def quant(
       self,
       x,
       *,
       calibration_axes,
   ) -> tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn]:
     """The core quantizing function."""
+    qt = self.calibrate(x, calibration_axes=calibration_axes)
+    qt, quant_grad = self.calculate_qvalue(x, qt)
+    return qt, quant_grad
+
+  def calibrate(self, x, *, calibration_axes) -> aqt_tensor.QTensor:
+    """Create incomplete QTensor with only quantization parameters."""
     if isinstance(self.numerics, no_numerics.NoNumerics):
       qt = aqt_tensor.QTensor(
           qvalue=x, scale=[], scale_t=[], dequant_dtype=x.dtype
       )
-      return qt, None
-
-    qt = self.calculate_scale(x, calibration_axes=calibration_axes)
-    qt, quant_grad = self.calculate_qvalue(x, qt)
-    return qt, quant_grad
+      return qt
 
-  def calculate_scale(
-      self,
-      x,
-      *,
-      calibration_axes,
-  ) -> aqt_tensor.QTensor:
-    """Create incomplete QTensor with only quantization parameters."""
     dequant_dtype = x.dtype
     # TODO(lew): We should cast earlier. xhs_q should be in cfg.xhs.dtype
     # TODO(lew): After we implement optimization to not double-quantize,
     #   what would happen if we pass fq value (xhs_q2) in residual?
     if self.calib_shared_axes == "per_tensor":
       shared_axes = list(range(x.ndim))
     else:
@@ -104,14 +99,19 @@
 
   def calculate_qvalue(
       self,
       x,
       qt: aqt_tensor.QTensor
   ) -> tuple[aqt_tensor.QTensor, aqt_tensor.GradientFn]:
     """Uses the quantization parameters in qt to quantize x."""
+    if isinstance(self.numerics, no_numerics.NoNumerics):
+      return qt, None
+
+    # TODO: b/333984742 - make numeric as a member of QTensor, and put
+    # numerics-related logics into the QTensor.
     qt = qt.quant(x)
 
     # TODO(lew): A logical thing would be if this call was part of
     # QTensor.quant.
     x_q, res = self.numerics.vjp_fwd(qt.qvalue, self.context)
     quant_grad = jax.tree_util.Partial(self.numerics.vjp_bwd, res)
 
@@ -123,15 +123,15 @@
     n_bits: int | None, preserve_max_val: bool = False
 ) -> Quantizer:
   """Makes Quantizer."""
   if n_bits is None:
     effective_numerics = no_numerics.NoNumerics()
   else:
     pz = False if n_bits == 1 else True
-    dtype = utils.infer_dtype_from_bits(n_bits, upcast=False) if pz else None
+    dtype = utils.infer_dtype_from_bits(n_bits) if pz else None
     effective_numerics = int_numerics.IntNumerics(
         bits=n_bits,
         preserve_zero=pz,
         preserve_max_val=preserve_max_val,
         clip=True,
         round=True,
         noise_fn=None,
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_tensor.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_tensor.py`

 * *Files 9% similar despite different names*

```diff
@@ -70,16 +70,23 @@
   scale_t: Optional[list[ArrayT]]
 
   # DType of the tensor before quantized.
   dequant_dtype: Optional[jnp.dtype] = flax.struct.field(
       pytree_node=False, default=None
   )
 
+  def is_full(self) -> bool:
+    return self.qvalue is not None
+
+  def without_qvalue(self) -> Self:
+    """Returns a copy of the QTensor without the qvalue."""
+    return self.replace(qvalue=None)  # pytype: disable=attribute-error
+
   def quant(self, x):
-    assert self.qvalue is None, 'Already quantized QTensor.'
+    assert not self.is_full(), 'Already quantized QTensor.'
     assert self.scale is not None, 'Missing scales to be used for quantization.'
 
     qvalue = x
     for s in self.scale:
       qvalue = qvalue * jax.lax.reciprocal(s)
 
     # TODO(lew): We should apply numerics here, so that 'quant' function
@@ -90,47 +97,51 @@
     """Dequantizes the QTensor."""
     assert self.scale is not None, 'Missing scales when dequantizing a QTensor.'
     msg = (
         'QTensor is manually created without setting a dequant_detype. It can'
         ' be used in dot_general, but to dequantize you need to set its dtype.'
     )
     assert self.dequant_dtype is not None, msg
-    assert self.qvalue is not None, _MSG_NO_QVALUE
+    assert self.is_full(), _MSG_NO_QVALUE
     ret = self.qvalue
     for scale in self.scale:
       ret = ret.astype(self.dequant_dtype) * scale.astype(self.dequant_dtype)  # pytype: disable=attribute-error
     return ret  # pytype: disable=bad-return-type
 
   def qvalue_astype(self, dtype) -> Self:
-    assert self.qvalue is not None, _MSG_NO_QVALUE
+    assert self.is_full(), _MSG_NO_QVALUE
     return self.replace(qvalue=self.qvalue.astype(dtype))  # pytype: disable=attribute-error
 
   def __getitem__(self, idx: jax_typing.ArrayLike) -> Self:
     """Returns the indexed subtensor on the first axis."""
     assert self.scale_t is None, 'scale_t is not supported in __getitem__'
-    assert self.qvalue is not None, _MSG_NO_QVALUE
+    assert self.is_full(), _MSG_NO_QVALUE
     qvalue = self.qvalue[idx]
     scale = [s[idx] for s in self.scale]
     return QTensor(
         qvalue=qvalue,
         scale=scale,
         scale_t=self.scale_t,
         dequant_dtype=self.dequant_dtype,
     )
 
   @property
   def ndim(self) -> int:
-    assert self.qvalue is not None, _MSG_NO_QVALUE
+    assert self.is_full(), _MSG_NO_QVALUE
     return self.qvalue.ndim  # pytype: disable=attribute-error
 
   @property
   def shape(self) -> Sequence[int]:
-    assert self.qvalue is not None, _MSG_NO_QVALUE
+    assert self.is_full(), _MSG_NO_QVALUE
     return self.qvalue.shape  # pytype: disable=attribute-error
 
+  def __len__(self) -> int:
+    assert self.qvalue is not None, _MSG_NO_QVALUE
+    return len(self.qvalue)
+
 
 def zeros(
     shape: Sequence[int], qdtype: jnp.dtype, dequant_dtype: jnp.dtype
 ) -> QTensor:
   return QTensor(
       qvalue=jnp.zeros(shape, dtype=qdtype),
       scale=[],
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/aqt_tensor_test.py` & `aqtp-0.7.2/aqt/jax/v2/aqt_tensor_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/calibration.py` & `aqtp-0.7.2/aqt/jax/v2/calibration.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/config.py` & `aqtp-0.7.2/aqt/jax/v2/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -530,14 +530,16 @@
     dlhs_local_aqt: Optional[LocalAqt] = None,
     drhs_local_aqt: Optional[LocalAqt] = None,
     # accumulator dtype by default is automatically set in set_bits,
     # but users can still configure a special dtype such as jnp.int16, etc.
     fwd_accumulator_dtype: Union[jnp.dtype, None, SkipT] = SKIP,
     dlhs_accumulator_dtype: Union[jnp.dtype, None, SkipT] = SKIP,
     drhs_accumulator_dtype: Union[jnp.dtype, None, SkipT] = SKIP,
+    dlhs_use_fwd_quant: Union[bool, None, SkipT] = SKIP,
+    drhs_use_fwd_quant: Union[bool, None, SkipT] = SKIP,
 ) -> DotGeneral:
   """Version 4 of user-visible AQT config."""
   cfg = default_unquantized_config()
   set_bits(
       cfg,
       fwd_lhs_bit=fwd_bits,
       fwd_rhs_bit=fwd_bits,
@@ -562,17 +564,19 @@
     set_static_bound(cfg, 1.0)
   set_local_aqt(
       cfg,
       fwd_local_aqt=SKIP,
       dlhs_local_aqt=dlhs_local_aqt,
       drhs_local_aqt=drhs_local_aqt,
   )
-  # TODO(yichizh): remove set_use_fwd_quant here since it will be automatically
-  # set in set_bits. Or make them as an argument.
-  set_use_fwd_quant(cfg, dlhs_use_fwd_quant=False, drhs_use_fwd_quant=False)
+  set_use_fwd_quant(
+      cfg,
+      dlhs_use_fwd_quant=dlhs_use_fwd_quant,
+      drhs_use_fwd_quant=drhs_use_fwd_quant,
+  )
   assert cfg.fwd.local_aqt is None, 'local_aqt is not yet supported in fwd.'
   return cfg
 
 
 def config_fwd_fp8(fwd_bits: fp8_numerics.FP8Dtype = 'e4m3') -> DotGeneral:
   """Configs for FP8 forward pass."""
   assert (
@@ -587,7 +591,20 @@
       dlhs_rhs_bit=None,
       drhs_lhs_bit=None,
       drhs_rhs_bit=None,
   )
   set_stochastic_rounding(cfg, False, False, 'jax.uniform')
   assert cfg.fwd.local_aqt is None, 'local_aqt is not yet supported in fwd.'
   return cfg
+
+
+def set_fwd_calibration(
+    cfg: DotGeneral,
+    calibration_factory
+) -> DotGeneral:
+  """Updates aqt_cfg for static range calibration."""
+  assert isinstance(
+      cfg.fwd.dg_quantizer, aqt_dot_general.DefaultDotGeneralQuantizer
+  )
+
+  cfg.fwd.dg_quantizer.lhs.calibration = calibration_factory
+  cfg.fwd.dg_quantizer.rhs.calibration = calibration_factory
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/config_test.py` & `aqtp-0.7.2/aqt/jax/v2/config_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/examples/examples.ipynb` & `aqtp-0.7.2/aqt/jax/v2/examples/examples.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/examples/flax_e2e_model.py` & `aqtp-0.7.2/aqt/jax/v2/examples/flax_e2e_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import sys
 from typing import Any, Callable
 from absl import app
 from aqt.jax.v2 import config as aqt_config
 from aqt.jax.v2 import tiled_dot_general
 from aqt.jax.v2 import utils
 from aqt.jax.v2.flax import aqt_flax
+from aqt.jax.v2.flax import aqt_flax_calibration
 from flax import linen as nn
 from flax import struct
 from flax.metrics import tensorboard
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
@@ -61,15 +62,16 @@
     )
     aqt_dg = functools.partial(
         aqt_flax.AqtDotGeneral,
         self.aqt_cfg,
         lhs_quant_mode=self.activation_quant_mode,
         rhs_quant_mode=self.weights_quant_mode,
         tiling_cfg=tiling_cfg,
-        use_legacy_freezer=False
+        use_legacy_freezer=False,
+        lhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION
     )
     use_running_avg = not self.bn_use_stats
     x = nn.Conv(features=32, kernel_size=(3, 3))(x)
     x = nn.BatchNorm(use_running_average=use_running_avg, dtype=x.dtype)(x)
     x = nn.relu(x)
     x = nn.avg_pool(x, window_shape=(2, 2), strides=(2, 2))
     x = nn.Conv(features=64, kernel_size=(3, 3))(x)
@@ -95,15 +97,17 @@
         # These assertions are useful when AqtEinsum definition is far away
         # from usage spot (through injection).
         # This is especially useful when specifying tiling.
         assert_eqn='bc,ab->ac',
         assert_lhs_shape=(10, 10),
         assert_rhs_shape=(None, 10),
         tile_sizes={'b': 5},
-        use_legacy_freezer=False
+        use_legacy_freezer=False,
+        lhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION_AND_VALUE,
+        rhs_freeze_mode=aqt_flax.FreezerMode.CALIBRATION,
     )
     # Note for AQT developers:
     #   This equation is harder because jnp.einsum and einsum swap lhs and rhs.
     x = einsum('bc,ab->ac', identity, x)
     return x
 
 
@@ -211,24 +215,29 @@
       model=model,
       tx=tx,
       opt_state=tx.init(model['params']),
   )
 
 
 def train_and_evaluate(
-    num_epochs: int, workdir: str, aqt_cfg: aqt_config.DotGeneral
+    num_epochs: int,
+    workdir: str,
+    aqt_cfg: aqt_config.DotGeneral | None = None,
+    state: TrainState | None = None,
 ) -> TrainState:
   """Execute model training and evaluation loop."""
   train_ds, test_ds = get_datasets()
   rng = jax.random.key(0)
 
   summary_writer = tensorboard.SummaryWriter(workdir)
 
   rng, init_rng = jax.random.split(rng)
-  state = create_train_state(init_rng, aqt_cfg)
+  if state is None:
+    assert aqt_cfg is not None
+    state = create_train_state(init_rng, aqt_cfg)
 
   batch_size = 128
   for epoch in range(1, num_epochs + 1):
     rng, input_rng = jax.random.split(rng)
     state, train_loss, train_accuracy = train_epoch(
         state, train_ds, batch_size, input_rng
     )
@@ -256,42 +265,50 @@
 
   summary_writer.flush()
   return state
 
 
 def serving_conversion(
     train_state: TrainState,
+    weight_only: bool = True
 ) -> tuple[Callable[..., Any], dict[str, Any]]:
   """Model conversion (quantized weights freezing).
 
   Convert the model parameter for serving. During conversion, quantized weights
   are created as variables, along with their scales.
 
   Args:
     train_state: TrainState containing model definitions and params.
+    weight_only: If set, does not quantize activations.
+
   Returns:
     A tuple of serving function, and converted model parameters.
   """
   aqt_cfg = train_state.cnn_eval.aqt_cfg
   input_shape = (1, 28, 28, 1)
+  activation_quant_mode = (
+      utils.QuantMode.TRAIN if weight_only else utils.QuantMode.CONVERT
+  )
   cnn_freeze = CNN(
       bn_use_stats=False,
       aqt_cfg=aqt_cfg,
       weights_quant_mode=utils.QuantMode.CONVERT,
+      activation_quant_mode=activation_quant_mode,
   )
   _, model_serving = cnn_freeze.apply(
       train_state.model,
       jnp.ones(input_shape),
       rngs={'params': jax.random.PRNGKey(0)},
       mutable=True,
   )
   cnn_serve = CNN(
       bn_use_stats=False,
       aqt_cfg=aqt_cfg,
       weights_quant_mode=utils.QuantMode.SERVE,
+      activation_quant_mode=activation_quant_mode,
   )
 
   return cnn_serve.apply, model_serving
 
 
 def _merge_pytrees(from_model, to_model):
   """Copies the parameters from from_model to to_model."""
@@ -310,14 +327,29 @@
   merged_model = jax.tree_util.tree_unflatten(
       to_model_treedef, [v for _, v in merged_flattened]
   )
 
   return merged_model
 
 
+def update_cfg_with_calibration(aqt_cfg):
+  """Updates aqt_cfg for static range calibration."""
+  sr_calibration_cls = functools.partial(
+      aqt_flax_calibration.MeanOfAbsMaxCalibration,
+      quant_collection='qc',
+  )
+
+  aqt_config.set_fwd_calibration(aqt_cfg, sr_calibration_cls)
+
+  # For static range calibration, the calibration axis for activation should
+  # be set to per_tensor, since its dimensions could be different during
+  # training and during inference.
+  aqt_cfg.fwd.dg_quantizer.lhs.calib_shared_axes = 'per_tensor'
+
+
 def calibration_conversion(
     train_state: TrainState,
 ) -> tuple[Callable[..., Any], dict[str, Any]]:
   """Model conversion (initializing calibration parameters).
 
   Newly initialize variables to store the quantization statistics collected
   during calibration process.
@@ -342,41 +374,65 @@
       jax.random.PRNGKey(0), jnp.ones([1, 28, 28, 1])
   )
   model_calibrated = _merge_pytrees(train_state.model, model_calibrated_init)
 
   return cnn_calibrate.apply, model_calibrated
 
 
-def calibrate(state, train_ds, batch_size, rng, calibration_steps):
-  """Calibrate."""
-  calibrate_func, model_calibrate = calibration_conversion(state)
-
+def calibrate_epoch(
+    calibrate_func,
+    model_calibrated,
+    train_ds,
+    batch_size,
+    rng,
+    calibration_steps,
+):
+  """Calibrates for a single epoch."""
   perms = _prepare_data_perm(train_ds, batch_size, rng, calibration_steps)
 
   for perm in perms:
     batch_images = train_ds['image'][perm, ...]
     batch_labels = train_ds['label'][perm, ...]
 
     # Calibration simply updates model during inference; it does NOT apply any
     # gradients.
-    _, _, _, model_calibrate = apply_model(
-        model_calibrate, batch_images, batch_labels, calibrate_func
+    _, _, _, model_calibrated = apply_model(
+        model_calibrated, batch_images, batch_labels, calibrate_func
     )
 
-  return model_calibrate
+  return model_calibrated
 
 
-@jax.jit
-def serve(state):
+def calibrate(state: TrainState, calibration_steps: int) -> TrainState:
+  """Calibrate."""
+  train_ds, _ = get_datasets()
+  rng = jax.random.key(0)
+  batch_size = 128
+  calibration_func, model_calibrated = calibration_conversion(state)
+
+  model_calibrated = calibrate_epoch(
+      calibration_func,
+      model_calibrated,
+      train_ds,
+      batch_size,
+      rng,
+      calibration_steps,
+  )
+
+  return state.replace(model=model_calibrated)
+
+
+@functools.partial(jax.jit, static_argnums=(1,))
+def serve(state: TrainState, weight_only: bool = True):
   """Take train state, freeze integer weights, and serve."""
   # get sample serving data
   _, test_ds = get_datasets()
   sample_image, sample_label = test_ds['image'][:64], test_ds['label'][:64]
   # serving
-  serve_fn, model_serving = serving_conversion(state)
+  serve_fn, model_serving = serving_conversion(state, weight_only=weight_only)
   logits = serve_fn(
       model_serving, sample_image, rngs={'params': jax.random.PRNGKey(0)}
   )
   # compute serving loss
   one_hot = jax.nn.one_hot(sample_label, 10)
   loss = jnp.mean(optax.softmax_cross_entropy(logits=logits, labels=one_hot))
   return loss
@@ -397,18 +453,30 @@
   ).as_hlo_module()
   return hlo
 
 
 def main(argv):
   del argv
 
-  # TODO(dhchoi): Extend to TRAIN-CALIBRATE-TRAIN-CONVERT-SERVE.
+  # 1. TRAIN.
   aqt_cfg = aqt_config.fully_quantized(fwd_bits=8, bwd_bits=8)
   state = train_and_evaluate(
-      num_epochs=2, workdir='/tmp/aqt_mnist_example', aqt_cfg=aqt_cfg
+      num_epochs=1, workdir='/tmp/aqt_mnist_example', aqt_cfg=aqt_cfg
   )
-  loss = serve(state)
+
+  # 2. Calibration.
+  update_cfg_with_calibration(state.cnn_train.aqt_cfg)
+  update_cfg_with_calibration(state.cnn_eval.aqt_cfg)
+  state = calibrate(state, calibration_steps=10)
+
+  # 3. TRAIN with the calibrated stats.
+  state = train_and_evaluate(
+      num_epochs=1, workdir='/tmp/aqt_mnist_example', state=state
+  )
+
+  # 4. CONVERT & SERVE.
+  loss = serve(state, weight_only=False)
   print('serve loss on sample ds: {}'.format(loss))
 
 
 if __name__ == '__main__':
   app.run(main)
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax.py` & `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Flax layer for AQT injection."""
 
 # pylint: disable=unnecessary-lambda
 # pylint: disable=g-importing-member
 import copy
+import enum
 import functools
 from typing import Callable, Iterable, Optional, Sequence, Union
 from aqt.jax.v2 import aqt_dot_general
 from aqt.jax.v2 import aqt_tensor
 from aqt.jax.v2 import config
 from aqt.jax.v2 import tiled_dot_general
 from aqt.jax.v2 import transpose
@@ -35,14 +36,20 @@
 
 NoShardingAxes = Sequence[utils.AxisIdx]
 AxisMetadataWrapper = Callable[
     [jnp.ndarray, NoShardingAxes], nn_meta.AxisMetadata
 ]
 
 
+class FreezerMode(enum.Enum):
+  NONE = 1
+  CALIBRATION = 2
+  CALIBRATION_AND_VALUE = 3
+
+
 class Freezer(nn.Module):
   """Identity function that can freeze its input.
 
   On default it is an identity function that saves the input in a variable.
   In 'quant_mode=QuantMode.Serve' mode, ignores the input and returns the frozen
   value. It is usefult to implement 'constant folding' and put quantized weights
   and scales in the checkpoint for serving. Specifically:
@@ -155,14 +162,19 @@
   rhs_init: nn.initializers.Initializer = jnp.zeros
   rhs_scale_init: nn.initializers.Initializer = jnp.zeros
 
   # Variables only for the new Freezer.
   lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
   rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
 
+  # Freeze mode. Set as FreezerMode.CALIBRATION to store only scales; set as
+  # CALIBRATION_AND_VALUE to store both scales and quantized values.
+  lhs_freeze_mode: FreezerMode = FreezerMode.NONE
+  rhs_freeze_mode: FreezerMode = FreezerMode.CALIBRATION_AND_VALUE
+
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
   tiling_cfg: Optional[tiled_dot_general.Cfg] = None
 
   # If set to True, use the current Freezer. Otherwise, use the new
   # QuantFreezer.
@@ -315,14 +327,43 @@
       rhs_qt = rhs_freezer.get() if rhs_apply_quant_mode else self.rhs_qtensor
 
       cfg.apply_custom_vjp_on_jax = False
       out, (out_lhs_qt, out_rhs_qt) = aqt_flax_dg_core.dg_core_flax_lifted(
           lhs, rhs, lhs_qt, rhs_qt, dimension_numbers, self, cfg
       )
 
+      # Remove qvalue of the activation to not to store it in Freezer.
+      match self.lhs_freeze_mode:
+        case FreezerMode.NONE:
+          if self.lhs_apply_quant_mode and self.lhs_quant_mode in {
+              QuantMode.CONVERT,
+              QuantMode.SERVE,
+          }:
+            raise ValueError('Freezer is used with Freezer mode NONE.')
+        case FreezerMode.CALIBRATION:
+          out_lhs_qt = out_lhs_qt.without_qvalue()
+        case FreezerMode.CALIBRATION_AND_VALUE:
+          pass
+        case _:
+          raise ValueError('Unknown freeze mode: %s' % self.lhs_freeze_mode)
+
+      match self.rhs_freeze_mode:
+        case FreezerMode.NONE:
+          if self.rhs_apply_quant_mode and self.rhs_quant_mode in {
+              QuantMode.CONVERT,
+              QuantMode.SERVE,
+          }:
+            raise ValueError('Freezer is used with Freezer mode NONE.')
+        case FreezerMode.CALIBRATION:
+          out_rhs_qt = out_rhs_qt.without_qvalue()
+        case FreezerMode.CALIBRATION_AND_VALUE:
+          pass
+        case _:
+          raise ValueError('Unknown freeze mode: %s' % self.rhs_freeze_mode)
+
       # Setter
       if self.lhs_apply_quant_mode:
         lhs_freezer.set(out_lhs_qt)
       if self.rhs_apply_quant_mode:
         rhs_freezer.set(out_rhs_qt)
 
       return out
@@ -395,14 +436,19 @@
   rhs_init: nn.initializers.Initializer = jnp.zeros
   rhs_scale_init: nn.initializers.Initializer = jnp.zeros
 
   # Variables only for the new Freezer.
   lhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
   rhs_axis_metadata_wrapper: Optional[AxisMetadataWrapper] = None
 
+  # Freeze mode. Set as FreezerMode.CALIBRATION to store only scales; set as
+  # CALIBRATION_AND_VALUE to store both scales and quantized values.
+  lhs_freeze_mode: FreezerMode = FreezerMode.NONE
+  rhs_freeze_mode: FreezerMode = FreezerMode.CALIBRATION_AND_VALUE
+
   # If you want use 'params' make sure that there is another mechanism to hide
   # these variables from the optimizer.
   quant_collection: str = 'aqt'
 
   assert_eqn: Optional[str] = None
   assert_lhs_shape: Optional[utils.ShapeTemplate] = None
   assert_rhs_shape: Optional[utils.ShapeTemplate] = None
@@ -466,14 +512,17 @@
     rhs_quant_mode = self.rhs_quant_mode
     rhs_init = self.rhs_init
     rhs_axis_metadata_wrapper = self.rhs_axis_metadata_wrapper
     rhs_scale_init = self.rhs_scale_init
     rhs_var_name = self.rhs_var_name
     rhs_qtensor = rhs_g if rhs_is_qt else None
 
+    lhs_freeze_mode = self.lhs_freeze_mode
+    rhs_freeze_mode = self.rhs_freeze_mode
+
     quant_collection = self.quant_collection
     tiling_config = None
     if self.tile_sizes is not None:
       tiling_config = tiled_dot_general.Cfg.from_einsum(eqn, self.tile_sizes)
 
     if yes_swap:
       if cfg is not None:
@@ -487,14 +536,15 @@
       lhs_var_name, rhs_var_name = rhs_var_name, lhs_var_name
       lhs_is_qt, rhs_is_qt = rhs_is_qt, lhs_is_qt
       lhs_qtensor, rhs_qtensor = rhs_qtensor, lhs_qtensor
       lhs_axis_metadata_wrapper, rhs_axis_metadata_wrapper = (
           rhs_axis_metadata_wrapper,
           lhs_axis_metadata_wrapper,
       )
+      lhs_freeze_mode, rhs_freeze_mode = rhs_freeze_mode, lhs_freeze_mode
       if tiling_config is not None:
         tiling_config = tiled_dot_general.Cfg(
             lhs=tiling_config.rhs, rhs=tiling_config.lhs
         )
 
     aqt_dg = AqtDotGeneral(
         cfg=cfg,
@@ -515,9 +565,11 @@
         rhs_axis_metadata_wrapper=rhs_axis_metadata_wrapper,
         rhs_scale_init=rhs_scale_init,
         rhs_var_name=rhs_var_name,
         rhs_qtensor=rhs_qtensor,
         quant_collection=quant_collection,
         tiling_cfg=tiling_config,
         use_legacy_freezer=self.use_legacy_freezer,
+        lhs_freeze_mode=lhs_freeze_mode,
+        rhs_freeze_mode=rhs_freeze_mode,
     )
     return einsum(lhs=lhs_in, rhs=rhs_in, dg=aqt_dg)
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax_dg_core.py` & `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_dg_core.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/aqt_flax_test.py` & `aqtp-0.7.2/aqt/jax/v2/flax/aqt_flax_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/freezer.py` & `aqtp-0.7.2/aqt/jax/v2/flax/freezer.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/freezer_test.py` & `aqtp-0.7.2/aqt/jax/v2/flax/freezer_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/intercept/README.md` & `aqtp-0.7.2/aqt/jax/v2/flax/intercept/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py` & `aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py` & `aqtp-0.7.2/aqt/jax/v2/flax/intercept/aqt_intercept_methods_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py` & `aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py` & `aqtp-0.7.2/aqt/jax/v2/flax/intercept/examples/flax_e2e_intercept_model_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/numerics/fp8_numerics.py` & `aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/numerics/fp8_numerics_test.py` & `aqtp-0.7.2/aqt/jax/v2/numerics/fp8_numerics_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -236,22 +236,24 @@
     print(f"{bits:016b} {i=: 3}, {f:.9f}")
 
 
 def illustrate_bf16_2():
   def pr(n):
     n = jnp.int16(n)
     bx = jax.lax.bitcast_convert_type(n, jnp.bfloat16)
-    fp8 = fp8_numerics.sr_mantissa(bx, 2, key=jax.random.PRNGKey(0))
+    # fp8 = fp8_numerics.fp_mantissa_round(bx, 2, key=jax.random.PRNGKey(0))
     # fp8 = bx.astype(jnp.float8_e5m2)
-    fp8_n = jax.lax.bitcast_convert_type(fp8, jnp.uint8)
+    # fp8_n = jax.lax.bitcast_convert_type(fp8, jnp.uint8)
     ns = f"{n:016b}"
     ns = ns[:1] + "s " + ns[1:9] + "e " + ns[9:] + "m"
-    ns_8 = f"{fp8_n:08b}"
-    ns_8 = ns_8[:1] + "s " + ns_8[1:6] + "e " + ns_8[6:] + "m"
-    print(f"{float(bx):03.8f}[{ns}] -> {float(fp8):03.8}[{ns_8}]")
+    # print("x1", fp8, fp8_n)
+    # ns_8 = f"{fp8_n:08b}"
+    # ns_8 = ns_8[:1] + "s " + ns_8[1:6] + "e " + ns_8[6:] + "m"
+    # print(f"{float(bx):03.8f}[{ns}] -> {float(fp8):03.8}[{ns_8}]")
+    print(f"{float(bx):03.8f}[{ns}]")
 
   pr(0b0_01111111_0000000)
   pr(0b0_01111111_0001000)
   pr(0b0_01111111_0010000)  #
   pr(0b0_01111111_0011000)
   print()
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/numerics/int_numerics.py` & `aqtp-0.7.2/aqt/jax/v2/numerics/int_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/numerics/no_numerics.py` & `aqtp-0.7.2/aqt/jax/v2/numerics/no_numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/numerics/numerics.py` & `aqtp-0.7.2/aqt/jax/v2/numerics/numerics.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/pax/pax_base_ops.py` & `aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 This file contains AQT variants of these.
 """
 
 import functools
 from aqt.jax.v2 import tiled_dot_general
 import aqt.jax.v2.aqt_dot_general as aqt
 import aqt.jax.v2.config as aqt_config
+import jax
 import jax.numpy as jnp
 from praxis import base_layer
 
 
 class AqtEinsum(base_layer.BaseLayer):
   """Quantized Einsum class for model injection."""
 
@@ -53,19 +54,20 @@
       if not self.do_eval:
         train_step = self.get_var('train_step')
         self.update_var('train_step', train_step + 1)
       # train_step starts from 0 and ends at exactly the total_train_step-1
       train_step = self.get_var('train_step')
     else:
       train_step = None
-    cfg = self.cfg
-    if cfg is not None:
+    dg = self.cfg
+    if dg is not None:
       key = self.next_prng_key()
-      cfg = aqt_config.set_context(cfg, key, train_step)
-    dg = aqt.make_dot_general(cfg)
+      dg = aqt_config.set_context(dg, key, train_step)
+    else:
+      dg = jax.lax.dot_general
     if self.tiling_cfg is not None:
       dg = functools.partial(
           tiled_dot_general.tiled_dot_general,
           self.tiling_cfg,
           dot_general=dg,
       )
     # jnp.einsum is by default jitted, which makes the key storing in cfg
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/pax/pax_base_ops_test.py` & `aqtp-0.7.2/aqt/jax/v2/pax/pax_base_ops_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/stochastic_rounding.py` & `aqtp-0.7.2/aqt/jax/v2/stochastic_rounding.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/tiled_dot_general.py` & `aqtp-0.7.2/aqt/jax/v2/tiled_dot_general.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/tiled_dot_general_test.py` & `aqtp-0.7.2/aqt/jax/v2/tiled_dot_general_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax/v2/transpose.py` & `aqtp-0.7.2/aqt/jax/v2/transpose.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,14 +75,81 @@
   start = len(rhs_ba)
   end = len(lhs_shape) - len(lhs_ca) - len(lhs_ba) + start
   rhs_dummy_axes = range(start, end)
   qrhs_scale_t = jnp.expand_dims(qrhs_scale_t, axis=rhs_dummy_axes)
   return qrhs_scale_t
 
 
+def _scale_trans_back(
+    scale_t: jax.Array, ca: Sequence[utils.AxisIdx], ba: Sequence[utils.AxisIdx]
+) -> jax.Array:
+  """Transposes scale (transposed for output) back to its original dimension.
+
+  Args:
+    scale_t: scale transposed for output, without other arguments' remaining
+      axis dimensions. Output of _scale_trans.
+    ca: contracting axis.
+    ba: batching axis.
+
+  Returns:
+    Recovered scale from the scale_t.
+  """
+  ca, ba = list(ca), list(ba)
+
+  start = len(scale_t.shape)
+  end = start + len(ca)
+  scale = jnp.expand_dims(scale_t, axis=range(start, end))
+
+  ra = utils.get_remaining_axes(scale.ndim, ca, ba)
+
+  transpose_back = [-1] * len(ba + ra + ca)
+  for axis_orig, axis_transposed in enumerate(ba + ra + ca):
+    transpose_back[axis_transposed] = axis_orig
+
+  assert -1 not in transpose_back
+
+  scale = jnp.transpose(scale, transpose_back)
+  return scale
+
+
+def lhs_recover_scale_from_scale_t(
+    lhs_scale_t: jax.Array,
+    dimension_numbers: jax.lax.DotDimensionNumbers,
+    lhs_shape: Sequence[int],
+    rhs_shape: Sequence[int],
+):
+  """Recovers lhs_scale from lhs_scale_t."""
+  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
+
+  # Remove dummy axes.
+  start = len(lhs_shape) - len(lhs_ca)
+  rhs_ra_ndim = len(rhs_shape) - len(rhs_ca) - len(rhs_ba)
+  lhs_scale = jnp.squeeze(lhs_scale_t, axis=range(start, start + rhs_ra_ndim))
+
+  return _scale_trans_back(lhs_scale, lhs_ca, lhs_ba)
+
+
+def rhs_recover_scale_from_scale_t(
+    rhs_scale_t: jax.Array,
+    dimension_numbers: jax.lax.DotDimensionNumbers,
+    lhs_shape: Sequence[int],
+    rhs_shape: Sequence[int],
+):
+  """Recovers rhs_scale from rhs_scale_t."""
+  del rhs_shape
+
+  (lhs_ca, rhs_ca), (lhs_ba, rhs_ba) = dimension_numbers
+
+  start = len(rhs_ba)
+  end = len(lhs_shape) - len(lhs_ca) - len(lhs_ba) + start
+  rhs_scale = jnp.squeeze(rhs_scale_t, axis=range(start, end))
+
+  return _scale_trans_back(rhs_scale, rhs_ca, rhs_ba)
+
+
 def _scale_trans_for_other_input(
     x: jax.Array,
     my_ca: Sequence[utils.AxisIdx],
     my_ba: Sequence[utils.AxisIdx],
     other_ca: Sequence[utils.AxisIdx],
     other_ba: Sequence[utils.AxisIdx],
     other_rank: int,
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/transpose_test.py` & `aqtp-0.7.2/aqt/jax/v2/transpose_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,14 +54,21 @@
     qlhs_scale_t = transpose.lhs_scale_transpose_to_output(
         lhs_scale, dimension_numbers, lhs.shape, rhs.shape
     )
 
     self.assertIsNotNone(qlhs_scale_t)
     self.assertEqual(qlhs_scale_t.shape, expected_qlhs_scale_t_shape)
 
+    # Test recover.
+    qlhs_scale_recovered = transpose.lhs_recover_scale_from_scale_t(
+        qlhs_scale_t, dimension_numbers, lhs.shape, rhs_shape
+    )
+    self.assertEqual(lhs_scale.shape, qlhs_scale_recovered.shape)
+    assert (lhs_scale == qlhs_scale_recovered).all()
+
   @parameterized.parameters(
       # 'bmnts,bsnh->bmtnh'
       (
           (2, 3, 4, 5, 6),
           (2, 1, 4, 1),
           (2, 6, 4, 7),
           (((4,), (1,)), ((0, 2), (0, 2))),
@@ -90,14 +97,21 @@
     qrhs_scale_t = transpose.rhs_scale_transpose_to_output(
         rhs_scale, dimension_numbers, lhs.shape, rhs.shape
     )
 
     self.assertIsNotNone(qrhs_scale_t)
     self.assertEqual(qrhs_scale_t.shape, expected_qrhs_scale_t_shape)
 
+    # Test recover.
+    qrhs_scale_recovered = transpose.rhs_recover_scale_from_scale_t(
+        qrhs_scale_t, dimension_numbers, lhs.shape, rhs_shape
+    )
+    self.assertEqual(rhs_scale.shape, qrhs_scale_recovered.shape)
+    assert (rhs_scale == qrhs_scale_recovered).all()
+
   @parameterized.parameters(
       # 'bmnts,bsnh->bmtnh'
       (
           (2, 1, 4, 1, 3),
           (2, 3, 4, 5),
           (((4,), (1,)), ((0, 2), (0, 2))),
           (2, 3, 4, 1),
```

### Comparing `aqtp-0.7.1/aqt/jax/v2/utils.py` & `aqtp-0.7.2/aqt/jax/v2/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -90,41 +90,25 @@
   str_input_b = input_b if isinstance(input_b, str) else pprint.pformat(input_b)
   if remove_memory_addresses:
     str_input_a = re.sub(r' at 0x.*>', '>', str_input_a, 0, re.MULTILINE)
     str_input_b = re.sub(r' at 0x.*>', '>', str_input_b, 0, re.MULTILINE)
   assert str_input_a == str_input_b, print_diff(str_input_a, str_input_b)
 
 
-def infer_dtype_from_bits(bits: int, upcast: bool = True) -> jnp.dtype | None:
+def infer_dtype_from_bits(bits: int) -> jnp.dtype | None:
   """Get the dtype for the number of bits provided.
 
   Args:
     bits: number of bits for the dtype.
-    upcast: if upcasting the return dtype for int4 when platform is cpu.
 
   Returns:
     The corresponding container dtype for the number of bits provided.
   """
   if bits == 4:
-    # this branch should return jnp.int4 directly but
-    # lax.dot_general(int4, int4) is illegal on cpu.
-    # TODO(aqt): Remove this platform check once
-    # https://github.com/google/jax/issues/19682 is fixed.
-    if jax.local_devices()[0].platform != 'cpu':
-      return jnp.int4
-    else:
-      # TODO(yichizh): It's better to assert False here with the following msg
-      # msg = (
-      #     'lax.dot_general(int4, int4) is illegal on cpu:'
-      #     ' https://github.com/google/jax/issues/19682. The simple workaround'
-      #     ' is to upcast to int8, but in that case please directly set the'
-      #     ' numerics bits to int8. Please contact the AQT team if you believe'
-      #     ' the workaround is needed.'
-      # )
-      return jnp.int8 if upcast else jnp.int4
+    return jnp.int4
   else:
     if bits <= 8 and bits >= 2:
       return jnp.int8
     else:
       return None
```

### Comparing `aqtp-0.7.1/aqt/jax_legacy/README.md` & `aqtp-0.7.2/aqt/jax_legacy/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb` & `aqtp-0.7.2/aqt/jax_legacy/colabs/gradients_wrt_variables_in_flax.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/README.md` & `aqtp-0.7.2/aqt/jax_legacy/jax/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/compute_cost_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/compute_cost_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/compute_cost_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax/struct.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax/struct.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax_attention.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax_attention_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax_attention_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax_layers.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/flax_layers_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/flax_layers_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/fp_cast.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/fp_cast_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/fp_cast_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/get_bounds.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/get_bounds_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/get_bounds_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/hlo_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/hlo_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/hlo_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/README.md` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/check_config_util.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/check_config_util.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/base_config.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/README.md` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w4_a4_init8_dense8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/paper/resnet50_w8_a8_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w1_a4_auto.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w8_a1_norelu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/experimental/resnet50_w_only_halfshift_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/pokebnn/pokebnn_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet101_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet152_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a2_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_dense8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_a4_init8_momax.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w4_init8_dense8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs/resnet50_w8_a8_fixed.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_script/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/configs_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/configs_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/hparams_config.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/hparams_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/imagenet.png` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/imagenet.png`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/input_pipeline.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/models.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/models_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/pokebnn.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/pokebnn_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/pokebnn_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/resnet_cost_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_benchmark.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_benchmark.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/imagenet/train_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/imagenet/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/primitives.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/primitives.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/primitives_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/primitives_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/quant_config.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/quant_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/quantization.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/quantization_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/quantization_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/shape_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/shape_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/sparsity/sparsity_core_depr_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/stats.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/stats_tag.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/stats_tag_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/stats_tag_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/stats_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/stats_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/test_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/test_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/train_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/train_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/train_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/train_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/utils.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/README.md` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/bleu.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/bleu.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/decode.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/decode.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/gen_hlo.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_config_scripts/config_schema_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/base_config.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_4bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_and_auto_acts_reset_stats.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/full_model_8bit_weights_only_int8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/minimal_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_2bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_auto_acts_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_auto_acts_float.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_8bit_weights_only_fq.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/small_model_bfloat16_no_logit_sharing.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_128_128.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_16_16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_32_32.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/snn2022-experiments/structure_decay/sparsity_sweep_64_64.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/dense_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_decoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_dense_weights_only_structured_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_acts_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/full_model_bfloat16_sparse_encoder_dense_weights_only_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_acts_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/small_model_bfloat16_sparse_encoder_decoder_dense_weights_only_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity/structured_sparsity_dense_weights_only_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/baseline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_acts/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_2bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/quant_4bit_weights_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sparsity_structured_1_8.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_and_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_attention_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_4bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/quant_8bit_sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sparsity_structured_2_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/sparsity_and_quantization/dense_weights/sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/dense_sparsity_decay_nm.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/model_size_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/quant_sparsity_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/small_model_decay_sparsity_1_4.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/sparsity_decay_nm_quant_wa.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/structured_sparsity_decay_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/experimental/tmlr/wa_quantization.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/__init__.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_4bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_auto_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_and_fixed_acts.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_8bit_weights_only.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/full_model_bfloat16.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/hparams_configs/leaderboard/leaderboard_sweep.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/input_pipeline.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/models.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/models_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/models_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/predict.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/predict.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_flags.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/train_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/train_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_generator_lib.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py` & `aqtp-0.7.2/aqt/jax_legacy/jax/wmt_mlperf/training_hparams_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/README.md` & `aqtp-0.7.2/aqt/jax_legacy/utils/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/__init__.py` & `aqtp-0.7.2/aqt/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,9 +7,10 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""Accurate Quantized Training library."""
 
-
+__version__ = "0.7.2"
```

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/analysis_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/analysis_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/analysis_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/common.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/common.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/config_schema_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/config_schema_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/config_schema_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/hparams_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/hparams_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/pandas_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/pandas_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/pandas_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/report_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/report_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/report_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/report_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/summary_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/summary_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/summary_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/tfevent_utils.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/jax_legacy/utils/tfevent_utils_test.py` & `aqtp-0.7.2/aqt/jax_legacy/utils/tfevent_utils_test.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/test/aqt_conv_test_base.py` & `aqtp-0.7.2/aqt/test/aqt_conv_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/test/aqt_matmul_test_base.py` & `aqtp-0.7.2/aqt/test/aqt_matmul_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/test/aqt_stats_test_base.py` & `aqtp-0.7.2/aqt/test/aqt_stats_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/test/aqt_tensor_test_base.py` & `aqtp-0.7.2/aqt/test/aqt_tensor_test_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/aqt/test/aqt_test_shared_base.py` & `aqtp-0.7.2/aqt/test/aqt_test_shared_base.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/papers/aqt/aqt.pdf` & `aqtp-0.7.2/papers/aqt/aqt.pdf`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/papers/aqt/aqt.tex` & `aqtp-0.7.2/papers/aqt/aqt.tex`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/papers/pokebnn/README.md` & `aqtp-0.7.2/papers/pokebnn/README.md`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/papers/pokebnn/cloudtpu_train_pokebnn.sh` & `aqtp-0.7.2/papers/pokebnn/cloudtpu_train_pokebnn.sh`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/papers/pokebnn/tensorboard.ipynb` & `aqtp-0.7.2/papers/pokebnn/tensorboard.ipynb`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/pyproject.toml` & `aqtp-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/setup.py` & `aqtp-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `aqtp-0.7.1/PKG-INFO` & `aqtp-0.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aqtp
-Version: 0.7.1
+Version: 0.7.2
 Summary: Accurate Quantized Training library.
 Author-email: Lukasz Lew <lew@google.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
```

