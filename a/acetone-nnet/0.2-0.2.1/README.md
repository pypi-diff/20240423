# Comparing `tmp/acetone_nnet-0.2.tar.gz` & `tmp/acetone_nnet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acetone_nnet-0.2.tar", last modified: Fri Apr 19 14:31:54 2024, max compression
+gzip compressed data, was "acetone_nnet-0.2.1.tar", last modified: Tue Apr 23 14:56:19 2024, max compression
```

## Comparing `acetone_nnet-0.2.tar` & `acetone_nnet-0.2.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.425223 acetone_nnet-0.2/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2/AUTHORS.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2/COPYING
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2/LICENSE
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7847 2024-04-19 14:31:54.425223 acetone_nnet-0.2/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6470 2024-04-16 12:29:53.000000 acetone_nnet-0.2/README.md
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2056 2024-04-19 14:31:46.000000 acetone_nnet-0.2/pyproject.toml
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-19 14:31:54.425223 acetone_nnet-0.2/setup.cfg
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.401222 acetone_nnet-0.2/src/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.407223 acetone_nnet-0.2/src/acetone_nnet/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.2/src/acetone_nnet/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.408223 acetone_nnet-0.2/src/acetone_nnet/bin/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2/src/acetone_nnet/bin/bin_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2/src/acetone_nnet/cli_acetone.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2/src/acetone_nnet/cli_compare.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.408223 acetone_nnet-0.2/src/acetone_nnet/code_generator/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/Layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-18 12:29:33.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/activation_functions.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.410223 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/AddBias.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3168 2024-04-17 09:50:55.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/BatchNormalization.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.411223 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1672 2024-04-18 13:27:34.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1677 2024-04-18 13:28:07.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1688 2024-04-18 13:28:11.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1687 2024-04-18 13:28:13.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Concatenate.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.412222 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Dense.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Dot.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Flatten.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Gather.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Gemm.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Input.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/MatMul.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.413223 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.414223 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.414223 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-15 06:49:35.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Softmax.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/__init__.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.2/src/acetone_nnet/code_generator/neural_network.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.415223 acetone_nnet-0.2/src/acetone_nnet/format_importer/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.415223 acetone_nnet-0.2/src/acetone_nnet/format_importer/H5_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18238 2024-04-19 13:55:52.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.415223 acetone_nnet-0.2/src/acetone_nnet/format_importer/JSON_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14173 2024-04-19 12:59:15.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.415223 acetone_nnet-0.2/src/acetone_nnet/format_importer/NNET_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.416223 acetone_nnet-0.2/src/acetone_nnet/format_importer/ONNX_importer/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)    27450 2024-04-18 12:36:48.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4103 2024-04-18 14:54:31.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3220 2024-04-19 13:56:29.000000 acetone_nnet-0.2/src/acetone_nnet/format_importer/parser.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.416223 acetone_nnet-0.2/src/acetone_nnet/graph/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/graph/graph_interpretor.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.417223 acetone_nnet-0.2/src/acetone_nnet/templates/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2/src/acetone_nnet/templates/__init__.py
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.419223 acetone_nnet-0.2/src/acetone_nnet/templates/layers/
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.421223 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.422223 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.423223 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.424223 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Dense.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Dot.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Gather.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.424223 acetone_nnet-0.2/src/acetone_nnet/templates/memory_layout/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.425223 acetone_nnet-0.2/src/acetone_nnet/templates/normalization/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_Makefile.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_global_var_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_header_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_main_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_source_file.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
-drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-19 14:31:54.425223 acetone_nnet-0.2/src/acetone_nnet.egg-info/
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7847 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/PKG-INFO
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/SOURCES.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/dependency_links.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/entry_points.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/requires.txt
--rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-19 14:31:54.000000 acetone_nnet-0.2/src/acetone_nnet.egg-info/top_level.txt
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.457060 acetone_nnet-0.2.1/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      521 2024-04-16 11:45:42.000000 acetone_nnet-0.2.1/AUTHORS.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7652 2024-03-15 08:14:43.000000 acetone_nnet-0.2.1/COPYING
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    35149 2024-03-15 08:14:43.000000 acetone_nnet-0.2.1/LICENSE
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7876 2024-04-23 14:56:19.457060 acetone_nnet-0.2.1/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6497 2024-04-19 14:35:17.000000 acetone_nnet-0.2.1/README.md
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2058 2024-04-23 14:55:49.000000 acetone_nnet-0.2.1/pyproject.toml
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       38 2024-04-23 14:56:19.457060 acetone_nnet-0.2.1/setup.cfg
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.088055 acetone_nnet-0.2.1/src/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.163056 acetone_nnet-0.2.1/src/acetone_nnet/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1790 2024-04-16 15:00:34.000000 acetone_nnet-0.2.1/src/acetone_nnet/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.165056 acetone_nnet-0.2.1/src/acetone_nnet/bin/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3252 2024-04-19 14:31:39.000000 acetone_nnet-0.2.1/src/acetone_nnet/bin/bin_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2788 2024-04-19 14:05:22.000000 acetone_nnet-0.2.1/src/acetone_nnet/cli_acetone.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3838 2024-04-15 08:13:08.000000 acetone_nnet-0.2.1/src/acetone_nnet/cli_compare.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.175056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4134 2024-04-15 07:57:10.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/Layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1896 2024-04-17 13:07:48.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4570 2024-04-18 12:29:33.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/activation_functions.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.177056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2775 2024-04-15 06:49:10.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/AddBias.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3168 2024-04-17 09:50:55.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/BatchNormalization.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.178056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1678 2024-04-23 14:51:52.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1569 2024-04-12 11:51:45.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4874 2024-04-18 12:32:50.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1683 2024-04-23 14:51:35.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1582 2024-04-12 11:52:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1581 2024-04-12 11:52:22.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1694 2024-04-23 14:51:42.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1693 2024-04-23 14:51:25.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1382 2024-04-15 09:49:48.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3996 2024-04-15 06:49:02.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Concatenate.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.179056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3756 2024-04-12 11:58:09.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2993 2024-04-15 11:39:05.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6147 2024-04-15 06:50:21.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5339 2024-04-15 06:50:17.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5462 2024-04-15 06:50:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1355 2024-04-15 09:50:26.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2971 2024-04-15 06:48:55.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Dense.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4577 2024-04-15 06:48:50.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Dot.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2378 2024-04-15 06:48:42.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Flatten.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3931 2024-04-15 06:48:36.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Gather.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     8032 2024-04-15 06:48:30.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Gemm.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2266 2024-04-15 06:48:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Input.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3196 2024-04-15 06:48:05.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/MatMul.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.180056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3329 2024-04-15 06:50:07.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3757 2024-04-15 06:50:03.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2583 2024-04-12 11:58:05.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3793 2024-04-15 06:49:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4025 2024-04-15 06:49:54.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1282 2024-04-15 09:51:29.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.181056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2014 2024-04-12 11:47:01.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1847 2024-04-12 11:47:16.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4895 2024-04-15 06:49:42.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1234 2024-04-15 09:51:58.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.182056 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7182 2024-04-12 11:57:55.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    10459 2024-04-22 07:07:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5009 2024-04-15 06:49:30.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4271 2024-04-15 09:47:36.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1267 2024-04-15 09:52:28.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2174 2024-04-15 06:47:37.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Softmax.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2223 2024-04-16 15:00:06.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/__init__.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    25022 2024-04-18 12:37:47.000000 acetone_nnet-0.2.1/src/acetone_nnet/code_generator/neural_network.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.182056 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.182056 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/H5_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7452 2024-04-18 15:31:47.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    18250 2024-04-23 14:53:07.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.182056 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/JSON_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    14173 2024-04-19 12:59:15.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.183056 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/NNET_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3873 2024-04-15 06:44:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5960 2024-04-12 14:44:42.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.183056 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/ONNX_importer/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)    27783 2024-04-23 14:51:14.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     4062 2024-04-23 14:52:35.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2976 2024-04-23 13:01:02.000000 acetone_nnet-0.2.1/src/acetone_nnet/format_importer/parser.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.183056 acetone_nnet-0.2.1/src/acetone_nnet/graph/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     5624 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/graph/graph_interpretor.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.244057 acetone_nnet-0.2.1/src/acetone_nnet/templates/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1046 2024-04-15 06:29:33.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/__init__.py
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.327058 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.381059 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1625 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      832 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      681 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      872 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      683 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      143 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_indirect_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      375 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_std_gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      875 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      868 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.401059 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_Gemm.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      853 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      705 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      748 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      729 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.425059 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1266 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      669 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1001 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      604 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      507 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Wrap_Pad.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.433059 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1268 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     3246 2024-04-22 07:07:11.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1021 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1445 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      778 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      352 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_AddBiase.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      532 2024-04-17 09:50:38.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     2282 2024-04-18 12:38:10.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1274 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      699 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Dense.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      733 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Dot.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      567 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1284 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Gather.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      658 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      831 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1265 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      312 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Softmax.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.441059 acetone_nnet-0.2.1/src/acetone_nnet/templates/memory_layout/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      118 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/memory_layout/template_channels_first_output.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      448 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/memory_layout/template_channels_last_output.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.452060 acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      341 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      238 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/template_normalization_cst_in_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      167 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/template_post_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      512 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      237 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_Makefile.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1034 2024-04-18 12:38:03.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_global_var_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1064 2024-04-18 12:38:21.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_header_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1105 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_main_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     1225 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_source_file.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      227 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_test_dataset_header.c.tpl
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       96 2024-04-11 15:00:57.000000 acetone_nnet-0.2.1/src/acetone_nnet/templates/template_test_dataset_source.c.tpl
+drwxr-xr-x   0 yaitaiss (108938) dtis      (4100)        0 2024-04-23 14:56:19.456060 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     7876 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/PKG-INFO
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)     6924 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/SOURCES.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)        1 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/dependency_links.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)      146 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/entry_points.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       82 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/requires.txt
+-rw-r--r--   0 yaitaiss (108938) dtis      (4100)       13 2024-04-23 14:56:19.000000 acetone_nnet-0.2.1/src/acetone_nnet.egg-info/top_level.txt
```

### Comparing `acetone_nnet-0.2/AUTHORS.md` & `acetone_nnet-0.2.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/COPYING` & `acetone_nnet-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/LICENSE` & `acetone_nnet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/PKG-INFO` & `acetone_nnet-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2
+Version: 0.2.1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -95,30 +95,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+acetone_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run them, use the `run_tests.py` script from the `tests/` folder.
@@ -140,27 +140,27 @@
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+acetone_generate tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
 make -C tests/models/acas/acas_decr128/output_acetone all
 ./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
-cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+acetone_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+acetone_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
```

### Comparing `acetone_nnet-0.2/README.md` & `acetone_nnet-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -68,30 +68,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+acetone_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run them, use the `run_tests.py` script from the `tests/` folder.
@@ -113,27 +113,27 @@
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+acetone_generate tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
 make -C tests/models/acas/acas_decr128/output_acetone all
 ./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
-cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+acetone_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+acetone_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
```

### Comparing `acetone_nnet-0.2/pyproject.toml` & `acetone_nnet-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 include-package-data = true
 
 [project]
 name = "acetone-nnet"
-version = "0.2"
+version = "0.2.1"
 requires-python = ">=3.10"
 
 authors = [
     { name="Yanis AIT-AISSA", email="Yanis.AIT-AISSA@student.isae-supaero.fr"},
     { name="Thomas CARLE", email="Thomas.Carle@irit.fr" },
     { name="Iryna DE ALBUQUERQUE SILVA", email="Iryna.De_Albuquerque_Silva@onera.fr" },
     { name="Adrien GAUFFRIAU", email="Adrien.Gauffriau@airbus.com" },
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/bin/bin_acetone.py` & `acetone_nnet-0.2.1/src/acetone_nnet/bin/bin_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/cli_acetone.py` & `acetone_nnet-0.2.1/src/acetone_nnet/cli_acetone.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/cli_compare.py` & `acetone_nnet-0.2.1/src/acetone_nnet/cli_compare.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/Layer.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/Layer.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/activation_functions.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/activation_functions.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/AddBias.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/AddBias.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/BatchNormalization.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/BatchNormalization.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,27 +16,27 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 
-#Addition of several tensor
-class Add(Broadcast):
+#Division of several tensors
+class Divide(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Add'
-        self.specific_operator = ' + '
+        self.name = 'Divide'
+        self.specific_operator = '/'
     
     def forward_path_layer(self, inputs):
         if(self.constant is None):
-            constant = 0
+            constant = 1
         else: 
             constant = self.constant
-        if(len(inputs.shape) == 4):
+        if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output *= input
+                output /= input
         else:
             output = inputs
-        return self.activation_function.compute(output+constant)
+        return self.activation_function.compute(output/constant)
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Average.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Broadcast.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Divide.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,27 +16,27 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 
-#Division of several tensors
-class Divide(Broadcast):
+#Multiplication of several tensors
+class Multiply(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Divide'
-        self.specific_operator = '/'
+        self.name = 'Multiply'
+        self.specific_operator = '*'
     
     def forward_path_layer(self, inputs):
         if(self.constant is None):
             constant = 1
         else: 
             constant = self.constant
-        if(len(inputs.shape) == 4):
+        if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
                 output *= input
         else:
             output = inputs
-        return self.activation_function.compute(output/constant)
+        return self.activation_function.compute(constant*output)
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Maximum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Minimum.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Multiply.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Add.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,27 +16,27 @@
  * You should have received a copy of the GNU Lesser General Public License along with this program ;
  * if not, write to the Free Software Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA 02111-1307  USA
  ******************************************************************************
 """
 
 from .Broadcast import Broadcast
 
-#Multiplication of several tensors
-class Multiply(Broadcast):
+#Addition of several tensor
+class Add(Broadcast):
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.name = 'Multiply'
-        self.specific_operator = '*'
+        self.name = 'Add'
+        self.specific_operator = ' + '
     
     def forward_path_layer(self, inputs):
         if(self.constant is None):
-            constant = 1
+            constant = 0
         else: 
             constant = self.constant
-        if(len(inputs.shape) == 4):
+        if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output *= input
+                output += input
         else:
             output = inputs
-        return self.activation_function.compute(constant*output)
+        return self.activation_function.compute(output+constant)
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/Subtract.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,14 @@
         self.specific_operator = ' - '
     
     def forward_path_layer(self, inputs):
         if(self.constant is None):
             constant = 0
         else: 
             constant = self.constant
-        if(len(inputs.shape) == 4):
+        if(len(self.previous_layer) > 1):
             output = inputs[0]
             for input in inputs[1:]:
-                output *= input
+                output -= input
         else:
             output = inputs
         return self.activation_function.compute(output-constant)
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Broadcast_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Concatenate.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Concatenate.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_6loops.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_indirect_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/Conv2D_std_gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Conv_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Dense.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Dense.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Dot.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Dot.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Flatten.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Flatten.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Gather.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Gather.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Gemm.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Gemm.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Input.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Input.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/MatMul.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/MatMul.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ConstantPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/EdgePad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/Pad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/ReflectPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/WrapPad.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pad_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/AveragePooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/MaxPooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/Pooling2D.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Pooling_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/Resize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeCubic.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeLinear.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/ResizeNearest.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Resize_layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/Softmax.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/Softmax.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/layers/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/code_generator/neural_network.py` & `acetone_nnet-0.2.1/src/acetone_nnet/code_generator/neural_network.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/H5_importer/JSON_from_keras_model.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/H5_importer/parser_h5.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/H5_importer/parser_h5.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,24 +56,26 @@
         return dimensions
     elif(len(dimensions) == 4):
         return (dimensions[0],dimensions[3],dimensions[1],dimensions[2])
     else:
         return dimensions
 
 def get_input_dimensions(input,data_format):
-    dimensions = input
-    if(data_format == 'channels_first'):
-        return dimensions
+    if(type(input) == list and len(input) == 1):
+        dimensions = input[0]
     else:
-        if(type(input) == list and len(input[0]) == 4):
-            return [(shape[0],shape[3],shape[1],shape[2]) for shape in dimensions]
-        elif(type(input) is not list and len(input) == 4):
-            return (dimensions[0],dimensions[3],dimensions[1],dimensions[2])
-        else: 
-            return dimensions
+        dimensions = input
+    
+    if(data_format == 'channels_last'):
+        if(type(dimensions) == list and len(dimensions[0]) == 4):
+            dimensions = [(shape[0],shape[3],shape[1],shape[2]) for shape in dimensions]
+        elif(type(dimensions) is not list and len(dimensions) == 4):
+            dimensions =  (dimensions[0],dimensions[3],dimensions[1],dimensions[2])
+    
+    return np.array(dimensions)
 
 def create_actv_function_obj(kears_activation_obj):
         if kears_activation_obj == keras.activations.sigmoid:
             return Sigmoid()
         elif kears_activation_obj == keras.activations.relu:
             return ReLu()
         elif kears_activation_obj == keras.activations.tanh:
@@ -94,23 +96,28 @@
         return Conv2D_std_gemm(**kwargs)   
 
     elif 'indirect_gemm' in algorithm:
         return Conv2D_indirect_gemm(**kwargs)
 
 def load_keras(file_to_parse:keras.Model, conv_algorithm):
 
+    if(type(file_to_parse) == str): 
+        model = keras.models.load_model(file_to_parse)
+    else:
+        model = file_to_parse
+
     input_layer_size = 1
-    for i in range(1, len(file_to_parse.input.shape)): #start in idx 1 cause idx 0 represents batch size, so it's None in inference phase
-        input_layer_size = input_layer_size * file_to_parse.input.shape[i]
+    for i in range(1, len(model.input.shape)): #start in idx 1 cause idx 0 represents batch size, so it's None in inference phase
+        input_layer_size = input_layer_size * model.input.shape[i]
     
     data_format = 'channels_first'
-    if(hasattr(layer, 'data_format') and layer.data_format == 'channels_last' for layer in file_to_parse.layers):
+    if(hasattr(layer, 'data_format') and layer.data_format == 'channels_last' for layer in model.layers):
         data_format = 'channels_last'
 
-    data_type = file_to_parse.layers[0].dtype
+    data_type = model.layers[0].dtype
 
     if data_type == 'float64':
         data_type = 'double'
         data_type_py = np.float64
 
     elif data_type == 'float32':
         data_type = 'float'
@@ -120,32 +127,32 @@
         data_type = 'long int'
         data_type_py = np.int32
     
     
     
     layers = []
 
-    if file_to_parse.layers[0].__class__.__name__ == 'InputLayer':
+    if model.layers[0].__class__.__name__ == 'InputLayer':
         l_temp = InputLayer(idx = 0,
-                            size = get_layer_size(file_to_parse.layers[0]),
-                            input_shape = get_input_dimensions(file_to_parse.layers[0].input_shape, data_format),
+                            size = get_layer_size(model.layers[0]),
+                            input_shape = get_input_dimensions(model.layers[0].input_shape, data_format),
                             data_format = data_format)
         start = 1
     else:
         l_temp = InputLayer(idx = 0, 
                             size = input_layer_size,
-                            input_shape = get_input_dimensions(file_to_parse.input_shape),
+                            input_shape = get_input_dimensions(model.input_shape, data_format),
                             data_format = data_format)
         start = 0
     
     layers.append(l_temp)
 
     nb_softmax_layers = 0
 
-    for idx, layer_keras in list(islice(enumerate(file_to_parse.layers), start, None)):
+    for idx, layer_keras in list(islice(enumerate(model.layers), start, None)):
         add_softmax_layer = False
         idx += 1-start
         idx += nb_softmax_layers
 
         if hasattr(layer_keras, 'activation'):
             if layer_keras.activation == keras.activations.softmax:
                 add_softmax_layer = True
@@ -190,34 +197,34 @@
                                               biases = biases,
                                               activation_function = create_actv_function_obj(layer_keras.activation))
         
         elif layer_keras.__class__.__name__ == 'AveragePooling2D':
             current_layer = AveragePooling2D(idx = idx,
                                              size = get_layer_size(layer_keras),
                                              padding = layer_keras.padding,
-                                             strides = layer_keras.strides,
-                                             pool_size = layer_keras.pool_size,
+                                             strides = layer_keras.strides[0],
+                                             pool_size = layer_keras.pool_size[0],
                                              input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
                                              output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
                                              activation_function = Linear())
             
         elif layer_keras.__class__.__name__ == 'MaxPooling2D':
             current_layer = MaxPooling2D(idx = idx,
                                          size = get_layer_size(layer_keras),
                                          padding = layer_keras.padding,
-                                         strides = layer_keras.strides,
-                                         pool_size = layer_keras.pool_size,
+                                         strides = layer_keras.strides[0],
+                                         pool_size = layer_keras.pool_size[0],
                                          input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
                                          output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
                                          activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'Flatten':
             current_layer = Flatten(idx = idx,
                                     size = get_layer_size(layer_keras),
-                                    intput_shape = get_input_dimensions(layer_keras.input_shape, data_format),
+                                    input_shape = get_input_dimensions(layer_keras.input_shape, data_format),
                                     data_format= data_format)
         
         elif layer_keras.__class__.__name__ == 'Add':
             current_layer = Add(idx = idx,
                                 size = get_layer_size(layer_keras),
                                 input_shapes = get_input_dimensions(layer_keras.input_shape, data_format),
                                 output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
@@ -265,21 +272,21 @@
                     axis =1
                 else: 
                     axis = axis + 1
             current_layer = Concatenate(idx = idx,
                                         size = get_layer_size(layer_keras),
                                         axis = axis,
                                         input_shapes = get_input_dimensions(layer_keras.input_shape, data_format),
-                                        output_shape = get_output_dimensions(layer_keras, data_format),
+                                        output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
                                         activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'Dot':
             current_layer = Dot(idx = idx,
                                 size = get_layer_size(layer_keras),
-                                axis = axis,
+                                axis = layer_keras.axes,
                                 input_shapes = get_input_dimensions(layer_keras.input_shape, data_format),
                                 output_shape = get_output_dimensions(layer_keras.output_shape, data_format),
                                 activation_function = Linear())
         
         elif layer_keras.__class__.__name__ == 'ZeroPadding2D':
             pads = layer_keras.padding
             if type(pads) == int:
@@ -319,39 +326,37 @@
 
         elif layer_keras.__class__.__name__ == 'Permute':
             continue
 
         else:
             raise TypeError("Error: layer "+layer_keras.__class__.__name__+" not supported\n")
 
-        if type(file_to_parse) == keras.Sequential:
-            if idx - 1 > 0:
+        if type(model) == keras.Sequential:
+            if idx - 1 >= 0:
                 current_layer.previous_layer.append(layers[idx-1])
                 layers[idx-1].next_layer.append(current_layer)
         else:
             if(type(layer_keras.input) == list):
                 for input in layer_keras.input:
-                    for k in range(len(file_to_parse.layers)):
-                        prev_layer = file_to_parse.layers[k]
+                    for k in range(len(model.layers)):
+                        prev_layer = model.layers[k]
                         if prev_layer.name == input._keras_history.layer.name:
                             current_layer.previous_layer.append(layers[k])
                             layers[k].next_layer.append(current_layer)
                             break
             else:
-                for k in range(len(file_to_parse.layers)):
-                    prev_layer = file_to_parse.layers[k]
+                for k in range(len(model.layers)):
+                    prev_layer = model.layers[k]
                     if prev_layer.name == layer_keras.input._keras_history.layer.name:
-                        print(current_layer.name, prev_layer.name, layer_keras.input._keras_history.layer.name, k)
                         current_layer.previous_layer.append(layers[k])
                         layers[k].next_layer.append(current_layer)
                         break
 
             
         l_temp = current_layer
-        layers.append(l_temp)
 
         if add_softmax_layer:
             nb_softmax_layers += 1
             current_layer = Softmax(idx = idx,
                                     size = l_temp.size)
             l_temp.next_layer.append(current_layer)
             current_layer.previous_layer.append(l_temp)
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/JSON_importer/parser_JSON.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/NNET_importer/nnet_normalize.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/NNET_importer/parser_NNET.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/ONNX_importer/create_layer.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Conv2D_6loops, Conv2D_std_gemm, Conv2D_indirect_gemm,
     Edge_pad, Wrap_pad, Reflect_pad, Constant_Pad,
     Add, Multiply, Subtract, Divide, Maximum, Minimum, Average,
     ResizeCubic, ResizeLinear, ResizeNearest,
     Concatenate, InputLayer, Softmax,  Dot, Gather, Gemm, MatMul, Add_Bias
 )
 
-from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm
+from ...code_generator.activation_functions import Linear, ReLu, Sigmoid, TanH, Clip, Exponential, Logarithm, LeakyReLu
 
 ###### Utility functions ######
 
 def create_conv2d_obj(algorithm, **kwargs):
        
     if '6loops' in algorithm:
         return Conv2D_6loops(**kwargs)
@@ -93,16 +93,16 @@
             shape = [info.type.tensor_type.shape.dim[i].dim_value for i in range(len(info.type.tensor_type.shape.dim))]
     for input in model.graph.input:
         if(shape_name == input.name):
             shape = [input.type.tensor_type.shape.dim[i].dim_value for i in range(len(input.type.tensor_type.shape.dim))]
     for output in model.graph.output:
         if(shape_name == output.name):
             shape = [output.type.tensor_type.shape.dim[i].dim_value for i in range(len(output.type.tensor_type.shape.dim))]
-    if (shape and len(shape)<=3):
-        shape = [1 for i in range(3-len(shape))] + shape
+    if (shape and len(shape)<=4):
+        shape = [1 for i in range(4-len(shape))] + shape
     for i in range(len(shape)):
         if shape[i] == 0:
             shape[i] = 1
     return shape
 
 #Return the size of the layer when given the list output_shape
 def find_size(output_shape):
@@ -666,30 +666,36 @@
     bypass(node,dict_output,model)
 
 #Fuse the activation layer Sigmoide with the prior layer
 def fuse_Exp(node,dict_output,model,layers):
     layers[dict_output[node.input[0]]].activation_function = Exponential()
     bypass(node,dict_output,model)
 
-#Fuse the activation layer Sigmoide with the prior layer
+#Fuse the activation layer Sigmoid with the prior layer
 def fuse_Log(node,dict_output,model,layers):
     layers[dict_output[node.input[0]]].activation_function = Logarithm()
     bypass(node,dict_output,model)
 
 #Fuse a layer Clip with the prior layer
 def fuse_Clip(node,dict_output,model,layers):
     min, max = float('-inf'), float('inf')
     if(node.input[1]):
         min = onnx.numpy_helper.to_array(look_for_initializer(node.input[1],model))[0]
     if(node.input[2]):
         max = onnx.numpy_helper.to_array(look_for_initializer(node.input[2],model))[0]
     layers[dict_output[node.input[0]]].activation_function = Clip(max=max,min=min)
     bypass(node,dict_output,model)
-    
+
+#Fuse the activation layer LeakyRelu with the prior layer
+def fuse_LeakyReLu(node,dict_output,model,layers):
+    attribut = extract_attribut(node)
+    layers[dict_output[node.input[0]]].activation_function = LeakyReLu(alpha=attribut['alpha'])
+    bypass(node,dict_output,model)
     
 ###### Dict of all the functions ######
 activation_layers = {"Relu":fuse_ReLu,
                      "Tanh":fuse_Tanh,
                      "Sigmoid":fuse_Sigmoid,
                      "Clip":fuse_Clip,
                      "Exp":fuse_Exp,
-                     "Log":fuse_Log}
+                     "Log":fuse_Log,
+                     "LeakyRelu":fuse_LeakyReLu}
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/ONNX_importer/parser_ONNX.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,17 +37,16 @@
     dict_output = {}
     #Dictionnary of the inputs of each layers: {layer_idx_to_which_the_inputs_go:[inputs_name]}
     dict_input = {}
     #Indice of the layer
     idx = 0
 
     #Creating and adding all the input layers to the list
-    for input_layer in model.graph.input:
-        layers.append(create_Input_Layer(input_layer,idx,dict_output))
-        idx+=1
+    layers.append(create_Input_Layer(model.graph.input[0],idx,dict_output))
+    idx+=1
     
     #Going through all the nodes to creat the layers and add them to the list
     for node in model.graph.node:
         if(node.op_type in layer_type): #If the node is a useful layer, we add it to the list
             if(node.op_type == "Conv"):    
                 layers.append(layer_type[node.op_type](node,idx,dict_input,dict_output,model,conv_algorithm))
                 idx+=1
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/format_importer/parser.py` & `acetone_nnet-0.2.1/src/acetone_nnet/format_importer/parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,22 +46,15 @@
         if("json" in  file_to_parse[-4:]):
             return load_json(file_to_parse, conv_algorithm)
         
         elif("onnx" in file_to_parse[-4:]):
             return load_onnx(file_to_parse, conv_algorithm)
         
         elif("h5" in file_to_parse[-4:]):
-            model = keras.models.load_model(file_to_parse)
-
-            print("Creating the .json file...")
-            new_path = get_path(file_to_parse,"json")
-            JSON_from_keras_model(model, new_path)
-            print("File created\n")
-
-            return load_json(new_path, conv_algorithm)
+            return load_keras(file_to_parse, conv_algorithm)
         
         elif("nnet" in file_to_parse[-4:]):
             return load_nnet(file_to_parse,normalize)
         
         else:
             print("\nError: model description ."+file_to_parse[-4:]+" not supported")
             raise TypeError("Error: model description ."+file_to_parse[-4:]+" not supported\nOnly description supported are: .nnet, .h5, .json, .onnx\n")
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet/graph/graph_interpretor.py` & `acetone_nnet-0.2.1/src/acetone_nnet/graph/graph_interpretor.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/__init__.py` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_6loops.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_Conv_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_im2col.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Conv/template_im2row.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_nt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tn.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Gemm/template_gemm_tt.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Constant_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Edge_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Pad_Non_Constant.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Pad/template_Reflect_Pad.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeCubic2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear1D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeLinear2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/Resize/template_ResizeNearest.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_BatchNormalization.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Broadcast.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Concatenate.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Dense.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Dense.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Dot.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Dot.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Flatten.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Flatten.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Gather.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Gather.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Input_Layer.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_MatMul.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_MatMul.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/layers/template_Pooling2D.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/normalization/template_pre_processing.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/template_global_var_file.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/template_global_var_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/template_header_file.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/template_header_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/template_main_file.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/template_main_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet/templates/template_source_file.c.tpl` & `acetone_nnet-0.2.1/src/acetone_nnet/templates/template_source_file.c.tpl`

 * *Files identical despite different names*

### Comparing `acetone_nnet-0.2/src/acetone_nnet.egg-info/PKG-INFO` & `acetone_nnet-0.2.1/src/acetone_nnet.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acetone-nnet
-Version: 0.2
+Version: 0.2.1
 Summary: Predictable programming framework for ML applications in safety-critical systems.
 Author-email: Yanis AIT-AISSA <Yanis.AIT-AISSA@student.isae-supaero.fr>, Thomas CARLE <Thomas.Carle@irit.fr>, Iryna DE ALBUQUERQUE SILVA <Iryna.De_Albuquerque_Silva@onera.fr>, Adrien GAUFFRIAU <Adrien.Gauffriau@airbus.com>, Benjamin LESAGE <benjamin.lesage@onera.fr>, Claire PAGETTI <Claire.Pagetti@onera.fr>
 Project-URL: Repository, https://github.com/onera/acetone/
 Project-URL: Bug Tracker, https://github.com/onera/acetone/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: C
@@ -95,30 +95,30 @@
   * The name of the function to generate (here 'lenet5')
   * The number of test to run (here 1)
   * The algorithm used for the convolution layer ('6loops','indirect_gemm_'+TYPE, 'std_gemm_'+TYPE, with TYPE being amongst 'nn','nt',    'tn','tt')
   * The directory in which the code will be generated
   * The input file with the test data
 
 ```
-cli-acetone tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_example/lenet5.h5  lenet5 1 std_gemm_nn tests/models/lenet5/lenet5_example/lenet5_generated tests/models/lenet5/lenet5_example/test_input_lenet5.txt
 ```
 
 * Compile the code
 ```
 make -C tests/models/lenet5/lenet5_example/lenet5_generated all
 ```
 
 * Execute the file with the path to the directory of the output file as argument
 ```
 ./tests/models/lenet5/lenet5_example/lenet5_generated/lenet5 ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt
 ```
 
 * Compare the output given by Keras and ACETONE
 ```
-cli_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
+acetone_compare ./tests/models/lenet5/lenet5_example/output_keras.txt ./tests/models/lenet5/lenet5_example/lenet5_generated/output_acetone.txt 1
 ```
 
 ## Tests
 
 Tests are implemented in the folder *tests*.
 
 To run them, use the `run_tests.py` script from the `tests/` folder.
@@ -140,27 +140,27 @@
 
 ## Reproduce the paper's experiments
 
 To reproduce the result of semantic experiment with ACETONE as described in the paper, use the following commands:
 
 * For the acas_decr128 model
 ```
-cli-acetone tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
+acetone_generate tests/models/acas/acas_decr128/acas_decr128.json acas_dcre128 1000 std_gemm_nn tests/models/acas/acas_decr128/output_acetone tests/models/acas/acas_decr128/test_input_acas_decr128.txt
 make -C tests/models/acas/acas_decr128/output_acetone all
 ./tests/models/acas/acas_decr128/output_acetone/acas_decr128 tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
-cli_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
+acetone_compare tests/models/acas/acas_decr128/output_keras.txt tests/models/acas/acas_decr128/output_acetone/output_acetone.txt
 ```
 
 * For the lent5 model
 
 ```
-cli-acetone tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
+acetone_generate tests/models/lenet5/lenet5_trained/lenet5_trained.json lenet5_trained 1000 std_gemm_nn tests/models/lenet5/lenet5_trained/output_acetone tests/models/lenet5_trained/test_input_lenet5.txt
 make -C tests/models/lenet5/lenet5_trained/output_acetone all
 ./tests/models/lenet5/lenet5_trained/output_acetone/lenet5_trained tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
-cli_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
+acetone_compare tests/models/lenet5/lenet5_trained/output_keras.txt tests/models/lenet5/lenet5_trained/output_acetone/output_acetone.txt
 ```
 
 ## Capability
 
 As of the 26/03/2024, the framework can generate code for neural network meeting the following condition:
 
 * The neural network is Sequential and Feedforward
```

### Comparing `acetone_nnet-0.2/src/acetone_nnet.egg-info/SOURCES.txt` & `acetone_nnet-0.2.1/src/acetone_nnet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

